# Comparing `tmp/taskiq_redis-0.5.5.tar.gz` & `tmp/taskiq_redis-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_redis-0.5.5.tar", max compression
+gzip compressed data, was "taskiq_redis-0.5.6.tar", max compression
```

## Comparing `taskiq_redis-0.5.5.tar` & `taskiq_redis-0.5.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2712 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/README.md
--rw-r--r--   0        0        0     3664 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      602 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/__init__.py
--rw-r--r--   0        0        0      561 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/py.typed
--rw-r--r--   0        0        0     8357 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/redis_backend.py
--rw-r--r--   0        0        0     3957 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/redis_broker.py
--rw-r--r--   0        0        0     2121 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/redis_cluster_broker.py
--rw-r--r--   0        0        0     6166 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/schedule_source.py
--rw-r--r--   0        0        0      416 2023-12-12 09:46:25.589141 taskiq_redis-0.5.5/taskiq_redis/serializer.py
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 taskiq_redis-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     3154 2024-04-19 22:24:22.021491 taskiq_redis-0.5.6/README.md
+-rw-r--r--   0        0        0     3664 2024-04-19 22:24:22.021491 taskiq_redis-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      602 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/__init__.py
+-rw-r--r--   0        0        0      561 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/py.typed
+-rw-r--r--   0        0        0     8914 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/redis_backend.py
+-rw-r--r--   0        0        0     4254 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/redis_broker.py
+-rw-r--r--   0        0        0     2121 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/redis_cluster_broker.py
+-rw-r--r--   0        0        0     6202 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/schedule_source.py
+-rw-r--r--   0        0        0      416 2024-04-19 22:24:22.025492 taskiq_redis-0.5.6/taskiq_redis/serializer.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 taskiq_redis-0.5.6/PKG-INFO
```

### Comparing `taskiq_redis-0.5.5/README.md` & `taskiq_redis-0.5.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -67,22 +67,28 @@
 
 Brokers parameters:
 * `url` - url to redis.
 * `task_id_generator` - custom task_id genertaor.
 * `result_backend` - custom result backend.
 * `queue_name` - name of the pub/sub channel in redis.
 * `max_connection_pool_size` - maximum number of connections in pool.
+* Any other keyword arguments are passed to `redis.asyncio.BlockingConnectionPool`.
+  Notably, you can use `timeout` to set custom timeout in seconds for reconnects
+  (or set it to `None` to try reconnects indefinitely).
 
 ## RedisAsyncResultBackend configuration
 
 RedisAsyncResultBackend parameters:
 * `redis_url` - url to redis.
 * `keep_results` - flag to not remove results from Redis after reading.
 * `result_ex_time` - expire time in seconds (by default - not specified)
 * `result_px_time` - expire time in milliseconds (by default - not specified)
+* Any other keyword arguments are passed to `redis.asyncio.BlockingConnectionPool`.
+  Notably, you can use `timeout` to set custom timeout in seconds for reconnects
+  (or set it to `None` to try reconnects indefinitely).
 > IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**
 > If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.
 >```python
 ># First variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_ex_time=1000,
```

### Comparing `taskiq_redis-0.5.5/pyproject.toml` & `taskiq_redis-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-redis"
-version = "0.5.5"
+version = "0.5.6"
 description = "Redis integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_redis-0.5.5/taskiq_redis/__init__.py` & `taskiq_redis-0.5.6/taskiq_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.5.5/taskiq_redis/exceptions.py` & `taskiq_redis-0.5.6/taskiq_redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.5.5/taskiq_redis/redis_backend.py` & `taskiq_redis-0.5.6/taskiq_redis/redis_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle
-from typing import Dict, Optional, TypeVar, Union
+from typing import Any, Dict, Optional, TypeVar, Union
 
-from redis.asyncio import ConnectionPool, Redis
+from redis.asyncio import BlockingConnectionPool, Redis
 from redis.asyncio.cluster import RedisCluster
 from taskiq import AsyncResultBackend
 from taskiq.abc.result_backend import TaskiqResult
 
 from taskiq_redis.exceptions import (
     DuplicateExpireTimeSelectedError,
     ExpireTimeMustBeMoreThanZeroError,
@@ -20,29 +20,37 @@
 
     def __init__(
         self,
         redis_url: str,
         keep_results: bool = True,
         result_ex_time: Optional[int] = None,
         result_px_time: Optional[int] = None,
+        max_connection_pool_size: Optional[int] = None,
+        **connection_kwargs: Any,
     ) -> None:
         """
         Constructs a new result backend.
 
         :param redis_url: url to redis.
         :param keep_results: flag to not remove results from Redis after reading.
         :param result_ex_time: expire time in seconds for result.
         :param result_px_time: expire time in milliseconds for result.
+        :param max_connection_pool_size: maximum number of connections in pool.
+        :param connection_kwargs: additional arguments for redis BlockingConnectionPool.
 
         :raises DuplicateExpireTimeSelectedError: if result_ex_time
             and result_px_time are selected.
         :raises ExpireTimeMustBeMoreThanZeroError: if result_ex_time
             and result_px_time are equal zero.
         """
-        self.redis_pool = ConnectionPool.from_url(redis_url)
+        self.redis_pool = BlockingConnectionPool.from_url(
+            url=redis_url,
+            max_connections=max_connection_pool_size,
+            **connection_kwargs,
+        )
         self.keep_results = keep_results
         self.result_ex_time = result_ex_time
         self.result_px_time = result_px_time
 
         unavailable_conditions = any(
             (
                 self.result_ex_time is not None and self.result_ex_time <= 0,
@@ -142,29 +150,34 @@
 
     def __init__(
         self,
         redis_url: str,
         keep_results: bool = True,
         result_ex_time: Optional[int] = None,
         result_px_time: Optional[int] = None,
+        **connection_kwargs: Any,
     ) -> None:
         """
         Constructs a new result backend.
 
         :param redis_url: url to redis cluster.
         :param keep_results: flag to not remove results from Redis after reading.
         :param result_ex_time: expire time in seconds for result.
         :param result_px_time: expire time in milliseconds for result.
+        :param connection_kwargs: additional arguments for RedisCluster.
 
         :raises DuplicateExpireTimeSelectedError: if result_ex_time
             and result_px_time are selected.
         :raises ExpireTimeMustBeMoreThanZeroError: if result_ex_time
             and result_px_time are equal zero.
         """
-        self.redis: RedisCluster[bytes] = RedisCluster.from_url(redis_url)
+        self.redis: RedisCluster[bytes] = RedisCluster.from_url(
+            redis_url,
+            **connection_kwargs,
+        )
         self.keep_results = keep_results
         self.result_ex_time = result_ex_time
         self.result_px_time = result_px_time
 
         unavailable_conditions = any(
             (
                 self.result_ex_time is not None and self.result_ex_time <= 0,
```

### Comparing `taskiq_redis-0.5.5/taskiq_redis/redis_broker.py` & `taskiq_redis-0.5.6/taskiq_redis/redis_broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from logging import getLogger
 from typing import Any, AsyncGenerator, Callable, Optional, TypeVar
 
-from redis.asyncio import ConnectionPool, Redis
+from redis.asyncio import BlockingConnectionPool, ConnectionPool, Redis
 from taskiq.abc.broker import AsyncBroker
 from taskiq.abc.result_backend import AsyncResultBackend
 from taskiq.message import BrokerMessage
 
 _T = TypeVar("_T")
 
 logger = getLogger("taskiq.redis_broker")
@@ -27,22 +27,24 @@
         Constructs a new broker.
 
         :param url: url to redis.
         :param task_id_generator: custom task_id generator.
         :param result_backend: custom result backend.
         :param queue_name: name for a list in redis.
         :param max_connection_pool_size: maximum number of connections in pool.
-        :param connection_kwargs: additional arguments for aio-redis ConnectionPool.
+            Each worker opens its own connection. Therefore this value has to be
+            at least number of workers + 1.
+        :param connection_kwargs: additional arguments for redis BlockingConnectionPool.
         """
         super().__init__(
             result_backend=result_backend,
             task_id_generator=task_id_generator,
         )
 
-        self.connection_pool: ConnectionPool = ConnectionPool.from_url(
+        self.connection_pool: ConnectionPool = BlockingConnectionPool.from_url(
             url=url,
             max_connections=max_connection_pool_size,
             **connection_kwargs,
         )
         self.queue_name = queue_name
 
     async def shutdown(self) -> None:
@@ -56,16 +58,17 @@
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Publish message over PUBSUB channel.
 
         :param message: message to send.
         """
+        queue_name = message.labels.get("queue_name") or self.queue_name
         async with Redis(connection_pool=self.connection_pool) as redis_conn:
-            await redis_conn.publish(self.queue_name, message.message)
+            await redis_conn.publish(queue_name, message.message)
 
     async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Listen redis queue for new messages.
 
         This function listens to the pubsub channel
         and yields all messages with proper types.
@@ -91,16 +94,17 @@
         """
         Put a message in a list.
 
         This method appends a message to the list of all messages.
 
         :param message: message to append.
         """
+        queue_name = message.labels.get("queue_name") or self.queue_name
         async with Redis(connection_pool=self.connection_pool) as redis_conn:
-            await redis_conn.lpush(self.queue_name, message.message)
+            await redis_conn.lpush(queue_name, message.message)
 
     async def listen(self) -> AsyncGenerator[bytes, None]:
         """
         Listen redis queue for new messages.
 
         This function listens to the queue
         and yields new messages if they have BrokerMessage type.
```

### Comparing `taskiq_redis-0.5.5/taskiq_redis/redis_cluster_broker.py` & `taskiq_redis-0.5.6/taskiq_redis/redis_cluster_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.5.5/taskiq_redis/schedule_source.py` & `taskiq_redis-0.5.6/taskiq_redis/schedule_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List, Optional
 
-from redis.asyncio import ConnectionPool, Redis, RedisCluster
+from redis.asyncio import BlockingConnectionPool, ConnectionPool, Redis, RedisCluster
 from taskiq import ScheduleSource
 from taskiq.abc.serializer import TaskiqSerializer
 from taskiq.compat import model_dump, model_validate
 from taskiq.scheduler.scheduled_task import ScheduledTask
 
 from taskiq_redis.serializer import PickleSerializer
 
@@ -18,28 +18,28 @@
 
     :param url: url to redis.
     :param prefix: prefix for redis schedule keys.
     :param buffer_size: buffer size for redis scan.
         This is how many keys will be fetched at once.
     :param max_connection_pool_size: maximum number of connections in pool.
     :param serializer: serializer for data.
-    :param connection_kwargs: additional arguments for aio-redis ConnectionPool.
+    :param connection_kwargs: additional arguments for redis BlockingConnectionPool.
     """
 
     def __init__(
         self,
         url: str,
         prefix: str = "schedule",
         buffer_size: int = 50,
         max_connection_pool_size: Optional[int] = None,
         serializer: Optional[TaskiqSerializer] = None,
         **connection_kwargs: Any,
     ) -> None:
         self.prefix = prefix
-        self.connection_pool: ConnectionPool = ConnectionPool.from_url(
+        self.connection_pool: ConnectionPool = BlockingConnectionPool.from_url(
             url=url,
             max_connections=max_connection_pool_size,
             **connection_kwargs,
         )
         self.buffer_size = buffer_size
         if serializer is None:
             serializer = PickleSerializer()
```

### Comparing `taskiq_redis-0.5.5/PKG-INFO` & `taskiq_redis-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-redis
-Version: 0.5.5
+Version: 0.5.6
 Summary: Redis integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-redis
 Keywords: taskiq,tasks,distributed,async,redis,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python
@@ -89,22 +89,28 @@
 
 Brokers parameters:
 * `url` - url to redis.
 * `task_id_generator` - custom task_id genertaor.
 * `result_backend` - custom result backend.
 * `queue_name` - name of the pub/sub channel in redis.
 * `max_connection_pool_size` - maximum number of connections in pool.
+* Any other keyword arguments are passed to `redis.asyncio.BlockingConnectionPool`.
+  Notably, you can use `timeout` to set custom timeout in seconds for reconnects
+  (or set it to `None` to try reconnects indefinitely).
 
 ## RedisAsyncResultBackend configuration
 
 RedisAsyncResultBackend parameters:
 * `redis_url` - url to redis.
 * `keep_results` - flag to not remove results from Redis after reading.
 * `result_ex_time` - expire time in seconds (by default - not specified)
 * `result_px_time` - expire time in milliseconds (by default - not specified)
+* Any other keyword arguments are passed to `redis.asyncio.BlockingConnectionPool`.
+  Notably, you can use `timeout` to set custom timeout in seconds for reconnects
+  (or set it to `None` to try reconnects indefinitely).
 > IMPORTANT: **It is highly recommended to use expire time ​​in RedisAsyncResultBackend**
 > If you want to add expiration, either `result_ex_time` or `result_px_time` must be set.
 >```python
 ># First variant
 >redis_async_result = RedisAsyncResultBackend(
 >    redis_url="redis://localhost:6379",
 >    result_ex_time=1000,
```

