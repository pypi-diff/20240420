# Comparing `tmp/greyhorse_clickhouse-0.1.tar.gz` & `tmp/greyhorse_clickhouse-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_clickhouse-0.1.tar", max compression
+gzip compressed data, was "greyhorse_clickhouse-0.2.tar", max compression
```

## Comparing `greyhorse_clickhouse-0.1.tar` & `greyhorse_clickhouse-0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0       96 2023-07-11 21:09:28.005345 greyhorse_clickhouse-0.1/greyhorse_clickhouse/__init__.py
--rw-r--r--   0        0        0     1262 2023-07-11 23:01:23.999306 greyhorse_clickhouse-0.1/greyhorse_clickhouse/config.py
--rw-r--r--   0        0        0     2815 2023-07-11 23:01:24.111303 greyhorse_clickhouse-0.1/greyhorse_clickhouse/containers.py
--rw-r--r--   0        0        0     1523 2023-07-11 21:13:38.066218 greyhorse_clickhouse-0.1/greyhorse_clickhouse/contexts.py
--rw-r--r--   0        0        0     1966 2023-07-11 23:01:23.827310 greyhorse_clickhouse-0.1/greyhorse_clickhouse/engine.py
--rw-r--r--   0        0        0     1304 2023-07-11 23:01:24.055304 greyhorse_clickhouse-0.1/greyhorse_clickhouse/factory.py
--rw-r--r--   0        0        0     2972 2023-07-11 23:01:23.919308 greyhorse_clickhouse-0.1/greyhorse_clickhouse/resources.py
--rw-r--r--   0        0        0      194 2023-07-11 21:07:46.751891 greyhorse_clickhouse-0.1/greyhorse_clickhouse/translations.toml
--rw-r--r--   0        0        0     1079 2023-07-11 22:59:25.810283 greyhorse_clickhouse-0.1/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 greyhorse_clickhouse-0.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-09 22:29:35.957597 greyhorse_clickhouse-0.2/greyhorse_clickhouse/__init__.py
+-rw-r--r--   0        0        0     1546 2024-04-20 12:39:12.122924 greyhorse_clickhouse-0.2/greyhorse_clickhouse/config.py
+-rw-r--r--   0        0        0      319 2024-04-20 12:39:12.134923 greyhorse_clickhouse-0.2/greyhorse_clickhouse/contexts.py
+-rw-r--r--   0        0        0     2472 2024-04-20 13:18:21.558923 greyhorse_clickhouse-0.2/greyhorse_clickhouse/engine.py
+-rw-r--r--   0        0        0      768 2024-04-20 12:39:12.078925 greyhorse_clickhouse-0.2/greyhorse_clickhouse/factory.py
+-rw-r--r--   0        0        0     2349 2024-04-20 12:39:12.106924 greyhorse_clickhouse-0.2/greyhorse_clickhouse/service.py
+-rw-r--r--   0        0        0      194 2023-07-11 23:07:25.000000 greyhorse_clickhouse-0.2/greyhorse_clickhouse/translations.toml
+-rw-r--r--   0        0        0     1217 2024-04-20 13:53:39.994775 greyhorse_clickhouse-0.2/pyproject.toml
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 greyhorse_clickhouse-0.2/PKG-INFO
```

### Comparing `greyhorse_clickhouse-0.1/greyhorse_clickhouse/config.py` & `greyhorse_clickhouse-0.2/greyhorse_clickhouse/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 
-from pydantic import AnyHttpUrl, BaseSettings, validator
+from pydantic import BaseModel, Field, field_validator
+from pydantic.networks import ClickHouseDsn
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
-@dataclass
-class EngineConfig:
-    dsn: str
+class EngineConf(BaseModel):
+    dsn: ClickHouseDsn
     echo: bool = False
+    pool_min_size: int = Field(default=1, gt=0)
+    pool_max_size: int = Field(default=8, gt=0)
+
+
+class ClickHouseSettings(BaseSettings):
+    host: str = 'localhost'
+    port: int = 9000
+    user: str = 'default'
+    password: str = ''
+    password_file: Path | None = None
+    database: str = 'default'
     pool_min_size: int = 1
-    pool_max_size: int = 8
+    pool_max_size: int = 4
 
+    dsn: ClickHouseDsn | None = None
 
-class CHSettings(BaseSettings):
-    CH_HOST: str = 'localhost'
-    CH_PORT: int = 9000
-    CH_USER: str = 'default'
-    CH_PASSWORD: str = ''
-    CH_PASSWORD_FILE: Path | None = None
-    CH_DB: str
-    CH_POOL_MIN_SIZE: int = 1
-    CH_POOL_MAX_SIZE: int = 4
-
-    CH_URI: AnyHttpUrl | None = None
-
-    @validator('CH_URI', pre=True)
-    def assemble_dsn(cls, v: str | None, values: dict[str, Any]) -> str:
-        if isinstance(v, str):
+    model_config = SettingsConfigDict(env_file='.env', case_sensitive=False, env_prefix='ch_')
+
+    @classmethod
+    @field_validator('dsn', mode='before')
+    def assemble_dsn(cls, v: ClickHouseDsn | None, values: dict[str, Any]) -> str:
+        if v is not None:
             return v
 
-        if 'CH_PASSWORD_FILE' in values:
-            password_file = values.get('CH_PASSWORD_FILE')
+        if 'password_file' in values:
+            password_file = values.get('password_file')
             if isinstance(password_file, Path) and password_file.exists():
                 with password_file.open() as f:
-                    values['CH_PASSWORD'] = f.read().strip()
-
-        return f'clickhouse://{values.get("CH_USER")}:{values.get("CH_PASSWORD")}' \
-               f'@{values.get("CH_HOST")}:{values.get("CH_PORT")}/{values.get("CH_DB", "")}'
+                    values['password'] = f.read().strip()
 
-    class Config:
-        case_sensitive = False
-        env_file = '.env'
+        return ClickHouseDsn.build(
+            scheme='clickhouse',
+            user=values.get('user'),
+            password=values.get('password'),
+            host=values.get('host'),
+            port=str(values.get('port')),
+            path=f'/{values.get("database", "default")}',
+        )
```

### Comparing `greyhorse_clickhouse-0.1/greyhorse_clickhouse/engine.py` & `greyhorse_clickhouse-0.2/greyhorse_clickhouse/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 import asyncio
 from contextlib import AbstractAsyncContextManager, asynccontextmanager
+from typing import override
 
 import asynch
 from asynch.cursors import DictCursor
 from asynch.pool import Pool
 
-from greyhorse_clickhouse.config import EngineConfig
-from greyhorse_core.engines.base import AsyncEngine
-from greyhorse_core.i18n import tr
-from greyhorse_core.logging import logger
+from greyhorse.app.context import AsyncContextBuilder, Context
+from greyhorse.data.storage import DataStorageEngine
+from greyhorse.i18n import tr
+from greyhorse.logging import logger
+from .config import EngineConf
+from .contexts import ClickHouseContext
 
-AsyncChannel = asynch.connection.Cursor
+type AsyncChannel = asynch.connection.Cursor
 
 
-class CHAsyncEngine(AsyncEngine[AsyncChannel]):
-    def __init__(self, name: str, config: EngineConfig):
+class ClickHouseAsyncEngine(DataStorageEngine):
+    def __init__(self, name: str, config: EngineConf):
         super().__init__(name)
         self._config = config
         self._counter = 0
         self._lock = asyncio.Lock()
         self._pool: Pool | None = None
 
     @property
-    def connection_class(self):
-        return AsyncChannel
-
-    @asynccontextmanager
-    async def session(self, *args, **kwargs) -> AbstractAsyncContextManager[AsyncChannel]:
-        async with self._pool.acquire() as conn:
-            async with conn.cursor() as cursor:
-                yield cursor
+    def active(self) -> bool:
+        return self._counter > 0
 
+    @override
     async def start(self):
         async with self._lock:
             if 0 == self._counter:
                 assert not self._pool
 
                 loop = asyncio.get_event_loop()
                 self._pool = Pool(
-                    dsn=self._config.dsn, echo=self._config.echo,
+                    dsn=str(self._config.dsn), echo=self._config.echo,
                     minsize=self._config.pool_min_size,
                     maxsize=self._config.pool_max_size,
                     loop=loop, cursor_cls=DictCursor,
                 )
                 logger.info(tr('greyhorse.engines.ch.engine.started').format(name=self.name))
 
             self._counter += 1
 
+    @override
     async def stop(self):
         async with self._lock:
             if 1 == self._counter:
                 assert self._pool
 
                 self._pool.close()
                 await self._pool.wait_closed()
 
                 self._pool = None
                 logger.info(tr('greyhorse.engines.ch.engine.stopped').format(name=self.name))
 
             self._counter = max(self._counter - 1, 0)
+
+    @asynccontextmanager
+    async def session(self) -> AbstractAsyncContextManager[AsyncChannel]:
+        async with self._pool.acquire() as conn:
+            async with conn.cursor() as cursor:
+                yield cursor
+
+    @override
+    def get_context[T: Context](self, kind: type[ClickHouseContext]) -> T | None:
+        if kind is ClickHouseContext:
+            builder = AsyncContextBuilder[ClickHouseContext](kind)
+            builder.add_param('name', self.name)
+            builder.add_param('connection', self.session())
+            return builder.build()
+        else:
+            return None
```

### Comparing `greyhorse_clickhouse-0.1/greyhorse_clickhouse/resources.py` & `greyhorse_clickhouse-0.2/greyhorse_clickhouse/service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,70 @@
-from typing import Mapping
+import asyncio
+from typing import Any, Mapping
 
-from dependency_injector.containers import Container
-
-from greyhorse_clickhouse.contexts import CHAsyncContext, CHAsyncContextFactory
-from greyhorse_clickhouse.engine import CHAsyncEngine
-from greyhorse_clickhouse.factory import CHAsyncEngineFactory
-from greyhorse_core.app import base
-from greyhorse_core.app.context import get_context
-
-
-class CHAsyncResource(base.Resource, base.HasContainer):
-    def __init__(
-        self, container: Container,
-        engine_factory: CHAsyncEngineFactory,
-        context_factory: CHAsyncContextFactory,
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
+from .contexts import ClickHouseContext, ClickHouseContextProvider
+from .factory import CHAsyncEngineFactory
+
+
+class ClickHouseService(Service):
+    def __init__(self, name: str, configs: Mapping[str, EngineConf]):
+        super().__init__(name)
+        self._configs = configs
+        self._engine_factory = CHAsyncEngineFactory()
+        self._active = False
+        self._event: asyncio.Event = asyncio.Event()
+        self._registry = ScopedRegistry[Any, Any](
+            factory=lambda: DictRegistry(), scope_func=current_scope_id,
+        )
+
+        for name in self._configs.keys():
+            self._provider_factories.set(
+                ClickHouseContextProvider,
+                lambda: ClickHouseContextProvider(self.create_context(name)),
+                name=name,
+            )
+
+    def create_context(self, name: str):
+        if instance := self._registry.get(ClickHouseContext, name=name):
+            return instance
+
+        engine = self._engine_factory.get_engine(name)
+        instance = engine.get_context(ClickHouseContext)
+        self._registry.set(ClickHouseContext, instance, name=name)
+        return instance
 
     @property
-    def engines(self) -> Mapping[str, CHAsyncEngine]:
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
-            if 'ch' not in ctx_storage:
-                ctx_storage.ch = ctx
-            elif isinstance(ctx_storage.ch, CHAsyncContext):
-                prev_ctx = ctx_storage.ch
-                ctx_storage.ch = {prev_ctx.name: prev_ctx, name: ctx}
-            else:
-                ctx_storage.ch[name] = ctx
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
-            if 'ch' not in ctx_storage:
-                break
-            elif isinstance(ctx_storage.ch, CHAsyncContext):
-                ctx = ctx_storage.ch
-                del ctx_storage.ch
-            else:
-                ctx = ctx_storage.ch.pop(name, None)
-
-            if ctx:
-                await ctx.__aexit__(None, None, None)
-
-    def get_engine(self, name: str) -> CHAsyncEngine | None:
-        return self._engine_factory.get_engine(name)
+    def wait(self):
+        return self._event
```

### Comparing `greyhorse_clickhouse-0.1/pyproject.toml` & `greyhorse_clickhouse-0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 [tool.poetry]
 name = "greyhorse-clickhouse"
-version = "0.1"
+version = "0.2"
 description = "Greyhorse ClickHouse library"
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
     { include = "greyhorse_clickhouse" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-greyhorse_core = { path = "../core/", develop = true }
+python = "^3.12"
+greyhorse = [
+#    { path = "../../core/", develop = true },
+    { version = "0.4.2" }
+]
+pydantic = {version = "^2.0", extras = ["dotenv"]}
+pydantic-settings = "^2.2.1"
 
-asynch = { version = "^0.2.2", optional = true }
+asynch = { version = "^0.2.3", optional = true }
 
 [tool.poetry.extras]
 async = ["asynch"]
 
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

