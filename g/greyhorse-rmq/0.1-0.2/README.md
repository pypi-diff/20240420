# Comparing `tmp/greyhorse_rmq-0.1.tar.gz` & `tmp/greyhorse_rmq-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_rmq-0.1.tar", max compression
+gzip compressed data, was "greyhorse_rmq-0.2.tar", max compression
```

## Comparing `greyhorse_rmq-0.1.tar` & `greyhorse_rmq-0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       96 2023-06-28 19:10:16.050500 greyhorse_rmq-0.1/greyhorse_rmq/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-28 20:12:59.255128 greyhorse_rmq-0.1/greyhorse_rmq/config.py
--rw-r--r--   0        0        0     3131 2023-06-28 19:15:42.876048 greyhorse_rmq-0.1/greyhorse_rmq/containers.py
--rw-r--r--   0        0        0     1523 2023-06-28 20:12:59.151131 greyhorse_rmq-0.1/greyhorse_rmq/contexts.py
--rw-r--r--   0        0        0     2539 2023-06-28 20:12:59.351125 greyhorse_rmq-0.1/greyhorse_rmq/engine.py
--rw-r--r--   0        0        0     1298 2023-06-28 16:56:50.912415 greyhorse_rmq-0.1/greyhorse_rmq/factory.py
--rw-r--r--   0        0        0     2973 2023-06-28 18:13:31.060356 greyhorse_rmq-0.1/greyhorse_rmq/resources.py
--rw-r--r--   0        0        0        0 2023-06-28 16:58:50.832666 greyhorse_rmq-0.1/greyhorse_rmq/rpc/__init__.py
--rw-r--r--   0        0        0     2943 2023-06-28 20:12:59.203130 greyhorse_rmq-0.1/greyhorse_rmq/rpc/client.py
--rw-r--r--   0        0        0     1706 2023-06-28 20:12:59.303126 greyhorse_rmq-0.1/greyhorse_rmq/rpc/server.py
--rw-r--r--   0        0        0      472 2023-06-28 16:29:49.139185 greyhorse_rmq-0.1/greyhorse_rmq/translations.toml
--rw-r--r--   0        0        0     1063 2023-06-28 20:05:06.850870 greyhorse_rmq-0.1/pyproject.toml
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 greyhorse_rmq-0.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-20 14:00:38.992739 greyhorse_rmq-0.2/greyhorse_rmq/__init__.py
+-rw-r--r--   0        0        0     1568 2024-04-20 14:19:27.684104 greyhorse_rmq-0.2/greyhorse_rmq/config.py
+-rw-r--r--   0        0        0      313 2024-04-20 14:19:27.700103 greyhorse_rmq-0.2/greyhorse_rmq/contexts.py
+-rw-r--r--   0        0        0     3031 2024-04-20 14:42:08.267890 greyhorse_rmq-0.2/greyhorse_rmq/engine.py
+-rw-r--r--   0        0        0      702 2024-04-20 14:19:27.668104 greyhorse_rmq-0.2/greyhorse_rmq/factory.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:44:32.190021 greyhorse_rmq-0.2/greyhorse_rmq/rpc/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-20 14:57:01.182999 greyhorse_rmq-0.2/greyhorse_rmq/rpc/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4965 2024-04-20 14:57:01.182999 greyhorse_rmq-0.2/greyhorse_rmq/rpc/__pycache__/client.cpython-312.pyc
+-rw-r--r--   0        0        0     4219 2024-04-20 15:17:32.605254 greyhorse_rmq-0.2/greyhorse_rmq/rpc/__pycache__/server.cpython-312.pyc
+-rw-r--r--   0        0        0     2921 2024-04-20 14:46:33.877299 greyhorse_rmq-0.2/greyhorse_rmq/rpc/client.py
+-rw-r--r--   0        0        0     2099 2024-04-20 15:17:26.553349 greyhorse_rmq-0.2/greyhorse_rmq/rpc/server.py
+-rw-r--r--   0        0        0     2335 2024-04-20 14:40:03.581296 greyhorse_rmq-0.2/greyhorse_rmq/service.py
+-rw-r--r--   0        0        0      472 2023-07-06 22:04:25.000000 greyhorse_rmq-0.2/greyhorse_rmq/translations.toml
+-rw-r--r--   0        0        0     1200 2024-04-20 13:58:59.131749 greyhorse_rmq-0.2/pyproject.toml
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 greyhorse_rmq-0.2/PKG-INFO
```

### Comparing `greyhorse_rmq-0.1/greyhorse_rmq/config.py` & `greyhorse_rmq-0.2/greyhorse_rmq/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 
-from pydantic import AmqpDsn, BaseSettings, validator
+from pydantic import BaseModel, Field, field_validator
+from pydantic.networks import AmqpDsn
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
-@dataclass
-class EngineConfig:
-    dsn: str
+class EngineConf(BaseModel):
+    dsn: AmqpDsn
+    virtualhost: str = '/'
+    timeout_seconds: int = 5
+    pool_max_connections: int = Field(default=4, gt=0)
+    pool_max_channels_per_connection: int = Field(default=100, gt=0)
+
+
+class RmqSettings(BaseSettings):
+    host: str = 'localhost'
+    port: int = 9200
+    user: str = 'elastic'
+    password: str = 'elastic'
+    password_file: Path | None = None
     virtualhost: str = '/'
     timeout_seconds: int = 5
     pool_max_connections: int = 4
     pool_max_channels_per_connection: int = 100
 
+    dsn: AmqpDsn | None = None
 
-class RmqSettings(BaseSettings):
-    RMQ_HOST: str = 'localhost'
-    RMQ_PORT: int = 5672
-    RMQ_USER: str = 'guest'
-    RMQ_PASSWORD: str = 'guest'
-    RMQ_PASSWORD_FILE: Path | None = None
-    RMQ_VIRTUALHOST: str = '/'
-    RMQ_TIMEOUT_SECONDS: int = 5
-    RMQ_POOL_MAX_CONNECTIONS: int = 4
-    RMQ_POOL_MAX_CHANNELS_PER_CONNECTION: int = 100
-
-    RMQ_URI: AmqpDsn | None = None
-
-    @validator('RMQ_URI', pre=True)
-    def assemble_dsn(cls, v: str | None, values: dict[str, Any]) -> str:
-        if isinstance(v, str):
+    model_config = SettingsConfigDict(env_file='.env', case_sensitive=False, env_prefix='rmq_')
+
+    @classmethod
+    @field_validator('dsn', mode='before')
+    def assemble_dsn(cls, v: AmqpDsn | None, values: dict[str, Any]) -> str:
+        if v is not None:
             return v
 
-        if 'RMQ_PASSWORD_FILE' in values:
-            password_file = values.get('RMQ_PASSWORD_FILE')
+        if 'password_file' in values:
+            password_file = values.get('password_file')
             if isinstance(password_file, Path) and password_file.exists():
                 with password_file.open() as f:
-                    values['RMQ_PASSWORD'] = f.read().strip()
+                    values['password'] = f.read().strip()
 
         return AmqpDsn.build(
             scheme='amqp',
-            user=values.get('RMQ_USER'),
-            password=values.get('RMQ_PASSWORD'),
-            host=values.get('RMQ_HOST'),
-            port=str(values.get('RMQ_PORT')),
+            user=values.get('user'),
+            password=values.get('password'),
+            host=values.get('host'),
+            port=str(values.get('port')),
         )
-
-    class Config:
-        case_sensitive = False
-        env_file = '.env'
```

### Comparing `greyhorse_rmq-0.1/greyhorse_rmq/engine.py` & `greyhorse_rmq-0.2/greyhorse_rmq/engine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import asyncio
 from contextlib import AbstractAsyncContextManager, asynccontextmanager
+from typing import override
 
 import aio_pika
 from aio_pika.pool import Pool
 
-from greyhorse_core.engines.base import AsyncEngine
-from greyhorse_core.i18n import tr
-from greyhorse_core.logging import logger
-from greyhorse_rmq.config import EngineConfig
+from greyhorse.app.context import AsyncContextBuilder, Context
+from greyhorse.data.storage import DataStorageEngine
+from greyhorse.i18n import tr
+from greyhorse.logging import logger
+from .config import EngineConf
+from .contexts import RmqAsyncContext
 
 AsyncChannel = aio_pika.RobustChannel
 
 
-class RmqAsyncEngine(AsyncEngine[AsyncChannel]):
-    def __init__(self, name: str, config: EngineConfig):
+class RmqAsyncEngine(DataStorageEngine):
+    def __init__(self, name: str, config: EngineConf):
         super().__init__(name)
         self._config = config
         self._counter = 0
         self._lock = asyncio.Lock()
         self._conn_pool: Pool | None = None
         self._chan_pool: Pool | None = None
 
     @property
-    def connection_class(self):
-        return AsyncChannel
-
-    @asynccontextmanager
-    async def session(self, *args, **kwargs) -> AbstractAsyncContextManager[AsyncChannel]:
-        async with self._chan_pool.acquire() as conn:
-            yield conn
+    def active(self) -> bool:
+        return self._counter > 0
 
+    @override
     async def start(self):
         async with self._lock:
             if 0 == self._counter:
                 assert not self._conn_pool
                 assert not self._chan_pool
 
                 loop = asyncio.get_event_loop()
@@ -45,14 +44,15 @@
                     self._get_channel, loop=loop,
                     max_size=self._config.pool_max_channels_per_connection,
                 )
                 logger.info(tr('greyhorse.engines.rmq.engine.started').format(name=self.name))
 
             self._counter += 1
 
+    @override
     async def stop(self):
         async with self._lock:
             if 1 == self._counter:
                 assert self._conn_pool
                 assert self._chan_pool
 
                 await self._chan_pool.close()
@@ -61,14 +61,29 @@
                 self._conn_pool = self._chan_pool = None
                 logger.info(tr('greyhorse.engines.rmq.engine.stopped').format(name=self.name))
 
             self._counter = max(self._counter - 1, 0)
 
     async def _get_connection(self) -> aio_pika.abc.AbstractRobustConnection:
         return await aio_pika.connect_robust(
-            self._config.dsn, virtualhost=self._config.virtualhost,
+            str(self._config.dsn), virtualhost=self._config.virtualhost,
             timeout=self._config.timeout_seconds,
         )
 
     async def _get_channel(self) -> aio_pika.Channel:
         async with self._conn_pool.acquire() as connection:
             return await connection.channel()
+
+    @asynccontextmanager
+    async def session(self) -> AbstractAsyncContextManager[AsyncChannel]:
+        async with self._chan_pool.acquire() as conn:
+            yield conn
+
+    @override
+    def get_context[T: Context](self, kind: type[RmqAsyncContext]) -> T | None:
+        if kind is RmqAsyncContext:
+            builder = AsyncContextBuilder[RmqAsyncContext](kind)
+            builder.add_param('name', self.name)
+            builder.add_param('connection', self.session())
+            return builder.build()
+        else:
+            return None
```

### Comparing `greyhorse_rmq-0.1/greyhorse_rmq/resources.py` & `greyhorse_rmq-0.2/greyhorse_rmq/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,70 @@
-from typing import Mapping
+import asyncio
+from typing import Any, Mapping
 
-from dependency_injector.containers import Container
-
-from greyhorse_core.app import base
-from greyhorse_core.app.context import get_context
-from greyhorse_rmq.contexts import RmqAsyncContext, RmqAsyncContextFactory
-from greyhorse_rmq.engine import RmqAsyncEngine
-from greyhorse_rmq.factory import RmqAsyncEngineFactory
-
-
-class RmqAsyncResource(base.Resource, base.HasContainer):
-    def __init__(
-        self, container: Container,
-        engine_factory: RmqAsyncEngineFactory,
-        context_factory: RmqAsyncContextFactory,
-        engine_names: list[str] | None = None,
-    ):
-        base.Resource.__init__(self)
-        base.HasContainer.__init__(self, container)
-
-        self._engine_factory = engine_factory
-        self._context_factory = context_factory
-        self._engine_names = engine_names or list()
+from greyhorse.app.context import current_scope_id
+from greyhorse.app.entities.service import Service
+from greyhorse.app.utils.registry import DictRegistry, ScopedRegistry
+from greyhorse.result import Result
+from .config import EngineConf
+from .contexts import RmqAsyncContext, RmqAsyncContextProvider
+from .factory import RmqAsyncEngineFactory
+
+
+class RmqAsyncService(Service):
+    def __init__(self, name: str, configs: Mapping[str, EngineConf]):
+        super().__init__(name)
+        self._configs = configs
+        self._engine_factory = RmqAsyncEngineFactory()
+        self._active = False
+        self._event: asyncio.Event = asyncio.Event()
+        self._registry = ScopedRegistry[Any, Any](
+            factory=lambda: DictRegistry(), scope_func=current_scope_id,
+        )
+
+        for name in self._configs.keys():
+            self._provider_factories.set(
+                RmqAsyncContextProvider,
+                lambda: RmqAsyncContextProvider(self.create_context(name)),
+                name=name,
+            )
+
+    def create_context(self, name: str):
+        if instance := self._registry.get(RmqAsyncContext, name=name):
+            return instance
+
+        engine = self._engine_factory.get_engine(name)
+        instance = engine.get_context(RmqAsyncContext)
+        self._registry.set(RmqAsyncContext, instance, name=name)
+        return instance
 
     @property
-    def engines(self) -> Mapping[str, RmqAsyncEngine]:
-        return self._engine_factory.get_engines()
-
-    async def create(
-        self, application: base.Application,
-        module: base.Module | None = None,
-        service: base.Service | None = None,
-    ):
-        for name in self._engine_names:
-            self.container.create_engine(name)
-        else:
-            self.container.create_engine()
+    def active(self) -> bool:
+        return self._active
 
-        for engine in self.engines.values():
+    def create(self) -> Result:
+        for name, conf in self._configs.items():
+            self._engine_factory.create_engine(name, conf)
+        return Result.from_ok()
+
+    def destroy(self) -> Result:
+        for name in self._configs.keys():
+            self._engine_factory.destroy_engine(name)
+        return Result.from_ok()
+
+    async def start(self):
+        for name in self._configs.keys():
+            engine = self._engine_factory.get_engine(name)
             await engine.start()
+        self._active = True
+        self._event.clear()
 
-    async def destroy(
-        self, application: base.Application,
-        module: base.Module | None = None,
-        service: base.Service | None = None,
-    ):
-        for engine in reversed(self.engines.values()):
+    async def stop(self):
+        self._registry.clear()
+        for name in self._configs.keys():
+            engine = self._engine_factory.get_engine(name)
             await engine.stop()
+        self._active = False
+        self._event.set()
 
-    async def acquire(
-        self, application: base.Application,
-        module: base.Module | None = None,
-        service: base.Service | None = None,
-    ):
-        ctx_storage = get_context()
-
-        for name, engine in self.engines.items():
-            ctx = self._context_factory(engine)
-
-            if 'rmq' not in ctx_storage:
-                ctx_storage.rmq = ctx
-            elif isinstance(ctx_storage.rmq, RmqAsyncContext):
-                prev_ctx = ctx_storage.rmq
-                ctx_storage.rmq = {prev_ctx.name: prev_ctx, name: ctx}
-            else:
-                ctx_storage.rmq[name] = ctx
-
-            await ctx.__aenter__()
-
-    async def release(
-        self, application: base.Application,
-        module: base.Module | None = None,
-        service: base.Service | None = None,
-    ):
-        ctx_storage = get_context()
-
-        for name, engine in self.engines.items():
-            if 'rmq' not in ctx_storage:
-                break
-            elif isinstance(ctx_storage.rmq, RmqAsyncContext):
-                ctx = ctx_storage.rmq
-                del ctx_storage.rmq
-            else:
-                ctx = ctx_storage.rmq.pop(name, None)
-
-            if ctx:
-                await ctx.__aexit__(None, None, None)
-
-    def get_engine(self, name: str) -> RmqAsyncEngine | None:
-        return self._engine_factory.get_engine(name)
+    def wait(self):
+        return self._event
```

### Comparing `greyhorse_rmq-0.1/greyhorse_rmq/rpc/client.py` & `greyhorse_rmq-0.2/greyhorse_rmq/rpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import uuid
 from typing import MutableMapping
 
 import aio_pika
 
-from greyhorse_core.i18n import tr
-from greyhorse_core.logging import logger
-from greyhorse_rmq.engine import AsyncChannel
+from greyhorse.i18n import tr
+from greyhorse.logging import logger
+from ..engine import AsyncChannel
 
 
 class AsyncRmqClient:
     def __init__(
         self, channel: AsyncChannel, routing_key: str,
         exchange: aio_pika.RobustExchange | None = None,
         app_id: str | None = None, queue_name: str | None = None,
```

### Comparing `greyhorse_rmq-0.1/pyproject.toml` & `greyhorse_rmq-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 [tool.poetry]
 name = "greyhorse-rmq"
-version = "0.1"
+version = "0.2"
 description = "Greyhorse RabbitMQ library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Typing :: Typed",
 ]
 
 packages = [
     { include = "greyhorse_rmq" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-greyhorse_core = { path = "../core/", develop = true }
+python = "^3.12"
+greyhorse = [
+    { path = "../../core/", develop = true },
+    { version = "0.4.2" }
+]
+pydantic = {version = "^2.0", extras = ["dotenv"]}
+pydantic-settings = "^2.2.1"
 
 aio-pika = {version = "^9.1", optional = true}
 
 [tool.poetry.extras]
 async = ["aio-pika"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2"
-pytest-asyncio = "^0.21"
-pytest-cov = "^4.0"
-pytest-mock = "^3.10"
+pytest = "^7.4"
+pytest-asyncio = "^0.23"
+pytest-cov = "^4.1"
+pytest-mock = "^3.12"
 pytest-faker = "^2.0"
-autoflake = "^2.0"
-black = "^23.1"
-flake8 = "^6.0"
+autoflake = "^2.2"
+black = "^23.11"
+flake8 = "^6.1"
 isort = "^5.12"
-mypy = "^1.1"
-pre-commit = "^3.2"
+mypy = "^1.7"
+pre-commit = "^3.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-monorepo-dependency-plugin]
 enable = true
```

### Comparing `greyhorse_rmq-0.1/PKG-INFO` & `greyhorse_rmq-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: greyhorse-rmq
-Version: 0.1
+Version: 0.2
 Summary: Greyhorse RabbitMQ library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Provides-Extra: async
 Requires-Dist: aio-pika (>=9.1,<10.0) ; extra == "async"
-Requires-Dist: greyhorse_core @ file:///home/plutonium/Projects/greyhorse/core
+Requires-Dist: greyhorse (==0.4.2)
+Requires-Dist: greyhorse @ file:///home/plutonium/projects/greyhorse/core
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

