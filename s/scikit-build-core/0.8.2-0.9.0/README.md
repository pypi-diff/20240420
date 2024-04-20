# Comparing `tmp/scikit_build_core-0.8.2.tar.gz` & `tmp/scikit_build_core-0.9.0.tar.gz`

## Comparing `scikit_build_core-0.8.2.tar` & `scikit_build_core-0.9.0.tar`

### file list

```diff
@@ -1,316 +1,331 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.gitattributes
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.packit.yaml
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.readthedocs.yml
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/noxfile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/.fmf/version
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/plans/examples.fmf
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/plans/rpminspect.fmf
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0    10063 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/codecov.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/build.md
--rw-r--r--   0        0        0    27711 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/changelog.md
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/cmakelists.md
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/conf.py
--rw-r--r--   0        0        0    19503 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/configuration.md
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/crosscompile.md
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/faqs.md
--rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/getting_started.md
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/index.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/man.md
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/migration_guide.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/.fmf/version
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/main.fmf
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/test.sh
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/main.fmf
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/main.fmf
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/main.fmf
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/abi3/main.fmf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/c/main.fmf
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/cython/main.fmf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/fortran/main.fmf
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/nanobind/example.cpp
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/nanobind/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/nanobind/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/pybind11/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/swig/main.fmf
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/docs/ext/conftabs.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_editable.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/generate.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    14526 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/__main__.py
--rw-r--r--   0        0        0     8604 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/metadata/regex.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/scikit-build.schema.json
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/documentation.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/json_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_docs.py
--rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0    13610 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_schema.py
--rw-r--r--   0        0        0    21745 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/constraints.txt
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_builder.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_cmake_config.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_custom_modules.py
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_editable.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_editable_redirect.py
--rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_editable_unit.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_file_processor.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_fileapi.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_generator_default.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_get_requires.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_json_schema.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_printouts.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_pyproject_purelib.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_schema.py
--rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_settings.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_settings_overrides.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_shutil.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_simplest_c.py
--rw-r--r--   0        0        0    18917 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/CMakeLists.txt
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/pyproject.toml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/python/shared_pkg/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/python/shared_pkg/py_module.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/src/shared_pkg/c_module.c
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/sdist_config/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/sdist_config/CMakeLists.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/sdist_config/input.cmake
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/sdist_config/main.cpp
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/sdist_config/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_purelib_package/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/LICENSE
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/README.md
--rw-r--r--   0        0        0    10982 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 scikit_build_core-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.gitattributes
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.packit.yaml
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/.fmf/version
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/plans/examples.fmf
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/plans/rpminspect.fmf
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/codecov.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/build.md
+-rw-r--r--   0        0        0    30046 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/cmakelists.md
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0    19684 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/configuration.md
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/crosscompile.md
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/faqs.md
+-rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/getting_started.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/man.md
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/migration_guide.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/.fmf/version
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.hatch.rst
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/test.sh
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/main.fmf
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/main.fmf
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/main.fmf
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/nanobind/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/ext/conftabs.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/plugins/hatchling.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/docs/plugins/setuptools.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_editable.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/generate.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/metadata.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/__main__.py
+-rw-r--r--   0        0        0     8604 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/hatch/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/hatch/hooks.py
+-rw-r--r--   0        0        0    10696 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/hatch/plugin.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/metadata/regex.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0    20596 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/documentation.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/json_schema.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_docs.py
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_schema.py
+-rw-r--r--   0        0        0    21975 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/constraints.txt
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_builder.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_editable.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_editable_redirect.py
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_editable_unit.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_generator_default.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_get_requires.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_hatchling.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_json_schema.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_logging.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_name_main.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_printouts.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_pyproject_purelib.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_schema.py
+-rw-r--r--   0        0        0    19424 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_settings.py
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_settings_overrides.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_shutil.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    18913 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/.gitignore
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/pyproject.toml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/cpp/example.cpp
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/src/hatchling_example/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/hatchling/src/hatchling_example/_core.pyi
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/CMakeLists.txt
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/pyproject.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/python/shared_pkg/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/python/shared_pkg/py_module.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/src/shared_pkg/c_module.c
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/sdist_config/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/sdist_config/CMakeLists.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/sdist_config/input.cmake
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/sdist_config/main.cpp
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/sdist_config/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_purelib_package/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/README.md
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    19706 2020-02-02 00:00:00.000000 scikit_build_core-0.9.0/PKG-INFO
```

### Comparing `scikit_build_core-0.8.2/.packit.yaml` & `scikit_build_core-0.9.0/.packit.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -24,51 +24,46 @@
     dest: plans/main.fmf
 upstream_package_name: scikit_build_core
 downstream_package_name: python-scikit-build-core
 update_release: false
 upstream_tag_template: v{version}
 
 jobs:
-  - job: copr_build
-    trigger: pull_request
+  - &copr_build
+    job: copr_build
+    trigger: release
     owner: "@scikit-build"
-    project: scikit-build-core
-    update_release: true
-    release_suffix: "{PACKIT_RPMSPEC_RELEASE}"
-    targets:
-      - fedora-all-x86_64
-      - fedora-all-aarch64
-  - job: tests
-    trigger: pull_request
-    targets:
-      - fedora-all-x86_64
-      - fedora-all-aarch64
+    project: release
+    # Drop F38 due to dependency
+    targets: &targets
+      - fedora-latest-x86_64
+      - fedora-latest-aarch64
+      - fedora-latest-stable-x86_64
+      - fedora-latest-stable-aarch64
+      - fedora-development-x86_64
+      - fedora-development-aarch64
+  - &tests
+    job: tests
+    trigger: release
+    targets: *targets
     fmf_path: .distro
-  - job: copr_build
+  - <<: *copr_build
     trigger: commit
     branch: main
-    owner: "@scikit-build"
     project: nightly
-    targets:
-      - fedora-all-x86_64
-      - fedora-all-aarch64
-  - job: tests
+  - <<: *tests
     trigger: commit
     branch: main
-    targets:
-      - fedora-all-x86_64
-      - fedora-all-aarch64
-    fmf_path: .distro
-  - job: copr_build
-    trigger: release
-    owner: "@scikit-build"
-    project: release
-    targets:
-      - fedora-all-x86_64
-      - fedora-all-aarch64
+  - <<: *copr_build
+    trigger: pull_request
+    project: scikit-build-core
+    update_release: true
+    release_suffix: "{PACKIT_RPMSPEC_RELEASE}"
+  - <<: *tests
+    trigger: pull_request
   - job: propose_downstream
     trigger: release
     dist_git_branches:
       # TODO: Switch to fedora-development and fedora-latest
       # There is an issue that the commits diverge on different PRs. In the meantime will create PRs on branched fedora
       # manually
       # https://github.com/packit/packit/issues/1724
```

### Comparing `scikit_build_core-0.8.2/.pre-commit-config.yaml` & `scikit_build_core-0.9.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 ci:
   autoupdate_commit_msg: "chore(deps): update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
+exclude: ^src/scikit_build_core/_vendor
+
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -18,15 +20,15 @@
         args: ["--pytest-test-first"]
         exclude: "^tests/packages/"
       - id: requirements-txt-fixer
       - id: trailing-whitespace
         exclude: "^tests"
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.7
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
@@ -52,15 +54,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests|src/scikit_build_core/resources/scikit-build.schema.json"
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         exclude: |
           (?x)^(
             tests/packages/simplest_c/src/simplest/__init__.py|
             tests/packages/dynamic_metadata/src/dynamic/__init__.py|
             tests/packages/.*/setup.py
@@ -75,20 +77,19 @@
           - hatch-fancy-pypi-readme>=24
           - importlib-metadata>=6.6.0
           - importlib-resources
           - markdown-it-py<3 # Python 3.7 compat needed for mypy check
           - ninja
           - nox
           - packaging
-          - pyproject_metadata
           - pytest<8
           - rich
           - setuptools-scm
           - tomli
-          - types-setuptools>=67.8
+          - types-setuptools>=69.2
 
   - repo: https://github.com/henryiii/check-sdist
     rev: "v0.1.3"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
@@ -98,15 +99,15 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         exclude: ^(LICENSE$|src/scikit_build_core/resources/find_python|tests/test_skbuild_settings.py$)
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.6
+    rev: v0.10.0.1
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
```

### Comparing `scikit_build_core-0.8.2/noxfile.py` & `scikit_build_core-0.9.0/noxfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import TYPE_CHECKING
 
 import nox
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
+nox.needs_version = ">=2024.3.2"
+nox.options.default_venv_backend = "uv|virtualenv"
+
 DIR = Path(__file__).parent.resolve()
 
 nox.options.sessions = [
     "lint",
     "pylint",
     "generate_schema",
     "readme",
@@ -50,28 +53,28 @@
     install_args: Sequence[str] = (),
     run_args: Sequence[str] = (),
     extras: Sequence[str] = (),
 ) -> None:
     posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
 
-    _install_args = list(install_args)
     # This will not work if system CMake is too old (<3.15)
     if shutil.which("cmake") is None and shutil.which("cmake3") is None:
-        _install_args.append("cmake")
+        session.install("cmake")
     if shutil.which("ninja") is None:
-        _install_args.append("ninja")
+        session.install("ninja")
 
     _extras = ["test", *extras]
     if "--cov" in posargs:
         _extras.append("cov")
         posargs.append("--cov-config=pyproject.toml")
 
     install_arg = f"-e.[{','.join(_extras)}]"
     session.install(install_arg, *install_args)
+    session.run("pip", "list")
     session.run("pytest", *run_args, *posargs, env=env)
 
 
 @nox.session(reuse_venv=True)
 def generate_schema(session: nox.Session) -> None:
     """
     (Re)generate src/scikit_build_core/resources/scikit-build.schema.json from model.
@@ -86,15 +89,15 @@
 
 
 @nox.session
 def tests(session: nox.Session) -> None:
     """
     Run the unit and regular tests. Includes coverage if --cov passed.
     """
-    _run_tests(session, extras=["test-meta,test-numpy,test-schema"])
+    _run_tests(session, extras=["test-meta,test-numpy,test-schema,test-hatchling"])
 
 
 @nox.session(reuse_venv=True)
 def readme(session: nox.Session) -> None:
     """
     Update the readme with cog. Pass --check to check instead.
     """
@@ -116,50 +119,40 @@
         run_args=["-Wdefault"],
     )
 
 
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links.
+    Build the docs. Use "--non-interactive" to avoid serving. Pass "-b linkcheck" to check links.
     """
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("--serve", action="store_true", help="Serve after building")
     parser.add_argument(
         "-b", dest="builder", default="html", help="Build target (default: html)"
     )
     args, posargs = parser.parse_known_args(session.posargs)
 
-    if args.builder != "html" and args.serve:
-        session.error("Must not specify non-HTML builder with --serve")
-
-    extra_installs = ["sphinx-autobuild"] if args.serve else []
+    serve = args.builder == "html" and session.interactive
+    extra_installs = ["sphinx-autobuild"] if serve else []
+    session.install("-e.[docs]", *extra_installs)
 
-    session.install("-e.[docs,pyproject]", *extra_installs)
-    session.run("pip", "list")
     session.chdir("docs")
 
-    if args.builder == "linkcheck":
-        session.run(
-            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
-        )
-        return
-
     shared_args = (
         "-n",  # nitpicky mode
         "-T",  # full tracebacks
         f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
-    if args.serve:
-        session.run("sphinx-autobuild", *shared_args)
+    if serve:
+        session.run("sphinx-autobuild", "--open-browser", *shared_args)
     else:
         session.run("sphinx-build", "--keep-going", *shared_args)
 
 
 @nox.session
 def build_api_docs(session: nox.Session) -> None:
     """
@@ -232,15 +225,15 @@
     parser.add_argument("-c", dest="code", help="Run some Python code")
     args, remaining = parser.parse_known_args(session.posargs)
 
     tmp_dir = Path(session.create_tmp())
     proj_dir = tmp_dir / "_".join(args.project.split("/"))
 
     session.install("build", "hatch-vcs", "hatchling")
-    session.install(".[pyproject]", "--no-build-isolation")
+    session.install(".", "--no-build-isolation")
 
     if proj_dir.is_dir():
         session.chdir(proj_dir)
         session.run("git", "pull", external=True)
     else:
         session.run(
             "git",
@@ -285,7 +278,33 @@
             ".",
         )
         if args.code:
             session.error("Must use editable install for code at the moment")
 
     if args.code:
         session.run("python", "-c", args.code)
+
+
+@nox.session(venv_backend="none")
+def vendor_pyproject_metadata(session: nox.Session) -> None:
+    """
+    Vendor pyproject.toml metadata.
+    """
+
+    parser = argparse.ArgumentParser(
+        prog=f"{Path(sys.argv[0]).name} -s vendor_pyproject_metadata"
+    )
+    parser.add_argument("version", help="A tag or ref to vendor")
+    args = parser.parse_args(session.posargs)
+
+    session.run(
+        "curl",
+        "-o",
+        "src/scikit_build_core/_vendor/pyproject_metadata/__init__.py",
+        f"https://raw.githubusercontent.com/pypa/pyproject-metadata/{args.version}/pyproject_metadata/__init__.py",
+    )
+    session.run(
+        "curl",
+        "-o",
+        "src/scikit_build_core/_vendor/pyproject_metadata/LICENSE",
+        f"https://raw.githubusercontent.com/pypa/pyproject-metadata/{args.version}/LICENSE",
+    )
```

### Comparing `scikit_build_core-0.8.2/.github/CONTRIBUTING.md` & `scikit_build_core-0.9.0/.github/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,24 @@
 This section covers the design of scikit-build-core.
 
 Included modules:
 
 - `.cmake`: `CMake`/`CMaker` general interface for building code
 - `.fileapi`: Interface for reading the CMake File API
 - `.builder`: Generalized backend builder and related helpers
+- `.settings`: The configuration system, reading from pyproject.toml, PEP 517
+
+The build backend and plugins:
+
 - `.build`: PEP 517 builder
-- `.setuptools`: The setuptools Extension interface (and PEP 517 hooks)
+- `.setuptools`: The setuptools Extension interface (and PEP 517 hooks) (will
+  likely be split out)
 - `.setuptools.build_api`: Wrapper injecting build requirements
-- `.settings`: The configuration system, reading from pyproject.toml, PEP 517
-  config, and envvars
+- `.hatch`: The hatchling extension (will likely be split out) config, and
+  envvars
 
 ## Basic CMake usage
 
 ```python
 from packaging.specifiers import SpecifierSet
 from scikit_build_core.cmake import CMake, CMaker
 
@@ -299,15 +304,16 @@
 ```
 
 ## Patterns
 
 ### Backports
 
 All backported standard library code is in `scikit_build_core._compat`, in a
-module with the stdlib name.
+module with the stdlib name. Ruff will ensure you use the backport instead of
+the original module.
 
 ### Detecting the platform
 
 Here are some common platforms and the reported values:
 
 | OS      | Compiler   | `sys.platform` | `sysconfig.get_platform()`   |
 | ------- | ---------- | -------------- | ---------------------------- |
```

### Comparing `scikit_build_core-0.8.2/.github/matchers/pylint.json` & `scikit_build_core-0.9.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/.github/workflows/cd.yml` & `scikit_build_core-0.9.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/.github/workflows/ci.yml` & `scikit_build_core-0.9.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -93,15 +93,32 @@
       - uses: actions/checkout@v4
 
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
 
-      - name: Install package
+      - uses: yezz123/setup-uv@v4
+        if:
+          matrix.python-version != '3.7' && matrix.python-version != 'pypy-3.8'
+          && matrix.python-version != 'pypy-3.7'
+
+      - name: Install package (uv)
+        if:
+          matrix.python-version != '3.7' && matrix.python-version != 'pypy-3.8'
+          && matrix.python-version != 'pypy-3.7'
+        run:
+          uv pip install
+          -e.[test,test-meta,test-numpy,test-schema,test-hatchling,wheels,cov]
+          --system
+
+      - name: Install package (pip)
+        if:
+          matrix.python-version == '3.7' || matrix.python-version == 'pypy-3.8'
+          || matrix.python-version == 'pypy-3.7'
         run: pip install -e.[test,test-meta,test-numpy,test-schema,wheels,cov]
 
       - name: Test package
         run: >-
           pytest -ra --showlocals --cov --cov-report=xml --cov-report=term
           --durations=20
 
@@ -132,16 +149,29 @@
           python-version: ${{ matrix.python-version }}
 
       # The min requirements are not compatible with some of the extra test
       # deps, so limit to just built-in deps.
       - name: Min requirements
         run: pip install --constraint tests/constraints.txt .[test] ninja
 
-      - name: Setup CMake ${{ matrix.cmake-version }}
+      - name: Setup CMake 3.15
         uses: jwlawson/actions-setup-cmake@v2.0
+        if: runner.os != 'Windows'
+        with:
+          cmake-version: "3.15.x"
+
+        # First version to support VS 17.0
+      - name: Setup CMake 3.21
+        uses: jwlawson/actions-setup-cmake@v2.0
+        if: runner.os == 'Windows'
+        with:
+          cmake-version: "3.21.x"
+
+      - name: Show installed packages
+        run: pip list
 
       - name: Test min package
         run: pytest -ra --showlocals -Wdefault
 
   cygwin:
     name: Tests on 🐍 3.9 • cygwin
     runs-on: windows-latest
@@ -251,15 +281,17 @@
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.runs-on }}
     timeout-minutes: 15
 
     steps:
       - uses: actions/checkout@v4
 
-      - uses: wntrblm/nox@2023.04.22
+      - uses: yezz123/setup-uv@v4
+
+      - uses: wntrblm/nox@2024.03.02
         with:
           python-versions: "3.11"
 
       - name: Linkcheck
         run: nox -s docs -- -b linkcheck
 
       - name: Manpage
```

### Comparing `scikit_build_core-0.8.2/docs/build.md` & `scikit_build_core-0.9.0/docs/build.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/changelog.md` & `scikit_build_core-0.9.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,67 @@
 # Changelog
 
+## Version 0.9.0
+
+This version adds the ability to `inherit` in override tables, matching a
+similar feature added to cibuildwheel 2.17's overrides. You can now write out
+extra metadata to `@{SKBUILD_METADATA_DIR}`. A new Hatchling plugin is provided
+as an experimental feature (will likely be made a separate package in the future
+like the setuptools plugin).
+
+The meaning of `wheel.exclude` has been changed to match on the wheel path,
+rather than the source path. We could not find any projects that would be
+affected by this change, so it was not added to the minimum-version protection
+policy. This now allows you to ignore CMake outputs as well.
+
+Features:
+
+- Preserve additivity of `cmake.define` across `overrides` tables by @stubbiali
+  in #564
+- Add metadata dir access by @henryiii in #702
+- Experimental hatchling builder by @henryiii and @aryamanjeendgar in #637
+- Vendor pyproject-metadata by @henryiii in #703
+- Always require pathspec by @henryiii in #711
+
+Fixes:
+
+- Exclude installed files if listed in exclude by @henryiii in #652
+- Make `.git_archival.txt` reproducible by @LecrisUT in #706
+- Use `cmake -E` capabilities instead of `cmake --version` by @KyleFromNVIDIA in
+  #675
+- Ensure many/musl tags not selected by @henryiii in #698
+- purelib should set py3 tag if unset by @henryiii in #661
+- Validate description for 0.9+ by @henryiii in #709
+- Support bools in config settings by @henryiii in #712
+
+API changes:
+
+- `extra_settings` for SettingsReader by @henryiii in #697
+- `GetRequires` args changed by @henryiii in #699
+- Make `from_file` a little more powerful by @henryiii in #700
+- Metadata is part of the build backend by @henryiii in #708
+
+Documentation:
+
+- `cmakelists.md` Windows `SOABI` suffix variable by @thewtex in #684
+- Fix hatch init command by @thewtex in #677
+- Fix install strip default by @henryiii in #681
+- Improve `ninja.make-fallback` description in the README by @thewtex in #676
+- Mention printouts by @henryiii in #660
+
+CI and testing:
+
+- Lower `pybind11` test dependency by @LecrisUT in #691
+- Some cleanup from uv branch by @henryiii in #686
+- Fedora CI maintenance by @LecrisUT in #689
+- Small additions by @henryiii in #694
+- Some changes from uv job by @henryiii in #693
+- Fix setuptools on Python 3.12 by @henryiii in #701
+- Fedora: Port downstream PR-49 by @LecrisUT in #678
+
 ## Version 0.8.2
 
 This version fixes a few small issues related to configuration. The wheel tag is
 fixed when `wheel.platlib` is False, inplace editable installs ignore
 `build-dir`, and `install-dir` no longer affects the generate path.
 
 Fixes:
```

### Comparing `scikit_build_core-0.8.2/docs/cmakelists.md` & `scikit_build_core-0.9.0/docs/cmakelists.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,31 @@
 as that include "Embed" component, which is not always present and is not
 related to making Python extension modules.
 
 If you are making a Limited ABI / Stable API package, you'll need the
 `Development.SABIModule` component instead. You can use the
 `SKBUILD_LIMITED_API` variable to check to see if it was requested.
 
+<!-- prettier-ignore-start -->
 :::{warning}
+:name: soabi
 
 If you want to cross-compile to Windows ARM, you'll need to use
 `${SKBUILD_SOABI}`, which is always correct, instead of trusting FindPython's
 `Python_SOABI` value. You can manually set the extension suffix after making a
 target:
 
 ```cmake
 if(CMAKE_SYSTEM_NAME STREQUAL "Windows")
-    set_property (TARGET ${name} PROPERTY SUFFIX "$.{SKBUILD_SOSABI}.pyd")
+    set_property (TARGET ${name} PROPERTY SUFFIX ".${SKBUILD_SOSABI}.pyd")
 else()
     set_property (TARGET ${name} PROPERTY SUFFIX ".${SKBUILD_SOSABI}${CMAKE_SHARED_MODULE_SUFFIX}")
 endif()
 ```
+<!-- prettier-ignore-end -->
 
 A quicker way to do this would be to instead override `Python_SOABI` after
 `find_package(Python)`:
 
 ```cmake
 set(Python_SOABI ${SKBUILD_SOABI})
 ```
@@ -99,14 +102,18 @@
   directly to site-packages when a wheel is installed.
 - `${SKBUILD_DATA_DIR}`: The data directory. Anything here goes to the root of
   the environment when a wheel is installed (use with care).
 - `${SKBUILD_HEADERS_DIR}`: The header directory. Anything in here gets
   installed to Python's header directory.
 - `${SKBUILD_SCRIPTS_DIR}`: The scripts directory. Anything placed in here will
   go to `bin` (Unix) or `Scripts` (Windows).
+- `${SKBUILD_METADATA_DIR}`: The dist-info directory. Licenses go in the
+  `licenses` subdirectory. _Note that CMake is not run in the
+  `prepare_metadata_\*` hooks, so anything written to this directory will only
+  be present when writing wheels.\_
 - `${SKBUILD_NULL_DIR}`: Anything installed here will not be placed in the
   wheel.
 
 ## Limited API / Stable ABI
 
 You can activate the limited ABI by setting When you do that,
 `${SKBUILD_SABI_COMPONENT}` will be set to `Development.SABIModule` if you can
```

### Comparing `scikit_build_core-0.8.2/docs/conf.py` & `scikit_build_core-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,21 +92,22 @@
 ]
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "packaging": ("https://packaging.pypa.io/en/stable", None),
     "setuptools": ("https://setuptools.pypa.io/en/latest", None),
-    "pyproject_metadata": ("https://pep621.readthedocs.io/en/latest", None),
+    "hatchling": ("https://hatch.pypa.io/latest", None),
 }
 
 nitpick_ignore = [
     ("py:class", "setuptools.dist.Distribution"),
     ("py:class", "T"),
     ("py:class", "scikit_build_core.settings.sources.T"),
+    ("py:class", "scikit_build_core._vendor.pyproject_metadata.StandardMetadata"),
 ]
 
 linkcheck_anchors_ignore = [
     # This seems to be broken on GitHub readmes
     "default-versioning-scheme",
     "git-archives",
 ]
```

### Comparing `scikit_build_core-0.8.2/docs/configuration.md` & `scikit_build_core-0.9.0/docs/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Configuration
 
 Scikit-build-core supports a powerful unified configuration system. Every option
 in scikit-build-core can be specified in one of three ways: as a
 `pyproject.toml` option (preferred if static), as a config-settings options
 (preferred if dynamic), or as an environment variable.
 
+(verbosity)=
+
 ## Verbosity
 
 You can increase the verbosity of the build with two settings - `cmake.verbose`
 is a shortcut for verbose build output, and logging.level controls
 scikit-build-core's internal logging. An example (with all configuration styles)
 of setting both is:
 
@@ -178,28 +180,28 @@
 
 If you do this, you'll want to have some artifact from the configure in your
 source directory; for example:
 
 ```cmake
 include(FetchContent)
 
+set(PYBIND11_FINDPYTHON ON)
+
 if(NOT SKBUILD_STATE STREQUAL "sdist"
    AND EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/pybind11/CMakeLists.txt")
   message(STATUS "Using integrated pybind11")
-  set(FETCHCONTENT_FULLY_DISCONNECTED ON)
+  add_subdirectory(pybind11)
+else()
+  FetchContent_Declare(
+    pybind11
+    GIT_REPOSITORY https://github.com/pybind/pybind11.git
+    GIT_TAG v2.12.0
+    SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/pybind11)
+  FetchContent_MakeAvailable(pybind11)
 endif()
-
-FetchContent_Declare(
-  pybind11
-  GIT_REPOSITORY https://github.com/pybind/pybind11.git
-  GIT_TAG v2.11.1
-  SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/pybind11)
-
-set(PYBIND11_FINDPYTHON ON)
-FetchContent_MakeAvailable(pybind11)
 ```
 
 The `/pybind11` directory is in the `.gitignore` and important parts are in
 `sdist.include`:
 
 ```toml
 [tool.scikit-build]
@@ -263,14 +265,21 @@
 as well (not guaranteed to be respected by editable installs):
 
 ```toml
 [tool.scikit-build]
 wheel.exclude = ["**.pyx"]
 ```
 
+:::{versionchanged} 0.9
+
+Before scikit-build-core 0.9, these were matched on the source path, rather than
+the wheel path, and didn't apply to CMake output.
+
+:::
+
 :::{note}
 
 There are two more settings that are primarily intended for `overrides` (see
 below). `wheel.cmake` defaults to `true`, and this enables/disables building
 with CMake. It also changes the default of `wheel.platlib` unless it's set
 explicitly; CMake builds assume `wheel.platlib = true`, and CMake-less builds
 assume `wheel.platlib = false` (purelib targeted instead).
```

### Comparing `scikit_build_core-0.8.2/docs/crosscompile.md` & `scikit_build_core-0.9.0/docs/crosscompile.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/faqs.md` & `scikit_build_core-0.9.0/docs/faqs.md`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,32 @@
 require the `Development.Embed` component, which will require the Python
 libraries to be found for linking. When building a module on Unix, you do not
 link to Python - the Python symbols are already loaded in the interpreter.
 What's more, the manylinux image (which is used to make redistributable Linux
 wheels) does not have the Python libraries, both to avoid this mistake, and to
 reduce size.
 
+## Cross compiling
+
+When cross compiling, FindPython may not get the correct SOABI extension.
+Scikit-build-core does know the correct extension, however, and sets it as
+`SKBUILD_SOABI`. See [the SOABI docs](#soabi).
+
+## Things to try
+
+If you want to debug a scikit-build-core build, you have several options. If you
+are using `pip`, make sure you are passing the `-v` flag, otherwise `pip`
+suppresses all output. You can
+[increase scikit-build-core's logging verbosity](#verbosity). You can also get a
+printout of the current settings using:
+
+```bash
+python -m scikit_build_core.builder
+```
+
 <!-- prettier-ignore-start -->
 
 [scientific python cookie]: https://github.com/scientific-python/cookie
-[scientific python development guide]: https://learn.scientific-python.org/development
+[scientific python development guidelines]: https://learn.scientific-python.org/development
 [pybind11 example]: https://github.com/pybind/scikit_build_example
 
 <!-- prettier-ignore-end -->
```

### Comparing `scikit_build_core-0.8.2/docs/getting_started.md` & `scikit_build_core-0.9.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/index.md` & `scikit_build_core-0.9.0/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,23 @@
 faqs
 changelog
 ```
 
 ```{toctree}
 :maxdepth: 1
 :titlesonly:
+:caption: Plugins
+
+plugins/setuptools
+plugins/hatchling
+```
+
+```{toctree}
+:maxdepth: 1
+:titlesonly:
 :caption: API docs
 
 api/scikit_build_core
 ```
 
 ## Indices and tables
```

### Comparing `scikit_build_core-0.8.2/docs/migration_guide.md` & `scikit_build_core-0.9.0/docs/migration_guide.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   [getting started](./getting_started.md) for more information.
 - If your project is primarily configured using setup.py or setup.cfg, you will
   need to move the configuration to pyproject.toml. The
   [project metadata spec](https://packaging.python.org/en/latest/specifications/pyproject-toml)
   shows the information that can be placed directly in the project table. For
   additional metadata, see [our configuration guide](./configuration.md). A
   useful trick for performing this migration is to change the `build-backend`
-  from `skbuild` to `setuptools`, install `hatch`, and run `hatch init --new`.
+  from `skbuild` to `setuptools`, install `hatch`, and run `hatch new --init`.
   This should automatically migrate the configuration to pyproject.toml, after
   which you can change the `build-backend` to `scikit-build-core`.
 - If you specify files to include in sdists via MANIFEST.in, with
   `scikit-build-core` you should now instead use the `sdist.include` and
   `sdist.exclude` fields in the `tool.scikit-build` table. Note that
   scikit-build-core uses all non `.gitignore`'d files by default, so this is
   often minimal or not needed.
```

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,49 @@
-scikit\_build\_core.build package
-=================================
+scikit\_build\_core package
+===========================
 
-.. automodule:: scikit_build_core.build
+.. automodule:: scikit_build_core
    :members:
    :undoc-members:
    :show-inheritance:
 
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   scikit_build_core.build
+   scikit_build_core.builder
+   scikit_build_core.file_api
+   scikit_build_core.hatch
+   scikit_build_core.metadata
+   scikit_build_core.resources
+   scikit_build_core.settings
+   scikit_build_core.setuptools
+
 Submodules
 ----------
 
-scikit\_build\_core.build.generate module
------------------------------------------
+scikit\_build\_core.cmake module
+--------------------------------
 
-.. automodule:: scikit_build_core.build.generate
+.. automodule:: scikit_build_core.cmake
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.build.sdist module
---------------------------------------
+scikit\_build\_core.errors module
+---------------------------------
 
-.. automodule:: scikit_build_core.build.sdist
+.. automodule:: scikit_build_core.errors
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.build.wheel module
---------------------------------------
+scikit\_build\_core.program\_search module
+------------------------------------------
 
-.. automodule:: scikit_build_core.build.wheel
+.. automodule:: scikit_build_core.program_search
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.build.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-scikit\_build\_core package
-===========================
+scikit\_build\_core.build package
+=================================
 
-.. automodule:: scikit_build_core
+.. automodule:: scikit_build_core.build
    :members:
    :undoc-members:
    :show-inheritance:
 
-Subpackages
------------
-
-.. toctree::
-   :maxdepth: 4
-
-   scikit_build_core.build
-   scikit_build_core.builder
-   scikit_build_core.file_api
-   scikit_build_core.metadata
-   scikit_build_core.resources
-   scikit_build_core.settings
-   scikit_build_core.setuptools
-
 Submodules
 ----------
 
-scikit\_build\_core.cmake module
---------------------------------
+scikit\_build\_core.build.generate module
+-----------------------------------------
+
+.. automodule:: scikit_build_core.build.generate
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scikit\_build\_core.build.metadata module
+-----------------------------------------
 
-.. automodule:: scikit_build_core.cmake
+.. automodule:: scikit_build_core.build.metadata
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.errors module
----------------------------------
+scikit\_build\_core.build.sdist module
+--------------------------------------
 
-.. automodule:: scikit_build_core.errors
+.. automodule:: scikit_build_core.build.sdist
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.program\_search module
-------------------------------------------
+scikit\_build\_core.build.wheel module
+--------------------------------------
 
-.. automodule:: scikit_build_core.program_search
+.. automodule:: scikit_build_core.build.wheel
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.settings.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,14 @@
 ------------------------------------------------
 
 .. automodule:: scikit_build_core.settings.json_schema
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.settings.metadata module
---------------------------------------------
-
-.. automodule:: scikit_build_core.settings.metadata
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 scikit\_build\_core.settings.skbuild\_docs module
 -------------------------------------------------
 
 .. automodule:: scikit_build_core.settings.skbuild_docs
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit_build_core-0.8.2/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.9.0/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/test.sh` & `scikit_build_core-0.9.0/docs/examples/test.sh`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    $ pip install .
   =====================================================================
   If you are a software developer, and this is your own package, then
   it is usually much more efficient to install the build dependencies
   in your environment once and use the following command that avoids
   a costly creation of a new virtual environment at every compilation:
   =====================================================================
-   $ pip install nanobind scikit-build-core[pyproject]
+   $ pip install nanobind scikit-build-core
    $ pip install --no-build-isolation -ve .
   =====================================================================
   You may optionally add -Ceditable.rebuild=true to auto-rebuild when
   the package is imported. Otherwise, you need to re-run the above
   after editing C++ files.")
 endif()
```

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.9.0/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.9.0/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.9.0/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.9.0/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-cmake_minimum_required(VERSION 3.15...3.26)
+cmake_minimum_required(VERSION 3.15)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
 find_package(
   Python
   COMPONENTS Interpreter Development.Module
   REQUIRED)
 
-find_program(CYTHON "cython")
-
 add_custom_command(
-  OUTPUT example.c
-  DEPENDS example.pyx
+  OUTPUT src/pkg2/two.c
+  DEPENDS src/pkg2/two.pyx
   VERBATIM
-  COMMAND "${CYTHON}" "${CMAKE_CURRENT_SOURCE_DIR}/example.pyx" --output-file
-          "${CMAKE_CURRENT_BINARY_DIR}/example.c")
+  COMMAND
+    Python::Interpreter -m cython
+    "${CMAKE_CURRENT_SOURCE_DIR}/src/pkg2/two.pyx" --output-file
+    "${CMAKE_CURRENT_BINARY_DIR}/src/pkg2/two.c")
 
-python_add_library(example MODULE "${CMAKE_CURRENT_BINARY_DIR}/example.c"
+python_add_library(two MODULE "${CMAKE_CURRENT_BINARY_DIR}/src/pkg2/two.c"
                    WITH_SOABI)
 
-install(TARGETS example DESTINATION .)
+install(TARGETS two DESTINATION pkg2/)
```

### Comparing `scikit_build_core-0.8.2/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.9.0/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.9.0/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/docs/ext/conftabs.py` & `scikit_build_core-0.9.0/docs/ext/conftabs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/_logging.py` & `scikit_build_core-0.9.0/src/scikit_build_core/_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             f"<FStringMessage {self.fmt!r} args={self.args!r} kwargs={self.kwargs!r}>"
         )
 
 
 if sys.version_info < (3, 8):
     opts: Any = {}
 else:
-    opts = {"stacklevel": 2}
+    opts: Any = {"stacklevel": 2}
 
 
 class ScikitBuildLogger:
     # pylint: disable-next=redefined-outer-name
     def __init__(self, logger: logging.Logger) -> None:
         self.logger = logger
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.9.0/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/cmake.py` & `scikit_build_core-0.9.0/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/errors.py` & `scikit_build_core-0.9.0/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/program_search.py` & `scikit_build_core-0.9.0/src/scikit_build_core/program_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import contextlib
+import json
 import shutil
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, NamedTuple
 
 from packaging.version import InvalidVersion, Version
 
@@ -73,22 +74,22 @@
 
 def get_cmake_program(cmake_path: Path) -> Program:
     """
     Get the Program (with version) for CMake given a path. The version will be
     None if it cannot be determined.
     """
     try:
-        result = Run().capture(cmake_path, "--version")
+        result = Run().capture(cmake_path, "-E", "capabilities")
     except (subprocess.CalledProcessError, PermissionError):
         return Program(cmake_path, None)
 
     try:
-        version = Version(result.stdout.splitlines()[0].split()[-1].split("-")[0])
-    except (IndexError, InvalidVersion):
-        logger.warning(f"Could not determine CMake version, got {result.stdout!r}")
+        version = Version(json.loads(result.stdout)["version"]["string"])
+    except (json.decoder.JSONDecodeError, KeyError, InvalidVersion):
+        logger.warning("Could not determine CMake version, got {!r}", result.stdout)
         return Program(cmake_path, None)
 
     logger.info("CMake version: {}", version)
     return Program(cmake_path, version)
 
 
 def get_cmake_programs(*, module: bool = True) -> Generator[Program, None, None]:
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.9.0/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,60 +97,54 @@
 
 
 def get_requires_for_build_sdist(
     config_settings: dict[str, str | list[str]] | None = None,
 ) -> list[str]:
     from ..builder.get_requires import GetRequires
 
-    requires = GetRequires(config_settings)
+    requires = GetRequires.from_config_settings(config_settings)
 
     # These are only injected if cmake is required for the SDist step
     cmake_requires = (
         [*requires.cmake(), *requires.ninja()] if requires.settings.sdist.cmake else []
     )
 
     return [
-        "pathspec",
-        "pyproject_metadata",
         *cmake_requires,
         *requires.dynamic_metadata(),
     ]
 
 
 def get_requires_for_build_wheel(
     config_settings: dict[str, str | list[str]] | None = None,
 ) -> list[str]:
     from ..builder.get_requires import GetRequires
 
-    requires = GetRequires(config_settings)
+    requires = GetRequires.from_config_settings(config_settings)
 
     # These are only injected if cmake is required for the wheel step
     cmake_requires = (
         [*requires.cmake(), *requires.ninja()] if requires.settings.wheel.cmake else []
     )
 
     return [
-        "pathspec",
-        "pyproject_metadata",
         *cmake_requires,
         *requires.dynamic_metadata(),
     ]
 
 
 def get_requires_for_build_editable(
     config_settings: dict[str, str | list[str]] | None = None,
 ) -> list[str]:
     from ..builder.get_requires import GetRequires
 
-    requires = GetRequires(config_settings)
+    requires = GetRequires.from_config_settings(config_settings)
 
     # These are only injected if cmake is required for the wheel step
     cmake_requires = (
         [*requires.cmake(), *requires.ninja()] if requires.settings.wheel.cmake else []
     )
 
     return [
-        "pathspec",
-        "pyproject_metadata",
         *cmake_requires,
         *requires.dynamic_metadata(),
     ]
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_editable.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_editable.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_pathutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+import pathspec
+
 from ._file_processor import each_unignored_file
 
 if TYPE_CHECKING:
     from collections.abc import Generator, Sequence
 
 __all__ = ["is_valid_module", "packages_to_file_mapping", "path_to_module", "scantree"]
 
@@ -33,28 +35,31 @@
 
 
 def packages_to_file_mapping(
     *,
     packages: Sequence[str],
     platlib_dir: Path,
     include: Sequence[str],
-    exclude: Sequence[str],
+    src_exclude: Sequence[str],
+    target_exclude: Sequence[str],
 ) -> dict[str, str]:
     mapping = {}
+    exclude_spec = pathspec.GitIgnoreSpec.from_lines(target_exclude)
     for package in packages:
         source_package = Path(package)
         base_path = source_package.parent
         for filepath in each_unignored_file(
             source_package,
             include=include,
-            exclude=exclude,
+            exclude=src_exclude,
         ):
-            package_dir = platlib_dir / filepath.relative_to(base_path)
-            if not package_dir.is_file():
-                mapping[str(filepath)] = str(package_dir)
+            rel_path = filepath.relative_to(base_path)
+            target_path = platlib_dir / rel_path
+            if not exclude_spec.match_file(rel_path) and not target_path.is_file():
+                mapping[str(filepath)] = str(target_path)
 
     return mapping
 
 
 def is_valid_module(path: Path) -> bool:
     parts = path.parts
     return (
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/_wheelfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from __future__ import annotations
 
 import base64
-import copy
 import csv
 import dataclasses
 import hashlib
 import io
 import os
 import stat
 import time
 import zipfile
 from email.message import Message
 from email.policy import EmailPolicy
 from pathlib import Path
 from typing import TYPE_CHECKING
 from zipfile import ZipInfo
 
-import packaging.utils
+import pathspec
 
 from .. import __version__
 
 if TYPE_CHECKING:
-    from collections.abc import Mapping, Set
+    from collections.abc import Mapping, Sequence, Set
 
     from packaging.tags import Tag
-    from pyproject_metadata import StandardMetadata
 
     from .._compat.typing import Self
+    from .._vendor.pyproject_metadata import StandardMetadata
 
 EMAIL_POLICY = EmailPolicy(max_line_length=0, mangle_from_=False, utf8=True)
 
 MIN_TIMESTAMP = 315532800  # 1980-01-01 00:00:00 UTC
 
 
 def _b64encode(data: bytes) -> bytes:
@@ -71,20 +70,20 @@
 class WheelWriter:
     """A general tool for writing wheels. Designed to look a little like ZipFile."""
 
     metadata: StandardMetadata
     folder: Path
     tags: Set[Tag]
     wheel_metadata: WheelMetadata
-    license_files: Mapping[Path, bytes] = dataclasses.field(default_factory=dict)
+    metadata_dir: Path | None
     _zipfile: zipfile.ZipFile | None = None
 
     @property
     def name_ver(self) -> str:
-        name = packaging.utils.canonicalize_name(self.metadata.name).replace("-", "_")
+        name = self.metadata.canonical_name.replace("-", "_")
         # replace - with _ as a local version separator
         version = str(self.metadata.version).replace("-", "_")
         return f"{name}-{version}"
 
     @property
     def basename(self) -> str:
         pyver = ".".join(sorted({t.interpreter for t in self.tags}))
@@ -120,50 +119,68 @@
                 entry_points.write(f"[{group}]\n")
                 for name, target in entries.items():
                     entry_points.write(f"{name} = {target}\n")
                 entry_points.write("\n")
 
         self.wheel_metadata.tags = self.tags
 
-        # Using deepcopy here because of a bug in pyproject-metadata
-        # https://github.com/FFY00/python-pyproject-metadata/pull/49
-        rfc822 = copy.deepcopy(self.metadata).as_rfc822()
-        for fp in self.license_files:
-            rfc822["License-File"] = f"{fp}"
+        rfc822 = self.metadata.as_rfc822()
 
-        license_entries = {
-            f"licenses/{fp}": data for fp, data in self.license_files.items()
+        metadata_files = self.metadata_dir.rglob("*") if self.metadata_dir else []
+        extra_metadata = {
+            str(f.relative_to(self.metadata_dir or Path())): f.read_bytes()
+            for f in metadata_files
+            if f.is_file()
         }
+        if {"METADATA", "WHEEL", "RECORD", "entry_points.txt"} & extra_metadata.keys():
+            msg = "Cannot have METADATA, WHEEL, RECORD, or entry_points.txt in metadata_dir"
+            raise ValueError(msg)
 
         return {
             "METADATA": bytes(rfc822),
             "WHEEL": self.wheel_metadata.as_bytes(),
             "entry_points.txt": entry_points.getvalue().encode("utf-8"),
-            **license_entries,
+            **extra_metadata,
         }
 
-    def build(self, wheel_dirs: dict[str, Path]) -> None:
+    def build(
+        self, wheel_dirs: Mapping[str, Path], exclude: Sequence[str] = ()
+    ) -> None:
         (targetlib,) = {"platlib", "purelib"} & set(wheel_dirs)
-        assert {targetlib, "data", "headers", "scripts", "null"} >= wheel_dirs.keys()
+        assert {
+            targetlib,
+            "data",
+            "headers",
+            "scripts",
+            "null",
+            "metadata",
+        } >= wheel_dirs.keys()
 
         # The "main" directory (platlib usually for us) will be handled specially below
         plans = {"": wheel_dirs[targetlib]}
         data_dir = f"{self.name_ver}.data"
 
         for key in sorted({"data", "headers", "scripts"} & wheel_dirs.keys()):
             plans[key] = wheel_dirs[key]
 
+        exclude_spec = pathspec.GitIgnoreSpec.from_lines(exclude)
+
         for key, path in plans.items():
             for filename in sorted(path.glob("**/*")):
-                is_in_dist_info = any(x.endswith(".dist-info") for x in filename.parts)
-                is_python_cache = filename.suffix in {".pyc", ".pyo"}
-                if filename.is_file() and not is_in_dist_info and not is_python_cache:
-                    relpath = filename.relative_to(path)
-                    target = Path(data_dir) / key / relpath if key else relpath
-                    self.write(str(filename), str(target))
+                if not filename.is_file():
+                    continue
+                if any(x.endswith(".dist-info") for x in filename.parts):
+                    continue
+                if filename.suffix in {".pyc", ".pyo"}:
+                    continue
+                relpath = filename.relative_to(path)
+                if exclude_spec.match_file(relpath):
+                    continue
+                target = Path(data_dir) / key / relpath if key else relpath
+                self.write(str(filename), str(target))
 
         dist_info_contents = self.dist_info_contents()
         for key, data in dist_info_contents.items():
             self.writestr(f"{self.dist_info}/{key}", data)
 
     def write(self, filename: str, arcname: str | None = None) -> None:
         """Write a file to the archive. Paths are normalized to Posix paths."""
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/generate.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 __all__ = ["generate_file_contents"]
 
 import dataclasses
 import string
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from pyproject_metadata import StandardMetadata
-
+    from .._vendor.pyproject_metadata import StandardMetadata
     from ..settings.skbuild_model import GenerateSettings
 
 
 def __dir__() -> list[str]:
     return __all__
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/sdist.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from packaging.utils import canonicalize_name
 from packaging.version import Version
 
 from .. import __version__
 from .._compat import tomllib
 from .._logging import rich_print
-from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._file_processor import each_unignored_file
 from ._init import setup_logging
 from .generate import generate_file_contents
+from .metadata import get_standard_metadata
 from .wheel import _build_wheel_impl
 
 __all__ = ["build_sdist"]
 
 
 def __dir__() -> list[str]:
     return __all__
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.9.0/src/scikit_build_core/build/wheel.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from .._compat import tomllib
 from .._compat.typing import Literal, assert_never
 from .._logging import logger, rich_print
 from .._shutil import fix_win_37_all_permissions
 from ..builder.builder import Builder, archs_to_tags, get_archs
 from ..builder.wheel_tag import WheelTag
 from ..cmake import CMake, CMaker
-from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._editable import editable_redirect, libdir_to_installed, mapping_to_modules
 from ._init import setup_logging
 from ._pathutil import (
     packages_to_file_mapping,
 )
 from ._scripts import process_script_dir
 from ._wheelfile import WheelMetadata, WheelWriter
 from .generate import generate_file_contents
+from .metadata import get_standard_metadata
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, Sequence
 
     from ..settings.skbuild_model import ScikitBuildSettings
 
 __all__ = ["_build_wheel_impl"]
@@ -197,14 +197,15 @@
 
         wheel_dirs = {
             targetlib: wheel_dir / targetlib,
             "data": wheel_dir / "data",
             "headers": wheel_dir / "headers",
             "scripts": wheel_dir / "scripts",
             "null": wheel_dir / "null",
+            "metadata": wheel_dir / "metadata",
         }
 
         for d in wheel_dirs.values():
             d.mkdir(parents=True)
 
         if ".." in settings.wheel.install_dir:
             msg = "wheel.install_dir must not contain '..'"
@@ -221,21 +222,25 @@
             install_dir = wheel_dirs[targetlib] / settings.wheel.install_dir
 
         # Include the metadata license.file entry if provided
         license_file_globs = list(settings.wheel.license_files)
         if metadata.license and metadata.license.file:
             license_file_globs.append(str(metadata.license.file))
 
-        license_files = {
-            x: x.read_bytes()
-            for y in license_file_globs
-            for x in Path().glob(y)
-            if x.is_file()
-        }
-        if settings.wheel.license_files and not license_files:
+        for y in license_file_globs:
+            for x in Path().glob(y):
+                if x.is_file():
+                    path = wheel_dirs["metadata"] / "licenses" / x
+                    path.parent.mkdir(parents=True, exist_ok=True)
+                    shutil.copy(x, path)
+
+        if (
+            settings.wheel.license_files
+            and not (wheel_dirs["metadata"] / "licenses").is_dir()
+        ):
             logger.warning(
                 "No license files found, set wheel.license-files to [] to suppress this warning"
             )
 
         for gen in settings.generate:
             if gen.location == "source":
                 contents = generate_file_contents(gen, metadata)
@@ -250,15 +255,15 @@
                 metadata,
                 Path(metadata_directory),
                 tags.as_tags_set(),
                 WheelMetadata(
                     root_is_purelib=targetlib == "purelib",
                     build_tag=settings.wheel.build_tag,
                 ),
-                license_files=license_files,
+                wheel_dirs["metadata"],
             )
             dist_info_contents = wheel.dist_info_contents()
             dist_info = Path(metadata_directory) / f"{wheel.name_ver}.dist-info"
             dist_info.mkdir(parents=True)
             for key, data in dist_info_contents.items():
                 path = dist_info / key
                 if not path.parent.is_dir():
@@ -340,15 +345,16 @@
             packages=settings.wheel.packages,
             name=normalized_name,
         )
         mapping = packages_to_file_mapping(
             packages=packages,
             platlib_dir=wheel_dirs[targetlib],
             include=settings.sdist.include,
-            exclude=[*settings.sdist.exclude, *settings.wheel.exclude],
+            src_exclude=settings.sdist.exclude,
+            target_exclude=settings.wheel.exclude,
         )
 
         if not editable:
             for filepath, package_dir in mapping.items():
                 Path(package_dir).parent.mkdir(exist_ok=True, parents=True)
                 shutil.copyfile(filepath, package_dir)
 
@@ -358,17 +364,17 @@
             metadata,
             Path(wheel_directory),
             tags.as_tags_set(),
             WheelMetadata(
                 root_is_purelib=targetlib == "purelib",
                 build_tag=settings.wheel.build_tag,
             ),
-            license_files=license_files,
+            wheel_dirs["metadata"],
         ) as wheel:
-            wheel.build(wheel_dirs)
+            wheel.build(wheel_dirs, exclude=settings.wheel.exclude)
 
             str_pkgs = (str(Path.cwd().joinpath(p).parent.resolve()) for p in packages)
             if editable and settings.editable.mode == "redirect":
                 reload_dir = build_dir.resolve() if settings.build_dir else None
 
                 _make_editable(
                     build_options=build_options,
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/__main__.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def main() -> None:
     rich_print(f"[bold]Scikit-build-core {__version__}[/bold] on Python {sys.version}")
 
     ip_sysconfig(color="green")
 
     rich_print(f"[bold blue]Default Wheel Tag:[/bold] {WheelTag.compute_best([])}")
     rich_print(
-        "[blue] - Note: use [bold]python -m scikit_build_core.builder.wheel_tag[/bold] for further options[/blue]"
+        "[blue] - Note: use [bold]python -m scikit_build_core.builder.wheel_tag -h[/bold] for further options[/blue]"
     )
 
     if Path("pyproject.toml").is_file():
         req = GetRequires()
         all_req = [*req.cmake(), *req.ninja(), *req.dynamic_metadata()]
         rich_print(f"[bold red]Get Requires:[/bold] {all_req!r}")
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/get_requires.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from ..resources import resources
 from ..settings._load_provider import load_provider
 from ..settings.skbuild_read_settings import SettingsReader
 
 if TYPE_CHECKING:
     from collections.abc import Generator, Mapping
 
-    from .._compat.typing import Literal
+    from .._compat.typing import Literal, Self
     from ..settings.skbuild_model import ScikitBuildSettings
 
 __all__ = ["GetRequires"]
 
 
 def __dir__() -> list[str]:
     return __all__
@@ -41,26 +41,31 @@
 
 
 @functools.lru_cache(maxsize=2)
 def is_known_platform(platforms: frozenset[str]) -> bool:
     return any(tag.platform in platforms for tag in sys_tags())
 
 
-@dataclasses.dataclass
-class GetRequires:
-    config_settings: Mapping[str, list[str] | str] | None = None
+def _load_scikit_build_settings(
+    config_settings: Mapping[str, list[str] | str] | None = None,
+) -> ScikitBuildSettings:
+    return SettingsReader.from_file("pyproject.toml", config_settings).settings
+
 
-    def __post_init__(self) -> None:
-        self._settings = SettingsReader.from_file(
-            "pyproject.toml", self.config_settings
-        ).settings
-
-    @property
-    def settings(self) -> ScikitBuildSettings:
-        return self._settings
+@dataclasses.dataclass(frozen=True)
+class GetRequires:
+    settings: ScikitBuildSettings = dataclasses.field(
+        default_factory=_load_scikit_build_settings
+    )
+
+    @classmethod
+    def from_config_settings(
+        cls, config_settings: Mapping[str, list[str] | str] | None
+    ) -> Self:
+        return cls(_load_scikit_build_settings(config_settings))
 
     def cmake(self) -> Generator[str, None, None]:
         if os.environ.get("CMAKE_EXECUTABLE", ""):
             return
 
         cmake_verset = self.settings.cmake.version
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.9.0/src/scikit_build_core/builder/wheel_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,22 @@
             if not build_tag[0].isdigit():
                 msg = f"Unexpected build-tag, must start with a digit, {build_tag!r} invalid"
                 raise AssertionError(msg)
             if "-" in build_tag:
                 msg = f"Unexpected build-tag, {build_tag!r} cannot contain dashes"
                 raise AssertionError(msg)
 
-        best_tag = next(packaging.tags.sys_tags())
+        # manylinux sometimes comes before linux, but can't assume manylinux, use auditwheel instead
+        best_tag = next(
+            iter(
+                p
+                for p in packaging.tags.sys_tags()
+                if "manylinux" not in p.platform and "muslllinux" not in p.platform
+            )
+        )
         interp, abi, *plats = (best_tag.interpreter, best_tag.abi, best_tag.platform)
         pyvers = [interp]
 
         if sys.platform.startswith("win") and archs:
             plats = [x.replace("-", "_") for x in archs]
         elif sys.platform.startswith("darwin"):
             pairs: Iterable[tuple[str | None, bool]]
@@ -77,14 +84,15 @@
             ]
             # Remove duplicates (e.g. universal2 if macOS > 11.0 and expanded)
             plats = list(dict.fromkeys(plats))
 
         if root_is_purelib:
             plats = ["any"]
             abi = "none"
+            pyvers = ["py3"]
 
         if py_api:
             pyvers_new = py_api.split(".")
             if all(x.startswith("cp3") and x[3:].isdecimal() for x in pyvers_new):
                 if len(pyvers_new) != 1:
                     msg = "Unexpected py-api, must be a single cp version (e.g. cp39), not {py_api}"
                     raise AssertionError(msg)
@@ -152,10 +160,15 @@
         help="Specify one or more archs (macOS only currently)",
     )
     parser.add_argument(
         "--abi",
         default="",
         help="Specify py-api, like 'cp37' or 'py3'",
     )
+    parser.add_argument(
+        "--purelib",
+        action="store_true",
+        help="Specify a non-platlib (pure) tag",
+    )
     args = parser.parse_args()
-    tag = WheelTag.compute_best(args.archs, args.abi)
+    tag = WheelTag.compute_best(args.archs, args.abi, root_is_purelib=args.purelib)
     print(tag)  # noqa: T201
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.9.0/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.9.0/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/metadata/regex.py` & `scikit_build_core-0.9.0/src/scikit_build_core/metadata/regex.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.9.0/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/scikit-build.schema.json` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/scikit-build.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761732987948265%*

 * *Differences: {"'$defs'": "{'inherit': OrderedDict([('enum', ['none', 'append', 'prepend']), ('default', "*

 * *            "'none')])}",*

 * * "'properties'": "{'ninja': {'properties': {'make-fallback': {'description': 'If Ninja is not "*

 * *                 'present on the system or is older than required, it will be downloaded via PyPI '*

 * *                 "if this is false.'}}}, 'wheel': {'properties': {'exclude': {'description': 'A "*

 * *                 'set of patterns to exclude from the wheel. This is additive to the SDist exclude  […]*

```diff
@@ -49,14 +49,22 @@
                 "state": {
                     "description": "The state of the build, one of `sdist`, `wheel`, `editable`, `metadata_wheel`, and `metadata_editable`. Takes a regex.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "inherit": {
+            "default": "none",
+            "enum": [
+                "none",
+                "append",
+                "prepend"
+            ]
+        },
         "metadata": {
             "properties": {
                 "provider": {
                     "type": "string"
                 },
                 "provider-path": {
                     "type": "string"
@@ -360,15 +368,15 @@
             "type": "string"
         },
         "ninja": {
             "additionalProperties": false,
             "properties": {
                 "make-fallback": {
                     "default": true,
-                    "description": "If CMake is not present on the system or is older required, it will be downloaded via PyPI if possible. An empty string will disable this check.",
+                    "description": "If Ninja is not present on the system or is older than required, it will be downloaded via PyPI if this is false.",
                     "type": "boolean"
                 },
                 "minimum-version": {
                     "deprecated": true,
                     "description": "DEPRECATED in 0.8; use version instead.",
                     "type": "string"
                 },
@@ -419,14 +427,71 @@
                                 "required": [
                                     "any"
                                 ],
                                 "type": "object"
                             }
                         ]
                     },
+                    "inherit": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "cmake": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "args": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "define": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "targets": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "install": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "components": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "sdist": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "exclude": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "include": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "wheel": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "exclude": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "license-files": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "packages": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "install": {
                         "$ref": "#/properties/install"
                     },
                     "logging": {
                         "$ref": "#/properties/logging"
                     },
                     "metadata": {
@@ -500,15 +565,15 @@
                 },
                 "cmake": {
                     "default": true,
                     "description": "If set to True (the default), CMake will be run before building the wheel.",
                     "type": "boolean"
                 },
                 "exclude": {
-                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the source files, not the final paths. Editable installs may not respect this exclusion.",
+                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the final paths in the wheel, and can exclude files from CMake output as well.  Editable installs may not respect this exclusion.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "expand-macos-universal-tags": {
                     "default": false,
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.9.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/_load_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,34 +16,32 @@
 def __dir__() -> list[str]:
     return __all__
 
 
 class DynamicMetadataProtocol(Protocol):
     def dynamic_metadata(
         self, fields: Iterable[str], settings: dict[str, Any]
-    ) -> dict[str, Any]:
-        ...
+    ) -> dict[str, Any]: ...
 
 
 class DynamicMetadataRequirementsProtocol(DynamicMetadataProtocol, Protocol):
-    def get_requires_for_dynamic_metadata(self, settings: dict[str, Any]) -> list[str]:
-        ...
+    def get_requires_for_dynamic_metadata(
+        self, settings: dict[str, Any]
+    ) -> list[str]: ...
 
 
 class DynamicMetadataWheelProtocol(DynamicMetadataProtocol, Protocol):
     def dynamic_wheel(
         self, field: str, settings: Mapping[str, Any] | None = None
-    ) -> bool:
-        ...
+    ) -> bool: ...
 
 
 class DynamicMetadataRequirementsWheelProtocol(
     DynamicMetadataRequirementsProtocol, DynamicMetadataWheelProtocol, Protocol
-):
-    ...
+): ...
 
 
 DMProtocols = Union[
     DynamicMetadataProtocol,
     DynamicMetadataRequirementsProtocol,
     DynamicMetadataWheelProtocol,
     DynamicMetadataRequirementsWheelProtocol,
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/documentation.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 def _get_value(value: ast.expr) -> str:
     if sys.version_info < (3, 8):
         assert isinstance(value, ast.Str)
         return value.s
 
     assert isinstance(value, ast.Constant)
+    assert isinstance(value.value, str)
     return value.value
 
 
 def pull_docs(dc: type[object]) -> dict[str, str]:
     """
     Pulls documentation from a dataclass.
     """
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/json_schema.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_docs.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_docs.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Makes documentation for the skbuild model.
     """
     items = list(mk_docs(ScikitBuildSettings))
     for item in items:
         if item.name == "minimum-version":
             item.default = f'"{version}"  # current version'
         if item.name == "install.strip":
-            item.default = "false"
+            item.default = "true"
         if item.name == "wheel.packages":
             item.default = '["src/<package>", "python/<package>", "<package>"]'
     return "\n".join(str(item) for item in items)
 
 
 if __name__ == "__main__":
     print(mk_skbuild_docs())  # noqa: T201
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,24 +89,24 @@
     The versions of Ninja to allow. If Ninja is not present on the system or does
     not pass this specifier, it will be downloaded via PyPI if possible. An empty
     string will disable this check.
     """
 
     make_fallback: bool = True
     """
-    If CMake is not present on the system or is older required, it will be
-    downloaded via PyPI if possible. An empty string will disable this check.
+    If Ninja is not present on the system or is older than required,
+    it will be downloaded via PyPI if this is false.
     """
 
 
 @dataclasses.dataclass
 class LoggingSettings:
-    level: Literal[
-        "NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
-    ] = "WARNING"
+    level: Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"] = (
+        "WARNING"
+    )
     """
     The logging level to display, "DEBUG", "INFO", "WARNING", and "ERROR" are
     possible options.
     """
 
 
 @dataclasses.dataclass
@@ -189,16 +189,17 @@
     Target the platlib or the purelib. If not set, the default is to target the
     platlib if wheel.cmake is true, and the purelib otherwise.
     """
 
     exclude: List[str] = dataclasses.field(default_factory=list)
     """
     A set of patterns to exclude from the wheel. This is additive to the SDist
-    exclude patterns. This applies to the source files, not the final paths.
-    Editable installs may not respect this exclusion.
+    exclude patterns. This applies to the final paths in the wheel, and can
+    exclude files from CMake output as well.  Editable installs may not respect
+    this exclusion.
     """
 
     build_tag: str = ""
     """
     The build tag to use for the wheel. If empty, no build tag is used.
     """
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -187,71 +187,122 @@
                 f"[red][bold]ERROR:[/bold] Cannot set both {name}.minimum_version and {name}.version; use version only for scikit-build-core >= 0.8."
             )
             raise SystemExit(7)
 
         dc.version = SpecifierSet(f">={dc.minimum_version}")
 
 
+def inherit_join(
+    value: list[str] | dict[str, str] | str | int | bool,
+    previous: list[str] | dict[str, str] | str | int | bool | None,
+    mode: str,
+) -> list[str] | dict[str, str] | str | int | bool:
+    if mode not in {"none", "append", "prepend"}:
+        msg = "Only 'none', 'append', and 'prepend' supported for inherit"
+        raise TypeError(msg)
+    if mode == "none" or previous is None:
+        return value
+    if isinstance(previous, list) and isinstance(value, list):
+        return [*previous, *value] if mode == "append" else [*value, *previous]
+    if isinstance(previous, dict) and isinstance(value, dict):
+        return {**previous, **value} if mode == "append" else {**value, **previous}
+    msg = "Append/prepend modes can only be used on lists or dicts"
+    raise TypeError(msg)
+
+
+def process_overides(
+    tool_skb: dict[str, Any],
+    state: Literal["sdist", "wheel", "editable", "metadata_wheel", "metadata_editable"],
+    env: Mapping[str, str] | None = None,
+) -> None:
+    """
+    Process overrides into the main dictionary if they match. Modifies the input dictionary.
+    """
+
+    for override in tool_skb.pop("overrides", []):
+        matched = True
+        if_override = override.pop("if", None)
+        if not if_override:
+            msg = "At least one 'if' override must be provided"
+            raise KeyError(msg)
+        if not isinstance(if_override, dict):
+            msg = "'if' override must be a table"
+            raise TypeError(msg)
+        if "any" in if_override:
+            any_override = if_override.pop("any")
+            select = {k.replace("-", "_"): v for k, v in any_override.items()}
+            matched = override_match(
+                match_all=False, current_env=env, current_state=state, **select
+            )
+
+        inherit_override = override.pop("inherit", {})
+        if not isinstance(inherit_override, dict):
+            msg = "'inherit' override must be a table"
+            raise TypeError(msg)
+
+        select = {k.replace("-", "_"): v for k, v in if_override.items()}
+        if select:
+            matched = matched and override_match(
+                match_all=True, current_env=env, current_state=state, **select
+            )
+        if matched:
+            for key, value in override.items():
+                inherit1 = inherit_override.get(key, {})
+                if isinstance(value, dict):
+                    for key2, value2 in value.items():
+                        inherit2 = inherit1.get(key2, "none")
+                        inner = tool_skb.get(key, {})
+                        inner[key2] = inherit_join(
+                            value2, inner.get(key2, None), inherit2
+                        )
+                        tool_skb[key] = inner
+                else:
+                    inherit_override_tmp = inherit_override or "none"
+                    if isinstance(inherit_override_tmp, dict):
+                        assert not inherit_override_tmp
+                    tool_skb[key] = inherit_join(
+                        value, tool_skb.get(key), inherit_override_tmp
+                    )
+
+
 class SettingsReader:
     def __init__(
         self,
         pyproject: dict[str, Any],
         config_settings: Mapping[str, str | list[str]],
         *,
         state: Literal[
             "sdist", "wheel", "editable", "metadata_wheel", "metadata_editable"
         ],
+        extra_settings: Mapping[str, Any] | None = None,
         verify_conf: bool = True,
         env: Mapping[str, str] | None = None,
     ) -> None:
+        self.state = state
+
         pyproject = copy.deepcopy(pyproject)
+        process_overides(pyproject.get("tool", {}).get("scikit-build", {}), state, env)
+        toml_srcs = [TOMLSource("tool", "scikit-build", settings=pyproject)]
 
-        # Process overrides into the main dictionary if they match
-        tool_skb = pyproject.get("tool", {}).get("scikit-build", {})
-        for override in tool_skb.pop("overrides", []):
-            matched = True
-            if_override = override.pop("if", None)
-            if not if_override:
-                msg = "At least one 'if' override must be provided"
-                raise KeyError(msg)
-            if not isinstance(if_override, dict):
-                msg = "'if' override must be a table"
-                raise TypeError(msg)
-            if "any" in if_override:
-                any_override = if_override.pop("any")
-                select = {k.replace("-", "_"): v for k, v in any_override.items()}
-                matched = override_match(
-                    match_all=False, current_env=env, current_state=state, **select
-                )
-            select = {k.replace("-", "_"): v for k, v in if_override.items()}
-            if select:
-                matched = matched and override_match(
-                    match_all=True, current_env=env, current_state=state, **select
-                )
-            if matched:
-                for key, value in override.items():
-                    if isinstance(value, dict):
-                        for key2, value2 in value.items():
-                            inner = tool_skb.get(key, {})
-                            inner[key2] = value2
-                            tool_skb[key] = inner
-                    else:
-                        tool_skb[key] = value
+        if extra_settings is not None:
+            extra_skb = copy.deepcopy(dict(extra_settings))
+            process_overides(extra_skb, state, env)
+            toml_srcs.insert(0, TOMLSource(settings=extra_skb))
 
         prefixed = {
             k: v for k, v in config_settings.items() if k.startswith("skbuild.")
         }
         remaining = {
             k: v for k, v in config_settings.items() if not k.startswith("skbuild.")
         }
         self.sources = SourceChain(
             EnvSource("SKBUILD"),
             ConfSource("skbuild", settings=prefixed, verify=verify_conf),
             ConfSource(settings=remaining, verify=verify_conf),
-            TOMLSource("tool", "scikit-build", settings=pyproject),
+            *toml_srcs,
             prefixes=["tool", "scikit-build"],
         )
         self.settings = self.sources.convert_target(ScikitBuildSettings)
 
         if self.settings.minimum_version:
             current_version = Version(__version__)
             minimum_version = self.settings.minimum_version
@@ -350,20 +401,27 @@
                 )
                 raise SystemExit(7)
 
     @classmethod
     def from_file(
         cls,
         pyproject_path: os.PathLike[str] | str,
-        config_settings: Mapping[str, str | list[str]] | None,
+        config_settings: Mapping[str, str | list[str]] | None = None,
         *,
         state: Literal[
             "sdist", "wheel", "editable", "metadata_wheel", "metadata_editable"
         ] = "sdist",
         verify_conf: bool = True,
+        extra_settings: Mapping[str, Any] | None = None,
+        env: Mapping[str, str] | None = None,
     ) -> SettingsReader:
         with Path(pyproject_path).open("rb") as f:
             pyproject = tomllib.load(f)
 
         return cls(
-            pyproject, config_settings or {}, verify_conf=verify_conf, state=state
+            pyproject,
+            config_settings or {},
+            verify_conf=verify_conf,
+            state=state,
+            extra_settings=extra_settings,
+            env=env,
         )
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/skbuild_schema.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/skbuild_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -123,14 +123,34 @@
                 },
                 "additionalProperties": False,
                 "minProperties": 1,
                 "description": "A table of environment variables mapped to either string regexs, or booleans. Valid 'truthy' environment variables are case insensitive `true`, `on`, `yes`, `y`, `t`, or a number more than 0.",
             },
         },
     }
+    schema["$defs"]["inherit"] = {
+        "enum": ["none", "append", "prepend"],
+        "default": "none",
+    }
+
+    inherit_props: dict[str, Any] = {
+        k: {
+            kk: {"$ref": "#/$defs/inherit"}
+            for kk, vv in v["properties"].items()
+            if vv.get("type", "") in {"object", "array"}
+        }
+        for k, v in schema["properties"].items()
+        if v.get("type", "") == "object"
+    }
+    inherit_props = {
+        k: {"type": "object", "additionalProperties": False, "properties": v}
+        for k, v in inherit_props.items()
+        if v
+    }
+
     schema["properties"]["overrides"] = {
         "type": "array",
         "description": "A list of overrides to apply to the settings, based on the `if` selector.",
         "items": {
             "type": "object",
             "required": ["if"],
             "minProperties": 2,
@@ -143,14 +163,19 @@
                             "type": "object",
                             "properties": {"any": {"$ref": "#/$defs/if_overrides"}},
                             "required": ["any"],
                             "additionalProperties": False,
                         },
                     ]
                 },
+                "inherit": {
+                    "type": "object",
+                    "properties": inherit_props,
+                    "additionalProperties": False,
+                },
                 **props,
             },
         },
     }
 
     return schema
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.9.0/src/scikit_build_core/settings/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,20 +310,23 @@
 class ConfSource:
     """
     This is a source for the PEP 517 configuration settings.
     You should initialize it with a dict from PEP 517. a.b will be treated as
     nested dicts. "verify" is a boolean that determines whether unrecognized
     options should be checked for. Only set this to false if this might be sharing
     config options at the same level.
+
+    While most mechanisms (pip, uv, build) only support text, gpep517 allows an
+    arbitrary json input, so this currently also handles bools.
     """
 
     def __init__(
         self,
         *prefixes: str,
-        settings: Mapping[str, str | list[str]],
+        settings: Mapping[str, str | list[str] | bool],
         verify: bool = True,
     ) -> None:
         self.prefixes = prefixes
         self.settings = settings
         self.verify = verify
 
     def _get_name(self, *fields: str) -> list[str]:
@@ -335,15 +338,17 @@
         name = ".".join(names)
 
         if is_dict:
             return any(k.startswith(f"{name}.") for k in self.settings)
 
         return name in self.settings
 
-    def get_item(self, *fields: str, is_dict: bool) -> str | list[str] | dict[str, str]:
+    def get_item(
+        self, *fields: str, is_dict: bool
+    ) -> str | list[str] | dict[str, str] | bool:
         names = self._get_name(*fields)
         name = ".".join(names)
         if is_dict:
             d = {
                 k[len(name) + 1 :]: str(v)
                 for k, v in self.settings.items()
                 if k.startswith(f"{name}.")
@@ -356,38 +361,38 @@
             return self.settings[name]
 
         msg = f"{name!r} not found in configuration settings"
         raise KeyError(msg)
 
     @classmethod
     def convert(
-        cls, item: str | list[str] | dict[str, str], target: type[Any]
+        cls, item: str | list[str] | dict[str, str] | bool, target: type[Any]
     ) -> object:
         target, _ = _process_annotated(target)
         raw_target = _get_target_raw_type(target)
         if dataclasses.is_dataclass(raw_target):
             msg = f"Array of dataclasses are not supported in configuration settings ({raw_target})"
             raise TypeError(msg)
         if raw_target is list:
             if isinstance(item, list):
                 return [cls.convert(i, _get_inner_type(target)) for i in item]
-            if isinstance(item, dict):
+            if isinstance(item, (dict, bool)):
                 msg = f"Expected {target}, got {type(item).__name__}"
                 raise TypeError(msg)
             return [
                 cls.convert(i.strip(), _get_inner_type(target)) for i in item.split(";")
             ]
         if raw_target is dict:
-            assert not isinstance(item, (str, list))
+            assert not isinstance(item, (str, list, bool))
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in item.items()}
         if isinstance(item, (list, dict)):
             msg = f"Expected {target}, got {type(item).__name__}"
             raise TypeError(msg)
         if raw_target is bool:
-            return _process_bool(item)
+            return item if isinstance(item, bool) else _process_bool(item)
         if raw_target is Union and str in get_args(target):
             return item
         if raw_target is Literal:
             if item not in get_args(_process_union(target)):
                 msg = f"{item!r} not in {get_args(_process_union(target))!r}"
                 raise TypeError(msg)
             return item
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.9.0/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 def _validate_settings() -> None:
-    settings = SettingsReader.from_file("pyproject.toml", {}).settings
+    settings = SettingsReader.from_file("pyproject.toml").settings
 
     assert (
         not settings.wheel.expand_macos_universal_tags
     ), "wheel.expand_macos_universal_tags is not supported in setuptools mode"
     assert (
         settings.logging.level == "WARNING"
     ), "Logging is not adjustable in setuptools mode yet"
@@ -108,15 +108,15 @@
         assert bdist_wheel is not None
         limited_api = bdist_wheel.py_limited_api  # type: ignore[attr-defined]
 
         # TODO: this is a hack due to moving temporary paths for isolation
         if build_temp.exists():
             shutil.rmtree(build_temp)
 
-        settings = SettingsReader.from_file("pyproject.toml", {}).settings
+        settings = SettingsReader.from_file("pyproject.toml").settings
 
         cmake = CMake.default_search(version=settings.cmake.version)
 
         config = CMaker(
             cmake,
             source_dir=Path(source_dir),
             build_dir=build_temp,
@@ -194,15 +194,15 @@
 
 def _prepare_build_cmake_command(dist: Distribution) -> None:
     # Prepare new build_cmake command and make sure build calls it
     build = dist.get_command_class("build")
     assert build is not None
     if "build_cmake" not in {x for x, _ in build.sub_commands}:
         build.sub_commands.append(
-            ("build_cmake", lambda cmd: _has_cmake(cmd.distribution))  # type: ignore[arg-type]
+            ("build_cmake", lambda cmd: _has_cmake(cmd.distribution))
         )
 
 
 def cmake_args(
     _dist: Distribution, attr: Literal["cmake_args"], value: list[str]
 ) -> None:
     assert attr == "cmake_args"
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.9.0/src/scikit_build_core/setuptools/build_meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,38 +38,38 @@
 
 def get_requires_for_build_sdist(
     config_settings: dict[str, str | list[str]] | None = None,
 ) -> list[str]:
     setuptools_reqs = setuptools.build_meta.get_requires_for_build_sdist(
         config_settings
     )
-    requires = GetRequires(config_settings)
+    requires = GetRequires.from_config_settings(config_settings)
 
     # These are only injected if cmake is required for the SDist step
     cmake_requires = (
         [*requires.cmake(), *requires.ninja()] if requires.settings.sdist.cmake else []
     )
     return [*setuptools_reqs, *cmake_requires]
 
 
 def get_requires_for_build_wheel(
     config_settings: dict[str, str | list[str]] | None = None,
 ) -> list[str]:
-    requires = GetRequires(config_settings)
+    requires = GetRequires.from_config_settings(config_settings)
 
     setuptools_reqs = setuptools.build_meta.get_requires_for_build_wheel(
         config_settings
     )
 
     return [*setuptools_reqs, *requires.cmake(), *requires.ninja()]
 
 
 if hasattr(setuptools.build_meta, "get_requires_for_build_editable"):
 
     def get_requires_for_build_editable(
         config_settings: dict[str, str | list[str]] | None = None,
     ) -> list[str]:
-        requires = GetRequires(config_settings)
+        requires = GetRequires.from_config_settings(config_settings)
         setuptools_reqs = setuptools.build_meta.get_requires_for_build_editable(
             config_settings
         )
         return [*setuptools_reqs, *requires.cmake(), *requires.ninja()]
```

### Comparing `scikit_build_core-0.8.2/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.9.0/src/scikit_build_core/setuptools/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     cmake_source_dir: str = "",
     cmake_with_sdist: bool = False,
     cmake_languages: Sequence[str] | None = None,
     cmake_minimum_required_version: str | None = None,
     cmake_process_manifest_hook: Callable[[list[str]], list[str]] | None = None,
     cmake_install_target: str = "install",
     **kw: Any,
-) -> None:
+) -> setuptools.Distribution:
     assert not cmake_install_dir, "cmake_install_dir not supported yet"
     assert not cmake_with_sdist, "cmake_with_sdist not supported yet"
     assert (
         cmake_process_manifest_hook is None
     ), "cmake_process_manifest_hook not supported yet"
     assert cmake_install_target == "install", "cmake_install_target not supported yet"
```

### Comparing `scikit_build_core-0.8.2/tests/conftest.py` & `scikit_build_core-0.9.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         [
             sys.executable,
             "-m",
             "pip",
             "wheel",
             "--wheel-dir",
             str(wheelhouse),
-            f"{BASE}[pyproject]",
+            f"{BASE}",
         ],
         check=True,
     )
     packages = [
         "build",
         "cython",
         "hatchling",
@@ -92,20 +92,18 @@
             self.execute("import sysconfig; print(sysconfig.get_path('platlib'))")
         )
         self.purelib = Path(
             self.execute("import sysconfig; print(sysconfig.get_path('purelib'))")
         )
 
     @overload
-    def run(self, *args: str, capture: Literal[True]) -> str:
-        ...
+    def run(self, *args: str, capture: Literal[True]) -> str: ...
 
     @overload
-    def run(self, *args: str, capture: Literal[False] = ...) -> None:
-        ...
+    def run(self, *args: str, capture: Literal[False] = ...) -> None: ...
 
     def run(self, *args: str, capture: bool = False) -> str | None:
         __tracebackhide__ = True
         env = os.environ.copy()
         paths = {str(self.executable.parent)}
         env["PATH"] = os.pathsep.join([*paths, env["PATH"]])
         env["VIRTUAL_ENV"] = str(self.env_dir)
@@ -206,18 +204,18 @@
 
 @pytest.fixture()
 def package_simple_pyproject_ext(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch
 ) -> PackageInfo:
     package = PackageInfo(
         "simple_pyproject_ext",
-        "6c5bb5f1b6c44f3aab37fc8f768004f644c24001ad0304759a69b754ca6ad46d",
-        "ba13e4195ae6333459412bc802ba8c02c231cf1c5ee143f6a3392786d80a49b4",
-        "f1a6050eae910de7cd86830ba97af5e74ff953f9acc2adab47aa9cdf2a3eca91",
-        "b861db81fd1de6dee4a0d6574af27af54424fbccce12b018644d1db136f218ac",
+        "5544d96810ce60ac40baf28cf8caf2e1e7e1fa7439b283d3fb52cdc1f87f12ac",
+        "aaa15c185dc3fbc301dc2fca937cc935442c38e55bc400fbefd424bd6ce92adb",
+        "ee3a564a37c42df3abdcee3862175baceeb6f6eff0b29931681b424ec5d96067",
+        "4c1d402621e7f00fce4ce5afdb73a9ba4cc25cd4bb57619113432841f779dd68",
     )
     process_package(package, tmp_path, monkeypatch)
     return package
 
 
 @pytest.fixture()
 def package_simple_pyproject_source_dir(
@@ -263,14 +261,21 @@
 ) -> PackageInfo:
     package = PackageInfo("dynamic_metadata")
     process_package(package, tmp_path, monkeypatch)
     return package
 
 
 @pytest.fixture()
+def package_hatchling(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> PackageInfo:
+    package = PackageInfo("hatchling")
+    process_package(package, tmp_path, monkeypatch)
+    return package
+
+
+@pytest.fixture()
 def package_simplest_c(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> PackageInfo:
     package = PackageInfo(
         "simplest_c",
     )
     process_package(package, tmp_path, monkeypatch)
     return package
```

### Comparing `scikit_build_core-0.8.2/tests/test_builder.py` & `scikit_build_core-0.9.0/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     assert get_python_include_dir().is_dir()
 
 
 @pytest.mark.xfail(
     strict=False, reason="Doesn't matter if this fails, usually not used"
 )
 def test_get_python_library():
-    pprint.pprint(sysconfig.get_config_vars())
+    pprint.pprint(
+        {
+            k: v
+            for k, v in sysconfig.get_config_vars().items()
+            if isinstance(v, str) and 128 > len(v) > 2 and not k.startswith("MODULE")
+        }
+    )
 
     lib = get_python_library({})
     if sysconfig.get_platform().startswith("win"):
         assert lib
         assert lib.is_file()
     else:
         assert lib is None
```

### Comparing `scikit_build_core-0.8.2/tests/test_cmake_config.py` & `scikit_build_core-0.9.0/tests/test_cmake_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,16 +28,22 @@
     if init:
         cmake_init = config.build_dir / "CMakeInit.txt"
         yield f"-C{cmake_init}"
 
 
 @pytest.mark.configure()
 def test_init_cache(fp, tmp_path):
-    fp.register([fp.program("cmake"), "--version"], stdout="3.14.0")
-    fp.register([fp.program("cmake3"), "--version"], stdout="3.14.0")
+    fp.register(
+        [fp.program("cmake"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
+    fp.register(
+        [fp.program("cmake3"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
 
     config = CMaker(
         CMake.default_search(),
         source_dir=DIR / "packages/simple_pure",
         build_dir=tmp_path / "build",
         build_type="Release",
     )
@@ -62,26 +68,38 @@
 """
     )
 
 
 @pytest.mark.configure()
 def test_too_old(fp, monkeypatch):
     monkeypatch.setattr(shutil, "which", lambda _: None)
-    fp.register([fp.program("cmake"), "--version"], stdout="3.14.0")
-    fp.register([fp.program("cmake3"), "--version"], stdout="3.14.0")
+    fp.register(
+        [fp.program("cmake"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
+    fp.register(
+        [fp.program("cmake3"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
 
     with pytest.raises(CMakeNotFoundError) as excinfo:
         CMake.default_search(version=SpecifierSet(">=3.15"))
     assert "Could not find CMake with version >=3.15" in excinfo.value.args[0]
 
 
 @pytest.mark.configure()
 def test_cmake_args(tmp_path, fp):
-    fp.register([fp.program("cmake"), "--version"], stdout="3.15.0")
-    fp.register([fp.program("cmake3"), "--version"], stdout="3.15.0")
+    fp.register(
+        [fp.program("cmake"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.15.0"}}',
+    )
+    fp.register(
+        [fp.program("cmake3"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.15.0"}}',
+    )
 
     config = CMaker(
         CMake.default_search(),
         source_dir=DIR / "packages/simple_pure",
         build_dir=tmp_path / "build",
         build_type="Release",
     )
@@ -95,16 +113,22 @@
     config.configure(cmake_args=["-DSOMETHING=one"])
 
     assert len(fp.calls) == 2
 
 
 @pytest.mark.configure()
 def test_cmake_paths(tmp_path, fp):
-    fp.register([fp.program("cmake"), "--version"], stdout="3.15.0")
-    fp.register([fp.program("cmake3"), "--version"], stdout="3.15.0")
+    fp.register(
+        [fp.program("cmake"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.15.0"}}',
+    )
+    fp.register(
+        [fp.program("cmake3"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.15.0"}}',
+    )
 
     config = CMaker(
         CMake.default_search(),
         source_dir=DIR / "packages/simple_pure",
         build_dir=tmp_path / "build",
         build_type="Release",
         prefix_dirs=[tmp_path / "prefix"],
@@ -120,12 +144,14 @@
 
     assert len(fp.calls) == 2
 
 
 def test_get_cmake_via_envvar(monkeypatch: pytest.MonkeyPatch, fp):
     monkeypatch.setattr("shutil.which", lambda x: x)
     cmake_path = Path("some-prog")
-    fp.register([cmake_path, "--version"], stdout="cmake version 3.20.0\n")
+    fp.register(
+        [cmake_path, "-E", "capabilities"], stdout='{"version":{"string":"3.20.0"}}'
+    )
     monkeypatch.setenv("CMAKE_EXECUTABLE", str(cmake_path))
     result = CMake.default_search(env=os.environ)
     assert result.cmake_path == cmake_path
     assert result.version == Version("3.20.0")
```

### Comparing `scikit_build_core-0.8.2/tests/test_custom_modules.py` & `scikit_build_core-0.9.0/tests/test_custom_modules.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 
 DIR = Path(__file__).parent
 PROJECT_DIR = DIR / "packages" / "custom_cmake"
 
 
 def test_ep(isolated):
-    isolated.install("hatchling", "scikit-build-core[pyproject]")
+    isolated.install("hatchling", "scikit-build-core")
     isolated.install(PROJECT_DIR / "extern", isolated=False)
     isolated.install(PROJECT_DIR, "-v", isolated=False)
 
     if sys.platform.startswith("win"):
         # TODO: maybe figure out how to make this work on windows?
         pytest.skip("Can't run script on Windows")
```

### Comparing `scikit_build_core-0.8.2/tests/test_dynamic_metadata.py` & `scikit_build_core-0.9.0/tests/test_dynamic_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import subprocess
 import sys
 import types
 import zipfile
 from pathlib import Path
 from typing import Any
 
-import pyproject_metadata
 import pytest
 from packaging.version import Version
 
 from scikit_build_core._compat import tomllib
+from scikit_build_core._vendor import pyproject_metadata
 from scikit_build_core.build import build_wheel
+from scikit_build_core.build.metadata import get_standard_metadata
 from scikit_build_core.builder.get_requires import GetRequires
 from scikit_build_core.metadata import regex
-from scikit_build_core.settings.metadata import get_standard_metadata
 from scikit_build_core.settings.skbuild_read_settings import SettingsReader
 
 
 # these are mock plugins returning known results
 # it turns out to be easier to create EntryPoint objects pointing to real
 # functions than to mock them.
 def ep_version(
```

### Comparing `scikit_build_core-0.8.2/tests/test_editable.py` & `scikit_build_core-0.9.0/tests/test_editable.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @pytest.mark.xfail(
     sys.version_info[:2] == (3, 9), reason="Python 3.9 not supported yet"
 )
 def test_navigate_editable(isolated, isolate, package):
     isolate_args = ["--no-build-isolation"] if not isolate else []
     isolated.install("pip>=23")
     if not isolate:
-        isolated.install("scikit-build-core[pyproject]")
+        isolated.install("scikit-build-core")
 
     if package:
         init_py = Path("python/shared_pkg/data/__init__.py")
         init_py.touch()
 
     isolated.install(
         "-v", "--config-settings=build-dir=build/{wheel_tag}", *isolate_args, "-e", "."
@@ -69,15 +69,15 @@
     package1 = PackageInfo(
         "cython_pxd_editable/pkg1",
     )
     tmp_path1 = tmp_path / "pkg1"
     tmp_path1.mkdir()
     process_package(package1, tmp_path1, monkeypatch)
 
-    isolated.install("pip>23", "cython", "scikit-build-core[pyproject]")
+    isolated.install("pip>23", "cython", "scikit-build-core")
 
     isolated.install(
         "-v",
         *config_mode_flags,
         "--no-build-isolation",
         *editable_flag,
         ".",
```

### Comparing `scikit_build_core-0.8.2/tests/test_editable_redirect.py` & `scikit_build_core-0.9.0/tests/test_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_editable_unit.py` & `scikit_build_core-0.9.0/tests/test_editable_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,16 @@
 
     # Create a fake editable install
     packages = ["pkg"]
     mapping = packages_to_file_mapping(
         packages=packages,
         platlib_dir=site_packages,
         include=[],
-        exclude=[],
+        src_exclude=[],
+        target_exclude=[],
     )
     assert mapping == {
         str(Path("pkg/__init__.py")): str(pkg_dir / "__init__.py"),
         str(Path("pkg/module.py")): str(pkg_dir / "module.py"),
         str(Path("pkg/namespace/module.py")): str(pkg_dir / "namespace/module.py"),
         str(Path("pkg/subpkg/__init__.py")): str(pkg_dir / "subpkg/__init__.py"),
         str(Path("pkg/subpkg/module.py")): str(pkg_dir / "subpkg/module.py"),
```

### Comparing `scikit_build_core-0.8.2/tests/test_file_processor.py` & `scikit_build_core-0.9.0/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_fileapi.py` & `scikit_build_core-0.9.0/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_fortran.py` & `scikit_build_core-0.9.0/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_generator_default.py` & `scikit_build_core-0.9.0/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_get_requires.py` & `scikit_build_core-0.9.0/tests/test_get_requires.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,41 +44,53 @@
             return None
         return orig_find_spec(name, package)
 
     monkeypatch.setattr(importlib.util, "find_spec", find_spec)
 
 
 def test_get_requires_parts(fp):
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
     assert set(GetRequires().cmake()) == {"cmake>=3.15"}
     assert set(GetRequires().ninja()) == {*ninja}
 
 
 def test_get_requires_parts_uneeded(fp):
-    fp.register([Path("cmake/path"), "--version"], stdout="3.18.0")
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.18.0"}}',
+    )
     assert set(GetRequires().cmake()) == set()
     assert set(GetRequires().ninja()) == {*ninja}
 
 
 def test_get_requires_parts_settings(fp):
-    fp.register([Path("cmake/path"), "--version"], stdout="3.18.0")
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.18.0"}}',
+    )
     config = {"cmake.version": ">=3.20"}
-    assert set(GetRequires(config).cmake()) == {"cmake>=3.20"}
-    assert set(GetRequires(config).ninja()) == {*ninja}
+    assert set(GetRequires.from_config_settings(config).cmake()) == {"cmake>=3.20"}
+    assert set(GetRequires.from_config_settings(config).ninja()) == {*ninja}
 
 
 def test_get_requires_parts_pyproject(fp, monkeypatch, tmp_path):
     monkeypatch.chdir(tmp_path)
     tmp_path.joinpath("pyproject.toml").write_text(
         """
         [tool.scikit-build.cmake]
         version = ">=3.21"
         """
     )
-    fp.register([Path("cmake/path"), "--version"], stdout="3.18.0")
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.18.0"}}',
+    )
 
     assert set(GetRequires().cmake()) == {"cmake>=3.21"}
     assert set(GetRequires().ninja()) == {*ninja}
 
 
 def test_get_requires_parts_pyproject_old(fp, monkeypatch, tmp_path):
     monkeypatch.chdir(tmp_path)
@@ -86,46 +98,65 @@
         """
         
         [tool.scikit-build]
         minimum-version = "0.0"
         cmake.minimum-version = "3.21"
         """
     )
-    fp.register([Path("cmake/path"), "--version"], stdout="3.18.0")
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.18.0"}}',
+    )
 
     assert set(GetRequires().cmake()) == {"cmake>=3.21"}
     assert set(GetRequires().ninja()) == {*ninja}
 
 
 def test_get_requires_for_build_sdist(fp):
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
-    assert set(get_requires_for_build_sdist({})) == {"pathspec", "pyproject_metadata"}
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
+    assert set(get_requires_for_build_sdist({})) == set()
 
 
 def test_get_requires_for_build_sdist_cmake(fp):
-    expected = {"pathspec", "pyproject_metadata", "cmake>=3.15", *ninja}
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
+    expected = {"cmake>=3.15", *ninja}
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
     assert set(get_requires_for_build_sdist({"sdist.cmake": "True"})) == expected
 
 
 def test_get_requires_for_build_wheel(fp):
-    expected = {"pathspec", "pyproject_metadata", "cmake>=3.15", *ninja}
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
+    expected = {"cmake>=3.15", *ninja}
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
     assert set(get_requires_for_build_wheel({})) == expected
 
 
 def test_get_requires_for_build_wheel_pure(fp):
-    expected = {"pathspec", "pyproject_metadata"}
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
-    assert set(get_requires_for_build_wheel({"wheel.cmake": "False"})) == expected
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
+    assert set(get_requires_for_build_wheel({"wheel.cmake": "False"})) == set()
 
 
 def test_get_requires_for_build_editable(fp):
-    expected = {"pathspec", "pyproject_metadata", "cmake>=3.15", *ninja}
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
+    expected = {"cmake>=3.15", *ninja}
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
     assert set(get_requires_for_build_editable({})) == expected
 
 
 def test_get_requires_for_build_editable_pure(fp):
-    expected = {"pathspec", "pyproject_metadata"}
-    fp.register([Path("cmake/path"), "--version"], stdout="3.14.0")
-    assert set(get_requires_for_build_editable({"wheel.cmake": "False"})) == expected
+    fp.register(
+        [Path("cmake/path"), "-E", "capabilities"],
+        stdout='{"version":{"string":"3.14.0"}}',
+    )
+    assert set(get_requires_for_build_editable({"wheel.cmake": "False"})) == set()
```

### Comparing `scikit_build_core-0.8.2/tests/test_json_schema.py` & `scikit_build_core-0.9.0/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_logging.py` & `scikit_build_core-0.9.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_module_dir.py` & `scikit_build_core-0.9.0/tests/test_module_dir.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,18 @@
             yield package_name
 
 
 def test_all_modules_filter_all():
     all_modules = on_all_modules("scikit_build_core", pkg=False)
     all_modules = (n for n in all_modules if not n.split(".")[-1].startswith("__"))
     for name in all_modules:
-        module = importlib.import_module(name)
+        try:
+            module = importlib.import_module(name)
+        except ModuleNotFoundError:
+            continue
 
         try:
             dir_module = set(dir(module))
         except Exception:
             print(f"dir() failed on {name}")
             raise
         items = ["annotations", "os", "sys"]
@@ -43,13 +46,16 @@
             assert item not in dir_module, f"{module.__file__} has {item!r}"
 
 
 def test_all_modules_has_all():
     all_modules = on_all_modules("scikit_build_core", pkg=True)
     all_modules = (n for n in all_modules if not n.split(".")[-1].startswith("_"))
     for name in all_modules:
-        module = importlib.import_module(name)
+        try:
+            module = importlib.import_module(name)
+        except ModuleNotFoundError:
+            continue
 
         dir_module = module.__dict__
         items = ["__all__"]
         for item in items:
             assert item in dir_module, f"{module.__file__} missing {item!r}"
```

### Comparing `scikit_build_core-0.8.2/tests/test_name_main.py` & `scikit_build_core-0.9.0/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_process_scripts.py` & `scikit_build_core-0.9.0/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_program_search.py` & `scikit_build_core-0.9.0/tests/test_program_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 
 
 def test_get_cmake_programs_all(monkeypatch, fp):
     monkeypatch.setattr("shutil.which", lambda x: x)
     cmake_path = Path("cmake")
     cmake3_path = Path("cmake3")
     fp.register(
-        [cmake_path, "--version"],
-        stdout="cmake version 3.20.0\n\nCMake suite maintained and supported by Kitware (kitware.com/cmake).",
+        [cmake_path, "-E", "capabilities"],
+        stdout='{"version":{"string":"3.20.0"}}',
     )
     fp.register(
-        [cmake3_path, "--version"],
-        stdout="cmake version 3.19.0\n\nCMake suite maintained and supported by Kitware (kitware.com/cmake).",
+        [cmake3_path, "-E", "capabilities"],
+        stdout='{"version":{"string":"3.19.0"}}',
     )
     programs = list(get_cmake_programs(module=False))
     assert len(programs) == 2
     assert programs[0].path.name == "cmake3"
     assert programs[0].version == Version("3.19.0")
     assert programs[1].path.name == "cmake"
     assert programs[1].version == Version("3.20.0")
@@ -88,21 +88,28 @@
 
 
 def test_get_cmake_programs_malformed(monkeypatch, fp, caplog):
     caplog.set_level(logging.WARNING)
     monkeypatch.setattr("shutil.which", lambda x: x)
     cmake_path = Path("cmake")
     cmake3_path = Path("cmake3")
-    fp.register([cmake_path, "--version"], stdout="scrambled output\n")
-    fp.register([cmake3_path, "--version"], stdout="cmake version 3.17.3\n")
+    fp.register([cmake_path, "-E", "capabilities"], stdout="scrambled output\n")
+    fp.register([cmake3_path, "-E", "capabilities"], stdout="{}")
     programs = list(get_cmake_programs(module=False))
     assert caplog.records
     assert "Could not determine CMake version" in str(caplog.records[0].msg)
+    assert "Could not determine CMake version" in str(caplog.records[1].msg)
     assert len(programs) == 2
 
+    fp.register([cmake_path, "-E", "capabilities"], stdout="scrambled output\n")
+    fp.register(
+        [cmake3_path, "-E", "capabilities"], stdout='{"version":{"string":"3.17.3"}}'
+    )
+    programs = list(get_cmake_programs(module=False))
+
     best_none = best_program(programs, version=None)
     assert best_none
     assert best_none.path.name == "cmake3"
 
     best_3_15 = best_program(programs, version=SpecifierSet(">=3.15"))
     assert best_3_15
     assert best_3_15.path.name == "cmake3"
```

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_abi3.py` & `scikit_build_core-0.9.0/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.9.0/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_pep517.py` & `scikit_build_core-0.9.0/tests/test_pyproject_pep517.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 import time
 import zipfile
 from pathlib import Path
 
 import build.util
 import pytest
 
-from scikit_build_core.build import _file_processor, build_sdist, build_wheel
+from scikit_build_core._compat.importlib.metadata import PathDistribution
+from scikit_build_core.build import (
+    _file_processor,
+    build_sdist,
+    build_wheel,
+    prepare_metadata_for_build_wheel,
+)
 
 ENTRYPOINTS = """\
 [one.two]
 three = four
 
 [console_scripts]
 something = other
@@ -288,14 +294,35 @@
     answer = {
         "Metadata-Version": "2.1",
         "Name": "CMake.Example",
         "Version": "0.0.1",
         "Requires-Python": ">=3.7",
         "Provides-Extra": "test",
         "Requires-Dist": 'pytest>=6.0; extra == "test"',
-        "License-File": "LICENSE",
     }
 
     for k, b in answer.items():
-        assert metadata[k] == b
+        assert metadata.get(k, None) == b
+
+    assert len(metadata) == len(answer)
+
+
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_prepare_metdata_for_build_wheel_by_hand(tmp_path):
+    mddir = tmp_path / "dist"
+    mddir.mkdir()
+    out = prepare_metadata_for_build_wheel(str(mddir), {})
+    print("Metadata dir:", (mddir / out).resolve())
+    metadata = PathDistribution(mddir / out).metadata
+    answer = {
+        "Metadata-Version": "2.1",
+        "Name": "CMake.Example",
+        "Version": "0.0.1",
+        "Requires-Python": ">=3.7",
+        "Provides-Extra": "test",
+        "Requires-Dist": 'pytest>=6.0; extra == "test"',
+    }
+
+    for k, b in answer.items():
+        assert metadata.get(k, None) == b
 
     assert len(metadata) == len(answer)
```

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_pep518.py` & `scikit_build_core-0.9.0/tests/test_pyproject_pep518.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 
     version = isolated.execute("import output; print(output.version)")
     assert version == "0.1.0"
 
     assert cleanup_overwrite.is_file()
 
 
+@pytest.mark.network()
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.usefixtures("package_simple_pyproject_ext")
 @pytest.mark.parametrize(
     "build_args", [(), ("--wheel",)], ids=["sdist_to_wheel", "wheel_directly"]
 )
@@ -192,14 +193,15 @@
     version = isolated.execute("import cmake_example; print(cmake_example.__version__)")
     assert version == "0.0.1"
 
     add = isolated.execute("import cmake_example; print(cmake_example.add(1, 2))")
     assert add == "3"
 
 
+@pytest.mark.network()
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.parametrize(
     "build_args", [(), ("--wheel",)], ids=["sdist_to_wheel", "wheel_directly"]
 )
 @pytest.mark.usefixtures("package_simple_pyproject_ext")
@@ -238,14 +240,15 @@
 
     isolated.install(wheel)
 
     version = isolated.execute("import cmake_example; print(cmake_example.__version__)")
     assert version == "0.0.1"
 
 
+@pytest.mark.network()
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.usefixtures("package_simple_pyproject_ext")
 def test_pep518_pip(isolated):
     isolated.install("-v", ".")
```

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_pep660.py` & `scikit_build_core-0.9.0/tests/test_pyproject_pep660.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 @pytest.mark.integration()
 @pytest.mark.parametrize("isolate", [True, False], ids=["isolated", "not_isolated"])
 @pytest.mark.usefixtures("package_simplest_c")
 def test_pep660_pip_isolated(isolated, isolate, editable_mode: str):
     isolate_args = ["--no-build-isolation"] if not isolate else []
     isolated.install("pip>=23")
     if not isolate:
-        isolated.install("scikit-build-core[pyproject]")
+        isolated.install("scikit-build-core")
 
     build_dir = "" if editable_mode == "inplace" else "build/{wheel_tag}"
 
     isolated.install(
         "-v",
         f"--config-settings=build-dir={build_dir}",
         f"--config-settings=editable.mode={editable_mode}",
```

### Comparing `scikit_build_core-0.8.2/tests/test_pyproject_purelib.py` & `scikit_build_core-0.9.0/tests/test_pyproject_purelib.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_schema.py` & `scikit_build_core-0.9.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_settings.py` & `scikit_build_core-0.9.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,24 @@
 
     settings = sources.convert_target(SettingBools)
 
     assert settings.false
     assert not settings.true
 
 
+def test_conf_settings_bools():
+    sources = SourceChain(
+        ConfSource(settings={"false": True, "true": False}),
+    )
+    settings = sources.convert_target(SettingBools)
+
+    assert settings.false
+    assert not settings.true
+
+
 @dataclasses.dataclass
 class SettingLists:
     list0: List[str] = dataclasses.field(default_factory=list)
     list1: List[str] = dataclasses.field(default_factory=list)
     list2: List[str] = dataclasses.field(default_factory=list)
     list3: List[str] = dataclasses.field(default_factory=list)
     list4: List[str] = dataclasses.field(default_factory=list)
```

### Comparing `scikit_build_core-0.8.2/tests/test_settings_overrides.py` & `scikit_build_core-0.9.0/tests/test_settings_overrides.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             cmake.define.SPAM = "EGGS"
             sdist.cmake = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if python_version == "3.10":
         assert settings.cmake.args == ["-DFOO=BAR"]
         assert settings.cmake.define == {"SPAM": "EGGS"}
         assert settings.experimental
         assert settings.sdist.cmake
@@ -73,15 +73,15 @@
             if.platform-system = "darwin"
             install.components = ["bindings"]
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if implementation_name == "pypy" and platform_system == "darwin":
         assert not settings.editable.verbose
         assert settings.install.components == ["headers"]
     elif implementation_name == "cpython" and platform_system == "darwin":
         assert settings.editable.verbose
@@ -118,15 +118,15 @@
             if.any.platform-system = "darwin"
             install.components = ["bindings"]
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if implementation_name == "cpython" or platform_system == "darwin":
         assert settings.editable.verbose == (
             platform_system == "linux" and implementation_name == "cpython"
         )
         assert settings.install.components == ["bindings"]
@@ -164,15 +164,15 @@
             editable.verbose = false
             install.components = ["headers"]
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if python_version == "3.10" and (
         implementation_name == "pypy" or platform_system == "darwin"
     ):
         assert not settings.editable.verbose
         assert settings.install.components == ["headers"]
@@ -194,15 +194,15 @@
             if.platform-node = "^match"
             experimental = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if platform_node == "matchthat":
         assert settings.experimental
     else:
         assert not settings.experimental
 
@@ -230,15 +230,15 @@
             if = {platform_machine = "x86_32"}
             install.components = ["headers_32"]
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if platform_machine == "x86_64":
         assert settings.install.components == ["headers"]
     elif platform_machine == "x86_32":
         assert settings.install.components == ["headers_32"]
     else:
@@ -256,15 +256,15 @@
             minimum-version="0.1"
             """
         ),
         encoding="utf-8",
     )
 
     with pytest.raises(KeyError, match="At least one 'if' override must be provided"):
-        SettingsReader.from_file(pyproject_toml, {})
+        SettingsReader.from_file(pyproject_toml)
 
 
 def test_skbuild_overrides_empty_if(
     tmp_path: Path,
 ):
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(
@@ -275,15 +275,15 @@
             minimum-version="0.1"
             """
         ),
         encoding="utf-8",
     )
 
     with pytest.raises(KeyError, match="At least one 'if' override must be provided"):
-        SettingsReader.from_file(pyproject_toml, {})
+        SettingsReader.from_file(pyproject_toml)
 
 
 def test_skbuild_overrides_invalid_key(
     tmp_path: Path,
 ):
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(
@@ -293,15 +293,15 @@
             if = {python_version = ">=3"}
             invalid-key = "Hi"
             """
         ),
         encoding="utf-8",
     )
 
-    settings = SettingsReader.from_file(pyproject_toml, {})
+    settings = SettingsReader.from_file(pyproject_toml)
     with pytest.raises(SystemExit):
         settings.validate_may_exit()
 
 
 @pytest.mark.parametrize("regex", ["is", "this", "^this", "string$"])
 def test_regex_match(regex: str):
     assert regex_match("this_is_a_string", regex)
@@ -329,15 +329,15 @@
             if.env.FOO = "BAR"
             sdist.cmake = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if envvar == "BAR":
         assert settings.sdist.cmake
     else:
         assert not settings.sdist.cmake
 
@@ -359,15 +359,15 @@
             if.env.FOO = true
             sdist.cmake = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if envvar in {"tRUE", "3"}:
         assert settings.sdist.cmake
     else:
         assert not settings.sdist.cmake
 
@@ -391,15 +391,15 @@
             if{any_str}.env.BAR = true
             sdist.cmake = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {})
+    settings_reader = SettingsReader.from_file(pyproject_toml)
     settings = settings_reader.settings
 
     if (foo == "true" and bar == "true") or (any and (foo == "true" or bar == "true")):
         assert settings.sdist.cmake
     else:
         assert not settings.sdist.cmake
 
@@ -414,14 +414,79 @@
             if.state = "{state}"
             experimental = true
             """
         ),
         encoding="utf-8",
     )
 
-    settings_reader = SettingsReader.from_file(pyproject_toml, {}, state="wheel")
+    settings_reader = SettingsReader.from_file(pyproject_toml, state="wheel")
     settings = settings_reader.settings
 
     if state == "wheel":
         assert settings.experimental
     else:
         assert not settings.experimental
+
+
+@pytest.mark.parametrize("inherit", ["none", "append", "prepend"])
+def test_skbuild_overrides_inherit(inherit: str, tmp_path: Path):
+    pyproject_toml = tmp_path / "pyproject.toml"
+    pyproject_toml.write_text(
+        dedent(
+            f"""\
+            [tool.scikit-build]
+            cmake.args = ["a", "b"]
+            cmake.targets = ["a", "b"]
+            wheel.packages = ["a", "b"]
+            wheel.license-files = ["a.txt", "b.txt"]
+            wheel.exclude = ["x", "y"]
+            install.components = ["a", "b"]
+            cmake.define = {{a="A", b="B"}}
+
+            [[tool.scikit-build.overrides]]
+            if.state = "wheel"
+            inherit.cmake.args = "{inherit}"
+            inherit.cmake.targets = "{inherit}"
+            inherit.wheel.packages = "{inherit}"
+            inherit.wheel.license-files = "{inherit}"
+            inherit.wheel.exclude = "{inherit}"
+            inherit.install.components = "{inherit}"
+            inherit.cmake.define = "{inherit}"
+            cmake.args = ["c", "d"]
+            cmake.targets = ["c", "d"]
+            wheel.packages = ["c", "d"]
+            wheel.license-files = ["c.txt", "d.txt"]
+            wheel.exclude = ["xx", "yy"]
+            install.components = ["c", "d"]
+            cmake.define = {{b="X", c="C"}}
+            """
+        ),
+        encoding="utf-8",
+    )
+
+    settings_reader = SettingsReader.from_file(pyproject_toml, state="wheel")
+    settings = settings_reader.settings
+
+    if inherit == "none":
+        assert settings.cmake.args == ["c", "d"]
+        assert settings.cmake.targets == ["c", "d"]
+        assert settings.wheel.packages == ["c", "d"]
+        assert settings.wheel.license_files == ["c.txt", "d.txt"]
+        assert settings.wheel.exclude == ["xx", "yy"]
+        assert settings.install.components == ["c", "d"]
+        assert settings.cmake.define == {"b": "X", "c": "C"}
+    elif inherit == "append":
+        assert settings.cmake.args == ["a", "b", "c", "d"]
+        assert settings.cmake.targets == ["a", "b", "c", "d"]
+        assert settings.wheel.packages == ["a", "b", "c", "d"]
+        assert settings.wheel.license_files == ["a.txt", "b.txt", "c.txt", "d.txt"]
+        assert settings.wheel.exclude == ["x", "y", "xx", "yy"]
+        assert settings.install.components == ["a", "b", "c", "d"]
+        assert settings.cmake.define == {"a": "A", "b": "X", "c": "C"}
+    elif inherit == "prepend":
+        assert settings.cmake.args == ["c", "d", "a", "b"]
+        assert settings.cmake.targets == ["c", "d", "a", "b"]
+        assert settings.wheel.packages == ["c", "d", "a", "b"]
+        assert settings.wheel.license_files == ["c.txt", "d.txt", "a.txt", "b.txt"]
+        assert settings.wheel.exclude == ["xx", "yy", "x", "y"]
+        assert settings.install.components == ["c", "d", "a", "b"]
+        assert settings.cmake.define == {"a": "A", "b": "B", "c": "C"}
```

### Comparing `scikit_build_core-0.8.2/tests/test_setuptools_abi3.py` & `scikit_build_core-0.9.0/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_setuptools_pep517.py` & `scikit_build_core-0.9.0/tests/test_setuptools_pep517.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,21 +26,22 @@
     )
     metadata_set = set(correct_metadata.strip().splitlines())
 
     dist = Path("dist")
     out = build_sdist("dist")
 
     (sdist,) = dist.iterdir()
-    assert sdist.name == "cmake-example-0.0.1.tar.gz"
+    assert sdist.name in {"cmake-example-0.0.1.tar.gz", "cmake_example-0.0.1.tar.gz"}
     assert sdist == dist / out
+    cmake_example = sdist.name[:13]
 
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
         assert file_names == {
-            f"cmake-example-0.0.1/{x}"
+            f"{cmake_example}-0.0.1/{x}"
             for x in (
                 # TODO: "CMakeLists.txt",
                 "PKG-INFO",
                 "src",
                 "src/cmake_example.egg-info",
                 "src/cmake_example.egg-info/PKG-INFO",
                 "src/cmake_example.egg-info/SOURCES.txt",
@@ -50,16 +51,16 @@
                 "src/cmake_example.egg-info/top_level.txt",
                 "pyproject.toml",
                 "setup.cfg",
                 "setup.py",
                 "LICENSE",
                 # TODO: "src/main.cpp",
             )
-        } | {"cmake-example-0.0.1"}
-        pkg_info = f.extractfile("cmake-example-0.0.1/PKG-INFO")
+        } | {f"{cmake_example}-0.0.1"}
+        pkg_info = f.extractfile(f"{cmake_example}-0.0.1/PKG-INFO")
         assert pkg_info
         pkg_info_contents = set(pkg_info.read().decode().strip().splitlines())
         assert metadata_set <= pkg_info_contents
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
```

### Comparing `scikit_build_core-0.8.2/tests/test_setuptools_pep518.py` & `scikit_build_core-0.9.0/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_shutil.py` & `scikit_build_core-0.9.0/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_simple_pure.py` & `scikit_build_core-0.9.0/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/test_simplest_c.py` & `scikit_build_core-0.9.0/tests/test_simplest_c.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             "data.txt",
             "excluded.txt",
             "sdist_only.txt",
         }
 
         if not component:
             expected_wheel_files.add("generated_ignored.txt")
+            expected_wheel_files.add("generated_no_wheel.txt")
 
         if not component or "Generated" in component:
             expected_wheel_files.add("generated.txt")
 
         assert len(filtered_pkg) == len(simplest_pkg) - 2
         assert {"simplest-0.0.1.dist-info", "simplest"} == file_names
         assert expected_wheel_files == filtered_pkg
@@ -106,41 +107,65 @@
         shutil.rmtree("dist")
 
     out = build_wheel(
         str(dist),
         {
             "sdist.include": "src/simplest/*included*.txt",
             "sdist.exclude": "src/simplest/*excluded*.txt",
-            "wheel.exclude": "src/simplest/sdist_only.txt",
+            "wheel.exclude": [
+                "simplest/sdist_only.txt",
+                "simplest/generated_no_wheel.txt",
+            ],
             "wheel.packages": ["src/simplest", "src/not_a_package"],
         },
     )
 
     (wheel,) = dist.glob("simplest-0.0.1-*.whl")
     assert wheel == dist / out
 
     virtualenv.install(wheel)
 
-    if sys.version_info >= (3, 8):
-        with wheel.open("rb") as f:
-            p = zipfile.Path(f)
-            file_names = {x.name for x in p.iterdir()}
-            simplest_pkg = {x.name for x in p.joinpath("simplest").iterdir()}
-            not_a_pkg = {x.name for x in p.joinpath("not_a_package").iterdir()}
+    with wheel.open("rb") as f:
+        file_names = set(zipfile.ZipFile(f).namelist())
 
-        filtered_pkg = {x for x in simplest_pkg if not x.startswith("_module")}
-
-        assert len(filtered_pkg) == len(simplest_pkg) - 2
-        assert {"simplest-0.0.1.dist-info", "simplest", "not_a_package"} == file_names
-        assert {
-            "__init__.py",
-            "data.txt",
-            "ignored_included.txt",
-            "generated.txt",
-            "generated_ignored.txt",
-        } == filtered_pkg
-        assert {"simple.txt"} == not_a_pkg
+    simplest_pkg = {
+        x.split("/", maxsplit=1)[-1] for x in file_names if x.startswith("simplest/")
+    }
+    not_a_pkg = {
+        x.split("/", maxsplit=1)[-1]
+        for x in file_names
+        if x.startswith("not_a_package/")
+    }
+    metadata_items = {
+        x.split("/", maxsplit=1)[-1]
+        for x in file_names
+        if x.startswith("simplest-0.0.1.dist-info/")
+    }
+
+    assert {
+        "licenses/LICENSE.txt",
+        "metadata_file.txt",
+        "RECORD",
+        "METADATA",
+        "WHEEL",
+        "entry_points.txt",
+    } == metadata_items
+
+    filtered_pkg = {x for x in simplest_pkg if not x.startswith("_module")}
+
+    assert len(filtered_pkg) == len(simplest_pkg) - 2
+    assert {"simplest-0.0.1.dist-info", "simplest", "not_a_package"} == {
+        x.split("/")[0] for x in file_names
+    }
+    assert {
+        "__init__.py",
+        "data.txt",
+        "ignored_included.txt",
+        "generated.txt",
+        "generated_ignored.txt",
+    } == filtered_pkg
+    assert {"simple.txt"} == not_a_pkg
 
     version = virtualenv.execute(
         "from simplest import square; print(square(2))",
     )
     assert version == "4.0"
```

### Comparing `scikit_build_core-0.8.2/tests/test_skbuild_settings.py` & `scikit_build_core-0.9.0/tests/test_skbuild_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
     )
 
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(
         "tool.scikit-build.cmake.version = '>=3.21'", encoding="utf-8"
     )
 
-    SettingsReader.from_file(pyproject_toml, {})
+    SettingsReader.from_file(pyproject_toml)
 
     with pytest.raises(SystemExit):
         SettingsReader.from_file(pyproject_toml, {"minimum-version": "0.7"})
 
 
 def test_skbuild_settings_pyproject_toml_envvar_defines(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch
```

### Comparing `scikit_build_core-0.8.2/tests/test_wheelfile_utils.py` & `scikit_build_core-0.9.0/tests/test_wheelfile_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import stat
 import zipfile
 
 from packaging.tags import Tag
-from pyproject_metadata import StandardMetadata
 
 import scikit_build_core.build._wheelfile
+from scikit_build_core._vendor.pyproject_metadata import StandardMetadata
 
 
 def test_wheel_metadata() -> None:
     metadata = scikit_build_core.build._wheelfile.WheelMetadata(
         generator="scikit-build-core 1.2.3"
     )
     assert (
@@ -29,14 +29,15 @@
     out_dir = tmp_path / "out"
 
     wheel = scikit_build_core.build._wheelfile.WheelWriter(
         metadata,
         out_dir,
         {Tag("py3", "none", "any")},
         scikit_build_core.build._wheelfile.WheelMetadata(),
+        None,
     )
     wheel.wheel_metadata.generator = "scikit-build-core 1.2.3"
 
     monkeypatch.setenv("SOURCE_DATE_EPOCH", "315532800")
     assert wheel.timestamp() == (1980, 1, 1, 0, 0, 0)
 
     assert wheel.name_ver == "something-1.2.3"
```

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.9.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.9.0/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.9.0/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
 find_package(
   Python
   COMPONENTS Interpreter Development.Module
   REQUIRED)
 
-find_program(CYTHON "cython")
-
 add_custom_command(
   OUTPUT src/pkg1/one.c
   DEPENDS src/pkg1/one.pyx
   VERBATIM
-  COMMAND "${CYTHON}" "${CMAKE_CURRENT_SOURCE_DIR}/src/pkg1/one.pyx"
-          --output-file "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c")
+  COMMAND
+    Python::Interpreter -m cython
+    "${CMAKE_CURRENT_SOURCE_DIR}/src/pkg1/one.pyx" --output-file
+    "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c")
 
 python_add_library(one MODULE "${CMAKE_CURRENT_BINARY_DIR}/src/pkg1/one.c"
                    WITH_SOABI)
 
 install(TARGETS one DESTINATION pkg1/)
```

### Comparing `scikit_build_core-0.8.2/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.9.0/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.9.0/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/navigate_editable/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/navigate_editable/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/navigate_editable/python/shared_pkg/py_module.py` & `scikit_build_core-0.9.0/tests/packages/navigate_editable/python/shared_pkg/py_module.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/navigate_editable/src/shared_pkg/c_module.c` & `scikit_build_core-0.9.0/tests/packages/navigate_editable/src/shared_pkg/c_module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/sdist_config/CMakeLists.txt` & `scikit_build_core-0.9.0/tests/packages/sdist_config/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 project(
   sdist_config
   LANGUAGES CXX
   VERSION ${SKBUILD_PROJECT_VERSION})
 
 include(FetchContent)
 
+set(PYBIND11_FINDPYTHON ON)
+
 if(NOT SKBUILD_STATE STREQUAL "sdist"
    AND EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/pybind11/CMakeLists.txt")
   message(STATUS "Using integrated pybind11")
-  set(FETCHCONTENT_FULLY_DISCONNECTED ON)
+  add_subdirectory(pybind11)
+else()
+  FetchContent_Declare(
+    pybind11
+    GIT_REPOSITORY https://github.com/pybind/pybind11.git
+    GIT_TAG v2.12.0
+    SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/pybind11)
+  FetchContent_MakeAvailable(pybind11)
 endif()
 
-FetchContent_Declare(
-  pybind11
-  GIT_REPOSITORY https://github.com/pybind/pybind11.git
-  GIT_TAG v2.11.1
-  SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/pybind11)
-
-set(PYBIND11_FINDPYTHON ON)
-FetchContent_MakeAvailable(pybind11)
-
 pybind11_add_module(sdist_config main.cpp)
 install(TARGETS sdist_config DESTINATION .)
 
 # Generation test
 include("${CMAKE_CURRENT_BINARY_DIR}/output.cmake")
 if(NOT "${MY_VERSION}" STREQUAL "${PROJECT_VERSION}")
   message(FATAL_ERROR "Version mismatch: ${MY_VERSION} != ${PROJECT_VERSION}")
```

### Comparing `scikit_build_core-0.8.2/tests/packages/sdist_config/pyproject.toml` & `scikit_build_core-0.9.0/tests/packages/sdist_config/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["scikit-build-core[pyproject]"]
+requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "sdist_config"
 version = "0.1.0"
 
 [tool.scikit-build]
```

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.9.0/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.9.0/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.9.0/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.9.0/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/.gitignore` & `scikit_build_core-0.9.0/tests/packages/hatchling/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/LICENSE` & `scikit_build_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.8.2/README.md` & `scikit_build_core-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,21 @@
 - Wheels are not fully reproducible yet (nor are they in most others systems,
   including setuptools)
 - Several editable mode caveats (mentioned in the docs).
 
 Other backends are also planned:
 
 - Setuptools integration highly experimental
+- Hatchling plugin highly experimental
 - The extensionlib integration is missing
-- No hatchling plugin yet.
 
 The recommended interface is the native pyproject builder. There is also a WIP
 setuptools-based interface that is being developed to provide a transition path
-for classic scikit-build.
+for classic scikit-build, and a WIP Hatchling plugin. Both might be moved to
+standalone packages in the future.
 
 > [!WARNING]
 >
 > Only the pyproject-based builder should be used; the setuptools backend is
 > experimental and likely to move to a separate package before being declared
 > stable, and internal API is still being solidified. A future version of this
 > package will support creating new build extensions.
@@ -107,17 +108,15 @@
 
 [project]
 name = "scikit_build_simplest"
 version = "0.0.1"
 ```
 
 You can (and should) specify the rest of the entries in `project`, but these are
-the minimum to get started. You can also `scikit-build-core[pyproject]` to
-pre-load some dependencies if you want; in some cases this might be marginally
-faster.
+the minimum to get started.
 
 An example `CMakeLists.txt`:
 
 ```cmake
 cmake_minimum_required(VERSION 3.15...3.27)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
@@ -187,16 +186,16 @@
 ninja.minimum-version = ""
 
 # The versions of Ninja to allow. If Ninja is not present on the system or does
 # not pass this specifier, it will be downloaded via PyPI if possible. An empty
 # string will disable this check.
 ninja.version = ">=1.5"
 
-# If CMake is not present on the system or is older required, it will be
-# downloaded via PyPI if possible. An empty string will disable this check.
+# If Ninja is not present on the system or is older than required, it will be
+# downloaded via PyPI if this is false.
 ninja.make-fallback = true
 
 # The logging level to display, "DEBUG", "INFO", "WARNING", and "ERROR" are
 # possible options.
 logging.level = "WARNING"
 
 # Files to include in the SDist even if they are skipped by default. Supports
@@ -247,16 +246,17 @@
 wheel.cmake = true
 
 # Target the platlib or the purelib. If not set, the default is to target the
 # platlib if wheel.cmake is true, and the purelib otherwise.
 wheel.platlib = ""
 
 # A set of patterns to exclude from the wheel. This is additive to the SDist
-# exclude patterns. This applies to the source files, not the final paths.
-# Editable installs may not respect this exclusion.
+# exclude patterns. This applies to the final paths in the wheel, and can
+# exclude files from CMake output as well.  Editable installs may not respect
+# this exclusion.
 wheel.exclude = []
 
 # The build tag to use for the wheel. If empty, no build tag is used.
 wheel.build-tag = ""
 
 # If CMake is less than this value, backport a copy of FindPython. Set to 0
 # disable this, or the empty string.
@@ -272,15 +272,15 @@
 # set.
 editable.rebuild = false
 
 # The components to install. If empty, all default components are installed.
 install.components = []
 
 # Whether to strip the binaries. True for scikit-build-core 0.5+.
-install.strip = false
+install.strip = true
 
 # The path (relative to platlib) for the file to generate.
 generate[].path = ""
 
 # The template to use for the file. This includes string.Template style
 # placeholders for all the metadata. If empty, a template-path must be set.
 generate[].template = ""
```

### Comparing `scikit_build_core-0.8.2/pyproject.toml` & `scikit_build_core-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -29,41 +29,45 @@
     "Development Status :: 4 - Beta",
     "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
-    "exceptiongroup; python_version<'3.11'",
-    "importlib-metadata; python_version<'3.8'",
+    "exceptiongroup >=1.0; python_version<'3.11'",
+    "importlib-metadata >=4.13; python_version<'3.8'",
     "importlib-resources >=1.3; python_version<'3.9'",
-    "packaging >=20.9",
-    "tomli >=1.1; python_version<'3.11'",
+    "packaging >=21.3",
+    "pathspec >=0.10.1",
+    "tomli >=1.2.2; python_version<'3.11'",
     "typing-extensions >=3.10.0; python_version<'3.9'",
 ]
 # Note: for building wheels and sdists, there are also additional dependencies
 # in the pyproject extra. And cmake and possibly ninja if those are not already
 # present (user controllable)
 
 [project.optional-dependencies]
 pyproject = [
-    "pathspec >=0.10.1",
-    "pyproject-metadata >=0.5",
 ]
 test = [
-    "build[virtualenv]",
+    "build >=0.8",
     "cattrs >=22.2.0",
-    "pathspec >=0.10.1",
-    "pybind11",
-    "pyproject-metadata >=0.5",
+    "pip >=22",
+    "pybind11 >=2.11",
     "pytest >=7.0",  # 7.2+ recommended for better tracebacks with ExceptionGroup
     "pytest-subprocess >=1.5",
-    "setuptools",
-    "virtualenv",
-    "wheel",
+    'setuptools >=43; python_version<"3.9"',
+    'setuptools >=45; python_version=="3.9"',
+    'setuptools >=49; python_version>="3.10" and python_version<"3.12"',
+    'setuptools >=66.1; python_version>="3.12"',
+    "virtualenv >=20.0.28",
+    "wheel >=0.40",
+]
+test-hatchling = [
+    "hatchling >=1.24.0",
 ]
 test-meta = [
     "hatch-fancy-pypi-readme>=22.3",
     "setuptools-scm",
 ]
 test-numpy = [
     "numpy; python_version<'3.12' and platform_python_implementation!='PyPy'",
@@ -83,22 +87,22 @@
     "ninja; sys_platform!='win32'",
 ]
 dev = [
     "rich",
 ]
 docs = [
     "furo",
+    "hatchling",
     "myst-parser >=0.13",
-    "pathspec >=0.10.1",
-    "pyproject-metadata >=0.5",
-    "sphinx >=7.0,<=7.1.2",  # workaround bug in setuptools, fix in pypa/setuptools#4023
+    "setuptools",
+    "sphinx >=7.0",
+    "sphinx-autodoc-typehints",
     "sphinx-copybutton",
     "sphinx-inline-tabs",
     "sphinx-jsonschema",
-    "sphinx-autodoc-typehints",
 ]
 
 [project.urls]
 Changelog = "https://scikit-build-core.readthedocs.io/en/latest/changelog.html"
 Discussions = "https://github.com/orgs/scikit-build/discussions"
 Documentation = "https://scikit-build-core.readthedocs.io"
 Homepage = "https://github.com/scikit-build/scikit-build-core"
@@ -106,14 +110,15 @@
 
 [project.entry-points]
 "distutils.commands".build_cmake = "scikit_build_core.setuptools.build_cmake:BuildCMake"
 "distutils.setup_keywords".cmake_source_dir = "scikit_build_core.setuptools.build_cmake:cmake_source_dir"
 "distutils.setup_keywords".cmake_args = "scikit_build_core.setuptools.build_cmake:cmake_args"
 "setuptools.finalize_distribution_options".scikit_build_entry = "scikit_build_core.setuptools.build_cmake:finalize_distribution_options"
 "validate_pyproject.tool_schema".scikit-build = "scikit_build_core.settings.skbuild_schema:get_skbuild_schema"
+hatch.scikit-build = "scikit_build_core.hatch.hooks"
 
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/scikit_build_core/_version.py"
 
 
 [tool.pytest.ini_options]
@@ -144,15 +149,15 @@
 ]
 norecursedirs = ["tests/packages/**"]
 
 
 [tool.mypy]
 files = ["src", "tests", "noxfile.py"]
 mypy_path = ["$MYPY_CONFIG_FILE_DIR/src"]
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 strict = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
 [[tool.mypy.overrides]]
@@ -187,27 +192,29 @@
     "unused-argument",  # Handled by Ruff
     "redefined-builtin",  # ExceptionGroup is a builtin
 ]
 
 
 [tool.coverage]
 run.source = ["scikit_build_core"]
+run.omit = ["src/scikit_build_core/_vendor"]
 report.exclude_lines = [
     'pragma: no cover',
     '\.\.\.',
     'if typing.TYPE_CHECKING:',
 ]
 
 
 [tool.check-wheel-contents]
 ignore = ["W002"]  # Triggers on __init__.py's
 
+
 [tool.ruff]
 src = ["src"]
-exclude = []  # Required due to "build" module
+exclude = ["src/scikit_build_core/_vendor"]  # Required due to "build" module
 
 [tool.ruff.lint]
 extend-select = [
     "ANN",         # flake8-annotations
     "ARG",         # flake8-unused-arguments
     "B",           # flake8-bugbear
     "C4",          # flake8-comprehensions
@@ -274,14 +281,15 @@
 "typing.assert_never".msg = "Add scikit_build_core._compat.typing.assert_never instead."
 "tomli".msg = "Use scikit_build_core._compat.tomllib instead."
 "tomllib".msg = "Use scikit_build_core._compat.tomllib instead."
 "importlib.metadata".msg = "Use scikit_build_core._compat.importlib.metadata instead."
 "importlib_metadata".msg = "Use scikit_build_core._compat.importlib.metadata instead."
 "importlib.resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
 "importlib_resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
+"pyproject_metadata".msg = "Use scikit_build_core._vendor.pyproject_metadata instead."
 
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**" = ["T20", "ANN", "FBT001"]
 "noxfile.py" = ["T20", "TID251"]
 "src/scikit_build_core/resources/*.py" = ["PTH", "ARG002", "FBT", "TID251"]
 "src/scikit_build_core/_compat/**.py" = ["TID251"]
```

### Comparing `scikit_build_core-0.8.2/PKG-INFO` & `scikit_build_core-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scikit_build_core
-Version: 0.8.2
+Version: 0.9.0
 Summary: Build backend for CMake based projects
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -23,48 +23,51 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: exceptiongroup; python_version < '3.11'
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Dist: exceptiongroup>=1.0; python_version < '3.11'
+Requires-Dist: importlib-metadata>=4.13; python_version < '3.8'
 Requires-Dist: importlib-resources>=1.3; python_version < '3.9'
-Requires-Dist: packaging>=20.9
-Requires-Dist: tomli>=1.1; python_version < '3.11'
+Requires-Dist: packaging>=21.3
+Requires-Dist: pathspec>=0.10.1
+Requires-Dist: tomli>=1.2.2; python_version < '3.11'
 Requires-Dist: typing-extensions>=3.10.0; python_version < '3.9'
 Provides-Extra: cov
 Requires-Dist: pytest-cov[toml]; extra == 'cov'
 Provides-Extra: dev
 Requires-Dist: rich; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
+Requires-Dist: hatchling; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
-Requires-Dist: pathspec>=0.10.1; extra == 'docs'
-Requires-Dist: pyproject-metadata>=0.5; extra == 'docs'
+Requires-Dist: setuptools; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs; extra == 'docs'
 Requires-Dist: sphinx-jsonschema; extra == 'docs'
-Requires-Dist: sphinx<=7.1.2,>=7.0; extra == 'docs'
+Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: pyproject
-Requires-Dist: pathspec>=0.10.1; extra == 'pyproject'
-Requires-Dist: pyproject-metadata>=0.5; extra == 'pyproject'
 Provides-Extra: test
-Requires-Dist: build[virtualenv]; extra == 'test'
+Requires-Dist: build>=0.8; extra == 'test'
 Requires-Dist: cattrs>=22.2.0; extra == 'test'
-Requires-Dist: pathspec>=0.10.1; extra == 'test'
-Requires-Dist: pybind11; extra == 'test'
-Requires-Dist: pyproject-metadata>=0.5; extra == 'test'
+Requires-Dist: pip>=22; extra == 'test'
+Requires-Dist: pybind11>=2.11; extra == 'test'
 Requires-Dist: pytest-subprocess>=1.5; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
-Requires-Dist: setuptools; extra == 'test'
-Requires-Dist: virtualenv; extra == 'test'
-Requires-Dist: wheel; extra == 'test'
+Requires-Dist: setuptools>=43; (python_version < '3.9') and extra == 'test'
+Requires-Dist: setuptools>=45; (python_version == '3.9') and extra == 'test'
+Requires-Dist: setuptools>=49; (python_version >= '3.10' and python_version < '3.12') and extra == 'test'
+Requires-Dist: setuptools>=66.1; (python_version >= '3.12') and extra == 'test'
+Requires-Dist: virtualenv>=20.0.28; extra == 'test'
+Requires-Dist: wheel>=0.40; extra == 'test'
+Provides-Extra: test-hatchling
+Requires-Dist: hatchling>=1.24.0; extra == 'test-hatchling'
 Provides-Extra: test-meta
 Requires-Dist: hatch-fancy-pypi-readme>=22.3; extra == 'test-meta'
 Requires-Dist: setuptools-scm; extra == 'test-meta'
 Provides-Extra: test-numpy
 Requires-Dist: numpy; (python_version < '3.12' and platform_python_implementation != 'PyPy') and extra == 'test-numpy'
 Requires-Dist: numpy~=1.21.0; (python_version == '3.7' and platform_python_implementation == 'PyPy' and sys_platform == 'linux') and extra == 'test-numpy'
 Requires-Dist: numpy~=1.24.0; (python_version == '3.8' and platform_python_implementation == 'PyPy') and extra == 'test-numpy'
@@ -154,20 +157,21 @@
 - Wheels are not fully reproducible yet (nor are they in most others systems,
   including setuptools)
 - Several editable mode caveats (mentioned in the docs).
 
 Other backends are also planned:
 
 - Setuptools integration highly experimental
+- Hatchling plugin highly experimental
 - The extensionlib integration is missing
-- No hatchling plugin yet.
 
 The recommended interface is the native pyproject builder. There is also a WIP
 setuptools-based interface that is being developed to provide a transition path
-for classic scikit-build.
+for classic scikit-build, and a WIP Hatchling plugin. Both might be moved to
+standalone packages in the future.
 
 > [!WARNING]
 >
 > Only the pyproject-based builder should be used; the setuptools backend is
 > experimental and likely to move to a separate package before being declared
 > stable, and internal API is still being solidified. A future version of this
 > package will support creating new build extensions.
@@ -186,17 +190,15 @@
 
 [project]
 name = "scikit_build_simplest"
 version = "0.0.1"
 ```
 
 You can (and should) specify the rest of the entries in `project`, but these are
-the minimum to get started. You can also `scikit-build-core[pyproject]` to
-pre-load some dependencies if you want; in some cases this might be marginally
-faster.
+the minimum to get started.
 
 An example `CMakeLists.txt`:
 
 ```cmake
 cmake_minimum_required(VERSION 3.15...3.27)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
@@ -266,16 +268,16 @@
 ninja.minimum-version = ""
 
 # The versions of Ninja to allow. If Ninja is not present on the system or does
 # not pass this specifier, it will be downloaded via PyPI if possible. An empty
 # string will disable this check.
 ninja.version = ">=1.5"
 
-# If CMake is not present on the system or is older required, it will be
-# downloaded via PyPI if possible. An empty string will disable this check.
+# If Ninja is not present on the system or is older than required, it will be
+# downloaded via PyPI if this is false.
 ninja.make-fallback = true
 
 # The logging level to display, "DEBUG", "INFO", "WARNING", and "ERROR" are
 # possible options.
 logging.level = "WARNING"
 
 # Files to include in the SDist even if they are skipped by default. Supports
@@ -326,16 +328,17 @@
 wheel.cmake = true
 
 # Target the platlib or the purelib. If not set, the default is to target the
 # platlib if wheel.cmake is true, and the purelib otherwise.
 wheel.platlib = ""
 
 # A set of patterns to exclude from the wheel. This is additive to the SDist
-# exclude patterns. This applies to the source files, not the final paths.
-# Editable installs may not respect this exclusion.
+# exclude patterns. This applies to the final paths in the wheel, and can
+# exclude files from CMake output as well.  Editable installs may not respect
+# this exclusion.
 wheel.exclude = []
 
 # The build tag to use for the wheel. If empty, no build tag is used.
 wheel.build-tag = ""
 
 # If CMake is less than this value, backport a copy of FindPython. Set to 0
 # disable this, or the empty string.
@@ -351,15 +354,15 @@
 # set.
 editable.rebuild = false
 
 # The components to install. If empty, all default components are installed.
 install.components = []
 
 # Whether to strip the binaries. True for scikit-build-core 0.5+.
-install.strip = false
+install.strip = true
 
 # The path (relative to platlib) for the file to generate.
 generate[].path = ""
 
 # The template to use for the file. This includes string.Template style
 # placeholders for all the metadata. If empty, a template-path must be set.
 generate[].template = ""
```

