# Comparing `tmp/fastapi_class-3.5.0.tar.gz` & `tmp/fastapi_class-3.6.0.tar.gz`

## Comparing `fastapi_class-3.5.0.tar` & `fastapi_class-3.6.0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/logger.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/openapi.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/routers.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/views.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/exception/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/fastapi_class/exception/handler.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/scripts/format.sh
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/scripts/lint.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/factory.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_exceptions.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_logger.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_metadata.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_openapi.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_routers.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/tests/test_views.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/LICENSE
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/README.md
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 fastapi_class-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/logger.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/openapi.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/routers.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/views.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/exception/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/fastapi_class/exception/handler.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/all.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/linting.in
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/linting.txt
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/testing.in
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/requirements/testing.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/scripts/clean.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/scripts/format.sh
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/scripts/lint.sh
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/scripts/requirements.sh
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/factory.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_logger.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_openapi.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_routers.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/tests/test_views.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/LICENSE
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/README.md
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 fastapi_class-3.6.0/PKG-INFO
```

### Comparing `fastapi_class-3.5.0/.github/workflows/ci.yml` & `fastapi_class-3.6.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,27 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install Dependencies
-        run: pip install -e .[lint]
-      - uses: pre-commit/action@v3.0.0
+
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
         with:
-          extra_args: --all-files --verbose
-      - name: Run mypy
+          uv-venv: ".venv"
+
+      - name: Install Dependencies
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/linting.txt
+
+      - name: Run Pre-commit
+        run: bash scripts/format.sh
+
+      - name: Run Mypy
         run: bash scripts/lint.sh
 
   tests:
 
     name: test py${{ matrix.python-version }} on ${{ matrix.os }}
 
     runs-on: ${{ matrix.os }}-latest
@@ -47,25 +54,35 @@
       - uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
+      - name: setup UV
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-venv: ".venv"
+
       - name: Install Dependencies
-        run: pip install -e .[test]
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt
 
       - name: Freeze Dependencies
-        run: pip freeze
+        run: uv pip freeze
 
-      - name: Test with pytest
+      - name: Test with pytest - ${{ matrix.os }} - py${{ matrix.python-version }}
         run: bash scripts/test.sh
+        env:
+          CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}-with-deps
 
-      - name: Upload coverage
+      - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          file: ./coverage.xml
 
   # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
   check:
     if: always()
     needs: [lint, tests]
     runs-on: ubuntu-latest
     steps:
```

### Comparing `fastapi_class-3.5.0/.github/workflows/release.yml` & `fastapi_class-3.6.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,14 @@
       - name: check GITHUB_REF matches package version
         uses: samuelcolvin/check-python-version@v4.1
         with:
           version_file_path: fastapi_class/__init__.py
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `fastapi_class-3.5.0/fastapi_class/__init__.py` & `fastapi_class-3.6.0/fastapi_class/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,21 @@
 
 @View(router)
 class ItemView:
 
     async def get(self, query: str = Query(), limit: int = 50, offset: int = 0):
         pass
 
-    def post(self, user: ItemModel):
+    async def post(self, user: ItemModel):
         pass
 ```
 
 """
 
-
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 
 from fastapi_class.exception import FormattedMessageException
 from fastapi_class.openapi import ExceptionModel, _exceptions_to_responses
 from fastapi_class.routers import Metadata, Method, endpoint
 from fastapi_class.views import View
 
 __all__ = [
```

### Comparing `fastapi_class-3.5.0/fastapi_class/openapi.py` & `fastapi_class-3.6.0/fastapi_class/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 
 def _exceptions_to_responses(
     exceptions: Iterable[HTTPException | Callable[..., HTTPException]],
 ):
     """
     Convert exceptions to responses.
 
-    :param exceptions: exceptions
-    :return: responses
-
-    :raise TypeError: if exception is not an instance of HTTPException or a factory function
-
-    :example:
+    ### example
     >>> from fastapi import HTTPException, status
     >>> from fastapi_class import _exceptions_to_responses
     >>> _exceptions_to_responses([HTTPException(status.HTTP_400_BAD_REQUEST, detail="Bad request")])
 
     Results:
 
     `{400: {'description': 'Bad request', 'model': <class 'fastapi_class.exceptions.ExceptionModel'>}}`
```

### Comparing `fastapi_class-3.5.0/fastapi_class/routers.py` & `fastapi_class-3.6.0/fastapi_class/routers.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,32 +7,43 @@
 from typing import Any, ClassVar
 
 from fastapi.responses import Response
 from pydantic import BaseModel
 
 
 class Method(str, Enum):
+    """
+    HTTP methods.
+    """
+
     GET = "get"
     POST = "post"
     PATCH = "patch"
     DELETE = "delete"
     PUT = "put"
 
 
 @dataclass(frozen=True, init=True, repr=True)
 class Metadata:
+    """
+    Metadata class, used to store endpoint metadata.
+    """
+
     methods: Iterable[str | Method]
     name: str | None = None
     path: str | None = None
     status_code: int | None = None
     response_model: type[BaseModel] | None = None
     response_class: type[Response] | None = None
     __default_method_suffix: ClassVar[str] = "_or_default"
 
     def __getattr__(self, __name: str) -> Any | Callable[[Any], Any]:
+        """
+        Dynamically return the value of the attribute.
+        """
         if __name.endswith(Metadata.__default_method_suffix):
             prefix = __name.replace(Metadata.__default_method_suffix, "")
             if hasattr(self, prefix):
                 return lambda _default: getattr(self, prefix, None) or _default
             return getattr(self, prefix)
         raise AttributeError(f"{self.__class__.__name__} has no attribute {__name}")
 
@@ -43,54 +54,47 @@
     name: str | None = None,
     path: str | None = None,
     status_code: int | None = None,
     response_model: type[BaseModel] | None = None,
     response_class: type[Response] | None = None,
 ):
     """
-    Endpoint decorator.
-
-    :param methods: methods
-    :param name: name
-    :param path: path
-    :param status_code: status code
-    :param response_model: response model
-    :param response_class: response class
-
-    :raise AssertionError: if response model or response class is not a subclass of BaseModel or Response respectively
-    :raise AssertionError: if methods is not an iterable of strings or Method enums
-
-    :example:
-    >>> from fastapi import FastAPI
-    >>> from fastapi_class import endpoint
-    >>> app = FastAPI()
-    >>> @endpoint()
-    ... def get():
-    ...     return {"message": "Hello, world!"}
-    >>> app.include_router(get)
+    Endpoint decorator for FastAPI.
 
-    Results:
-
-    `GET /get`
+    ### Example:
+        >>> from fastapi import FastAPI
+        >>> from fastapi_class import endpoint
+        >>> app = FastAPI()
+        >>> @endpoint()
+        ... async def get():
+        ...     return {"message": "Hello, world!"}
+        >>> app.include_router(get)
     """
     assert all(
         issubclass(_type, expected_type)
         for _type, expected_type in (
             (response_model, BaseModel),
             (response_class, Response),
         )
         if _type is not None
     ), "Response model and response class must be subclasses of BaseModel and Response respectively."
     assert (
         isinstance(methods, (Iterable, str)) or methods is None
     ), "Methods must be an string, iterable of strings or Method enums."
 
     def _decorator(function: Callable):
+        """
+        Decorate the function.
+        """
+
         @wraps(function)
         async def _wrapper(*args, **kwargs):
+            """
+            Wrapper for the function.
+            """
             return await function(*args, **kwargs)
 
         parsed_method = set()
         _methods = (
             (methods,)
             if isinstance(methods, str)
             else methods or ((name,) if name else (function.__name__,))
```

### Comparing `fastapi_class-3.5.0/fastapi_class/views.py` & `fastapi_class-3.6.0/fastapi_class/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from fastapi import APIRouter, FastAPI, HTTPException, status
 from fastapi.responses import JSONResponse
 
 from fastapi_class.openapi import _exceptions_to_responses
 from fastapi_class.routers import Metadata, Method
 
 COMMON_KEYWORD = "common"
-RESPONSE_MODEL_ATTRIBUTE_NAME = "RESPONSE_MODEL"
-RESPONSE_CLASS_ATTRIBUTE_NAME = "RESPONSE_CLASS"
-ENDPOINT_METADATA_ATTRIBUTE_NAME = "ENDPOINT_METADATA"
+RESPONSE_MODEL_ATTRIBUTE_NAME = "response_model"
+RESPONSE_CLASS_ATTRIBUTE_NAME = "response_class"
+ENDPOINT_METADATA_ATTRIBUTE_NAME = "__endpoint_metadata"
 EXCEPTIONS_ATTRIBUTE_NAME = "EXCEPTIONS"
 
 
 def _view_class_name_default_parser(cls: object, method: str):
     class_name = " ".join(re.findall(r"[A-Z][^A-Z]*", cls.__name__.replace("View", "")))  # type: ignore
     return f"{method.capitalize()} {class_name}"
 
@@ -25,36 +25,25 @@
     router: FastAPI | APIRouter,
     *,
     path: str = "/",
     default_status_code: int = status.HTTP_200_OK,
     name_parser: Callable[[object, str], str] = _view_class_name_default_parser,
 ):
     """
-    Class-based view decorator.
+    Class-based view decorator for FastAPI.
 
-    :param router: router
-    :param path: path
-    :param default_status_code: default status code
-    :param name_parser: name parser
-
-    :raise AssertionError: if router is not an instance of FastAPI or APIRouter
-
-    :example:
-    >>> from fastapi import FastAPI
-    >>> from fastapi_class import View
-    >>> app = FastAPI()
-    >>> @View(app)
-    ... class MyView:
-    ...     def get(self):
-    ...         return {"message": "Hello, world!"}
-    >>> app.include_router(MyView.router)
-
-    Results:
-
-    `GET /my-view`
+    ### Example:
+        >>> from fastapi import FastAPI
+        >>> from fastapi_class import View
+
+        >>> app = FastAPI()
+        >>> @View(app)
+        ... class MyView:
+        ...     async def get(self):
+        ...         return {"message": "Hello, world!"}
     """
 
     def _decorator(cls) -> None:
         obj = cls()
         cls_based_response_model = getattr(obj, RESPONSE_MODEL_ATTRIBUTE_NAME, {})
         cls_based_response_class = getattr(obj, RESPONSE_CLASS_ATTRIBUTE_NAME, {})
         common_exceptions = getattr(obj, EXCEPTIONS_ATTRIBUTE_NAME, {}).get(
```

### Comparing `fastapi_class-3.5.0/fastapi_class/exception/handler.py` & `fastapi_class-3.6.0/fastapi_class/exception/handler.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/scripts/clean.sh` & `fastapi_class-3.6.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/tests/test_exceptions.py` & `fastapi_class-3.6.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/tests/test_metadata.py` & `fastapi_class-3.6.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/tests/test_openapi.py` & `fastapi_class-3.6.0/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/tests/test_routers.py` & `fastapi_class-3.6.0/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/tests/test_views.py` & `fastapi_class-3.6.0/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,21 @@
         endpoints=None,
     ):
         data = data or {}
         methods = methods or []
         endpoints = endpoints or []
         for method in methods:
 
-            def dummy(self):
-                ...
+            def dummy(self): ...
 
             dummy.__name__ = method.value
             data[method.value] = dummy
         for _endpoint in endpoints:
 
-            def dummy(self):
-                ...
+            def dummy(self): ...
 
             data[_endpoint.get("alternative_name") or dummy.__name__] = _endpoint[
                 "decorator"
             ](dummy)
         class_base_view = type(name, (object,), data)
 
         return class_base_view
```

### Comparing `fastapi_class-3.5.0/.gitignore` & `fastapi_class-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/LICENSE` & `fastapi_class-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.5.0/README.md` & `fastapi_class-3.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,106 +37,100 @@
 `fastapi_class` provides a `class-based view` decorator `@View` to help reduce the amount of boilerplate necessary when developing related routes.
 
 > Highly inspired by [Fastapi-utils](https://fastapi-utils.davidmontague.xyz/user-guide/class-based-views/), Thanks to [@dmontagu](https://github.com/dmontagu) for the great work.
 
 - Example:
 
 ```python
-from fastapi import FastAPI, APIRouter, Query
+from fastapi import FastAPI, Query
 from pydantic import BaseModel
 from fastapi_class import View
 
 app = FastAPI()
-router = APIRouter()
 
 class ItemModel(BaseModel):
     id: int
     name: str
     description: str = None
 
-@View(router)
+@View(app)
 class ItemView:
-    def post(self, item: ItemModel):
+    async def post(self, item: ItemModel):
         return item
 
-    def get(self, item_id: int = Query(..., gt=0)):
+    async def get(self, item_id: int = Query(..., gt=0)):
         return {"item_id": item_id}
 
-app.include_router(router)
 ```
 
 ### Response model 📦
 
 `Exception` in list need to be either function that return `fastapi.HTTPException` itself. In case of a function it is required to have all of it's arguments to be `optional`.
 
 ```py
-from fastapi import FastAPI, APIRouter, HTTPException, status
+from fastapi import FastAPI, HTTPException, status
 from fastapi.responses import PlainTextResponse
 from pydantic import BaseModel
 
 from fastapi_class import View
 
 app = FastAPI()
-router = APIRouter()
 
 NOT_AUTHORIZED = HTTPException(401, "Not authorized.")
 NOT_ALLOWED = HTTPException(405, "Method not allowed.")
 NOT_FOUND = lambda item_id="item_id": HTTPException(404, f"Item with {item_id} not found.")
 
 class ItemResponse(BaseModel):
     field: str | None = None
 
-@View(router)
+@View(app)
 class MyView:
     exceptions = {
         "__all__": [NOT_AUTHORIZED],
         "put": [NOT_ALLOWED, NOT_FOUND]
     }
 
     RESPONSE_MODEL = {
         "put": ItemResponse
     }
 
     RESPONSE_CLASS = {
         "delete": PlainTextResponse
     }
 
-    def get(self):
+    async def get(self):
         ...
 
-    def put(self):
+    async def put(self):
         ...
 
-    def delete(self):
+    async def delete(self):
         ...
-
-app.include_router(router)
 ```
 
 ### Customized Endpoints
 
 ```py
-from fastapi import FastAPI, APIRouter, HTTPException
+from fastapi import FastAPI, HTTPException
 from fastapi.responses import PlainTextResponse
 from pydantic import BaseModel
 
 from fastapi_class import View, endpoint
 
 app = FastAPI()
-router = APIRouter()
 
 NOT_AUTHORIZED = HTTPException(401, "Not authorized.")
 NOT_ALLOWED = HTTPException(405, "Method not allowed.")
 NOT_FOUND = lambda item_id="item_id": HTTPException(404, f"Item with {item_id} not found.")
 EXCEPTION = HTTPException(400, "Example.")
 
 class UserResponse(BaseModel):
     field: str | None = None
 
-@View(router)
+@View(app)
 class MyView:
     exceptions = {
         "__all__": [NOT_AUTHORIZED],
         "put": [NOT_ALLOWED, NOT_FOUND],
         "edit": [EXCEPTION]
     }
 
@@ -145,25 +139,25 @@
         "edit": UserResponse
     }
 
     RESPONSE_CLASS = {
         "delete": PlainTextResponse
     }
 
-    def get(self):
+    async def get(self):
         ...
 
-    def put(self):
+    async def put(self):
         ...
 
-    def delete(self):
+    async def delete(self):
         ...
 
-    @endpoint(("PUT",), path="edit")
-    def edit(self):
+    @endpoint(("PUT"), path="edit")
+    async def edit(self):
         ...
 ```
 
 **Note:** The `edit()` endpoint is decorated with the `@endpoint(("PUT",), path="edit")` decorator, which specifies that this endpoint should handle `PUT` requests to the `/edit` path,
 using `@endpoint("PUT", path="edit")` has the same effect
 
 ## Development 🚧
@@ -178,17 +172,25 @@
 
 ```bash
 source venv/bin/activate
 ```
 
 And then install the development dependencies:
 
+__Note:__ You should have `uv` installed, if not you can install it with:
+
+```bash
+pip install uv
+```
+
+Then you can install the dependencies with:
+
 ```bash
 # Install dependencies
-pip install -e .[test,lint]
+uv pip install -r requirements/all.txt
 ```
 
 ### Run tests 🌝
 
 You can run all the tests with:
 
 ```bash
```

### Comparing `fastapi_class-3.5.0/pyproject.toml` & `fastapi_class-3.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -21,49 +21,37 @@
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
+    "Framework :: Pydantic :: 2",
     "Framework :: AsyncIO",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<3.0.0",
-    "fastapi >=0.65.2,<0.109.3",
+    "fastapi >=0.100.0,<0.120.0",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/yezz123/fastapi-class"
 Funding = 'https://github.com/sponsors/yezz123'
 
-[project.optional-dependencies]
-lint = [
-    "pre-commit==3.6.0",
-    "mypy==1.8.0",
-]
-test = [
-    "requests==2.31.0",
-    "pytest==7.4.4",
-    "pytest-asyncio == 0.23.4",
-    "pytest-cov==4.1.0",
-    "pytest-pretty==1.2.0",
-]
 
 [tool.hatch.version]
 path = "fastapi_class/__init__.py"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["pydantic", "typing_extensions"]
@@ -92,14 +80,25 @@
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [tool.mypy]
 plugins = "pydantic.mypy"
 follow_imports = "silent"
 
+[tool.coverage.run]
+source = ["fastapi_class"]
+branch = true
+context = '${CONTEXT}'
+
+[tool.coverage.paths]
+source = [
+    'fastapi_class/',
+    '/Users/runner/work/fastapi_class/fastapi_class/fastapi_class/',
+    'D:\a\fastapi_class\fastapi_class\fastapi_class',
+]
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
     "raise NotImplemented",
```

### Comparing `fastapi_class-3.5.0/PKG-INFO` & `fastapi_class-3.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_class
-Version: 3.5.0
+Version: 3.6.0
 Summary: Simplifies class-based views for more organized and maintainable code in FastAPI.
 Project-URL: Homepage, https://github.com/yezz123/fastapi-class
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: FastAPI,MVC,class-based,class-based-views,pydantic
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: fastapi<0.109.3,>=0.65.2
-Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<3.0.0,>=1.6.2
-Provides-Extra: lint
-Requires-Dist: mypy==1.8.0; extra == 'lint'
-Requires-Dist: pre-commit==3.6.0; extra == 'lint'
-Provides-Extra: test
-Requires-Dist: pytest-asyncio==0.23.4; extra == 'test'
-Requires-Dist: pytest-cov==4.1.0; extra == 'test'
-Requires-Dist: pytest-pretty==1.2.0; extra == 'test'
-Requires-Dist: pytest==7.4.4; extra == 'test'
-Requires-Dist: requests==2.31.0; extra == 'test'
+Requires-Dist: fastapi<0.120.0,>=0.100.0
 Description-Content-Type: text/markdown
 
 ![Class](https://user-images.githubusercontent.com/52716203/137606695-f110f129-08b1-45f3-a445-962c1f28378c.png)
 
 <p align="center">
     <em>Classes and Decorators to use FastAPI with Class based routing</em>
 </p>
@@ -76,106 +67,100 @@
 `fastapi_class` provides a `class-based view` decorator `@View` to help reduce the amount of boilerplate necessary when developing related routes.
 
 > Highly inspired by [Fastapi-utils](https://fastapi-utils.davidmontague.xyz/user-guide/class-based-views/), Thanks to [@dmontagu](https://github.com/dmontagu) for the great work.
 
 - Example:
 
 ```python
-from fastapi import FastAPI, APIRouter, Query
+from fastapi import FastAPI, Query
 from pydantic import BaseModel
 from fastapi_class import View
 
 app = FastAPI()
-router = APIRouter()
 
 class ItemModel(BaseModel):
     id: int
     name: str
     description: str = None
 
-@View(router)
+@View(app)
 class ItemView:
-    def post(self, item: ItemModel):
+    async def post(self, item: ItemModel):
         return item
 
-    def get(self, item_id: int = Query(..., gt=0)):
+    async def get(self, item_id: int = Query(..., gt=0)):
         return {"item_id": item_id}
 
-app.include_router(router)
 ```
 
 ### Response model 📦
 
 `Exception` in list need to be either function that return `fastapi.HTTPException` itself. In case of a function it is required to have all of it's arguments to be `optional`.
 
 ```py
-from fastapi import FastAPI, APIRouter, HTTPException, status
+from fastapi import FastAPI, HTTPException, status
 from fastapi.responses import PlainTextResponse
 from pydantic import BaseModel
 
 from fastapi_class import View
 
 app = FastAPI()
-router = APIRouter()
 
 NOT_AUTHORIZED = HTTPException(401, "Not authorized.")
 NOT_ALLOWED = HTTPException(405, "Method not allowed.")
 NOT_FOUND = lambda item_id="item_id": HTTPException(404, f"Item with {item_id} not found.")
 
 class ItemResponse(BaseModel):
     field: str | None = None
 
-@View(router)
+@View(app)
 class MyView:
     exceptions = {
         "__all__": [NOT_AUTHORIZED],
         "put": [NOT_ALLOWED, NOT_FOUND]
     }
 
     RESPONSE_MODEL = {
         "put": ItemResponse
     }
 
     RESPONSE_CLASS = {
         "delete": PlainTextResponse
     }
 
-    def get(self):
+    async def get(self):
         ...
 
-    def put(self):
+    async def put(self):
         ...
 
-    def delete(self):
+    async def delete(self):
         ...
-
-app.include_router(router)
 ```
 
 ### Customized Endpoints
 
 ```py
-from fastapi import FastAPI, APIRouter, HTTPException
+from fastapi import FastAPI, HTTPException
 from fastapi.responses import PlainTextResponse
 from pydantic import BaseModel
 
 from fastapi_class import View, endpoint
 
 app = FastAPI()
-router = APIRouter()
 
 NOT_AUTHORIZED = HTTPException(401, "Not authorized.")
 NOT_ALLOWED = HTTPException(405, "Method not allowed.")
 NOT_FOUND = lambda item_id="item_id": HTTPException(404, f"Item with {item_id} not found.")
 EXCEPTION = HTTPException(400, "Example.")
 
 class UserResponse(BaseModel):
     field: str | None = None
 
-@View(router)
+@View(app)
 class MyView:
     exceptions = {
         "__all__": [NOT_AUTHORIZED],
         "put": [NOT_ALLOWED, NOT_FOUND],
         "edit": [EXCEPTION]
     }
 
@@ -184,25 +169,25 @@
         "edit": UserResponse
     }
 
     RESPONSE_CLASS = {
         "delete": PlainTextResponse
     }
 
-    def get(self):
+    async def get(self):
         ...
 
-    def put(self):
+    async def put(self):
         ...
 
-    def delete(self):
+    async def delete(self):
         ...
 
-    @endpoint(("PUT",), path="edit")
-    def edit(self):
+    @endpoint(("PUT"), path="edit")
+    async def edit(self):
         ...
 ```
 
 **Note:** The `edit()` endpoint is decorated with the `@endpoint(("PUT",), path="edit")` decorator, which specifies that this endpoint should handle `PUT` requests to the `/edit` path,
 using `@endpoint("PUT", path="edit")` has the same effect
 
 ## Development 🚧
@@ -217,17 +202,25 @@
 
 ```bash
 source venv/bin/activate
 ```
 
 And then install the development dependencies:
 
+__Note:__ You should have `uv` installed, if not you can install it with:
+
+```bash
+pip install uv
+```
+
+Then you can install the dependencies with:
+
 ```bash
 # Install dependencies
-pip install -e .[test,lint]
+uv pip install -r requirements/all.txt
 ```
 
 ### Run tests 🌝
 
 You can run all the tests with:
 
 ```bash
```

