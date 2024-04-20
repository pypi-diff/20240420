# Comparing `tmp/greyhorse-0.4.1.tar.gz` & `tmp/greyhorse-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse-0.4.1.tar", max compression
+gzip compressed data, was "greyhorse-0.4.2.tar", max compression
```

## Comparing `greyhorse-0.4.1.tar` & `greyhorse-0.4.2.tar`

### file list

```diff
@@ -1,62 +1,60 @@
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/app/builders/__init__.py
--rw-r--r--   0        0        0    13843 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/app/builders/module.py
--rw-r--r--   0        0        0     2858 2024-04-09 22:29:40.601420 greyhorse-0.4.1/greyhorse/app/builders/resource.py
--rw-r--r--   0        0        0     1568 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/app/context.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.1/greyhorse/app/entities/__init__.py
--rw-r--r--   0        0        0     8340 2024-04-10 16:01:20.918796 greyhorse-0.4.1/greyhorse/app/entities/application.py
--rw-r--r--   0        0        0     4610 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/controller.py
--rw-r--r--   0        0        0      789 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/deps.py
--rw-r--r--   0        0        0    18024 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/module.py
--rw-r--r--   0        0        0      300 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/operator.py
--rw-r--r--   0        0        0     3139 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/providers.py
--rw-r--r--   0        0        0     1577 2024-04-09 22:29:40.601420 greyhorse-0.4.1/greyhorse/app/entities/resource.py
--rw-r--r--   0        0        0     6110 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/entities/service.py
--rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.1/greyhorse/app/errors.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/schemas/__init__.py
--rw-r--r--   0        0        0      897 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/schemas/components.py
--rw-r--r--   0        0        0      644 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/schemas/controller.py
--rw-r--r--   0        0        0     1790 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/schemas/module.py
--rw-r--r--   0        0        0      647 2024-04-09 22:29:35.965597 greyhorse-0.4.1/greyhorse/app/schemas/service.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/app/tasks/__init__.py
--rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/app/tasks/app.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/app/utils/__init__.py
--rw-r--r--   0        0        0     4145 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/app/utils/registry.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/cache/__init__.py
--rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/cache/base.py
--rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/cache/method.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/models/__init__.py
--rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.1/greyhorse/data/models/base.py
--rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/models/fields.py
--rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/models/filterable.py
--rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/models/model.py
--rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/models/serializable.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/repositories/__init__.py
--rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/repositories/base.py
--rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/repositories/filterable.py
--rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/serializers/__init__.py
--rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/serializers/base.py
--rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/data/serializers/pickle.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/engines/__init__.py
--rw-r--r--   0        0        0     1419 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/engines/base.py
--rw-r--r--   0        0        0      917 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/engines/factory.py
--rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.1/greyhorse/i18n/__init__.py
--rw-r--r--   0        0        0     2764 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/i18n/translator.py
--rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/logging.py
--rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/messagebus.py
--rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/result.py
--rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.1/greyhorse/translations.toml
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/confs.py
--rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/dicts.py
--rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/hashes.py
--rw-r--r--   0        0        0      922 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/imports.py
--rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/injectors.py
--rw-r--r--   0        0        0     1456 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/invoke.py
--rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/json.py
--rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/strings.py
--rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.1/greyhorse/utils/time.py
--rw-r--r--   0        0        0     1253 2024-04-10 16:11:00.398342 greyhorse-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/builders/__init__.py
+-rw-r--r--   0        0        0    13843 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/builders/module.py
+-rw-r--r--   0        0        0     2858 2024-04-09 22:29:40.601420 greyhorse-0.4.2/greyhorse/app/builders/resource.py
+-rw-r--r--   0        0        0    10686 2024-04-20 11:56:32.782673 greyhorse-0.4.2/greyhorse/app/context.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.2/greyhorse/app/entities/__init__.py
+-rw-r--r--   0        0        0     8340 2024-04-10 16:01:20.918796 greyhorse-0.4.2/greyhorse/app/entities/application.py
+-rw-r--r--   0        0        0     4812 2024-04-14 12:30:24.508646 greyhorse-0.4.2/greyhorse/app/entities/controller.py
+-rw-r--r--   0        0        0      910 2024-04-14 12:24:31.419245 greyhorse-0.4.2/greyhorse/app/entities/deps.py
+-rw-r--r--   0        0        0    19413 2024-04-17 16:38:43.638882 greyhorse-0.4.2/greyhorse/app/entities/module.py
+-rw-r--r--   0        0        0      253 2024-04-18 23:28:44.736666 greyhorse-0.4.2/greyhorse/app/entities/operator.py
+-rw-r--r--   0        0        0     2903 2024-04-20 10:49:17.227923 greyhorse-0.4.2/greyhorse/app/entities/providers.py
+-rw-r--r--   0        0        0     1577 2024-04-09 22:29:40.601420 greyhorse-0.4.2/greyhorse/app/entities/resource.py
+-rw-r--r--   0        0        0     6110 2024-04-09 22:29:35.965597 greyhorse-0.4.2/greyhorse/app/entities/service.py
+-rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.2/greyhorse/app/errors.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.2/greyhorse/app/schemas/__init__.py
+-rw-r--r--   0        0        0      883 2024-04-20 11:54:14.943578 greyhorse-0.4.2/greyhorse/app/schemas/components.py
+-rw-r--r--   0        0        0      587 2024-04-20 11:54:14.975577 greyhorse-0.4.2/greyhorse/app/schemas/controller.py
+-rw-r--r--   0        0        0     1762 2024-04-20 11:54:14.955577 greyhorse-0.4.2/greyhorse/app/schemas/module.py
+-rw-r--r--   0        0        0      590 2024-04-20 11:54:14.963577 greyhorse-0.4.2/greyhorse/app/schemas/service.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/tasks/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/tasks/app.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/app/utils/__init__.py
+-rw-r--r--   0        0        0     6880 2024-04-17 14:33:40.645939 greyhorse-0.4.2/greyhorse/app/utils/registry.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/__init__.py
+-rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/base.py
+-rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/cache/method.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/models/__init__.py
+-rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.2/greyhorse/data/models/base.py
+-rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/fields.py
+-rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/filterable.py
+-rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/model.py
+-rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/models/serializable.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/__init__.py
+-rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/base.py
+-rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/repositories/filterable.py
+-rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/base.py
+-rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/data/serializers/pickle.py
+-rw-r--r--   0        0        0     1902 2024-04-20 11:58:08.771261 greyhorse-0.4.2/greyhorse/data/storage.py
+-rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.2/greyhorse/i18n/__init__.py
+-rw-r--r--   0        0        0     2663 2024-04-18 23:30:16.265809 greyhorse-0.4.2/greyhorse/i18n/translator.py
+-rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/logging.py
+-rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/messagebus.py
+-rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/result.py
+-rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.2/greyhorse/translations.toml
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/confs.py
+-rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/dicts.py
+-rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/hashes.py
+-rw-r--r--   0        0        0      922 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/imports.py
+-rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/injectors.py
+-rw-r--r--   0        0        0     1573 2024-04-20 10:13:14.653404 greyhorse-0.4.2/greyhorse/utils/invoke.py
+-rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/json.py
+-rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/strings.py
+-rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.2/greyhorse/utils/time.py
+-rw-r--r--   0        0        0     1040 2024-04-20 11:58:08.375275 greyhorse-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.2/PKG-INFO
```

### Comparing `greyhorse-0.4.1/greyhorse/app/builders/module.py` & `greyhorse-0.4.2/greyhorse/app/builders/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/builders/resource.py` & `greyhorse-0.4.2/greyhorse/app/builders/resource.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/application.py` & `greyhorse-0.4.2/greyhorse/app/entities/application.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/controller.py` & `greyhorse-0.4.2/greyhorse/app/entities/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,19 @@
         return None
 
     def set_resource(self, key: type, instance: Any, name: str | None = None) -> bool:
         if not self._deps_operator:
             return False
         return self._deps_operator.set_resource(key, instance, name=name)
 
+    def reset_resource(self, key: type, name: str | None = None) -> bool:
+        if not self._deps_operator:
+            return False
+        return self._deps_operator.reset_resource(key, name=name)
+
     @property
     def operator_factories(self) -> OperatorFactoryRegistry:
         return self._op_factories
 
     def create(self) -> Awaitable[Result] | Result:
         return Result.from_ok()
```

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/deps.py` & `greyhorse-0.4.2/greyhorse/app/entities/deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,13 @@
 class DepsOperator(ABC):
 
     @abstractmethod
     def set_resource(
         self, key: Any, instance: Any, name: str | None = None,
     ) -> bool:
         ...
+
+    @abstractmethod
+    def reset_resource(
+        self, key: Any, name: str | None = None,
+    ) -> bool:
+        ...
```

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/module.py` & `greyhorse-0.4.2/greyhorse/app/entities/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from dataclasses import dataclass
 from typing import Any, Literal, Mapping, Self, TYPE_CHECKING, cast, override
 
 from greyhorse.result import Error, Result
 from greyhorse.utils.invoke import invoke_sync
 from .controller import Controller, ControllerKey
 from .deps import DepsOperator, DepsProvider
@@ -101,14 +102,26 @@
             name_pattern = self._resources_write[key]
             if name_pattern is not None:
                 if name is None or not name_pattern.match(name):
                     return False
             return self._deps_registry.set(key, instance, name)
         return False
 
+    @override
+    def reset_resource(
+        self, key: Any, name: str | None = None,
+    ) -> bool:
+        if key in self._resources_write:
+            name_pattern = self._resources_write[key]
+            if name_pattern is not None:
+                if name is None or not name_pattern.match(name):
+                    return False
+            return self._deps_registry.reset(key, name)
+        return False
+
 
 class Module:
     def __init__(self, name: str, conf: 'ModuleConf'):
         self._name = name
         self._conf = conf
         self._modules: dict[str, Self] = {}
         self._controllers = DictRegistry[ControllerKey, Controller]()
@@ -249,17 +262,35 @@
 
     @property
     def operator_factories(self) -> OperatorFactoryRegistry:
         return self._operator_factories
 
     def satisfy_provider_claims(self, items: list[ModuleProviderItem]) -> list[ModuleErrorsItem]:
         errors: list[ModuleErrorsItem] = []
-
+        items_set: dict[ProviderKey, dict[str | None, ProviderFactoryFn]] = defaultdict(dict)
         for item in items:
-            self._provider_factories.set(item.key, item.instance, name=item.name)
+            items_set[item.key][item.name] = item.instance
+
+        for claim in self.config.provider_claims:
+            result = False
+
+            for name, instance in items_set.get(claim.key, {}).items():
+                if claim.name_pattern is not None:
+                    if claim.name_pattern.match(name):
+                        result = self._provider_factories.set(claim.key, instance, name=name)
+                        break
+                else:
+                    result = self._provider_factories.set(claim.key, instance, name=name)
+
+            if not result:
+                claim_name = f'{claim.key}' + (f' ("{claim.name_pattern}")' if claim.name_pattern else '')
+                error = ProvClaimPolicyViolation(type='module', name=self.name, claim_name=claim_name)
+                errors.append(ModuleErrorsItem(
+                    where='provider', name=claim_name, errors=[error],
+                ))
 
         for module in self._modules.values():
             sub_errors = module._resolve_claims(self)
             for error_item in sub_errors:
                 errors.append(ModuleErrorsItem(
                     where='module', name=module.name, errors=error_item.errors,
                 ))
@@ -401,43 +432,43 @@
 
         logger.info(tr('app.entities.module.destroy-finish').format(name=self.name))
         return errors
 
     def start(self):
         logger.info(tr('app.entities.module.start-start').format(name=self.name))
 
-        for key in self._services.list_keys():
-            for name in self._services.get_names(key):
-                instance = self._services.get(key, name)
+        for key in self._controllers.list_keys():
+            for name in self._controllers.get_names(key):
+                instance = self._controllers.get(key, name)
                 invoke_sync(instance.start)
-                logger.info(tr('app.entities.module.service-started').format(name=name))
+                logger.info(tr('app.entities.module.ctrl-started').format(name=name))
 
         for module in self._modules.values():
             module.start()
 
-        for key in self._controllers.list_keys():
-            for name in self._controllers.get_names(key):
-                instance = self._controllers.get(key, name)
+        for key in self._services.list_keys():
+            for name in self._services.get_names(key):
+                instance = self._services.get(key, name)
                 invoke_sync(instance.start)
-                logger.info(tr('app.entities.module.ctrl-started').format(name=name))
+                logger.info(tr('app.entities.module.service-started').format(name=name))
 
         logger.info(tr('app.entities.module.start-finish').format(name=self.name))
 
     def stop(self):
         logger.info(tr('app.entities.module.stop-start').format(name=self.name))
 
-        for key in self._controllers.list_keys():
-            for name in self._controllers.get_names(key):
-                instance = self._controllers.get(key, name)
+        for key in self._services.list_keys():
+            for name in self._services.get_names(key):
+                instance = self._services.get(key, name)
                 invoke_sync(instance.stop)
-                logger.info(tr('app.entities.module.ctrl-stopped').format(name=name))
+                logger.info(tr('app.entities.module.service-stopped').format(name=name))
 
         for module in reversed(self._modules.values()):
             module.stop()
 
-        for key in self._services.list_keys():
-            for name in self._services.get_names(key):
-                instance = self._services.get(key, name)
+        for key in self._controllers.list_keys():
+            for name in self._controllers.get_names(key):
+                instance = self._controllers.get(key, name)
                 invoke_sync(instance.stop)
-                logger.info(tr('app.entities.module.service-stopped').format(name=name))
+                logger.info(tr('app.entities.module.ctrl-stopped').format(name=name))
 
         logger.info(tr('app.entities.module.stop-finish').format(name=self.name))
```

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/resource.py` & `greyhorse-0.4.2/greyhorse/app/entities/resource.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/entities/service.py` & `greyhorse-0.4.2/greyhorse/app/entities/service.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/errors.py` & `greyhorse-0.4.2/greyhorse/app/errors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/app/schemas/components.py` & `greyhorse-0.4.2/greyhorse/app/schemas/components.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import Any, Pattern
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, Field
 
 from ..entities.operator import OperatorKey
 from ..entities.providers import ProviderKey
 
 
-class DepsPolicy[DK](BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class DepsPolicy[DK](BaseModel, frozen=True, arbitrary_types_allowed=True):
     key: DK
     name_pattern: Pattern | None = None
 
 
 class ResourcePolicy(DepsPolicy[Any]):
     pass
 
@@ -21,17 +19,15 @@
     pass
 
 
 class OperatorPolicy(DepsPolicy[OperatorKey]):
     pass
 
 
-class ResourceConf[K](BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class ResourceConf[K](BaseModel, frozen=True, arbitrary_types_allowed=True):
     key: K
     name: str | None = None
     args: dict[str, Any] = Field(default_factory=dict)
     enabled: bool = Field(default=True)
     resources_read: list[ResourcePolicy] = Field(default_factory=list)
     providers_read: list[ProviderPolicy] = Field(default_factory=list)
     operators_read: list[OperatorPolicy] = Field(default_factory=list)
```

### Comparing `greyhorse-0.4.1/greyhorse/app/schemas/controller.py` & `greyhorse-0.4.2/greyhorse/app/schemas/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from typing import Pattern
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, Field
 
 from .components import ResourceConf, ResourcePolicy
 from ..entities.controller import ControllerKey
 from ..entities.operator import OperatorKey
 
 
-class OperatorMappingPolicy(BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class OperatorMappingPolicy(BaseModel, frozen=True, arbitrary_types_allowed=True):
     key: OperatorKey
     map_to: OperatorKey
     name_pattern: Pattern | None = None
 
 
 class ControllerConf(ResourceConf[ControllerKey]):
-    model_config = ConfigDict(frozen=True)
-
     operator_mapping: list[OperatorMappingPolicy] = Field(default_factory=list)
     resources_write: list[ResourcePolicy] = Field(default_factory=list)
```

### Comparing `greyhorse-0.4.1/greyhorse/app/schemas/module.py` & `greyhorse-0.4.2/greyhorse/app/schemas/module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 from typing import Any, Callable, Optional, Pattern
 
-from pydantic import BaseModel, ConfigDict, Field, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr
 
 from greyhorse.utils.invoke import caller_path
 from .controller import ControllerConf
 from .service import ServiceConf
 from ..entities.controller import ControllerFactoryMapping
 from ..entities.module import Module
 from ..entities.operator import OperatorKey
 from ..entities.providers import ProviderKey
 from ..entities.service import ServiceFactoryMapping
 
 
-class ProviderClaim(BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class ProviderClaim(BaseModel, frozen=True, arbitrary_types_allowed=True):
     key: ProviderKey
     name_pattern: Pattern | None = None
 
 
-class OperatorExport(BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class OperatorExport(BaseModel, frozen=True, arbitrary_types_allowed=True):
     key: OperatorKey
     name_pattern: Pattern | None = None
 
 
 class ModuleDesc(BaseModel):
     path: str = Field(frozen=True)
     args: dict[str, Any] = Field(default_factory=dict)
     enabled: bool = Field(default=True, frozen=True)
 
     _conf: Optional['ModuleConf'] = PrivateAttr(default=None)
     _initpath: list[str] = PrivateAttr(default_factory=lambda: caller_path(5))
 
 
-class ModuleConf(BaseModel):
-    model_config = ConfigDict(frozen=True)
-
+class ModuleConf(BaseModel, arbitrary_types_allowed=True):
     name: str = Field(frozen=True)
     enabled: bool = Field(default=True)
     factory: Callable[[...], Module] = Field(default=Module, frozen=True)
 
     submodules: list[ModuleDesc] = Field(default_factory=list)
 
     controllers: list[ControllerConf] = Field(default_factory=list)
```

### Comparing `greyhorse-0.4.1/greyhorse/app/tasks/app.py` & `greyhorse-0.4.2/greyhorse/app/tasks/app.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/cache/base.py` & `greyhorse-0.4.2/greyhorse/data/cache/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/cache/method.py` & `greyhorse-0.4.2/greyhorse/data/cache/method.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/models/base.py` & `greyhorse-0.4.2/greyhorse/data/models/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/models/fields.py` & `greyhorse-0.4.2/greyhorse/data/models/fields.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/models/filterable.py` & `greyhorse-0.4.2/greyhorse/data/models/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/models/model.py` & `greyhorse-0.4.2/greyhorse/data/models/model.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/models/serializable.py` & `greyhorse-0.4.2/greyhorse/data/models/serializable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/repositories/base.py` & `greyhorse-0.4.2/greyhorse/data/repositories/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/repositories/filterable.py` & `greyhorse-0.4.2/greyhorse/data/repositories/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/serializers/base.py` & `greyhorse-0.4.2/greyhorse/data/serializers/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/data/serializers/pickle.py` & `greyhorse-0.4.2/greyhorse/data/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/i18n/translator.py` & `greyhorse-0.4.2/greyhorse/i18n/translator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from importlib.resources import Package, as_file, files
 from pathlib import Path
 
 import tomlkit
 
-from greyhorse.app.context import get_context
 from greyhorse.utils.dicts import build_dotted_keys_from_dict
 
 
 class StaticTranslator:
     def __init__(self):
         self._data = dict()
         self._defaults = dict()
@@ -44,16 +43,14 @@
         self._defaults[namespace] = lang
         return True
 
     def namespaces(self) -> set[str]:
         return set(self._defaults.keys())
 
     def __call__(self, key: str, lang: str | None = None, default: str = '') -> str:
-        lang = lang or get_context().data.get('lang')
-
         if len(self._defaults) == 1:
             ns = list(self._defaults.keys())[0]
         else:
             ns = key.find('.')
             ns = key[0:ns] if ns != -1 else None
 
         tries = []
```

### Comparing `greyhorse-0.4.1/greyhorse/logging.py` & `greyhorse-0.4.2/greyhorse/logging.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/messagebus.py` & `greyhorse-0.4.2/greyhorse/messagebus.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/result.py` & `greyhorse-0.4.2/greyhorse/result.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/translations.toml` & `greyhorse-0.4.2/greyhorse/translations.toml`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/dicts.py` & `greyhorse-0.4.2/greyhorse/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/hashes.py` & `greyhorse-0.4.2/greyhorse/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/imports.py` & `greyhorse-0.4.2/greyhorse/utils/imports.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/injectors.py` & `greyhorse-0.4.2/greyhorse/utils/injectors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/invoke.py` & `greyhorse-0.4.2/greyhorse/utils/invoke.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,21 +26,27 @@
             return run_main(func(*args, **kwargs))
     elif callable(func):
         return func(*args, **kwargs)
     else:
         return func
 
 
-async def invoke_async[T, **P](func: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> T:
+async def invoke_async[T, **P](
+    func: Callable[P, T], to_thread: bool = False,
+    *args: P.args, **kwargs: P.kwargs,
+) -> T:
     if is_awaitable(func):
         if iscoroutine(func):
             return await func
         return await func(*args, **kwargs)
     elif callable(func):
-        return await asyncio.to_thread(func, *args, **kwargs)
+        if to_thread:
+            return await asyncio.to_thread(func, *args, **kwargs)
+        else:
+            return func(*args, **kwargs)
     else:
         future = Future()
         future.set_result(func)
         return future
 
 
 def caller_path(depth: int) -> list[str]:
```

### Comparing `greyhorse-0.4.1/greyhorse/utils/strings.py` & `greyhorse-0.4.2/greyhorse/utils/strings.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/greyhorse/utils/time.py` & `greyhorse-0.4.2/greyhorse/utils/time.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.1/pyproject.toml` & `greyhorse-0.4.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse"
-version = "0.4.1"
+version = "0.4.2"
 description = "Greyhorse library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -24,32 +24,22 @@
 pydantic = {version = "^2.0", extras = ["dotenv", "email"]}
 pytz = "^2023.0"
 timeparse-plus = "^1.2"
 tomlkit = "^0.11"
 orjson = "^3.8"
 
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
-requires = ["poetry-core", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
-build-backend = "poetry_dynamic_versioning.backend"
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-pattern = "default-unprefixed"
-style = "pep440"
-bump = true
-strict = false
-latest-tag = true
-dirty = false
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `greyhorse-0.4.1/PKG-INFO` & `greyhorse-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse
-Version: 0.4.1
+Version: 0.4.2
 Summary: Greyhorse library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
```

