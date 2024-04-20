# Comparing `tmp/fastapi_sqlmodel_starter-1.0.0b1.tar.gz` & `tmp/fastapi_sqlmodel_starter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sqlmodel_starter-1.0.0b1.tar", max compression
+gzip compressed data, was "fastapi_sqlmodel_starter-1.0.1.tar", max compression
```

## Comparing `fastapi_sqlmodel_starter-1.0.0b1.tar` & `fastapi_sqlmodel_starter-1.0.1.tar`

### file list

```diff
@@ -1,264 +1,164 @@
--rw-r--r--   0        0        0     1085 2024-04-12 11:51:13.244253 fastapi_sqlmodel_starter-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     2196 2024-04-13 07:51:59.629874 fastapi_sqlmodel_starter-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2715 2024-04-13 07:58:31.878911 fastapi_sqlmodel_starter-1.0.0b1/README.md
--rw-r--r--   0        0        0    69632 2024-04-13 07:26:42.863114 fastapi_sqlmodel_starter-1.0.0b1/src/.coverage
--rw-r--r--   0        0        0      940 2024-04-13 06:18:35.281365 fastapi_sqlmodel_starter-1.0.0b1/src/.env.example
--rw-r--r--   0        0        0     3811 2024-04-12 11:51:13.253984 fastapi_sqlmodel_starter-1.0.0b1/src/alembic.ini
--rw-r--r--   0        0        0      736 2024-04-12 11:51:13.253984 fastapi_sqlmodel_starter-1.0.0b1/src/Dockerfile
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.254962 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__init__.py
--rw-r--r--   0        0        0      178 2024-04-12 13:52:27.167753 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      108 2024-04-12 11:52:25.137476 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      109 2024-04-12 11:51:13.254962 fastapi_sqlmodel_starter-1.0.0b1/src/fss/apiserver.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.255934 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__init__.py
--rw-r--r--   0        0        0      185 2024-04-12 13:52:27.168727 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      115 2024-04-12 11:52:25.150129 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4230 2024-04-12 13:52:27.169713 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     2468 2024-04-12 13:52:05.648727 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.256904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__init__.py
--rw-r--r--   0        0        0      191 2024-04-12 13:52:27.843248 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      173 2024-04-12 13:52:06.327106 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2113 2024-04-12 13:52:27.844221 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/cache.cpython-311.pyc
--rw-r--r--   0        0        0     1583 2024-04-12 13:52:06.333920 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/cache.cpython-38.pyc
--rw-r--r--   0        0        0     2237 2024-04-12 13:52:29.604173 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc
--rw-r--r--   0        0        0     1528 2024-04-12 13:52:08.023657 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-38.pyc
--rw-r--r--   0        0        0     1078 2024-04-12 11:51:13.256904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/cache.py
--rw-r--r--   0        0        0      994 2024-04-12 11:51:13.257880 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/page_cache.py
--rw-r--r--   0        0        0     1682 2024-04-12 11:51:13.258850 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/redis_cache.py
--rw-r--r--   0        0        0     1926 2024-04-12 11:51:13.258850 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/config.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.259824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__init__.py
--rw-r--r--   0        0        0      190 2024-04-12 13:52:27.845194 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-04-12 13:52:06.334904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1316 2024-04-12 13:52:27.846168 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-311.pyc
--rw-r--r--   0        0        0     1012 2024-04-12 13:52:06.341709 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-38.pyc
--rw-r--r--   0        0        0      481 2024-04-12 11:51:13.259824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/enum.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.260797 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__init__.py
--rw-r--r--   0        0        0      195 2024-04-12 13:52:27.572672 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      177 2024-04-12 13:52:06.013718 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1050 2024-04-12 13:52:27.573635 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-311.pyc
--rw-r--r--   0        0        0      812 2024-04-12 13:52:06.020546 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-38.pyc
--rw-r--r--   0        0        0      428 2024-04-12 11:51:13.260797 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/exception.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.261771 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__init__.py
--rw-r--r--   0        0        0      197 2024-04-12 13:52:27.855900 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      127 2024-04-12 11:52:25.152076 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4875 2024-04-12 13:52:27.856884 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2024-04-12 13:52:06.372865 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     1732 2024-04-12 13:52:27.960133 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc
--rw-r--r--   0        0        0     1184 2024-04-12 11:52:25.154022 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-38.pyc
--rw-r--r--   0        0        0      510 2024-04-12 13:52:27.857847 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/mapper.cpython-311.pyc
--rw-r--r--   0        0        0      402 2024-04-12 13:52:06.378696 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/mapper.cpython-38.pyc
--rw-r--r--   0        0        0    13268 2024-04-13 06:05:45.222433 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc
--rw-r--r--   0        0        0     6828 2024-04-12 13:52:06.464346 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-38.pyc
--rw-r--r--   0        0        0     2521 2024-04-12 11:51:13.262744 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_mapper.py
--rw-r--r--   0        0        0      814 2024-04-12 11:51:13.263724 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_model.py
--rw-r--r--   0        0        0       80 2024-04-12 11:51:13.264696 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/mapper.py
--rw-r--r--   0        0        0     7039 2024-04-13 05:57:14.379609 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/sqlmodel_impl.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__init__.py
--rw-r--r--   0        0        0      192 2024-04-12 13:52:27.977642 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      174 2024-04-12 13:52:06.529601 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3889 2024-04-12 13:52:27.979614 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/result.cpython-311.pyc
--rw-r--r--   0        0        0     2493 2024-04-12 13:52:06.539331 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/result.cpython-38.pyc
--rw-r--r--   0        0        0     2016 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/result.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__init__.py
--rw-r--r--   0        0        0      192 2024-04-12 13:52:27.848126 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      174 2024-04-12 13:52:06.342681 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1133 2024-04-12 13:52:27.849098 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/schema.cpython-311.pyc
--rw-r--r--   0        0        0      796 2024-04-12 13:52:06.349494 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/schema.cpython-38.pyc
--rw-r--r--   0        0        0      315 2024-04-12 11:51:13.266637 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/schema.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.266637 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__init__.py
--rw-r--r--   0        0        0      194 2024-04-12 13:52:27.989249 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      176 2024-04-12 13:52:06.549108 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2156 2024-04-12 13:52:27.990300 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/security.cpython-311.pyc
--rw-r--r--   0        0        0     1482 2024-04-12 13:52:06.556889 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/security.cpython-38.pyc
--rw-r--r--   0        0        0     1305 2024-04-12 11:51:13.267622 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/security.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.267622 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__init__.py
--rw-r--r--   0        0        0      193 2024-04-12 13:52:27.852017 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      175 2024-04-12 13:52:06.354361 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4490 2024-04-12 13:52:27.859794 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/service.cpython-311.pyc
--rw-r--r--   0        0        0     3214 2024-04-12 13:52:06.385508 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/service.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.268660 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__init__.py
--rw-r--r--   0        0        0      198 2024-04-12 13:52:27.852981 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      180 2024-04-12 13:52:06.356306 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6783 2024-04-12 13:52:27.854937 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc
--rw-r--r--   0        0        0     4105 2024-04-12 13:52:06.365069 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-38.pyc
--rw-r--r--   0        0        0     2850 2024-04-12 13:07:40.882205 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/service_impl.py
--rw-r--r--   0        0        0     2052 2024-04-12 11:51:13.269251 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/service.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.270148 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__init__.py
--rw-r--r--   0        0        0      190 2024-04-12 13:52:27.574608 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      120 2024-04-12 11:52:25.156943 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3360 2024-04-12 14:08:26.649563 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/security.cpython-311.pyc
--rw-r--r--   0        0        0     1889 2024-04-12 13:52:06.029300 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/security.cpython-38.pyc
--rw-r--r--   0        0        0     2450 2024-04-12 13:52:27.961021 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/snowflake.cpython-311.pyc
--rw-r--r--   0        0        0     1503 2024-04-12 11:52:25.159862 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/snowflake.cpython-38.pyc
--rw-r--r--   0        0        0     1291 2024-04-13 07:46:45.486153 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/excel.py
--rw-r--r--   0        0        0     1634 2024-04-12 14:08:19.414967 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/security.py
--rw-r--r--   0        0        0     1580 2024-04-12 11:51:13.271119 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/snowflake.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.271119 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__init__.py
--rw-r--r--   0        0        0      189 2024-04-12 13:52:27.743976 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      171 2024-04-12 13:52:06.208653 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8242 2024-04-12 13:52:27.745923 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc
--rw-r--r--   0        0        0     5230 2024-04-12 13:52:06.216440 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-38.pyc
--rw-r--r--   0        0        0     4684 2024-04-12 11:51:13.272093 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/db_session_middleware.py
--rw-r--r--   0        0        0      221 2024-04-12 11:51:13.273070 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__init__.py
--rw-r--r--   0        0        0      707 2024-04-12 13:52:27.243673 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      361 2024-04-12 11:52:25.139422 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8875 2024-04-12 13:52:27.245629 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/server.cpython-311.pyc
--rw-r--r--   0        0        0     5191 2024-04-12 13:52:05.724720 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     5977 2024-04-12 11:51:13.273070 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/server.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.274042 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__init__.py
--rw-r--r--   0        0        0      193 2024-04-12 13:52:27.830596 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      123 2024-04-12 11:52:25.141368 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.274042 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__init__.py
--rw-r--r--   0        0        0      197 2024-04-12 13:52:27.833516 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      179 2024-04-12 13:52:06.299854 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.275013 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__init__.py
--rw-r--r--   0        0        0      200 2024-04-12 13:52:27.834489 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-04-12 13:52:06.301799 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1987 2024-04-12 13:52:27.836467 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc
--rw-r--r--   0        0        0     1203 2024-04-12 13:52:06.308614 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-38.pyc
--rw-r--r--   0        0        0     6254 2024-04-13 06:38:33.855758 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/user_controller.cpython-311.pyc
--rw-r--r--   0        0        0     2516 2024-04-12 13:52:06.528586 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/user_controller.cpython-38.pyc
--rw-r--r--   0        0        0      981 2024-04-12 11:51:13.275013 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/probe_controller.py
--rw-r--r--   0        0        0     3453 2024-04-13 06:38:25.879538 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/user_controller.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.275986 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__init__.py
--rw-r--r--   0        0        0      198 2024-04-12 13:52:27.838380 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      180 2024-04-12 13:52:06.309586 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1331 2024-04-12 13:52:27.839432 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0     1057 2024-04-12 13:52:06.315439 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/system.cpython-38.pyc
--rw-r--r--   0        0        0      501 2024-04-12 11:51:13.276964 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/system.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.276964 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__init__.py
--rw-r--r--   0        0        0      203 2024-04-12 13:52:27.860777 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-04-12 13:52:06.386482 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1136 2024-04-12 13:52:27.861751 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0      778 2024-04-12 13:52:06.393294 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-38.pyc
--rw-r--r--   0        0        0      358 2024-04-12 11:51:13.277933 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/system.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.277933 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__init__.py
--rw-r--r--   0        0        0      200 2024-04-12 13:52:27.862724 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-04-12 13:52:06.394277 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2005 2024-04-12 13:52:27.863697 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc
--rw-r--r--   0        0        0     1419 2024-04-12 13:52:06.401081 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2024-04-12 11:51:13.278906 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/user_mapper.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.279881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__init__.py
--rw-r--r--   0        0        0      199 2024-04-12 13:52:27.947394 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2024-04-12 11:52:25.143317 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-04-12 13:54:19.806764 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/migrate.cpython-311.pyc
--rw-r--r--   0        0        0      311 2024-04-12 11:52:25.145262 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/migrate.cpython-38.pyc
--rw-r--r--   0        0        0     1772 2024-04-12 13:52:27.954298 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc
--rw-r--r--   0        0        0     1127 2024-04-12 11:52:25.148187 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-38.pyc
--rw-r--r--   0        0        0      168 2024-04-12 11:51:13.279881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/migrate.py
--rw-r--r--   0        0        0      728 2024-04-12 11:51:13.280857 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/user_do.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.280857 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__init__.py
--rw-r--r--   0        0        0      200 2024-04-12 13:52:27.831568 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-04-12 13:52:06.293040 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      751 2024-04-12 13:52:27.832542 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0      542 2024-04-12 13:52:06.298881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-38.pyc
--rw-r--r--   0        0        0      376 2024-04-12 11:51:13.281826 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/system.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.281826 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__init__.py
--rw-r--r--   0        0        0      200 2024-04-12 13:52:27.970761 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-04-12 13:52:06.505301 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1845 2024-04-13 06:05:45.237824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc
--rw-r--r--   0        0        0     1160 2024-04-12 13:52:06.512086 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/user_schema.cpython-38.pyc
--rw-r--r--   0        0        0      627 2024-04-13 07:46:45.274124 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/user_schema.py
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.282800 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__init__.py
--rw-r--r--   0        0        0      201 2024-04-12 13:52:27.840338 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      183 2024-04-12 13:52:06.316411 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2279 2024-04-13 06:05:45.242830 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/user_service.cpython-311.pyc
--rw-r--r--   0        0        0     1083 2024-04-12 13:52:06.520875 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/user_service.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.283776 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__init__.py
--rw-r--r--   0        0        0      206 2024-04-12 13:52:27.841301 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      188 2024-04-12 13:52:06.317373 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    11050 2024-04-13 06:34:47.200390 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc
--rw-r--r--   0        0        0     3117 2024-04-12 13:52:06.325169 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-38.pyc
--rw-r--r--   0        0        0     4621 2024-04-13 07:46:45.486153 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/user_service_impl.py
--rw-r--r--   0        0        0     1017 2024-04-13 05:25:39.587003 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/user_service.py
--rw-r--r--   0        0        0       29 2024-04-12 14:20:41.845120 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/.gitignore
--rw-r--r--   0        0        0    22489 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.761504 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876___init___py.html
--rw-r--r--   0        0        0    12152 2024-04-12 14:20:41.764406 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876_user_do_py.html
--rw-r--r--   0        0        0     4524 2024-04-12 14:20:41.672841 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3___init___py.html
--rw-r--r--   0        0        0    26048 2024-04-12 14:20:41.678768 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3_result_py.html
--rw-r--r--   0        0        0     4508 2024-04-12 14:20:41.786793 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_160d2543108c5886___init___py.html
--rw-r--r--   0        0        0     4510 2024-04-12 14:20:41.625246 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a___init___py.html
--rw-r--r--   0        0        0    14792 2024-04-12 14:20:41.628143 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_cache_py.html
--rw-r--r--   0        0        0    14113 2024-04-12 14:20:41.631060 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_page_cache_py.html
--rw-r--r--   0        0        0     4528 2024-04-12 14:20:41.736180 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_204be9a6e4696b99___init___py.html
--rw-r--r--   0        0        0     4504 2024-04-12 14:20:41.622306 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6___init___py.html
--rw-r--r--   0        0        0    25319 2024-04-12 14:20:41.636902 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6_config_py.html
--rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.642752 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d___init___py.html
--rw-r--r--   0        0        0     8329 2024-04-12 14:20:41.644686 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d_exception_py.html
--rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.683621 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f___init___py.html
--rw-r--r--   0        0        0    14975 2024-04-12 14:20:41.686540 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f_security_py.html
--rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.787787 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0___init___py.html
--rw-r--r--   0        0        0     9732 2024-04-12 14:20:41.790689 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_probe_test_py.html
--rw-r--r--   0        0        0    39415 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_user_test_py.html
--rw-r--r--   0        0        0     4512 2024-04-12 14:20:41.703108 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0___init___py.html
--rw-r--r--   0        0        0    20691 2024-04-12 14:20:41.707959 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_security_py.html
--rw-r--r--   0        0        0    20821 2024-04-12 14:20:41.712826 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_snowflake_py.html
--rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.756622 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9___init___py.html
--rw-r--r--   0        0        0    13167 2024-04-12 14:20:41.759543 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9_user_mapper_py.html
--rw-r--r--   0        0        0     7078 2024-04-12 14:20:41.723529 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e___init___py.html
--rw-r--r--   0        0        0    51456 2024-04-12 14:20:41.733260 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e_server_py.html
--rw-r--r--   0        0        0     4540 2024-04-12 14:20:41.747861 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036___init___py.html
--rw-r--r--   0        0        0    10098 2024-04-12 14:20:41.750787 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036_system_py.html
--rw-r--r--   0        0        0     4516 2024-04-12 14:20:41.735209 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_5d95fe6a529b7852___init___py.html
--rw-r--r--   0        0        0     4520 2024-04-12 14:20:41.688491 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983___init___py.html
--rw-r--r--   0        0        0    25667 2024-04-12 14:20:41.702121 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983_service_py.html
--rw-r--r--   0        0        0     4440 2024-04-12 14:20:41.620356 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_794d731f07d9e36c___init___py.html
--rw-r--r--   0        0        0     4502 2024-04-12 14:20:41.638849 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec___init___py.html
--rw-r--r--   0        0        0    10386 2024-04-12 14:20:41.640798 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec_enum_py.html
--rw-r--r--   0        0        0     4510 2024-04-12 14:20:41.679727 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a___init___py.html
--rw-r--r--   0        0        0     8101 2024-04-12 14:20:41.681673 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a_schema_py.html
--rw-r--r--   0        0        0     4538 2024-04-12 14:20:41.689472 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a___init___py.html
--rw-r--r--   0        0        0    33428 2024-04-13 07:26:53.842997 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a_service_impl_py.html
--rw-r--r--   0        0        0     4550 2024-04-12 14:20:41.738132 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8___init___py.html
--rw-r--r--   0        0        0    13961 2024-04-12 14:20:41.741050 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_probe_controller_py.html
--rw-r--r--   0        0        0    38279 2024-04-13 07:26:53.863012 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_user_controller_py.html
--rw-r--r--   0        0        0     4502 2024-04-12 14:20:41.784846 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     4532 2024-04-12 14:20:41.752728 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014___init___py.html
--rw-r--r--   0        0        0     8287 2024-04-12 14:20:41.754673 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014_system_py.html
--rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.645660 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695___init___py.html
--rw-r--r--   0        0        0    30040 2024-04-12 14:20:41.651500 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_mapper_py.html
--rw-r--r--   0        0        0    12529 2024-04-12 14:20:41.654432 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_model_py.html
--rw-r--r--   0        0        0     5790 2024-04-12 14:20:41.656368 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_mapper_py.html
--rw-r--r--   0        0        0    71690 2024-04-13 07:26:53.832931 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_sqlmodel_impl_py.html
--rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.769282 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dab9b2a1903716f2___init___py.html
--rw-r--r--   0        0        0    13862 2024-04-13 07:26:53.888210 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dab9b2a1903716f2_user_schema_py.html
--rw-r--r--   0        0        0     4540 2024-04-12 14:20:41.714770 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76___init___py.html
--rw-r--r--   0        0        0    39917 2024-04-12 14:20:41.721582 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76_db_session_middleware_py.html
--rw-r--r--   0        0        0     4528 2024-04-12 14:20:41.765384 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660___init___py.html
--rw-r--r--   0        0        0     7878 2024-04-12 14:20:41.768312 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660_system_py.html
--rw-r--r--   0        0        0     4564 2024-04-12 14:20:41.775113 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_f83affef05b47916___init___py.html
--rw-r--r--   0        0        0    53392 2024-04-13 07:26:53.903255 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_f83affef05b47916_user_service_impl_py.html
--rw-r--r--   0        0        0     4542 2024-04-12 14:20:41.773182 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269___init___py.html
--rw-r--r--   0        0        0    13819 2024-04-13 07:26:53.905298 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269_user_service_py.html
--rw-r--r--   0        0        0     1732 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    22048 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_open.png
--rw-r--r--   0        0        0    13435 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/status.json
--rw-r--r--   0        0        0    12703 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/style.css
--rw-r--r--   0        0        0     4552 2024-04-12 13:54:19.599443 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0     2408 2024-04-12 11:52:24.738430 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-38.pyc
--rw-r--r--   0        0        0    28672 2024-04-13 07:42:12.020194 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/db/fss.db
--rw-r--r--   0        0        0       15 2024-04-12 11:51:13.288642 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/db/README
--rw-r--r--   0        0        0     2714 2024-04-12 11:51:13.288642 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/env.py
--rw-r--r--   0        0        0       39 2024-04-12 11:51:13.286695 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/README
--rw-r--r--   0        0        0      577 2024-04-12 11:51:13.289618 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/script.py.mako
--rw-r--r--   0        0        0     1516 2024-04-12 11:51:13.291565 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/947dad7dbfdb_init_project.py
--rw-r--r--   0        0        0     2495 2024-04-12 13:54:19.861271 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc
--rw-r--r--   0        0        0     1342 2024-04-12 11:52:25.233119 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.291565 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__init__.py
--rw-r--r--   0        0        0      180 2024-04-12 13:52:26.321928 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      162 2024-04-12 13:52:04.950923 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.292551 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__init__.py
--rw-r--r--   0        0        0      187 2024-04-12 13:52:26.322901 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      169 2024-04-12 13:52:04.951811 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2024-04-12 11:51:13.292551 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__init__.py
--rw-r--r--   0        0        0      190 2024-04-12 13:52:26.323873 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-04-12 13:52:04.952785 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4373 2024-04-12 13:52:26.327768 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     2009 2024-04-12 13:52:04.962595 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/probe_test.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0        0        0    16631 2024-04-13 07:25:55.722716 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/user_test.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     5051 2024-04-12 13:52:06.605481 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/user_test.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      527 2024-04-12 11:51:13.293506 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/probe_test.py
--rw-r--r--   0        0        0     3833 2024-04-13 07:24:44.674018 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/user_test.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 fastapi_sqlmodel_starter-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-20 04:56:22.280207 fastapi_sqlmodel_starter-1.0.1/fss/.env.example
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/__init__.py
+-rw-r--r--   0        0        0     3811 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/alembic.ini
+-rw-r--r--   0        0        0      109 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/apiserver.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/common/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-20 06:01:48.844437 fastapi_sqlmodel_starter-1.0.1/fss/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3671 2024-04-20 15:29:32.605734 fastapi_sqlmodel_starter-1.0.1/fss/common/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-20 06:01:49.781479 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2302 2024-04-20 06:01:49.781479 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     2233 2024-04-20 06:14:27.989605 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/page_cache.cpython-311.pyc
+-rw-r--r--   0        0        0     2140 2024-04-20 06:14:27.989605 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/redis_cache.cpython-311.pyc
+-rw-r--r--   0        0        0     2193 2024-04-20 06:01:49.781479 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/redis_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     1137 2024-04-19 12:42:42.854799 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/cache.py
+-rw-r--r--   0        0        0      994 2024-04-18 14:46:02.664929 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/page_cache.py
+-rw-r--r--   0        0        0      882 2024-04-19 13:40:21.381061 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/redis_cache.py
+-rw-r--r--   0        0        0      959 2024-04-19 13:40:21.382035 fastapi_sqlmodel_starter-1.0.1/fss/common/cache/redis_manager.py
+-rw-r--r--   0        0        0     1756 2024-04-20 15:25:44.176883 fastapi_sqlmodel_starter-1.0.1/fss/common/config.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/enum/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-20 06:01:50.282032 fastapi_sqlmodel_starter-1.0.1/fss/common/enum/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1295 2024-04-20 06:01:50.282032 fastapi_sqlmodel_starter-1.0.1/fss/common/enum/__pycache__/enum.cpython-311.pyc
+-rw-r--r--   0        0        0      464 2024-04-19 13:07:28.857098 fastapi_sqlmodel_starter-1.0.1/fss/common/enum/enum.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-20 06:01:48.844437 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1031 2024-04-20 06:01:49.313634 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/__pycache__/exception.cpython-311.pyc
+-rw-r--r--   0        0        0     3250 2024-04-20 06:01:48.844437 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/__pycache__/exception_handler.cpython-311.pyc
+-rw-r--r--   0        0        0      413 2024-04-19 13:07:28.846521 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/exception.py
+-rw-r--r--   0        0        0     2323 2024-04-19 12:20:10.659027 fastapi_sqlmodel_starter-1.0.1/fss/common/exception/exception_handler.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-20 06:01:50.375823 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3762 2024-04-20 06:01:50.375823 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0     1728 2024-04-20 06:01:50.469760 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/base_model.cpython-311.pyc
+-rw-r--r--   0        0        0    16261 2024-04-20 15:29:33.373946 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     1644 2024-04-19 15:51:44.642121 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/base_mapper.py
+-rw-r--r--   0        0        0      814 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/base_model.py
+-rw-r--r--   0        0        0     9921 2024-04-20 15:22:48.656668 fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/sqlmodel_impl.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/result/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-20 06:01:50.501012 fastapi_sqlmodel_starter-1.0.1/fss/common/result/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1647 2024-04-20 12:16:47.828292 fastapi_sqlmodel_starter-1.0.1/fss/common/result/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0      714 2024-04-20 12:09:21.079798 fastapi_sqlmodel_starter-1.0.1/fss/common/result/result.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/schema/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-20 06:01:50.282032 fastapi_sqlmodel_starter-1.0.1/fss/common/schema/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1050 2024-04-20 06:01:50.282032 fastapi_sqlmodel_starter-1.0.1/fss/common/schema/__pycache__/schema.cpython-311.pyc
+-rw-r--r--   0        0        0      309 2024-04-19 13:40:21.382035 fastapi_sqlmodel_starter-1.0.1/fss/common/schema/schema.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/security/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-20 06:01:50.297574 fastapi_sqlmodel_starter-1.0.1/fss/common/security/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5246 2024-04-20 15:20:30.343920 fastapi_sqlmodel_starter-1.0.1/fss/common/security/__pycache__/security.cpython-311.pyc
+-rw-r--r--   0        0        0     2912 2024-04-20 15:19:36.724188 fastapi_sqlmodel_starter-1.0.1/fss/common/security/security.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/service/__init__.py
+-rw-r--r--   0        0        0      189 2024-04-20 06:01:50.375823 fastapi_sqlmodel_starter-1.0.1/fss/common/service/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3535 2024-04-20 12:16:47.801474 fastapi_sqlmodel_starter-1.0.1/fss/common/service/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/service/impl/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-20 06:01:50.375823 fastapi_sqlmodel_starter-1.0.1/fss/common/service/impl/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6437 2024-04-20 15:29:33.358403 fastapi_sqlmodel_starter-1.0.1/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     3097 2024-04-20 15:29:14.203717 fastapi_sqlmodel_starter-1.0.1/fss/common/service/impl/service_impl.py
+-rw-r--r--   0        0        0     1296 2024-04-20 12:16:39.973255 fastapi_sqlmodel_starter-1.0.1/fss/common/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/common/util/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-20 06:01:50.391452 fastapi_sqlmodel_starter-1.0.1/fss/common/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2578 2024-04-20 06:01:50.391452 fastapi_sqlmodel_starter-1.0.1/fss/common/util/__pycache__/excel.cpython-311.pyc
+-rw-r--r--   0        0        0     2562 2024-04-20 06:01:50.469760 fastapi_sqlmodel_starter-1.0.1/fss/common/util/__pycache__/snowflake.cpython-311.pyc
+-rw-r--r--   0        0        0     1289 2024-04-20 01:18:54.401028 fastapi_sqlmodel_starter-1.0.1/fss/common/util/excel.py
+-rw-r--r--   0        0        0     1820 2024-04-19 13:36:06.157993 fastapi_sqlmodel_starter-1.0.1/fss/common/util/snowflake.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/middleware/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-20 06:01:49.456018 fastapi_sqlmodel_starter-1.0.1/fss/middleware/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8582 2024-04-20 06:01:49.459982 fastapi_sqlmodel_starter-1.0.1/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc
+-rw-r--r--   0        0        0     1376 2024-04-20 06:01:49.703433 fastapi_sqlmodel_starter-1.0.1/fss/middleware/__pycache__/ip_block_middleware.cpython-311.pyc
+-rw-r--r--   0        0        0     1077 2024-04-20 06:01:49.703433 fastapi_sqlmodel_starter-1.0.1/fss/middleware/__pycache__/rate_limit_middleware.cpython-311.pyc
+-rw-r--r--   0        0        0     4942 2024-04-19 08:36:52.438194 fastapi_sqlmodel_starter-1.0.1/fss/middleware/db_session_middleware.py
+-rw-r--r--   0        0        0      806 2024-04-20 01:04:24.451367 fastapi_sqlmodel_starter-1.0.1/fss/middleware/ip_block_middleware.py
+-rw-r--r--   0        0        0     1661 2024-04-19 13:40:15.970411 fastapi_sqlmodel_starter-1.0.1/fss/middleware/jwt_middleware.py
+-rw-r--r--   0        0        0      655 2024-04-20 01:06:23.366365 fastapi_sqlmodel_starter-1.0.1/fss/middleware/rate_limit_middleware.py
+-rw-r--r--   0        0        0     4552 2024-04-20 06:14:22.051661 fastapi_sqlmodel_starter-1.0.1/fss/migrations/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0       15 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/migrations/db/README
+-rw-r--r--   0        0        0     2714 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/migrations/env.py
+-rw-r--r--   0        0        0       39 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/migrations/README
+-rw-r--r--   0        0        0      577 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/migrations/script.py.mako
+-rw-r--r--   0        0        0     1516 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/947dad7dbfdb_init_project.py
+-rw-r--r--   0        0        0     2495 2024-04-20 06:14:23.689472 fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc
+-rw-r--r--   0        0        0     3907 2024-04-20 14:46:46.285390 fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/__pycache__/aa3b6ded81f6_add_role_and_user_role_table.cpython-311.pyc
+-rw-r--r--   0        0        0     2481 2024-04-20 15:38:01.240347 fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/aa3b6ded81f6_add_role_and_user_role_table.py
+-rw-r--r--   0        0        0      503 2024-04-20 01:08:39.020459 fastapi_sqlmodel_starter-1.0.1/fss/starter/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-20 06:01:48.844437 fastapi_sqlmodel_starter-1.0.1/fss/starter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1950 2024-04-20 06:01:49.313634 fastapi_sqlmodel_starter-1.0.1/fss/starter/__pycache__/server.cpython-311.pyc
+-rw-r--r--   0        0        0      996 2024-04-19 12:37:23.572623 fastapi_sqlmodel_starter-1.0.1/fss/starter/server.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/__init__.py
+-rw-r--r--   0        0        0      189 2024-04-20 06:01:49.750227 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-20 06:01:49.765893 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-20 06:01:49.765893 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2883 2024-04-20 06:01:49.765893 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc
+-rw-r--r--   0        0        0     6031 2024-04-20 14:01:30.737248 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/__pycache__/role_controller.cpython-311.pyc
+-rw-r--r--   0        0        0    11475 2024-04-20 15:12:26.224999 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/__pycache__/user_controller.cpython-311.pyc
+-rw-r--r--   0        0        0     1689 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/probe_controller.py
+-rw-r--r--   0        0        0     3924 2024-04-20 12:43:50.923485 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/role_controller.py
+-rw-r--r--   0        0        0     7655 2024-04-20 15:11:23.597196 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/api/v1/user_controller.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/enum/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-20 06:01:49.828415 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/enum/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1842 2024-04-20 06:01:49.828415 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/enum/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0     1007 2024-04-19 15:18:21.191244 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/enum/system.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/exception/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-20 06:01:50.391452 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1165 2024-04-20 06:01:50.391452 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/exception/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0      382 2024-04-19 15:51:44.642121 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/exception/system.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-20 06:01:50.391452 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      702 2024-04-20 06:01:50.610447 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__pycache__/role_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0     2874 2024-04-20 06:01:50.407077 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0      728 2024-04-20 06:01:50.516664 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__pycache__/user_role_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0      232 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/role_mapper.py
+-rw-r--r--   0        0        0     1476 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/user_mapper.py
+-rw-r--r--   0        0        0      265 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/user_role_mapper.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.680559 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-20 06:01:50.469760 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      563 2024-04-20 06:14:23.658227 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/migrate.cpython-311.pyc
+-rw-r--r--   0        0        0     1703 2024-04-20 06:01:50.610447 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/role_do.cpython-311.pyc
+-rw-r--r--   0        0        0     1768 2024-04-20 06:01:50.469760 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc
+-rw-r--r--   0        0        0     1609 2024-04-20 15:12:26.228921 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/user_role_do.cpython-311.pyc
+-rw-r--r--   0        0        0      297 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/migrate.py
+-rw-r--r--   0        0        0      664 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/role_do.py
+-rw-r--r--   0        0        0      728 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/user_do.py
+-rw-r--r--   0        0        0      697 2024-04-20 15:11:39.357036 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/user_role_do.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/router/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-20 06:01:49.750227 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/router/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2024-04-20 06:01:49.765893 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/router/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0      672 2024-04-19 12:20:10.679751 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/router/system.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-20 06:01:50.485427 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1130 2024-04-20 14:43:33.296260 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/__pycache__/role_schema.cpython-311.pyc
+-rw-r--r--   0        0        0     1869 2024-04-20 06:01:50.485427 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc
+-rw-r--r--   0        0        0      329 2024-04-20 14:03:30.170378 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/role_schema.py
+-rw-r--r--   0        0        0      627 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/user_schema.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-20 06:01:49.844493 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      701 2024-04-20 06:01:50.626033 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/__pycache__/role_service.cpython-311.pyc
+-rw-r--r--   0        0        0      724 2024-04-20 06:01:50.516664 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/__pycache__/user_role_service.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2024-04-20 06:01:50.485427 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/__pycache__/user_service.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-20 06:01:49.844493 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1898 2024-04-20 06:01:50.610447 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__pycache__/role_service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     1396 2024-04-20 06:01:50.516664 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__pycache__/user_role_service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0    11688 2024-04-20 15:29:32.826929 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0      969 2024-04-19 15:20:33.315517 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/role_service_impl.py
+-rw-r--r--   0        0        0      750 2024-04-19 15:51:44.642121 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/user_role_service_impl.py
+-rw-r--r--   0        0        0     7282 2024-04-20 15:26:01.395257 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/user_service_impl.py
+-rw-r--r--   0        0        0      209 2024-04-19 08:29:36.577319 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/role_service.py
+-rw-r--r--   0        0        0      230 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/user_role_service.py
+-rw-r--r--   0        0        0     1079 2024-04-19 15:51:44.714408 fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/user_service.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/tests/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-20 06:14:24.783462 fastapi_sqlmodel_starter-1.0.1/fss/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-20 06:14:24.783462 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-18 14:46:02.696174 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-20 06:14:24.783462 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3217 2024-04-20 14:49:02.183724 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0    16817 2024-04-20 14:49:03.616150 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/__pycache__/role_test.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0    28306 2024-04-20 15:20:35.034009 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/__pycache__/user_test.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      568 2024-04-20 14:03:30.171378 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/probe_test.py
+-rw-r--r--   0        0        0     4898 2024-04-20 14:03:30.171378 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/role_test.py
+-rw-r--r--   0        0        0     9380 2024-04-20 15:17:35.519888 fastapi_sqlmodel_starter-1.0.1/fss/tests/system/v1/user_test.py
+-rw-r--r--   0        0        0     1066 2024-04-20 03:01:56.133498 fastapi_sqlmodel_starter-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2579 2024-04-20 15:51:06.358883 fastapi_sqlmodel_starter-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3140 2024-04-20 08:55:30.786445 fastapi_sqlmodel_starter-1.0.1/README.md
+-rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 fastapi_sqlmodel_starter-1.0.1/PKG-INFO
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/LICENSE` & `fastapi_sqlmodel_starter-1.0.1/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 FastapiSqlmodelStarter group
+Copyright (c) 2024 Fss group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/pyproject.toml` & `fastapi_sqlmodel_starter-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core",
 ]
 
 [tool.poetry]
 name = "fastapi-sqlmodel-starter"
-version = "1.0.0-beta.1"
+version = "1.0.1"
 description = "Fss aims to be one of top scaffold in PyWeb."
 license = "MIT"
 authors = [
   "tyvekZhang <tyvekzhang@gmail.com>",
 ]
 maintainers = [
   "tyvekZhang <tyvekzhang@gmail.com>",
@@ -28,15 +28,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 packages = [
-  { include = "src"},
+  { include = "fss"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 loguru = "^0.7.2"
 fastapi = "^0.110.0"
 fastapi-pagination = "^0.12.21"
@@ -56,29 +56,44 @@
 aiomysql = "^0.2.0"
 redis = {extras = ["hiredis"], version = "^5.0.3"}
 eval-type-backport = "^0.1.3"
 diskcache = "^5.6.3"
 pandas = "^2.2.2"
 xlsxwriter = "^3.2.0"
 openpyxl = "^3.1.2"
+slowapi = "^0.1.9"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 httpx = "^0.27.0"
 coverage = "^7.4.4"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "*"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
 
 [tool.poetry.scripts]
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 priority = "primary"
 
 [tool.coverage.run]
 parallel = true
 branch = true
-source = ["src/fss", "src/tests"]
+source = ["fss/common", "fss/middleware", "fss/starter", "fss/tests"]
 
 [tool.coverage.report]
+fail_under = 85
 show_missing = true
+exclude_also = [
+    "def __repr__",
+    "if self.debug:",
+    "if settings.DEBUG",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "if 0:",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+    "class .*\\bProtocol\\):",
+    "@(abc\\.)?abstractmethod",
+    ]
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/README.md` & `fastapi_sqlmodel_starter-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div  align="center" style="margin-top: 3%">
    <h1>
-     FastAPI Sqlmodel Starter (Fss)
+     FastAPI SQLModel Starter (Fss)
    </h1>
    <p>
-     <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/logo.png" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
+     <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/source/_static/img/fss.svg" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
    </p>
    <p>
      <img alt="GitHub License" src="https://img.shields.io/github/license/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fastapi-sqlmodel-starter">
      <img alt="CI" src="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/actions/workflows/ci.yaml/badge.svg">
      <img alt="Codecov" src="https://img.shields.io/codecov/c/github/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="Read the Docs" src="https://img.shields.io/readthedocs/fastapi-sqlmodel-starter">
@@ -22,24 +22,40 @@
     PyWeb领域最好用的脚手架之一。
    </h3>
 </div>
 
 
 ## 特性
 
-- 开箱即用, 内置常见数据库、缓存([默认]Sqlite, PostgreSQL, MySQL, [默认]文件缓存, Redis)
-- 自带单表的几乎所有操作
-- 数据库迁移, 静态代码扫描, 接口文档等一众特性
+- ⚡ 开箱即用, 实现中间件的零依赖
+   - 默认使用Sqlite, 也可自由切换PostgreSQL、MySQL数据库
+   - 可选文件或Redis缓存
+- 🚢 开启Python代码操作数据库的新体验
+- 🚀 简化ORM操作, 内置单表常见操作
+- 🎨 丰富的插件机制
+   - Jwt安全认证
+   - 访问限流
+   - Ip黑名单
+- 🐋 完备的容器化解决方案
+  - Docker
+  - Docker-compose
+  - Kubernetes
+- ✅ 基于GitHub Actions的CI (持续集成) 和 CD (持续交付)
+
+## 文档
+- 交互式API文档
+  <img alt="API doc"  src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/api_doc.png">
+- 在线文档: [Read the docs](https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/)
 
 ## 快速开始
-1. 首先确保python的版本是3.9及以上的
+1. 首先确保python版本为3.9及以上
 2. 克隆代码
 ```shell
 git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter
-cd fastapi-sqlmodel-starter/src
+cd fastapi-sqlmodel-starter/fss
 ```
 3. [可选]创建虚拟环境, 本篇以venv为例, 类似的工具还有conda, virtualenv等
 ```shell
 python3 -m venv .env_fss
 ```
 4. [可选]激活虚拟环境
     - Windows: .env_fss\Scripts\activate
@@ -50,25 +66,24 @@
 poetry install
 ```
 6. 数据库迁移
 ```shell
 alembic upgrade head
 ```
 7. 启动
-   - Windows: python3 fss\apiserver.py
-   - macOS 或 Linux: python3 fss/apiserver.py
+   - Windows: python3 apiserver.py
+   - macOS 或 Linux: python3 apiserver.py
 8. 访问: http://127.0.0.1:9010/docs
-9. 首先通过注册接口新建用户, 接着进行认证, 一切Ok.
-## 文档
-- https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/
+> 成功访问后需要创建用户并认证
+
 ## 贡献
 
 欢迎为 FastapiSqlmodelStarter 做出贡献！你可以通过以下方式参与：
 
-- 提交 Bug 或功能需求到 [Issue 追踪器](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
+- 提交 Bug 或功能需求到 [Issue清单](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
 - 提交代码改进的 Pull Request
 - 编写和改进文档
 - 分享你使用 FastapiSqlmodelStarter 的经验和想法
 
 ## 许可证
 
 FastapiSqlmodelStarter 采用 [MIT 许可证](https://opensource.org/licenses/MIT)开源。
```

#### html2text {}

```diff
@@ -1,28 +1,32 @@
-                 ************ FFaassttAAPPII SSqqllmmooddeell SSttaarrtteerr ((FFssss)) ************
+                 ************ FFaassttAAPPII SSQQLLMMooddeell SSttaarrtteerr ((FFssss)) ************
                                     [logo]
       [GitHub License][PyPI - Python Version][CI][Codecov][Read the Docs]
                         ****** ?ç?®??ä?½??ä?¸?­?æ?? || _EE_nn_gg_ll_ii_ss_hh ******
               ******** PPyyWWeebb?é?¢??å???æ???å?¥?½?ç??¨?ç???è???æ???æ??¶?ä?¹??ä?¸??ã?? ********
-## ç¹æ§ - å¼ç®±å³ç¨, åç½®å¸¸è§æ°æ®åºãç¼å­([é»è®¤]Sqlite,
-PostgreSQL, MySQL, [é»è®¤]æä»¶ç¼å­, Redis) -
-èªå¸¦åè¡¨çå ä¹æææä½ - æ°æ®åºè¿ç§», éæä»£ç æ«æ,
-æ¥å£ææ¡£ç­ä¸ä¼ç¹æ§ ## å¿«éå¼å§ 1.
-é¦åç¡®ä¿pythonççæ¬æ¯3.9åä»¥ä¸ç 2. åéä»£ç  ```shell git
-clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd fastapi-
-sqlmodel-starter/src ``` 3. [å¯é]åå»ºèæç¯å¢, æ¬ç¯ä»¥venvä¸ºä¾,
-ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3 -m venv .env_fss ```
-4. [å¯é]æ¿æ´»èæç¯å¢ - Windows: .env_fss\Scripts\activate - macOS æ
-Linux: source .env_fss/bin/activate 5. å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell
-pip install poetry --trusted-host=mirrors.tuna.tsinghua.edu.cn --index-
-url=https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
+## ç¹æ§ - â¡ å¼ç®±å³ç¨, å®ç°ä¸­é´ä»¶çé¶ä¾èµ - é»è®¤ä½¿ç¨Sqlite,
+ä¹å¯èªç±åæ¢PostgreSQLãMySQLæ°æ®åº - å¯éæä»¶æRedisç¼å­ -
+ð¢ å¼å¯Pythonä»£ç æä½æ°æ®åºçæ°ä½éª - ð ç®åORMæä½,
+åç½®åè¡¨å¸¸è§æä½ - ð¨ ä¸°å¯çæä»¶æºå¶ - Jwtå®å¨è®¤è¯ -
+è®¿é®éæµ - Ipé»åå - ð å®å¤çå®¹å¨åè§£å³æ¹æ¡ - Docker -
+Docker-compose - Kubernetes - â åºäºGitHub ActionsçCI (æç»­éæ) å
+CD (æç»­äº¤ä») ## ææ¡£ - äº¤äºå¼APIææ¡£ [API doc]- å¨çº¿ææ¡£: [Read
+the docs](https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/) ##
+å¿«éå¼å§ 1. é¦åç¡®ä¿pythonçæ¬ä¸º3.9åä»¥ä¸ 2. åéä»£ç 
+```shell git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd
+fastapi-sqlmodel-starter/fss ``` 3. [å¯é]åå»ºèæç¯å¢,
+æ¬ç¯ä»¥venvä¸ºä¾, ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3
+-m venv .env_fss ``` 4. [å¯é]æ¿æ´»èæç¯å¢ - Windows:
+.env_fss\Scripts\activate - macOS æ Linux: source .env_fss/bin/activate 5.
+å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell pip install poetry --trusted-
+host=mirrors.tuna.tsinghua.edu.cn --index-url=https://
+mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
 æ°æ®åºè¿ç§» ```shell alembic upgrade head ``` 7. å¯å¨ - Windows: python3
-fss\apiserver.py - macOS æ Linux: python3 fss/apiserver.py 8. è®¿é®: http://
-127.0.0.1:9010/docs 9. é¦åéè¿æ³¨åæ¥å£æ°å»ºç¨æ·,
-æ¥çè¿è¡è®¤è¯, ä¸åOk. ## ææ¡£ - https://fastapi-sqlmodel-
-starter.readthedocs.io/en/latest/ ## è´¡ç® æ¬¢è¿ä¸º FastapiSqlmodelStarter
+apiserver.py - macOS æ Linux: python3 apiserver.py 8. è®¿é®: http://
+127.0.0.1:9010/docs > æåè®¿é®åéè¦åå»ºç¨æ·å¹¶è®¤è¯ ## è´¡ç®
+æ¬¢è¿ä¸º FastapiSqlmodelStarter
 ååºè´¡ç®ï¼ä½ å¯ä»¥éè¿ä»¥ä¸æ¹å¼åä¸ï¼ - æäº¤ Bug
-æåè½éæ±å° [Issue è¿½è¸ªå¨](https://github.com/tyvekzhang/fastapi-
+æåè½éæ±å° [Issueæ¸å](https://github.com/tyvekzhang/fastapi-
 sqlmodel-starter/issues) - æäº¤ä»£ç æ¹è¿ç Pull Request -
 ç¼ååæ¹è¿ææ¡£ - åäº«ä½ ä½¿ç¨ FastapiSqlmodelStarter
 çç»éªåæ³æ³ ## è®¸å¯è¯ FastapiSqlmodelStarter éç¨ [MIT è®¸å¯è¯]
 (https://opensource.org/licenses/MIT)å¼æºã
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/alembic.ini` & `fastapi_sqlmodel_starter-1.0.1/fss/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/cache/__pycache__/page_cache.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
 files sz: 994
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -32,15 +32,15 @@
                 30 IMPORT_NAME              4 (fss.common.cache.cache)
                 32 IMPORT_FROM              5 (Cache)
                 34 STORE_NAME               5 (Cache)
                 36 POP_TOP
    
     10          38 PUSH_NULL
                 40 LOAD_BUILD_CLASS
-                42 LOAD_CONST               5 (<code object PageCache, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 10>)
+                42 LOAD_CONST               5 (<code object PageCache, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 10>)
                 44 MAKE_FUNCTION            0
                 46 LOAD_CONST               6 ('PageCache')
                 48 LOAD_NAME                5 (Cache)
                 50 PRECALL                  3
                 54 CALL                     3
                 64 STORE_NAME               6 (PageCache)
                 66 LOAD_CONST               3 (None)
@@ -63,56 +63,56 @@
             0b64055300
           10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PageCache')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               1 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 11>)
+          11          10 LOAD_CONST               1 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 11>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
           14          16 LOAD_CONST               2 ('key')
                       18 LOAD_NAME                4 (str)
                       20 LOAD_CONST               3 ('return')
                       22 LOAD_NAME                5 (Any)
                       24 BUILD_TUPLE              4
-                      26 LOAD_CONST               4 (<code object get, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 14>)
+                      26 LOAD_CONST               4 (<code object get, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 14>)
                       28 MAKE_FUNCTION            4 (annotations)
                       30 STORE_NAME               6 (get)
          
           18          32 LOAD_CONST              11 ((None,))
                       34 LOAD_CONST               2 ('key')
                       36 LOAD_NAME                4 (str)
                       38 LOAD_CONST               6 ('value')
                       40 LOAD_NAME                5 (Any)
                       42 LOAD_CONST               7 ('timeout')
                       44 LOAD_NAME                7 (int)
                       46 LOAD_CONST               3 ('return')
                       48 LOAD_CONST               5 (None)
                       50 BUILD_TUPLE              8
-                      52 LOAD_CONST               8 (<code object set, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 18>)
+                      52 LOAD_CONST               8 (<code object set, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 18>)
                       54 MAKE_FUNCTION            5 (defaults, annotations)
                       56 STORE_NAME               8 (set)
          
           24          58 LOAD_CONST               2 ('key')
                       60 LOAD_NAME                4 (str)
                       62 LOAD_CONST               3 ('return')
                       64 LOAD_NAME                9 (bool)
                       66 BUILD_TUPLE              4
-                      68 LOAD_CONST               9 (<code object delete, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 24>)
+                      68 LOAD_CONST               9 (<code object delete, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 24>)
                       70 MAKE_FUNCTION            4 (annotations)
                       72 STORE_NAME              10 (delete)
          
           31          74 LOAD_CONST               2 ('key')
                       76 LOAD_NAME                4 (str)
                       78 LOAD_CONST               3 ('return')
                       80 LOAD_NAME                9 (bool)
                       82 BUILD_TUPLE              4
-                      84 LOAD_CONST              10 (<code object exists, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\cache\page_cache.py", line 31>)
+                      84 LOAD_CONST              10 (<code object exists, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\cache\page_cache.py", line 31>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              11 (exists)
                       90 LOAD_CONST               5 (None)
                       92 RETURN_VALUE
          consts
             'PageCache'
             code
@@ -135,15 +135,15 @@
                             52 RETURN_VALUE
                consts
                   None
                names      ('diskcache', 'Cache', 'cache')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
                name       '__init__'
                firstlineno 11
                lnotab 0x0201
             'key'
             'return'
             code
                argcount  : 2
@@ -166,15 +166,15 @@
                             56 RETURN_VALUE
                consts
                   'Retrieve a value by key from the in-memory cache.'
                names      ('cache', 'get')
                varnames   ('self', 'key')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
                name       'get'
                firstlineno 14
                lnotab 0x0602
             None
             'value'
             'timeout'
             code
@@ -220,15 +220,15 @@
                consts
                   'Set the value for a key in the in-memory cache.'
                   None
                names      ('cache', 'set', 'expire')
                varnames   ('self', 'key', 'value', 'timeout')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
                name       'set'
                firstlineno 18
                lnotab 0x0602360104013aff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -264,15 +264,15 @@
                   'Delete a key from the in-memory cache.'
                   True
                   False
                names      ('cache', 'delete')
                varnames   ('self', 'key')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
                name       'delete'
                firstlineno 24
                lnotab 0x0602120134010401
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -299,29 +299,29 @@
                   'Check if a key exists in the in-memory cache.'
                   True
                   False
                names      ('cache',)
                varnames   ('self', 'key')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
                name       'exists'
                firstlineno 31
                lnotab 0x060212010401
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'Any', 'get', 'int', 'set', 'bool', 'delete', 'exists')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
          name       'PageCache'
          firstlineno 10
          lnotab 0x0a01060310041a061007
       'PageCache'
    names      ('__doc__', 'typing', 'Any', 'diskcache', 'fss.common.cache.cache', 'Cache', 'PageCache')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\cache\\page_cache.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\cache\\page_cache.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020c0208020c03
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/cache.py` & `fastapi_sqlmodel_starter-1.0.1/fss/common/cache/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """Abstract base class for Cache"""
 
 from abc import ABC, abstractmethod
+from typing import Any
 
-
+from fss.common.cache.redis_manager import RedisManager
 from fss.common.config import configs
 
 
 class Cache(ABC):
     @abstractmethod
-    async def get(self, key):
+    async def get(self, key: str) -> Any:
         """Retrieve a value by key from the cache."""
         pass
 
     @abstractmethod
-    async def set(self, key, value, timeout=None):
+    async def set(self, key: str, value: Any, timeout=None):
         """Set the value of a key in the cache with an optional timeout."""
         pass
 
     @abstractmethod
-    async def delete(self, key):
+    async def delete(self, key: str):
         """Delete a key from the cache."""
         pass
 
     @abstractmethod
-    async def exists(self, key):
+    async def exists(self, key: str):
         """Check if a key exists in the cache."""
         pass
 
 
 async def get_cache_client() -> Cache:
     """
     Init redis client or page cache client
     :return:
     """
-    if configs.enable_redis:
-        from fss.common.cache.redis_cache import RedisCache
-        from fss.common.cache.redis_cache import RedisManager
 
-        redis_client = await RedisManager.get_instance()
+    from fss.common.cache.redis_cache import RedisCache
+
+    redis_client = await RedisManager.get_instance()
+    if configs.enable_redis:
         return RedisCache(redis_client)
-    from fss.common.cache.page_cache import PageCache
+    else:
+        from fss.common.cache.page_cache import PageCache
 
-    return PageCache()
+        return PageCache()
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/page_cache.py` & `fastapi_sqlmodel_starter-1.0.1/fss/common/cache/page_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/enum/__pycache__/enum.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,68 +1,68 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 481
+moddate:  0x906c2266 (Fri Apr 19 13:07:28 2024 UTC)
+files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a0201000200470064038400640465
       036502a6040000ab0400000000000000005a040200470064058400640665
       036502a6040000ab0400000000000000005a050200470064078400640865
       036502a6040000ab0400000000000000005a0664095300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('The enumerations used in the project')
+     1           2 LOAD_CONST               0 ('Common enumerations')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('Enum',))
                 10 IMPORT_NAME              1 (enum)
                 12 IMPORT_FROM              2 (Enum)
                 14 STORE_NAME               2 (Enum)
                 16 POP_TOP
    
      6          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object ModeEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\enum\enum.py", line 6>)
+                22 LOAD_CONST               3 (<code object ModeEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\enum\enum.py", line 6>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               4 ('ModeEnum')
                 28 LOAD_NAME                3 (str)
                 30 LOAD_NAME                2 (Enum)
                 32 PRECALL                  4
                 36 CALL                     4
                 46 STORE_NAME               4 (ModeEnum)
    
     16          48 PUSH_NULL
                 50 LOAD_BUILD_CLASS
-                52 LOAD_CONST               5 (<code object SortEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\enum\enum.py", line 16>)
+                52 LOAD_CONST               5 (<code object SortEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\enum\enum.py", line 16>)
                 54 MAKE_FUNCTION            0
                 56 LOAD_CONST               6 ('SortEnum')
                 58 LOAD_NAME                3 (str)
                 60 LOAD_NAME                2 (Enum)
                 62 PRECALL                  4
                 66 CALL                     4
                 76 STORE_NAME               5 (SortEnum)
    
     25          78 PUSH_NULL
                 80 LOAD_BUILD_CLASS
-                82 LOAD_CONST               7 (<code object TokenTypeEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\enum\enum.py", line 25>)
+                82 LOAD_CONST               7 (<code object TokenTypeEnum, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\enum\enum.py", line 25>)
                 84 MAKE_FUNCTION            0
                 86 LOAD_CONST               8 ('TokenTypeEnum')
                 88 LOAD_NAME                3 (str)
                 90 LOAD_NAME                2 (Enum)
                 92 PRECALL                  4
                 96 CALL                     4
                106 STORE_NAME               6 (TokenTypeEnum)
                108 LOAD_CONST               9 (None)
                110 RETURN_VALUE
    consts
-      'The enumerations used in the project'
+      'Common enumerations'
       0
       ('Enum',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
@@ -95,15 +95,15 @@
             'prod'
             'test'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'development', 'production', 'testing')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\enum\\enum.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\enum\\enum.py'
          name       'ModeEnum'
          firstlineno 6
          lnotab 0x0a01040404010401
       'ModeEnum'
       code
          argcount  : 0
          nlocals   : 0
@@ -132,15 +132,15 @@
             'asc'
             'desc'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'ascending', 'descending')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\enum\\enum.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\enum\\enum.py'
          name       'SortEnum'
          firstlineno 16
          lnotab 0x0a0104040401
       'SortEnum'
       code
          argcount  : 0
          nlocals   : 0
@@ -169,21 +169,21 @@
             'access'
             'refresh'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'access', 'refresh')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\enum\\enum.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\enum\\enum.py'
          name       'TokenTypeEnum'
          firstlineno 25
          lnotab 0x0a0104040401
       'TokenTypeEnum'
       None
    names      ('__doc__', 'enum', 'Enum', 'str', 'ModeEnum', 'SortEnum', 'TokenTypeEnum')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\enum\\enum.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\enum\\enum.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020c031e0a1e09
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/exception/__pycache__/exception.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,41 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 428
+moddate:  0x906c2266 (Fri Apr 19 13:07:28 2024 UTC)
+files sz: 413
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a01020047006403840064046502a60300
       00ab0300000000000000005a0364025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 ('The exceptions used in the project')
+     1           2 LOAD_CONST               0 ('Customer exceptions')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (http)
                 12 STORE_NAME               1 (http)
    
      6          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               3 (<code object ServiceException, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\exception\exception.py", line 6>)
+                18 LOAD_CONST               3 (<code object ServiceException, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\exception\exception.py", line 6>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               4 ('ServiceException')
                 24 LOAD_NAME                2 (Exception)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               3 (ServiceException)
                 42 LOAD_CONST               2 (None)
                 44 RETURN_VALUE
    consts
-      'The exceptions used in the project'
+      'Customer exceptions'
       0
       None
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
@@ -55,15 +55,15 @@
                       34 LOAD_CONST               1 ('code')
                       36 LOAD_NAME                6 (int)
                       38 LOAD_CONST               2 ('msg')
                       40 LOAD_NAME                7 (str)
                       42 LOAD_CONST               3 ('status_code')
                       44 LOAD_NAME                6 (int)
                       46 BUILD_TUPLE              6
-                      48 LOAD_CONST               4 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\exception\exception.py", line 7>)
+                      48 LOAD_CONST               4 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\exception\exception.py", line 7>)
                       50 MAKE_FUNCTION            5 (defaults, annotations)
                       52 STORE_NAME               8 (__init__)
                       54 LOAD_CONST               5 (None)
                       56 RETURN_VALUE
          consts
             'ServiceException'
             'code'
@@ -95,29 +95,29 @@
                consts
                   '\n        Base service exception\n        :param code: error code\n        :param msg: error message\n        :param status_code: http status code\n        '
                   None
                names      ('code', 'msg', 'status_code')
                varnames   ('self', 'code', 'msg', 'status_code')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\exception\\exception.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\exception\\exception.py'
                name       '__init__'
                firstlineno 7
                lnotab 0x02070e010e01
             None
          names      ('__name__', '__module__', '__qualname__', 'http', 'HTTPStatus', 'OK', 'int', 'str', '__init__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\exception\\exception.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\exception\\exception.py'
          name       'ServiceException'
          firstlineno 6
          lnotab 0x0a01
       'ServiceException'
    names      ('__doc__', 'http', 'Exception', 'ServiceException')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\exception\\exception.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\exception\\exception.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020803
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/base_model.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
 files sz: 814
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -52,25 +52,25 @@
                 62 IMPORT_NAME             10 (fss.common.util.snowflake)
                 64 IMPORT_FROM             11 (snowflake_id)
                 66 STORE_NAME              11 (snowflake_id)
                 68 POP_TOP
    
     12          70 PUSH_NULL
                 72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               7 (<code object BaseModel, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\base_model.py", line 12>)
+                74 LOAD_CONST               7 (<code object BaseModel, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\base_model.py", line 12>)
                 76 MAKE_FUNCTION            0
                 78 LOAD_CONST               8 ('BaseModel')
                 80 LOAD_NAME                8 (_SQLModel)
                 82 PRECALL                  3
                 86 CALL                     3
                 96 STORE_NAME              12 (BaseModel)
    
     26          98 PUSH_NULL
                100 LOAD_BUILD_CLASS
-               102 LOAD_CONST               9 (<code object ModelExt, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\base_model.py", line 26>)
+               102 LOAD_CONST               9 (<code object ModelExt, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\base_model.py", line 26>)
                104 MAKE_FUNCTION            0
                106 LOAD_CONST              10 ('ModelExt')
                108 LOAD_NAME                8 (_SQLModel)
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME              13 (ModelExt)
                126 LOAD_CONST              11 (None)
@@ -133,15 +133,15 @@
             ('default_factory', 'primary_key', 'index', 'nullable', 'sa_type')
             'id'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Field', 'snowflake_id', 'BigInteger', 'id', 'int', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\base_model.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\base_model.py'
          name       'BaseModel'
          firstlineno 12
          lnotab 0x0c0104040401020102010201020102fb
       'BaseModel'
       code
          argcount  : 0
          nlocals   : 0
@@ -209,21 +209,21 @@
             ('default_factory', 'sa_column_kwargs')
             'update_time'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Field', 'datetime', 'now', 'create_time', 'Optional', '__annotations__', 'update_time')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\base_model.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\base_model.py'
          name       'ModelExt'
          firstlineno 26
          lnotab 0x0c010404380104011cff
       'ModelExt'
       None
    names      ('__doc__', 'datetime', 'typing', 'Optional', 'sqlalchemy', 'BigInteger', 'sqlmodel', 'SQLModel', '_SQLModel', 'Field', 'fss.common.util.snowflake', 'snowflake_id', 'BaseModel', 'ModelExt')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\base_model.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\base_model.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020c010c020c0110020c031c0e
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xba1e1a66 (Sat Apr 13 05:57:14 2024 UTC)
-files sz: 7039
+moddate:  0xc8dd2366 (Sat Apr 20 15:22:48 2024 UTC)
+files sz: 9921
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
@@ -142,15 +142,15 @@
                254 KW_NAMES                11
                256 PRECALL                  2
                260 CALL                     2
                270 STORE_NAME              31 (T)
    
     21         272 PUSH_NULL
                274 LOAD_BUILD_CLASS
-               276 LOAD_CONST              16 (<code object SqlModelMapper, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 21>)
+               276 LOAD_CONST              16 (<code object SqlModelMapper, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 21>)
                278 MAKE_FUNCTION            0
                280 LOAD_CONST              17 ('SqlModelMapper')
                282 LOAD_NAME                2 (Generic)
                284 LOAD_NAME               27 (ModelType)
                286 BINARY_SUBSCR
                296 LOAD_NAME               24 (BaseMapper)
                298 PRECALL                  4
@@ -174,388 +174,329 @@
       'CreateSchemaType'
       'UpdateSchemaType'
       'SchemaType'
       'T'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 16
+         stacksize : 14
          flags     : 0
          code
             0x970065005a0164005a0264016503650419000000000000000000660264
-            0284045a05640365036506190000000000000000006602640484045a0764
-            0564069c0164076508650465096602190000000000000000006408650865
-            0a64056602190000000000000000006403650b6606640984065a0c640564
-            069c01640a650d650619000000000000000000640865066403650b660664
-            0b84065a0e640564069c01640c650664086506640365066606640d84065a
-            0f640e6405640f9c026410650d6506190000000000000000006411650b64
-            0865066403650d6506190000000000000000006608641284065a10640564
-            069c01640865066403650b6604641384065a1164146415640564169c0364
-            17650b6418650b64196506640865066403650d6506190000000000000000
-            00660a641a84065a1264146415640564169c036417650b6418650b641965
-            06641b6506641c6506640865066403650d65061900000000000000000066
-            0e641d84065a13640564069c01641e650664196506640865066403650d65
-            06190000000000000000006608641f84065a14640564056405640564209c
-            04641e650664196506641b6506641c6506640865066403650d6506190000
-            00000000000000660c642184065a15640564069c01640765066408650664
-            03650b6606642284065a16640564069c01640a650d650619000000000000
-            000000640865066403650b6606642384065a17640564069c01640c650664
-            0865066403650b6606642484065a18640564069c016410650d6506190000
-            00000000000000640865066403650b6606642584065a1964055300
+            0284045a05640364049c0164056506650465076602190000000000000000
+            006406650665086403660219000000000000000000640765096606640884
+            065a0a640364049c016409650b6509190000000000000000006406650964
+            07650c6606640a84065a0d640364049c01640b6509640665096407650966
+            06640c84065a0e640364049c01640665096407650c6604640d84065a0f64
+            0e640f640364109c036411650c6412650c640665096407650b6509190000
+            000000000000006608641384065a10640e640f64036403640364149c0564
+            11650c6412650c6415650964166509640665096407650b65091900000000
+            0000000000660c641784065a11640364049c016418650964066509640765
+            0b6509190000000000000000006606641984065a12640364036403641a9c
+            03641865096415650964166509640665096407650b650919000000000000
+            000000660a641b84065a13640364049c0164056509640665096407650c66
+            06641c84065a14640364049c01641d650b65091900000000000000000064
+            056515640665096407650c6608641e84065a16640364049c01640b650964
+            0665096407650c6606641f84065a17640364049c01641d650b6509190000
+            00000000000000640665096407650c6606642084065a1864035300
           21           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SqlModelMapper')
                        8 STORE_NAME               2 (__qualname__)
          
           22          10 LOAD_CONST               1 ('model')
                       12 LOAD_NAME                3 (Type)
                       14 LOAD_NAME                4 (ModelType)
                       16 BINARY_SUBSCR
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 22>)
+                      28 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 22>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (__init__)
          
-          26          34 LOAD_CONST               3 ('return')
-                      36 LOAD_NAME                3 (Type)
-                      38 LOAD_NAME                6 (Any)
-                      40 BINARY_SUBSCR
-                      50 BUILD_TUPLE              2
-                      52 LOAD_CONST               4 (<code object get_db_session, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 26>)
-                      54 MAKE_FUNCTION            4 (annotations)
-                      56 STORE_NAME               7 (get_db_session)
+          30          34 LOAD_CONST               3 (None)
          
-          33          58 LOAD_CONST               5 (None)
+          26          36 LOAD_CONST               4 (('db_session',))
+                      38 BUILD_CONST_KEY_MAP      1
+                      40 LOAD_CONST               5 ('data')
          
-          29          60 LOAD_CONST               6 (('db_session',))
-                      62 BUILD_CONST_KEY_MAP      1
-                      64 LOAD_CONST               7 ('data')
+          29          42 LOAD_NAME                6 (Union)
+                      44 LOAD_NAME                4 (ModelType)
+                      46 LOAD_NAME                7 (SchemaType)
+                      48 BUILD_TUPLE              2
+                      50 BINARY_SUBSCR
          
-          32          66 LOAD_NAME                8 (Union)
-                      68 LOAD_NAME                4 (ModelType)
-                      70 LOAD_NAME                9 (SchemaType)
-                      72 BUILD_TUPLE              2
-                      74 BINARY_SUBSCR
+          26          60 LOAD_CONST               6 ('db_session')
          
-          29          84 LOAD_CONST               8 ('db_session')
+          30          62 LOAD_NAME                6 (Union)
+                      64 LOAD_NAME                8 (AsyncSession)
+                      66 LOAD_CONST               3 (None)
+                      68 BUILD_TUPLE              2
+                      70 BINARY_SUBSCR
          
-          33          86 LOAD_NAME                8 (Union)
-                      88 LOAD_NAME               10 (AsyncSession)
-                      90 LOAD_CONST               5 (None)
-                      92 BUILD_TUPLE              2
-                      94 BINARY_SUBSCR
+          26          80 LOAD_CONST               7 ('return')
          
-          29         104 LOAD_CONST               3 ('return')
+          31          82 LOAD_NAME                9 (Any)
          
-          34         106 LOAD_NAME               11 (int)
+          26          84 BUILD_TUPLE              6
+                      86 LOAD_CONST               8 (<code object insert, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 26>)
+                      88 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                      90 STORE_NAME              10 (insert)
          
-          29         108 BUILD_TUPLE              6
-                     110 LOAD_CONST               9 (<code object insert, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 29>)
-                     112 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     114 STORE_NAME              12 (insert)
+          48          92 LOAD_CONST               3 (None)
          
-          41         116 LOAD_CONST               5 (None)
+          47          94 LOAD_CONST               4 (('db_session',))
+                      96 BUILD_CONST_KEY_MAP      1
+                      98 LOAD_CONST               9 ('data_list')
          
-          40         118 LOAD_CONST               6 (('db_session',))
-                     120 BUILD_CONST_KEY_MAP      1
-                     122 LOAD_CONST              10 ('data_list')
+          48         100 LOAD_NAME               11 (List)
+                     102 LOAD_NAME                9 (Any)
+                     104 BINARY_SUBSCR
          
-          41         124 LOAD_NAME               13 (List)
-                     126 LOAD_NAME                6 (Any)
-                     128 BINARY_SUBSCR
+          47         114 LOAD_CONST               6 ('db_session')
          
-          40         138 LOAD_CONST               8 ('db_session')
+          48         116 LOAD_NAME                9 (Any)
          
-          41         140 LOAD_NAME                6 (Any)
+          47         118 LOAD_CONST               7 ('return')
          
-          40         142 LOAD_CONST               3 ('return')
+          49         120 LOAD_NAME               12 (int)
          
-          42         144 LOAD_NAME               11 (int)
+          47         122 BUILD_TUPLE              6
+                     124 LOAD_CONST              10 (<code object insert_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 47>)
+                     126 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     128 STORE_NAME              13 (insert_batch)
          
-          40         146 BUILD_TUPLE              6
-                     148 LOAD_CONST              11 (<code object insert_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 40>)
-                     150 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     152 STORE_NAME              14 (insert_batch)
+          66         130 LOAD_CONST               3 (None)
+                     132 LOAD_CONST               4 (('db_session',))
+                     134 BUILD_CONST_KEY_MAP      1
+                     136 LOAD_CONST              11 ('id')
+                     138 LOAD_NAME                9 (Any)
+                     140 LOAD_CONST               6 ('db_session')
+                     142 LOAD_NAME                9 (Any)
+                     144 LOAD_CONST               7 ('return')
+                     146 LOAD_NAME                9 (Any)
+                     148 BUILD_TUPLE              6
+                     150 LOAD_CONST              12 (<code object select_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 66>)
+                     152 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     154 STORE_NAME              14 (select_by_id)
          
-          51         154 LOAD_CONST               5 (None)
-                     156 LOAD_CONST               6 (('db_session',))
-                     158 BUILD_CONST_KEY_MAP      1
-                     160 LOAD_CONST              12 ('id')
-                     162 LOAD_NAME                6 (Any)
-                     164 LOAD_CONST               8 ('db_session')
-                     166 LOAD_NAME                6 (Any)
-                     168 LOAD_CONST               3 ('return')
-                     170 LOAD_NAME                6 (Any)
-                     172 BUILD_TUPLE              6
-                     174 LOAD_CONST              13 (<code object select_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 51>)
-                     176 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     178 STORE_NAME              15 (select_by_id)
+          82         156 LOAD_CONST               3 (None)
+                     158 LOAD_CONST               4 (('db_session',))
+                     160 BUILD_CONST_KEY_MAP      1
+                     162 LOAD_CONST               6 ('db_session')
+                     164 LOAD_NAME                9 (Any)
+                     166 LOAD_CONST               7 ('return')
+                     168 LOAD_NAME               12 (int)
+                     170 BUILD_TUPLE              4
+                     172 LOAD_CONST              13 (<code object select_count, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 82>)
+                     174 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     176 STORE_NAME              15 (select_count)
          
-          58         180 LOAD_CONST              14 (1000)
-                     182 LOAD_CONST               5 (None)
+          99         178 LOAD_CONST              14 (1)
+                     180 LOAD_CONST              15 (100)
+                     182 LOAD_CONST               3 (None)
          
-          57         184 LOAD_CONST              15 (('batch_size', 'db_session'))
-                     186 BUILD_CONST_KEY_MAP      2
-                     188 LOAD_CONST              16 ('ids')
+          98         184 LOAD_CONST              16 (('page', 'size', 'db_session'))
+                     186 BUILD_CONST_KEY_MAP      3
+                     188 LOAD_CONST              17 ('page')
          
-          58         190 LOAD_NAME               13 (List)
-                     192 LOAD_NAME                6 (Any)
-                     194 BINARY_SUBSCR
+          99         190 LOAD_NAME               12 (int)
          
-          57         204 LOAD_CONST              17 ('batch_size')
+          98         192 LOAD_CONST              18 ('size')
          
-          58         206 LOAD_NAME               11 (int)
+          99         194 LOAD_NAME               12 (int)
          
-          57         208 LOAD_CONST               8 ('db_session')
+          98         196 LOAD_CONST               6 ('db_session')
          
-          58         210 LOAD_NAME                6 (Any)
+          99         198 LOAD_NAME                9 (Any)
          
-          57         212 LOAD_CONST               3 ('return')
+          98         200 LOAD_CONST               7 ('return')
          
-          59         214 LOAD_NAME               13 (List)
-                     216 LOAD_NAME                6 (Any)
-                     218 BINARY_SUBSCR
+         100         202 LOAD_NAME               11 (List)
+                     204 LOAD_NAME                9 (Any)
+                     206 BINARY_SUBSCR
          
-          57         228 BUILD_TUPLE              8
-                     230 LOAD_CONST              18 (<code object select_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 57>)
-                     232 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     234 STORE_NAME              16 (select_by_ids)
+          98         216 BUILD_TUPLE              8
+                     218 LOAD_CONST              19 (<code object select_list, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 98>)
+                     220 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     222 STORE_NAME              16 (select_list)
          
-          69         236 LOAD_CONST               5 (None)
-                     238 LOAD_CONST               6 (('db_session',))
-                     240 BUILD_CONST_KEY_MAP      1
-                     242 LOAD_CONST               8 ('db_session')
-                     244 LOAD_NAME                6 (Any)
-                     246 LOAD_CONST               3 ('return')
-                     248 LOAD_NAME               11 (int)
-                     250 BUILD_TUPLE              4
-                     252 LOAD_CONST              19 (<code object select_count, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 69>)
-                     254 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     256 STORE_NAME              17 (select_count)
+         129         224 LOAD_CONST              14 (1)
          
-          77         258 LOAD_CONST              20 (1)
-                     260 LOAD_CONST              21 (100)
-                     262 LOAD_CONST               5 (None)
+         130         226 LOAD_CONST              15 (100)
          
-          76         264 LOAD_CONST              22 (('page', 'size', 'db_session'))
-                     266 BUILD_CONST_KEY_MAP      3
-                     268 LOAD_CONST              23 ('page')
+         131         228 LOAD_CONST               3 (None)
          
-          77         270 LOAD_NAME               11 (int)
+         132         230 LOAD_CONST               3 (None)
          
-          76         272 LOAD_CONST              24 ('size')
+         133         232 LOAD_CONST               3 (None)
          
-          77         274 LOAD_NAME               11 (int)
+         126         234 LOAD_CONST              20 (('page', 'size', 'order_by', 'sort_order', 'db_session'))
+                     236 BUILD_CONST_KEY_MAP      5
+                     238 LOAD_CONST              17 ('page')
          
-          76         276 LOAD_CONST              25 ('query')
+         129         240 LOAD_NAME               12 (int)
          
-          77         278 LOAD_NAME                6 (Any)
+         126         242 LOAD_CONST              18 ('size')
          
-          76         280 LOAD_CONST               8 ('db_session')
+         130         244 LOAD_NAME               12 (int)
          
-          77         282 LOAD_NAME                6 (Any)
+         126         246 LOAD_CONST              21 ('order_by')
          
-          76         284 LOAD_CONST               3 ('return')
+         131         248 LOAD_NAME                9 (Any)
          
-          78         286 LOAD_NAME               13 (List)
-                     288 LOAD_NAME                6 (Any)
-                     290 BINARY_SUBSCR
+         126         250 LOAD_CONST              22 ('sort_order')
          
-          76         300 BUILD_TUPLE             10
-                     302 LOAD_CONST              26 (<code object select_list, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 76>)
-                     304 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     306 STORE_NAME              18 (select_list)
+         132         252 LOAD_NAME                9 (Any)
          
-          93         308 LOAD_CONST              20 (1)
+         126         254 LOAD_CONST               6 ('db_session')
          
-          94         310 LOAD_CONST              21 (100)
+         133         256 LOAD_NAME                9 (Any)
          
-          98         312 LOAD_CONST               5 (None)
+         126         258 LOAD_CONST               7 ('return')
          
-          90         314 LOAD_CONST              22 (('page', 'size', 'db_session'))
-                     316 BUILD_CONST_KEY_MAP      3
-                     318 LOAD_CONST              23 ('page')
+         135         260 LOAD_NAME               11 (List)
+                     262 LOAD_NAME                9 (Any)
+                     264 BINARY_SUBSCR
          
-          93         320 LOAD_NAME               11 (int)
+         126         274 BUILD_TUPLE             12
+                     276 LOAD_CONST              23 (<code object select_list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 126>)
+                     278 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     280 STORE_NAME              17 (select_list_ordered)
          
-          90         322 LOAD_CONST              24 ('size')
+         174         282 LOAD_CONST               3 (None)
+                     284 LOAD_CONST               4 (('db_session',))
+                     286 BUILD_CONST_KEY_MAP      1
+                     288 LOAD_CONST              24 ('params')
+                     290 LOAD_NAME                9 (Any)
+                     292 LOAD_CONST               6 ('db_session')
+                     294 LOAD_NAME                9 (Any)
+                     296 LOAD_CONST               7 ('return')
+                     298 LOAD_NAME               11 (List)
+                     300 LOAD_NAME                9 (Any)
+                     302 BINARY_SUBSCR
+                     312 BUILD_TUPLE              6
+                     314 LOAD_CONST              25 (<code object select_page, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 174>)
+                     316 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     318 STORE_NAME              18 (select_page)
          
-          94         324 LOAD_NAME               11 (int)
+         190         320 LOAD_CONST               3 (None)
          
-          90         326 LOAD_CONST              25 ('query')
+         191         322 LOAD_CONST               3 (None)
          
-          95         328 LOAD_NAME                6 (Any)
+         192         324 LOAD_CONST               3 (None)
          
-          90         330 LOAD_CONST              27 ('order_by')
+         186         326 LOAD_CONST              26 (('order_by', 'sort_order', 'db_session'))
+                     328 BUILD_CONST_KEY_MAP      3
+                     330 LOAD_CONST              24 ('params')
          
-          96         332 LOAD_NAME                6 (Any)
+         189         332 LOAD_NAME                9 (Any)
          
-          90         334 LOAD_CONST              28 ('sort_order')
+         186         334 LOAD_CONST              21 ('order_by')
          
-          97         336 LOAD_NAME                6 (Any)
+         190         336 LOAD_NAME                9 (Any)
          
-          90         338 LOAD_CONST               8 ('db_session')
+         186         338 LOAD_CONST              22 ('sort_order')
          
-          98         340 LOAD_NAME                6 (Any)
+         191         340 LOAD_NAME                9 (Any)
          
-          90         342 LOAD_CONST               3 ('return')
+         186         342 LOAD_CONST               6 ('db_session')
          
-          99         344 LOAD_NAME               13 (List)
-                     346 LOAD_NAME                6 (Any)
-                     348 BINARY_SUBSCR
+         192         344 LOAD_NAME                9 (Any)
          
-          90         358 BUILD_TUPLE             14
-                     360 LOAD_CONST              29 (<code object select_list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 90>)
-                     362 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     364 STORE_NAME              19 (select_list_ordered)
+         186         346 LOAD_CONST               7 ('return')
          
-         122         366 LOAD_CONST               5 (None)
+         193         348 LOAD_NAME               11 (List)
+                     350 LOAD_NAME                9 (Any)
+                     352 BINARY_SUBSCR
          
-         121         368 LOAD_CONST               6 (('db_session',))
-                     370 BUILD_CONST_KEY_MAP      1
-                     372 LOAD_CONST              30 ('params')
+         186         362 BUILD_TUPLE             10
+                     364 LOAD_CONST              27 (<code object select_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 186>)
+                     366 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     368 STORE_NAME              19 (select_page_ordered)
          
-         122         374 LOAD_NAME                6 (Any)
+         213         370 LOAD_CONST               3 (None)
+                     372 LOAD_CONST               4 (('db_session',))
+                     374 BUILD_CONST_KEY_MAP      1
+                     376 LOAD_CONST               5 ('data')
+                     378 LOAD_NAME                9 (Any)
+                     380 LOAD_CONST               6 ('db_session')
+                     382 LOAD_NAME                9 (Any)
+                     384 LOAD_CONST               7 ('return')
+                     386 LOAD_NAME               12 (int)
+                     388 BUILD_TUPLE              6
+                     390 LOAD_CONST              28 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 213>)
+                     392 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     394 STORE_NAME              20 (update_by_id)
          
-         121         376 LOAD_CONST              25 ('query')
+         229         396 LOAD_CONST               3 (None)
          
-         122         378 LOAD_NAME                6 (Any)
+         228         398 LOAD_CONST               4 (('db_session',))
+                     400 BUILD_CONST_KEY_MAP      1
+                     402 LOAD_CONST              29 ('ids')
          
-         121         380 LOAD_CONST               8 ('db_session')
+         229         404 LOAD_NAME               11 (List)
+                     406 LOAD_NAME                9 (Any)
+                     408 BINARY_SUBSCR
          
-         122         382 LOAD_NAME                6 (Any)
+         228         418 LOAD_CONST               5 ('data')
          
-         121         384 LOAD_CONST               3 ('return')
+         229         420 LOAD_NAME               21 (dict)
          
-         123         386 LOAD_NAME               13 (List)
-                     388 LOAD_NAME                6 (Any)
-                     390 BINARY_SUBSCR
+         228         422 LOAD_CONST               6 ('db_session')
          
-         121         400 BUILD_TUPLE              8
-                     402 LOAD_CONST              31 (<code object select_list_page, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 121>)
-                     404 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     406 STORE_NAME              20 (select_list_page)
+         229         424 LOAD_NAME                9 (Any)
          
-         134         408 LOAD_CONST               5 (None)
+         228         426 LOAD_CONST               7 ('return')
          
-         135         410 LOAD_CONST               5 (None)
+         230         428 LOAD_NAME               12 (int)
          
-         136         412 LOAD_CONST               5 (None)
+         228         430 BUILD_TUPLE              8
+                     432 LOAD_CONST              30 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 228>)
+                     434 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     436 STORE_NAME              22 (update_batch_by_ids)
          
-         137         414 LOAD_CONST               5 (None)
-         
-         130         416 LOAD_CONST              32 (('query', 'order_by', 'sort_order', 'db_session'))
-                     418 BUILD_CONST_KEY_MAP      4
-                     420 LOAD_CONST              30 ('params')
-         
-         133         422 LOAD_NAME                6 (Any)
-         
-         130         424 LOAD_CONST              25 ('query')
-         
-         134         426 LOAD_NAME                6 (Any)
-         
-         130         428 LOAD_CONST              27 ('order_by')
-         
-         135         430 LOAD_NAME                6 (Any)
+         246         438 LOAD_CONST               3 (None)
+                     440 LOAD_CONST               4 (('db_session',))
+                     442 BUILD_CONST_KEY_MAP      1
+                     444 LOAD_CONST              11 ('id')
+                     446 LOAD_NAME                9 (Any)
+                     448 LOAD_CONST               6 ('db_session')
+                     450 LOAD_NAME                9 (Any)
+                     452 LOAD_CONST               7 ('return')
+                     454 LOAD_NAME               12 (int)
+                     456 BUILD_TUPLE              6
+                     458 LOAD_CONST              31 (<code object delete_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 246>)
+                     460 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     462 STORE_NAME              23 (delete_by_id)
          
-         130         432 LOAD_CONST              28 ('sort_order')
+         260         464 LOAD_CONST               3 (None)
          
-         136         434 LOAD_NAME                6 (Any)
+         259         466 LOAD_CONST               4 (('db_session',))
+                     468 BUILD_CONST_KEY_MAP      1
+                     470 LOAD_CONST              29 ('ids')
          
-         130         436 LOAD_CONST               8 ('db_session')
+         260         472 LOAD_NAME               11 (List)
+                     474 LOAD_NAME                9 (Any)
+                     476 BINARY_SUBSCR
          
-         137         438 LOAD_NAME                6 (Any)
+         259         486 LOAD_CONST               6 ('db_session')
          
-         130         440 LOAD_CONST               3 ('return')
+         260         488 LOAD_NAME                9 (Any)
          
-         138         442 LOAD_NAME               13 (List)
-                     444 LOAD_NAME                6 (Any)
-                     446 BINARY_SUBSCR
+         259         490 LOAD_CONST               7 ('return')
          
-         130         456 BUILD_TUPLE             12
-                     458 LOAD_CONST              33 (<code object select_list_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 130>)
-                     460 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     462 STORE_NAME              21 (select_list_page_ordered)
+         261         492 LOAD_NAME               12 (int)
          
-         150         464 LOAD_CONST               5 (None)
-                     466 LOAD_CONST               6 (('db_session',))
-                     468 BUILD_CONST_KEY_MAP      1
-                     470 LOAD_CONST               7 ('data')
-                     472 LOAD_NAME                6 (Any)
-                     474 LOAD_CONST               8 ('db_session')
-                     476 LOAD_NAME                6 (Any)
-                     478 LOAD_CONST               3 ('return')
-                     480 LOAD_NAME               11 (int)
-                     482 BUILD_TUPLE              6
-                     484 LOAD_CONST              34 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 150>)
-                     486 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     488 STORE_NAME              22 (update_by_id)
-         
-         168         490 LOAD_CONST               5 (None)
-         
-         167         492 LOAD_CONST               6 (('db_session',))
-                     494 BUILD_CONST_KEY_MAP      1
-                     496 LOAD_CONST              10 ('data_list')
-         
-         168         498 LOAD_NAME               13 (List)
-                     500 LOAD_NAME                6 (Any)
-                     502 BINARY_SUBSCR
-         
-         167         512 LOAD_CONST               8 ('db_session')
-         
-         168         514 LOAD_NAME                6 (Any)
-         
-         167         516 LOAD_CONST               3 ('return')
-         
-         169         518 LOAD_NAME               11 (int)
-         
-         167         520 BUILD_TUPLE              6
-                     522 LOAD_CONST              35 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 167>)
-                     524 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     526 STORE_NAME              23 (update_batch_by_ids)
-         
-         181         528 LOAD_CONST               5 (None)
-                     530 LOAD_CONST               6 (('db_session',))
-                     532 BUILD_CONST_KEY_MAP      1
-                     534 LOAD_CONST              12 ('id')
-                     536 LOAD_NAME                6 (Any)
-                     538 LOAD_CONST               8 ('db_session')
-                     540 LOAD_NAME                6 (Any)
-                     542 LOAD_CONST               3 ('return')
-                     544 LOAD_NAME               11 (int)
-                     546 BUILD_TUPLE              6
-                     548 LOAD_CONST              36 (<code object delete_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 181>)
-                     550 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     552 STORE_NAME              24 (delete_by_id)
-         
-         189         554 LOAD_CONST               5 (None)
-         
-         188         556 LOAD_CONST               6 (('db_session',))
-                     558 BUILD_CONST_KEY_MAP      1
-                     560 LOAD_CONST              16 ('ids')
-         
-         189         562 LOAD_NAME               13 (List)
-                     564 LOAD_NAME                6 (Any)
-                     566 BINARY_SUBSCR
-         
-         188         576 LOAD_CONST               8 ('db_session')
-         
-         189         578 LOAD_NAME                6 (Any)
-         
-         188         580 LOAD_CONST               3 ('return')
-         
-         190         582 LOAD_NAME               11 (int)
-         
-         188         584 BUILD_TUPLE              6
-                     586 LOAD_CONST              37 (<code object delete_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 188>)
-                     588 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     590 STORE_NAME              25 (delete_batch_by_ids)
-                     592 LOAD_CONST               5 (None)
-                     594 RETURN_VALUE
+         259         494 BUILD_TUPLE              6
+                     496 LOAD_CONST              32 (<code object delete_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 259>)
+                     498 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     500 STORE_NAME              24 (delete_batch_by_ids)
+                     502 LOAD_CONST               3 (None)
+                     504 RETURN_VALUE
          consts
             'SqlModelMapper'
             'model'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -576,188 +517,187 @@
                             42 RETURN_VALUE
                consts
                   None
                names      ('model', 'db')
                varnames   ('self', 'model')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       '__init__'
                firstlineno 22
                lnotab 0x02010e01
-            'return'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
-               flags     : 3
-               code 0x97007c006a0000000000000000005300
-                26           0 RESUME                   0
-               
-                27           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (db)
-                            14 RETURN_VALUE
-               consts
-                  None
-               names      ('db',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
-               name       'get_db_session'
-               firstlineno 26
-               lnotab 0x0201
             None
             ('db_session',)
             'data'
             'db_session'
+            'return'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027c006a020000000000000000a0030000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007d037c02a0
                   0400000000000000000000000000000000000000007c03a6010000ab0100
                   0000000000000001007c035300
-                29           0 RETURN_GENERATOR
+                26           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                35           6 LOAD_FAST                2 (db_session)
+                42           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-                36          34 LOAD_FAST                0 (self)
+                43          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (model)
                             46 LOAD_METHOD              3 (model_validate)
                             68 LOAD_FAST                1 (data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               3 (orm_data)
                
-                37          86 LOAD_FAST                2 (db_session)
+                44          86 LOAD_FAST                2 (db_session)
                             88 LOAD_METHOD              4 (add)
                            110 LOAD_FAST                3 (orm_data)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 POP_TOP
                
-                38         128 LOAD_FAST                3 (orm_data)
+                45         128 LOAD_FAST                3 (orm_data)
                            130 RETURN_VALUE
                consts
-                  None
+                  '\n        Inserts a single row into the database.\n\n        Args:\n            data: The data to be inserted, either a Model instance or a Schema dict.\n            db_session: The database session to use. If None, uses the default session.\n\n        Returns:\n            The inserted row with ID.\n        '
                names      ('db', 'session', 'model', 'model_validate', 'add')
                varnames   ('self', 'data', 'db_session', 'orm_data')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'insert'
-               firstlineno 29
-               lnotab 0x06061c0134012a01
+               firstlineno 26
+               lnotab 0x06101c0134012a01
             'data_list'
             code
                argcount  : 1
                nlocals   : 6
-               stacksize : 6
+               stacksize : 4
                flags     : 131
                code
-                  0x4b00010097007c02700b7c006a0000000000000000006a010000000000
-                  0000007d0267007d037c0144005d2f7d047c03a002000000000000000000
-                  00000000000000000000007c006a030000000000000000a0040000000000
-                  0000000000000000000000000000007c04a6010000ab0100000000000000
-                  00a6010000ab01000000000000000001008c30740b000000000000000000
-                  007c006a030000000000000000a6010000ab010000000000000000a00600
-                  00000000000000000000000000000000000000640184007c034400a60000
-                  00ab000000000000000000a6010000ab0100000000000000007d057c02a0
-                  0700000000000000000000000000000000000000007c05a6010000ab0100
-                  00000000000000830064007b035600970386040100741100000000000000
-                  0000007c01a6010000ab0100000000000000005300
-                40           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                43           6 LOAD_FAST                2 (db_session)
-                             8 JUMP_IF_TRUE_OR_POP     11 (to 32)
-                            10 LOAD_FAST                0 (self)
-                            12 LOAD_ATTR                0 (db)
-                            22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               2 (db_session)
-               
-                44          34 BUILD_LIST               0
-                            36 STORE_FAST               3 (orm_datas)
-               
-                45          38 LOAD_FAST                1 (data_list)
-                            40 GET_ITER
-                       >>   42 FOR_ITER                47 (to 138)
-                            44 STORE_FAST               4 (data)
-               
-                46          46 LOAD_FAST                3 (orm_datas)
-                            48 LOAD_METHOD              2 (append)
-                            70 LOAD_FAST                0 (self)
-                            72 LOAD_ATTR                3 (model)
-                            82 LOAD_METHOD              4 (model_validate)
-                           104 LOAD_FAST                4 (data)
-                           106 PRECALL                  1
-                           110 CALL                     1
-                           120 PRECALL                  1
-                           124 CALL                     1
-                           134 POP_TOP
-                           136 JUMP_BACKWARD           48 (to 42)
-               
-                47     >>  138 LOAD_GLOBAL             11 (NULL + insert)
-                           150 LOAD_FAST                0 (self)
-                           152 LOAD_ATTR                3 (model)
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 LOAD_METHOD              6 (values)
-                           198 LOAD_CONST               1 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 47>)
-                           200 MAKE_FUNCTION            0
-                           202 LOAD_FAST                3 (orm_datas)
-                           204 GET_ITER
-                           206 PRECALL                  0
-                           210 CALL                     0
-                           220 PRECALL                  1
-                           224 CALL                     1
-                           234 STORE_FAST               5 (statement)
-               
-                48         236 LOAD_FAST                2 (db_session)
-                           238 LOAD_METHOD              7 (execute)
-                           260 LOAD_FAST                5 (statement)
-                           262 PRECALL                  1
-                           266 CALL                     1
-                           276 GET_AWAITABLE            0
-                           278 LOAD_CONST               0 (None)
-                       >>  280 SEND                     3 (to 288)
-                           282 YIELD_VALUE
-                           284 RESUME                   3
-                           286 JUMP_BACKWARD_NO_INTERRUPT     4 (to 280)
-                       >>  288 POP_TOP
-               
-                49         290 LOAD_GLOBAL             17 (NULL + len)
-                           302 LOAD_FAST                1 (data_list)
-                           304 PRECALL                  1
-                           308 CALL                     1
-                           318 RETURN_VALUE
+                  0x87004b00010097007c02700b89006a0000000000000000006a01000000
+                  00000000007d0288006601640184087c014400a6000000ab000000000000
+                  0000007d0374050000000000000000000089006a030000000000000000a6
+                  010000ab010000000000000000a004000000000000000000000000000000
+                  0000000000640284007c034400a6000000ab000000000000000000a60100
+                  00ab0100000000000000007d047c02a00500000000000000000000000000
+                  000000000000007c04a6010000ab010000000000000000830064037b0356
+                  00970386047d057c056a0600000000000000005300
+                             0 MAKE_CELL                0 (self)
+               
+                47           2 RETURN_GENERATOR
+                             4 POP_TOP
+                             6 RESUME                   0
+               
+                60           8 LOAD_FAST                2 (db_session)
+                            10 JUMP_IF_TRUE_OR_POP     11 (to 34)
+                            12 LOAD_DEREF               0 (self)
+                            14 LOAD_ATTR                0 (db)
+                            24 LOAD_ATTR                1 (session)
+                       >>   34 STORE_FAST               2 (db_session)
+               
+                61          36 LOAD_CLOSURE             0 (self)
+                            38 BUILD_TUPLE              1
+                            40 LOAD_CONST               1 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 61>)
+                            42 MAKE_FUNCTION            8 (closure)
+                            44 LOAD_FAST                1 (data_list)
+                            46 GET_ITER
+                            48 PRECALL                  0
+                            52 CALL                     0
+                            62 STORE_FAST               3 (orm_datas)
+               
+                62          64 LOAD_GLOBAL              5 (NULL + insert)
+                            76 LOAD_DEREF               0 (self)
+                            78 LOAD_ATTR                3 (model)
+                            88 PRECALL                  1
+                            92 CALL                     1
+                           102 LOAD_METHOD              4 (values)
+                           124 LOAD_CONST               2 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\persistence\sqlmodel_impl.py", line 62>)
+                           126 MAKE_FUNCTION            0
+                           128 LOAD_FAST                3 (orm_datas)
+                           130 GET_ITER
+                           132 PRECALL                  0
+                           136 CALL                     0
+                           146 PRECALL                  1
+                           150 CALL                     1
+                           160 STORE_FAST               4 (statement)
+               
+                63         162 LOAD_FAST                2 (db_session)
+                           164 LOAD_METHOD              5 (execute)
+                           186 LOAD_FAST                4 (statement)
+                           188 PRECALL                  1
+                           192 CALL                     1
+                           202 GET_AWAITABLE            0
+                           204 LOAD_CONST               3 (None)
+                       >>  206 SEND                     3 (to 214)
+                           208 YIELD_VALUE
+                           210 RESUME                   3
+                           212 JUMP_BACKWARD_NO_INTERRUPT     4 (to 206)
+                       >>  214 STORE_FAST               5 (result)
+               
+                64         216 LOAD_FAST                5 (result)
+                           218 LOAD_ATTR                6 (rowcount)
+                           228 RETURN_VALUE
                consts
-                  None
+                  '\n        Inserts multiple rows into the database in a single batch.\n\n        Args:\n            data_list: A list of data to be inserted, each item either a Model instance or a Schema dict.\n            db_session: The database session to use. If None, uses the default session.\n\n        Returns:\n            The number of rows inserted.\n        '
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 5
+                     flags     : 19
+                     code
+                        0x9501970067007c005d1c7d0189026a000000000000000000a001000000
+                        00000000000000000000000000000000007c01a6010000ab010000000000
+                        00000091028c1d5300
+                                   0 COPY_FREE_VARS           1
+                     
+                      61           2 RESUME                   0
+                                   4 BUILD_LIST               0
+                                   6 LOAD_FAST                0 (.0)
+                             >>    8 FOR_ITER                28 (to 66)
+                                  10 STORE_FAST               1 (data)
+                                  12 LOAD_DEREF               2 (self)
+                                  14 LOAD_ATTR                0 (model)
+                                  24 LOAD_METHOD              1 (model_validate)
+                                  46 LOAD_FAST                1 (data)
+                                  48 PRECALL                  1
+                                  52 CALL                     1
+                                  62 LIST_APPEND              2
+                                  64 JUMP_BACKWARD           29 (to 8)
+                             >>   66 RETURN_VALUE
+                     consts
+                     names      ('model', 'model_validate')
+                     varnames   ('.0', 'data')
+                     freevars   ('self',)
+                     cellvars   ()
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
+                     name       '<listcomp>'
+                     firstlineno 61
+                     lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c01a000000000000000000000000000000000
                         0000000000a6000000ab00000000000000000091028c175300
-                      47           0 RESUME                   0
+                      62           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 STORE_FAST               1 (data)
                                   10 LOAD_FAST                1 (data)
                                   12 LOAD_METHOD              0 (model_dump)
                                   34 PRECALL                  0
@@ -766,240 +706,128 @@
                                   50 JUMP_BACKWARD           23 (to 6)
                              >>   52 RETURN_VALUE
                      consts
                      names      ('model_dump',)
                      varnames   ('.0', 'data')
                      freevars   ()
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                      name       '<listcomp>'
-                     firstlineno 47
+                     firstlineno 62
                      lnotab 0x
-               names      ('db', 'session', 'append', 'model', 'model_validate', 'insert', 'values', 'execute', 'len')
-               varnames   ('self', 'data_list', 'db_session', 'orm_datas', 'data', 'statement')
+                  None
+               names      ('db', 'session', 'insert', 'model', 'values', 'execute', 'rowcount')
+               varnames   ('self', 'data_list', 'db_session', 'orm_datas', 'statement', 'result')
                freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               cellvars   ('self',)
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'insert_batch'
-               firstlineno 40
-               lnotab 0x06031c01040108015c0162013601
+               firstlineno 47
+               lnotab 0x080d1c011c0162013601
             'id'
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a0500000000000000007c016b
                   0200000000a6010000ab0100000000000000007d037c02a0060000000000
                   0000000000000000000000000000007c03a6010000ab0100000000000000
-                  00830064007b035600970386047d047c04a0070000000000000000000000
+                  00830064017b035600970386047d047c04a0070000000000000000000000
                   000000000000000000a6000000ab0000000000000000005300
-                51           0 RETURN_GENERATOR
+                66           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                52           6 LOAD_FAST                2 (db_session)
+                77           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-                53          34 LOAD_GLOBAL              5 (NULL + select)
+                78          34 LOAD_GLOBAL              5 (NULL + select)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
                            106 LOAD_ATTR                5 (id)
                            116 LOAD_FAST                1 (id)
                            118 COMPARE_OP               2 (==)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 STORE_FAST               3 (statement)
                
-                54         140 LOAD_FAST                2 (db_session)
+                79         140 LOAD_FAST                2 (db_session)
                            142 LOAD_METHOD              6 (execute)
                            164 LOAD_FAST                3 (statement)
                            166 PRECALL                  1
                            170 CALL                     1
                            180 GET_AWAITABLE            0
-                           182 LOAD_CONST               0 (None)
+                           182 LOAD_CONST               1 (None)
                        >>  184 SEND                     3 (to 192)
                            186 YIELD_VALUE
                            188 RESUME                   3
                            190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
                        >>  192 STORE_FAST               4 (response)
                
-                55         194 LOAD_FAST                4 (response)
+                80         194 LOAD_FAST                4 (response)
                            196 LOAD_METHOD              7 (scalar_one_or_none)
                            218 PRECALL                  0
                            222 CALL                     0
                            232 RETURN_VALUE
                consts
+                  '\n        Retrieves a single row by its ID.\n\n        Args:\n            id: The ID of the row to retrieve.\n            db_session: The database session to use. If None, uses the default session.\n\n        Returns:\n            The retrieved row, or None if not found.\n        '
                   None
                names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one_or_none')
                varnames   ('self', 'id', 'db_session', 'statement', 'response')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_by_id'
-               firstlineno 51
-               lnotab 0x06011c016a013601
-            1000
-            ('batch_size', 'db_session')
-            'ids'
-            'batch_size'
-            code
-               argcount  : 1
-               nlocals   : 9
-               stacksize : 6
-               flags     : 131
-               code
-                  0x4b00010097007c03700b7c006a0000000000000000006a010000000000
-                  0000007d0367007d04740500000000000000000000640174070000000000
-                  00000000007c01a6010000ab0100000000000000007c02a6030000ab0300
-                  0000000000000044005d957d057c017c057c057c027a0000008502190000
-                  000000000000007d067409000000000000000000007c006a050000000000
-                  000000a6010000ab010000000000000000a0060000000000000000000000
-                  0000000000000000007c006a0500000000000000006a0700000000000000
-                  00a00800000000000000000000000000000000000000007c06a6010000ab
-                  010000000000000000a6010000ab0100000000000000007d077c03a00900
-                  000000000000000000000000000000000000007c07a6010000ab01000000
-                  0000000000a00a0000000000000000000000000000000000000000a60000
-                  00ab000000000000000000830064007b035600970386047d087c04a00b00
-                  000000000000000000000000000000000000007c08a6010000ab01000000
-                  000000000001008c967c045300
-                57           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                60           6 LOAD_FAST                3 (db_session)
-                             8 JUMP_IF_TRUE_OR_POP     11 (to 32)
-                            10 LOAD_FAST                0 (self)
-                            12 LOAD_ATTR                0 (db)
-                            22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               3 (db_session)
-               
-                61          34 BUILD_LIST               0
-                            36 STORE_FAST               4 (result_set)
-               
-                62          38 LOAD_GLOBAL              5 (NULL + range)
-                            50 LOAD_CONST               1 (0)
-                            52 LOAD_GLOBAL              7 (NULL + len)
-                            64 LOAD_FAST                1 (ids)
-                            66 PRECALL                  1
-                            70 CALL                     1
-                            80 LOAD_FAST                2 (batch_size)
-                            82 PRECALL                  3
-                            86 CALL                     3
-                            96 GET_ITER
-                       >>   98 FOR_ITER               149 (to 398)
-                           100 STORE_FAST               5 (i)
-               
-                63         102 LOAD_FAST                1 (ids)
-                           104 LOAD_FAST                5 (i)
-                           106 LOAD_FAST                5 (i)
-                           108 LOAD_FAST                2 (batch_size)
-                           110 BINARY_OP                0 (+)
-                           114 BUILD_SLICE              2
-                           116 BINARY_SUBSCR
-                           126 STORE_FAST               6 (batch_ids)
-               
-                64         128 LOAD_GLOBAL              9 (NULL + select)
-                           140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                5 (model)
-                           152 PRECALL                  1
-                           156 CALL                     1
-                           166 LOAD_METHOD              6 (where)
-                           188 LOAD_FAST                0 (self)
-                           190 LOAD_ATTR                5 (model)
-                           200 LOAD_ATTR                7 (id)
-                           210 LOAD_METHOD              8 (in_)
-                           232 LOAD_FAST                6 (batch_ids)
-                           234 PRECALL                  1
-                           238 CALL                     1
-                           248 PRECALL                  1
-                           252 CALL                     1
-                           262 STORE_FAST               7 (statement)
-               
-                65         264 LOAD_FAST                3 (db_session)
-                           266 LOAD_METHOD              9 (exec)
-                           288 LOAD_FAST                7 (statement)
-                           290 PRECALL                  1
-                           294 CALL                     1
-                           304 LOAD_METHOD             10 (all)
-                           326 PRECALL                  0
-                           330 CALL                     0
-                           340 GET_AWAITABLE            0
-                           342 LOAD_CONST               0 (None)
-                       >>  344 SEND                     3 (to 352)
-                           346 YIELD_VALUE
-                           348 RESUME                   3
-                           350 JUMP_BACKWARD_NO_INTERRUPT     4 (to 344)
-                       >>  352 STORE_FAST               8 (results)
-               
-                66         354 LOAD_FAST                4 (result_set)
-                           356 LOAD_METHOD             11 (extend)
-                           378 LOAD_FAST                8 (results)
-                           380 PRECALL                  1
-                           384 CALL                     1
-                           394 POP_TOP
-                           396 JUMP_BACKWARD          150 (to 98)
-               
-                67     >>  398 LOAD_FAST                4 (result_set)
-                           400 RETURN_VALUE
-               consts
-                  None
-                  0
-               names      ('db', 'session', 'range', 'len', 'select', 'model', 'where', 'id', 'in_', 'exec', 'all', 'extend')
-               varnames   ('self', 'ids', 'batch_size', 'db_session', 'result_set', 'i', 'batch_ids', 'statement', 'results')
-               freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
-               name       'select_by_ids'
-               firstlineno 57
-               lnotab 0x06031c01040140011a0188015a012c01
+               firstlineno 66
+               lnotab 0x060b1c016a013601
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c01700b7c006a0000000000000000006a010000000000
                   0000007d017c01a002000000000000000000000000000000000000000074
                   07000000000000000000007409000000000000000000006a050000000000
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
                   00a006000000000000000000000000000000000000000074070000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   00a0080000000000000000000000000000000000000000a6000000ab0000
                   00000000000000a6010000ab010000000000000000a6010000ab01000000
-                  0000000000830064007b035600970386047d027c02a00900000000000000
+                  0000000000830064017b035600970386047d027c02a00900000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                69           0 RETURN_GENERATOR
+                82           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                70           6 LOAD_FAST                1 (db_session)
+                92           6 LOAD_FAST                1 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               1 (db_session)
                
-                71          34 LOAD_FAST                1 (db_session)
+                93          34 LOAD_FAST                1 (db_session)
                             36 LOAD_METHOD              2 (execute)
                
-                72          58 LOAD_GLOBAL              7 (NULL + select)
+                94          58 LOAD_GLOBAL              7 (NULL + select)
                             70 LOAD_GLOBAL              9 (NULL + func)
                             82 LOAD_ATTR                5 (count)
                             92 PRECALL                  0
                             96 CALL                     0
                            106 PRECALL                  1
                            110 CALL                     1
                            120 LOAD_METHOD              6 (select_from)
@@ -1010,509 +838,653 @@
                            170 CALL                     1
                            180 LOAD_METHOD              8 (subquery)
                            202 PRECALL                  0
                            206 CALL                     0
                            216 PRECALL                  1
                            220 CALL                     1
                
-                71         230 PRECALL                  1
+                93         230 PRECALL                  1
                            234 CALL                     1
                            244 GET_AWAITABLE            0
-                           246 LOAD_CONST               0 (None)
+                           246 LOAD_CONST               1 (None)
                        >>  248 SEND                     3 (to 256)
                            250 YIELD_VALUE
                            252 RESUME                   3
                            254 JUMP_BACKWARD_NO_INTERRUPT     4 (to 248)
                        >>  256 STORE_FAST               2 (response)
                
-                74         258 LOAD_FAST                2 (response)
+                96         258 LOAD_FAST                2 (response)
                            260 LOAD_METHOD              9 (scalar_one)
                            282 PRECALL                  0
                            286 CALL                     0
                            296 RETURN_VALUE
                consts
+                  '\n        Retrieves the total count of rows in the table.\n\n        Args:\n            db_session: The database session to use. If None, uses the default session.\n\n        Returns:\n            The total count of rows.\n        '
                   None
                names      ('db', 'session', 'execute', 'select', 'func', 'count', 'select_from', 'model', 'subquery', 'scalar_one')
                varnames   ('self', 'db_session', 'response')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_count'
-               firstlineno 69
-               lnotab 0x06011c011801acff1c03
+               firstlineno 82
+               lnotab 0x060a1c011801acff1c03
             1
             100
             ('page', 'size', 'db_session')
             'page'
             'size'
-            'query'
             code
                argcount  : 1
-               nlocals   : 6
-               stacksize : 4
-               flags     : 131
+               nlocals   : 9
+               stacksize : 7
+               flags     : 139
                code
-                  0x4b00010097007c04700b7c006a0000000000000000006a010000000000
-                  0000007d047c03805d7405000000000000000000007c006a030000000000
-                  000000a6010000ab010000000000000000a0040000000000000000000000
-                  0000000000000000007c0164017a0a00007c027a050000a6010000ab0100
-                  00000000000000a00500000000000000000000000000000000000000007c
-                  02a6010000ab010000000000000000a00600000000000000000000000000
-                  000000000000007c006a0300000000000000006a070000000000000000a6
-                  010000ab0100000000000000007d037c04a0080000000000000000000000
-                  0000000000000000007c03a6010000ab010000000000000000830064007b
-                  035600970386047d057c05a0090000000000000000000000000000000000
-                  000000a6000000ab000000000000000000a00a0000000000000000000000
+                  0x4b00010097007c03700b7c006a0000000000000000006a010000000000
+                  0000007d037405000000000000000000007c006a030000000000000000a6
+                  010000ab0100000000000000007d0564017c047600721402007c056a0400
+                  00000000000000640669007c04640119000000000000000000a4018e017d
+                  056e1f64027c047600721b7c05a005000000000000000000000000000000
+                  00000000007c04640219000000000000000000a6010000ab010000000000
+                  0000007d0564037c047600725b7c04640319000000000000000000a00600
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  00000044005d405c0200007d067d077c05a0050000000000000000000000
+                  000000000000000000740f000000000000000000007c006a030000000000
+                  0000007c06a6020000ab020000000000000000a008000000000000000000
+                  00000000000000000000007c07a6010000ab010000000000000000a60100
+                  00ab0100000000000000007d058c417c05a0090000000000000000000000
+                  0000000000000000007c0164047a0a00007c027a050000a6010000ab0100
+                  00000000000000a00a00000000000000000000000000000000000000007c
+                  02a6010000ab010000000000000000a00b00000000000000000000000000
+                  000000000000007c006a0300000000000000006a0c0000000000000000a6
+                  010000ab0100000000000000007d057c03a00d0000000000000000000000
+                  0000000000000000007c05a6010000ab010000000000000000830064057b
+                  035600970386047d087c08a00e0000000000000000000000000000000000
+                  000000a6000000ab000000000000000000a00f0000000000000000000000
                   000000000000000000a6000000ab0000000000000000005300
-                76           0 RETURN_GENERATOR
+                98           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                79           6 LOAD_FAST                4 (db_session)
+               113           6 LOAD_FAST                3 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               4 (db_session)
+                       >>   32 STORE_FAST               3 (db_session)
                
-                80          34 LOAD_FAST                3 (query)
-                            36 POP_JUMP_FORWARD_IF_NOT_NONE    93 (to 224)
+               114          34 LOAD_GLOBAL              5 (NULL + select)
+                            46 LOAD_FAST                0 (self)
+                            48 LOAD_ATTR                3 (model)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 STORE_FAST               5 (query)
                
-                82          38 LOAD_GLOBAL              5 (NULL + select)
-                            50 LOAD_FAST                0 (self)
-                            52 LOAD_ATTR                3 (model)
-                            62 PRECALL                  1
-                            66 CALL                     1
-               
-                83          76 LOAD_METHOD              4 (offset)
-                            98 LOAD_FAST                1 (page)
-                           100 LOAD_CONST               1 (1)
-                           102 BINARY_OP               10 (-)
-                           106 LOAD_FAST                2 (size)
-                           108 BINARY_OP                5 (*)
-                           112 PRECALL                  1
-                           116 CALL                     1
+               115          74 LOAD_CONST               1 ('filter_by')
+                            76 LOAD_FAST                4 (kwargs)
+                            78 CONTAINS_OP              0
+                            80 POP_JUMP_FORWARD_IF_FALSE    20 (to 122)
+               
+               116          82 PUSH_NULL
+                            84 LOAD_FAST                5 (query)
+                            86 LOAD_ATTR                4 (filter_by)
+                            96 LOAD_CONST               6 (())
+                            98 BUILD_MAP                0
+                           100 LOAD_FAST                4 (kwargs)
+                           102 LOAD_CONST               1 ('filter_by')
+                           104 BINARY_SUBSCR
+                           114 DICT_MERGE               1
+                           116 CALL_FUNCTION_EX         1
+                           118 STORE_FAST               5 (query)
+                           120 JUMP_FORWARD            31 (to 184)
+               
+               117     >>  122 LOAD_CONST               2 ('filter')
+                           124 LOAD_FAST                4 (kwargs)
+                           126 CONTAINS_OP              0
+                           128 POP_JUMP_FORWARD_IF_FALSE    27 (to 184)
+               
+               118         130 LOAD_FAST                5 (query)
+                           132 LOAD_METHOD              5 (filter)
+                           154 LOAD_FAST                4 (kwargs)
+                           156 LOAD_CONST               2 ('filter')
+                           158 BINARY_SUBSCR
+                           168 PRECALL                  1
+                           172 CALL                     1
+                           182 STORE_FAST               5 (query)
+               
+               119     >>  184 LOAD_CONST               3 ('like')
+                           186 LOAD_FAST                4 (kwargs)
+                           188 CONTAINS_OP              0
+                           190 POP_JUMP_FORWARD_IF_FALSE    91 (to 374)
+               
+               120         192 LOAD_FAST                4 (kwargs)
+                           194 LOAD_CONST               3 ('like')
+                           196 BINARY_SUBSCR
+                           206 LOAD_METHOD              6 (items)
+                           228 PRECALL                  0
+                           232 CALL                     0
+                           242 GET_ITER
+                       >>  244 FOR_ITER                64 (to 374)
+                           246 UNPACK_SEQUENCE          2
+                           250 STORE_FAST               6 (column)
+                           252 STORE_FAST               7 (value)
+               
+               121         254 LOAD_FAST                5 (query)
+                           256 LOAD_METHOD              5 (filter)
+                           278 LOAD_GLOBAL             15 (NULL + getattr)
+                           290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                3 (model)
+                           302 LOAD_FAST                6 (column)
+                           304 PRECALL                  2
+                           308 CALL                     2
+                           318 LOAD_METHOD              8 (like)
+                           340 LOAD_FAST                7 (value)
+                           342 PRECALL                  1
+                           346 CALL                     1
+                           356 PRECALL                  1
+                           360 CALL                     1
+                           370 STORE_FAST               5 (query)
+                           372 JUMP_BACKWARD           65 (to 244)
                
-                84         126 LOAD_METHOD              5 (limit)
-                           148 LOAD_FAST                2 (size)
-                           150 PRECALL                  1
-                           154 CALL                     1
-               
-                85         164 LOAD_METHOD              6 (order_by)
-                           186 LOAD_FAST                0 (self)
-                           188 LOAD_ATTR                3 (model)
-                           198 LOAD_ATTR                7 (id)
-                           208 PRECALL                  1
-                           212 CALL                     1
-               
-                81         222 STORE_FAST               3 (query)
-               
-                87     >>  224 LOAD_FAST                4 (db_session)
-                           226 LOAD_METHOD              8 (execute)
-                           248 LOAD_FAST                3 (query)
-                           250 PRECALL                  1
-                           254 CALL                     1
-                           264 GET_AWAITABLE            0
-                           266 LOAD_CONST               0 (None)
-                       >>  268 SEND                     3 (to 276)
-                           270 YIELD_VALUE
-                           272 RESUME                   3
-                           274 JUMP_BACKWARD_NO_INTERRUPT     4 (to 268)
-                       >>  276 STORE_FAST               5 (response)
-               
-                88         278 LOAD_FAST                5 (response)
-                           280 LOAD_METHOD              9 (scalars)
-                           302 PRECALL                  0
-                           306 CALL                     0
-                           316 LOAD_METHOD             10 (all)
-                           338 PRECALL                  0
-                           342 CALL                     0
-                           352 RETURN_VALUE
+               122     >>  374 LOAD_FAST                5 (query)
+                           376 LOAD_METHOD              9 (offset)
+                           398 LOAD_FAST                1 (page)
+                           400 LOAD_CONST               4 (1)
+                           402 BINARY_OP               10 (-)
+                           406 LOAD_FAST                2 (size)
+                           408 BINARY_OP                5 (*)
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 LOAD_METHOD             10 (limit)
+                           448 LOAD_FAST                2 (size)
+                           450 PRECALL                  1
+                           454 CALL                     1
+                           464 LOAD_METHOD             11 (order_by)
+                           486 LOAD_FAST                0 (self)
+                           488 LOAD_ATTR                3 (model)
+                           498 LOAD_ATTR               12 (id)
+                           508 PRECALL                  1
+                           512 CALL                     1
+                           522 STORE_FAST               5 (query)
+               
+               123         524 LOAD_FAST                3 (db_session)
+                           526 LOAD_METHOD             13 (execute)
+                           548 LOAD_FAST                5 (query)
+                           550 PRECALL                  1
+                           554 CALL                     1
+                           564 GET_AWAITABLE            0
+                           566 LOAD_CONST               5 (None)
+                       >>  568 SEND                     3 (to 576)
+                           570 YIELD_VALUE
+                           572 RESUME                   3
+                           574 JUMP_BACKWARD_NO_INTERRUPT     4 (to 568)
+                       >>  576 STORE_FAST               8 (response)
+               
+               124         578 LOAD_FAST                8 (response)
+                           580 LOAD_METHOD             14 (scalars)
+                           602 PRECALL                  0
+                           606 CALL                     0
+                           616 LOAD_METHOD             15 (all)
+                           638 PRECALL                  0
+                           642 CALL                     0
+                           652 RETURN_VALUE
                consts
-                  None
+                  '\n        Retrieves a list of rows, with optional filtering and pagination.\n\n        Args:\n            page: The page number to retrieve (1-indexed).\n            size: The number of rows per page.\n            db_session: The database session to use. If None, uses the default session.\n            **kwargs: Additional filter criteria, such as `filter_by` or `like`.\n\n        Returns:\n            A list of retrieved rows.\n        '
+                  'filter_by'
+                  'filter'
+                  'like'
                   1
-               names      ('db', 'session', 'select', 'model', 'offset', 'limit', 'order_by', 'id', 'execute', 'scalars', 'all')
-               varnames   ('self', 'page', 'size', 'query', 'db_session', 'response')
+                  None
+                  ()
+               names      ('db', 'session', 'select', 'model', 'filter_by', 'filter', 'items', 'getattr', 'like', 'offset', 'limit', 'order_by', 'id', 'execute', 'scalars', 'all')
+               varnames   ('self', 'page', 'size', 'db_session', 'kwargs', 'query', 'column', 'value', 'response')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list'
-               firstlineno 76
-               lnotab 0x06031c0104022601320126013afc02063601
+               firstlineno 98
+               lnotab 0x060f1c012801080128010801360108013e01780196013601
+            ('page', 'size', 'order_by', 'sort_order', 'db_session')
             'order_by'
             'sort_order'
             code
                argcount  : 1
-               nlocals   : 9
-               stacksize : 4
-               flags     : 131
+               nlocals   : 12
+               stacksize : 7
+               flags     : 139
                code
-                  0x4b00010097007c06700b7c006a0000000000000000006a010000000000
-                  0000007d067c006a0200000000000000006a0300000000000000006a0400
-                  000000000000007d077c0481047c047c077601720264017d047c05740a00
-                  0000000000000000006a0600000000000000006b0200000000726c740f00
-                  0000000000000000007c006a020000000000000000a6010000ab01000000
-                  0000000000a00800000000000000000000000000000000000000007c0164
-                  027a0a00007c027a050000a6010000ab010000000000000000a009000000
-                  00000000000000000000000000000000007c02a6010000ab010000000000
-                  000000a00a00000000000000000000000000000000000000007c077c0419
-                  000000000000000000a00b00000000000000000000000000000000000000
-                  00a6000000ab000000000000000000a6010000ab0100000000000000007d
-                  036e6b740f000000000000000000007c006a020000000000000000a60100
-                  00ab010000000000000000a0080000000000000000000000000000000000
-                  0000007c0164027a0a00007c027a050000a6010000ab0100000000000000
-                  00a00900000000000000000000000000000000000000007c02a6010000ab
-                  010000000000000000a00a00000000000000000000000000000000000000
-                  007c077c0419000000000000000000a00c00000000000000000000000000
-                  00000000000000a6000000ab000000000000000000a6010000ab01000000
-                  00000000007d037c06a00d00000000000000000000000000000000000000
-                  007c03a6010000ab010000000000000000830064007b035600970386047d
-                  087c08a00e0000000000000000000000000000000000000000a6000000ab
-                  000000000000000000a00f00000000000000000000000000000000000000
-                  00a6000000ab0000000000000000005300
-                90           0 RETURN_GENERATOR
+                  0x4b00010097007c05700b7c006a0000000000000000006a010000000000
+                  0000007d057405000000000000000000007c006a030000000000000000a6
+                  010000ab0100000000000000007d0764017c067600721402007c076a0400
+                  00000000000000640769007c06640119000000000000000000a4018e017d
+                  076e1f64027c067600721b7c07a005000000000000000000000000000000
+                  00000000007c06640219000000000000000000a6010000ab010000000000
+                  0000007d0764037c067600725b7c06640319000000000000000000a00600
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  00000044005d405c0200007d087d097c07a0050000000000000000000000
+                  000000000000000000740f000000000000000000007c006a030000000000
+                  0000007c08a6020000ab020000000000000000a008000000000000000000
+                  00000000000000000000007c09a6010000ab010000000000000000a60100
+                  00ab0100000000000000007d078c417c006a0300000000000000006a0900
+                  000000000000006a0a00000000000000007d0a7c0381047c037c0a760172
+                  0264057d037c0481107c047416000000000000000000006a0c0000000000
+                  0000006b0200000000725a7c07a00d000000000000000000000000000000
+                  00000000007c0164067a0a00007c027a050000a6010000ab010000000000
+                  000000a00e00000000000000000000000000000000000000007c02a60100
+                  00ab010000000000000000a00f0000000000000000000000000000000000
+                  0000007c0a7c0319000000000000000000a0100000000000000000000000
+                  000000000000000000a6000000ab000000000000000000a6010000ab0100
+                  000000000000007d076e597c07a00d000000000000000000000000000000
+                  00000000007c0164067a0a00007c027a050000a6010000ab010000000000
+                  000000a00e00000000000000000000000000000000000000007c02a60100
+                  00ab010000000000000000a00f0000000000000000000000000000000000
+                  0000007c0a7c0319000000000000000000a0110000000000000000000000
+                  000000000000000000a6000000ab000000000000000000a6010000ab0100
+                  000000000000007d077c05a0120000000000000000000000000000000000
+                  0000007c07a6010000ab010000000000000000830064047b035600970386
+                  047d0b7c0ba0130000000000000000000000000000000000000000a60000
+                  00ab000000000000000000a0140000000000000000000000000000000000
+                  000000a6000000ab0000000000000000005300
+               126           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               100           6 LOAD_FAST                6 (db_session)
+               147           6 LOAD_FAST                5 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               6 (db_session)
-               
-               101          34 LOAD_FAST                0 (self)
-                            36 LOAD_ATTR                2 (model)
-                            46 LOAD_ATTR                3 (__table__)
-                            56 LOAD_ATTR                4 (columns)
-                            66 STORE_FAST               7 (columns)
-               
-               102          68 LOAD_FAST                4 (order_by)
-                            70 POP_JUMP_FORWARD_IF_NONE     4 (to 80)
-                            72 LOAD_FAST                4 (order_by)
-                            74 LOAD_FAST                7 (columns)
-                            76 CONTAINS_OP              1
-                            78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
-               
-               103     >>   80 LOAD_CONST               1 ('id')
-                            82 STORE_FAST               4 (order_by)
-               
-               104     >>   84 LOAD_FAST                5 (sort_order)
-                            86 LOAD_GLOBAL             10 (SortEnum)
-                            98 LOAD_ATTR                6 (ascending)
-                           108 COMPARE_OP               2 (==)
-                           114 POP_JUMP_FORWARD_IF_FALSE   108 (to 332)
+                       >>   32 STORE_FAST               5 (db_session)
                
-               106         116 LOAD_GLOBAL             15 (NULL + select)
-                           128 LOAD_FAST                0 (self)
-                           130 LOAD_ATTR                2 (model)
-                           140 PRECALL                  1
-                           144 CALL                     1
+               148          34 LOAD_GLOBAL              5 (NULL + select)
+                            46 LOAD_FAST                0 (self)
+                            48 LOAD_ATTR                3 (model)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 STORE_FAST               7 (query)
                
-               107         154 LOAD_METHOD              8 (offset)
-                           176 LOAD_FAST                1 (page)
-                           178 LOAD_CONST               2 (1)
-                           180 BINARY_OP               10 (-)
-                           184 LOAD_FAST                2 (size)
-                           186 BINARY_OP                5 (*)
-                           190 PRECALL                  1
-                           194 CALL                     1
-               
-               108         204 LOAD_METHOD              9 (limit)
-                           226 LOAD_FAST                2 (size)
-                           228 PRECALL                  1
-                           232 CALL                     1
-               
-               109         242 LOAD_METHOD             10 (order_by)
-                           264 LOAD_FAST                7 (columns)
-                           266 LOAD_FAST                4 (order_by)
-                           268 BINARY_SUBSCR
-                           278 LOAD_METHOD             11 (asc)
-                           300 PRECALL                  0
-                           304 CALL                     0
-                           314 PRECALL                  1
-                           318 CALL                     1
-               
-               105         328 STORE_FAST               3 (query)
-                           330 JUMP_FORWARD           107 (to 546)
-               
-               113     >>  332 LOAD_GLOBAL             15 (NULL + select)
-                           344 LOAD_FAST                0 (self)
-                           346 LOAD_ATTR                2 (model)
+               149          74 LOAD_CONST               1 ('filter_by')
+                            76 LOAD_FAST                6 (kwargs)
+                            78 CONTAINS_OP              0
+                            80 POP_JUMP_FORWARD_IF_FALSE    20 (to 122)
+               
+               150          82 PUSH_NULL
+                            84 LOAD_FAST                7 (query)
+                            86 LOAD_ATTR                4 (filter_by)
+                            96 LOAD_CONST               7 (())
+                            98 BUILD_MAP                0
+                           100 LOAD_FAST                6 (kwargs)
+                           102 LOAD_CONST               1 ('filter_by')
+                           104 BINARY_SUBSCR
+                           114 DICT_MERGE               1
+                           116 CALL_FUNCTION_EX         1
+                           118 STORE_FAST               7 (query)
+                           120 JUMP_FORWARD            31 (to 184)
+               
+               151     >>  122 LOAD_CONST               2 ('filter')
+                           124 LOAD_FAST                6 (kwargs)
+                           126 CONTAINS_OP              0
+                           128 POP_JUMP_FORWARD_IF_FALSE    27 (to 184)
+               
+               152         130 LOAD_FAST                7 (query)
+                           132 LOAD_METHOD              5 (filter)
+                           154 LOAD_FAST                6 (kwargs)
+                           156 LOAD_CONST               2 ('filter')
+                           158 BINARY_SUBSCR
+                           168 PRECALL                  1
+                           172 CALL                     1
+                           182 STORE_FAST               7 (query)
+               
+               153     >>  184 LOAD_CONST               3 ('like')
+                           186 LOAD_FAST                6 (kwargs)
+                           188 CONTAINS_OP              0
+                           190 POP_JUMP_FORWARD_IF_FALSE    91 (to 374)
+               
+               154         192 LOAD_FAST                6 (kwargs)
+                           194 LOAD_CONST               3 ('like')
+                           196 BINARY_SUBSCR
+                           206 LOAD_METHOD              6 (items)
+                           228 PRECALL                  0
+                           232 CALL                     0
+                           242 GET_ITER
+                       >>  244 FOR_ITER                64 (to 374)
+                           246 UNPACK_SEQUENCE          2
+                           250 STORE_FAST               8 (column)
+                           252 STORE_FAST               9 (value)
+               
+               155         254 LOAD_FAST                7 (query)
+                           256 LOAD_METHOD              5 (filter)
+                           278 LOAD_GLOBAL             15 (NULL + getattr)
+                           290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                3 (model)
+                           302 LOAD_FAST                8 (column)
+                           304 PRECALL                  2
+                           308 CALL                     2
+                           318 LOAD_METHOD              8 (like)
+                           340 LOAD_FAST                9 (value)
+                           342 PRECALL                  1
+                           346 CALL                     1
                            356 PRECALL                  1
                            360 CALL                     1
+                           370 STORE_FAST               7 (query)
+                           372 JUMP_BACKWARD           65 (to 244)
                
-               114         370 LOAD_METHOD              8 (offset)
-                           392 LOAD_FAST                1 (page)
-                           394 LOAD_CONST               2 (1)
-                           396 BINARY_OP               10 (-)
-                           400 LOAD_FAST                2 (size)
-                           402 BINARY_OP                5 (*)
-                           406 PRECALL                  1
-                           410 CALL                     1
-               
-               115         420 LOAD_METHOD              9 (limit)
-                           442 LOAD_FAST                2 (size)
-                           444 PRECALL                  1
-                           448 CALL                     1
-               
-               116         458 LOAD_METHOD             10 (order_by)
-                           480 LOAD_FAST                7 (columns)
-                           482 LOAD_FAST                4 (order_by)
-                           484 BINARY_SUBSCR
-                           494 LOAD_METHOD             12 (desc)
-                           516 PRECALL                  0
-                           520 CALL                     0
-                           530 PRECALL                  1
-                           534 CALL                     1
-               
-               112         544 STORE_FAST               3 (query)
-               
-               118     >>  546 LOAD_FAST                6 (db_session)
-                           548 LOAD_METHOD             13 (execute)
-                           570 LOAD_FAST                3 (query)
-                           572 PRECALL                  1
-                           576 CALL                     1
-                           586 GET_AWAITABLE            0
-                           588 LOAD_CONST               0 (None)
-                       >>  590 SEND                     3 (to 598)
-                           592 YIELD_VALUE
-                           594 RESUME                   3
-                           596 JUMP_BACKWARD_NO_INTERRUPT     4 (to 590)
-                       >>  598 STORE_FAST               8 (response)
-               
-               119         600 LOAD_FAST                8 (response)
-                           602 LOAD_METHOD             14 (scalars)
-                           624 PRECALL                  0
-                           628 CALL                     0
-                           638 LOAD_METHOD             15 (all)
-                           660 PRECALL                  0
-                           664 CALL                     0
-                           674 RETURN_VALUE
+               156     >>  374 LOAD_FAST                0 (self)
+                           376 LOAD_ATTR                3 (model)
+                           386 LOAD_ATTR                9 (__table__)
+                           396 LOAD_ATTR               10 (columns)
+                           406 STORE_FAST              10 (columns)
+               
+               157         408 LOAD_FAST                3 (order_by)
+                           410 POP_JUMP_FORWARD_IF_NONE     4 (to 420)
+                           412 LOAD_FAST                3 (order_by)
+                           414 LOAD_FAST               10 (columns)
+                           416 CONTAINS_OP              1
+                           418 POP_JUMP_FORWARD_IF_FALSE     2 (to 424)
+               
+               158     >>  420 LOAD_CONST               5 ('id')
+                           422 STORE_FAST               3 (order_by)
+               
+               159     >>  424 LOAD_FAST                4 (sort_order)
+                           426 POP_JUMP_FORWARD_IF_NONE    16 (to 460)
+                           428 LOAD_FAST                4 (sort_order)
+                           430 LOAD_GLOBAL             22 (SortEnum)
+                           442 LOAD_ATTR               12 (ascending)
+                           452 COMPARE_OP               2 (==)
+                           458 POP_JUMP_FORWARD_IF_FALSE    90 (to 640)
+               
+               161     >>  460 LOAD_FAST                7 (query)
+                           462 LOAD_METHOD             13 (offset)
+                           484 LOAD_FAST                1 (page)
+                           486 LOAD_CONST               6 (1)
+                           488 BINARY_OP               10 (-)
+                           492 LOAD_FAST                2 (size)
+                           494 BINARY_OP                5 (*)
+                           498 PRECALL                  1
+                           502 CALL                     1
+               
+               162         512 LOAD_METHOD             14 (limit)
+                           534 LOAD_FAST                2 (size)
+                           536 PRECALL                  1
+                           540 CALL                     1
+               
+               163         550 LOAD_METHOD             15 (order_by)
+                           572 LOAD_FAST               10 (columns)
+                           574 LOAD_FAST                3 (order_by)
+                           576 BINARY_SUBSCR
+                           586 LOAD_METHOD             16 (asc)
+                           608 PRECALL                  0
+                           612 CALL                     0
+                           622 PRECALL                  1
+                           626 CALL                     1
+               
+               160         636 STORE_FAST               7 (query)
+                           638 JUMP_FORWARD            89 (to 818)
+               
+               167     >>  640 LOAD_FAST                7 (query)
+                           642 LOAD_METHOD             13 (offset)
+                           664 LOAD_FAST                1 (page)
+                           666 LOAD_CONST               6 (1)
+                           668 BINARY_OP               10 (-)
+                           672 LOAD_FAST                2 (size)
+                           674 BINARY_OP                5 (*)
+                           678 PRECALL                  1
+                           682 CALL                     1
+               
+               168         692 LOAD_METHOD             14 (limit)
+                           714 LOAD_FAST                2 (size)
+                           716 PRECALL                  1
+                           720 CALL                     1
+               
+               169         730 LOAD_METHOD             15 (order_by)
+                           752 LOAD_FAST               10 (columns)
+                           754 LOAD_FAST                3 (order_by)
+                           756 BINARY_SUBSCR
+                           766 LOAD_METHOD             17 (des)
+                           788 PRECALL                  0
+                           792 CALL                     0
+                           802 PRECALL                  1
+                           806 CALL                     1
+               
+               166         816 STORE_FAST               7 (query)
+               
+               171     >>  818 LOAD_FAST                5 (db_session)
+                           820 LOAD_METHOD             18 (execute)
+                           842 LOAD_FAST                7 (query)
+                           844 PRECALL                  1
+                           848 CALL                     1
+                           858 GET_AWAITABLE            0
+                           860 LOAD_CONST               4 (None)
+                       >>  862 SEND                     3 (to 870)
+                           864 YIELD_VALUE
+                           866 RESUME                   3
+                           868 JUMP_BACKWARD_NO_INTERRUPT     4 (to 862)
+                       >>  870 STORE_FAST              11 (response)
+               
+               172         872 LOAD_FAST               11 (response)
+                           874 LOAD_METHOD             19 (scalars)
+                           896 PRECALL                  0
+                           900 CALL                     0
+                           910 LOAD_METHOD             20 (all)
+                           932 PRECALL                  0
+                           936 CALL                     0
+                           946 RETURN_VALUE
                consts
+                  '\n        Retrieve a list of rows, with optional filtering, pagination, and ordering.\n\n        Parameters:\n            page : The page number to retrieve (1-indexed)\n            size : The number of rows per page\n            order_by : The column to order by\n            sort_order : The sort order (ascending or descending)\n            db_session : The database session to use\n            **kwargs: Additional filter criteria\n        '
+                  'filter_by'
+                  'filter'
+                  'like'
                   None
                   'id'
                   1
-               names      ('db', 'session', 'model', '__table__', 'columns', 'SortEnum', 'ascending', 'select', 'offset', 'limit', 'order_by', 'asc', 'desc', 'execute', 'scalars', 'all')
-               varnames   ('self', 'page', 'size', 'query', 'order_by', 'sort_order', 'db_session', 'columns', 'response')
+                  ()
+               names      ('db', 'session', 'select', 'model', 'filter_by', 'filter', 'items', 'getattr', 'like', '__table__', 'columns', 'SortEnum', 'ascending', 'offset', 'limit', 'order_by', 'asc', 'des', 'execute', 'scalars', 'all')
+               varnames   ('self', 'page', 'size', 'order_by', 'sort_order', 'db_session', 'kwargs', 'query', 'column', 'value', 'columns', 'response')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list_ordered'
-               firstlineno 90
+               firstlineno 126
                lnotab
-                  0x060a1c0122010c010401200226013201260156fc040826013201260156
-                  fc02063601
+                  0x06151c012801080128010801360108013e01780122010c010401240234
+                  01260156fd04073401260156fd02053601
             'params'
             code
                argcount  : 1
-               nlocals   : 5
+               nlocals   : 4
                stacksize : 5
                flags     : 131
                code
-                  0x4b00010097007c03700b7c006a0000000000000000006a010000000000
-                  0000007d037c0280147405000000000000000000007c006a030000000000
-                  000000a6010000ab0100000000000000007d027409000000000000000000
-                  007c037c027c01a6030000ab030000000000000000830064007b03560097
-                  0386047d047c045300
-               121           0 RETURN_GENERATOR
+                  0x4b00010097007c02700b7c006a0000000000000000006a010000000000
+                  0000007d027405000000000000000000007c006a030000000000000000a6
+                  010000ab0100000000000000007d037409000000000000000000007c027c
+                  037c01a6030000ab030000000000000000830064017b0356009703860453
+                  00
+               174           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               124           6 LOAD_FAST                3 (db_session)
+               182           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               3 (db_session)
-               
-               125          34 LOAD_FAST                2 (query)
-                            36 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 78)
+                       >>   32 STORE_FAST               2 (db_session)
                
-               126          38 LOAD_GLOBAL              5 (NULL + select)
-                            50 LOAD_FAST                0 (self)
-                            52 LOAD_ATTR                3 (model)
-                            62 PRECALL                  1
-                            66 CALL                     1
-                            76 STORE_FAST               2 (query)
-               
-               127     >>   78 LOAD_GLOBAL              9 (NULL + paginate)
-                            90 LOAD_FAST                3 (db_session)
-                            92 LOAD_FAST                2 (query)
-                            94 LOAD_FAST                1 (params)
-                            96 PRECALL                  3
-                           100 CALL                     3
-                           110 GET_AWAITABLE            0
-                           112 LOAD_CONST               0 (None)
-                       >>  114 SEND                     3 (to 122)
-                           116 YIELD_VALUE
-                           118 RESUME                   3
-                           120 JUMP_BACKWARD_NO_INTERRUPT     4 (to 114)
-                       >>  122 STORE_FAST               4 (response)
+               183          34 LOAD_GLOBAL              5 (NULL + select)
+                            46 LOAD_FAST                0 (self)
+                            48 LOAD_ATTR                3 (model)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 STORE_FAST               3 (query)
                
-               128         124 LOAD_FAST                4 (response)
-                           126 RETURN_VALUE
+               184          74 LOAD_GLOBAL              9 (NULL + paginate)
+                            86 LOAD_FAST                2 (db_session)
+                            88 LOAD_FAST                3 (query)
+                            90 LOAD_FAST                1 (params)
+                            92 PRECALL                  3
+                            96 CALL                     3
+                           106 GET_AWAITABLE            0
+                           108 LOAD_CONST               1 (None)
+                       >>  110 SEND                     3 (to 118)
+                           112 YIELD_VALUE
+                           114 RESUME                   3
+                           116 JUMP_BACKWARD_NO_INTERRUPT     4 (to 110)
+                       >>  118 RETURN_VALUE
                consts
+                  '\n        Retrieve a page of rows, with optional filtering and pagination.\n\n        Parameters:\n            params : The pagination parameters\n            db_session : The database session to use\n        '
                   None
                names      ('db', 'session', 'select', 'model', 'paginate')
-               varnames   ('self', 'params', 'query', 'db_session', 'response')
+               varnames   ('self', 'params', 'db_session', 'query')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
-               name       'select_list_page'
-               firstlineno 121
-               lnotab 0x06031c01040128012e01
-            ('query', 'order_by', 'sort_order', 'db_session')
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
+               name       'select_page'
+               firstlineno 174
+               lnotab 0x06081c012801
+            ('order_by', 'sort_order', 'db_session')
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 5
                flags     : 131
                code
-                  0x4b00010097007c05700b7c006a0000000000000000006a010000000000
-                  0000007d057c006a0200000000000000006a0300000000000000006a0400
-                  000000000000007d067c0381047c037c067601720264017d037c02808f7c
-                  04740a000000000000000000006a0600000000000000006b020000000072
-                  40740f000000000000000000007c006a020000000000000000a6010000ab
-                  010000000000000000a00800000000000000000000000000000000000000
-                  007c067c0319000000000000000000a00900000000000000000000000000
-                  00000000000000a6000000ab000000000000000000a6010000ab01000000
-                  00000000007d026e3f740f000000000000000000007c006a020000000000
-                  000000a6010000ab010000000000000000a0080000000000000000000000
-                  0000000000000000007c067c0319000000000000000000a00a0000000000
-                  000000000000000000000000000000a6000000ab000000000000000000a6
-                  010000ab0100000000000000007d027417000000000000000000007c057c
-                  027c01a6030000ab030000000000000000830064007b0356009703860453
-                  00
-               130           0 RETURN_GENERATOR
+                  0x4b00010097007c04700b7c006a0000000000000000006a010000000000
+                  0000007d047c006a0200000000000000006a0300000000000000006a0400
+                  000000000000007d057c0281047c027c057601720264027d027c03740a00
+                  0000000000000000006a0600000000000000006b02000000007240740f00
+                  0000000000000000007c006a020000000000000000a6010000ab01000000
+                  0000000000a00800000000000000000000000000000000000000007c057c
+                  0219000000000000000000a0090000000000000000000000000000000000
+                  000000a6000000ab000000000000000000a6010000ab0100000000000000
+                  007d066e3f740f000000000000000000007c006a020000000000000000a6
+                  010000ab010000000000000000a008000000000000000000000000000000
+                  00000000007c057c0219000000000000000000a00a000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a6010000ab
+                  0100000000000000007d067417000000000000000000007c047c067c01a6
+                  030000ab030000000000000000830064017b035600970386045300
+               186           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               139           6 LOAD_FAST                5 (db_session)
+               203           6 LOAD_FAST                4 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               5 (db_session)
+                       >>   32 STORE_FAST               4 (db_session)
                
-               140          34 LOAD_FAST                0 (self)
+               204          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (model)
                             46 LOAD_ATTR                3 (__table__)
                             56 LOAD_ATTR                4 (columns)
-                            66 STORE_FAST               6 (columns)
+                            66 STORE_FAST               5 (columns)
                
-               141          68 LOAD_FAST                3 (order_by)
+               205          68 LOAD_FAST                2 (order_by)
                             70 POP_JUMP_FORWARD_IF_NONE     4 (to 80)
-                            72 LOAD_FAST                3 (order_by)
-                            74 LOAD_FAST                6 (columns)
+                            72 LOAD_FAST                2 (order_by)
+                            74 LOAD_FAST                5 (columns)
                             76 CONTAINS_OP              1
                             78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
                
-               142     >>   80 LOAD_CONST               1 ('id')
-                            82 STORE_FAST               3 (order_by)
-               
-               143     >>   84 LOAD_FAST                2 (query)
-                            86 POP_JUMP_FORWARD_IF_NOT_NONE   143 (to 374)
+               206     >>   80 LOAD_CONST               2 ('id')
+                            82 STORE_FAST               2 (order_by)
                
-               144          88 LOAD_FAST                4 (sort_order)
-                            90 LOAD_GLOBAL             10 (SortEnum)
-                           102 LOAD_ATTR                6 (ascending)
-                           112 COMPARE_OP               2 (==)
-                           118 POP_JUMP_FORWARD_IF_FALSE    64 (to 248)
-               
-               145         120 LOAD_GLOBAL             15 (NULL + select)
-                           132 LOAD_FAST                0 (self)
-                           134 LOAD_ATTR                2 (model)
-                           144 PRECALL                  1
-                           148 CALL                     1
-                           158 LOAD_METHOD              8 (order_by)
-                           180 LOAD_FAST                6 (columns)
-                           182 LOAD_FAST                3 (order_by)
-                           184 BINARY_SUBSCR
-                           194 LOAD_METHOD              9 (asc)
-                           216 PRECALL                  0
-                           220 CALL                     0
-                           230 PRECALL                  1
-                           234 CALL                     1
-                           244 STORE_FAST               2 (query)
-                           246 JUMP_FORWARD            63 (to 374)
+               207     >>   84 LOAD_FAST                3 (sort_order)
+                            86 LOAD_GLOBAL             10 (SortEnum)
+                            98 LOAD_ATTR                6 (ascending)
+                           108 COMPARE_OP               2 (==)
+                           114 POP_JUMP_FORWARD_IF_FALSE    64 (to 244)
                
-               147     >>  248 LOAD_GLOBAL             15 (NULL + select)
-                           260 LOAD_FAST                0 (self)
-                           262 LOAD_ATTR                2 (model)
-                           272 PRECALL                  1
-                           276 CALL                     1
-                           286 LOAD_METHOD              8 (order_by)
-                           308 LOAD_FAST                6 (columns)
-                           310 LOAD_FAST                3 (order_by)
-                           312 BINARY_SUBSCR
-                           322 LOAD_METHOD             10 (desc)
-                           344 PRECALL                  0
-                           348 CALL                     0
-                           358 PRECALL                  1
-                           362 CALL                     1
-                           372 STORE_FAST               2 (query)
-               
-               148     >>  374 LOAD_GLOBAL             23 (NULL + paginate)
-                           386 LOAD_FAST                5 (db_session)
-                           388 LOAD_FAST                2 (query)
-                           390 LOAD_FAST                1 (params)
-                           392 PRECALL                  3
-                           396 CALL                     3
-                           406 GET_AWAITABLE            0
-                           408 LOAD_CONST               0 (None)
-                       >>  410 SEND                     3 (to 418)
-                           412 YIELD_VALUE
-                           414 RESUME                   3
-                           416 JUMP_BACKWARD_NO_INTERRUPT     4 (to 410)
-                       >>  418 RETURN_VALUE
+               208         116 LOAD_GLOBAL             15 (NULL + select)
+                           128 LOAD_FAST                0 (self)
+                           130 LOAD_ATTR                2 (model)
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 LOAD_METHOD              8 (order_by)
+                           176 LOAD_FAST                5 (columns)
+                           178 LOAD_FAST                2 (order_by)
+                           180 BINARY_SUBSCR
+                           190 LOAD_METHOD              9 (asc)
+                           212 PRECALL                  0
+                           216 CALL                     0
+                           226 PRECALL                  1
+                           230 CALL                     1
+                           240 STORE_FAST               6 (query)
+                           242 JUMP_FORWARD            63 (to 370)
+               
+               210     >>  244 LOAD_GLOBAL             15 (NULL + select)
+                           256 LOAD_FAST                0 (self)
+                           258 LOAD_ATTR                2 (model)
+                           268 PRECALL                  1
+                           272 CALL                     1
+                           282 LOAD_METHOD              8 (order_by)
+                           304 LOAD_FAST                5 (columns)
+                           306 LOAD_FAST                2 (order_by)
+                           308 BINARY_SUBSCR
+                           318 LOAD_METHOD             10 (desc)
+                           340 PRECALL                  0
+                           344 CALL                     0
+                           354 PRECALL                  1
+                           358 CALL                     1
+                           368 STORE_FAST               6 (query)
+               
+               211     >>  370 LOAD_GLOBAL             23 (NULL + paginate)
+                           382 LOAD_FAST                4 (db_session)
+                           384 LOAD_FAST                6 (query)
+                           386 LOAD_FAST                1 (params)
+                           388 PRECALL                  3
+                           392 CALL                     3
+                           402 GET_AWAITABLE            0
+                           404 LOAD_CONST               1 (None)
+                       >>  406 SEND                     3 (to 414)
+                           408 YIELD_VALUE
+                           410 RESUME                   3
+                           412 JUMP_BACKWARD_NO_INTERRUPT     4 (to 406)
+                       >>  414 RETURN_VALUE
                consts
+                  '\n        Retrieve a page of rows, with optional filtering, pagination, and ordering.\n\n        Parameters:\n            params : The pagination parameters\n            order_by : The column to order by\n            sort_order : The sort order (ascending or descending)\n            db_session : The database session to use\n        '
                   None
                   'id'
                names      ('db', 'session', 'model', '__table__', 'columns', 'SortEnum', 'ascending', 'select', 'order_by', 'asc', 'desc', 'paginate')
-               varnames   ('self', 'params', 'query', 'order_by', 'sort_order', 'db_session', 'columns')
+               varnames   ('self', 'params', 'order_by', 'sort_order', 'db_session', 'columns', 'query')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
-               name       'select_list_page_ordered'
-               firstlineno 130
-               lnotab 0x06091c0122010c0104010401200180027e01
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
+               name       'select_page_ordered'
+               firstlineno 186
+               lnotab 0x06111c0122010c010401200180027e01
             code
                argcount  : 1
-               nlocals   : 8
-               stacksize : 7
+               nlocals   : 6
+               stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a0500000000000000007c016a
                   0500000000000000006b0200000000a6010000ab0100000000000000007d
-                  037c02a00600000000000000000000000000000000000000007c03a60100
-                  00ab010000000000000000830064007b035600970386047d047c04800264
-                  0153007c04a0070000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d057411000000000000000000007c01741200
-                  000000000000000000a6020000ab02000000000000000072037c017d066e
-                  167c01a00a00000000000000000000000000000000000000006402ac03a6
-                  010000ab0100000000000000007d067c0644005d197d0774170000000000
-                  00000000007c057c077c067c0719000000000000000000a6030000ab0300
-                  0000000000000001008c1a7c02a00c000000000000000000000000000000
-                  00000000007c05a6010000ab01000000000000000001007c055300
-               150           0 RETURN_GENERATOR
+                  037c01a00600000000000000000000000000000000000000006401ac02a6
+                  010000ab0100000000000000007d0402007c036a07000000000000000064
+                  0469007c04a4018e017d037c02a008000000000000000000000000000000
+                  00000000007c03a6010000ab010000000000000000830064037b03560097
+                  0386047d057c056a0900000000000000005300
+               213           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               151           6 LOAD_FAST                2 (db_session)
+               221           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               152          34 LOAD_GLOBAL              5 (NULL + select)
+               222          34 LOAD_GLOBAL              5 (NULL + update)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
@@ -1520,313 +1492,295 @@
                            116 LOAD_FAST                1 (data)
                            118 LOAD_ATTR                5 (id)
                            128 COMPARE_OP               2 (==)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               3 (query)
                
-               153         150 LOAD_FAST                2 (db_session)
-                           152 LOAD_METHOD              6 (execute)
-                           174 LOAD_FAST                3 (query)
-                           176 PRECALL                  1
-                           180 CALL                     1
-                           190 GET_AWAITABLE            0
-                           192 LOAD_CONST               0 (None)
-                       >>  194 SEND                     3 (to 202)
-                           196 YIELD_VALUE
-                           198 RESUME                   3
-                           200 JUMP_BACKWARD_NO_INTERRUPT     4 (to 194)
-                       >>  202 STORE_FAST               4 (result)
-               
-               154         204 LOAD_FAST                4 (result)
-                           206 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 212)
-               
-               155         208 LOAD_CONST               1 (0)
-                           210 RETURN_VALUE
-               
-               156     >>  212 LOAD_FAST                4 (result)
-                           214 LOAD_METHOD              7 (scalar_one)
-                           236 PRECALL                  0
-                           240 CALL                     0
-                           250 STORE_FAST               5 (db_data)
-               
-               157         252 LOAD_GLOBAL             17 (NULL + isinstance)
-                           264 LOAD_FAST                1 (data)
-                           266 LOAD_GLOBAL             18 (dict)
-                           278 PRECALL                  2
-                           282 CALL                     2
-                           292 POP_JUMP_FORWARD_IF_FALSE     3 (to 300)
-               
-               158         294 LOAD_FAST                1 (data)
-                           296 STORE_FAST               6 (update_data)
-                           298 JUMP_FORWARD            22 (to 344)
-               
-               160     >>  300 LOAD_FAST                1 (data)
-                           302 LOAD_METHOD             10 (model_dump)
-                           324 LOAD_CONST               2 (True)
-                           326 KW_NAMES                 3
-                           328 PRECALL                  1
-                           332 CALL                     1
-                           342 STORE_FAST               6 (update_data)
-               
-               161     >>  344 LOAD_FAST                6 (update_data)
-                           346 GET_ITER
-                       >>  348 FOR_ITER                25 (to 400)
-                           350 STORE_FAST               7 (field)
-               
-               162         352 LOAD_GLOBAL             23 (NULL + setattr)
-                           364 LOAD_FAST                5 (db_data)
-                           366 LOAD_FAST                7 (field)
-                           368 LOAD_FAST                6 (update_data)
-                           370 LOAD_FAST                7 (field)
-                           372 BINARY_SUBSCR
-                           382 PRECALL                  3
-                           386 CALL                     3
-                           396 POP_TOP
-                           398 JUMP_BACKWARD           26 (to 348)
-               
-               164     >>  400 LOAD_FAST                2 (db_session)
-                           402 LOAD_METHOD             12 (add)
-                           424 LOAD_FAST                5 (db_data)
-                           426 PRECALL                  1
-                           430 CALL                     1
-                           440 POP_TOP
-               
-               165         442 LOAD_FAST                5 (db_data)
-                           444 RETURN_VALUE
+               223         150 LOAD_FAST                1 (data)
+                           152 LOAD_METHOD              6 (model_dump)
+                           174 LOAD_CONST               1 (True)
+                           176 KW_NAMES                 2
+                           178 PRECALL                  1
+                           182 CALL                     1
+                           192 STORE_FAST               4 (values)
+               
+               224         194 PUSH_NULL
+                           196 LOAD_FAST                3 (query)
+                           198 LOAD_ATTR                7 (values)
+                           208 LOAD_CONST               4 (())
+                           210 BUILD_MAP                0
+                           212 LOAD_FAST                4 (values)
+                           214 DICT_MERGE               1
+                           216 CALL_FUNCTION_EX         1
+                           218 STORE_FAST               3 (query)
+               
+               225         220 LOAD_FAST                2 (db_session)
+                           222 LOAD_METHOD              8 (execute)
+                           244 LOAD_FAST                3 (query)
+                           246 PRECALL                  1
+                           250 CALL                     1
+                           260 GET_AWAITABLE            0
+                           262 LOAD_CONST               3 (None)
+                       >>  264 SEND                     3 (to 272)
+                           266 YIELD_VALUE
+                           268 RESUME                   3
+                           270 JUMP_BACKWARD_NO_INTERRUPT     4 (to 264)
+                       >>  272 STORE_FAST               5 (result)
+               
+               226         274 LOAD_FAST                5 (result)
+                           276 LOAD_ATTR                9 (rowcount)
+                           286 RETURN_VALUE
                consts
-                  None
-                  0
+                  '\n        Update a single row by its ID.\n\n        Parameters:\n            data : The data to update\n            db_session : The database session to use\n        '
                   True
                   ('exclude_unset',)
-               names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one', 'isinstance', 'dict', 'model_dump', 'setattr', 'add')
-               varnames   ('self', 'data', 'db_session', 'query', 'result', 'db_data', 'update_data', 'field')
+                  None
+                  ()
+               names      ('db', 'session', 'update', 'model', 'where', 'id', 'model_dump', 'values', 'execute', 'rowcount')
+               varnames   ('self', 'data', 'db_session', 'query', 'values', 'result')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'update_by_id'
-               firstlineno 150
-               lnotab 0x06011c01740136010401040128012a0106022c01080130022a01
+               firstlineno 213
+               lnotab 0x06081c0174012c011a013601
+            'ids'
             code
                argcount  : 1
-               nlocals   : 5
-               stacksize : 8
+               nlocals   : 9
+               stacksize : 6
                flags     : 131
                code
-                  0x4b00010097007c02700b7c006a0000000000000000006a010000000000
-                  0000007d027c0144005d867d037405000000000000000000007c036401a6
-                  020000ab020000000000000000727402007407000000000000000000007c
-                  006a040000000000000000a6010000ab010000000000000000a005000000
-                  00000000000000000000000000000000007c006a0400000000000000006a
-                  0600000000000000007c036a0600000000000000006b0200000000a60100
-                  00ab0100000000000000006a070000000000000000640469007c03a00800
-                  000000000000000000000000000000000000006402ac03a6010000ab0100
-                  00000000000000a4018e017d047c02a00900000000000000000000000000
-                  000000000000007c04a6010000ab010000000000000000830064007b0356
-                  009703860401008c877415000000000000000000007c01a6010000ab0100
-                  000000000000005300
-               167           0 RETURN_GENERATOR
+                  0x4b00010097007c03700b7c006a0000000000000000006a010000000000
+                  0000003400830164017b035600970386047d047405000000000000000000
+                  007c006a030000000000000000a6010000ab010000000000000000a00400
+                  000000000000000000000000000000000000007c006a0300000000000000
+                  006a050000000000000000a0060000000000000000000000000000000000
+                  0000007c01a6010000ab010000000000000000a6010000ab010000000000
+                  0000007d057c02a0070000000000000000000000000000000000000000a6
+                  000000ab00000000000000000044005d1c5c0200007d067d077c05a00800
+                  000000000000000000000000000000000000007c067c076901a6010000ab
+                  0100000000000000007d058c1d7c04a00900000000000000000000000000
+                  000000000000007c05a6010000ab010000000000000000830064017b0356
+                  00970386047d087c086a0a00000000000000006302640164016401a60200
+                  00ab020000000000000000830264017b0356009703860401005300230031
+                  00830264017b035600970386047304770278035900770101005900010001
+                  0064015300
+               228           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               170           6 LOAD_FAST                2 (db_session)
+               239           6 LOAD_FAST                3 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
-                       >>   32 STORE_FAST               2 (db_session)
-               
-               171          34 LOAD_FAST                1 (data_list)
-                            36 GET_ITER
-                       >>   38 FOR_ITER               134 (to 308)
-                            40 STORE_FAST               3 (data)
-               
-               172          42 LOAD_GLOBAL              5 (NULL + hasattr)
-                            54 LOAD_FAST                3 (data)
-                            56 LOAD_CONST               1 ('id')
-                            58 PRECALL                  2
-                            62 CALL                     2
-                            72 POP_JUMP_FORWARD_IF_FALSE   116 (to 306)
-               
-               174          74 PUSH_NULL
-                            76 LOAD_GLOBAL              7 (NULL + update)
-                            88 LOAD_FAST                0 (self)
-                            90 LOAD_ATTR                4 (model)
-                           100 PRECALL                  1
-                           104 CALL                     1
-               
-               175         114 LOAD_METHOD              5 (where)
-                           136 LOAD_FAST                0 (self)
-                           138 LOAD_ATTR                4 (model)
-                           148 LOAD_ATTR                6 (id)
-                           158 LOAD_FAST                3 (data)
-                           160 LOAD_ATTR                6 (id)
-                           170 COMPARE_OP               2 (==)
-                           176 PRECALL                  1
-                           180 CALL                     1
-               
-               176         190 LOAD_ATTR                7 (values)
-               
-               174         200 LOAD_CONST               4 (())
-                           202 BUILD_MAP                0
-               
-               176         204 LOAD_FAST                3 (data)
-                           206 LOAD_METHOD              8 (dict)
-                           228 LOAD_CONST               2 (True)
-                           230 KW_NAMES                 3
-                           232 PRECALL                  1
-                           236 CALL                     1
-               
-               174         246 DICT_MERGE               1
-                           248 CALL_FUNCTION_EX         1
-               
-               173         250 STORE_FAST               4 (statement)
-               
-               178         252 LOAD_FAST                2 (db_session)
-                           254 LOAD_METHOD              9 (execute)
-                           276 LOAD_FAST                4 (statement)
-                           278 PRECALL                  1
-                           282 CALL                     1
-                           292 GET_AWAITABLE            0
-                           294 LOAD_CONST               0 (None)
-                       >>  296 SEND                     3 (to 304)
-                           298 YIELD_VALUE
-                           300 RESUME                   3
-                           302 JUMP_BACKWARD_NO_INTERRUPT     4 (to 296)
-                       >>  304 POP_TOP
-                       >>  306 JUMP_BACKWARD          135 (to 38)
-               
-               179     >>  308 LOAD_GLOBAL             21 (NULL + len)
-                           320 LOAD_FAST                1 (data_list)
-                           322 PRECALL                  1
-                           326 CALL                     1
-                           336 RETURN_VALUE
+                       >>   32 BEFORE_ASYNC_WITH
+                            34 GET_AWAITABLE            1
+                            36 LOAD_CONST               1 (None)
+                       >>   38 SEND                     3 (to 46)
+                            40 YIELD_VALUE
+                            42 RESUME                   3
+                            44 JUMP_BACKWARD_NO_INTERRUPT     4 (to 38)
+                       >>   46 STORE_FAST               4 (session)
+               
+               240          48 LOAD_GLOBAL              5 (NULL + update)
+                            60 LOAD_FAST                0 (self)
+                            62 LOAD_ATTR                3 (model)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 LOAD_METHOD              4 (where)
+                           108 LOAD_FAST                0 (self)
+                           110 LOAD_ATTR                3 (model)
+                           120 LOAD_ATTR                5 (id)
+                           130 LOAD_METHOD              6 (in_)
+                           152 LOAD_FAST                1 (ids)
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 PRECALL                  1
+                           172 CALL                     1
+                           182 STORE_FAST               5 (statement)
+               
+               241         184 LOAD_FAST                2 (data)
+                           186 LOAD_METHOD              7 (items)
+                           208 PRECALL                  0
+                           212 CALL                     0
+                           222 GET_ITER
+                       >>  224 FOR_ITER                28 (to 282)
+                           226 UNPACK_SEQUENCE          2
+                           230 STORE_FAST               6 (key)
+                           232 STORE_FAST               7 (value)
+               
+               242         234 LOAD_FAST                5 (statement)
+                           236 LOAD_METHOD              8 (values)
+                           258 LOAD_FAST                6 (key)
+                           260 LOAD_FAST                7 (value)
+                           262 BUILD_MAP                1
+                           264 PRECALL                  1
+                           268 CALL                     1
+                           278 STORE_FAST               5 (statement)
+                           280 JUMP_BACKWARD           29 (to 224)
+               
+               243     >>  282 LOAD_FAST                4 (session)
+                           284 LOAD_METHOD              9 (execute)
+                           306 LOAD_FAST                5 (statement)
+                           308 PRECALL                  1
+                           312 CALL                     1
+                           322 GET_AWAITABLE            0
+                           324 LOAD_CONST               1 (None)
+                       >>  326 SEND                     3 (to 334)
+                           328 YIELD_VALUE
+                           330 RESUME                   3
+                           332 JUMP_BACKWARD_NO_INTERRUPT     4 (to 326)
+                       >>  334 STORE_FAST               8 (result)
+               
+               244         336 LOAD_FAST                8 (result)
+                           338 LOAD_ATTR               10 (rowcount)
+               
+               239         348 SWAP                     2
+                           350 LOAD_CONST               1 (None)
+                           352 LOAD_CONST               1 (None)
+                           354 LOAD_CONST               1 (None)
+                           356 PRECALL                  2
+                           360 CALL                     2
+                           370 GET_AWAITABLE            2
+                           372 LOAD_CONST               1 (None)
+                       >>  374 SEND                     3 (to 382)
+                           376 YIELD_VALUE
+                           378 RESUME                   3
+                           380 JUMP_BACKWARD_NO_INTERRUPT     4 (to 374)
+                       >>  382 POP_TOP
+                           384 RETURN_VALUE
+                       >>  386 PUSH_EXC_INFO
+                           388 WITH_EXCEPT_START
+                           390 GET_AWAITABLE            2
+                           392 LOAD_CONST               1 (None)
+                       >>  394 SEND                     3 (to 402)
+                           396 YIELD_VALUE
+                           398 RESUME                   3
+                           400 JUMP_BACKWARD_NO_INTERRUPT     4 (to 394)
+                       >>  402 POP_JUMP_FORWARD_IF_TRUE     4 (to 412)
+                           404 RERAISE                  2
+                       >>  406 COPY                     3
+                           408 POP_EXCEPT
+                           410 RERAISE                  1
+                       >>  412 POP_TOP
+                           414 POP_EXCEPT
+                           416 POP_TOP
+                           418 POP_TOP
+                           420 LOAD_CONST               1 (None)
+                           422 RETURN_VALUE
+               ExceptionTable:
+                 46 to 346 -> 386 [1] lasti
+                 386 to 404 -> 406 [3] lasti
+                 412 to 412 -> 406 [3] lasti
                consts
+                  '\n        Update multiple rows by their IDs.\n\n        Parameters:\n            ids : The IDs of the rows to update\n            data : The data to update\n            db_session : The database session to use\n        '
                   None
-                  'id'
-                  True
-                  ('exclude_unset',)
-                  ()
-               names      ('db', 'session', 'hasattr', 'update', 'model', 'where', 'id', 'values', 'dict', 'execute', 'len')
-               varnames   ('self', 'data_list', 'db_session', 'data', 'statement')
+               names      ('db', 'session', 'update', 'model', 'where', 'id', 'in_', 'items', 'values', 'execute', 'rowcount')
+               varnames   ('self', 'ids', 'data', 'db_session', 'session', 'statement', 'key', 'value', 'result')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'update_batch_by_ids'
-               firstlineno 167
-               lnotab 0x06031c010801200228014c010afe04022afe04ff02053801
+               firstlineno 228
+               lnotab 0x060b2a0188013201300136010cfb
             code
                argcount  : 1
-               nlocals   : 6
+               nlocals   : 5
                stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a0500000000000000007c016b
                   0200000000a6010000ab0100000000000000007d037c02a0060000000000
                   0000000000000000000000000000007c03a6010000ab0100000000000000
-                  00830064007b035600970386047d047c04a0070000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007d057c02a00800
-                  000000000000000000000000000000000000007c05a6010000ab01000000
-                  0000000000830064007b035600970386045300
-               181           0 RETURN_GENERATOR
+                  00830064017b035600970386047d047c046a0700000000000000005300
+               246           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               182           6 LOAD_FAST                2 (db_session)
+               254           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               183          34 LOAD_GLOBAL              5 (NULL + select)
+               255          34 LOAD_GLOBAL              5 (NULL + delete)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
                            106 LOAD_ATTR                5 (id)
                            116 LOAD_FAST                1 (id)
                            118 COMPARE_OP               2 (==)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 STORE_FAST               3 (statement)
                
-               184         140 LOAD_FAST                2 (db_session)
+               256         140 LOAD_FAST                2 (db_session)
                            142 LOAD_METHOD              6 (execute)
                            164 LOAD_FAST                3 (statement)
                            166 PRECALL                  1
                            170 CALL                     1
                            180 GET_AWAITABLE            0
-                           182 LOAD_CONST               0 (None)
+                           182 LOAD_CONST               1 (None)
                        >>  184 SEND                     3 (to 192)
                            186 YIELD_VALUE
                            188 RESUME                   3
                            190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
-                       >>  192 STORE_FAST               4 (response)
-               
-               185         194 LOAD_FAST                4 (response)
-                           196 LOAD_METHOD              7 (scalar_one)
-                           218 PRECALL                  0
-                           222 CALL                     0
-                           232 STORE_FAST               5 (data)
+                       >>  192 STORE_FAST               4 (result)
                
-               186         234 LOAD_FAST                2 (db_session)
-                           236 LOAD_METHOD              8 (delete)
-                           258 LOAD_FAST                5 (data)
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 GET_AWAITABLE            0
-                           276 LOAD_CONST               0 (None)
-                       >>  278 SEND                     3 (to 286)
-                           280 YIELD_VALUE
-                           282 RESUME                   3
-                           284 JUMP_BACKWARD_NO_INTERRUPT     4 (to 278)
-                       >>  286 RETURN_VALUE
+               257         194 LOAD_FAST                4 (result)
+                           196 LOAD_ATTR                7 (rowcount)
+                           206 RETURN_VALUE
                consts
+                  '\n        Delete a single row by its ID.\n\n        Parameters:\n            id : The ID of the row to delete\n            db_session : The database session to use\n        '
                   None
-               names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one', 'delete')
-               varnames   ('self', 'id', 'db_session', 'statement', 'response', 'data')
+               names      ('db', 'session', 'delete', 'model', 'where', 'id', 'execute', 'rowcount')
+               varnames   ('self', 'id', 'db_session', 'statement', 'result')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'delete_by_id'
-               firstlineno 181
-               lnotab 0x06011c016a0136012801
+               firstlineno 246
+               lnotab 0x06081c016a013601
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a050000000000000000a00600
                   000000000000000000000000000000000000007c01a6010000ab01000000
                   0000000000a6010000ab0100000000000000007d037c02a0070000000000
                   0000000000000000000000000000007c03a6010000ab0100000000000000
-                  00830064007b035600970386047d047c046a0800000000000000005300
-               188           0 RETURN_GENERATOR
+                  00830064017b035600970386047d047c046a0800000000000000005300
+               259           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               191           6 LOAD_FAST                2 (db_session)
+               269           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               192          34 LOAD_GLOBAL              5 (NULL + delete)
+               270          34 LOAD_GLOBAL              5 (NULL + delete)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
@@ -1835,61 +1789,60 @@
                            138 LOAD_FAST                1 (ids)
                            140 PRECALL                  1
                            144 CALL                     1
                            154 PRECALL                  1
                            158 CALL                     1
                            168 STORE_FAST               3 (statement)
                
-               193         170 LOAD_FAST                2 (db_session)
+               271         170 LOAD_FAST                2 (db_session)
                            172 LOAD_METHOD              7 (execute)
                            194 LOAD_FAST                3 (statement)
                            196 PRECALL                  1
                            200 CALL                     1
                            210 GET_AWAITABLE            0
-                           212 LOAD_CONST               0 (None)
+                           212 LOAD_CONST               1 (None)
                        >>  214 SEND                     3 (to 222)
                            216 YIELD_VALUE
                            218 RESUME                   3
                            220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 214)
                        >>  222 STORE_FAST               4 (result)
                
-               194         224 LOAD_FAST                4 (result)
+               272         224 LOAD_FAST                4 (result)
                            226 LOAD_ATTR                8 (rowcount)
                            236 RETURN_VALUE
                consts
+                  '\n        Delete multiple rows by their IDs.\n\n        Parameters:\n            ids : The IDs of the rows to update\n            db_session : The database session to use\n        '
                   None
                names      ('db', 'session', 'delete', 'model', 'where', 'id', 'in_', 'execute', 'rowcount')
                varnames   ('self', 'ids', 'db_session', 'statement', 'result')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'delete_batch_by_ids'
-               firstlineno 188
-               lnotab 0x06031c0188013601
-         names      ('__name__', '__module__', '__qualname__', 'Type', 'ModelType', '__init__', 'Any', 'get_db_session', 'Union', 'SchemaType', 'AsyncSession', 'int', 'insert', 'List', 'insert_batch', 'select_by_id', 'select_by_ids', 'select_count', 'select_list', 'select_list_ordered', 'select_list_page', 'select_list_page_ordered', 'update_by_id', 'update_batch_by_ids', 'delete_by_id', 'delete_batch_by_ids')
+               firstlineno 259
+               lnotab 0x060a1c0188013601
+         names      ('__name__', '__module__', '__qualname__', 'Type', 'ModelType', '__init__', 'Union', 'SchemaType', 'AsyncSession', 'Any', 'insert', 'List', 'int', 'insert_batch', 'select_by_id', 'select_count', 'select_list', 'select_list_ordered', 'select_page', 'select_page_ordered', 'update_by_id', 'dict', 'update_batch_by_ids', 'delete_by_id', 'delete_batch_by_ids')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
          name       'SqlModelMapper'
          firstlineno 21
          lnotab
-            0x0a011804180702fc060312fd020412fc020502fb080c02ff06010eff02
-            0102ff020202fe080b1a0704ff06010eff020102ff020102ff02020efe08
-            0c160806ff060102ff020102ff020102ff020102ff02020efe0811020102
-            0402f8060302fd020402fc020502fb020602fa020702f9020802f802090e
-            f7082002ff060102ff020102ff020102ff02020efe080d02010201020102
-            f9060302fd020402fc020502fb020602fa020702f902080ef808141a1202
-            ff06010eff020102ff020202fe080e1a0802ff06010eff020102ff020202
-            fe
+            0x0a01180802fc060312fd020412fc020502fb081602ff06010eff020102
+            ff020202fe08131a10161106ff060102ff020102ff020102ff02020efe08
+            1f020102010201020102f9060302fd020402fc020502fb020602fa020702
+            f902090ef7083026100201020102fa060302fd020402fc020502fb020602
+            fa02070ef9081b1a1002ff06010eff020102ff020102ff020202fe08121a
+            0e02ff06010eff020102ff020202fe
       'SqlModelMapper'
       None
    names      ('__doc__', 'typing', 'Generic', 'TypeVar', 'List', 'Any', 'Type', 'Union', 'fastapi_pagination.ext.sqlmodel', 'paginate', 'pydantic', 'BaseModel', 'sqlmodel', 'SQLModel', 'select', 'func', 'insert', 'update', 'delete', 'sqlmodel.ext.asyncio.session', 'AsyncSession', 'fss.common.enum.enum', 'SortEnum', 'fss.common.persistence.base_mapper', 'BaseMapper', 'fss.middleware.db_session_middleware', 'db', 'ModelType', 'CreateSchemaType', 'UpdateSchemaType', 'SchemaType', 'T', 'SqlModelMapper')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\persistence\\sqlmodel_impl.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201040220020c010c0120010c020c010c010c021a011a011a011a
       011a03
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_model.py` & `fastapi_sqlmodel_starter-1.0.1/fss/common/persistence/base_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x1c321966 (Fri Apr 12 13:07:40 2024 UTC)
-files sz: 2850
+moddate:  0x4adf2366 (Sat Apr 20 15:29:14 2024 UTC)
+files sz: 3097
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
-      065a060100640164036c076d085a080100640164046c096d0a5a0a010002
-      00650364056502ac06a6020000ab0200000000000000005a0b0200650364
-      076508ac06a6020000ab0200000000000000005a0c020047006408840064
-      096505650c650b660219000000000000000000650a650b19000000000000
-      000000a6040000ab0400000000000000005a0d640a5300
+      065a060100640164036c076d085a080100640164046c096d0a5a0a010064
+      0164056c0b6d0c5a0c0100640164066c0d6d0e5a0e010002006503640765
+      02ac08a6020000ab0200000000000000005a0f0200650364096508ac08a6
+      020000ab0200000000000000005a1002004700640a8400640b6505651065
+      0f660219000000000000000000650a650f19000000000000000000a60400
+      00ab0400000000000000005a11640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Common service impl')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('Any', 'TypeVar', 'List', 'Generic', 'Type'))
@@ -43,552 +44,396 @@
      6          46 LOAD_CONST               1 (0)
                 48 LOAD_CONST               4 (('Service',))
                 50 IMPORT_NAME              9 (fss.common.service.service)
                 52 IMPORT_FROM             10 (Service)
                 54 STORE_NAME              10 (Service)
                 56 POP_TOP
    
-     8          58 PUSH_NULL
-                60 LOAD_NAME                3 (TypeVar)
-                62 LOAD_CONST               5 ('T')
-                64 LOAD_NAME                2 (Any)
-                66 KW_NAMES                 6
-                68 PRECALL                  2
-                72 CALL                     2
-                82 STORE_NAME              11 (T)
+     7          58 LOAD_CONST               1 (0)
+                60 LOAD_CONST               5 (('SystemResponseCode',))
+                62 IMPORT_NAME             11 (fss.starter.system.enum.system)
+                64 IMPORT_FROM             12 (SystemResponseCode)
+                66 STORE_NAME              12 (SystemResponseCode)
+                68 POP_TOP
    
-     9          84 PUSH_NULL
-                86 LOAD_NAME                3 (TypeVar)
-                88 LOAD_CONST               7 ('M')
-                90 LOAD_NAME                8 (BaseMapper)
-                92 KW_NAMES                 6
-                94 PRECALL                  2
-                98 CALL                     2
-               108 STORE_NAME              12 (M)
+     8          70 LOAD_CONST               1 (0)
+                72 LOAD_CONST               6 (('SystemException',))
+                74 IMPORT_NAME             13 (fss.starter.system.exception.system)
+                76 IMPORT_FROM             14 (SystemException)
+                78 STORE_NAME              14 (SystemException)
+                80 POP_TOP
    
-    12         110 PUSH_NULL
-               112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               8 (<code object ServiceImpl, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 12>)
-               116 MAKE_FUNCTION            0
-               118 LOAD_CONST               9 ('ServiceImpl')
-               120 LOAD_NAME                5 (Generic)
-               122 LOAD_NAME               12 (M)
-               124 LOAD_NAME               11 (T)
-               126 BUILD_TUPLE              2
-               128 BINARY_SUBSCR
-               138 LOAD_NAME               10 (Service)
-               140 LOAD_NAME               11 (T)
-               142 BINARY_SUBSCR
-               152 PRECALL                  4
-               156 CALL                     4
-               166 STORE_NAME              13 (ServiceImpl)
-               168 LOAD_CONST              10 (None)
-               170 RETURN_VALUE
+    10          82 PUSH_NULL
+                84 LOAD_NAME                3 (TypeVar)
+                86 LOAD_CONST               7 ('T')
+                88 LOAD_NAME                2 (Any)
+                90 KW_NAMES                 8
+                92 PRECALL                  2
+                96 CALL                     2
+               106 STORE_NAME              15 (T)
+   
+    11         108 PUSH_NULL
+               110 LOAD_NAME                3 (TypeVar)
+               112 LOAD_CONST               9 ('M')
+               114 LOAD_NAME                8 (BaseMapper)
+               116 KW_NAMES                 8
+               118 PRECALL                  2
+               122 CALL                     2
+               132 STORE_NAME              16 (M)
+   
+    14         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST              10 (<code object ServiceImpl, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 14>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST              11 ('ServiceImpl')
+               144 LOAD_NAME                5 (Generic)
+               146 LOAD_NAME               16 (M)
+               148 LOAD_NAME               15 (T)
+               150 BUILD_TUPLE              2
+               152 BINARY_SUBSCR
+               162 LOAD_NAME               10 (Service)
+               164 LOAD_NAME               15 (T)
+               166 BINARY_SUBSCR
+               176 PRECALL                  4
+               180 CALL                     4
+               190 STORE_NAME              17 (ServiceImpl)
+               192 LOAD_CONST              12 (None)
+               194 RETURN_VALUE
    consts
       'Common service impl'
       0
       ('Any', 'TypeVar', 'List', 'Generic', 'Type')
       ('BaseMapper',)
       ('Service',)
+      ('SystemResponseCode',)
+      ('SystemException',)
       'T'
       ('bound',)
       'M'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 13
+         stacksize : 12
          flags     : 0
          code
             0x970065005a0164005a0264016503650419000000000000000000660264
-            0284045a0564036506640465076604640584045a08640365066404650766
-            04640684045a096407650a65061900000000000000000064046507660464
-            0884045a0b6407650a650619000000000000000000640465076604640984
-            045a0c640a6506640465066604640b84045a0d640c640d9c01640e650a65
-            0619000000000000000000640f650e6404650a650f190000000000000000
-            006606641084065a106404650e6602641184045a116412650e6413650e64
-            1465066404650a6506190000000000000000006608641584045a12641265
-            0e6413650e6414650664166506641765066404650a650619000000000000
-            000000660c641884045a1364196506641465066404650a65061900000000
-            00000000006606641a84045a146419650664146506641765066404650a65
-            06190000000000000000006608641b84045a156403650664046507660464
-            1c84045a166407650a650619000000000000000000640465076604641d84
-            045a17640a6506640465076604641e84045a18640e650a650f1900000000
-            0000000000640465076604641f84045a1964205300
-          12           0 RESUME                   0
+            0284045a0564036506640465066604640584045a07640665086506190000
+            00000000000000640465096604640784045a0a6408650664046506660464
+            0984045a0b6404650c6602640a84045a0d640b650c640c650c6404650865
+            06190000000000000000006606640d84045a0e640e640e640f9c02640b65
+            0c640c650c64106506641165066404650865061900000000000000000066
+            0a641284065a0f6413650664046508650619000000000000000000660464
+            1484045a10640e64159c0164136506640465086506190000000000000000
+            006604641684065a1164036506640465096604641784045a12640e64189c
+            016419650865131900000000000000000064036514641a65136404650966
+            08641b84065a1564086506640465096604641c84045a1664196508651319
+            000000000000000000640465096604641d84045a17640e5300
+          14           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ServiceImpl')
                        8 STORE_NAME               2 (__qualname__)
          
-          13          10 LOAD_CONST               1 ('mapper')
+          15          10 LOAD_CONST               1 ('mapper')
                       12 LOAD_NAME                3 (Type)
                       14 LOAD_NAME                4 (M)
                       16 BINARY_SUBSCR
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 13>)
+                      28 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 15>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               5 (__init__)
          
-          16          34 LOAD_CONST               3 ('data')
+          18          34 LOAD_CONST               3 ('data')
                       36 LOAD_NAME                6 (T)
                       38 LOAD_CONST               4 ('return')
-                      40 LOAD_NAME                7 (bool)
+                      40 LOAD_NAME                6 (T)
                       42 BUILD_TUPLE              4
-                      44 LOAD_CONST               5 (<code object save, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 16>)
+                      44 LOAD_CONST               5 (<code object save, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 18>)
                       46 MAKE_FUNCTION            4 (annotations)
-                      48 STORE_NAME               8 (save)
+                      48 STORE_NAME               7 (save)
          
-          20          50 LOAD_CONST               3 ('data')
-                      52 LOAD_NAME                6 (T)
-                      54 LOAD_CONST               4 ('return')
-                      56 LOAD_NAME                7 (bool)
-                      58 BUILD_TUPLE              4
-                      60 LOAD_CONST               6 (<code object save_or_update, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 20>)
-                      62 MAKE_FUNCTION            4 (annotations)
-                      64 STORE_NAME               9 (save_or_update)
-         
-          27          66 LOAD_CONST               7 ('data_list')
-                      68 LOAD_NAME               10 (List)
-                      70 LOAD_NAME                6 (T)
-                      72 BINARY_SUBSCR
+          21          50 LOAD_CONST               6 ('data_list')
+                      52 LOAD_NAME                8 (List)
+                      54 LOAD_NAME                6 (T)
+                      56 BINARY_SUBSCR
+                      66 LOAD_CONST               4 ('return')
+                      68 LOAD_NAME                9 (bool)
+                      70 BUILD_TUPLE              4
+                      72 LOAD_CONST               7 (<code object save_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 21>)
+                      74 MAKE_FUNCTION            4 (annotations)
+                      76 STORE_NAME              10 (save_batch)
+         
+          25          78 LOAD_CONST               8 ('id')
+                      80 LOAD_NAME                6 (T)
                       82 LOAD_CONST               4 ('return')
-                      84 LOAD_NAME                7 (bool)
+                      84 LOAD_NAME                6 (T)
                       86 BUILD_TUPLE              4
-                      88 LOAD_CONST               8 (<code object save_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 27>)
+                      88 LOAD_CONST               9 (<code object get_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 25>)
                       90 MAKE_FUNCTION            4 (annotations)
-                      92 STORE_NAME              11 (save_batch)
+                      92 STORE_NAME              11 (get_by_id)
          
-          31          94 LOAD_CONST               7 ('data_list')
-                      96 LOAD_NAME               10 (List)
-                      98 LOAD_NAME                6 (T)
-                     100 BINARY_SUBSCR
-                     110 LOAD_CONST               4 ('return')
-                     112 LOAD_NAME                7 (bool)
-                     114 BUILD_TUPLE              4
-                     116 LOAD_CONST               9 (<code object save_or_update_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 31>)
-                     118 MAKE_FUNCTION            4 (annotations)
-                     120 STORE_NAME              12 (save_or_update_batch)
-         
-          39         122 LOAD_CONST              10 ('id')
-                     124 LOAD_NAME                6 (T)
-                     126 LOAD_CONST               4 ('return')
-                     128 LOAD_NAME                6 (T)
-                     130 BUILD_TUPLE              4
-                     132 LOAD_CONST              11 (<code object get_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 39>)
+          28          94 LOAD_CONST               4 ('return')
+                      96 LOAD_NAME               12 (int)
+                      98 BUILD_TUPLE              2
+                     100 LOAD_CONST              10 (<code object count, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 28>)
+                     102 MAKE_FUNCTION            4 (annotations)
+                     104 STORE_NAME              13 (count)
+         
+          31         106 LOAD_CONST              11 ('page')
+                     108 LOAD_NAME               12 (int)
+                     110 LOAD_CONST              12 ('size')
+                     112 LOAD_NAME               12 (int)
+                     114 LOAD_CONST               4 ('return')
+                     116 LOAD_NAME                8 (List)
+                     118 LOAD_NAME                6 (T)
+                     120 BINARY_SUBSCR
+                     130 BUILD_TUPLE              6
+                     132 LOAD_CONST              13 (<code object list, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 31>)
                      134 MAKE_FUNCTION            4 (annotations)
-                     136 STORE_NAME              13 (get_by_id)
+                     136 STORE_NAME              14 (list)
+         
+          39         138 LOAD_CONST              14 (None)
          
-          42         138 LOAD_CONST              12 (1000)
-                     140 LOAD_CONST              13 (('batch_size',))
-                     142 BUILD_CONST_KEY_MAP      1
-                     144 LOAD_CONST              14 ('ids')
-                     146 LOAD_NAME               10 (List)
-                     148 LOAD_NAME                6 (T)
-                     150 BINARY_SUBSCR
-                     160 LOAD_CONST              15 ('batch_size')
-                     162 LOAD_NAME               14 (int)
-                     164 LOAD_CONST               4 ('return')
-                     166 LOAD_NAME               10 (List)
-                     168 LOAD_NAME               15 (Any)
-                     170 BINARY_SUBSCR
-                     180 BUILD_TUPLE              6
-                     182 LOAD_CONST              16 (<code object get_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 42>)
-                     184 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     186 STORE_NAME              16 (get_by_ids)
-         
-          45         188 LOAD_CONST               4 ('return')
-                     190 LOAD_NAME               14 (int)
-                     192 BUILD_TUPLE              2
-                     194 LOAD_CONST              17 (<code object count, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 45>)
-                     196 MAKE_FUNCTION            4 (annotations)
-                     198 STORE_NAME              17 (count)
-         
-          48         200 LOAD_CONST              18 ('page')
-                     202 LOAD_NAME               14 (int)
-                     204 LOAD_CONST              19 ('size')
-                     206 LOAD_NAME               14 (int)
-                     208 LOAD_CONST              20 ('query')
-                     210 LOAD_NAME                6 (T)
-                     212 LOAD_CONST               4 ('return')
-                     214 LOAD_NAME               10 (List)
-                     216 LOAD_NAME                6 (T)
-                     218 BINARY_SUBSCR
-                     228 BUILD_TUPLE              8
-                     230 LOAD_CONST              21 (<code object list, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 48>)
-                     232 MAKE_FUNCTION            4 (annotations)
-                     234 STORE_NAME              18 (list)
-         
-          51         236 LOAD_CONST              18 ('page')
-         
-          52         238 LOAD_NAME               14 (int)
-         
-          51         240 LOAD_CONST              19 ('size')
-         
-          52         242 LOAD_NAME               14 (int)
-         
-          51         244 LOAD_CONST              20 ('query')
-         
-          52         246 LOAD_NAME                6 (T)
-         
-          51         248 LOAD_CONST              22 ('order_by')
-         
-          52         250 LOAD_NAME                6 (T)
-         
-          51         252 LOAD_CONST              23 ('sort_order')
-         
-          52         254 LOAD_NAME                6 (T)
-         
-          51         256 LOAD_CONST               4 ('return')
-         
-          53         258 LOAD_NAME               10 (List)
-                     260 LOAD_NAME                6 (T)
-                     262 BINARY_SUBSCR
-         
-          51         272 BUILD_TUPLE             12
-                     274 LOAD_CONST              24 (<code object list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 51>)
-                     276 MAKE_FUNCTION            4 (annotations)
-                     278 STORE_NAME              19 (list_ordered)
-         
-          58         280 LOAD_CONST              25 ('params')
-                     282 LOAD_NAME                6 (T)
-                     284 LOAD_CONST              20 ('query')
-                     286 LOAD_NAME                6 (T)
-                     288 LOAD_CONST               4 ('return')
-                     290 LOAD_NAME               10 (List)
-                     292 LOAD_NAME                6 (T)
-                     294 BINARY_SUBSCR
-                     304 BUILD_TUPLE              6
-                     306 LOAD_CONST              26 (<code object list_page, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 58>)
-                     308 MAKE_FUNCTION            4 (annotations)
-                     310 STORE_NAME              20 (list_page)
-         
-          61         312 LOAD_CONST              25 ('params')
-                     314 LOAD_NAME                6 (T)
-                     316 LOAD_CONST              20 ('query')
-                     318 LOAD_NAME                6 (T)
-                     320 LOAD_CONST              23 ('sort_order')
-                     322 LOAD_NAME                6 (T)
-                     324 LOAD_CONST               4 ('return')
-                     326 LOAD_NAME               10 (List)
-                     328 LOAD_NAME                6 (T)
-                     330 BINARY_SUBSCR
-                     340 BUILD_TUPLE              8
-                     342 LOAD_CONST              27 (<code object list_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 61>)
-                     344 MAKE_FUNCTION            4 (annotations)
-                     346 STORE_NAME              21 (list_page_ordered)
-         
-          66         348 LOAD_CONST               3 ('data')
-                     350 LOAD_NAME                6 (T)
-                     352 LOAD_CONST               4 ('return')
-                     354 LOAD_NAME                7 (bool)
-                     356 BUILD_TUPLE              4
-                     358 LOAD_CONST              28 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 66>)
-                     360 MAKE_FUNCTION            4 (annotations)
-                     362 STORE_NAME              22 (update_by_id)
-         
-          69         364 LOAD_CONST               7 ('data_list')
-                     366 LOAD_NAME               10 (List)
-                     368 LOAD_NAME                6 (T)
-                     370 BINARY_SUBSCR
-                     380 LOAD_CONST               4 ('return')
-                     382 LOAD_NAME                7 (bool)
-                     384 BUILD_TUPLE              4
-                     386 LOAD_CONST              29 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 69>)
-                     388 MAKE_FUNCTION            4 (annotations)
-                     390 STORE_NAME              23 (update_batch_by_ids)
-         
-          72         392 LOAD_CONST              10 ('id')
-                     394 LOAD_NAME                6 (T)
-                     396 LOAD_CONST               4 ('return')
-                     398 LOAD_NAME                7 (bool)
-                     400 BUILD_TUPLE              4
-                     402 LOAD_CONST              30 (<code object remove_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 72>)
-                     404 MAKE_FUNCTION            4 (annotations)
-                     406 STORE_NAME              24 (remove_by_id)
-         
-          75         408 LOAD_CONST              14 ('ids')
-                     410 LOAD_NAME               10 (List)
-                     412 LOAD_NAME               15 (Any)
-                     414 BINARY_SUBSCR
-                     424 LOAD_CONST               4 ('return')
-                     426 LOAD_NAME                7 (bool)
-                     428 BUILD_TUPLE              4
-                     430 LOAD_CONST              31 (<code object remove_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\service\impl\service_impl.py", line 75>)
-                     432 MAKE_FUNCTION            4 (annotations)
-                     434 STORE_NAME              25 (remove_batch_by_ids)
-                     436 LOAD_CONST              32 (None)
-                     438 RETURN_VALUE
+          40         140 LOAD_CONST              14 (None)
+         
+          34         142 LOAD_CONST              15 (('order_by', 'sort_order'))
+                     144 BUILD_CONST_KEY_MAP      2
+                     146 LOAD_CONST              11 ('page')
+         
+          37         148 LOAD_NAME               12 (int)
+         
+          34         150 LOAD_CONST              12 ('size')
+         
+          38         152 LOAD_NAME               12 (int)
+         
+          34         154 LOAD_CONST              16 ('order_by')
+         
+          39         156 LOAD_NAME                6 (T)
+         
+          34         158 LOAD_CONST              17 ('sort_order')
+         
+          40         160 LOAD_NAME                6 (T)
+         
+          34         162 LOAD_CONST               4 ('return')
+         
+          42         164 LOAD_NAME                8 (List)
+                     166 LOAD_NAME                6 (T)
+                     168 BINARY_SUBSCR
+         
+          34         178 BUILD_TUPLE             10
+                     180 LOAD_CONST              18 (<code object list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 34>)
+                     182 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     184 STORE_NAME              15 (list_ordered)
+         
+          47         186 LOAD_CONST              19 ('params')
+                     188 LOAD_NAME                6 (T)
+                     190 LOAD_CONST               4 ('return')
+                     192 LOAD_NAME                8 (List)
+                     194 LOAD_NAME                6 (T)
+                     196 BINARY_SUBSCR
+                     206 BUILD_TUPLE              4
+                     208 LOAD_CONST              20 (<code object list_page, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 47>)
+                     210 MAKE_FUNCTION            4 (annotations)
+                     212 STORE_NAME              16 (list_page)
+         
+          50         214 LOAD_CONST              14 (None)
+                     216 LOAD_CONST              21 (('params',))
+                     218 BUILD_CONST_KEY_MAP      1
+                     220 LOAD_CONST              19 ('params')
+                     222 LOAD_NAME                6 (T)
+                     224 LOAD_CONST               4 ('return')
+                     226 LOAD_NAME                8 (List)
+                     228 LOAD_NAME                6 (T)
+                     230 BINARY_SUBSCR
+                     240 BUILD_TUPLE              4
+                     242 LOAD_CONST              22 (<code object list_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 50>)
+                     244 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     246 STORE_NAME              17 (list_page_ordered)
+         
+          53         248 LOAD_CONST               3 ('data')
+                     250 LOAD_NAME                6 (T)
+                     252 LOAD_CONST               4 ('return')
+                     254 LOAD_NAME                9 (bool)
+                     256 BUILD_TUPLE              4
+                     258 LOAD_CONST              23 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 53>)
+                     260 MAKE_FUNCTION            4 (annotations)
+                     262 STORE_NAME              18 (update_by_id)
+         
+          63         264 LOAD_CONST              14 (None)
+         
+          62         266 LOAD_CONST              24 (('db_session',))
+                     268 BUILD_CONST_KEY_MAP      1
+                     270 LOAD_CONST              25 ('ids')
+         
+          63         272 LOAD_NAME                8 (List)
+                     274 LOAD_NAME               19 (Any)
+                     276 BINARY_SUBSCR
+         
+          62         286 LOAD_CONST               3 ('data')
+         
+          63         288 LOAD_NAME               20 (dict)
+         
+          62         290 LOAD_CONST              26 ('db_session')
+         
+          63         292 LOAD_NAME               19 (Any)
+         
+          62         294 LOAD_CONST               4 ('return')
+         
+          64         296 LOAD_NAME                9 (bool)
+         
+          62         298 BUILD_TUPLE              8
+                     300 LOAD_CONST              27 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 62>)
+                     302 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     304 STORE_NAME              21 (update_batch_by_ids)
+         
+          73         306 LOAD_CONST               8 ('id')
+                     308 LOAD_NAME                6 (T)
+                     310 LOAD_CONST               4 ('return')
+                     312 LOAD_NAME                9 (bool)
+                     314 BUILD_TUPLE              4
+                     316 LOAD_CONST              28 (<code object remove_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 73>)
+                     318 MAKE_FUNCTION            4 (annotations)
+                     320 STORE_NAME              22 (remove_by_id)
+         
+          82         322 LOAD_CONST              25 ('ids')
+                     324 LOAD_NAME                8 (List)
+                     326 LOAD_NAME               19 (Any)
+                     328 BINARY_SUBSCR
+                     338 LOAD_CONST               4 ('return')
+                     340 LOAD_NAME                9 (bool)
+                     342 BUILD_TUPLE              4
+                     344 LOAD_CONST              29 (<code object remove_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\common\service\impl\service_impl.py", line 82>)
+                     346 MAKE_FUNCTION            4 (annotations)
+                     348 STORE_NAME              23 (remove_batch_by_ids)
+                     350 LOAD_CONST              14 (None)
+                     352 RETURN_VALUE
          consts
             'ServiceImpl'
             'mapper'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c017c005f00000000000000000064005300
-                13           0 RESUME                   0
+                15           0 RESUME                   0
                
-                14           2 LOAD_FAST                1 (mapper)
+                16           2 LOAD_FAST                1 (mapper)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (mapper)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('mapper',)
                varnames   ('self', 'mapper')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       '__init__'
-               firstlineno 13
+               firstlineno 15
                lnotab 0x0201
             'data'
             'return'
             code
                argcount  : 1
-               nlocals   : 3
+               nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386047d027c025300
-                16           0 RETURN_GENERATOR
+                  0064007b035600970386045300
+                18           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                17           6 LOAD_FAST                0 (self)
+                19           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (insert)
                             40 LOAD_FAST                1 (data)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               0 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 STORE_FAST               2 (result)
-               
-                18          72 LOAD_FAST                2 (result)
-                            74 RETURN_VALUE
+                       >>   70 RETURN_VALUE
                consts
                   None
                   ('data',)
                names      ('mapper', 'insert')
-               varnames   ('self', 'data', 'result')
+               varnames   ('self', 'data')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'save'
-               firstlineno 16
-               lnotab 0x06014201
-            code
-               argcount  : 1
-               nlocals   : 3
-               stacksize : 3
-               flags     : 131
-               code
-                  0x4b00010097007c016a00000000000000000080227c006a010000000000
-                  000000a00200000000000000000000000000000000000000007c01ac01a6
-                  010000ab010000000000000000830064007b035600970386047d026e1c7c
-                  00a00300000000000000000000000000000000000000007c01ac01a60100
-                  00ab010000000000000000830064007b035600970386047d027c025300
-                20           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                21           6 LOAD_FAST                1 (data)
-                             8 LOAD_ATTR                0 (id)
-                            18 POP_JUMP_FORWARD_IF_NOT_NONE    34 (to 88)
-               
-                22          20 LOAD_FAST                0 (self)
-                            22 LOAD_ATTR                1 (mapper)
-                            32 LOAD_METHOD              2 (insert)
-                            54 LOAD_FAST                1 (data)
-                            56 KW_NAMES                 1
-                            58 PRECALL                  1
-                            62 CALL                     1
-                            72 GET_AWAITABLE            0
-                            74 LOAD_CONST               0 (None)
-                       >>   76 SEND                     3 (to 84)
-                            78 YIELD_VALUE
-                            80 RESUME                   3
-                            82 JUMP_BACKWARD_NO_INTERRUPT     4 (to 76)
-                       >>   84 STORE_FAST               2 (result)
-                            86 JUMP_FORWARD            28 (to 144)
-               
-                24     >>   88 LOAD_FAST                0 (self)
-                            90 LOAD_METHOD              3 (update_by_id)
-                           112 LOAD_FAST                1 (data)
-                           114 KW_NAMES                 1
-                           116 PRECALL                  1
-                           120 CALL                     1
-                           130 GET_AWAITABLE            0
-                           132 LOAD_CONST               0 (None)
-                       >>  134 SEND                     3 (to 142)
-                           136 YIELD_VALUE
-                           138 RESUME                   3
-                           140 JUMP_BACKWARD_NO_INTERRUPT     4 (to 134)
-                       >>  142 STORE_FAST               2 (result)
-               
-                25     >>  144 LOAD_FAST                2 (result)
-                           146 RETURN_VALUE
-               consts
-                  None
-                  ('data',)
-               names      ('id', 'mapper', 'insert', 'update_by_id')
-               varnames   ('self', 'data', 'result')
-               freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
-               name       'save_or_update'
-               firstlineno 20
-               lnotab 0x06010e0144023801
+               firstlineno 18
+               lnotab 0x0601
             'data_list'
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 4
+               nlocals   : 2
+               stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386047d027c027405000000000000000000007c01a6
-                  010000ab0100000000000000006b02000000005300
-                27           0 RETURN_GENERATOR
+                  0064007b03560097038604010064025300
+                21           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                28           6 LOAD_FAST                0 (self)
+                22           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (insert_batch)
                             40 LOAD_FAST                1 (data_list)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               0 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 STORE_FAST               2 (result)
+                       >>   70 POP_TOP
                
-                29          72 LOAD_FAST                2 (result)
-                            74 LOAD_GLOBAL              5 (NULL + len)
-                            86 LOAD_FAST                1 (data_list)
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 COMPARE_OP               2 (==)
-                           108 RETURN_VALUE
+                23          72 LOAD_CONST               2 (True)
+                            74 RETURN_VALUE
                consts
                   None
                   ('data_list',)
-               names      ('mapper', 'insert_batch', 'len')
-               varnames   ('self', 'data_list', 'result')
+                  True
+               names      ('mapper', 'insert_batch')
+               varnames   ('self', 'data_list')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'save_batch'
-               firstlineno 27
+               firstlineno 21
                lnotab 0x06014201
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 3
-               flags     : 131
-               code
-                  0x4b00010097007401000000000000000000007c01a6010000ab01000000
-                  000000000064016b02000000007202640253007c01640119000000000000
-                  0000006a010000000000000000801c7c00a0020000000000000000000000
-                  0000000000000000007c01ac03a6010000ab010000000000000000830064
-                  007b0356009703860453007c00a003000000000000000000000000000000
-                  00000000007c01ac03a6010000ab010000000000000000830064007b0356
-                  00970386045300
-                31           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                32           6 LOAD_GLOBAL              1 (NULL + len)
-                            18 LOAD_FAST                1 (data_list)
-                            20 PRECALL                  1
-                            24 CALL                     1
-                            34 LOAD_CONST               1 (0)
-                            36 COMPARE_OP               2 (==)
-                            42 POP_JUMP_FORWARD_IF_FALSE     2 (to 48)
-               
-                33          44 LOAD_CONST               2 (False)
-                            46 RETURN_VALUE
-               
-                34     >>   48 LOAD_FAST                1 (data_list)
-                            50 LOAD_CONST               1 (0)
-                            52 BINARY_SUBSCR
-                            62 LOAD_ATTR                1 (id)
-                            72 POP_JUMP_FORWARD_IF_NOT_NONE    28 (to 130)
-               
-                35          74 LOAD_FAST                0 (self)
-                            76 LOAD_METHOD              2 (save_batch)
-                            98 LOAD_FAST                1 (data_list)
-                           100 KW_NAMES                 3
-                           102 PRECALL                  1
-                           106 CALL                     1
-                           116 GET_AWAITABLE            0
-                           118 LOAD_CONST               0 (None)
-                       >>  120 SEND                     3 (to 128)
-                           122 YIELD_VALUE
-                           124 RESUME                   3
-                           126 JUMP_BACKWARD_NO_INTERRUPT     4 (to 120)
-                       >>  128 RETURN_VALUE
-               
-                37     >>  130 LOAD_FAST                0 (self)
-                           132 LOAD_METHOD              3 (update_batch_by_ids)
-                           154 LOAD_FAST                1 (data_list)
-                           156 KW_NAMES                 3
-                           158 PRECALL                  1
-                           162 CALL                     1
-                           172 GET_AWAITABLE            0
-                           174 LOAD_CONST               0 (None)
-                       >>  176 SEND                     3 (to 184)
-                           178 YIELD_VALUE
-                           180 RESUME                   3
-                           182 JUMP_BACKWARD_NO_INTERRUPT     4 (to 176)
-                       >>  184 RETURN_VALUE
-               consts
-                  None
-                  0
-                  False
-                  ('data_list',)
-               names      ('len', 'id', 'save_batch', 'update_batch_by_ids')
-               varnames   ('self', 'data_list')
-               freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
-               name       'save_or_update_batch'
-               firstlineno 31
-               lnotab 0x0601260104011a013802
             'id'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
                   0064007b035600970386045300
-                39           0 RETURN_GENERATOR
+                25           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                40           6 LOAD_FAST                0 (self)
+                26           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_by_id)
                             40 LOAD_FAST                1 (id)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
@@ -601,75 +446,32 @@
                consts
                   None
                   ('id',)
                names      ('mapper', 'select_by_id')
                varnames   ('self', 'id')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'get_by_id'
-               firstlineno 39
-               lnotab 0x0601
-            1000
-            ('batch_size',)
-            'ids'
-            'batch_size'
-            code
-               argcount  : 1
-               nlocals   : 3
-               stacksize : 4
-               flags     : 131
-               code
-                  0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c017c02ac01a6020000ab0200000000000000
-                  00830064007b035600970386045300
-                42           0 RETURN_GENERATOR
-                             2 POP_TOP
-                             4 RESUME                   0
-               
-                43           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_by_ids)
-                            40 LOAD_FAST                1 (ids)
-                            42 LOAD_FAST                2 (batch_size)
-                            44 KW_NAMES                 1
-                            46 PRECALL                  2
-                            50 CALL                     2
-                            60 GET_AWAITABLE            0
-                            62 LOAD_CONST               0 (None)
-                       >>   64 SEND                     3 (to 72)
-                            66 YIELD_VALUE
-                            68 RESUME                   3
-                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
-                       >>   72 RETURN_VALUE
-               consts
-                  None
-                  ('ids', 'batch_size')
-               names      ('mapper', 'select_by_ids')
-               varnames   ('self', 'ids', 'batch_size')
-               freevars   ()
-               cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
-               name       'get_by_ids'
-               firstlineno 42
+               firstlineno 25
                lnotab 0x0601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000830064007b
                   035600970386045300
-                45           0 RETURN_GENERATOR
+                28           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                46           6 LOAD_FAST                0 (self)
+                29           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_count)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 GET_AWAITABLE            0
                             56 LOAD_CONST               0 (None)
                        >>   58 SEND                     3 (to 66)
@@ -679,355 +481,482 @@
                        >>   66 RETURN_VALUE
                consts
                   None
                names      ('mapper', 'select_count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'count'
-               firstlineno 45
+               firstlineno 28
                lnotab 0x0601
             'page'
             'size'
-            'query'
             code
                argcount  : 1
                nlocals   : 4
-               stacksize : 5
-               flags     : 131
+               stacksize : 6
+               flags     : 139
                code
-                  0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c017c027c03ac01a6030000ab030000000000
-                  000000830064007b035600970386045300
-                48           0 RETURN_GENERATOR
+                  0x4b000100970002007c006a0000000000000000006a0100000000000000
+                  0064027c017c0264019c027c03a4018e01830064007b0356009703860453
+                  00
+                31           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                49           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_list)
-                            40 LOAD_FAST                1 (page)
-                            42 LOAD_FAST                2 (size)
-                            44 LOAD_FAST                3 (query)
-                            46 KW_NAMES                 1
-                            48 PRECALL                  3
-                            52 CALL                     3
-                            62 GET_AWAITABLE            0
-                            64 LOAD_CONST               0 (None)
-                       >>   66 SEND                     3 (to 74)
-                            68 YIELD_VALUE
-                            70 RESUME                   3
-                            72 JUMP_BACKWARD_NO_INTERRUPT     4 (to 66)
-                       >>   74 RETURN_VALUE
+                32           6 PUSH_NULL
+                             8 LOAD_FAST                0 (self)
+                            10 LOAD_ATTR                0 (mapper)
+                            20 LOAD_ATTR                1 (select_list)
+                            30 LOAD_CONST               2 (())
+                            32 LOAD_FAST                1 (page)
+                            34 LOAD_FAST                2 (size)
+                            36 LOAD_CONST               1 (('page', 'size'))
+                            38 BUILD_CONST_KEY_MAP      2
+                            40 LOAD_FAST                3 (kwargs)
+                            42 DICT_MERGE               1
+                            44 CALL_FUNCTION_EX         1
+                            46 GET_AWAITABLE            0
+                            48 LOAD_CONST               0 (None)
+                       >>   50 SEND                     3 (to 58)
+                            52 YIELD_VALUE
+                            54 RESUME                   3
+                            56 JUMP_BACKWARD_NO_INTERRUPT     4 (to 50)
+                       >>   58 RETURN_VALUE
                consts
                   None
-                  ('page', 'size', 'query')
+                  ('page', 'size')
+                  ()
                names      ('mapper', 'select_list')
-               varnames   ('self', 'page', 'size', 'query')
+               varnames   ('self', 'page', 'size', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'list'
-               firstlineno 48
+               firstlineno 31
                lnotab 0x0601
+            None
+            ('order_by', 'sort_order')
             'order_by'
             'sort_order'
             code
                argcount  : 1
                nlocals   : 6
-               stacksize : 7
-               flags     : 131
+               stacksize : 8
+               flags     : 139
                code
-                  0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c017c027c037c047c05ac01a6050000ab0500
-                  00000000000000830064007b035600970386045300
-                51           0 RETURN_GENERATOR
+                  0x4b000100970002007c006a0000000000000000006a0100000000000000
+                  0064027c017c027c037c0464019c047c05a4018e01830064007b03560097
+                  0386045300
+                34           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                54           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_list_ordered)
+                43           6 PUSH_NULL
+                             8 LOAD_FAST                0 (self)
+                            10 LOAD_ATTR                0 (mapper)
+                            20 LOAD_ATTR                1 (select_list_ordered)
+                            30 LOAD_CONST               2 (())
+               
+                44          32 LOAD_FAST                1 (page)
+                            34 LOAD_FAST                2 (size)
+                            36 LOAD_FAST                3 (order_by)
+                            38 LOAD_FAST                4 (sort_order)
                
-                55          40 LOAD_FAST                1 (page)
-                            42 LOAD_FAST                2 (size)
-                            44 LOAD_FAST                3 (query)
-                            46 LOAD_FAST                4 (order_by)
-                            48 LOAD_FAST                5 (sort_order)
-               
-                54          50 KW_NAMES                 1
-                            52 PRECALL                  5
-                            56 CALL                     5
-                            66 GET_AWAITABLE            0
-                            68 LOAD_CONST               0 (None)
-                       >>   70 SEND                     3 (to 78)
-                            72 YIELD_VALUE
-                            74 RESUME                   3
-                            76 JUMP_BACKWARD_NO_INTERRUPT     4 (to 70)
-                       >>   78 RETURN_VALUE
+                43          40 LOAD_CONST               1 (('page', 'size', 'order_by', 'sort_order'))
+                            42 BUILD_CONST_KEY_MAP      4
+               
+                44          44 LOAD_FAST                5 (kwargs)
+               
+                43          46 DICT_MERGE               1
+                            48 CALL_FUNCTION_EX         1
+                            50 GET_AWAITABLE            0
+                            52 LOAD_CONST               0 (None)
+                       >>   54 SEND                     3 (to 62)
+                            56 YIELD_VALUE
+                            58 RESUME                   3
+                            60 JUMP_BACKWARD_NO_INTERRUPT     4 (to 54)
+                       >>   62 RETURN_VALUE
                consts
                   None
-                  ('page', 'size', 'query', 'order_by', 'sort_order')
+                  ('page', 'size', 'order_by', 'sort_order')
+                  ()
                names      ('mapper', 'select_list_ordered')
-               varnames   ('self', 'page', 'size', 'query', 'order_by', 'sort_order')
+               varnames   ('self', 'page', 'size', 'order_by', 'sort_order', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'list_ordered'
-               firstlineno 51
-               lnotab 0x060322010aff
+               firstlineno 34
+               lnotab 0x06091a0108ff040102ff
             'params'
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 4
+               nlocals   : 2
+               stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c017c02ac01a6020000ab0200000000000000
-                  00830064007b035600970386045300
-                58           0 RETURN_GENERATOR
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
+                47           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                59           6 LOAD_FAST                0 (self)
+                48           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_list_page)
+                            18 LOAD_METHOD              1 (select_page)
                             40 LOAD_FAST                1 (params)
-                            42 LOAD_FAST                2 (query)
-                            44 KW_NAMES                 1
-                            46 PRECALL                  2
-                            50 CALL                     2
-                            60 GET_AWAITABLE            0
-                            62 LOAD_CONST               0 (None)
-                       >>   64 SEND                     3 (to 72)
-                            66 YIELD_VALUE
-                            68 RESUME                   3
-                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
-                       >>   72 RETURN_VALUE
+                            42 KW_NAMES                 1
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
-                  ('params', 'query')
-               names      ('mapper', 'select_list_page')
-               varnames   ('self', 'params', 'query')
+                  ('params',)
+               names      ('mapper', 'select_page')
+               varnames   ('self', 'params')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'list_page'
-               firstlineno 58
+               firstlineno 47
                lnotab 0x0601
+            ('params',)
             code
                argcount  : 1
-               nlocals   : 4
-               stacksize : 5
+               nlocals   : 2
+               stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c017c027c03ac01a6030000ab030000000000
-                  000000830064007b035600970386045300
-                61           0 RETURN_GENERATOR
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
+                50           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                62           6 LOAD_FAST                0 (self)
+                51           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_list_page_ordered)
-               
-                63          40 LOAD_FAST                1 (params)
-                            42 LOAD_FAST                2 (query)
-                            44 LOAD_FAST                3 (sort_order)
-               
-                62          46 KW_NAMES                 1
-                            48 PRECALL                  3
-                            52 CALL                     3
-                            62 GET_AWAITABLE            0
-                            64 LOAD_CONST               0 (None)
-                       >>   66 SEND                     3 (to 74)
-                            68 YIELD_VALUE
-                            70 RESUME                   3
-                            72 JUMP_BACKWARD_NO_INTERRUPT     4 (to 66)
-                       >>   74 RETURN_VALUE
+                            18 LOAD_METHOD              1 (select_page_ordered)
+                            40 LOAD_FAST                1 (params)
+                            42 KW_NAMES                 1
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
-                  ('params', 'query', 'sort_order')
-               names      ('mapper', 'select_list_page_ordered')
-               varnames   ('self', 'params', 'query', 'sort_order')
+                  ('params',)
+               names      ('mapper', 'select_page_ordered')
+               varnames   ('self', 'params')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'list_page_ordered'
-               firstlineno 61
-               lnotab 0x0601220106ff
+               firstlineno 50
+               lnotab 0x0601
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 3
+               stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386045300
-                66           0 RETURN_GENERATOR
+                  0064007b035600970386047d027c0264026b0300000000722e7405000000
+                  000000000000007406000000000000000000006a0400000000000000006a
+                  0500000000000000007406000000000000000000006a0400000000000000
+                  006a060000000000000000a6020000ab0200000000000000008201640353
+                  00
+                53           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                67           6 LOAD_FAST                0 (self)
+                54           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (update_by_id)
                             40 LOAD_FAST                1 (data)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               0 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 RETURN_VALUE
+                       >>   70 STORE_FAST               2 (affect_row)
+               
+                55          72 LOAD_FAST                2 (affect_row)
+                            74 LOAD_CONST               2 (1)
+                            76 COMPARE_OP               3 (!=)
+                            82 POP_JUMP_FORWARD_IF_FALSE    46 (to 176)
+               
+                56          84 LOAD_GLOBAL              5 (NULL + SystemException)
+               
+                57          96 LOAD_GLOBAL              6 (SystemResponseCode)
+                           108 LOAD_ATTR                4 (PARAMETER_ERROR)
+                           118 LOAD_ATTR                5 (code)
+               
+                58         128 LOAD_GLOBAL              6 (SystemResponseCode)
+                           140 LOAD_ATTR                4 (PARAMETER_ERROR)
+                           150 LOAD_ATTR                6 (msg)
+               
+                56         160 PRECALL                  2
+                           164 CALL                     2
+                           174 RAISE_VARARGS            1
+               
+                60     >>  176 LOAD_CONST               3 (True)
+                           178 RETURN_VALUE
                consts
                   None
                   ('data',)
-               names      ('mapper', 'update_by_id')
-               varnames   ('self', 'data')
+                  1
+                  True
+               names      ('mapper', 'update_by_id', 'SystemException', 'SystemResponseCode', 'PARAMETER_ERROR', 'code', 'msg')
+               varnames   ('self', 'data', 'affect_row')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'update_by_id'
-               firstlineno 66
-               lnotab 0x0601
+               firstlineno 53
+               lnotab 0x060142010c010c01200120fe1004
+            ('db_session',)
+            'ids'
+            'db_session'
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 5
+               stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386045300
-                69           0 RETURN_GENERATOR
+                  00000000000000000000007c017c02ac01a6020000ab0200000000000000
+                  00830064007b035600970386047d047405000000000000000000007c01a6
+                  010000ab0100000000000000007c046b0300000000722e74070000000000
+                  00000000007408000000000000000000006a0500000000000000006a0600
+                  000000000000007408000000000000000000006a0500000000000000006a
+                  070000000000000000a6020000ab020000000000000000820164025300
+                62           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                70           6 LOAD_FAST                0 (self)
+                65           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (update_batch_by_ids)
-                            40 LOAD_FAST                1 (data_list)
-                            42 KW_NAMES                 1
-                            44 PRECALL                  1
-                            48 CALL                     1
-                            58 GET_AWAITABLE            0
-                            60 LOAD_CONST               0 (None)
-                       >>   62 SEND                     3 (to 70)
-                            64 YIELD_VALUE
-                            66 RESUME                   3
-                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 RETURN_VALUE
+                            40 LOAD_FAST                1 (ids)
+                            42 LOAD_FAST                2 (data)
+                            44 KW_NAMES                 1
+                            46 PRECALL                  2
+                            50 CALL                     2
+                            60 GET_AWAITABLE            0
+                            62 LOAD_CONST               0 (None)
+                       >>   64 SEND                     3 (to 72)
+                            66 YIELD_VALUE
+                            68 RESUME                   3
+                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
+                       >>   72 STORE_FAST               4 (affect_row)
+               
+                66          74 LOAD_GLOBAL              5 (NULL + len)
+                            86 LOAD_FAST                1 (ids)
+                            88 PRECALL                  1
+                            92 CALL                     1
+                           102 LOAD_FAST                4 (affect_row)
+                           104 COMPARE_OP               3 (!=)
+                           110 POP_JUMP_FORWARD_IF_FALSE    46 (to 204)
+               
+                67         112 LOAD_GLOBAL              7 (NULL + SystemException)
+               
+                68         124 LOAD_GLOBAL              8 (SystemResponseCode)
+                           136 LOAD_ATTR                5 (PARAMETER_ERROR)
+                           146 LOAD_ATTR                6 (code)
+               
+                69         156 LOAD_GLOBAL              8 (SystemResponseCode)
+                           168 LOAD_ATTR                5 (PARAMETER_ERROR)
+                           178 LOAD_ATTR                7 (msg)
+               
+                67         188 PRECALL                  2
+                           192 CALL                     2
+                           202 RAISE_VARARGS            1
+               
+                71     >>  204 LOAD_CONST               2 (True)
+                           206 RETURN_VALUE
                consts
                   None
-                  ('data_list',)
-               names      ('mapper', 'update_batch_by_ids')
-               varnames   ('self', 'data_list')
+                  ('ids', 'data')
+                  True
+               names      ('mapper', 'update_batch_by_ids', 'len', 'SystemException', 'SystemResponseCode', 'PARAMETER_ERROR', 'code', 'msg')
+               varnames   ('self', 'ids', 'data', 'db_session', 'affect_row')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'update_batch_by_ids'
-               firstlineno 69
-               lnotab 0x0601
+               firstlineno 62
+               lnotab 0x0603440126010c01200120fe1004
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 3
+               stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386045300
-                72           0 RETURN_GENERATOR
+                  0064007b035600970386047d027c0264026b0300000000722e7405000000
+                  000000000000007406000000000000000000006a0400000000000000006a
+                  0500000000000000007406000000000000000000006a0400000000000000
+                  006a060000000000000000a6020000ab0200000000000000008201640353
+                  00
+                73           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                73           6 LOAD_FAST                0 (self)
+                74           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (delete_by_id)
                             40 LOAD_FAST                1 (id)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               0 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 RETURN_VALUE
+                       >>   70 STORE_FAST               2 (affect_row)
+               
+                75          72 LOAD_FAST                2 (affect_row)
+                            74 LOAD_CONST               2 (1)
+                            76 COMPARE_OP               3 (!=)
+                            82 POP_JUMP_FORWARD_IF_FALSE    46 (to 176)
+               
+                76          84 LOAD_GLOBAL              5 (NULL + SystemException)
+               
+                77          96 LOAD_GLOBAL              6 (SystemResponseCode)
+                           108 LOAD_ATTR                4 (PARAMETER_ERROR)
+                           118 LOAD_ATTR                5 (code)
+               
+                78         128 LOAD_GLOBAL              6 (SystemResponseCode)
+                           140 LOAD_ATTR                4 (PARAMETER_ERROR)
+                           150 LOAD_ATTR                6 (msg)
+               
+                76         160 PRECALL                  2
+                           164 CALL                     2
+                           174 RAISE_VARARGS            1
+               
+                80     >>  176 LOAD_CONST               3 (True)
+                           178 RETURN_VALUE
                consts
                   None
                   ('id',)
-               names      ('mapper', 'delete_by_id')
-               varnames   ('self', 'id')
+                  1
+                  True
+               names      ('mapper', 'delete_by_id', 'SystemException', 'SystemResponseCode', 'PARAMETER_ERROR', 'code', 'msg')
+               varnames   ('self', 'id', 'affect_row')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'remove_by_id'
-               firstlineno 72
-               lnotab 0x0601
+               firstlineno 73
+               lnotab 0x060142010c010c01200120fe1004
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 3
+               stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386045300
-                75           0 RETURN_GENERATOR
+                  0064007b035600970386047d027405000000000000000000007c01a60100
+                  00ab0100000000000000007c026b0300000000722e740700000000000000
+                  0000007408000000000000000000006a0500000000000000006a06000000
+                  00000000007408000000000000000000006a0500000000000000006a0700
+                  00000000000000a6020000ab020000000000000000820164025300
+                82           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                76           6 LOAD_FAST                0 (self)
+                83           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (delete_batch_by_ids)
                             40 LOAD_FAST                1 (ids)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               0 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
-                       >>   70 RETURN_VALUE
+                       >>   70 STORE_FAST               2 (affect_row)
+               
+                84          72 LOAD_GLOBAL              5 (NULL + len)
+                            84 LOAD_FAST                1 (ids)
+                            86 PRECALL                  1
+                            90 CALL                     1
+                           100 LOAD_FAST                2 (affect_row)
+                           102 COMPARE_OP               3 (!=)
+                           108 POP_JUMP_FORWARD_IF_FALSE    46 (to 202)
+               
+                85         110 LOAD_GLOBAL              7 (NULL + SystemException)
+               
+                86         122 LOAD_GLOBAL              8 (SystemResponseCode)
+                           134 LOAD_ATTR                5 (PARAMETER_ERROR)
+                           144 LOAD_ATTR                6 (code)
+               
+                87         154 LOAD_GLOBAL              8 (SystemResponseCode)
+                           166 LOAD_ATTR                5 (PARAMETER_ERROR)
+                           176 LOAD_ATTR                7 (msg)
+               
+                85         186 PRECALL                  2
+                           190 CALL                     2
+                           200 RAISE_VARARGS            1
+               
+                89     >>  202 LOAD_CONST               2 (True)
+                           204 RETURN_VALUE
                consts
                   None
                   ('ids',)
-               names      ('mapper', 'delete_batch_by_ids')
-               varnames   ('self', 'ids')
+                  True
+               names      ('mapper', 'delete_batch_by_ids', 'len', 'SystemException', 'SystemResponseCode', 'PARAMETER_ERROR', 'code', 'msg')
+               varnames   ('self', 'ids', 'affect_row')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
                name       'remove_batch_by_ids'
-               firstlineno 75
-               lnotab 0x0601
-            None
-         names      ('__name__', '__module__', '__qualname__', 'Type', 'M', '__init__', 'T', 'bool', 'save', 'save_or_update', 'List', 'save_batch', 'save_or_update_batch', 'get_by_id', 'int', 'Any', 'get_by_ids', 'count', 'list', 'list_ordered', 'list_page', 'list_page_ordered', 'update_by_id', 'update_batch_by_ids', 'remove_by_id', 'remove_batch_by_ids')
+               firstlineno 82
+               lnotab 0x0601420126010c01200120fe1004
+         names      ('__name__', '__module__', '__qualname__', 'Type', 'M', '__init__', 'T', 'save', 'List', 'bool', 'save_batch', 'get_by_id', 'int', 'count', 'list', 'list_ordered', 'list_page', 'list_page_ordered', 'update_by_id', 'Any', 'dict', 'update_batch_by_ids', 'remove_by_id', 'remove_batch_by_ids')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
          name       'ServiceImpl'
-         firstlineno 12
+         firstlineno 14
          lnotab
-            0x0a011803100410071c041c08100332030c032403020102ff020102ff02
-            0102ff020102ff020102ff02020efe08072003240510031c031003
+            0x0a01180310031c0410030c032008020102fa060302fd020402fc020502
+            fb020602fa02080ef8080d1c032203100a02ff06010eff020102ff020102
+            ff020202fe080b1009
       'ServiceImpl'
       None
-   names      ('__doc__', 'typing', 'Any', 'TypeVar', 'List', 'Generic', 'Type', 'fss.common.persistence.base_mapper', 'BaseMapper', 'fss.common.service.service', 'Service', 'T', 'M', 'ServiceImpl')
+   names      ('__doc__', 'typing', 'Any', 'TypeVar', 'List', 'Generic', 'Type', 'fss.common.persistence.base_mapper', 'BaseMapper', 'fss.common.service.service', 'Service', 'fss.starter.system.enum.system', 'SystemResponseCode', 'fss.starter.system.exception.system', 'SystemException', 'T', 'M', 'ServiceImpl')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\service\\impl\\service_impl.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\common\\service\\impl\\service_impl.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104021c020c010c021a011a03
+   lnotab 0x00ff020104021c020c010c010c010c021a011a03
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/excel.py` & `fastapi_sqlmodel_starter-1.0.1/fss/common/util/excel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+"""Excel util"""
+
 import io
 from datetime import datetime
 from typing import List
 
 import pandas as pd
 from loguru import logger
 from pydantic import BaseModel
 from starlette.responses import StreamingResponse
 
 
 async def export_template(
     schema: BaseModel, file_name: str, data_list: List[BaseModel] = None
 ) -> StreamingResponse:
     """
-    Export template or date
+    Export template or template with date
     """
     global excel_writer
-    field_names = schema.__fields__
+    field_names = schema.model_fields
     user_export_df = pd.DataFrame(columns=field_names)
     if data_list is not None:
-        data_dicts = [item.dict() for item in data_list]
+        data_dicts = [item.model_dump() for item in data_list]
         user_export_df = user_export_df._append(data_dicts, ignore_index=True)
     filename = f"{file_name}_{datetime.now().strftime('%Y%m%d%H%M%S')}.xlsx"
     stream = io.BytesIO()
     try:
         excel_writer = pd.ExcelWriter(stream, engine="xlsxwriter")
         user_export_df.to_excel(excel_writer, index=False)
         excel_writer._save()
@@ -30,9 +32,7 @@
         return StreamingResponse(
             io.BytesIO(stream.getvalue()),
             media_type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
             headers={"Content-Disposition": f"attachment; filename={filename}"},
         )
     except Exception as e:
         logger.error(f"{e}")
-    finally:
-        excel_writer.close()
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,25 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 4684
+moddate:  0x242d2266 (Fri Apr 19 08:36:52 2024 UTC)
+files sz: 4942
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a046d
       055a056d065a060100640164046c076d085a080100640164056c096d0a5a
       0a0100640164066c0b6d0c5a0c6d0d5a0d0100640164076c0e6d0f5a0f6d
-      105a100100640164086c116d125a120100640164096c136d145a14010009
-      006401640a6c0b6d155a1501006e11230065162400720901006401640b6c
-      176d185a15010059006e047700780359007701640c84005a1902006519a6
-      000000ab0000000000000000005c0200005a1a5a1b02004700640d840064
-      0e651ca6030000ab0300000000000000005a1d02004700640f8400641065
-      1ca6030000ab0300000000000000005a1e64115300
+      105a100100640164086c116d125a120100640164096c136d145a14010064
+      01640a6c156d165a1601006401640b6c176d185a18010009006401640c6c
+      0b6d195a1901006e112300651a2400720901006401640d6c1b6d1c5a1901
+      0059006e047700780359007701640e84005a1d0200651da6000000ab0000
+      000000000000005c0200005a1e5a1f02004700640f840064106520a60300
+      00ab0300000000000000005a21020047006411840064126520a6030000ab
+      0300000000000000005a22020065186a230000000000000000651e020065
+      2465166a250000000000000000a6010000ab010000000000000000641365
+      166a2600000000000000006901ac14a6030000ab03000000000000000001
+      0064155300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Session proxy used in the project')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('ContextVar',))
@@ -81,92 +85,132 @@
     11         106 LOAD_CONST               1 (0)
                108 LOAD_CONST               9 (('ASGIApp',))
                110 IMPORT_NAME             19 (starlette.types)
                112 IMPORT_FROM             20 (ASGIApp)
                114 STORE_NAME              20 (ASGIApp)
                116 POP_TOP
    
-    14         118 NOP
+    13         118 LOAD_CONST               1 (0)
+               120 LOAD_CONST              10 (('configs',))
+               122 IMPORT_NAME             21 (fss.common.config)
+               124 IMPORT_FROM             22 (configs)
+               126 STORE_NAME              22 (configs)
+               128 POP_TOP
    
-    15         120 LOAD_CONST               1 (0)
-               122 LOAD_CONST              10 (('async_sessionmaker',))
-               124 IMPORT_NAME             11 (sqlalchemy.ext.asyncio)
-               126 IMPORT_FROM             21 (async_sessionmaker)
-               128 STORE_NAME              21 (async_sessionmaker)
-               130 POP_TOP
-               132 JUMP_FORWARD            17 (to 168)
-           >>  134 PUSH_EXC_INFO
-   
-    16         136 LOAD_NAME               22 (ImportError)
-               138 CHECK_EXC_MATCH
-               140 POP_JUMP_FORWARD_IF_FALSE     9 (to 160)
-               142 POP_TOP
+    14         130 LOAD_CONST               1 (0)
+               132 LOAD_CONST              11 (('app',))
+               134 IMPORT_NAME             23 (fss.starter.server)
+               136 IMPORT_FROM             24 (app)
+               138 STORE_NAME              24 (app)
+               140 POP_TOP
+   
+    16         142 NOP
    
     17         144 LOAD_CONST               1 (0)
-               146 LOAD_CONST              11 (('sessionmaker',))
-               148 IMPORT_NAME             23 (sqlalchemy.orm)
-               150 IMPORT_FROM             24 (sessionmaker)
-               152 STORE_NAME              21 (async_sessionmaker)
+               146 LOAD_CONST              12 (('async_sessionmaker',))
+               148 IMPORT_NAME             11 (sqlalchemy.ext.asyncio)
+               150 IMPORT_FROM             25 (async_sessionmaker)
+               152 STORE_NAME              25 (async_sessionmaker)
                154 POP_TOP
-               156 POP_EXCEPT
-               158 JUMP_FORWARD             4 (to 168)
+               156 JUMP_FORWARD            17 (to 192)
+           >>  158 PUSH_EXC_INFO
+   
+    18         160 LOAD_NAME               26 (ImportError)
+               162 CHECK_EXC_MATCH
+               164 POP_JUMP_FORWARD_IF_FALSE     9 (to 184)
+               166 POP_TOP
+   
+    19         168 LOAD_CONST               1 (0)
+               170 LOAD_CONST              13 (('sessionmaker',))
+               172 IMPORT_NAME             27 (sqlalchemy.orm)
+               174 IMPORT_FROM             28 (sessionmaker)
+               176 STORE_NAME              25 (async_sessionmaker)
+               178 POP_TOP
+               180 POP_EXCEPT
+               182 JUMP_FORWARD             4 (to 192)
+   
+    18     >>  184 RERAISE                  0
+           >>  186 COPY                     3
+               188 POP_EXCEPT
+               190 RERAISE                  1
+   
+    22     >>  192 LOAD_CONST              14 (<code object create_middleware_and_session_proxy, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 22>)
+               194 MAKE_FUNCTION            0
+               196 STORE_NAME              29 (create_middleware_and_session_proxy)
+   
+   105         198 PUSH_NULL
+               200 LOAD_NAME               29 (create_middleware_and_session_proxy)
+               202 PRECALL                  0
+               206 CALL                     0
+               216 UNPACK_SEQUENCE          2
+               220 STORE_NAME              30 (SQLAlchemyMiddleware)
+               222 STORE_NAME              31 (db)
+   
+   108         224 PUSH_NULL
+               226 LOAD_BUILD_CLASS
+               228 LOAD_CONST              15 (<code object MissingSessionException, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 108>)
+               230 MAKE_FUNCTION            0
+               232 LOAD_CONST              16 ('MissingSessionException')
+               234 LOAD_NAME               32 (Exception)
+               236 PRECALL                  3
+               240 CALL                     3
+               250 STORE_NAME              33 (MissingSessionException)
+   
+   126         252 PUSH_NULL
+               254 LOAD_BUILD_CLASS
+               256 LOAD_CONST              17 (<code object SessionNotInitialisedException, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 126>)
+               258 MAKE_FUNCTION            0
+               260 LOAD_CONST              18 ('SessionNotInitialisedException')
+               262 LOAD_NAME               32 (Exception)
+               264 PRECALL                  3
+               268 CALL                     3
+               278 STORE_NAME              34 (SessionNotInitialisedException)
+   
+   141         280 PUSH_NULL
+               282 LOAD_NAME               24 (app)
+               284 LOAD_ATTR               35 (add_middleware)
+   
+   142         294 LOAD_NAME               30 (SQLAlchemyMiddleware)
+   
+   143         296 PUSH_NULL
+               298 LOAD_NAME               36 (str)
+               300 LOAD_NAME               22 (configs)
+               302 LOAD_ATTR               37 (sqlalchemy_database_url)
+               312 PRECALL                  1
+               316 CALL                     1
+   
+   145         326 LOAD_CONST              19 ('echo')
+               328 LOAD_NAME               22 (configs)
+               330 LOAD_ATTR               38 (echo_sql)
+   
+   144         340 BUILD_MAP                1
    
-    16     >>  160 RERAISE                  0
-           >>  162 COPY                     3
-               164 POP_EXCEPT
-               166 RERAISE                  1
-   
-    20     >>  168 LOAD_CONST              12 (<code object create_middleware_and_session_proxy, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 20>)
-               170 MAKE_FUNCTION            0
-               172 STORE_NAME              25 (create_middleware_and_session_proxy)
-   
-   103         174 PUSH_NULL
-               176 LOAD_NAME               25 (create_middleware_and_session_proxy)
-               178 PRECALL                  0
-               182 CALL                     0
-               192 UNPACK_SEQUENCE          2
-               196 STORE_NAME              26 (SQLAlchemyMiddleware)
-               198 STORE_NAME              27 (db)
-   
-   106         200 PUSH_NULL
-               202 LOAD_BUILD_CLASS
-               204 LOAD_CONST              13 (<code object MissingSessionException, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 106>)
-               206 MAKE_FUNCTION            0
-               208 LOAD_CONST              14 ('MissingSessionException')
-               210 LOAD_NAME               28 (Exception)
-               212 PRECALL                  3
-               216 CALL                     3
-               226 STORE_NAME              29 (MissingSessionException)
-   
-   124         228 PUSH_NULL
-               230 LOAD_BUILD_CLASS
-               232 LOAD_CONST              15 (<code object SessionNotInitialisedException, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 124>)
-               234 MAKE_FUNCTION            0
-               236 LOAD_CONST              16 ('SessionNotInitialisedException')
-               238 LOAD_NAME               28 (Exception)
-               240 PRECALL                  3
-               244 CALL                     3
-               254 STORE_NAME              30 (SessionNotInitialisedException)
-               256 LOAD_CONST              17 (None)
-               258 RETURN_VALUE
+   141         342 KW_NAMES                20
+               344 PRECALL                  3
+               348 CALL                     3
+               358 POP_TOP
+               360 LOAD_CONST              21 (None)
+               362 RETURN_VALUE
    ExceptionTable:
-     120 to 130 -> 134 [0]
-     134 to 154 -> 162 [1] lasti
-     160 to 160 -> 162 [1] lasti
+     144 to 154 -> 158 [0]
+     158 to 178 -> 186 [1] lasti
+     184 to 184 -> 186 [1] lasti
    consts
       'Session proxy used in the project'
       0
       ('ContextVar',)
       ('Dict', 'Optional', 'Union')
       ('Engine',)
       ('URL',)
       ('AsyncSession', 'create_async_engine')
       ('BaseHTTPMiddleware', 'RequestResponseEndpoint')
       ('Request',)
       ('ASGIApp',)
+      ('configs',)
+      ('app',)
       ('async_sessionmaker',)
       ('sessionmaker',)
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 5
          flags     : 3
@@ -177,68 +221,68 @@
             0002004700880388046602640584086406740400000000000000000000a6
             030000ab0300000000000000007d01020047008803880466026407840864
             087c01ac09a6030000ab0300000000000000008a027c00890266025300
                        0 MAKE_CELL                2 (DBSession)
                        2 MAKE_CELL                3 (_Session)
                        4 MAKE_CELL                4 (_session)
          
-          20           6 RESUME                   0
+          22           6 RESUME                   0
          
-          21           8 LOAD_CONST               0 (None)
+          23           8 LOAD_CONST               0 (None)
                       10 STORE_DEREF              3 (_Session)
          
-          25          12 LOAD_GLOBAL              1 (NULL + ContextVar)
+          27          12 LOAD_GLOBAL              1 (NULL + ContextVar)
                       24 LOAD_CONST               1 ('_session')
                       26 LOAD_CONST               0 (None)
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_DEREF              4 (_session)
          
-          27          46 PUSH_NULL
+          29          46 PUSH_NULL
                       48 LOAD_BUILD_CLASS
                       50 LOAD_CLOSURE             2 (DBSession)
                       52 LOAD_CLOSURE             3 (_Session)
                       54 BUILD_TUPLE              2
-                      56 LOAD_CONST               3 (<code object SQLAlchemyMiddleware, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 27>)
+                      56 LOAD_CONST               3 (<code object SQLAlchemyMiddleware, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 29>)
                       58 MAKE_FUNCTION            8 (closure)
                       60 LOAD_CONST               4 ('SQLAlchemyMiddleware')
                       62 LOAD_GLOBAL              2 (BaseHTTPMiddleware)
                       74 PRECALL                  3
                       78 CALL                     3
                       88 STORE_FAST               0 (SQLAlchemyMiddleware)
          
-          60          90 PUSH_NULL
+          62          90 PUSH_NULL
                       92 LOAD_BUILD_CLASS
                       94 LOAD_CLOSURE             3 (_Session)
                       96 LOAD_CLOSURE             4 (_session)
                       98 BUILD_TUPLE              2
-                     100 LOAD_CONST               5 (<code object DBSessionMeta, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 60>)
+                     100 LOAD_CONST               5 (<code object DBSessionMeta, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 62>)
                      102 MAKE_FUNCTION            8 (closure)
                      104 LOAD_CONST               6 ('DBSessionMeta')
                      106 LOAD_GLOBAL              4 (type)
                      118 PRECALL                  3
                      122 CALL                     3
                      132 STORE_FAST               1 (DBSessionMeta)
          
-          73         134 PUSH_NULL
+          75         134 PUSH_NULL
                      136 LOAD_BUILD_CLASS
                      138 LOAD_CLOSURE             3 (_Session)
                      140 LOAD_CLOSURE             4 (_session)
                      142 BUILD_TUPLE              2
-                     144 LOAD_CONST               7 (<code object DBSession, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 73>)
+                     144 LOAD_CONST               7 (<code object DBSession, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 75>)
                      146 MAKE_FUNCTION            8 (closure)
                      148 LOAD_CONST               8 ('DBSession')
                      150 LOAD_FAST                1 (DBSessionMeta)
                      152 KW_NAMES                 9
                      154 PRECALL                  3
                      158 CALL                     3
                      168 STORE_DEREF              2 (DBSession)
          
-         100         170 LOAD_FAST                0 (SQLAlchemyMiddleware)
+         102         170 LOAD_FAST                0 (SQLAlchemyMiddleware)
                      172 LOAD_DEREF               2 (DBSession)
                      174 BUILD_TUPLE              2
                      176 RETURN_VALUE
          consts
             None
             '_session'
             ('default',)
@@ -252,79 +296,79 @@
                   036404650465056506650766021900000000000000000019000000000000
                   000000640565046508190000000000000000006406650964076509640865
                   0a660c8802880066026409840d5a0b640a650c640b650d66048801660164
                   0c840c5a0e880078015a0f5300
                              0 COPY_FREE_VARS           2
                              2 MAKE_CELL                0 (__class__)
                
-                27           4 RESUME                   0
+                29           4 RESUME                   0
                              6 LOAD_NAME                0 (__name__)
                              8 STORE_NAME               1 (__module__)
                             10 LOAD_CONST               0 ('create_middleware_and_session_proxy.<locals>.SQLAlchemyMiddleware')
                             12 STORE_NAME               2 (__qualname__)
                
-                31          14 NOP
+                33          14 NOP
                
-                32          16 NOP
+                34          16 NOP
                
-                33          18 NOP
+                35          18 NOP
                
-                34          20 NOP
+                36          20 NOP
                
-                35          22 NOP
+                37          22 NOP
                
-                28          24 LOAD_CONST              13 ((None, None, None, None, True))
+                30          24 LOAD_CONST              13 ((None, None, None, None, True))
                             26 LOAD_CONST               3 ('app')
                
-                30          28 LOAD_NAME                3 (ASGIApp)
+                32          28 LOAD_NAME                3 (ASGIApp)
                
-                28          30 LOAD_CONST               4 ('db_url')
+                30          30 LOAD_CONST               4 ('db_url')
                
-                31          32 LOAD_NAME                4 (Optional)
+                33          32 LOAD_NAME                4 (Optional)
                             34 LOAD_NAME                5 (Union)
                             36 LOAD_NAME                6 (str)
                             38 LOAD_NAME                7 (URL)
                             40 BUILD_TUPLE              2
                             42 BINARY_SUBSCR
                             52 BINARY_SUBSCR
                
-                28          62 LOAD_CONST               5 ('custom_engine')
+                30          62 LOAD_CONST               5 ('custom_engine')
                
-                32          64 LOAD_NAME                4 (Optional)
+                34          64 LOAD_NAME                4 (Optional)
                             66 LOAD_NAME                8 (Engine)
                             68 BINARY_SUBSCR
                
-                28          78 LOAD_CONST               6 ('engine_args')
+                30          78 LOAD_CONST               6 ('engine_args')
                
-                33          80 LOAD_NAME                9 (Dict)
+                35          80 LOAD_NAME                9 (Dict)
                
-                28          82 LOAD_CONST               7 ('session_args')
+                30          82 LOAD_CONST               7 ('session_args')
                
-                34          84 LOAD_NAME                9 (Dict)
+                36          84 LOAD_NAME                9 (Dict)
                
-                28          86 LOAD_CONST               8 ('commit_on_exit')
+                30          86 LOAD_CONST               8 ('commit_on_exit')
                
-                35          88 LOAD_NAME               10 (bool)
+                37          88 LOAD_NAME               10 (bool)
                
-                28          90 BUILD_TUPLE             12
+                30          90 BUILD_TUPLE             12
                             92 LOAD_CLOSURE             2 (_Session)
                             94 LOAD_CLOSURE             0 (__class__)
                             96 BUILD_TUPLE              2
-                            98 LOAD_CONST               9 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 28>)
+                            98 LOAD_CONST               9 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 30>)
                            100 MAKE_FUNCTION           13 (defaults, annotations, closure)
                            102 STORE_NAME              11 (__init__)
                
-                56         104 LOAD_CONST              10 ('request')
+                58         104 LOAD_CONST              10 ('request')
                            106 LOAD_NAME               12 (Request)
                            108 LOAD_CONST              11 ('call_next')
                            110 LOAD_NAME               13 (RequestResponseEndpoint)
                            112 BUILD_TUPLE              4
                            114 LOAD_CLOSURE             1 (DBSession)
                            116 BUILD_TUPLE              1
-                           118 LOAD_CONST              12 (<code object dispatch, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 56>)
+                           118 LOAD_CONST              12 (<code object dispatch, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 58>)
                            120 MAKE_FUNCTION           12 (annotations, closure)
                            122 STORE_NAME              14 (dispatch)
                            124 LOAD_CLOSURE             0 (__class__)
                            126 COPY                     1
                            128 STORE_NAME              15 (__classcell__)
                            130 RETURN_VALUE
                consts
@@ -349,99 +393,99 @@
                         007d047c05700169007d057c0373117c02730f7407000000000000000000
                         006401a6010000ab01000000000000000082017c03730e74090000000000
                         00000000007c02660169007c04a4018e017d076e027c037d07740b000000
                         000000000000007c076601740c00000000000000000000640264039c027c
                         05a4018e018a0864005300
                                    0 COPY_FREE_VARS           2
                      
-                      28           2 RESUME                   0
+                      30           2 RESUME                   0
                      
-                      37           4 LOAD_GLOBAL              1 (NULL + super)
+                      39           4 LOAD_GLOBAL              1 (NULL + super)
                                   16 PRECALL                  0
                                   20 CALL                     0
                                   30 LOAD_METHOD              1 (__init__)
                                   52 LOAD_FAST                1 (app)
                                   54 PRECALL                  1
                                   58 CALL                     1
                                   68 POP_TOP
                      
-                      38          70 LOAD_FAST                6 (commit_on_exit)
+                      40          70 LOAD_FAST                6 (commit_on_exit)
                                   72 LOAD_FAST                0 (self)
                                   74 STORE_ATTR               2 (commit_on_exit)
                      
-                      39          84 LOAD_FAST                4 (engine_args)
+                      41          84 LOAD_FAST                4 (engine_args)
                                   86 JUMP_IF_TRUE_OR_POP      1 (to 90)
                                   88 BUILD_MAP                0
                              >>   90 STORE_FAST               4 (engine_args)
                      
-                      40          92 LOAD_FAST                5 (session_args)
+                      42          92 LOAD_FAST                5 (session_args)
                                   94 JUMP_IF_TRUE_OR_POP      1 (to 98)
                                   96 BUILD_MAP                0
                              >>   98 STORE_FAST               5 (session_args)
                      
-                      42         100 LOAD_FAST                3 (custom_engine)
+                      44         100 LOAD_FAST                3 (custom_engine)
                                  102 POP_JUMP_FORWARD_IF_TRUE    17 (to 138)
                                  104 LOAD_FAST                2 (db_url)
                                  106 POP_JUMP_FORWARD_IF_TRUE    15 (to 138)
                      
-                      43         108 LOAD_GLOBAL              7 (NULL + ValueError)
+                      45         108 LOAD_GLOBAL              7 (NULL + ValueError)
                      
-                      44         120 LOAD_CONST               1 ('You need to pass a db_url or a custom_engine parameter.')
+                      46         120 LOAD_CONST               1 ('You need to pass a db_url or a custom_engine parameter.')
                      
-                      43         122 PRECALL                  1
+                      45         122 PRECALL                  1
                                  126 CALL                     1
                                  136 RAISE_VARARGS            1
                      
-                      46     >>  138 LOAD_FAST                3 (custom_engine)
+                      48     >>  138 LOAD_FAST                3 (custom_engine)
                                  140 POP_JUMP_FORWARD_IF_TRUE    14 (to 170)
                      
-                      47         142 LOAD_GLOBAL              9 (NULL + create_async_engine)
+                      49         142 LOAD_GLOBAL              9 (NULL + create_async_engine)
                                  154 LOAD_FAST                2 (db_url)
                                  156 BUILD_TUPLE              1
                                  158 BUILD_MAP                0
                                  160 LOAD_FAST                4 (engine_args)
                                  162 DICT_MERGE               1
                                  164 CALL_FUNCTION_EX         1
                                  166 STORE_FAST               7 (engine)
                                  168 JUMP_FORWARD             2 (to 174)
                      
-                      49     >>  170 LOAD_FAST                3 (custom_engine)
+                      51     >>  170 LOAD_FAST                3 (custom_engine)
                                  172 STORE_FAST               7 (engine)
                      
-                      52     >>  174 LOAD_GLOBAL             11 (NULL + async_sessionmaker)
+                      54     >>  174 LOAD_GLOBAL             11 (NULL + async_sessionmaker)
                      
-                      53         186 LOAD_FAST                7 (engine)
+                      55         186 LOAD_FAST                7 (engine)
                      
-                      52         188 BUILD_TUPLE              1
+                      54         188 BUILD_TUPLE              1
                      
-                      53         190 LOAD_GLOBAL             12 (AsyncSession)
+                      55         190 LOAD_GLOBAL             12 (AsyncSession)
                                  202 LOAD_CONST               2 (False)
                      
-                      52         204 LOAD_CONST               3 (('class_', 'expire_on_commit'))
+                      54         204 LOAD_CONST               3 (('class_', 'expire_on_commit'))
                                  206 BUILD_CONST_KEY_MAP      2
                      
-                      53         208 LOAD_FAST                5 (session_args)
+                      55         208 LOAD_FAST                5 (session_args)
                      
-                      52         210 DICT_MERGE               1
+                      54         210 DICT_MERGE               1
                                  212 CALL_FUNCTION_EX         1
                                  214 STORE_DEREF              8 (_Session)
                                  216 LOAD_CONST               0 (None)
                                  218 RETURN_VALUE
                      consts
                         None
                         'You need to pass a db_url or a custom_engine parameter.'
                         False
                         ('class_', 'expire_on_commit')
                      names      ('super', '__init__', 'commit_on_exit', 'ValueError', 'create_async_engine', 'async_sessionmaker', 'AsyncSession')
                      varnames   ('self', 'app', 'db_url', 'custom_engine', 'engine_args', 'session_args', 'commit_on_exit', 'engine')
                      freevars   ('_Session', '__class__')
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       '__init__'
-                     firstlineno 28
+                     firstlineno 30
                      lnotab
                         0x040942010e010801080208010c0102ff100304011c0204030c0102ff02
                         010eff040102ff
                   'request'
                   'call_next'
                   code
                      argcount  : 3
@@ -453,19 +497,19 @@
                         00ab0100000000000000003400830164007b03560097038604010002007c
                         027c01a6010000ab010000000000000000830064007b0356009703860463
                         02640064006400a6020000ab020000000000000000830264007b03560097
                         0386040100530023003100830264007b0356009703860473047702780359
                         007701010059000100010064005300
                                    0 COPY_FREE_VARS           1
                      
-                      56           2 RETURN_GENERATOR
+                      58           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                      57           8 PUSH_NULL
+                      59           8 PUSH_NULL
                                   10 LOAD_DEREF               3 (DBSession)
                                   12 LOAD_FAST                0 (self)
                                   14 LOAD_ATTR                0 (commit_on_exit)
                                   24 KW_NAMES                 1
                                   26 PRECALL                  1
                                   30 CALL                     1
                                   40 BEFORE_ASYNC_WITH
@@ -473,27 +517,27 @@
                                   44 LOAD_CONST               0 (None)
                              >>   46 SEND                     3 (to 54)
                                   48 YIELD_VALUE
                                   50 RESUME                   3
                                   52 JUMP_BACKWARD_NO_INTERRUPT     4 (to 46)
                              >>   54 POP_TOP
                      
-                      58          56 PUSH_NULL
+                      60          56 PUSH_NULL
                                   58 LOAD_FAST                2 (call_next)
                                   60 LOAD_FAST                1 (request)
                                   62 PRECALL                  1
                                   66 CALL                     1
                                   76 GET_AWAITABLE            0
                                   78 LOAD_CONST               0 (None)
                              >>   80 SEND                     3 (to 88)
                                   82 YIELD_VALUE
                                   84 RESUME                   3
                                   86 JUMP_BACKWARD_NO_INTERRUPT     4 (to 80)
                      
-                      57     >>   88 SWAP                     2
+                      59     >>   88 SWAP                     2
                                   90 LOAD_CONST               0 (None)
                                   92 LOAD_CONST               0 (None)
                                   94 LOAD_CONST               0 (None)
                                   96 PRECALL                  2
                                  100 CALL                     2
                                  110 GET_AWAITABLE            2
                                  112 LOAD_CONST               0 (None)
@@ -529,61 +573,61 @@
                      consts
                         None
                         ('commit_on_exit',)
                      names      ('commit_on_exit',)
                      varnames   ('self', 'request', 'call_next')
                      freevars   ('DBSession',)
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       'dispatch'
-                     firstlineno 56
+                     firstlineno 58
                      lnotab 0x0801300120ff
                   (None, None, None, None, True)
                names      ('__name__', '__module__', '__qualname__', 'ASGIApp', 'Optional', 'Union', 'str', 'URL', 'Engine', 'Dict', 'bool', '__init__', 'Request', 'RequestResponseEndpoint', 'dispatch', '__classcell__')
                varnames   ()
                freevars   ('DBSession', '_Session')
                cellvars   ('__class__',)
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                name       'SQLAlchemyMiddleware'
-               firstlineno 27
+               firstlineno 29
                lnotab
                   0x0e04020102010201020102f9040202fe02031efd02040efc020502fb02
                   0602fa020702f90e1c
             'SQLAlchemyMiddleware'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x9502970065005a0164005a026503640165046602880088016602640284
                   0ca6000000ab0000000000000000005a0564035300
                              0 COPY_FREE_VARS           2
                
-                60           2 RESUME                   0
+                62           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create_middleware_and_session_proxy.<locals>.DBSessionMeta')
                             10 STORE_NAME               2 (__qualname__)
                
-                61          12 LOAD_NAME                3 (property)
+                63          12 LOAD_NAME                3 (property)
                
-                62          14 LOAD_CONST               1 ('return')
+                64          14 LOAD_CONST               1 ('return')
                             16 LOAD_NAME                4 (AsyncSession)
                             18 BUILD_TUPLE              2
                             20 LOAD_CLOSURE             0 (_Session)
                             22 LOAD_CLOSURE             1 (_session)
                             24 BUILD_TUPLE              2
-                            26 LOAD_CONST               2 (<code object session, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 61>)
+                            26 LOAD_CONST               2 (<code object session, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 63>)
                             28 MAKE_FUNCTION           12 (annotations, closure)
                
-                61          30 PRECALL                  0
+                63          30 PRECALL                  0
                             34 CALL                     0
                
-                62          44 STORE_NAME               5 (session)
+                64          44 STORE_NAME               5 (session)
                             46 LOAD_CONST               3 (None)
                             48 RETURN_VALUE
                consts
                   'create_middleware_and_session_proxy.<locals>.DBSessionMeta'
                   'return'
                   code
                      argcount  : 1
@@ -592,92 +636,92 @@
                      flags     : 19
                      code
                         0x950297008902800774000000000000000000000082018903a001000000
                         0000000000000000000000000000000000a6000000ab0000000000000000
                         007d017c01800774040000000000000000000082017c015300
                                    0 COPY_FREE_VARS           2
                      
-                      61           2 RESUME                   0
+                      63           2 RESUME                   0
                      
-                      64           4 LOAD_DEREF               2 (_Session)
+                      66           4 LOAD_DEREF               2 (_Session)
                                    6 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 22)
                      
-                      65           8 LOAD_GLOBAL              0 (SessionNotInitialisedException)
+                      67           8 LOAD_GLOBAL              0 (SessionNotInitialisedException)
                                   20 RAISE_VARARGS            1
                      
-                      67     >>   22 LOAD_DEREF               3 (_session)
+                      69     >>   22 LOAD_DEREF               3 (_session)
                                   24 LOAD_METHOD              1 (get)
                                   46 PRECALL                  0
                                   50 CALL                     0
                                   60 STORE_FAST               1 (session)
                      
-                      68          62 LOAD_FAST                1 (session)
+                      70          62 LOAD_FAST                1 (session)
                                   64 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 80)
                      
-                      69          66 LOAD_GLOBAL              4 (MissingSessionException)
+                      71          66 LOAD_GLOBAL              4 (MissingSessionException)
                                   78 RAISE_VARARGS            1
                      
-                      71     >>   80 LOAD_FAST                1 (session)
+                      73     >>   80 LOAD_FAST                1 (session)
                                   82 RETURN_VALUE
                      consts
                         'Return an instance of Session local to the current async context.'
                      names      ('SessionNotInitialisedException', 'get', 'MissingSessionException')
                      varnames   ('self', 'session')
                      freevars   ('_Session', '_session')
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       'session'
-                     firstlineno 61
+                     firstlineno 63
                      lnotab 0x040304010e02280104010e02
                   None
                names      ('__name__', '__module__', '__qualname__', 'property', 'AsyncSession', 'session')
                varnames   ()
                freevars   ('_Session', '_session')
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                name       'DBSessionMeta'
-               firstlineno 60
+               firstlineno 62
                lnotab 0x0c01020110ff0e01
             'DBSessionMeta'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 5
                flags     : 0
                code
                   0x9502970065005a0164005a02640864036503640465046604640584055a
                   05880088016602640684085a0688016601640784085a0764015300
                              0 COPY_FREE_VARS           2
                
-                73           2 RESUME                   0
+                75           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create_middleware_and_session_proxy.<locals>.DBSession')
                             10 STORE_NAME               2 (__qualname__)
                
-                74          12 LOAD_CONST               8 ((None, False))
+                76          12 LOAD_CONST               8 ((None, False))
                             14 LOAD_CONST               3 ('session_args')
                             16 LOAD_NAME                3 (Dict)
                             18 LOAD_CONST               4 ('commit_on_exit')
                             20 LOAD_NAME                4 (bool)
                             22 BUILD_TUPLE              4
-                            24 LOAD_CONST               5 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 74>)
+                            24 LOAD_CONST               5 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 76>)
                             26 MAKE_FUNCTION            5 (defaults, annotations)
                             28 STORE_NAME               5 (__init__)
                
-                79          30 LOAD_CLOSURE             0 (_Session)
+                81          30 LOAD_CLOSURE             0 (_Session)
                             32 LOAD_CLOSURE             1 (_session)
                             34 BUILD_TUPLE              2
-                            36 LOAD_CONST               6 (<code object __aenter__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 79>)
+                            36 LOAD_CONST               6 (<code object __aenter__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 81>)
                             38 MAKE_FUNCTION            8 (closure)
                             40 STORE_NAME               6 (__aenter__)
                
-                86          42 LOAD_CLOSURE             1 (_session)
+                88          42 LOAD_CLOSURE             1 (_session)
                             44 BUILD_TUPLE              1
-                            46 LOAD_CONST               7 (<code object __aexit__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 86>)
+                            46 LOAD_CONST               7 (<code object __aexit__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 88>)
                             48 MAKE_FUNCTION            8 (closure)
                             50 STORE_NAME               7 (__aexit__)
                             52 LOAD_CONST               1 (None)
                             54 RETURN_VALUE
                consts
                   'create_middleware_and_session_proxy.<locals>.DBSession'
                   None
@@ -688,40 +732,40 @@
                      argcount  : 3
                      nlocals   : 3
                      stacksize : 2
                      flags     : 19
                      code
                         0x970064007c005f0000000000000000007c01700169007c005f01000000
                         00000000007c027c005f02000000000000000064005300
-                      74           0 RESUME                   0
+                      76           0 RESUME                   0
                      
-                      75           2 LOAD_CONST               0 (None)
+                      77           2 LOAD_CONST               0 (None)
                                    4 LOAD_FAST                0 (self)
                                    6 STORE_ATTR               0 (token)
                      
-                      76          16 LOAD_FAST                1 (session_args)
+                      78          16 LOAD_FAST                1 (session_args)
                                   18 JUMP_IF_TRUE_OR_POP      1 (to 22)
                                   20 BUILD_MAP                0
                              >>   22 LOAD_FAST                0 (self)
                                   24 STORE_ATTR               1 (session_args)
                      
-                      77          34 LOAD_FAST                2 (commit_on_exit)
+                      79          34 LOAD_FAST                2 (commit_on_exit)
                                   36 LOAD_FAST                0 (self)
                                   38 STORE_ATTR               2 (commit_on_exit)
                                   48 LOAD_CONST               0 (None)
                                   50 RETURN_VALUE
                      consts
                         None
                      names      ('token', 'session_args', 'commit_on_exit')
                      varnames   ('self', 'session_args', 'commit_on_exit')
                      freevars   ()
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       '__init__'
-                     firstlineno 74
+                     firstlineno 76
                      lnotab 0x02010e011201
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 7
                      flags     : 147
                      code
@@ -729,58 +773,58 @@
                         0000000000a6020000ab0200000000000000007307740400000000000000
                         00000082018902a003000000000000000000000000000000000000000002
                         008901640169007c006a040000000000000000a4018e01a6010000ab0100
                         000000000000007c005f050000000000000000740d000000000000000000
                         007c00a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           2
                      
-                      79           2 RETURN_GENERATOR
+                      81           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                      80           8 LOAD_GLOBAL              1 (NULL + isinstance)
+                      82           8 LOAD_GLOBAL              1 (NULL + isinstance)
                                   20 LOAD_DEREF               1 (_Session)
                                   22 LOAD_GLOBAL              2 (async_sessionmaker)
                                   34 PRECALL                  2
                                   38 CALL                     2
                                   48 POP_JUMP_FORWARD_IF_TRUE     7 (to 64)
                      
-                      81          50 LOAD_GLOBAL              4 (SessionNotInitialisedException)
+                      83          50 LOAD_GLOBAL              4 (SessionNotInitialisedException)
                                   62 RAISE_VARARGS            1
                      
-                      83     >>   64 LOAD_DEREF               2 (_session)
+                      85     >>   64 LOAD_DEREF               2 (_session)
                                   66 LOAD_METHOD              3 (set)
                                   88 PUSH_NULL
                                   90 LOAD_DEREF               1 (_Session)
                                   92 LOAD_CONST               1 (())
                                   94 BUILD_MAP                0
                                   96 LOAD_FAST                0 (self)
                                   98 LOAD_ATTR                4 (session_args)
                                  108 DICT_MERGE               1
                                  110 CALL_FUNCTION_EX         1
                                  112 PRECALL                  1
                                  116 CALL                     1
                                  126 LOAD_FAST                0 (self)
                                  128 STORE_ATTR               5 (token)
                      
-                      84         138 LOAD_GLOBAL             13 (NULL + type)
+                      86         138 LOAD_GLOBAL             13 (NULL + type)
                                  150 LOAD_FAST                0 (self)
                                  152 PRECALL                  1
                                  156 CALL                     1
                                  166 RETURN_VALUE
                      consts
                         None
                         ()
                      names      ('isinstance', 'async_sessionmaker', 'SessionNotInitialisedException', 'set', 'session_args', 'token', 'type')
                      varnames   ('self',)
                      freevars   ('_Session', '_session')
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       '__aenter__'
-                     firstlineno 79
+                     firstlineno 81
                      lnotab 0x08012a010e024a01
                   code
                      argcount  : 4
                      nlocals   : 5
                      stacksize : 5
                      flags     : 147
                      code
@@ -796,95 +840,95 @@
                         0000000000000001006400530023007c04a0040000000000000000000000
                         000000000000000000a6000000ab000000000000000000830064007b0356
                         009703860401008905a00500000000000000000000000000000000000000
                         007c006a060000000000000000a6010000ab010000000000000000010077
                         00780359007701
                                    0 COPY_FREE_VARS           1
                      
-                      86           2 RETURN_GENERATOR
+                      88           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                      87           8 LOAD_DEREF               5 (_session)
+                      89           8 LOAD_DEREF               5 (_session)
                                   10 LOAD_METHOD              0 (get)
                                   32 PRECALL                  0
                                   36 CALL                     0
                                   46 STORE_FAST               4 (session)
                      
-                      89          48 NOP
+                      91          48 NOP
                      
-                      90          50 LOAD_FAST                1 (exc_type)
+                      92          50 LOAD_FAST                1 (exc_type)
                                   52 POP_JUMP_FORWARD_IF_NONE    27 (to 108)
                      
-                      91          54 LOAD_FAST                4 (session)
+                      93          54 LOAD_FAST                4 (session)
                                   56 LOAD_METHOD              1 (rollback)
                                   78 PRECALL                  0
                                   82 CALL                     0
                                   92 GET_AWAITABLE            0
                                   94 LOAD_CONST               0 (None)
                              >>   96 SEND                     3 (to 104)
                                   98 YIELD_VALUE
                                  100 RESUME                   3
                                  102 JUMP_BACKWARD_NO_INTERRUPT     4 (to 96)
                              >>  104 POP_TOP
                                  106 JUMP_FORWARD            33 (to 174)
                      
-                      93     >>  108 LOAD_FAST                0 (self)
+                      95     >>  108 LOAD_FAST                0 (self)
                                  110 LOAD_ATTR                2 (commit_on_exit)
                      
-                      92         120 POP_JUMP_FORWARD_IF_FALSE    26 (to 174)
+                      94         120 POP_JUMP_FORWARD_IF_FALSE    26 (to 174)
                      
-                      95         122 LOAD_FAST                4 (session)
+                      97         122 LOAD_FAST                4 (session)
                                  124 LOAD_METHOD              3 (commit)
                                  146 PRECALL                  0
                                  150 CALL                     0
                                  160 GET_AWAITABLE            0
                                  162 LOAD_CONST               0 (None)
                              >>  164 SEND                     3 (to 172)
                                  166 YIELD_VALUE
                                  168 RESUME                   3
                                  170 JUMP_BACKWARD_NO_INTERRUPT     4 (to 164)
                              >>  172 POP_TOP
                      
-                      97     >>  174 LOAD_FAST                4 (session)
+                      99     >>  174 LOAD_FAST                4 (session)
                                  176 LOAD_METHOD              4 (close)
                                  198 PRECALL                  0
                                  202 CALL                     0
                                  212 GET_AWAITABLE            0
                                  214 LOAD_CONST               0 (None)
                              >>  216 SEND                     3 (to 224)
                                  218 YIELD_VALUE
                                  220 RESUME                   3
                                  222 JUMP_BACKWARD_NO_INTERRUPT     4 (to 216)
                              >>  224 POP_TOP
                      
-                      98         226 LOAD_DEREF               5 (_session)
+                     100         226 LOAD_DEREF               5 (_session)
                                  228 LOAD_METHOD              5 (reset)
                                  250 LOAD_FAST                0 (self)
                                  252 LOAD_ATTR                6 (token)
                                  262 PRECALL                  1
                                  266 CALL                     1
                                  276 POP_TOP
                                  278 LOAD_CONST               0 (None)
                                  280 RETURN_VALUE
                              >>  282 PUSH_EXC_INFO
                      
-                      97         284 LOAD_FAST                4 (session)
+                      99         284 LOAD_FAST                4 (session)
                                  286 LOAD_METHOD              4 (close)
                                  308 PRECALL                  0
                                  312 CALL                     0
                                  322 GET_AWAITABLE            0
                                  324 LOAD_CONST               0 (None)
                              >>  326 SEND                     3 (to 334)
                                  328 YIELD_VALUE
                                  330 RESUME                   3
                                  332 JUMP_BACKWARD_NO_INTERRUPT     4 (to 326)
                              >>  334 POP_TOP
                      
-                      98         336 LOAD_DEREF               5 (_session)
+                     100         336 LOAD_DEREF               5 (_session)
                                  338 LOAD_METHOD              5 (reset)
                                  360 LOAD_FAST                0 (self)
                                  362 LOAD_ATTR                6 (token)
                                  372 PRECALL                  1
                                  376 CALL                     1
                                  386 POP_TOP
                                  388 RERAISE                  0
@@ -896,59 +940,59 @@
                        282 to 388 -> 390 [1] lasti
                      consts
                         None
                      names      ('get', 'rollback', 'commit_on_exit', 'commit', 'close', 'reset', 'token')
                      varnames   ('self', 'exc_type', 'exc_value', 'traceback', 'session')
                      freevars   ('_session',)
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                      name       '__aexit__'
-                     firstlineno 86
+                     firstlineno 88
                      lnotab 0x080128020201040136020cff0203340234013aff3401
                   (None, False)
                names      ('__name__', '__module__', '__qualname__', 'Dict', 'bool', '__init__', '__aenter__', '__aexit__')
                varnames   ()
                freevars   ('_Session', '_session')
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                name       'DBSession'
-               firstlineno 73
+               firstlineno 75
                lnotab 0x0c0112050c07
             'DBSession'
             ('metaclass',)
          names      ('ContextVar', 'BaseHTTPMiddleware', 'type')
          varnames   ('SQLAlchemyMiddleware', 'DBSessionMeta')
          freevars   ()
          cellvars   ('DBSession', '_Session', '_session')
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
          name       'create_middleware_and_session_proxy'
-         firstlineno 20
+         firstlineno 22
          lnotab 0x0801040422022c212c0d241b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         106           2 RESUME                   0
+         108           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('MissingSessionException')
                       10 STORE_NAME               2 (__qualname__)
          
-         107          12 LOAD_CONST               1 ('\n    Exception raised for when the user tries to access a database session before it is created.\n    ')
+         109          12 LOAD_CONST               1 ('\n    Exception raised for when the user tries to access a database session before it is created.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         111          16 LOAD_CLOSURE             0 (__class__)
+         113          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 111>)
+                      20 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 113>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -961,20 +1005,20 @@
                flags     : 3
                code
                   0x9501970064017d01740100000000000000000000a6000000ab00000000
                   0000000000a00100000000000000000000000000000000000000007c01a6
                   010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               111           2 RESUME                   0
+               113           2 RESUME                   0
                
-               112           4 LOAD_CONST               1 ('\n        No session found! Either you are not currently in a request context,\n        or you need to manually create a session context by using a `db` instance as\n        a context manager e.g.:\n\n        async with db():\n            await db.session.execute(foo.select()).fetchall()\n        ')
+               114           4 LOAD_CONST               1 ('\n        No session found! Either you are not currently in a request context,\n        or you need to manually create a session context by using a `db` instance as\n        a context manager e.g.:\n\n        async with db():\n            await db.session.execute(foo.select()).fetchall()\n        ')
                              6 STORE_FAST               1 (detail)
                
-               121           8 LOAD_GLOBAL              1 (NULL + super)
+               123           8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_METHOD              1 (__init__)
                             56 LOAD_FAST                1 (detail)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
@@ -983,49 +1027,49 @@
                consts
                   None
                   '\n        No session found! Either you are not currently in a request context,\n        or you need to manually create a session context by using a `db` instance as\n        a context manager e.g.:\n\n        async with db():\n            await db.session.execute(foo.select()).fetchall()\n        '
                names      ('super', '__init__')
                varnames   ('self', 'detail')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                name       '__init__'
-               firstlineno 111
+               firstlineno 113
                lnotab 0x04010409
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
          name       'MissingSessionException'
-         firstlineno 106
+         firstlineno 108
          lnotab 0x0c010404
       'MissingSessionException'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         124           2 RESUME                   0
+         126           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SessionNotInitialisedException')
                       10 STORE_NAME               2 (__qualname__)
          
-         125          12 LOAD_CONST               1 ('\n    Exception raised when the user creates a new DB session without first initialising it.\n    ')
+         127          12 LOAD_CONST               1 ('\n    Exception raised when the user creates a new DB session without first initialising it.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         129          16 LOAD_CLOSURE             0 (__class__)
+         131          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\middleware\db_session_middleware.py", line 129>)
+                      20 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\middleware\db_session_middleware.py", line 131>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -1038,20 +1082,20 @@
                flags     : 3
                code
                   0x9501970064017d01740100000000000000000000a6000000ab00000000
                   0000000000a00100000000000000000000000000000000000000007c01a6
                   010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-               129           2 RESUME                   0
+               131           2 RESUME                   0
                
-               130           4 LOAD_CONST               1 ('\n        Session not initialised! Ensure that DBSessionMiddleware has been initialised before\n        attempting database access.\n        ')
+               132           4 LOAD_CONST               1 ('\n        Session not initialised! Ensure that DBSessionMiddleware has been initialised before\n        attempting database access.\n        ')
                              6 STORE_FAST               1 (detail)
                
-               135           8 LOAD_GLOBAL              1 (NULL + super)
+               137           8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_METHOD              1 (__init__)
                             56 LOAD_FAST                1 (detail)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
@@ -1060,31 +1104,33 @@
                consts
                   None
                   '\n        Session not initialised! Ensure that DBSessionMiddleware has been initialised before\n        attempting database access.\n        '
                names      ('super', '__init__')
                varnames   ('self', 'detail')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
                name       '__init__'
-               firstlineno 129
+               firstlineno 131
                lnotab 0x04010405
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
          name       'SessionNotInitialisedException'
-         firstlineno 124
+         firstlineno 126
          lnotab 0x0c010404
       'SessionNotInitialisedException'
+      'echo'
+      ('db_url', 'engine_args')
       None
-   names      ('__doc__', 'contextvars', 'ContextVar', 'typing', 'Dict', 'Optional', 'Union', 'sqlalchemy.engine', 'Engine', 'sqlalchemy.engine.url', 'URL', 'sqlalchemy.ext.asyncio', 'AsyncSession', 'create_async_engine', 'starlette.middleware.base', 'BaseHTTPMiddleware', 'RequestResponseEndpoint', 'starlette.requests', 'Request', 'starlette.types', 'ASGIApp', 'async_sessionmaker', 'ImportError', 'sqlalchemy.orm', 'sessionmaker', 'create_middleware_and_session_proxy', 'SQLAlchemyMiddleware', 'db', 'Exception', 'MissingSessionException', 'SessionNotInitialisedException')
+   names      ('__doc__', 'contextvars', 'ContextVar', 'typing', 'Dict', 'Optional', 'Union', 'sqlalchemy.engine', 'Engine', 'sqlalchemy.engine.url', 'URL', 'sqlalchemy.ext.asyncio', 'AsyncSession', 'create_async_engine', 'starlette.middleware.base', 'BaseHTTPMiddleware', 'RequestResponseEndpoint', 'starlette.requests', 'Request', 'starlette.types', 'ASGIApp', 'fss.common.config', 'configs', 'fss.starter.server', 'app', 'async_sessionmaker', 'ImportError', 'sqlalchemy.orm', 'sessionmaker', 'create_middleware_and_session_proxy', 'SQLAlchemyMiddleware', 'db', 'Exception', 'MissingSessionException', 'SessionNotInitialisedException', 'add_middleware', 'str', 'sqlalchemy_database_url', 'echo_sql')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\middleware\\db_session_middleware.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\middleware\\db_session_middleware.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104020c0114020c010c01100110010c010c0302011001080110
-      ff080406531a031c12
+      0x00ff020104020c0114020c010c01100110010c010c020c010c02020110
+      01080110ff080406531a031c121c0f0e0102011e020eff02fd
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/db_session_middleware.py` & `fastapi_sqlmodel_starter-1.0.1/fss/middleware/db_session_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.url import URL
 from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.types import ASGIApp
 
+from fss.common.config import configs
+from fss.starter.server import app
 
 try:
     from sqlalchemy.ext.asyncio import async_sessionmaker
 except ImportError:
     from sqlalchemy.orm import sessionmaker as async_sessionmaker
 
 
@@ -129,7 +131,17 @@
     def __init__(self):
         detail = """
         Session not initialised! Ensure that DBSessionMiddleware has been initialised before
         attempting database access.
         """
 
         super().__init__(detail)
+
+
+# Add SQLAlchemyMiddleware
+app.add_middleware(
+    SQLAlchemyMiddleware,
+    db_url=str(configs.sqlalchemy_database_url),
+    engine_args={
+        "echo": configs.echo_sql,
+    },
+)
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/exception/__pycache__/system.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,81 +1,85 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 358
+moddate:  0x10932266 (Fri Apr 19 15:51:44 2024 UTC)
+files sz: 382
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a02010002004700640384
-      0064046502a6030000ab0300000000000000005a0364015300
+      0x970064005a00640164026c015a01640164036c026d035a030100020047
+      006404840064056503a6030000ab0300000000000000005a0464025300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (http)
-                 8 STORE_NAME               0 (http)
+     1           2 LOAD_CONST               0 ('System exception')
+                 4 STORE_NAME               0 (__doc__)
    
-     3          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('ServiceException',))
-                14 IMPORT_NAME              1 (fss.common.exception.exception)
-                16 IMPORT_FROM              2 (ServiceException)
-                18 STORE_NAME               2 (ServiceException)
-                20 POP_TOP
+     3           6 LOAD_CONST               1 (0)
+                 8 LOAD_CONST               2 (None)
+                10 IMPORT_NAME              1 (http)
+                12 STORE_NAME               1 (http)
    
-     6          22 PUSH_NULL
-                24 LOAD_BUILD_CLASS
-                26 LOAD_CONST               3 (<code object SystemException, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\exception\system.py", line 6>)
-                28 MAKE_FUNCTION            0
-                30 LOAD_CONST               4 ('SystemException')
-                32 LOAD_NAME                2 (ServiceException)
-                34 PRECALL                  3
-                38 CALL                     3
-                48 STORE_NAME               3 (SystemException)
-                50 LOAD_CONST               1 (None)
-                52 RETURN_VALUE
+     5          14 LOAD_CONST               1 (0)
+                16 LOAD_CONST               3 (('ServiceException',))
+                18 IMPORT_NAME              2 (fss.common.exception.exception)
+                20 IMPORT_FROM              3 (ServiceException)
+                22 STORE_NAME               3 (ServiceException)
+                24 POP_TOP
+   
+     8          26 PUSH_NULL
+                28 LOAD_BUILD_CLASS
+                30 LOAD_CONST               4 (<code object SystemException, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\exception\system.py", line 8>)
+                32 MAKE_FUNCTION            0
+                34 LOAD_CONST               5 ('SystemException')
+                36 LOAD_NAME                3 (ServiceException)
+                38 PRECALL                  3
+                42 CALL                     3
+                52 STORE_NAME               4 (SystemException)
+                54 LOAD_CONST               2 (None)
+                56 RETURN_VALUE
    consts
+      'System exception'
       0
       None
       ('ServiceException',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0365046a0500000000000000006a
             060000000000000000660164026507640365086404650766068800660164
             05840d5a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-           6           2 RESUME                   0
+           8           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SystemException')
                       10 STORE_NAME               2 (__qualname__)
          
-           7          12 LOAD_CONST               1 ('\n    System module exception\n    ')
+           9          12 LOAD_CONST               1 ('\n    System module exception\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          11          16 LOAD_NAME                4 (http)
+          13          16 LOAD_NAME                4 (http)
                       18 LOAD_ATTR                5 (HTTPStatus)
                       28 LOAD_ATTR                6 (OK)
                       38 BUILD_TUPLE              1
                       40 LOAD_CONST               2 ('code')
                       42 LOAD_NAME                7 (int)
                       44 LOAD_CONST               3 ('msg')
                       46 LOAD_NAME                8 (str)
                       48 LOAD_CONST               4 ('status_code')
                       50 LOAD_NAME                7 (int)
                       52 BUILD_TUPLE              6
                       54 LOAD_CLOSURE             0 (__class__)
                       56 BUILD_TUPLE              1
-                      58 LOAD_CONST               5 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\exception\system.py", line 11>)
+                      58 LOAD_CONST               5 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\exception\system.py", line 13>)
                       60 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       62 STORE_NAME               9 (__init__)
                       64 LOAD_CLOSURE             0 (__class__)
                       66 COPY                     1
                       68 STORE_NAME              10 (__classcell__)
                       70 RETURN_VALUE
          consts
@@ -92,54 +96,54 @@
                code
                   0x950197007401000000000000000000007402000000000000000000007c
                   00a6020000ab020000000000000000a00200000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000001
                   0064005300
                              0 COPY_FREE_VARS           1
                
-                11           2 RESUME                   0
+                13           2 RESUME                   0
                
-                12           4 LOAD_GLOBAL              1 (NULL + super)
+                14           4 LOAD_GLOBAL              1 (NULL + super)
                             16 LOAD_GLOBAL              2 (SystemException)
                             28 LOAD_FAST                0 (self)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_METHOD              2 (__init__)
                
-                13          66 LOAD_FAST                1 (code)
+                15          66 LOAD_FAST                1 (code)
                             68 LOAD_FAST                2 (msg)
                             70 LOAD_FAST                3 (status_code)
                
-                12          72 KW_NAMES                 1
+                14          72 KW_NAMES                 1
                             74 PRECALL                  3
                             78 CALL                     3
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                consts
                   None
                   ('code', 'msg', 'status_code')
                names      ('super', 'SystemException', '__init__')
                varnames   ('self', 'code', 'msg', 'status_code')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\exception\\system.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\exception\\system.py'
                name       '__init__'
-               firstlineno 11
+               firstlineno 13
                lnotab 0x04013e0106ff
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'http', 'HTTPStatus', 'OK', 'int', 'str', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\exception\\system.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\exception\\system.py'
          name       'SystemException'
-         firstlineno 6
+         firstlineno 8
          lnotab 0x0c010404
       'SystemException'
-   names      ('http', 'fss.common.exception.exception', 'ServiceException', 'SystemException')
+   names      ('__doc__', 'http', 'fss.common.exception.exception', 'ServiceException', 'SystemException')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\exception\\system.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\exception\\system.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108020c03
+   lnotab 0x00ff0201040208020c03
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 1045
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
+files sz: 1476
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
@@ -50,25 +50,25 @@
                 58 IMPORT_NAME              9 (fss.starter.system.model.user_do)
                 60 IMPORT_FROM             10 (UserDO)
                 62 STORE_NAME              10 (UserDO)
                 64 POP_TOP
    
     12          66 PUSH_NULL
                 68 LOAD_BUILD_CLASS
-                70 LOAD_CONST               7 (<code object UserMapper, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\mapper\user_mapper.py", line 12>)
+                70 LOAD_CONST               7 (<code object UserMapper, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\mapper\user_mapper.py", line 12>)
                 72 MAKE_FUNCTION            0
                 74 LOAD_CONST               8 ('UserMapper')
                 76 LOAD_NAME                8 (SqlModelMapper)
                 78 LOAD_NAME               10 (UserDO)
                 80 BINARY_SUBSCR
                 90 PRECALL                  3
                 94 CALL                     3
                104 STORE_NAME              11 (UserMapper)
    
-    34         106 PUSH_NULL
+    45         106 PUSH_NULL
                108 LOAD_NAME               11 (UserMapper)
                110 LOAD_NAME               10 (UserDO)
                112 PRECALL                  1
                116 CALL                     1
                126 STORE_NAME              12 (userMapper)
                128 LOAD_CONST               9 (None)
                130 RETURN_VALUE
@@ -84,15 +84,18 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02640164029c0164036503640465046505640166
             021900000000000000000064056504650664016602190000000000000000
-            006606640684065a0764015300
+            006606640684065a07640164029c01640765086503190000000000000000
+            006404650465056401660219000000000000000000640565046508650619
+            00000000000000000064016602190000000000000000006606640884065a
+            0964015300
           12           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserMapper')
                        8 STORE_NAME               2 (__qualname__)
          
           14          10 LOAD_CONST               1 (None)
@@ -116,19 +119,52 @@
           15          42 LOAD_NAME                4 (Union)
                       44 LOAD_NAME                6 (UserDO)
                       46 LOAD_CONST               1 (None)
                       48 BUILD_TUPLE              2
                       50 BINARY_SUBSCR
          
           13          60 BUILD_TUPLE              6
-                      62 LOAD_CONST               6 (<code object get_user_by_username, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\mapper\user_mapper.py", line 13>)
+                      62 LOAD_CONST               6 (<code object get_user_by_username, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\mapper\user_mapper.py", line 13>)
                       64 MAKE_FUNCTION            6 (kwdefaults, annotations)
                       66 STORE_NAME               7 (get_user_by_username)
-                      68 LOAD_CONST               1 (None)
-                      70 RETURN_VALUE
+         
+          34          68 LOAD_CONST               1 (None)
+         
+          33          70 LOAD_CONST               2 (('db_session',))
+                      72 BUILD_CONST_KEY_MAP      1
+                      74 LOAD_CONST               7 ('usernames')
+         
+          34          76 LOAD_NAME                8 (list)
+                      78 LOAD_NAME                3 (str)
+                      80 BINARY_SUBSCR
+         
+          33          90 LOAD_CONST               4 ('db_session')
+         
+          34          92 LOAD_NAME                4 (Union)
+                      94 LOAD_NAME                5 (AsyncSession)
+                      96 LOAD_CONST               1 (None)
+                      98 BUILD_TUPLE              2
+                     100 BINARY_SUBSCR
+         
+          33         110 LOAD_CONST               5 ('return')
+         
+          35         112 LOAD_NAME                4 (Union)
+                     114 LOAD_NAME                8 (list)
+                     116 LOAD_NAME                6 (UserDO)
+                     118 BINARY_SUBSCR
+                     128 LOAD_CONST               1 (None)
+                     130 BUILD_TUPLE              2
+                     132 BINARY_SUBSCR
+         
+          33         142 BUILD_TUPLE              6
+                     144 LOAD_CONST               8 (<code object get_user_by_usernames, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\mapper\user_mapper.py", line 33>)
+                     146 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     148 STORE_NAME               9 (get_user_by_usernames)
+                     150 LOAD_CONST               1 (None)
+                     152 RETURN_VALUE
          consts
             'UserMapper'
             None
             ('db_session',)
             'username'
             'db_session'
             'return'
@@ -190,29 +226,107 @@
                consts
                   '\n        Retrieve a user record by username.\n\n        Args:\n            username (str): The username to query.\n            db_session (AsyncSession or None, optional): The database session instance. If None, use the default\n            session.\n\n        Returns:\n            Union[UserDO, None]: The UserDO instance if found, otherwise None.\n        '
                   None
                names      ('db', 'session', 'execute', 'select', 'UserDO', 'where', 'username', 'scalar_one_or_none')
                varnames   ('self', 'username', 'db_session', 'user')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\mapper\\user_mapper.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\mapper\\user_mapper.py'
                name       'get_user_by_username'
                firstlineno 13
                lnotab 0x060e1c01180168ff1c03
-         names      ('__name__', '__module__', '__qualname__', 'str', 'Union', 'AsyncSession', 'UserDO', 'get_user_by_username')
+            'usernames'
+            code
+               argcount  : 1
+               nlocals   : 5
+               stacksize : 5
+               flags     : 131
+               code
+                  0x4b00010097007c02700b7c006a0000000000000000006a010000000000
+                  0000007d02740500000000000000000000740600000000000000000000a6
+                  010000ab010000000000000000a004000000000000000000000000000000
+                  00000000007406000000000000000000006a050000000000000000a00600
+                  000000000000000000000000000000000000007c01a6010000ab01000000
+                  0000000000a6010000ab0100000000000000007d037c02a0070000000000
+                  0000000000000000000000000000007c03a6010000ab0100000000000000
+                  00830064017b035600970386047d047c04a0080000000000000000000000
+                  000000000000000000a6000000ab000000000000000000a0090000000000
+                  000000000000000000000000000000a6000000ab00000000000000000053
+                  00
+                33           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
+               
+                39           6 LOAD_FAST                2 (db_session)
+                             8 JUMP_IF_TRUE_OR_POP     11 (to 32)
+                            10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (db)
+                            22 LOAD_ATTR                1 (session)
+                       >>   32 STORE_FAST               2 (db_session)
+               
+                40          34 LOAD_GLOBAL              5 (NULL + select)
+                            46 LOAD_GLOBAL              6 (UserDO)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 LOAD_METHOD              4 (where)
+                            94 LOAD_GLOBAL              6 (UserDO)
+                           106 LOAD_ATTR                5 (username)
+                           116 LOAD_METHOD              6 (in_)
+                           138 LOAD_FAST                1 (usernames)
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 STORE_FAST               3 (statement)
+               
+                41         170 LOAD_FAST                2 (db_session)
+                           172 LOAD_METHOD              7 (execute)
+                           194 LOAD_FAST                3 (statement)
+                           196 PRECALL                  1
+                           200 CALL                     1
+                           210 GET_AWAITABLE            0
+                           212 LOAD_CONST               1 (None)
+                       >>  214 SEND                     3 (to 222)
+                           216 YIELD_VALUE
+                           218 RESUME                   3
+                           220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 214)
+                       >>  222 STORE_FAST               4 (results)
+               
+                42         224 LOAD_FAST                4 (results)
+                           226 LOAD_METHOD              8 (scalars)
+                           248 PRECALL                  0
+                           252 CALL                     0
+                           262 LOAD_METHOD              9 (all)
+                           284 PRECALL                  0
+                           288 CALL                     0
+                           298 RETURN_VALUE
+               consts
+                  '\n        Query user by usernames\n        '
+                  None
+               names      ('db', 'session', 'select', 'UserDO', 'where', 'username', 'in_', 'execute', 'scalars', 'all')
+               varnames   ('self', 'usernames', 'db_session', 'statement', 'results')
+               freevars   ()
+               cellvars   ()
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\mapper\\user_mapper.py'
+               name       'get_user_by_usernames'
+               firstlineno 33
+               lnotab 0x06061c0188013601
+         names      ('__name__', '__module__', '__qualname__', 'str', 'Union', 'AsyncSession', 'UserDO', 'get_user_by_username', 'list', 'get_user_by_usernames')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\mapper\\user_mapper.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\mapper\\user_mapper.py'
          name       'UserMapper'
          firstlineno 12
-         lnotab 0x0a0202ff060102ff020112ff020212fe
+         lnotab
+            0x0a0202ff060102ff020112ff020212fe081502ff06010eff020112ff02
+            021efe
       'UserMapper'
       None
    names      ('__doc__', 'typing', 'Union', 'sqlmodel', 'select', 'sqlmodel.ext.asyncio.session', 'AsyncSession', 'fss.common.persistence.sqlmodel_impl', 'SqlModelMapper', 'fss.starter.system.model.user_do', 'UserDO', 'UserMapper', 'userMapper')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\mapper\\user_mapper.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\mapper\\user_mapper.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c020c010c020c010c032816
+   lnotab 0x00ff020104020c020c010c020c010c032821
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/user_mapper.py` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/mapper/user_mapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,9 +26,20 @@
         """
         db_session = db_session or self.db.session
         user = await db_session.execute(
             select(UserDO).where(UserDO.username == username)
         )
         return user.scalar_one_or_none()
 
+    async def get_user_by_usernames(
+        self, *, usernames: list[str], db_session: Union[AsyncSession, None] = None
+    ) -> Union[list[UserDO], None]:
+        """
+        Query user by usernames
+        """
+        db_session = db_session or self.db.session
+        statement = select(UserDO).where(UserDO.username.in_(usernames))
+        results = await db_session.execute(statement)
+        return results.scalars().all()
+
 
 userMapper = UserMapper(UserDO)
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
 files sz: 728
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
@@ -44,25 +44,25 @@
                 50 STORE_NAME               9 (ModelExt)
                 52 IMPORT_FROM             10 (BaseModel)
                 54 STORE_NAME              10 (BaseModel)
                 56 POP_TOP
    
     10          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object BaseUser, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\model\user_do.py", line 10>)
+                62 LOAD_CONST               5 (<code object BaseUser, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\model\user_do.py", line 10>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('BaseUser')
                 68 LOAD_NAME                7 (SQLModel)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME              11 (BaseUser)
    
     24          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object UserDO, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\model\user_do.py", line 24>)
+                90 LOAD_CONST               7 (<code object UserDO, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\model\user_do.py", line 24>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('UserDO')
                 96 LOAD_NAME                9 (ModelExt)
                 98 LOAD_NAME               11 (BaseUser)
                100 LOAD_NAME               10 (BaseModel)
                102 LOAD_CONST               9 (True)
                104 KW_NAMES                10
@@ -199,15 +199,15 @@
             '昵称'
             ('comment',)
             'nickname'
          names      ('__name__', '__module__', '__qualname__', 'Field', 'Column', 'String', 'username', 'str', '__annotations__', 'password', 'nickname', 'Optional')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\model\\user_do.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\model\\user_do.py'
          name       'BaseUser'
          firstlineno 10
          lnotab 0x0c01040104011cff10ff1c0504012eff1c0304012cff
       'BaseUser'
       code
          argcount  : 0
          nlocals   : 0
@@ -235,23 +235,23 @@
             'comment'
             '用户信息表'
             None
          names      ('__name__', '__module__', '__qualname__', '__tablename__', '__table_args__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\model\\user_do.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\model\\user_do.py'
          name       'UserDO'
          firstlineno 24
          lnotab 0x0a010401
       'UserDO'
       True
       ('table',)
       None
    names      ('__doc__', 'typing', 'Optional', 'sqlmodel', 'Field', 'Column', 'String', 'SQLModel', 'fss.common.persistence.base_model', 'ModelExt', 'BaseModel', 'BaseUser', 'UserDO')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\model\\user_do.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\model\\user_do.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020c02180210031c0e
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/user_do.py` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/model/user_do.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/router/__pycache__/system.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,90 +1,143 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
-files sz: 376
+moddate:  0x7a612266 (Fri Apr 19 12:20:10 2024 UTC)
+files sz: 672
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
-      00640164046c056d065a06010002006502a6000000ab0000000000000000
-      005a076507a0080000000000000000000000000000000000000000650464
-      0567016406ac07a6030000ab03000000000000000001006507a008000000
-      00000000000000000000000000000000006506640867016409ac07a60300
-      00ab0300000000000000000100640a5300
+      00640164046c056d065a060100640164056c076d085a080100640164066c
+      096d0a5a0a0100640164076c0b6d0c5a0c010002006502a6000000ab0000
+      000000000000005a0d650da00e0000000000000000000000000000000000
+      0000006508640867016409ac0aa6030000ab030000000000000000010065
+      0da00e0000000000000000000000000000000000000000650a640b670164
+      0cac0aa6030000ab0300000000000000000100650da00e00000000000000
+      00000000000000000000000000650c640d6701640eac0aa6030000ab0300
+      000000000000000100020065066a0e0000000000000000650d65046a0f00
+      00000000000000ac0fa6020000ab020000000000000000010064105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Routing of system modules')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('APIRouter',))
                 10 IMPORT_NAME              1 (fastapi)
                 12 IMPORT_FROM              2 (APIRouter)
                 14 STORE_NAME               2 (APIRouter)
                 16 POP_TOP
    
      5          18 LOAD_CONST               1 (0)
-                20 LOAD_CONST               3 (('probe_router',))
-                22 IMPORT_NAME              3 (fss.starter.system.api.v1.probe_controller)
-                24 IMPORT_FROM              4 (probe_router)
-                26 STORE_NAME               4 (probe_router)
+                20 LOAD_CONST               3 (('configs',))
+                22 IMPORT_NAME              3 (fss.common.config)
+                24 IMPORT_FROM              4 (configs)
+                26 STORE_NAME               4 (configs)
                 28 POP_TOP
    
      6          30 LOAD_CONST               1 (0)
-                32 LOAD_CONST               4 (('user_router',))
-                34 IMPORT_NAME              5 (fss.starter.system.api.v1.user_controller)
-                36 IMPORT_FROM              6 (user_router)
-                38 STORE_NAME               6 (user_router)
+                32 LOAD_CONST               4 (('app',))
+                34 IMPORT_NAME              5 (fss.starter.server)
+                36 IMPORT_FROM              6 (app)
+                38 STORE_NAME               6 (app)
                 40 POP_TOP
    
-     8          42 PUSH_NULL
-                44 LOAD_NAME                2 (APIRouter)
-                46 PRECALL                  0
-                50 CALL                     0
-                60 STORE_NAME               7 (system_router)
-   
-     9          62 LOAD_NAME                7 (system_router)
-                64 LOAD_METHOD              8 (include_router)
-                86 LOAD_NAME                4 (probe_router)
-                88 LOAD_CONST               5 ('probe')
-                90 BUILD_LIST               1
-                92 LOAD_CONST               6 ('/probe')
-                94 KW_NAMES                 7
-                96 PRECALL                  3
-               100 CALL                     3
-               110 POP_TOP
-   
-    10         112 LOAD_NAME                7 (system_router)
-               114 LOAD_METHOD              8 (include_router)
-               136 LOAD_NAME                6 (user_router)
-               138 LOAD_CONST               8 ('user')
-               140 BUILD_LIST               1
-               142 LOAD_CONST               9 ('/user')
-               144 KW_NAMES                 7
-               146 PRECALL                  3
-               150 CALL                     3
-               160 POP_TOP
-               162 LOAD_CONST              10 (None)
-               164 RETURN_VALUE
+     7          42 LOAD_CONST               1 (0)
+                44 LOAD_CONST               5 (('probe_router',))
+                46 IMPORT_NAME              7 (fss.starter.system.api.v1.probe_controller)
+                48 IMPORT_FROM              8 (probe_router)
+                50 STORE_NAME               8 (probe_router)
+                52 POP_TOP
+   
+     8          54 LOAD_CONST               1 (0)
+                56 LOAD_CONST               6 (('user_router',))
+                58 IMPORT_NAME              9 (fss.starter.system.api.v1.user_controller)
+                60 IMPORT_FROM             10 (user_router)
+                62 STORE_NAME              10 (user_router)
+                64 POP_TOP
+   
+     9          66 LOAD_CONST               1 (0)
+                68 LOAD_CONST               7 (('role_router',))
+                70 IMPORT_NAME             11 (fss.starter.system.api.v1.role_controller)
+                72 IMPORT_FROM             12 (role_router)
+                74 STORE_NAME              12 (role_router)
+                76 POP_TOP
+   
+    11          78 PUSH_NULL
+                80 LOAD_NAME                2 (APIRouter)
+                82 PRECALL                  0
+                86 CALL                     0
+                96 STORE_NAME              13 (system_router)
+   
+    12          98 LOAD_NAME               13 (system_router)
+               100 LOAD_METHOD             14 (include_router)
+               122 LOAD_NAME                8 (probe_router)
+               124 LOAD_CONST               8 ('probe')
+               126 BUILD_LIST               1
+               128 LOAD_CONST               9 ('/probe')
+               130 KW_NAMES                10
+               132 PRECALL                  3
+               136 CALL                     3
+               146 POP_TOP
+   
+    13         148 LOAD_NAME               13 (system_router)
+               150 LOAD_METHOD             14 (include_router)
+               172 LOAD_NAME               10 (user_router)
+               174 LOAD_CONST              11 ('user')
+               176 BUILD_LIST               1
+               178 LOAD_CONST              12 ('/user')
+               180 KW_NAMES                10
+               182 PRECALL                  3
+               186 CALL                     3
+               196 POP_TOP
+   
+    14         198 LOAD_NAME               13 (system_router)
+               200 LOAD_METHOD             14 (include_router)
+               222 LOAD_NAME               12 (role_router)
+               224 LOAD_CONST              13 ('role')
+               226 BUILD_LIST               1
+               228 LOAD_CONST              14 ('/role')
+               230 KW_NAMES                10
+               232 PRECALL                  3
+               236 CALL                     3
+               246 POP_TOP
+   
+    17         248 PUSH_NULL
+               250 LOAD_NAME                6 (app)
+               252 LOAD_ATTR               14 (include_router)
+               262 LOAD_NAME               13 (system_router)
+               264 LOAD_NAME                4 (configs)
+               266 LOAD_ATTR               15 (api_version)
+               276 KW_NAMES                15
+               278 PRECALL                  2
+               282 CALL                     2
+               292 POP_TOP
+               294 LOAD_CONST              16 (None)
+               296 RETURN_VALUE
    consts
       'Routing of system modules'
       0
       ('APIRouter',)
+      ('configs',)
+      ('app',)
       ('probe_router',)
       ('user_router',)
+      ('role_router',)
       'probe'
       '/probe'
       ('tags', 'prefix')
       'user'
       '/user'
+      'role'
+      '/role'
+      ('prefix',)
       None
-   names      ('__doc__', 'fastapi', 'APIRouter', 'fss.starter.system.api.v1.probe_controller', 'probe_router', 'fss.starter.system.api.v1.user_controller', 'user_router', 'system_router', 'include_router')
+   names      ('__doc__', 'fastapi', 'APIRouter', 'fss.common.config', 'configs', 'fss.starter.server', 'app', 'fss.starter.system.api.v1.probe_controller', 'probe_router', 'fss.starter.system.api.v1.user_controller', 'user_router', 'fss.starter.system.api.v1.role_controller', 'role_router', 'system_router', 'include_router', 'api_version')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\router\\system.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\router\\system.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020104020c020c010c0214013201
+   lnotab 0x00ff020104020c020c010c010c010c010c021401320132013203
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa4111a66 (Sat Apr 13 05:01:24 2024 UTC)
-files sz: 622
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
+files sz: 627
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a0201000200470064038400640465
@@ -23,61 +23,61 @@
                 10 IMPORT_NAME              1 (pydantic)
                 12 IMPORT_FROM              2 (BaseModel)
                 14 STORE_NAME               2 (BaseModel)
                 16 POP_TOP
    
      6          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               3 (<code object UserCreateCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\schema\user_schema.py", line 6>)
+                22 LOAD_CONST               3 (<code object UserCreateCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\schema\user_schema.py", line 6>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               4 ('UserCreateCmd')
                 28 LOAD_NAME                2 (BaseModel)
                 30 PRECALL                  3
                 34 CALL                     3
                 44 STORE_NAME               3 (UserCreateCmd)
    
     16          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               5 (<code object UserQuery, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\schema\user_schema.py", line 16>)
+                50 LOAD_CONST               5 (<code object UserQuery, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\schema\user_schema.py", line 16>)
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               6 ('UserQuery')
                 56 LOAD_NAME                2 (BaseModel)
                 58 PRECALL                  3
                 62 CALL                     3
                 72 STORE_NAME               4 (UserQuery)
    
     26          74 PUSH_NULL
                 76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               7 (<code object LoginCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\schema\user_schema.py", line 26>)
+                78 LOAD_CONST               7 (<code object LoginCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\schema\user_schema.py", line 26>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               8 ('LoginCmd')
                 84 LOAD_NAME                2 (BaseModel)
                 86 PRECALL                  3
                 90 CALL                     3
                100 STORE_NAME               5 (LoginCmd)
    
     35         102 PUSH_NULL
                104 LOAD_BUILD_CLASS
-               106 LOAD_CONST               9 (<code object UpdateUserCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\schema\user_schema.py", line 35>)
+               106 LOAD_CONST               9 (<code object UpdateUserCmd, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\schema\user_schema.py", line 35>)
                108 MAKE_FUNCTION            0
                110 LOAD_CONST              10 ('UpdateUserCmd')
                112 LOAD_NAME                2 (BaseModel)
                114 PRECALL                  3
                118 CALL                     3
                128 STORE_NAME               6 (UpdateUserCmd)
    
     44         130 PUSH_NULL
                132 LOAD_BUILD_CLASS
-               134 LOAD_CONST              11 (<code object UserDO, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\schema\user_schema.py", line 44>)
+               134 LOAD_CONST              11 (<code object UserExport, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\schema\user_schema.py", line 44>)
                136 MAKE_FUNCTION            0
-               138 LOAD_CONST              12 ('UserDO')
+               138 LOAD_CONST              12 ('UserExport')
                140 LOAD_NAME                2 (BaseModel)
                142 PRECALL                  3
                146 CALL                     3
-               156 STORE_NAME               7 (UserDO)
+               156 STORE_NAME               7 (UserExport)
                158 LOAD_CONST              13 (None)
                160 RETURN_VALUE
    consts
       'User domain schema'
       0
       ('BaseModel',)
       code
@@ -121,15 +121,15 @@
             'password'
             'nickname'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
          name       'UserCreateCmd'
          firstlineno 6
          lnotab 0x0c0104040a010a01
       'UserCreateCmd'
       code
          argcount  : 0
          nlocals   : 0
@@ -171,15 +171,15 @@
             'username'
             'nickname'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'int', '__annotations__', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
          name       'UserQuery'
          firstlineno 16
          lnotab 0x0c0104040a010a01
       'UserQuery'
       code
          argcount  : 0
          nlocals   : 0
@@ -215,15 +215,15 @@
             'username'
             'password'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
          name       'LoginCmd'
          firstlineno 26
          lnotab 0x0c0104040a01
       'LoginCmd'
       code
          argcount  : 0
          nlocals   : 0
@@ -259,15 +259,15 @@
             'id'
             'nickname'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'int', '__annotations__', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
          name       'UpdateUserCmd'
          firstlineno 35
          lnotab 0x0c0104040a01
       'UpdateUserCmd'
       code
          argcount  : 0
          nlocals   : 0
@@ -275,19 +275,19 @@
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c000000650465
             0564033c0000006504650564043c00000064055300
           44           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('UserDO')
+                       6 LOAD_CONST               0 ('UserExport')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          45          12 LOAD_CONST               1 ('\n    UserQuery schema\n    ')
+          45          12 LOAD_CONST               1 ('\n    UserExport schema\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           49          16 LOAD_NAME                4 (str)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('username')
                       22 STORE_SUBSCR
          
@@ -299,31 +299,31 @@
           51          36 LOAD_NAME                4 (str)
                       38 LOAD_NAME                5 (__annotations__)
                       40 LOAD_CONST               4 ('nickname')
                       42 STORE_SUBSCR
                       46 LOAD_CONST               5 (None)
                       48 RETURN_VALUE
          consts
-            'UserDO'
-            '\n    UserQuery schema\n    '
+            'UserExport'
+            '\n    UserExport schema\n    '
             'username'
             'password'
             'nickname'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
-         name       'UserDO'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
+         name       'UserExport'
          firstlineno 44
          lnotab 0x0c0104040a010a01
-      'UserDO'
+      'UserExport'
       None
-   names      ('__doc__', 'pydantic', 'BaseModel', 'UserCreateCmd', 'UserQuery', 'LoginCmd', 'UpdateUserCmd', 'UserDO')
+   names      ('__doc__', 'pydantic', 'BaseModel', 'UserCreateCmd', 'UserQuery', 'LoginCmd', 'UpdateUserCmd', 'UserExport')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\schema\\user_schema.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\schema\\user_schema.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104020c031c0a1c0a1c091c09
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/user_schema.py` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/schema/user_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,1403 +1,1300 @@
 magic:    0xa70d0d0a
-moddate:  0x84271a66 (Sat Apr 13 06:34:44 2024 UTC)
-files sz: 6194
+moddate:  0x89de2366 (Sat Apr 20 15:26:01 2024 UTC)
+files sz: 7282
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
-      0x970064005a00640164026c015a01640164036c026d035a036d025a0201
-      00640164046c046d055a050100640164026c065a07640164056c086d095a
-      090100640164066c0a6d0b5a0b0100640164076c0c6d0d5a0d0100640164
-      086c0e6d0f5a0f0100640164096c106d115a116d125a1201006401640a6c
-      136d145a1401006401640b6c156d165a1601006401640c6c176d185a1801
-      006401640d6c196d1a5a1a01006401640e6c1b6d1c5a1c01006401640f6c
-      1d6d1e5a1e6d1f5a1f0100640164106c206d215a216d225a220100640164
-      116c236d245a240100640164126c256d265a266d275a270100640164136c
-      286d295a296d2a5a2a6d2b5a2b0100640164146c2c6d2d5a2d0100020047
-      00641584006416651a6526652b660219000000000000000000652da60400
-      00ab0400000000000000005a2e6417652d6602641884045a2f64025300
+      0x970064005a00640164026c015a01640164026c025a02640164036c036d
+      045a040100640164046c056d065a066d075a070100640164026c085a0964
+      0164056c0a6d0b5a0b0100640164066c0c6d0d5a0d0100640164076c0e6d
+      0f5a0f0100640164086c106d115a116d125a120100640164096c136d145a
+      1401006401640a6c156d165a1601006401640b6c176d185a180100640164
+      0c6c196d1a5a1a01006401640d6c1b6d1c5a1c01006401640e6c1d6d1e5a
+      1e01006401640f6c1f6d205a200100640164106c216d225a226d235a2301
+      00640164116c246d255a256d265a260100640164126c276d285a28010064
+      0164136c296d2a5a2a6d2b5a2b0100640164146c2c6d2d5a2d0100640164
+      156c2e6d2f5a2f6d305a306d315a316d325a320100640164166c336d345a
+      34010002004700641784006418651e652a652d6602190000000000000000
+      006534a6040000ab0400000000000000005a35641965346602641a84045a
+      3664025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('User domain service impl')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
-                10 IMPORT_NAME              1 (io)
-                12 STORE_NAME               1 (io)
+                10 IMPORT_NAME              1 (http)
+                12 STORE_NAME               1 (http)
    
      4          14 LOAD_CONST               1 (0)
-                16 LOAD_CONST               3 (('timedelta', 'datetime'))
-                18 IMPORT_NAME              2 (datetime)
-                20 IMPORT_FROM              3 (timedelta)
-                22 STORE_NAME               3 (timedelta)
-                24 IMPORT_FROM              2 (datetime)
-                26 STORE_NAME               2 (datetime)
-                28 POP_TOP
-   
-     5          30 LOAD_CONST               1 (0)
-                32 LOAD_CONST               4 (('Optional',))
-                34 IMPORT_NAME              4 (typing)
-                36 IMPORT_FROM              5 (Optional)
-                38 STORE_NAME               5 (Optional)
-                40 POP_TOP
-   
-     7          42 LOAD_CONST               1 (0)
-                44 LOAD_CONST               2 (None)
-                46 IMPORT_NAME              6 (pandas)
-                48 STORE_NAME               7 (pd)
+                16 LOAD_CONST               2 (None)
+                18 IMPORT_NAME              2 (io)
+                20 STORE_NAME               2 (io)
+   
+     5          22 LOAD_CONST               1 (0)
+                24 LOAD_CONST               3 (('timedelta',))
+                26 IMPORT_NAME              3 (datetime)
+                28 IMPORT_FROM              4 (timedelta)
+                30 STORE_NAME               4 (timedelta)
+                32 POP_TOP
+   
+     6          34 LOAD_CONST               1 (0)
+                36 LOAD_CONST               4 (('Optional', 'List'))
+                38 IMPORT_NAME              5 (typing)
+                40 IMPORT_FROM              6 (Optional)
+                42 STORE_NAME               6 (Optional)
+                44 IMPORT_FROM              7 (List)
+                46 STORE_NAME               7 (List)
+                48 POP_TOP
    
      8          50 LOAD_CONST               1 (0)
-                52 LOAD_CONST               5 (('UploadFile',))
-                54 IMPORT_NAME              8 (fastapi)
-                56 IMPORT_FROM              9 (UploadFile)
-                58 STORE_NAME               9 (UploadFile)
-                60 POP_TOP
-   
-     9          62 LOAD_CONST               1 (0)
-                64 LOAD_CONST               6 (('Params',))
-                66 IMPORT_NAME             10 (fastapi_pagination)
-                68 IMPORT_FROM             11 (Params)
-                70 STORE_NAME              11 (Params)
-                72 POP_TOP
-   
-    10          74 LOAD_CONST               1 (0)
-                76 LOAD_CONST               7 (('logger',))
-                78 IMPORT_NAME             12 (loguru)
-                80 IMPORT_FROM             13 (logger)
-                82 STORE_NAME              13 (logger)
-                84 POP_TOP
-   
-    11          86 LOAD_CONST               1 (0)
-                88 LOAD_CONST               8 (('StreamingResponse',))
-                90 IMPORT_NAME             14 (starlette.responses)
-                92 IMPORT_FROM             15 (StreamingResponse)
-                94 STORE_NAME              15 (StreamingResponse)
-                96 POP_TOP
-   
-    13          98 LOAD_CONST               1 (0)
-               100 LOAD_CONST               9 (('get_cache_client', 'Cache'))
-               102 IMPORT_NAME             16 (fss.common.cache.cache)
-               104 IMPORT_FROM             17 (get_cache_client)
-               106 STORE_NAME              17 (get_cache_client)
-               108 IMPORT_FROM             18 (Cache)
-               110 STORE_NAME              18 (Cache)
-               112 POP_TOP
-   
-    14         114 LOAD_CONST               1 (0)
-               116 LOAD_CONST              10 (('configs',))
-               118 IMPORT_NAME             19 (fss.common.config)
-               120 IMPORT_FROM             20 (configs)
-               122 STORE_NAME              20 (configs)
-               124 POP_TOP
-   
-    15         126 LOAD_CONST               1 (0)
-               128 LOAD_CONST              11 (('TokenTypeEnum',))
-               130 IMPORT_NAME             21 (fss.common.enum.enum)
-               132 IMPORT_FROM             22 (TokenTypeEnum)
-               134 STORE_NAME              22 (TokenTypeEnum)
-               136 POP_TOP
-   
-    16         138 LOAD_CONST               1 (0)
-               140 LOAD_CONST              12 (('Token',))
-               142 IMPORT_NAME             23 (fss.common.schema.schema)
-               144 IMPORT_FROM             24 (Token)
-               146 STORE_NAME              24 (Token)
-               148 POP_TOP
-   
-    17         150 LOAD_CONST               1 (0)
-               152 LOAD_CONST              13 (('ServiceImpl',))
-               154 IMPORT_NAME             25 (fss.common.service.impl.service_impl)
-               156 IMPORT_FROM             26 (ServiceImpl)
-               158 STORE_NAME              26 (ServiceImpl)
-               160 POP_TOP
-   
-    18         162 LOAD_CONST               1 (0)
-               164 LOAD_CONST              14 (('security',))
-               166 IMPORT_NAME             27 (fss.common.util)
-               168 IMPORT_FROM             28 (security)
-               170 STORE_NAME              28 (security)
-               172 POP_TOP
-   
-    19         174 LOAD_CONST               1 (0)
-               176 LOAD_CONST              15 (('verify_password', 'get_password_hash'))
-               178 IMPORT_NAME             29 (fss.common.util.security)
-               180 IMPORT_FROM             30 (verify_password)
-               182 STORE_NAME              30 (verify_password)
-               184 IMPORT_FROM             31 (get_password_hash)
-               186 STORE_NAME              31 (get_password_hash)
-               188 POP_TOP
-   
-    20         190 LOAD_CONST               1 (0)
-               192 LOAD_CONST              16 (('SystemResponseCode', 'SystemConstantCode'))
-               194 IMPORT_NAME             32 (fss.starter.system.enum.system)
-               196 IMPORT_FROM             33 (SystemResponseCode)
-               198 STORE_NAME              33 (SystemResponseCode)
-               200 IMPORT_FROM             34 (SystemConstantCode)
-               202 STORE_NAME              34 (SystemConstantCode)
-               204 POP_TOP
-   
-    21         206 LOAD_CONST               1 (0)
-               208 LOAD_CONST              17 (('SystemException',))
-               210 IMPORT_NAME             35 (fss.starter.system.exception.system)
-               212 IMPORT_FROM             36 (SystemException)
-               214 STORE_NAME              36 (SystemException)
-               216 POP_TOP
-   
-    22         218 LOAD_CONST               1 (0)
-               220 LOAD_CONST              18 (('UserMapper', 'userMapper'))
-               222 IMPORT_NAME             37 (fss.starter.system.mapper.user_mapper)
-               224 IMPORT_FROM             38 (UserMapper)
-               226 STORE_NAME              38 (UserMapper)
-               228 IMPORT_FROM             39 (userMapper)
-               230 STORE_NAME              39 (userMapper)
-               232 POP_TOP
-   
-    23         234 LOAD_CONST               1 (0)
-               236 LOAD_CONST              19 (('UserQuery', 'LoginCmd', 'UserDO'))
-               238 IMPORT_NAME             40 (fss.starter.system.schema.user_schema)
-               240 IMPORT_FROM             41 (UserQuery)
-               242 STORE_NAME              41 (UserQuery)
-               244 IMPORT_FROM             42 (LoginCmd)
-               246 STORE_NAME              42 (LoginCmd)
-               248 IMPORT_FROM             43 (UserDO)
-               250 STORE_NAME              43 (UserDO)
+                52 LOAD_CONST               2 (None)
+                54 IMPORT_NAME              8 (pandas)
+                56 STORE_NAME               9 (pd)
+   
+     9          58 LOAD_CONST               1 (0)
+                60 LOAD_CONST               5 (('UploadFile',))
+                62 IMPORT_NAME             10 (fastapi)
+                64 IMPORT_FROM             11 (UploadFile)
+                66 STORE_NAME              11 (UploadFile)
+                68 POP_TOP
+   
+    10          70 LOAD_CONST               1 (0)
+                72 LOAD_CONST               6 (('Params',))
+                74 IMPORT_NAME             12 (fastapi_pagination)
+                76 IMPORT_FROM             13 (Params)
+                78 STORE_NAME              13 (Params)
+                80 POP_TOP
+   
+    11          82 LOAD_CONST               1 (0)
+                84 LOAD_CONST               7 (('StreamingResponse',))
+                86 IMPORT_NAME             14 (starlette.responses)
+                88 IMPORT_FROM             15 (StreamingResponse)
+                90 STORE_NAME              15 (StreamingResponse)
+                92 POP_TOP
+   
+    13          94 LOAD_CONST               1 (0)
+                96 LOAD_CONST               8 (('get_cache_client', 'Cache'))
+                98 IMPORT_NAME             16 (fss.common.cache.cache)
+               100 IMPORT_FROM             17 (get_cache_client)
+               102 STORE_NAME              17 (get_cache_client)
+               104 IMPORT_FROM             18 (Cache)
+               106 STORE_NAME              18 (Cache)
+               108 POP_TOP
+   
+    14         110 LOAD_CONST               1 (0)
+               112 LOAD_CONST               9 (('configs',))
+               114 IMPORT_NAME             19 (fss.common.config)
+               116 IMPORT_FROM             20 (configs)
+               118 STORE_NAME              20 (configs)
+               120 POP_TOP
+   
+    15         122 LOAD_CONST               1 (0)
+               124 LOAD_CONST              10 (('TokenTypeEnum',))
+               126 IMPORT_NAME             21 (fss.common.enum.enum)
+               128 IMPORT_FROM             22 (TokenTypeEnum)
+               130 STORE_NAME              22 (TokenTypeEnum)
+               132 POP_TOP
+   
+    16         134 LOAD_CONST               1 (0)
+               136 LOAD_CONST              11 (('ServiceException',))
+               138 IMPORT_NAME             23 (fss.common.exception.exception)
+               140 IMPORT_FROM             24 (ServiceException)
+               142 STORE_NAME              24 (ServiceException)
+               144 POP_TOP
+   
+    17         146 LOAD_CONST               1 (0)
+               148 LOAD_CONST              12 (('Token',))
+               150 IMPORT_NAME             25 (fss.common.schema.schema)
+               152 IMPORT_FROM             26 (Token)
+               154 STORE_NAME              26 (Token)
+               156 POP_TOP
+   
+    18         158 LOAD_CONST               1 (0)
+               160 LOAD_CONST              13 (('security',))
+               162 IMPORT_NAME             27 (fss.common.security)
+               164 IMPORT_FROM             28 (security)
+               166 STORE_NAME              28 (security)
+               168 POP_TOP
+   
+    19         170 LOAD_CONST               1 (0)
+               172 LOAD_CONST              14 (('ServiceImpl',))
+               174 IMPORT_NAME             29 (fss.common.service.impl.service_impl)
+               176 IMPORT_FROM             30 (ServiceImpl)
+               178 STORE_NAME              30 (ServiceImpl)
+               180 POP_TOP
+   
+    20         182 LOAD_CONST               1 (0)
+               184 LOAD_CONST              15 (('export_template',))
+               186 IMPORT_NAME             31 (fss.common.util.excel)
+               188 IMPORT_FROM             32 (export_template)
+               190 STORE_NAME              32 (export_template)
+               192 POP_TOP
+   
+    21         194 LOAD_CONST               1 (0)
+               196 LOAD_CONST              16 (('verify_password', 'get_password_hash'))
+               198 IMPORT_NAME             33 (fss.common.security.security)
+               200 IMPORT_FROM             34 (verify_password)
+               202 STORE_NAME              34 (verify_password)
+               204 IMPORT_FROM             35 (get_password_hash)
+               206 STORE_NAME              35 (get_password_hash)
+               208 POP_TOP
+   
+    22         210 LOAD_CONST               1 (0)
+               212 LOAD_CONST              17 (('SystemResponseCode', 'SystemConstantCode'))
+               214 IMPORT_NAME             36 (fss.starter.system.enum.system)
+               216 IMPORT_FROM             37 (SystemResponseCode)
+               218 STORE_NAME              37 (SystemResponseCode)
+               220 IMPORT_FROM             38 (SystemConstantCode)
+               222 STORE_NAME              38 (SystemConstantCode)
+               224 POP_TOP
+   
+    23         226 LOAD_CONST               1 (0)
+               228 LOAD_CONST              18 (('SystemException',))
+               230 IMPORT_NAME             39 (fss.starter.system.exception.system)
+               232 IMPORT_FROM             40 (SystemException)
+               234 STORE_NAME              40 (SystemException)
+               236 POP_TOP
+   
+    24         238 LOAD_CONST               1 (0)
+               240 LOAD_CONST              19 (('UserMapper', 'userMapper'))
+               242 IMPORT_NAME             41 (fss.starter.system.mapper.user_mapper)
+               244 IMPORT_FROM             42 (UserMapper)
+               246 STORE_NAME              42 (UserMapper)
+               248 IMPORT_FROM             43 (userMapper)
+               250 STORE_NAME              43 (userMapper)
                252 POP_TOP
    
-    24         254 LOAD_CONST               1 (0)
-               256 LOAD_CONST              20 (('UserService',))
-               258 IMPORT_NAME             44 (fss.starter.system.service.user_service)
-               260 IMPORT_FROM             45 (UserService)
-               262 STORE_NAME              45 (UserService)
+    25         254 LOAD_CONST               1 (0)
+               256 LOAD_CONST              20 (('UserDO',))
+               258 IMPORT_NAME             44 (fss.starter.system.model.user_do)
+               260 IMPORT_FROM             45 (UserDO)
+               262 STORE_NAME              45 (UserDO)
                264 POP_TOP
    
-    27         266 PUSH_NULL
-               268 LOAD_BUILD_CLASS
-               270 LOAD_CONST              21 (<code object UserServiceImpl, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 27>)
-               272 MAKE_FUNCTION            0
-               274 LOAD_CONST              22 ('UserServiceImpl')
-               276 LOAD_NAME               26 (ServiceImpl)
-               278 LOAD_NAME               38 (UserMapper)
-               280 LOAD_NAME               43 (UserDO)
-               282 BUILD_TUPLE              2
-               284 BINARY_SUBSCR
-               294 LOAD_NAME               45 (UserService)
-               296 PRECALL                  4
-               300 CALL                     4
-               310 STORE_NAME              46 (UserServiceImpl)
-   
-   155         312 LOAD_CONST              23 ('return')
-               314 LOAD_NAME               45 (UserService)
-               316 BUILD_TUPLE              2
-               318 LOAD_CONST              24 (<code object get_user_service, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 155>)
-               320 MAKE_FUNCTION            4 (annotations)
-               322 STORE_NAME              47 (get_user_service)
-               324 LOAD_CONST               2 (None)
-               326 RETURN_VALUE
+    26         266 LOAD_CONST               1 (0)
+               268 LOAD_CONST              21 (('UserQuery', 'LoginCmd', 'UserExport', 'UserCreateCmd'))
+               270 IMPORT_NAME             46 (fss.starter.system.schema.user_schema)
+               272 IMPORT_FROM             47 (UserQuery)
+               274 STORE_NAME              47 (UserQuery)
+               276 IMPORT_FROM             48 (LoginCmd)
+               278 STORE_NAME              48 (LoginCmd)
+               280 IMPORT_FROM             49 (UserExport)
+               282 STORE_NAME              49 (UserExport)
+               284 IMPORT_FROM             50 (UserCreateCmd)
+               286 STORE_NAME              50 (UserCreateCmd)
+               288 POP_TOP
+   
+    32         290 LOAD_CONST               1 (0)
+               292 LOAD_CONST              22 (('UserService',))
+               294 IMPORT_NAME             51 (fss.starter.system.service.user_service)
+               296 IMPORT_FROM             52 (UserService)
+               298 STORE_NAME              52 (UserService)
+               300 POP_TOP
+   
+    35         302 PUSH_NULL
+               304 LOAD_BUILD_CLASS
+               306 LOAD_CONST              23 (<code object UserServiceImpl, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 35>)
+               308 MAKE_FUNCTION            0
+               310 LOAD_CONST              24 ('UserServiceImpl')
+               312 LOAD_NAME               30 (ServiceImpl)
+               314 LOAD_NAME               42 (UserMapper)
+               316 LOAD_NAME               45 (UserDO)
+               318 BUILD_TUPLE              2
+               320 BINARY_SUBSCR
+               330 LOAD_NAME               52 (UserService)
+               332 PRECALL                  4
+               336 CALL                     4
+               346 STORE_NAME              53 (UserServiceImpl)
+   
+   202         348 LOAD_CONST              25 ('return')
+               350 LOAD_NAME               52 (UserService)
+               352 BUILD_TUPLE              2
+               354 LOAD_CONST              26 (<code object get_user_service, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 202>)
+               356 MAKE_FUNCTION            4 (annotations)
+               358 STORE_NAME              54 (get_user_service)
+               360 LOAD_CONST               2 (None)
+               362 RETURN_VALUE
    consts
       'User domain service impl'
       0
       None
-      ('timedelta', 'datetime')
-      ('Optional',)
+      ('timedelta',)
+      ('Optional', 'List')
       ('UploadFile',)
       ('Params',)
-      ('logger',)
       ('StreamingResponse',)
       ('get_cache_client', 'Cache')
       ('configs',)
       ('TokenTypeEnum',)
+      ('ServiceException',)
       ('Token',)
-      ('ServiceImpl',)
       ('security',)
+      ('ServiceImpl',)
+      ('export_template',)
       ('verify_password', 'get_password_hash')
       ('SystemResponseCode', 'SystemConstantCode')
       ('SystemException',)
       ('UserMapper', 'userMapper')
-      ('UserQuery', 'LoginCmd', 'UserDO')
+      ('UserDO',)
+      ('UserQuery', 'LoginCmd', 'UserExport', 'UserCreateCmd')
       ('UserService',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 5
+         stacksize : 8
          flags     : 0
          code
-            0x8700970065005a0164005a02640165036602880066016402840c5a0464
-            036505640465066507190000000000000000006604640584045a08640665
-            096404650a6604640784045a0b6404650c6602640884045a0d6409650e66
-            02640a84045a0f640b65106404650c6604640c84045a11880078015a1253
-            00
+            0x8700970065005a0164005a0264015a0364026504660288006601640384
+            0c5a0564046506640565076508190000000000000000006604640684045a
+            096407650a6405650b6604640884045a0c6405650d6602640984045a0e64
+            0a650f6602640b84045a10640c65116405650d6604640d84045a12640e65
+            13640565146604640f84045a156410650664116506640565076516650819
+            000000000000000000190000000000000000006606641284045a17880078
+            015a185300
                        0 MAKE_CELL                0 (__class__)
          
-          27           2 RESUME                   0
+          35           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('UserServiceImpl')
                       10 STORE_NAME               2 (__qualname__)
          
-          28          12 LOAD_CONST               1 ('mapper')
-                      14 LOAD_NAME                3 (UserMapper)
-                      16 BUILD_TUPLE              2
-                      18 LOAD_CLOSURE             0 (__class__)
-                      20 BUILD_TUPLE              1
-                      22 LOAD_CONST               2 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 28>)
-                      24 MAKE_FUNCTION           12 (annotations, closure)
-                      26 STORE_NAME               4 (__init__)
+          36          12 LOAD_CONST               1 ('\n    Implementation of the UserService interface.\n    ')
+                      14 STORE_NAME               3 (__doc__)
+         
+          40          16 LOAD_CONST               2 ('mapper')
+                      18 LOAD_NAME                4 (UserMapper)
+                      20 BUILD_TUPLE              2
+                      22 LOAD_CLOSURE             0 (__class__)
+                      24 BUILD_TUPLE              1
+                      26 LOAD_CONST               3 (<code object __init__, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 40>)
+                      28 MAKE_FUNCTION           12 (annotations, closure)
+                      30 STORE_NAME               5 (__init__)
+         
+          50          32 LOAD_CONST               4 ('id')
+                      34 LOAD_NAME                6 (int)
+                      36 LOAD_CONST               5 ('return')
+                      38 LOAD_NAME                7 (Optional)
+                      40 LOAD_NAME                8 (UserQuery)
+                      42 BINARY_SUBSCR
+                      52 BUILD_TUPLE              4
+                      54 LOAD_CONST               6 (<code object find_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 50>)
+                      56 MAKE_FUNCTION            4 (annotations)
+                      58 STORE_NAME               9 (find_by_id)
+         
+          63          60 LOAD_CONST               7 ('loginCmd')
+                      62 LOAD_NAME               10 (LoginCmd)
+                      64 LOAD_CONST               5 ('return')
+                      66 LOAD_NAME               11 (Token)
+                      68 BUILD_TUPLE              4
+                      70 LOAD_CONST               8 (<code object login, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 63>)
+                      72 MAKE_FUNCTION            4 (annotations)
+                      74 STORE_NAME              12 (login)
          
-          32          28 LOAD_CONST               3 ('id')
-                      30 LOAD_NAME                5 (int)
-                      32 LOAD_CONST               4 ('return')
-                      34 LOAD_NAME                6 (Optional)
-                      36 LOAD_NAME                7 (UserQuery)
-                      38 BINARY_SUBSCR
-                      48 BUILD_TUPLE              4
-                      50 LOAD_CONST               5 (<code object find_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 32>)
-                      52 MAKE_FUNCTION            4 (annotations)
-                      54 STORE_NAME               8 (find_by_id)
+         108          76 LOAD_CONST               5 ('return')
          
-          44          56 LOAD_CONST               6 ('loginCmd')
-                      58 LOAD_NAME                9 (LoginCmd)
-                      60 LOAD_CONST               4 ('return')
-                      62 LOAD_NAME               10 (Token)
-                      64 BUILD_TUPLE              4
-                      66 LOAD_CONST               7 (<code object login, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 44>)
-                      68 MAKE_FUNCTION            4 (annotations)
-                      70 STORE_NAME              11 (login)
+         110          78 LOAD_NAME               13 (StreamingResponse)
          
-          83          72 LOAD_CONST               4 ('return')
+         108          80 BUILD_TUPLE              2
+                      82 LOAD_CONST               9 (<code object export_user_template, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 108>)
+                      84 MAKE_FUNCTION            4 (annotations)
+                      86 STORE_NAME              14 (export_user_template)
          
-          85          74 LOAD_NAME               12 (StreamingResponse)
+         116          88 LOAD_CONST              10 ('file')
+                      90 LOAD_NAME               15 (UploadFile)
+                      92 BUILD_TUPLE              2
+                      94 LOAD_CONST              11 (<code object import_user, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 116>)
+                      96 MAKE_FUNCTION            4 (annotations)
+                      98 STORE_NAME              16 (import_user)
          
-          83          76 BUILD_TUPLE              2
-                      78 LOAD_CONST               8 (<code object export_user_template, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 83>)
-                      80 MAKE_FUNCTION            4 (annotations)
-                      82 STORE_NAME              13 (export_user_template)
+         150         100 LOAD_CONST              12 ('params')
+                     102 LOAD_NAME               17 (Params)
+                     104 LOAD_CONST               5 ('return')
+                     106 LOAD_NAME               13 (StreamingResponse)
+                     108 BUILD_TUPLE              4
+                     110 LOAD_CONST              13 (<code object export_user, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 150>)
+                     112 MAKE_FUNCTION            4 (annotations)
+                     114 STORE_NAME              18 (export_user)
          
-         109          84 LOAD_CONST               9 ('file')
-                      86 LOAD_NAME               14 (UploadFile)
-                      88 BUILD_TUPLE              2
-                      90 LOAD_CONST              10 (<code object import_user, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 109>)
-                      92 MAKE_FUNCTION            4 (annotations)
-                      94 STORE_NAME              15 (import_user)
+         169         116 LOAD_CONST              14 ('data')
+                     118 LOAD_NAME               19 (UserCreateCmd)
+                     120 LOAD_CONST               5 ('return')
+                     122 LOAD_NAME               20 (UserDO)
+                     124 BUILD_TUPLE              4
+                     126 LOAD_CONST              15 (<code object register, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 169>)
+                     128 MAKE_FUNCTION            4 (annotations)
+                     130 STORE_NAME              21 (register)
          
-         124          96 LOAD_CONST              11 ('params')
-                      98 LOAD_NAME               16 (Params)
-                     100 LOAD_CONST               4 ('return')
-                     102 LOAD_NAME               12 (StreamingResponse)
-                     104 BUILD_TUPLE              4
-                     106 LOAD_CONST              12 (<code object export_user, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 124>)
-                     108 MAKE_FUNCTION            4 (annotations)
-                     110 STORE_NAME              17 (export_user)
-                     112 LOAD_CLOSURE             0 (__class__)
-                     114 COPY                     1
-                     116 STORE_NAME              18 (__classcell__)
-                     118 RETURN_VALUE
+         187         132 LOAD_CONST              16 ('page')
+                     134 LOAD_NAME                6 (int)
+                     136 LOAD_CONST              17 ('size')
+                     138 LOAD_NAME                6 (int)
+                     140 LOAD_CONST               5 ('return')
+                     142 LOAD_NAME                7 (Optional)
+                     144 LOAD_NAME               22 (List)
+                     146 LOAD_NAME                8 (UserQuery)
+                     148 BINARY_SUBSCR
+                     158 BINARY_SUBSCR
+                     168 BUILD_TUPLE              6
+                     170 LOAD_CONST              18 (<code object list_user, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 187>)
+                     172 MAKE_FUNCTION            4 (annotations)
+                     174 STORE_NAME              23 (list_user)
+                     176 LOAD_CLOSURE             0 (__class__)
+                     178 COPY                     1
+                     180 STORE_NAME              24 (__classcell__)
+                     182 RETURN_VALUE
          consts
             'UserServiceImpl'
+            '\n    Implementation of the UserService interface.\n    '
             'mapper'
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 4
+               stacksize : 3
                flags     : 3
                code
-                  0x950197007401000000000000000000007402000000000000000000007c
-                  00a6020000ab020000000000000000a00200000000000000000000000000
-                  000000000000007c01ac01a6010000ab01000000000000000001007c017c
-                  005f03000000000000000064005300
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01ac01a60100
+                  00ab01000000000000000001007c017c005f020000000000000000640253
+                  00
                              0 COPY_FREE_VARS           1
                
-                28           2 RESUME                   0
+                40           2 RESUME                   0
                
-                29           4 LOAD_GLOBAL              1 (NULL + super)
-                            16 LOAD_GLOBAL              2 (UserServiceImpl)
-                            28 LOAD_FAST                0 (self)
-                            30 PRECALL                  2
-                            34 CALL                     2
-                            44 LOAD_METHOD              2 (__init__)
-                            66 LOAD_FAST                1 (mapper)
-                            68 KW_NAMES                 1
-                            70 PRECALL                  1
-                            74 CALL                     1
-                            84 POP_TOP
-               
-                30          86 LOAD_FAST                1 (mapper)
-                            88 LOAD_FAST                0 (self)
-                            90 STORE_ATTR               3 (mapper)
-                           100 LOAD_CONST               0 (None)
-                           102 RETURN_VALUE
+                47           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (__init__)
+                            52 LOAD_FAST                1 (mapper)
+                            54 KW_NAMES                 1
+                            56 PRECALL                  1
+                            60 CALL                     1
+                            70 POP_TOP
+               
+                48          72 LOAD_FAST                1 (mapper)
+                            74 LOAD_FAST                0 (self)
+                            76 STORE_ATTR               2 (mapper)
+                            86 LOAD_CONST               2 (None)
+                            88 RETURN_VALUE
                consts
-                  None
+                  '\n        Initialize the UserServiceImpl instance.\n\n        Args:\n            mapper (UserMapper): The UserMapper instance to use for database operations.\n        '
                   ('mapper',)
-               names      ('super', 'UserServiceImpl', '__init__', 'mapper')
+                  None
+               names      ('super', '__init__', 'mapper')
                varnames   ('self', 'mapper')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                name       '__init__'
-               firstlineno 28
-               lnotab 0x04015201
+               firstlineno 40
+               lnotab 0x04074401
             'id'
             'return'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
                   0064027b035600970386047d027c02721e74050000000000000000000064
                   0369007c02a0030000000000000000000000000000000000000000a60000
-                  00ab000000000000000000a4018e01530064025300
-                32           0 RETURN_GENERATOR
+                  00ab000000000000000000a4018e016e0164025300
+                50           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                38           6 LOAD_FAST                0 (self)
+                60           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_by_id)
                             40 LOAD_FAST                1 (id)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
                             60 LOAD_CONST               2 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
                        >>   70 STORE_FAST               2 (user_do)
                
-                39          72 LOAD_FAST                2 (user_do)
+                61          72 LOAD_FAST                2 (user_do)
                             74 POP_JUMP_FORWARD_IF_FALSE    30 (to 136)
-               
-                40          76 LOAD_GLOBAL              5 (NULL + UserQuery)
+                            76 LOAD_GLOBAL              5 (NULL + UserQuery)
                             88 LOAD_CONST               3 (())
                             90 BUILD_MAP                0
                             92 LOAD_FAST                2 (user_do)
                             94 LOAD_METHOD              3 (model_dump)
                            116 PRECALL                  0
                            120 CALL                     0
                            130 DICT_MERGE               1
                            132 CALL_FUNCTION_EX         1
-                           134 RETURN_VALUE
-               
-                42     >>  136 LOAD_CONST               2 (None)
-                           138 RETURN_VALUE
+                           134 JUMP_FORWARD             1 (to 138)
+                       >>  136 LOAD_CONST               2 (None)
+                       >>  138 RETURN_VALUE
                consts
-                  '\n        Retrieval user through user id\n        :param id: user id\n        :return: user or none\n        '
+                  '\n        Retrieve a user by ID.\n\n        Args:\n            id (int): The user ID to retrieve.\n\n        Returns:\n            Optional[UserQuery]: The user query object if found, None otherwise.\n        '
                   ('id',)
                   None
                   ()
                names      ('mapper', 'select_by_id', 'UserQuery', 'model_dump')
                varnames   ('self', 'id', 'user_do')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                name       'find_by_id'
-               firstlineno 32
-               lnotab 0x0606420104013c02
+               firstlineno 50
+               lnotab 0x060a4201
             'loginCmd'
             code
                argcount  : 2
-               nlocals   : 10
-               stacksize : 10
+               nlocals   : 9
+               stacksize : 11
                flags     : 131
                code
                   0x4b00010097007c016a0000000000000000007d027c006a010000000000
                   000000a00200000000000000000000000000000000000000007c02ac01a6
-                  010000ab010000000000000000830064027b035600970386047d037c0372
-                  207407000000000000000000007c016a0400000000000000007c036a0400
-                  00000000000000a6020000ab020000000000000000830064027b03560097
-                  038604732e740b00000000000000000000740c000000000000000000006a
-                  0700000000000000006a080000000000000000740c000000000000000000
-                  006a0700000000000000006a090000000000000000a6020000ab02000000
-                  000000000082017415000000000000000000007416000000000000000000
-                  006a0c0000000000000000ac03a6010000ab0100000000000000007d0474
-                  15000000000000000000007416000000000000000000006a0d0000000000
-                  000000ac03a6010000ab0100000000000000007d05741d00000000000000
-                  0000006a0f00000000000000007c036a1000000000000000007c04742200
-                  0000000000000000006a120000000000000000ac04a6030000ab03000000
-                  0000000000830064027b035600970386047d06741d000000000000000000
-                  006a0f00000000000000007c036a1000000000000000007c057422000000
-                  000000000000006a130000000000000000ac04a6030000ab030000000000
-                  000000830064027b035600970386047d077429000000000000000000007c
-                  06742b000000000000000000007c04a01600000000000000000000000000
-                  00000000000000a6000000ab000000000000000000a6010000ab01000000
-                  000000000064057c07742b000000000000000000007c05a0160000000000
-                  000000000000000000000000000000a6000000ab000000000000000000a6
-                  010000ab010000000000000000ac06a6050000ab0500000000000000007d
-                  08742f00000000000000000000a6000000ab000000000000000000830064
-                  027b035600970386047d097c09a018000000000000000000000000000000
-                  00000000007432000000000000000000006a1a00000000000000006a0900
-                  000000000000009b007c036a1000000000000000009b009d027c067c04a6
-                  030000ab030000000000000000830064027b0356009703860401007c0853
-                  00
-                44           0 RETURN_GENERATOR
+                  010000ab010000000000000000830064027b035600970386047d037c0381
+                  1a7407000000000000000000007c016a0400000000000000007c036a0400
+                  00000000000000a6020000ab020000000000000000733f740b0000000000
+                  0000000000740c000000000000000000006a0700000000000000006a0800
+                  00000000000000740c000000000000000000006a0700000000000000006a
+                  0900000000000000007414000000000000000000006a0b00000000000000
+                  006a0c0000000000000000ac03a6030000ab030000000000000000820174
+                  1b00000000000000000000741c000000000000000000006a0f0000000000
+                  000000ac04a6010000ab0100000000000000007d04742100000000000000
+                  0000006a1100000000000000007c036a1200000000000000007c04742600
+                  0000000000000000006a140000000000000000ac05a6030000ab03000000
+                  0000000000830064027b035600970386047d057421000000000000000000
+                  006a1100000000000000007c036a12000000000000000074260000000000
+                  00000000006a150000000000000000ac06a6020000ab0200000000000000
+                  00830064027b035600970386047d06742d000000000000000000007c0574
+                  2f000000000000000000007c04a018000000000000000000000000000000
+                  0000000000a6000000ab000000000000000000a6010000ab010000000000
+                  00000064077c06742f00000000000000000000741b000000000000000000
+                  00741c000000000000000000006a190000000000000000ac04a6010000ab
+                  010000000000000000a01800000000000000000000000000000000000000
+                  00a6000000ab000000000000000000a6010000ab010000000000000000ac
+                  08a6050000ab0500000000000000007d07743500000000000000000000a6
+                  000000ab000000000000000000830064027b035600970386047d087c08a0
+                  1b0000000000000000000000000000000000000000743800000000000000
+                  0000006a1d00000000000000006a0900000000000000009b007c036a1200
+                  000000000000009b009d027c057c04a6030000ab03000000000000000083
+                  0064027b0356009703860401007c075300
+                63           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                50           6 LOAD_FAST                1 (loginCmd)
+                73           6 LOAD_FAST                1 (loginCmd)
                              8 LOAD_ATTR                0 (username)
                             18 STORE_FAST               2 (username)
                
-                51          20 LOAD_FAST                0 (self)
+                74          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (mapper)
                             32 LOAD_METHOD              2 (get_user_by_username)
                             54 LOAD_FAST                2 (username)
                             56 KW_NAMES                 1
                             58 PRECALL                  1
                             62 CALL                     1
                             72 GET_AWAITABLE            0
                             74 LOAD_CONST               2 (None)
                        >>   76 SEND                     3 (to 84)
                             78 YIELD_VALUE
                             80 RESUME                   3
                             82 JUMP_BACKWARD_NO_INTERRUPT     4 (to 76)
                        >>   84 STORE_FAST               3 (userDO)
                
-                52          86 LOAD_FAST                3 (userDO)
-                            88 POP_JUMP_FORWARD_IF_FALSE    32 (to 154)
+                75          86 LOAD_FAST                3 (userDO)
+                            88 POP_JUMP_FORWARD_IF_NONE    26 (to 142)
                             90 LOAD_GLOBAL              7 (NULL + verify_password)
                            102 LOAD_FAST                1 (loginCmd)
                            104 LOAD_ATTR                4 (password)
                            114 LOAD_FAST                3 (userDO)
                            116 LOAD_ATTR                4 (password)
                            126 PRECALL                  2
                            130 CALL                     2
-                           140 GET_AWAITABLE            0
-                           142 LOAD_CONST               2 (None)
-                       >>  144 SEND                     3 (to 152)
-                           146 YIELD_VALUE
-                           148 RESUME                   3
-                           150 JUMP_BACKWARD_NO_INTERRUPT     4 (to 144)
-                       >>  152 POP_JUMP_FORWARD_IF_TRUE    46 (to 246)
-               
-                53     >>  154 LOAD_GLOBAL             11 (NULL + SystemException)
-               
-                54         166 LOAD_GLOBAL             12 (SystemResponseCode)
-                           178 LOAD_ATTR                7 (AUTH_FAILED)
-                           188 LOAD_ATTR                8 (code)
-                           198 LOAD_GLOBAL             12 (SystemResponseCode)
-                           210 LOAD_ATTR                7 (AUTH_FAILED)
-                           220 LOAD_ATTR                9 (msg)
-               
-                53         230 PRECALL                  2
-                           234 CALL                     2
-                           244 RAISE_VARARGS            1
-               
-                56     >>  246 LOAD_GLOBAL             21 (NULL + timedelta)
-                           258 LOAD_GLOBAL             22 (configs)
-                           270 LOAD_ATTR               12 (access_token_expire_minutes)
-                           280 KW_NAMES                 3
-                           282 PRECALL                  1
-                           286 CALL                     1
-                           296 STORE_FAST               4 (access_token_expires)
-               
-                57         298 LOAD_GLOBAL             21 (NULL + timedelta)
-                           310 LOAD_GLOBAL             22 (configs)
-                           322 LOAD_ATTR               13 (refresh_token_expire_minutes)
-                           332 KW_NAMES                 3
-                           334 PRECALL                  1
-                           338 CALL                     1
-                           348 STORE_FAST               5 (refresh_token_expires)
-               
-                58         350 LOAD_GLOBAL             29 (NULL + security)
-                           362 LOAD_ATTR               15 (create_token)
-               
-                59         372 LOAD_FAST                3 (userDO)
-                           374 LOAD_ATTR               16 (id)
-               
-                60         384 LOAD_FAST                4 (access_token_expires)
-               
-                61         386 LOAD_GLOBAL             34 (TokenTypeEnum)
-                           398 LOAD_ATTR               18 (access)
-               
-                58         408 KW_NAMES                 4
-                           410 PRECALL                  3
-                           414 CALL                     3
-                           424 GET_AWAITABLE            0
-                           426 LOAD_CONST               2 (None)
-                       >>  428 SEND                     3 (to 436)
-                           430 YIELD_VALUE
-                           432 RESUME                   3
-                           434 JUMP_BACKWARD_NO_INTERRUPT     4 (to 428)
-                       >>  436 STORE_FAST               6 (access_token)
-               
-                63         438 LOAD_GLOBAL             29 (NULL + security)
-                           450 LOAD_ATTR               15 (create_token)
-               
-                64         460 LOAD_FAST                3 (userDO)
-                           462 LOAD_ATTR               16 (id)
-               
-                65         472 LOAD_FAST                5 (refresh_token_expires)
-               
-                66         474 LOAD_GLOBAL             34 (TokenTypeEnum)
-                           486 LOAD_ATTR               19 (refresh)
-               
-                63         496 KW_NAMES                 4
-                           498 PRECALL                  3
-                           502 CALL                     3
-                           512 GET_AWAITABLE            0
-                           514 LOAD_CONST               2 (None)
-                       >>  516 SEND                     3 (to 524)
-                           518 YIELD_VALUE
-                           520 RESUME                   3
-                           522 JUMP_BACKWARD_NO_INTERRUPT     4 (to 516)
-                       >>  524 STORE_FAST               7 (refresh_token)
-               
-                68         526 LOAD_GLOBAL             41 (NULL + Token)
-               
-                69         538 LOAD_FAST                6 (access_token)
-               
-                70         540 LOAD_GLOBAL             43 (NULL + int)
-                           552 LOAD_FAST                4 (access_token_expires)
-                           554 LOAD_METHOD             22 (total_seconds)
-                           576 PRECALL                  0
-                           580 CALL                     0
-                           590 PRECALL                  1
-                           594 CALL                     1
-               
-                71         604 LOAD_CONST               5 ('bearer')
-               
-                72         606 LOAD_FAST                7 (refresh_token)
-               
-                73         608 LOAD_GLOBAL             43 (NULL + int)
-                           620 LOAD_FAST                5 (refresh_token_expires)
-                           622 LOAD_METHOD             22 (total_seconds)
-                           644 PRECALL                  0
-                           648 CALL                     0
-                           658 PRECALL                  1
-                           662 CALL                     1
-               
-                68         672 KW_NAMES                 6
-                           674 PRECALL                  5
-                           678 CALL                     5
-                           688 STORE_FAST               8 (token)
-               
-                75         690 LOAD_GLOBAL             47 (NULL + get_cache_client)
-                           702 PRECALL                  0
-                           706 CALL                     0
-                           716 GET_AWAITABLE            0
-                           718 LOAD_CONST               2 (None)
-                       >>  720 SEND                     3 (to 728)
-                           722 YIELD_VALUE
-                           724 RESUME                   3
-                           726 JUMP_BACKWARD_NO_INTERRUPT     4 (to 720)
-                       >>  728 STORE_FAST               9 (cache_client)
-               
-                76         730 LOAD_FAST                9 (cache_client)
-                           732 LOAD_METHOD             24 (set)
-               
-                77         754 LOAD_GLOBAL             50 (SystemConstantCode)
-                           766 LOAD_ATTR               26 (USER_KEY)
-                           776 LOAD_ATTR                9 (msg)
-                           786 FORMAT_VALUE             0
-                           788 LOAD_FAST                3 (userDO)
-                           790 LOAD_ATTR               16 (id)
-                           800 FORMAT_VALUE             0
-                           802 BUILD_STRING             2
-               
-                78         804 LOAD_FAST                6 (access_token)
-               
-                79         806 LOAD_FAST                4 (access_token_expires)
-               
-                76         808 PRECALL                  3
-                           812 CALL                     3
-                           822 GET_AWAITABLE            0
-                           824 LOAD_CONST               2 (None)
-                       >>  826 SEND                     3 (to 834)
-                           828 YIELD_VALUE
-                           830 RESUME                   3
-                           832 JUMP_BACKWARD_NO_INTERRUPT     4 (to 826)
-                       >>  834 POP_TOP
+                           140 POP_JUMP_FORWARD_IF_TRUE    63 (to 268)
+               
+                76     >>  142 LOAD_GLOBAL             11 (NULL + SystemException)
+               
+                77         154 LOAD_GLOBAL             12 (SystemResponseCode)
+                           166 LOAD_ATTR                7 (AUTH_FAILED)
+                           176 LOAD_ATTR                8 (code)
+               
+                78         186 LOAD_GLOBAL             12 (SystemResponseCode)
+                           198 LOAD_ATTR                7 (AUTH_FAILED)
+                           208 LOAD_ATTR                9 (msg)
+               
+                79         218 LOAD_GLOBAL             20 (http)
+                           230 LOAD_ATTR               11 (HTTPStatus)
+                           240 LOAD_ATTR               12 (UNAUTHORIZED)
+               
+                76         250 KW_NAMES                 3
+                           252 PRECALL                  3
+                           256 CALL                     3
+                           266 RAISE_VARARGS            1
+               
+                81     >>  268 LOAD_GLOBAL             27 (NULL + timedelta)
+                           280 LOAD_GLOBAL             28 (configs)
+                           292 LOAD_ATTR               15 (access_token_expire_minutes)
+                           302 KW_NAMES                 4
+                           304 PRECALL                  1
+                           308 CALL                     1
+                           318 STORE_FAST               4 (access_token_expires)
+               
+                82         320 LOAD_GLOBAL             33 (NULL + security)
+                           332 LOAD_ATTR               17 (create_token)
+               
+                83         342 LOAD_FAST                3 (userDO)
+                           344 LOAD_ATTR               18 (id)
+               
+                84         354 LOAD_FAST                4 (access_token_expires)
+               
+                85         356 LOAD_GLOBAL             38 (TokenTypeEnum)
+                           368 LOAD_ATTR               20 (access)
+               
+                82         378 KW_NAMES                 5
+                           380 PRECALL                  3
+                           384 CALL                     3
+                           394 GET_AWAITABLE            0
+                           396 LOAD_CONST               2 (None)
+                       >>  398 SEND                     3 (to 406)
+                           400 YIELD_VALUE
+                           402 RESUME                   3
+                           404 JUMP_BACKWARD_NO_INTERRUPT     4 (to 398)
+                       >>  406 STORE_FAST               5 (access_token)
+               
+                87         408 LOAD_GLOBAL             33 (NULL + security)
+                           420 LOAD_ATTR               17 (create_token)
+               
+                88         430 LOAD_FAST                3 (userDO)
+                           432 LOAD_ATTR               18 (id)
+               
+                89         442 LOAD_GLOBAL             38 (TokenTypeEnum)
+                           454 LOAD_ATTR               21 (refresh)
+               
+                87         464 KW_NAMES                 6
+                           466 PRECALL                  2
+                           470 CALL                     2
+                           480 GET_AWAITABLE            0
+                           482 LOAD_CONST               2 (None)
+                       >>  484 SEND                     3 (to 492)
+                           486 YIELD_VALUE
+                           488 RESUME                   3
+                           490 JUMP_BACKWARD_NO_INTERRUPT     4 (to 484)
+                       >>  492 STORE_FAST               6 (refresh_token)
+               
+                91         494 LOAD_GLOBAL             45 (NULL + Token)
+               
+                92         506 LOAD_FAST                5 (access_token)
+               
+                93         508 LOAD_GLOBAL             47 (NULL + int)
+                           520 LOAD_FAST                4 (access_token_expires)
+                           522 LOAD_METHOD             24 (total_seconds)
+                           544 PRECALL                  0
+                           548 CALL                     0
+                           558 PRECALL                  1
+                           562 CALL                     1
+               
+                94         572 LOAD_CONST               7 ('bearer')
+               
+                95         574 LOAD_FAST                6 (refresh_token)
+               
+                96         576 LOAD_GLOBAL             47 (NULL + int)
+               
+                97         588 LOAD_GLOBAL             27 (NULL + timedelta)
+                           600 LOAD_GLOBAL             28 (configs)
+                           612 LOAD_ATTR               25 (refresh_token_expire_minutes)
+                           622 KW_NAMES                 4
+                           624 PRECALL                  1
+                           628 CALL                     1
+                           638 LOAD_METHOD             24 (total_seconds)
+                           660 PRECALL                  0
+                           664 CALL                     0
+               
+                96         674 PRECALL                  1
+                           678 CALL                     1
+               
+                91         688 KW_NAMES                 8
+                           690 PRECALL                  5
+                           694 CALL                     5
+                           704 STORE_FAST               7 (token)
+               
+               100         706 LOAD_GLOBAL             53 (NULL + get_cache_client)
+                           718 PRECALL                  0
+                           722 CALL                     0
+                           732 GET_AWAITABLE            0
+                           734 LOAD_CONST               2 (None)
+                       >>  736 SEND                     3 (to 744)
+                           738 YIELD_VALUE
+                           740 RESUME                   3
+                           742 JUMP_BACKWARD_NO_INTERRUPT     4 (to 736)
+                       >>  744 STORE_FAST               8 (cache_client)
+               
+               101         746 LOAD_FAST                8 (cache_client)
+                           748 LOAD_METHOD             27 (set)
+               
+               102         770 LOAD_GLOBAL             56 (SystemConstantCode)
+                           782 LOAD_ATTR               29 (USER_KEY)
+                           792 LOAD_ATTR                9 (msg)
+                           802 FORMAT_VALUE             0
+                           804 LOAD_FAST                3 (userDO)
+                           806 LOAD_ATTR               18 (id)
+                           816 FORMAT_VALUE             0
+                           818 BUILD_STRING             2
+               
+               103         820 LOAD_FAST                5 (access_token)
+               
+               104         822 LOAD_FAST                4 (access_token_expires)
+               
+               101         824 PRECALL                  3
+                           828 CALL                     3
+                           838 GET_AWAITABLE            0
+                           840 LOAD_CONST               2 (None)
+                       >>  842 SEND                     3 (to 850)
+                           844 YIELD_VALUE
+                           846 RESUME                   3
+                           848 JUMP_BACKWARD_NO_INTERRUPT     4 (to 842)
+                       >>  850 POP_TOP
                
-                81         836 LOAD_FAST                8 (token)
-                           838 RETURN_VALUE
+               106         852 LOAD_FAST                7 (token)
+                           854 RETURN_VALUE
                consts
-                  '\n        Do log in\n        :param loginCmd: loginCmd\n        :return: access token and refresh token\n        '
+                  '\n        Perform login and return an access token and refresh token.\n\n        Args:\n            loginCmd (LoginCmd): The login command containing username and password.\n\n        Returns:\n            Token: The access token and refresh token.\n        '
                   ('username',)
                   None
+                  ('status_code',)
                   ('minutes',)
                   ('subject', 'expires_delta', 'token_type')
+                  ('subject', 'token_type')
                   'bearer'
                   ('access_token', 'expired_at', 'token_type', 'refresh_token', 're_expired_at')
-               names      ('username', 'mapper', 'get_user_by_username', 'verify_password', 'password', 'SystemException', 'SystemResponseCode', 'AUTH_FAILED', 'code', 'msg', 'timedelta', 'configs', 'access_token_expire_minutes', 'refresh_token_expire_minutes', 'security', 'create_token', 'id', 'TokenTypeEnum', 'access', 'refresh', 'Token', 'int', 'total_seconds', 'get_cache_client', 'set', 'SystemConstantCode', 'USER_KEY')
-               varnames   ('self', 'loginCmd', 'username', 'userDO', 'access_token_expires', 'refresh_token_expires', 'access_token', 'refresh_token', 'token', 'cache_client')
+               names      ('username', 'mapper', 'get_user_by_username', 'verify_password', 'password', 'SystemException', 'SystemResponseCode', 'AUTH_FAILED', 'code', 'msg', 'http', 'HTTPStatus', 'UNAUTHORIZED', 'timedelta', 'configs', 'access_token_expire_minutes', 'security', 'create_token', 'id', 'TokenTypeEnum', 'access', 'refresh', 'Token', 'int', 'total_seconds', 'refresh_token_expire_minutes', 'get_cache_client', 'set', 'SystemConstantCode', 'USER_KEY')
+               varnames   ('self', 'loginCmd', 'username', 'userDO', 'access_token_expires', 'access_token', 'refresh_token', 'token', 'cache_client')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                name       'login'
-               firstlineno 44
+               firstlineno 63
                lnotab
-                  0x06060e01420144010c0140ff10033401340116010c01020116fd1e0516
-                  010c01020116fd1e050c01020140010201020140fb120728011801320102
-                  0102fd1c05
+                  0x060a0e01420138010c012001200120fd1205340116010c01020116fd1e
+                  0516010c0116fe1e040c0102014001020102010c0156ff0efb1209280118
+                  013201020102fd1c05
             code
                argcount  : 1
-               nlocals   : 7
-               stacksize : 7
+               nlocals   : 1
+               stacksize : 4
                flags     : 131
                code
-                  0x4b000100970064017d017400000000000000000000006a010000000000
-                  0000007d027405000000000000000000006a0300000000000000007c02ac
-                  02a6010000ab0100000000000000007d0364037409000000000000000000
-                  006a050000000000000000a6000000ab000000000000000000a006000000
-                  00000000000000000000000000000000006404a6010000ab010000000000
-                  0000009b0064059d037d04740f000000000000000000006a080000000000
-                  000000a6000000ab0000000000000000007d050900740500000000000000
-                  0000006a0900000000000000007c056406ac07a6020000ab020000000000
-                  0000007d017c03a00a00000000000000000000000000000000000000007c
-                  016408ac09a6020000ab02000000000000000001007c01a00b0000000000
-                  000000000000000000000000000000a6000000ab00000000000000000001
-                  007c05a00c0000000000000000000000000000000000000000640aa60100
-                  00ab0100000000000000000100741b00000000000000000000740f000000
-                  000000000000006a0800000000000000007c05a00e000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a6010000ab
-                  010000000000000000640b640c640d7c049b009d026901ac0ea6030000ab
-                  0300000000000000007c01a00f0000000000000000000000000000000000
-                  000000a6000000ab00000000000000000001005300230074200000000000
-                  00000000002400721f7d067423000000000000000000006a120000000000
-                  0000007c069b00a6010000ab0100000000000000000100590064017d067e
-                  066e0864017d067e067701770078035900770109007c01a00f0000000000
-                  000000000000000000000000000000a6000000ab00000000000000000001
-                  006401530023007c01a00f00000000000000000000000000000000000000
-                  00a6000000ab00000000000000000001007700780359007701
-                83           0 RETURN_GENERATOR
+                  0x4b00010097007401000000000000000000007402000000000000000000
+                  006401ac02a6020000ab020000000000000000830064037b035600970386
+                  045300
+               108           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                89           6 LOAD_CONST               1 (None)
-                             8 STORE_FAST               1 (excel_writer)
-               
-                90          10 LOAD_GLOBAL              0 (UserDO)
-                            22 LOAD_ATTR                1 (__fields__)
-                            32 STORE_FAST               2 (field_names)
-               
-                91          34 LOAD_GLOBAL              5 (NULL + pd)
-                            46 LOAD_ATTR                3 (DataFrame)
-                            56 LOAD_FAST                2 (field_names)
-                            58 KW_NAMES                 2
-                            60 PRECALL                  1
-                            64 CALL                     1
-                            74 STORE_FAST               3 (user_export_df)
-               
-                92          76 LOAD_CONST               3 ('user_template_')
-                            78 LOAD_GLOBAL              9 (NULL + datetime)
-                            90 LOAD_ATTR                5 (now)
-                           100 PRECALL                  0
-                           104 CALL                     0
-                           114 LOAD_METHOD              6 (strftime)
-                           136 LOAD_CONST               4 ('%Y%m%d%H%M%S')
-                           138 PRECALL                  1
-                           142 CALL                     1
-                           152 FORMAT_VALUE             0
-                           154 LOAD_CONST               5 ('.xlsx')
-                           156 BUILD_STRING             3
-                           158 STORE_FAST               4 (filename)
-               
-                93         160 LOAD_GLOBAL             15 (NULL + io)
-                           172 LOAD_ATTR                8 (BytesIO)
-                           182 PRECALL                  0
-                           186 CALL                     0
-                           196 STORE_FAST               5 (stream)
-               
-                94         198 NOP
-               
-                95         200 LOAD_GLOBAL              5 (NULL + pd)
-                           212 LOAD_ATTR                9 (ExcelWriter)
-                           222 LOAD_FAST                5 (stream)
-                           224 LOAD_CONST               6 ('xlsxwriter')
-                           226 KW_NAMES                 7
-                           228 PRECALL                  2
-                           232 CALL                     2
-                           242 STORE_FAST               1 (excel_writer)
-               
-                96         244 LOAD_FAST                3 (user_export_df)
-                           246 LOAD_METHOD             10 (to_excel)
-                           268 LOAD_FAST                1 (excel_writer)
-                           270 LOAD_CONST               8 (False)
-                           272 KW_NAMES                 9
-                           274 PRECALL                  2
-                           278 CALL                     2
-                           288 POP_TOP
-               
-                97         290 LOAD_FAST                1 (excel_writer)
-                           292 LOAD_METHOD             11 (_save)
-                           314 PRECALL                  0
-                           318 CALL                     0
-                           328 POP_TOP
-               
-                98         330 LOAD_FAST                5 (stream)
-                           332 LOAD_METHOD             12 (seek)
-                           354 LOAD_CONST              10 (0)
-                           356 PRECALL                  1
-                           360 CALL                     1
-                           370 POP_TOP
-               
-                99         372 LOAD_GLOBAL             27 (NULL + StreamingResponse)
-               
-               100         384 LOAD_GLOBAL             15 (NULL + io)
-                           396 LOAD_ATTR                8 (BytesIO)
-                           406 LOAD_FAST                5 (stream)
-                           408 LOAD_METHOD             14 (getvalue)
-                           430 PRECALL                  0
-                           434 CALL                     0
-                           444 PRECALL                  1
-                           448 CALL                     1
-               
-               101         458 LOAD_CONST              11 ('application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-               
-               102         460 LOAD_CONST              12 ('Content-Disposition')
-                           462 LOAD_CONST              13 ('attachment; filename=')
-                           464 LOAD_FAST                4 (filename)
-                           466 FORMAT_VALUE             0
-                           468 BUILD_STRING             2
-                           470 BUILD_MAP                1
-               
-                99         472 KW_NAMES                14
-                           474 PRECALL                  3
-                           478 CALL                     3
-               
-               107         488 LOAD_FAST                1 (excel_writer)
-                           490 LOAD_METHOD             15 (close)
-                           512 PRECALL                  0
-                           516 CALL                     0
-                           526 POP_TOP
-                           528 RETURN_VALUE
-                       >>  530 PUSH_EXC_INFO
-               
-               104         532 LOAD_GLOBAL             32 (Exception)
-                           544 CHECK_EXC_MATCH
-                           546 POP_JUMP_FORWARD_IF_FALSE    31 (to 610)
-                           548 STORE_FAST               6 (e)
-               
-               105         550 LOAD_GLOBAL             35 (NULL + logger)
-                           562 LOAD_ATTR               18 (error)
-                           572 LOAD_FAST                6 (e)
-                           574 FORMAT_VALUE             0
-                           576 PRECALL                  1
-                           580 CALL                     1
-                           590 POP_TOP
-                           592 POP_EXCEPT
-                           594 LOAD_CONST               1 (None)
-                           596 STORE_FAST               6 (e)
-                           598 DELETE_FAST              6 (e)
-                           600 JUMP_FORWARD             8 (to 618)
-                       >>  602 LOAD_CONST               1 (None)
-                           604 STORE_FAST               6 (e)
-                           606 DELETE_FAST              6 (e)
-                           608 RERAISE                  1
-               
-               104     >>  610 RERAISE                  0
-                       >>  612 COPY                     3
-                           614 POP_EXCEPT
-                           616 RERAISE                  1
-               
-               105     >>  618 NOP
-               
-               107         620 LOAD_FAST                1 (excel_writer)
-                           622 LOAD_METHOD             15 (close)
-                           644 PRECALL                  0
-                           648 CALL                     0
-                           658 POP_TOP
-                           660 LOAD_CONST               1 (None)
-                           662 RETURN_VALUE
-                       >>  664 PUSH_EXC_INFO
-                           666 LOAD_FAST                1 (excel_writer)
-                           668 LOAD_METHOD             15 (close)
-                           690 PRECALL                  0
-                           694 CALL                     0
-                           704 POP_TOP
-                           706 RERAISE                  0
-                       >>  708 COPY                     3
-                           710 POP_EXCEPT
-                           712 RERAISE                  1
-               ExceptionTable:
-                 200 to 486 -> 530 [0]
-                 530 to 548 -> 612 [1] lasti
-                 550 to 590 -> 602 [1] lasti
-                 592 to 600 -> 664 [0]
-                 602 to 610 -> 612 [1] lasti
-                 612 to 616 -> 664 [0]
-                 664 to 706 -> 708 [1] lasti
+               114           6 LOAD_GLOBAL              1 (NULL + export_template)
+                            18 LOAD_GLOBAL              2 (UserExport)
+                            30 LOAD_CONST               1 ('user_template')
+                            32 KW_NAMES                 2
+                            34 PRECALL                  2
+                            38 CALL                     2
+                            48 GET_AWAITABLE            0
+                            50 LOAD_CONST               3 (None)
+                       >>   52 SEND                     3 (to 60)
+                            54 YIELD_VALUE
+                            56 RESUME                   3
+                            58 JUMP_BACKWARD_NO_INTERRUPT     4 (to 52)
+                       >>   60 RETURN_VALUE
                consts
-                  '\n        Export empty user import template\n        '
+                  '\n        Export an empty user import template.\n        '
+                  'user_template'
+                  ('schema', 'file_name')
                   None
-                  ('columns',)
-                  'user_template_'
-                  '%Y%m%d%H%M%S'
-                  '.xlsx'
-                  'xlsxwriter'
-                  ('engine',)
-                  False
-                  ('index',)
-                  0
-                  'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
-                  'Content-Disposition'
-                  'attachment; filename='
-                  ('media_type', 'headers')
-               names      ('UserDO', '__fields__', 'pd', 'DataFrame', 'datetime', 'now', 'strftime', 'io', 'BytesIO', 'ExcelWriter', 'to_excel', '_save', 'seek', 'StreamingResponse', 'getvalue', 'close', 'Exception', 'logger', 'error')
-               varnames   ('self', 'excel_writer', 'field_names', 'user_export_df', 'filename', 'stream', 'e')
+               names      ('export_template', 'UserExport')
+               varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                name       'export_user_template'
-               firstlineno 83
-               lnotab
-                  0x0606040118012a015401260102012c012e0128012a010c014a0102010c
-                  fd10082cfd12013cff08010202
+               firstlineno 108
+               lnotab 0x0606
             'file'
             code
                argcount  : 2
-               nlocals   : 8
+               nlocals   : 12
                stacksize : 6
                flags     : 131
                code
                   0x4b00010097007c01a00000000000000000000000000000000000000000
                   00a6000000ab000000000000000000830064017b035600970386047d0274
                   03000000000000000000006a020000000000000000740700000000000000
                   0000006a0400000000000000007c02a6010000ab010000000000000000a6
                   010000ab0100000000000000007d03640284007c03a00500000000000000
                   000000000000000000000000006403ac04a6010000ab0100000000000000
-                  004400a6000000ab0000000000000000007d0467007d057c0444005d427d
-                  06740d00000000000000000000640669007c06a4018e017d07740f000000
-                  000000000000007c076a080000000000000000a6010000ab010000000000
-                  000000830064017b035600970386047c075f0800000000000000007c05a0
-                  0900000000000000000000000000000000000000007c07a6010000ab0100
-                  0000000000000001008c437c01a00a000000000000000000000000000000
-                  0000000000a6000000ab000000000000000000830064017b035600970386
-                  0401007c006a0b0000000000000000a00c00000000000000000000000000
-                  000000000000007c05ac05a6010000ab010000000000000000830064017b
-                  03560097038604010064015300
-               109           0 RETURN_GENERATOR
+                  004400a6000000ab0000000000000000007d0467007d0567007d067c0444
+                  005d5c7d07740d00000000000000000000640a69007c07a4018e017d0874
+                  0f000000000000000000007c086a080000000000000000a6010000ab0100
+                  00000000000000830064017b035600970386047c085f0800000000000000
+                  007c05a00900000000000000000000000000000000000000007c08a60100
+                  00ab01000000000000000001007c06a00900000000000000000000000000
+                  000000000000007c086a0a0000000000000000a6010000ab010000000000
+                  00000001008c5d7c01a00b00000000000000000000000000000000000000
+                  00a6000000ab000000000000000000830064017b0356009703860401007c
+                  006a0c0000000000000000a00d0000000000000000000000000000000000
+                  0000007c06ac05a6010000ab010000000000000000830064017b03560097
+                  0386047d09741d000000000000000000007c09a6010000ab010000000000
+                  00000064066b0400000000725264077d0a7c0944005d1c7d0b7c0a640874
+                  1f000000000000000000007c0b6a0a0000000000000000a6010000ab0100
+                  000000000000007a0000007a0d00007d0a8c1d7421000000000000000000
+                  007422000000000000000000006a1200000000000000006a130000000000
+                  0000007422000000000000000000006a1200000000000000006a14000000
+                  00000000007c0a7a000000a6020000ab02000000000000000082017c006a
+                  0c0000000000000000a01500000000000000000000000000000000000000
+                  007c05ac09a6010000ab010000000000000000830064017b035600970386
+                  04010064015300
+               116           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               113           6 LOAD_FAST                1 (file)
+               123           6 LOAD_FAST                1 (file)
                              8 LOAD_METHOD              0 (read)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_AWAITABLE            0
                             46 LOAD_CONST               1 (None)
                        >>   48 SEND                     3 (to 56)
                             50 YIELD_VALUE
                             52 RESUME                   3
                             54 JUMP_BACKWARD_NO_INTERRUPT     4 (to 48)
                        >>   56 STORE_FAST               2 (contents)
                
-               114          58 LOAD_GLOBAL              3 (NULL + pd)
+               124          58 LOAD_GLOBAL              3 (NULL + pd)
                             70 LOAD_ATTR                2 (read_excel)
                             80 LOAD_GLOBAL              7 (NULL + io)
                             92 LOAD_ATTR                4 (BytesIO)
                            102 LOAD_FAST                2 (contents)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 STORE_FAST               3 (import_df)
                
-               115         134 LOAD_CONST               2 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 115>)
+               125         134 LOAD_CONST               2 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 125>)
                            136 MAKE_FUNCTION            0
-                           138 LOAD_FAST                3 (import_df)
+               
+               126         138 LOAD_FAST                3 (import_df)
                            140 LOAD_METHOD              5 (to_dict)
                            162 LOAD_CONST               3 ('records')
                            164 KW_NAMES                 4
                            166 PRECALL                  1
                            170 CALL                     1
-                           180 GET_ITER
+               
+               125         180 GET_ITER
                            182 PRECALL                  0
                            186 CALL                     0
                            196 STORE_FAST               4 (user_datas)
                
-               116         198 BUILD_LIST               0
+               128         198 BUILD_LIST               0
                            200 STORE_FAST               5 (user_import_list)
                
-               117         202 LOAD_FAST                4 (user_datas)
-                           204 GET_ITER
-                       >>  206 FOR_ITER                66 (to 340)
-                           208 STORE_FAST               6 (user_data)
-               
-               118         210 LOAD_GLOBAL             13 (NULL + UserDO)
-                           222 LOAD_CONST               6 (())
-                           224 BUILD_MAP                0
-                           226 LOAD_FAST                6 (user_data)
-                           228 DICT_MERGE               1
-                           230 CALL_FUNCTION_EX         1
-                           232 STORE_FAST               7 (user_import)
-               
-               119         234 LOAD_GLOBAL             15 (NULL + get_password_hash)
-                           246 LOAD_FAST                7 (user_import)
-                           248 LOAD_ATTR                8 (password)
-                           258 PRECALL                  1
-                           262 CALL                     1
-                           272 GET_AWAITABLE            0
-                           274 LOAD_CONST               1 (None)
-                       >>  276 SEND                     3 (to 284)
-                           278 YIELD_VALUE
-                           280 RESUME                   3
-                           282 JUMP_BACKWARD_NO_INTERRUPT     4 (to 276)
-                       >>  284 LOAD_FAST                7 (user_import)
-                           286 STORE_ATTR               8 (password)
-               
-               120         296 LOAD_FAST                5 (user_import_list)
-                           298 LOAD_METHOD              9 (append)
-                           320 LOAD_FAST                7 (user_import)
-                           322 PRECALL                  1
-                           326 CALL                     1
-                           336 POP_TOP
-                           338 JUMP_BACKWARD           67 (to 206)
-               
-               121     >>  340 LOAD_FAST                1 (file)
-                           342 LOAD_METHOD             10 (close)
-                           364 PRECALL                  0
-                           368 CALL                     0
-                           378 GET_AWAITABLE            0
-                           380 LOAD_CONST               1 (None)
-                       >>  382 SEND                     3 (to 390)
-                           384 YIELD_VALUE
-                           386 RESUME                   3
-                           388 JUMP_BACKWARD_NO_INTERRUPT     4 (to 382)
-                       >>  390 POP_TOP
-               
-               122         392 LOAD_FAST                0 (self)
-                           394 LOAD_ATTR               11 (mapper)
-                           404 LOAD_METHOD             12 (insert_batch)
-                           426 LOAD_FAST                5 (user_import_list)
-                           428 KW_NAMES                 5
-                           430 PRECALL                  1
-                           434 CALL                     1
-                           444 GET_AWAITABLE            0
-                           446 LOAD_CONST               1 (None)
-                       >>  448 SEND                     3 (to 456)
-                           450 YIELD_VALUE
-                           452 RESUME                   3
-                           454 JUMP_BACKWARD_NO_INTERRUPT     4 (to 448)
-                       >>  456 POP_TOP
-                           458 LOAD_CONST               1 (None)
-                           460 RETURN_VALUE
+               129         202 BUILD_LIST               0
+                           204 STORE_FAST               6 (user_name_list)
+               
+               130         206 LOAD_FAST                4 (user_datas)
+                           208 GET_ITER
+                       >>  210 FOR_ITER                92 (to 396)
+                           212 STORE_FAST               7 (user_data)
+               
+               131         214 LOAD_GLOBAL             13 (NULL + UserDO)
+                           226 LOAD_CONST              10 (())
+                           228 BUILD_MAP                0
+                           230 LOAD_FAST                7 (user_data)
+                           232 DICT_MERGE               1
+                           234 CALL_FUNCTION_EX         1
+                           236 STORE_FAST               8 (user_import)
+               
+               132         238 LOAD_GLOBAL             15 (NULL + get_password_hash)
+                           250 LOAD_FAST                8 (user_import)
+                           252 LOAD_ATTR                8 (password)
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 GET_AWAITABLE            0
+                           278 LOAD_CONST               1 (None)
+                       >>  280 SEND                     3 (to 288)
+                           282 YIELD_VALUE
+                           284 RESUME                   3
+                           286 JUMP_BACKWARD_NO_INTERRUPT     4 (to 280)
+                       >>  288 LOAD_FAST                8 (user_import)
+                           290 STORE_ATTR               8 (password)
+               
+               133         300 LOAD_FAST                5 (user_import_list)
+                           302 LOAD_METHOD              9 (append)
+                           324 LOAD_FAST                8 (user_import)
+                           326 PRECALL                  1
+                           330 CALL                     1
+                           340 POP_TOP
+               
+               134         342 LOAD_FAST                6 (user_name_list)
+                           344 LOAD_METHOD              9 (append)
+                           366 LOAD_FAST                8 (user_import)
+                           368 LOAD_ATTR               10 (username)
+                           378 PRECALL                  1
+                           382 CALL                     1
+                           392 POP_TOP
+                           394 JUMP_BACKWARD           93 (to 210)
+               
+               135     >>  396 LOAD_FAST                1 (file)
+                           398 LOAD_METHOD             11 (close)
+                           420 PRECALL                  0
+                           424 CALL                     0
+                           434 GET_AWAITABLE            0
+                           436 LOAD_CONST               1 (None)
+                       >>  438 SEND                     3 (to 446)
+                           440 YIELD_VALUE
+                           442 RESUME                   3
+                           444 JUMP_BACKWARD_NO_INTERRUPT     4 (to 438)
+                       >>  446 POP_TOP
+               
+               136         448 LOAD_FAST                0 (self)
+                           450 LOAD_ATTR               12 (mapper)
+                           460 LOAD_METHOD             13 (get_user_by_usernames)
+               
+               137         482 LOAD_FAST                6 (user_name_list)
+               
+               136         484 KW_NAMES                 5
+                           486 PRECALL                  1
+                           490 CALL                     1
+                           500 GET_AWAITABLE            0
+                           502 LOAD_CONST               1 (None)
+                       >>  504 SEND                     3 (to 512)
+                           506 YIELD_VALUE
+                           508 RESUME                   3
+                           510 JUMP_BACKWARD_NO_INTERRUPT     4 (to 504)
+                       >>  512 STORE_FAST               9 (user_list)
+               
+               140         514 LOAD_GLOBAL             29 (NULL + len)
+                           526 LOAD_FAST                9 (user_list)
+                           528 PRECALL                  1
+                           532 CALL                     1
+                           542 LOAD_CONST               6 (0)
+                           544 COMPARE_OP               4 (>)
+                           550 POP_JUMP_FORWARD_IF_FALSE    82 (to 716)
+               
+               141         552 LOAD_CONST               7 ('')
+                           554 STORE_FAST              10 (err_msg)
+               
+               142         556 LOAD_FAST                9 (user_list)
+                           558 GET_ITER
+                       >>  560 FOR_ITER                28 (to 618)
+                           562 STORE_FAST              11 (user)
+               
+               143         564 LOAD_FAST               10 (err_msg)
+                           566 LOAD_CONST               8 (',')
+                           568 LOAD_GLOBAL             31 (NULL + str)
+                           580 LOAD_FAST               11 (user)
+                           582 LOAD_ATTR               10 (username)
+                           592 PRECALL                  1
+                           596 CALL                     1
+                           606 BINARY_OP                0 (+)
+                           610 BINARY_OP               13 (+=)
+                           614 STORE_FAST              10 (err_msg)
+                           616 JUMP_BACKWARD           29 (to 560)
+               
+               144     >>  618 LOAD_GLOBAL             33 (NULL + SystemException)
+               
+               145         630 LOAD_GLOBAL             34 (SystemResponseCode)
+                           642 LOAD_ATTR               18 (USER_NAME_EXISTS)
+                           652 LOAD_ATTR               19 (code)
+               
+               146         662 LOAD_GLOBAL             34 (SystemResponseCode)
+                           674 LOAD_ATTR               18 (USER_NAME_EXISTS)
+                           684 LOAD_ATTR               20 (msg)
+                           694 LOAD_FAST               10 (err_msg)
+                           696 BINARY_OP                0 (+)
+               
+               144         700 PRECALL                  2
+                           704 CALL                     2
+                           714 RAISE_VARARGS            1
+               
+               148     >>  716 LOAD_FAST                0 (self)
+                           718 LOAD_ATTR               12 (mapper)
+                           728 LOAD_METHOD             21 (insert_batch)
+                           750 LOAD_FAST                5 (user_import_list)
+                           752 KW_NAMES                 9
+                           754 PRECALL                  1
+                           758 CALL                     1
+                           768 GET_AWAITABLE            0
+                           770 LOAD_CONST               1 (None)
+                       >>  772 SEND                     3 (to 780)
+                           774 YIELD_VALUE
+                           776 RESUME                   3
+                           778 JUMP_BACKWARD_NO_INTERRUPT     4 (to 772)
+                       >>  780 POP_TOP
+                           782 LOAD_CONST               1 (None)
+                           784 RETURN_VALUE
                consts
-                  '\n        Import user data\n        '
+                  '\n        Import user data from an Excel file.\n\n        Args:\n            file (UploadFile): The Excel file containing user data.\n        '
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     115           0 RESUME                   0
+                     125           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
-                                   8 STORE_FAST               1 (user_data)
+                     
+                     126           8 STORE_FAST               1 (user_data)
                                   10 LOAD_FAST                1 (user_data)
-                                  12 LIST_APPEND              2
+                     
+                     125          12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'user_data')
                      freevars   ()
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                      name       '<listcomp>'
-                     firstlineno 115
-                     lnotab 0x
+                     firstlineno 125
+                     lnotab 0x080104ff
                   'records'
                   ('orient',)
+                  ('usernames',)
+                  0
+                  ''
+                  ','
                   ('data_list',)
                   ()
-               names      ('read', 'pd', 'read_excel', 'io', 'BytesIO', 'to_dict', 'UserDO', 'get_password_hash', 'password', 'append', 'close', 'mapper', 'insert_batch')
-               varnames   ('self', 'file', 'contents', 'import_df', 'user_datas', 'user_import_list', 'user_data', 'user_import')
+               names      ('read', 'pd', 'read_excel', 'io', 'BytesIO', 'to_dict', 'UserDO', 'get_password_hash', 'password', 'append', 'username', 'close', 'mapper', 'get_user_by_usernames', 'len', 'str', 'SystemException', 'SystemResponseCode', 'USER_NAME_EXISTS', 'code', 'msg', 'insert_batch')
+               varnames   ('self', 'file', 'contents', 'import_df', 'user_datas', 'user_import_list', 'user_name_list', 'user_data', 'user_import', 'user_list', 'err_msg', 'user')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                name       'import_user'
-               firstlineno 109
-               lnotab 0x060434014c0140010401080118013e012c013401
+               firstlineno 116
+               lnotab
+                  0x060734014c0104012aff120304010401080118013e012a013601340122
+                  0102ff1e0426010401080136010c01200126fe1004
             'params'
             code
                argcount  : 2
-               nlocals   : 12
+               nlocals   : 6
                stacksize : 9
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c01ac01a6010000ab01000000000000000083
-                  0064007b035600970386047d027405000000000000000000007407000000
-                  000000000000007c02a6010000ab010000000000000000a6010000ab0100
-                  0000000000000001007405000000000000000000007c02a6010000ab0100
-                  0000000000000001007c026a040000000000000000640219000000000000
-                  0000007d0367007d047c0344005d337d057c04a005000000000000000000
-                  0000000000000000000000740d00000000000000000000641369007c05a0
-                  070000000000000000000000000000000000000000a6000000ab00000000
-                  0000000000a4018e01a6010000ab01000000000000000001008c34740c00
-                  0000000000000000006a0800000000000000007d06741300000000000000
-                  0000006a0a00000000000000007c06ac03a6010000ab0100000000000000
-                  007d07640484007c044400a6000000ab0000000000000000007d087c07a0
-                  0b00000000000000000000000000000000000000007c086405ac06a60200
-                  00ab0200000000000000007d0764077419000000000000000000006a0d00
-                  00000000000000a6000000ab000000000000000000a00e00000000000000
-                  000000000000000000000000006408a6010000ab0100000000000000009b
-                  0064099d037d09741f000000000000000000006a100000000000000000a6
-                  000000ab0000000000000000007d0a09007413000000000000000000006a
-                  1100000000000000007c0a640aac0ba6020000ab02000000000000000061
-                  127c07a01300000000000000000000000000000000000000007424000000
-                  00000000000000640cac0da6020000ab0200000000000000000100742400
-                  000000000000000000a01400000000000000000000000000000000000000
-                  00a6000000ab00000000000000000001007c0aa015000000000000000000
-                  0000000000000000000000640ea6010000ab010000000000000000010074
-                  2d00000000000000000000741f000000000000000000006a100000000000
-                  0000007c0aa0170000000000000000000000000000000000000000a60000
-                  00ab000000000000000000a6010000ab010000000000000000640f641064
-                  117c099b009d026901ac12a6030000ab0300000000000000007424000000
-                  00000000000000a0180000000000000000000000000000000000000000a6
-                  000000ab0000000000000000000100530023007432000000000000000000
-                  002400721f7d0b7435000000000000000000006a1b00000000000000007c
-                  0b9b00a6010000ab0100000000000000000100590064007d0b7e0b6e0864
-                  007d0b7e0b770177007803590077010900742400000000000000000000a0
-                  180000000000000000000000000000000000000000a6000000ab00000000
-                  00000000000100640053002300742400000000000000000000a018000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  0001007700780359007701
-               124           0 RETURN_GENERATOR
+                  0064027b035600970386047d027c026a0200000000000000006403190000
+                  000000000000007d0367007d047c0344005d337d057c04a0030000000000
+                  000000000000000000000000000000740900000000000000000000640669
+                  007c05a0050000000000000000000000000000000000000000a6000000ab
+                  000000000000000000a4018e01a6010000ab01000000000000000001008c
+                  34740d0000000000000000000074080000000000000000000064047c04ac
+                  05a6030000ab030000000000000000830064027b035600970386045300
+               150           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               126           6 LOAD_FAST                0 (self)
+               160           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
-                            18 LOAD_METHOD              1 (select_list_page_ordered)
+                            18 LOAD_METHOD              1 (select_page)
                             40 LOAD_FAST                1 (params)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 GET_AWAITABLE            0
-                            60 LOAD_CONST               0 (None)
+                            60 LOAD_CONST               2 (None)
                        >>   62 SEND                     3 (to 70)
                             64 YIELD_VALUE
                             66 RESUME                   3
                             68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
                        >>   70 STORE_FAST               2 (user_pages)
                
-               127          72 LOAD_GLOBAL              5 (NULL + print)
-                            84 LOAD_GLOBAL              7 (NULL + type)
-                            96 LOAD_FAST                2 (user_pages)
-                            98 PRECALL                  1
-                           102 CALL                     1
-                           112 PRECALL                  1
-                           116 CALL                     1
-                           126 POP_TOP
-               
-               128         128 LOAD_GLOBAL              5 (NULL + print)
-                           140 LOAD_FAST                2 (user_pages)
-                           142 PRECALL                  1
-                           146 CALL                     1
-                           156 POP_TOP
-               
-               129         158 LOAD_FAST                2 (user_pages)
-                           160 LOAD_ATTR                4 (__dict__)
-                           170 LOAD_CONST               2 ('items')
-                           172 BINARY_SUBSCR
-                           182 STORE_FAST               3 (user_items)
-               
-               130         184 BUILD_LIST               0
-                           186 STORE_FAST               4 (user_data)
-               
-               131         188 LOAD_FAST                3 (user_items)
-                           190 GET_ITER
-                       >>  192 FOR_ITER                51 (to 296)
-                           194 STORE_FAST               5 (user)
-               
-               132         196 LOAD_FAST                4 (user_data)
-                           198 LOAD_METHOD              5 (append)
-                           220 LOAD_GLOBAL             13 (NULL + UserQuery)
-                           232 LOAD_CONST              19 (())
-                           234 BUILD_MAP                0
-                           236 LOAD_FAST                5 (user)
-                           238 LOAD_METHOD              7 (model_dump)
-                           260 PRECALL                  0
-                           264 CALL                     0
-                           274 DICT_MERGE               1
-                           276 CALL_FUNCTION_EX         1
-                           278 PRECALL                  1
-                           282 CALL                     1
-                           292 POP_TOP
-                           294 JUMP_BACKWARD           52 (to 192)
-               
-               133     >>  296 LOAD_GLOBAL             12 (UserQuery)
-                           308 LOAD_ATTR                8 (__fields__)
-                           318 STORE_FAST               6 (field_names)
-               
-               134         320 LOAD_GLOBAL             19 (NULL + pd)
-                           332 LOAD_ATTR               10 (DataFrame)
-                           342 LOAD_FAST                6 (field_names)
-                           344 KW_NAMES                 3
-                           346 PRECALL                  1
-                           350 CALL                     1
-                           360 STORE_FAST               7 (user_export_df)
-               
-               135         362 LOAD_CONST               4 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\starter\system\service\impl\user_service_impl.py", line 135>)
-                           364 MAKE_FUNCTION            0
-                           366 LOAD_FAST                4 (user_data)
-                           368 GET_ITER
-                           370 PRECALL                  0
-                           374 CALL                     0
-                           384 STORE_FAST               8 (user_dicts)
-               
-               136         386 LOAD_FAST                7 (user_export_df)
-                           388 LOAD_METHOD             11 (_append)
-                           410 LOAD_FAST                8 (user_dicts)
-                           412 LOAD_CONST               5 (True)
-                           414 KW_NAMES                 6
-                           416 PRECALL                  2
-                           420 CALL                     2
-                           430 STORE_FAST               7 (user_export_df)
-               
-               137         432 LOAD_CONST               7 ('user_data_')
-                           434 LOAD_GLOBAL             25 (NULL + datetime)
-                           446 LOAD_ATTR               13 (now)
-                           456 PRECALL                  0
-                           460 CALL                     0
-                           470 LOAD_METHOD             14 (strftime)
-                           492 LOAD_CONST               8 ('%Y%m%d%H%M%S')
-                           494 PRECALL                  1
-                           498 CALL                     1
-                           508 FORMAT_VALUE             0
-                           510 LOAD_CONST               9 ('.xlsx')
-                           512 BUILD_STRING             3
-                           514 STORE_FAST               9 (filename)
-               
-               138         516 LOAD_GLOBAL             31 (NULL + io)
-                           528 LOAD_ATTR               16 (BytesIO)
-                           538 PRECALL                  0
-                           542 CALL                     0
-                           552 STORE_FAST              10 (stream)
-               
-               139         554 NOP
-               
-               140         556 LOAD_GLOBAL             19 (NULL + pd)
-                           568 LOAD_ATTR               17 (ExcelWriter)
-                           578 LOAD_FAST               10 (stream)
-                           580 LOAD_CONST              10 ('xlsxwriter')
-                           582 KW_NAMES                11
-                           584 PRECALL                  2
-                           588 CALL                     2
-                           598 STORE_GLOBAL            18 (excel_writer)
-               
-               141         600 LOAD_FAST                7 (user_export_df)
-                           602 LOAD_METHOD             19 (to_excel)
-                           624 LOAD_GLOBAL             36 (excel_writer)
-                           636 LOAD_CONST              12 (False)
-                           638 KW_NAMES                13
-                           640 PRECALL                  2
-                           644 CALL                     2
-                           654 POP_TOP
-               
-               142         656 LOAD_GLOBAL             36 (excel_writer)
-                           668 LOAD_METHOD             20 (_save)
-                           690 PRECALL                  0
-                           694 CALL                     0
-                           704 POP_TOP
-               
-               143         706 LOAD_FAST               10 (stream)
-                           708 LOAD_METHOD             21 (seek)
-                           730 LOAD_CONST              14 (0)
-                           732 PRECALL                  1
-                           736 CALL                     1
-                           746 POP_TOP
-               
-               144         748 LOAD_GLOBAL             45 (NULL + StreamingResponse)
-               
-               145         760 LOAD_GLOBAL             31 (NULL + io)
-                           772 LOAD_ATTR               16 (BytesIO)
-                           782 LOAD_FAST               10 (stream)
-                           784 LOAD_METHOD             23 (getvalue)
-                           806 PRECALL                  0
-                           810 CALL                     0
-                           820 PRECALL                  1
-                           824 CALL                     1
-               
-               146         834 LOAD_CONST              15 ('application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-               
-               147         836 LOAD_CONST              16 ('Content-Disposition')
-                           838 LOAD_CONST              17 ('attachment; filename=')
-                           840 LOAD_FAST                9 (filename)
-                           842 FORMAT_VALUE             0
-                           844 BUILD_STRING             2
-                           846 BUILD_MAP                1
-               
-               144         848 KW_NAMES                18
-                           850 PRECALL                  3
-                           854 CALL                     3
-               
-               152         864 LOAD_GLOBAL             36 (excel_writer)
-                           876 LOAD_METHOD             24 (close)
-                           898 PRECALL                  0
-                           902 CALL                     0
-                           912 POP_TOP
-                           914 RETURN_VALUE
-                       >>  916 PUSH_EXC_INFO
-               
-               149         918 LOAD_GLOBAL             50 (Exception)
-                           930 CHECK_EXC_MATCH
-                           932 POP_JUMP_FORWARD_IF_FALSE    31 (to 996)
-                           934 STORE_FAST              11 (e)
-               
-               150         936 LOAD_GLOBAL             53 (NULL + logger)
-                           948 LOAD_ATTR               27 (error)
-                           958 LOAD_FAST               11 (e)
-                           960 FORMAT_VALUE             0
-                           962 PRECALL                  1
-                           966 CALL                     1
-                           976 POP_TOP
-                           978 POP_EXCEPT
-                           980 LOAD_CONST               0 (None)
-                           982 STORE_FAST              11 (e)
-                           984 DELETE_FAST             11 (e)
-                           986 JUMP_FORWARD             8 (to 1004)
-                       >>  988 LOAD_CONST               0 (None)
-                           990 STORE_FAST              11 (e)
-                           992 DELETE_FAST             11 (e)
-                           994 RERAISE                  1
-               
-               149     >>  996 RERAISE                  0
-                       >>  998 COPY                     3
-                          1000 POP_EXCEPT
-                          1002 RERAISE                  1
-               
-               150     >> 1004 NOP
-               
-               152        1006 LOAD_GLOBAL             36 (excel_writer)
-                          1018 LOAD_METHOD             24 (close)
-                          1040 PRECALL                  0
-                          1044 CALL                     0
-                          1054 POP_TOP
-                          1056 LOAD_CONST               0 (None)
-                          1058 RETURN_VALUE
-                       >> 1060 PUSH_EXC_INFO
-                          1062 LOAD_GLOBAL             36 (excel_writer)
-                          1074 LOAD_METHOD             24 (close)
-                          1096 PRECALL                  0
-                          1100 CALL                     0
-                          1110 POP_TOP
-                          1112 RERAISE                  0
-                       >> 1114 COPY                     3
-                          1116 POP_EXCEPT
-                          1118 RERAISE                  1
-               ExceptionTable:
-                 556 to 862 -> 916 [0]
-                 916 to 934 -> 998 [1] lasti
-                 936 to 976 -> 988 [1] lasti
-                 978 to 986 -> 1060 [0]
-                 988 to 996 -> 998 [1] lasti
-                 998 to 1002 -> 1060 [0]
-                 1060 to 1112 -> 1114 [1] lasti
+               161          72 LOAD_FAST                2 (user_pages)
+                            74 LOAD_ATTR                2 (__dict__)
+                            84 LOAD_CONST               3 ('items')
+                            86 BINARY_SUBSCR
+                            96 STORE_FAST               3 (user_items)
+               
+               162          98 BUILD_LIST               0
+                           100 STORE_FAST               4 (user_data)
+               
+               163         102 LOAD_FAST                3 (user_items)
+                           104 GET_ITER
+                       >>  106 FOR_ITER                51 (to 210)
+                           108 STORE_FAST               5 (user)
+               
+               164         110 LOAD_FAST                4 (user_data)
+                           112 LOAD_METHOD              3 (append)
+                           134 LOAD_GLOBAL              9 (NULL + UserQuery)
+                           146 LOAD_CONST               6 (())
+                           148 BUILD_MAP                0
+                           150 LOAD_FAST                5 (user)
+                           152 LOAD_METHOD              5 (model_dump)
+                           174 PRECALL                  0
+                           178 CALL                     0
+                           188 DICT_MERGE               1
+                           190 CALL_FUNCTION_EX         1
+                           192 PRECALL                  1
+                           196 CALL                     1
+                           206 POP_TOP
+                           208 JUMP_BACKWARD           52 (to 106)
+               
+               165     >>  210 LOAD_GLOBAL             13 (NULL + export_template)
+               
+               166         222 LOAD_GLOBAL              8 (UserQuery)
+                           234 LOAD_CONST               4 ('user')
+                           236 LOAD_FAST                4 (user_data)
+               
+               165         238 KW_NAMES                 5
+                           240 PRECALL                  3
+                           244 CALL                     3
+                           254 GET_AWAITABLE            0
+                           256 LOAD_CONST               2 (None)
+                       >>  258 SEND                     3 (to 266)
+                           260 YIELD_VALUE
+                           262 RESUME                   3
+                           264 JUMP_BACKWARD_NO_INTERRUPT     4 (to 258)
+                       >>  266 RETURN_VALUE
                consts
-                  None
+                  '\n        Export user data to an Excel file.\n\n        Args:\n            params (Params): The query parameters for filtering users.\n\n        Returns:\n            StreamingResponse: The Excel file containing user data.\n        '
                   ('params',)
+                  None
                   'items'
-                  ('columns',)
+                  'user'
+                  ('schema', 'file_name', 'data_list')
+                  ()
+               names      ('mapper', 'select_page', '__dict__', 'append', 'UserQuery', 'model_dump', 'export_template')
+               varnames   ('self', 'params', 'user_pages', 'user_items', 'user_data', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               name       'export_user'
+               firstlineno 150
+               lnotab 0x060a42011a010401080164010c0110ff
+            'data'
+            code
+               argcount  : 2
+               nlocals   : 3
+               stacksize : 4
+               flags     : 131
+               code
+                  0x4b00010097007c006a000000000000000000a001000000000000000000
+                  00000000000000000000007c016a020000000000000000ac01a6010000ab
+                  010000000000000000830064027b035600970386047d027c02812e740700
+                  0000000000000000007408000000000000000000006a0500000000000000
+                  006a0600000000000000007408000000000000000000006a050000000000
+                  0000006a070000000000000000a6020000ab02000000000000000082017c
+                  006a000000000000000000a0080000000000000000000000000000000000
+                  0000007c01ac03a6010000ab010000000000000000830064027b03560097
+                  0386045300
+               169           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
+               
+               179           6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (mapper)
+                            18 LOAD_METHOD              1 (get_user_by_username)
+                            40 LOAD_FAST                1 (data)
+                            42 LOAD_ATTR                2 (username)
+                            52 KW_NAMES                 1
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 GET_AWAITABLE            0
+                            70 LOAD_CONST               2 (None)
+                       >>   72 SEND                     3 (to 80)
+                            74 YIELD_VALUE
+                            76 RESUME                   3
+                            78 JUMP_BACKWARD_NO_INTERRUPT     4 (to 72)
+                       >>   80 STORE_FAST               2 (user)
+               
+               180          82 LOAD_FAST                2 (user)
+                            84 POP_JUMP_FORWARD_IF_NONE    46 (to 178)
+               
+               181          86 LOAD_GLOBAL              7 (NULL + ServiceException)
+               
+               182          98 LOAD_GLOBAL              8 (SystemResponseCode)
+                           110 LOAD_ATTR                5 (USER_NAME_EXISTS)
+                           120 LOAD_ATTR                6 (code)
+               
+               183         130 LOAD_GLOBAL              8 (SystemResponseCode)
+                           142 LOAD_ATTR                5 (USER_NAME_EXISTS)
+                           152 LOAD_ATTR                7 (msg)
+               
+               181         162 PRECALL                  2
+                           166 CALL                     2
+                           176 RAISE_VARARGS            1
+               
+               185     >>  178 LOAD_FAST                0 (self)
+                           180 LOAD_ATTR                0 (mapper)
+                           190 LOAD_METHOD              8 (insert)
+                           212 LOAD_FAST                1 (data)
+                           214 KW_NAMES                 3
+                           216 PRECALL                  1
+                           220 CALL                     1
+                           230 GET_AWAITABLE            0
+                           232 LOAD_CONST               2 (None)
+                       >>  234 SEND                     3 (to 242)
+                           236 YIELD_VALUE
+                           238 RESUME                   3
+                           240 JUMP_BACKWARD_NO_INTERRUPT     4 (to 234)
+                       >>  242 RETURN_VALUE
+               consts
+                  '\n        Register a new user.\n\n        Args:\n            data (UserCreateCmd): The user creation command containing username and password.\n\n        Returns:\n            UserDO: The newly created user.\n        '
+                  ('username',)
+                  None
+                  ('data',)
+               names      ('mapper', 'get_user_by_username', 'username', 'ServiceException', 'SystemResponseCode', 'USER_NAME_EXISTS', 'code', 'msg', 'insert')
+               varnames   ('self', 'data', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               name       'register'
+               firstlineno 169
+               lnotab 0x060a4c0104010c01200120fe1004
+            'page'
+            'size'
+            code
+               argcount  : 3
+               nlocals   : 4
+               stacksize : 4
+               flags     : 131
+               code
+                  0x4b00010097007c006a000000000000000000a001000000000000000000
+                  00000000000000000000007c017c02ac01a6020000ab0200000000000000
+                  00830064027b035600970386047d03640384007c034400a6000000ab0000
+                  000000000000005300
+               187           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
+               
+               198           6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (mapper)
+                            18 LOAD_METHOD              1 (select_list)
+                            40 LOAD_FAST                1 (page)
+                            42 LOAD_FAST                2 (size)
+                            44 KW_NAMES                 1
+                            46 PRECALL                  2
+                            50 CALL                     2
+                            60 GET_AWAITABLE            0
+                            62 LOAD_CONST               2 (None)
+                       >>   64 SEND                     3 (to 72)
+                            66 YIELD_VALUE
+                            68 RESUME                   3
+                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
+                       >>   72 STORE_FAST               3 (results)
+               
+               199          74 LOAD_CONST               3 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\starter\system\service\impl\user_service_impl.py", line 199>)
+                            76 MAKE_FUNCTION            0
+                            78 LOAD_FAST                3 (results)
+                            80 GET_ITER
+                            82 PRECALL                  0
+                            86 CALL                     0
+                            96 RETURN_VALUE
+               consts
+                  '\n        List users with pagination.\n\n        Args:\n            page (int): The page number.\n            size (int): The page size.\n\n        Returns:\n            Optional[List[UserQuery]]: The list of users or None if no users are found.\n        '
+                  ('page', 'size')
+                  None
                   code
                      argcount  : 1
                      nlocals   : 2
-                     stacksize : 4
+                     stacksize : 8
                      flags     : 19
                      code
-                        0x970067007c005d167d017c01a000000000000000000000000000000000
-                        0000000000a6000000ab00000000000000000091028c175300
-                     135           0 RESUME                   0
+                        0x970067007c005d207d01740100000000000000000000640069007c01a0
+                        010000000000000000000000000000000000000000a6000000ab00000000
+                        0000000000a4018e0191028c215300
+                     199           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
-                             >>    6 FOR_ITER                22 (to 52)
-                                   8 STORE_FAST               1 (item)
-                                  10 LOAD_FAST                1 (item)
-                                  12 LOAD_METHOD              0 (dict)
-                                  34 PRECALL                  0
-                                  38 CALL                     0
-                                  48 LIST_APPEND              2
-                                  50 JUMP_BACKWARD           23 (to 6)
-                             >>   52 RETURN_VALUE
+                             >>    6 FOR_ITER                32 (to 72)
+                                   8 STORE_FAST               1 (user)
+                                  10 LOAD_GLOBAL              1 (NULL + UserQuery)
+                                  22 LOAD_CONST               0 (())
+                                  24 BUILD_MAP                0
+                                  26 LOAD_FAST                1 (user)
+                                  28 LOAD_METHOD              1 (model_dump)
+                                  50 PRECALL                  0
+                                  54 CALL                     0
+                                  64 DICT_MERGE               1
+                                  66 CALL_FUNCTION_EX         1
+                                  68 LIST_APPEND              2
+                                  70 JUMP_BACKWARD           33 (to 6)
+                             >>   72 RETURN_VALUE
                      consts
-                     names      ('dict',)
-                     varnames   ('.0', 'item')
+                        ()
+                     names      ('UserQuery', 'model_dump')
+                     varnames   ('.0', 'user')
                      freevars   ()
                      cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
                      name       '<listcomp>'
-                     firstlineno 135
+                     firstlineno 199
                      lnotab 0x
-                  True
-                  ('ignore_index',)
-                  'user_data_'
-                  '%Y%m%d%H%M%S'
-                  '.xlsx'
-                  'xlsxwriter'
-                  ('engine',)
-                  False
-                  ('index',)
-                  0
-                  'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
-                  'Content-Disposition'
-                  'attachment; filename='
-                  ('media_type', 'headers')
-                  ()
-               names      ('mapper', 'select_list_page_ordered', 'print', 'type', '__dict__', 'append', 'UserQuery', 'model_dump', '__fields__', 'pd', 'DataFrame', '_append', 'datetime', 'now', 'strftime', 'io', 'BytesIO', 'ExcelWriter', 'excel_writer', 'to_excel', '_save', 'seek', 'StreamingResponse', 'getvalue', 'close', 'Exception', 'logger', 'error')
-               varnames   ('self', 'params', 'user_pages', 'user_items', 'user_data', 'user', 'field_names', 'user_export_df', 'user_dicts', 'filename', 'stream', 'e')
+               names      ('mapper', 'select_list')
+               varnames   ('self', 'page', 'size', 'results')
                freevars   ()
                cellvars   ()
-               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
-               name       'export_user'
-               firstlineno 124
-               lnotab
-                  0x0602420138011e011a0104010801640118012a0118012e015401260102
-                  012c01380132012a010c014a0102010cfd100836fd12013cff08010202
-         names      ('__name__', '__module__', '__qualname__', 'UserMapper', '__init__', 'int', 'Optional', 'UserQuery', 'find_by_id', 'LoginCmd', 'Token', 'login', 'StreamingResponse', 'export_user_template', 'UploadFile', 'import_user', 'Params', 'export_user', '__classcell__')
+               filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+               name       'list_user'
+               firstlineno 187
+               lnotab 0x060b4401
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'UserMapper', '__init__', 'int', 'Optional', 'UserQuery', 'find_by_id', 'LoginCmd', 'Token', 'login', 'StreamingResponse', 'export_user_template', 'UploadFile', 'import_user', 'Params', 'export_user', 'UserCreateCmd', 'UserDO', 'register', 'List', 'list_user', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
          name       'UserServiceImpl'
-         firstlineno 27
-         lnotab 0x0c0110041c0c1027020202fe081a0c0f
+         firstlineno 35
+         lnotab 0x0c010404100a1c0d102d020202fe08080c2210131012
       'UserServiceImpl'
       'return'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x9700740100000000000000000000740200000000000000000000ac01a6
             010000ab0100000000000000005300
-         155           0 RESUME                   0
+         202           0 RESUME                   0
          
-         156           2 LOAD_GLOBAL              1 (NULL + UserServiceImpl)
+         209           2 LOAD_GLOBAL              1 (NULL + UserServiceImpl)
                       14 LOAD_GLOBAL              2 (userMapper)
                       26 KW_NAMES                 1
                       28 PRECALL                  1
                       32 CALL                     1
                       42 RETURN_VALUE
          consts
-            None
+            '\n    Return an instance of the UserService implementation.\n\n    Returns:\n        UserService: An instance of the UserServiceImpl class.\n    '
             ('mapper',)
          names      ('UserServiceImpl', 'userMapper')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
          name       'get_user_service'
-         firstlineno 155
-         lnotab 0x0201
-   names      ('__doc__', 'io', 'datetime', 'timedelta', 'typing', 'Optional', 'pandas', 'pd', 'fastapi', 'UploadFile', 'fastapi_pagination', 'Params', 'loguru', 'logger', 'starlette.responses', 'StreamingResponse', 'fss.common.cache.cache', 'get_cache_client', 'Cache', 'fss.common.config', 'configs', 'fss.common.enum.enum', 'TokenTypeEnum', 'fss.common.schema.schema', 'Token', 'fss.common.service.impl.service_impl', 'ServiceImpl', 'fss.common.util', 'security', 'fss.common.util.security', 'verify_password', 'get_password_hash', 'fss.starter.system.enum.system', 'SystemResponseCode', 'SystemConstantCode', 'fss.starter.system.exception.system', 'SystemException', 'fss.starter.system.mapper.user_mapper', 'UserMapper', 'userMapper', 'fss.starter.system.schema.user_schema', 'UserQuery', 'LoginCmd', 'UserDO', 'fss.starter.system.service.user_service', 'UserService', 'UserServiceImpl', 'get_user_service')
+         firstlineno 202
+         lnotab 0x0207
+   names      ('__doc__', 'http', 'io', 'datetime', 'timedelta', 'typing', 'Optional', 'List', 'pandas', 'pd', 'fastapi', 'UploadFile', 'fastapi_pagination', 'Params', 'starlette.responses', 'StreamingResponse', 'fss.common.cache.cache', 'get_cache_client', 'Cache', 'fss.common.config', 'configs', 'fss.common.enum.enum', 'TokenTypeEnum', 'fss.common.exception.exception', 'ServiceException', 'fss.common.schema.schema', 'Token', 'fss.common.security', 'security', 'fss.common.service.impl.service_impl', 'ServiceImpl', 'fss.common.util.excel', 'export_template', 'fss.common.security.security', 'verify_password', 'get_password_hash', 'fss.starter.system.enum.system', 'SystemResponseCode', 'SystemConstantCode', 'fss.starter.system.exception.system', 'SystemException', 'fss.starter.system.mapper.user_mapper', 'UserMapper', 'userMapper', 'fss.starter.system.model.user_do', 'UserDO', 'fss.starter.system.schema.user_schema', 'UserQuery', 'LoginCmd', 'UserExport', 'UserCreateCmd', 'fss.starter.system.service.user_service', 'UserService', 'UserServiceImpl', 'get_user_service')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\starter\\system\\service\\impl\\user_service_impl.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010402080110010c0208010c010c010c010c0210010c010c010c
-      010c010c01100110010c01100114010c032e7f0001
+      0x00ff02010402080108010c01100208010c010c010c0210010c010c010c
+      010c010c010c010c01100110010c0110010c0118060c032e7f0028
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/user_service_impl.py` & `fastapi_sqlmodel_starter-1.0.1/fss/starter/system/service/impl/user_service_impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,209 @@
 """User domain service impl"""
 
+import http
 import io
 from datetime import timedelta
-from typing import Optional
+from typing import Optional, List
 
 import pandas as pd
 from fastapi import UploadFile
 from fastapi_pagination import Params
 from starlette.responses import StreamingResponse
 
 from fss.common.cache.cache import get_cache_client, Cache
 from fss.common.config import configs
 from fss.common.enum.enum import TokenTypeEnum
+from fss.common.exception.exception import ServiceException
 from fss.common.schema.schema import Token
+from fss.common.security import security
 from fss.common.service.impl.service_impl import ServiceImpl
-from fss.common.util import security
 from fss.common.util.excel import export_template
-from fss.common.util.security import verify_password, get_password_hash
+from fss.common.security.security import verify_password, get_password_hash
 from fss.starter.system.enum.system import SystemResponseCode, SystemConstantCode
 from fss.starter.system.exception.system import SystemException
 from fss.starter.system.mapper.user_mapper import UserMapper, userMapper
 from fss.starter.system.model.user_do import UserDO
-from fss.starter.system.schema.user_schema import UserQuery, LoginCmd, UserExport
+from fss.starter.system.schema.user_schema import (
+    UserQuery,
+    LoginCmd,
+    UserExport,
+    UserCreateCmd,
+)
 from fss.starter.system.service.user_service import UserService
 
 
 class UserServiceImpl(ServiceImpl[UserMapper, UserDO], UserService):
+    """
+    Implementation of the UserService interface.
+    """
+
     def __init__(self, mapper: UserMapper):
-        super(UserServiceImpl, self).__init__(mapper=mapper)
+        """
+        Initialize the UserServiceImpl instance.
+
+        Args:
+            mapper (UserMapper): The UserMapper instance to use for database operations.
+        """
+        super().__init__(mapper=mapper)
         self.mapper = mapper
 
     async def find_by_id(self, id: int) -> Optional[UserQuery]:
         """
-        Retrieval user through user id
-        :param id: user id
-        :return: user or none
+        Retrieve a user by ID.
+
+        Args:
+            id (int): The user ID to retrieve.
+
+        Returns:
+            Optional[UserQuery]: The user query object if found, None otherwise.
         """
         user_do = await self.mapper.select_by_id(id=id)
-        if user_do:
-            return UserQuery(**user_do.model_dump())
-        else:
-            return None
+        return UserQuery(**user_do.model_dump()) if user_do else None
 
     async def login(self, loginCmd: LoginCmd) -> Token:
         """
-        Do log in
-        :param loginCmd: loginCmd
-        :return: access token and refresh token
+        Perform login and return an access token and refresh token.
+
+        Args:
+            loginCmd (LoginCmd): The login command containing username and password.
+
+        Returns:
+            Token: The access token and refresh token.
         """
         username: str = loginCmd.username
         userDO: UserDO = await self.mapper.get_user_by_username(username=username)
-        if not userDO or not await verify_password(loginCmd.password, userDO.password):
+        if userDO is None or not verify_password(loginCmd.password, userDO.password):
             raise SystemException(
-                SystemResponseCode.AUTH_FAILED.code, SystemResponseCode.AUTH_FAILED.msg
+                SystemResponseCode.AUTH_FAILED.code,
+                SystemResponseCode.AUTH_FAILED.msg,
+                status_code=http.HTTPStatus.UNAUTHORIZED,
             )
         access_token_expires = timedelta(minutes=configs.access_token_expire_minutes)
-        refresh_token_expires = timedelta(minutes=configs.refresh_token_expire_minutes)
         access_token = await security.create_token(
             subject=userDO.id,
             expires_delta=access_token_expires,
             token_type=TokenTypeEnum.access,
         )
         refresh_token = await security.create_token(
             subject=userDO.id,
-            expires_delta=refresh_token_expires,
             token_type=TokenTypeEnum.refresh,
         )
         token = Token(
             access_token=access_token,
             expired_at=int(access_token_expires.total_seconds()),
             token_type="bearer",
             refresh_token=refresh_token,
-            re_expired_at=int(refresh_token_expires.total_seconds()),
+            re_expired_at=int(
+                timedelta(minutes=configs.refresh_token_expire_minutes).total_seconds()
+            ),
         )
         cache_client: Cache = await get_cache_client()
         await cache_client.set(
             f"{SystemConstantCode.USER_KEY.msg}{userDO.id}",
             access_token,
             access_token_expires,
         )
         return token
 
     async def export_user_template(
         self,
     ) -> StreamingResponse:
         """
-        Export empty user import template
+        Export an empty user import template.
         """
         return await export_template(schema=UserExport, file_name="user_template")
 
     async def import_user(self, file: UploadFile):
         """
-        Import user data
+        Import user data from an Excel file.
+
+        Args:
+            file (UploadFile): The Excel file containing user data.
         """
         contents = await file.read()
         import_df = pd.read_excel(io.BytesIO(contents))
         user_datas: UserQuery = [
             user_data for user_data in import_df.to_dict(orient="records")
         ]
         user_import_list = []
+        user_name_list = []
         for user_data in user_datas:
             user_import = UserDO(**user_data)
             user_import.password = await get_password_hash(user_import.password)
             user_import_list.append(user_import)
+            user_name_list.append(user_import.username)
         await file.close()
+        user_list: List[UserDO] = await self.mapper.get_user_by_usernames(
+            usernames=user_name_list
+        )
+
+        if len(user_list) > 0:
+            err_msg = ""
+            for user in user_list:
+                err_msg += "," + str(user.username)
+            raise SystemException(
+                SystemResponseCode.USER_NAME_EXISTS.code,
+                SystemResponseCode.USER_NAME_EXISTS.msg + err_msg,
+            )
         await self.mapper.insert_batch(data_list=user_import_list)
 
     async def export_user(self, params: Params) -> StreamingResponse:
-        user_pages = await self.mapper.select_list_page_ordered(params=params)
+        """
+        Export user data to an Excel file.
+
+        Args:
+            params (Params): The query parameters for filtering users.
+
+        Returns:
+            StreamingResponse: The Excel file containing user data.
+        """
+        user_pages = await self.mapper.select_page(params=params)
         user_items = user_pages.__dict__["items"]
         user_data = []
         for user in user_items:
             user_data.append(UserQuery(**user.model_dump()))
         return await export_template(
             schema=UserQuery, file_name="user", data_list=user_data
         )
 
+    async def register(self, data: UserCreateCmd) -> UserDO:
+        """
+        Register a new user.
+
+        Args:
+            data (UserCreateCmd): The user creation command containing username and password.
+
+        Returns:
+            UserDO: The newly created user.
+        """
+        user: UserDO = await self.mapper.get_user_by_username(username=data.username)
+        if user is not None:
+            raise ServiceException(
+                SystemResponseCode.USER_NAME_EXISTS.code,
+                SystemResponseCode.USER_NAME_EXISTS.msg,
+            )
+        return await self.mapper.insert(data=data)
+
+    async def list_user(self, page: int, size: int) -> Optional[List[UserQuery]]:
+        """
+        List users with pagination.
+
+        Args:
+            page (int): The page number.
+            size (int): The page size.
+
+        Returns:
+            Optional[List[UserQuery]]: The list of users or None if no users are found.
+        """
+        results: List[UserDO] = await self.mapper.select_list(page=page, size=size)
+        return [UserQuery(**user.model_dump()) for user in results]
+
 
 def get_user_service() -> UserService:
+    """
+    Return an instance of the UserService implementation.
+
+    Returns:
+        UserService: An instance of the UserServiceImpl class.
+    """
     return UserServiceImpl(mapper=userMapper)
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/migrations/__pycache__/env.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
 files sz: 2714
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
@@ -162,34 +162,34 @@
                434 POP_TOP
    
     35     >>  436 LOAD_NAME               14 (SQLModel)
                438 LOAD_ATTR               31 (metadata)
                448 STORE_NAME              32 (target_metadata)
    
     44         450 LOAD_CONST              16 (('return', None))
-               452 LOAD_CONST              11 (<code object run_migrations_offline, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\env.py", line 44>)
+               452 LOAD_CONST              11 (<code object run_migrations_offline, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\env.py", line 44>)
                454 MAKE_FUNCTION            4 (annotations)
                456 STORE_NAME              33 (run_migrations_offline)
    
     68         458 LOAD_CONST              12 ('connection')
                460 LOAD_NAME               10 (Connection)
                462 LOAD_CONST              10 ('return')
                464 LOAD_CONST               1 (None)
                466 BUILD_TUPLE              4
-               468 LOAD_CONST              13 (<code object do_run_migrations, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\env.py", line 68>)
+               468 LOAD_CONST              13 (<code object do_run_migrations, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\env.py", line 68>)
                470 MAKE_FUNCTION            4 (annotations)
                472 STORE_NAME              34 (do_run_migrations)
    
     75         474 LOAD_CONST              16 (('return', None))
-               476 LOAD_CONST              14 (<code object run_async_migrations, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\env.py", line 75>)
+               476 LOAD_CONST              14 (<code object run_async_migrations, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\env.py", line 75>)
                478 MAKE_FUNCTION            4 (annotations)
                480 STORE_NAME              35 (run_async_migrations)
    
     93         482 LOAD_CONST              16 (('return', None))
-               484 LOAD_CONST              15 (<code object run_migrations_online, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\env.py", line 93>)
+               484 LOAD_CONST              15 (<code object run_migrations_online, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\env.py", line 93>)
                486 MAKE_FUNCTION            4 (annotations)
                488 STORE_NAME              36 (run_migrations_online)
    
     99         490 PUSH_NULL
                492 LOAD_NAME               16 (context)
                494 LOAD_ATTR               37 (is_offline_mode)
                504 PRECALL                  0
@@ -311,15 +311,15 @@
             'named'
             ('url', 'target_metadata', 'literal_binds', 'dialect_opts')
             None
          names      ('config', 'get_main_option', 'context', 'configure', 'target_metadata', 'begin_transaction', 'run_migrations')
          varnames   ('url',)
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\env.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\env.py'
          name       'run_migrations_offline'
          firstlineno 44
          lnotab 0x020c3401160102010c01020106fc1207280126ff
       'connection'
       code
          argcount  : 1
          nlocals   : 1
@@ -385,15 +385,15 @@
          consts
             None
             ('connection', 'target_metadata')
          names      ('context', 'configure', 'target_metadata', 'begin_transaction', 'run_migrations')
          varnames   ('connection',)
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\env.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\env.py'
          name       'do_run_migrations'
          firstlineno 68
          lnotab 0x02013602280126ff
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 6
@@ -515,15 +515,15 @@
             'sqlalchemy.'
             ('prefix', 'poolclass')
             None
          names      ('async_engine_from_config', 'config', 'get_section', 'config_ini_section', 'pool', 'NullPool', 'connect', 'run_sync', 'do_run_migrations', 'dispose')
          varnames   ('connectable', 'connection')
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\env.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\env.py'
          name       'run_async_migrations'
          firstlineno 75
          lnotab 0x06060c014801020116fd1206360140ff4603
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -547,22 +547,22 @@
          consts
             "Run migrations in 'online' mode."
             None
          names      ('asyncio', 'run', 'run_async_migrations')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\env.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\env.py'
          name       'run_migrations_online'
          firstlineno 93
          lnotab 0x0203
       ('return', None)
    names      ('os', 'sys', 'pathlib', 'Path', 'asyncio', 'logging.config', 'fileConfig', 'sqlalchemy', 'pool', 'sqlalchemy.engine', 'Connection', 'sqlalchemy.ext.asyncio', 'async_engine_from_config', 'sqlmodel', 'SQLModel', 'alembic', 'context', 'path', 'dirname', 'abspath', '__file__', 'current_dir', 'str', 'parent', 'project_dir', 'insert', 'fss.starter.system.model.migrate', 'start_signal', 'print', 'config', 'config_file_name', 'metadata', 'target_metadata', 'run_migrations_offline', 'do_run_migrations', 'run_async_migrations', 'run_migrations_online', 'is_offline_mode')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\env.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\env.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c0108010c020c010c010c010c020c0276013c0136
       020c0216040e040e0120060e0908181007081208061e011802
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/env.py` & `fastapi_sqlmodel_starter-1.0.1/fss/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/script.py.mako` & `fastapi_sqlmodel_starter-1.0.1/fss/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/947dad7dbfdb_init_project.py` & `fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/947dad7dbfdb_init_project.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.1/fss/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
+moddate:  0x2a322166 (Thu Apr 18 14:46:02 2024 UTC)
 files sz: 1516
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -34,19 +34,19 @@
    
     16          34 LOAD_CONST               3 (None)
                 36 STORE_NAME               7 (branch_labels)
    
     17          38 LOAD_CONST               3 (None)
                 40 STORE_NAME               8 (depends_on)
    
-    20          42 LOAD_CONST               5 (<code object upgrade, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\versions\947dad7dbfdb_init_project.py", line 20>)
+    20          42 LOAD_CONST               5 (<code object upgrade, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\versions\947dad7dbfdb_init_project.py", line 20>)
                 44 MAKE_FUNCTION            0
                 46 STORE_NAME               9 (upgrade)
    
-    41          48 LOAD_CONST               6 (<code object downgrade, file "E:\user\train\production\fastapi-sqlmodel-starter\src\migrations\versions\947dad7dbfdb_init_project.py", line 41>)
+    41          48 LOAD_CONST               6 (<code object downgrade, file "E:\user\train\production\fastapi-sqlmodel-starter\fss\migrations\versions\947dad7dbfdb_init_project.py", line 41>)
                 50 MAKE_FUNCTION            0
                 52 STORE_NAME              10 (downgrade)
                 54 LOAD_CONST               3 (None)
                 56 RETURN_VALUE
    consts
       'init project\n\nRevision ID: 947dad7dbfdb\nRevises:\nCreate Date: 2024-04-02 14:28:52.629148\n\n'
       0
@@ -244,15 +244,15 @@
             'ix_system_user_id'
             ('unique',)
             'ix_system_user_username'
          names      ('op', 'create_table', 'sa', 'Column', 'BigInteger', 'String', 'DateTime', 'PrimaryKeyConstraint', 'create_index', 'f')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\versions\\947dad7dbfdb_init_project.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\versions\\947dad7dbfdb_init_project.py'
          name       'upgrade'
          firstlineno 20
          lnotab
             0x0203160102014e015401540154014e014e01260102f7120b560116012e
             ff
       code
          argcount  : 0
@@ -309,19 +309,19 @@
             'system_user'
             ('table_name',)
             'ix_system_user_id'
          names      ('op', 'drop_index', 'f', 'drop_table')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\versions\\947dad7dbfdb_init_project.py'
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\versions\\947dad7dbfdb_init_project.py'
          name       'downgrade'
          firstlineno 41
          lnotab 0x020250015001
    names      ('__doc__', 'alembic', 'op', 'sqlalchemy', 'sa', 'revision', 'down_revision', 'branch_labels', 'depends_on', 'upgrade', 'downgrade')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\migrations\\versions\\947dad7dbfdb_init_project.py'
+   filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\fss\\migrations\\versions\\947dad7dbfdb_init_project.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104080c01080404010401040104030615
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b1/PKG-INFO` & `fastapi_sqlmodel_starter-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sqlmodel-starter
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Fss aims to be one of top scaffold in PyWeb.
 Home-page: https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 License: MIT
 Keywords: fastapi,sqlmodel,tools,web,scaffold
 Author: tyvekZhang
 Author-email: tyvekzhang@gmail.com
 Maintainer: tyvekZhang
@@ -36,28 +36,29 @@
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: redis[hiredis] (>=5.0.3,<6.0.0)
+Requires-Dist: slowapi (>=0.1.9,<0.2.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: Documentation, https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki
 Project-URL: Repository, https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 Description-Content-Type: text/markdown
 
 <div  align="center" style="margin-top: 3%">
    <h1>
-     FastAPI Sqlmodel Starter (Fss)
+     FastAPI SQLModel Starter (Fss)
    </h1>
    <p>
-     <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/logo.png" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
+     <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/source/_static/img/fss.svg" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
    </p>
    <p>
      <img alt="GitHub License" src="https://img.shields.io/github/license/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fastapi-sqlmodel-starter">
      <img alt="CI" src="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/actions/workflows/ci.yaml/badge.svg">
      <img alt="Codecov" src="https://img.shields.io/codecov/c/github/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="Read the Docs" src="https://img.shields.io/readthedocs/fastapi-sqlmodel-starter">
@@ -72,24 +73,40 @@
     PyWeb领域最好用的脚手架之一。
    </h3>
 </div>
 
 
 ## 特性
 
-- 开箱即用, 内置常见数据库、缓存([默认]Sqlite, PostgreSQL, MySQL, [默认]文件缓存, Redis)
-- 自带单表的几乎所有操作
-- 数据库迁移, 静态代码扫描, 接口文档等一众特性
+- ⚡ 开箱即用, 实现中间件的零依赖
+   - 默认使用Sqlite, 也可自由切换PostgreSQL、MySQL数据库
+   - 可选文件或Redis缓存
+- 🚢 开启Python代码操作数据库的新体验
+- 🚀 简化ORM操作, 内置单表常见操作
+- 🎨 丰富的插件机制
+   - Jwt安全认证
+   - 访问限流
+   - Ip黑名单
+- 🐋 完备的容器化解决方案
+  - Docker
+  - Docker-compose
+  - Kubernetes
+- ✅ 基于GitHub Actions的CI (持续集成) 和 CD (持续交付)
+
+## 文档
+- 交互式API文档
+  <img alt="API doc"  src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/api_doc.png">
+- 在线文档: [Read the docs](https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/)
 
 ## 快速开始
-1. 首先确保python的版本是3.9及以上的
+1. 首先确保python版本为3.9及以上
 2. 克隆代码
 ```shell
 git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter
-cd fastapi-sqlmodel-starter/src
+cd fastapi-sqlmodel-starter/fss
 ```
 3. [可选]创建虚拟环境, 本篇以venv为例, 类似的工具还有conda, virtualenv等
 ```shell
 python3 -m venv .env_fss
 ```
 4. [可选]激活虚拟环境
     - Windows: .env_fss\Scripts\activate
@@ -100,25 +117,24 @@
 poetry install
 ```
 6. 数据库迁移
 ```shell
 alembic upgrade head
 ```
 7. 启动
-   - Windows: python3 fss\apiserver.py
-   - macOS 或 Linux: python3 fss/apiserver.py
+   - Windows: python3 apiserver.py
+   - macOS 或 Linux: python3 apiserver.py
 8. 访问: http://127.0.0.1:9010/docs
-9. 首先通过注册接口新建用户, 接着进行认证, 一切Ok.
-## 文档
-- https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/
+> 成功访问后需要创建用户并认证
+
 ## 贡献
 
 欢迎为 FastapiSqlmodelStarter 做出贡献！你可以通过以下方式参与：
 
-- 提交 Bug 或功能需求到 [Issue 追踪器](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
+- 提交 Bug 或功能需求到 [Issue清单](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
 - 提交代码改进的 Pull Request
 - 编写和改进文档
 - 分享你使用 FastapiSqlmodelStarter 的经验和想法
 
 ## 许可证
 
 FastapiSqlmodelStarter 采用 [MIT 许可证](https://opensource.org/licenses/MIT)开源。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-sqlmodel-starter Version: 1.0.0b1 Summary:
+Metadata-Version: 2.1 Name: fastapi-sqlmodel-starter Version: 1.0.1 Summary:
 Fss aims to be one of top scaffold in PyWeb. Home-page: https://github.com/
 tyvekzhang/fastapi-sqlmodel-starter License: MIT Keywords:
 fastapi,sqlmodel,tools,web,scaffold Author: tyvekZhang Author-email:
 tyvekzhang@gmail.com Maintainer: tyvekZhang Maintainer-email:
 tyvekzhang@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -18,41 +18,46 @@
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: fastapi-async-
 sqlalchemy (>=0.6.1,<0.7.0) Requires-Dist: fastapi-offline (>=1.7.1,<2.0.0)
 Requires-Dist: fastapi-pagination (>=0.12.21,<0.13.0) Requires-Dist: loguru
 (>=0.7.2,<0.8.0) Requires-Dist: openpyxl (>=3.1.2,<4.0.0) Requires-Dist: pandas
 (>=2.2.2,<3.0.0) Requires-Dist: passlib (>=1.7.4,<2.0.0) Requires-Dist: python-
 dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-jose[cryptography]
 (>=3.3.0,<4.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-
-Dist: redis[hiredis] (>=5.0.3,<6.0.0) Requires-Dist: sqlalchemy-utils
-(>=0.41.2,<0.42.0) Requires-Dist: sqlmodel (>=0.0.16,<0.0.17) Requires-Dist:
-uvicorn (>=0.29.0,<0.30.0) Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0) Project-
-URL: Documentation, https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki
-Project-URL: Repository, https://github.com/tyvekzhang/fastapi-sqlmodel-starter
-Description-Content-Type: text/markdown
-                 ************ FFaassttAAPPII SSqqllmmooddeell SSttaarrtteerr ((FFssss)) ************
+Dist: redis[hiredis] (>=5.0.3,<6.0.0) Requires-Dist: slowapi (>=0.1.9,<0.2.0)
+Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0) Requires-Dist: sqlmodel
+(>=0.0.16,<0.0.17) Requires-Dist: uvicorn (>=0.29.0,<0.30.0) Requires-Dist:
+xlsxwriter (>=3.2.0,<4.0.0) Project-URL: Documentation, https://github.com/
+tyvekzhang/fastapi-sqlmodel-starter/wiki Project-URL: Repository, https://
+github.com/tyvekzhang/fastapi-sqlmodel-starter Description-Content-Type: text/
+markdown
+                 ************ FFaassttAAPPII SSQQLLMMooddeell SSttaarrtteerr ((FFssss)) ************
                                     [logo]
       [GitHub License][PyPI - Python Version][CI][Codecov][Read the Docs]
                         ****** ?ç?®??ä?½??ä?¸?­?æ?? || _EE_nn_gg_ll_ii_ss_hh ******
               ******** PPyyWWeebb?é?¢??å???æ???å?¥?½?ç??¨?ç???è???æ???æ??¶?ä?¹??ä?¸??ã?? ********
-## ç¹æ§ - å¼ç®±å³ç¨, åç½®å¸¸è§æ°æ®åºãç¼å­([é»è®¤]Sqlite,
-PostgreSQL, MySQL, [é»è®¤]æä»¶ç¼å­, Redis) -
-èªå¸¦åè¡¨çå ä¹æææä½ - æ°æ®åºè¿ç§», éæä»£ç æ«æ,
-æ¥å£ææ¡£ç­ä¸ä¼ç¹æ§ ## å¿«éå¼å§ 1.
-é¦åç¡®ä¿pythonççæ¬æ¯3.9åä»¥ä¸ç 2. åéä»£ç  ```shell git
-clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd fastapi-
-sqlmodel-starter/src ``` 3. [å¯é]åå»ºèæç¯å¢, æ¬ç¯ä»¥venvä¸ºä¾,
-ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3 -m venv .env_fss ```
-4. [å¯é]æ¿æ´»èæç¯å¢ - Windows: .env_fss\Scripts\activate - macOS æ
-Linux: source .env_fss/bin/activate 5. å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell
-pip install poetry --trusted-host=mirrors.tuna.tsinghua.edu.cn --index-
-url=https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
+## ç¹æ§ - â¡ å¼ç®±å³ç¨, å®ç°ä¸­é´ä»¶çé¶ä¾èµ - é»è®¤ä½¿ç¨Sqlite,
+ä¹å¯èªç±åæ¢PostgreSQLãMySQLæ°æ®åº - å¯éæä»¶æRedisç¼å­ -
+ð¢ å¼å¯Pythonä»£ç æä½æ°æ®åºçæ°ä½éª - ð ç®åORMæä½,
+åç½®åè¡¨å¸¸è§æä½ - ð¨ ä¸°å¯çæä»¶æºå¶ - Jwtå®å¨è®¤è¯ -
+è®¿é®éæµ - Ipé»åå - ð å®å¤çå®¹å¨åè§£å³æ¹æ¡ - Docker -
+Docker-compose - Kubernetes - â åºäºGitHub ActionsçCI (æç»­éæ) å
+CD (æç»­äº¤ä») ## ææ¡£ - äº¤äºå¼APIææ¡£ [API doc]- å¨çº¿ææ¡£: [Read
+the docs](https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/) ##
+å¿«éå¼å§ 1. é¦åç¡®ä¿pythonçæ¬ä¸º3.9åä»¥ä¸ 2. åéä»£ç 
+```shell git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd
+fastapi-sqlmodel-starter/fss ``` 3. [å¯é]åå»ºèæç¯å¢,
+æ¬ç¯ä»¥venvä¸ºä¾, ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3
+-m venv .env_fss ``` 4. [å¯é]æ¿æ´»èæç¯å¢ - Windows:
+.env_fss\Scripts\activate - macOS æ Linux: source .env_fss/bin/activate 5.
+å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell pip install poetry --trusted-
+host=mirrors.tuna.tsinghua.edu.cn --index-url=https://
+mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
 æ°æ®åºè¿ç§» ```shell alembic upgrade head ``` 7. å¯å¨ - Windows: python3
-fss\apiserver.py - macOS æ Linux: python3 fss/apiserver.py 8. è®¿é®: http://
-127.0.0.1:9010/docs 9. é¦åéè¿æ³¨åæ¥å£æ°å»ºç¨æ·,
-æ¥çè¿è¡è®¤è¯, ä¸åOk. ## ææ¡£ - https://fastapi-sqlmodel-
-starter.readthedocs.io/en/latest/ ## è´¡ç® æ¬¢è¿ä¸º FastapiSqlmodelStarter
+apiserver.py - macOS æ Linux: python3 apiserver.py 8. è®¿é®: http://
+127.0.0.1:9010/docs > æåè®¿é®åéè¦åå»ºç¨æ·å¹¶è®¤è¯ ## è´¡ç®
+æ¬¢è¿ä¸º FastapiSqlmodelStarter
 ååºè´¡ç®ï¼ä½ å¯ä»¥éè¿ä»¥ä¸æ¹å¼åä¸ï¼ - æäº¤ Bug
-æåè½éæ±å° [Issue è¿½è¸ªå¨](https://github.com/tyvekzhang/fastapi-
+æåè½éæ±å° [Issueæ¸å](https://github.com/tyvekzhang/fastapi-
 sqlmodel-starter/issues) - æäº¤ä»£ç æ¹è¿ç Pull Request -
 ç¼ååæ¹è¿ææ¡£ - åäº«ä½ ä½¿ç¨ FastapiSqlmodelStarter
 çç»éªåæ³æ³ ## è®¸å¯è¯ FastapiSqlmodelStarter éç¨ [MIT è®¸å¯è¯]
 (https://opensource.org/licenses/MIT)å¼æºã
```

