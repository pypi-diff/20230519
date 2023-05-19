# Comparing `tmp/scikit_build_core-0.3.3.tar.gz` & `tmp/scikit_build_core-0.4.0.tar.gz`

## Comparing `scikit_build_core-0.3.3.tar` & `scikit_build_core-0.4.0.tar`

### file list

```diff
@@ -1,216 +1,237 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.gitattributes
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.packit.yaml
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.readthedocs.yml
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/noxfile.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.distro/scikit-build-core.spec
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0    13231 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/changelog.md
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/conf.py
--rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/extension.py
--rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/conftest.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_fileapi.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_get_requires.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_simplest_c.py
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/LICENSE
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/README.md
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.packit.yaml
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/noxfile.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/.fmf/version
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/changelog.md
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9653 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_get_requires.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/README.md
+-rw-r--r--   0        0        0     8263 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12466 2020-02-02 00:00:00.000000 scikit_build_core-0.4.0/PKG-INFO
```

### Comparing `scikit_build_core-0.3.3/.packit.yaml` & `scikit_build_core-0.4.0/.packit.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 # See the documentation for more information:
 # https://packit.dev/docs/configuration/
 
-specfile_path: .distro/scikit-build-core.spec
+specfile_path: .distro/python-scikit-build-core.spec
 
 files_to_sync:
-  - src: .distro/scikit-build-core.spec
+  - src: .distro/python-scikit-build-core.spec
     dest: python-scikit-build-core.spec
   - .packit.yaml
   - src: .distro/python-scikit-build-core.rpmlintrc
     dest: python-scikit-build-core.rpmlintrc
+  # tmt setup
+  - src: .distro/.fmf/
+    dest: .fmf/
+  - src: .distro/plans/
+    dest: plans/
+    filters:
+      - "- .distro/plans/main.fmf.dist-git"
+      - "- .distro/plans/rpmlint.fmf"
+  - src: .distro/plans/main.fmf.dist-git
+    dest: plans/main.fmf
 upstream_package_name: scikit_build_core
 downstream_package_name: python-scikit-build-core
 update_release: false
 upstream_tag_template: v{version}
 
 jobs:
   - job: copr_build
     trigger: pull_request
     owner: "@scikit-build"
     project: scikit-build-core
     update_release: true
     release_suffix: "{PACKIT_RPMSPEC_RELEASE}"
     targets:
       - fedora-development
+  - job: tests
+    trigger: pull_request
+    targets:
+      - fedora-development
+    fmf_path: .distro
   - job: copr_build
     trigger: commit
     branch: main
     owner: "@scikit-build"
     project: nightly
     targets:
       - fedora-development-x86_64
       - fedora-latest-x86_64
       - fedora-development-aarch64
       - fedora-latest-aarch64
+  - job: tests
+    trigger: commit
+    branch: main
+    targets:
+      - fedora-development
+      - fedora-latest
+    fmf_path: .distro
   - job: copr_build
     trigger: release
     owner: "@scikit-build"
     project: release
     targets:
       - fedora-development-x86_64
       - fedora-latest-x86_64
```

### Comparing `scikit_build_core-0.3.3/.pre-commit-config.yaml` & `scikit_build_core-0.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -50,21 +50,21 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.267
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         exclude: |
           (?x)^(
             tests/packages/simplest_c/src/simplest/__init__.py|
             tests/packages/dynamic_metadata/src/dynamic/__init__.py|
             tests/packages/.*/setup.py
```

### Comparing `scikit_build_core-0.3.3/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.0/.github/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -274,24 +274,14 @@
 
 target_compile_definitions(cmake_example
                            PRIVATE VERSION_INFO=${PROJECT_VERSION})
 
 install(TARGETS cmake_example DESTINATION .)
 ```
 
-This is built on top of CMakeExtension, which looks like this:
-
-```
-from scikit_build_core.setuptoools.extension import CMakeExtension
-...
-cmake_extensions=[CMakeExtension("cmake_example")],
-```
-
-Which should eventually support multiple extensions.
-
 ## Patterns
 
 ### Backports
 
 All backported standard library code is in `scikit_build_core._compat`, in a
 module with the stdlib name.
```

### Comparing `scikit_build_core-0.3.3/.github/matchers/pylint.json` & `scikit_build_core-0.4.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/.github/workflows/ci.yml` & `scikit_build_core-0.4.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,17 @@
         run: >-
           pytest -ra --showlocals --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v3
         with:
-          name: ${{ runner.os }}-${{ matrix.python-version }}
+          name:
+            ${{ runner.os }}-${{ matrix.python-version }}-${{
+            matrix.cmake-version }}
           verbose: true
           token: 6d9cc0e0-158a-41ee-b8f4-0318d3595ac2
 
       # the min requirements are not compatible with the metadata plugin
       # packages so we remove those first (they then won't be tested)
       - name: Min requirements
         run: |
@@ -116,15 +118,15 @@
         uses: jwlawson/actions-setup-cmake@v1.14
         with:
           cmake-version: "${{ matrix.cmake-version }}"
 
       # Skipped on pypy to keep the tests fast
       - name: Test min package
         if: matrix.python-version != 'pypy-3.8'
-        run: pytest -ra --showlocals
+        run: pytest -ra --showlocals -Wdefault
 
   cygwin:
     name: Tests on 🐍 3.9 • cygwin
     runs-on: windows-latest
     timeout-minutes: 30
 
     steps:
```

### Comparing `scikit_build_core-0.3.3/docs/changelog.md` & `scikit_build_core-0.4.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # Changelog
 
+## Version 0.4.0
+
+An important fix/feature: LICENSE files were not being included in the wheel's
+metadata folder. You can configure the license file selection via a new
+configuration option, and a reasonable default was added. You can now select a
+source directory for your CMakeLists.txt. A lot of work was done on the still
+experimental setuptools backend; it still should be seen as completely
+experimental while it is being finished.
+
+Features:
+
+- `cmake.source-dir` for CMakeLists in subdirectories by @henryiii in #323
+- Add `LICENSE` file option by @henryiii in #321
+
+Fixes:
+
+- Ninja wasn't being used if present by @henryiii in #310
+- Wheels were not including the `LICENSE` file by @henryiii in #321
+
+Setuptools plugin:
+
+- Refactor plugin as custom setuptools command by @henryiii in #312
+- Adding `cmake_args` by @henryiii in #314
+- Add wrapper for `skbuild.setup` compat by @henryiii in #315
+
+Other:
+
+- ci: add rpmlint and smoke tests by @LecrisUT in #313
+
 ## Version 0.3.3
 
 This version improves WebAssembly support (Pyodide) and fixes a reported bug in
 the new editable mode.
 
 Fixes:
```

### Comparing `scikit_build_core-0.3.3/docs/cmakelists.md` & `scikit_build_core-0.4.0/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/conf.py` & `scikit_build_core-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/configuration.md` & `scikit_build_core-0.4.0/docs/configuration.md`

 * *Files 5% similar despite different names*

```diff
@@ -173,14 +173,24 @@
 
 You can select a different wheel target directory, as well, but that syntax is
 experimental; install to `${SKBUILD_DATA_DIR}`, etc. from within CMake instead
 for now.
 
 :::
 
+By default, any `LICENSE*`, `COPYING*`, or `COPYRIGHT*` file in the root of the
+build directory will be picked up. You can specify an exact list of files if you
+prefer, or if you your license file is in a different directory. The files must
+have unique names. Globbing patterns are supported.
+
+```toml
+[tool.scikit-build]
+wheel.license-files = ["LICENSE"]
+```
+
 ## Customizing the output wheel
 
 The python API tags for your wheel will be correct assuming you are building a
 CPython extension. If you are building a Limited ABI extension, you should set
 the wheel tags for the version you support:
 
 ```toml
@@ -366,23 +376,23 @@
 ```yaml
 SKBUILD_CMAKE_ARGS: -DSOME_DEFINE=ON;-DOTHER=OFF
 CMAKE_ARGS: -DSOME_DEFINE=ON;-DOTHER=OFF
 ```
 
 ````
 
-## Dynamic metadata (WIP)
+## Dynamic metadata
+
+Scikit-build-core 0.3.0 supports dynamic metadata with two built-in plugins.
 
-Scikit-build-core 0.3.0 will support dynamic metadata. This is not ready for
-plugin development outside of scikit-build-core;
-`tool.scikit-build.experimental=true` is required to use external plugins, since
-the interface is provisional. Nested arbitrary dicts (as seen here) are not
-supported in config-settings or environment variables.
+:::{warning}
 
-There currently are two built-in plugins for dynamic metadata.
+This is not ready for plugin development outside of scikit-build-core;
+`tool.scikit-build.experimental=true` is required to use plugins that are not
+shipped with scikit-build-core, since the interface is provisional. :::
 
 :::{tab} Setuptools-scm
 
 You can use [setuptools-scm](https://github.com/pypa/setuptools_scm) to pull the
 version from VCS:
 
 ```toml
```

### Comparing `scikit_build_core-0.3.3/docs/getting_started.md` & `scikit_build_core-0.4.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/index.md` & `scikit_build_core-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.0/docs/api/scikit_build_core.setuptools.rst`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,30 @@
    :members:
    :undoc-members:
    :show-inheritance:
 
 Submodules
 ----------
 
+scikit\_build\_core.setuptools.build\_cmake module
+--------------------------------------------------
+
+.. automodule:: scikit_build_core.setuptools.build_cmake
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 scikit\_build\_core.setuptools.build\_meta module
 -------------------------------------------------
 
 .. automodule:: scikit_build_core.setuptools.build_meta
    :members:
    :undoc-members:
    :show-inheritance:
 
-scikit\_build\_core.setuptools.extension module
------------------------------------------------
+scikit\_build\_core.setuptools.wrapper module
+---------------------------------------------
 
-.. automodule:: scikit_build_core.setuptools.extension
+.. automodule:: scikit_build_core.setuptools.wrapper
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit_build_core-0.3.3/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.0/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.0/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.0/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.0/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.15...3.26)
+cmake_minimum_required(VERSION 3.17.2...3.26)
 project(${SKBUILD_PROJECT_NAME} LANGUAGES C Fortran)
 
 find_package(
   Python
   COMPONENTS Interpreter Development.Module NumPy
   REQUIRED)
```

### Comparing `scikit_build_core-0.3.3/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.0/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.0/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.0/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.0/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.0/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.0/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.0/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.0/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.0/src/scikit_build_core/build/wheel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import dataclasses
+import glob
 import os
 import shutil
 import sys
 import sysconfig
 import tempfile
 from collections.abc import Sequence
 from pathlib import Path
@@ -143,15 +144,15 @@
                 raise AssertionError(msg)
             install_dir = wheel_dir / settings.wheel.install_dir[1:]
         else:
             install_dir = wheel_dirs["platlib"] / settings.wheel.install_dir
 
         config = CMaker(
             cmake,
-            source_dir=Path("."),
+            source_dir=Path(settings.cmake.source_dir or "."),
             build_dir=build_dir,
             build_type=settings.cmake.build_type,
         )
 
         builder = Builder(
             settings=settings,
             config=config,
@@ -178,15 +179,17 @@
             cache_entries=cache_entries,
             name=metadata.name,
             version=metadata.version,
         )
 
         generator = builder.config.env.get(
             "CMAKE_GENERATOR",
-            "MSVC" if sysconfig.get_platform().startswith("win") else "Unknown",
+            "MSVC"
+            if sysconfig.get_platform().startswith("win")
+            else "Default generator",
         )
         rich_print(
             f"[green]***[/green] [bold]Building project with [blue]{generator}[/blue]..."
         )
         build_args: list[str] = []
         builder.build(build_args=build_args)
 
@@ -208,16 +211,28 @@
         if not editable:
             for filepath, package_dir in mapping.items():
                 Path(package_dir).parent.mkdir(exist_ok=True, parents=True)
                 shutil.copyfile(filepath, package_dir)
 
             process_script_dir(wheel_dirs["scripts"])
 
+        license_files = [
+            Path(x)
+            for y in settings.wheel.license_files
+            for x in glob.glob(y, recursive=True)
+        ]
+        if settings.wheel.license_files and not license_files:
+            logger.warning(
+                "No license files found, set wheel.license-files to [] to suppress this warning"
+            )
+
         with WheelWriter(metadata, Path(wheel_directory), tags.as_tags_set()) as wheel:
             wheel.build(wheel_dirs)
+            for license_file in license_files:
+                wheel.write(str(license_file), license_file.name)
 
             if editable:
                 modules = {
                     path_to_module(Path(v).relative_to(wheel_dirs["platlib"])): str(
                         Path(k).resolve()
                     )
                     for k, v in mapping.items()
```

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
 import re
 import sys
 import sysconfig
-from collections.abc import Mapping, Sequence
+from collections.abc import Iterable, Mapping, Sequence
 from pathlib import Path
 
 from packaging.version import Version
 
 from .. import __version__
 from .._compat.importlib import metadata, resources
 from .._logging import logger
@@ -79,14 +79,15 @@
         self,
         *,
         defines: Mapping[str, str],
         cache_entries: Mapping[str, str | Path] | None = None,
         name: str | None = None,
         version: Version | None = None,
         limited_abi: bool | None = None,
+        configure_args: Iterable[str] = (),
     ) -> None:
         cmake_defines = dict(defines)
 
         # Add any extra CMake modules
         eps = metadata.entry_points(group="cmake.module")
         self.config.module_dirs.extend(resources.files(ep.load()) for ep in eps)
 
@@ -177,15 +178,15 @@
                 cmake_defines["CMAKE_OSX_ARCHITECTURES"] = ";".join(archs)
 
         # Add the pre-defined or passed CMake defines
         cmake_defines.update(self.settings.cmake.define)
 
         self.config.configure(
             defines=cmake_defines,
-            cmake_args=self.get_cmake_args(),
+            cmake_args=[*self.get_cmake_args(), *configure_args],
         )
 
     def build(self, build_args: list[str]) -> None:
         self.config.build(build_args=build_args, verbose=self.settings.cmake.verbose)
 
     def install(self, install_dir: Path) -> None:
         self.config.install(install_dir)
```

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,19 @@
         env.setdefault("CMAKE_GENERATOR_PLATFORM", get_cmake_platform(env))
         return {}
 
     if sys.platform.startswith("win") and not sysconfig.get_platform().startswith(
         "win"
     ):
         # Non-MSVC Windows platforms require Ninja
-        env.setdefault("CMAKE_GENERATOR", "Ninja")
+        default = "Ninja"
+
+    # Try Ninja if it is available, even if make is CMake default
+    if default == "Unix Makefiles":
+        default = "Ninja"
 
     if env.get("CMAKE_GENERATOR", default or "Ninja") == "Ninja":
         min_ninja = Version(ninja_settings.minimum_version)
         ninja = best_program(get_ninja_programs(), minimum_version=min_ninja)
 
         if ninja is not None:
             env.setdefault("CMAKE_GENERATOR", "Ninja")
```

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.0/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.0/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.0/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.0/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.0/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.0/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.0/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     verbose: bool = False
 
     #: The build type to use when building the project.
     #: Valid options are: "Debug", "Release", "RelWithDebInfo", "MinSizeRel",
     #: "", etc.
     build_type: str = "Release"
 
+    #: The source directory to use when building the project. Currently only affects
+    #: the native builder (not the setuptools plugin).
+    source_dir: str = ""
+
 
 @dataclasses.dataclass
 class LoggingSettings:
     #: The logging level to display.
     level: str = "WARNING"
 
 
@@ -90,14 +94,19 @@
     expand_macos_universal_tags: bool = False
 
     #: The install directory for the wheel. This is relative to the platlib root.
     #: EXPERIMENTAL: An absolute path will be one level higher than the platlib
     #: root, giving access to "/platlib", "/data", "/headers", and "/scripts".
     install_dir: str = ""
 
+    #: A list of license files to include in the wheel. Supports glob patterns.
+    license_files: List[str] = dataclasses.field(
+        default_factory=lambda: ["LICENSE*", "COPYING*", "COPYRIGHT*"]
+    )
+
 
 @dataclasses.dataclass
 class BackportSettings:
     #: If CMake is less than this value, backport a copy of FindPython. Set
     #: to 0 disable this, or the empty string.
     find_python: str = "3.26.1"
```

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.0/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.0/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.0/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/conftest.py` & `scikit_build_core-0.4.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -219,18 +219,29 @@
 
 @pytest.fixture()
 def package_simple_pyproject_ext(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch
 ) -> PackageInfo:
     package = PackageInfo(
         "simple_pyproject_ext",
-        "f1b86c7fbcc70ed82786fd3446caf880091096b7d6c0085eab8fe64466b95c4f",
-        "463bdfcfad8b71a0f2b48b7b5abea191c9073170326183c04b7f23da19d6b61b",
-        "aa1f2cd959998cb58316f72526ad7b2d3078bf47d00c5c9f8903d9b5980c0e35",
-        "9e4713843829659b4862e73c8a9ae783178d620a78fed1f757efb82ea77ff82f",
+        "920c8475bf53c67231dbe3a08c1b533306e89f79dfbd09c1fe2ec55ec6c8fe0c",
+        "617737581c2e6f42137539c46c0bf904ea43a7b653925dbbcf8dce88e4a835a8",
+        "b41badc7999eddd2f4a59aa244baa04b9498d699888c2ced33655396108616a4",
+        "2fb6482b83f624d1fe83e30579f9507167e1db9e5256bc0f47a907abb9ae98ec",
+    )
+    process_package(package, tmp_path, monkeypatch)
+    return package
+
+
+@pytest.fixture()
+def package_simple_pyproject_source_dir(
+    tmp_path: Path, monkeypatch: pytest.MonkeyPatch
+) -> PackageInfo:
+    package = PackageInfo(
+        "simple_pyproject_source_dir",
     )
     process_package(package, tmp_path, monkeypatch)
     return package
 
 
 @pytest.fixture()
 def package_simple_setuptools_ext(
@@ -238,14 +249,23 @@
 ) -> PackageInfo:
     package = PackageInfo("simple_setuptools_ext")
     process_package(package, tmp_path, monkeypatch)
     return package
 
 
 @pytest.fixture()
+def package_mixed_setuptools(
+    tmp_path: Path, monkeypatch: pytest.MonkeyPatch
+) -> PackageInfo:
+    package = PackageInfo("mixed_setuptools")
+    process_package(package, tmp_path, monkeypatch)
+    return package
+
+
+@pytest.fixture()
 def package_filepath_pure(
     tmp_path: Path, monkeypatch: pytest.MonkeyPatch
 ) -> PackageInfo:
     package = PackageInfo("filepath_pure")
     process_package(package, tmp_path, monkeypatch)
     return package
```

### Comparing `scikit_build_core-0.3.3/tests/test_builder.py` & `scikit_build_core-0.4.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_cmake_config.py` & `scikit_build_core-0.4.0/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.0/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_fileapi.py` & `scikit_build_core-0.4.0/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_fortran.py` & `scikit_build_core-0.4.0/tests/test_fortran.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import shutil
 import sys
 import sysconfig
 import zipfile
 from pathlib import Path
 
 import pytest
+from packaging.version import Version
 
 from scikit_build_core.build import build_wheel
+from scikit_build_core.program_search import (
+    best_program,
+    get_cmake_programs,
+    get_ninja_programs,
+)
 
 np = pytest.importorskip("numpy")
 
 DIR = Path(__file__).parent.resolve()
 FORTRAN_EXAMPLE = DIR / "packages/fortran_example"
 
 
+cmake_info = best_program(get_cmake_programs(), minimum_version=Version("3.17.2"))
+ninja_info = best_program(get_ninja_programs(), minimum_version=Version("1.10"))
+
+
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.fortran()
 @pytest.mark.skipif(shutil.which("gfortran") is None, reason="gfortran not available")
 @pytest.mark.skipif(
     sysconfig.get_platform().startswith("win"),
     reason="No reasonable Fortran compiler for MSVC",
 )
+@pytest.mark.skipif(
+    cmake_info is None, reason="CMake needs to be 3.17.2+ to support Fortran with Ninja"
+)
+@pytest.mark.skipif(
+    ninja_info is None, reason="Ninja needs to be 1.10+ to support Fortran with CMake"
+)
 def test_pep517_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(FORTRAN_EXAMPLE)
     if Path("dist").is_dir():
         shutil.rmtree("dist")
     out = build_wheel(str(dist))
```

### Comparing `scikit_build_core-0.3.3/tests/test_generator_default.py` & `scikit_build_core-0.4.0/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_get_requires.py` & `scikit_build_core-0.4.0/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_module_dir.py` & `scikit_build_core-0.4.0/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_name_main.py` & `scikit_build_core-0.4.0/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.0/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_process_scripts.py` & `scikit_build_core-0.4.0/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_program_search.py` & `scikit_build_core-0.4.0/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.0/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.0/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.0/tests/test_pyproject_pep517.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         assert file_names == {
             f"cmake-example-0.0.1/{x}"
             for x in (
                 "CMakeLists.txt",
                 "pyproject.toml",
                 "src/main.cpp",
                 "PKG-INFO",
+                "LICENSE",
             )
         }
         pkg_info = f.extractfile("cmake-example-0.0.1/PKG-INFO")
         assert pkg_info
         pkg_info_contents = pkg_info.read().decode()
         assert pkg_info_contents == METADATA
 
@@ -156,17 +157,66 @@
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
             metadata = p.joinpath("cmake_example-0.0.1.dist-info/METADATA").read_text()
             entry_points = p.joinpath(
                 "cmake_example-0.0.1.dist-info/entry_points.txt"
             ).read_text()
 
-        assert len(file_names) == 2
+        assert len(file_names) == 3
         assert "cmake_example-0.0.1.dist-info" in file_names
         file_names.remove("cmake_example-0.0.1.dist-info")
+        file_names.remove("LICENSE")
+        (so_file,) = file_names
+
+        assert so_file.startswith("cmake_example")
+        print("SOFILE:", so_file)
+
+        print(entry_points == ENTRYPOINTS)
+        assert 'Requires-Dist: pytest>=6.0; extra == "test"' in metadata
+        assert "Metadata-Version: 2.1" in metadata
+        assert "Name: cmake-example" in metadata
+        assert "Version: 0.0.1" in metadata
+        assert "Requires-Python: >=3.7" in metadata
+        assert "Provides-Extra: test" in metadata
+
+    virtualenv.install(wheel)
+
+    version = virtualenv.execute(
+        "import cmake_example; print(cmake_example.__version__)",
+    )
+    assert version.strip() == "0.0.1"
+
+    add = virtualenv.execute(
+        "import cmake_example; print(cmake_example.add(1, 2))",
+    )
+    assert add.strip() == "3"
+
+
+@pytest.mark.compile()
+@pytest.mark.configure()
+@pytest.mark.usefixtures("package_simple_pyproject_source_dir")
+def test_pep517_wheel_source_dir(virtualenv):
+    dist = Path("dist")
+    out = build_wheel("dist")
+    (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
+    assert wheel == dist / out
+
+    if sys.version_info >= (3, 8):
+        with wheel.open("rb") as f:
+            p = zipfile.Path(f)
+            file_names = [p.name for p in p.iterdir()]
+            metadata = p.joinpath("cmake_example-0.0.1.dist-info/METADATA").read_text()
+            entry_points = p.joinpath(
+                "cmake_example-0.0.1.dist-info/entry_points.txt"
+            ).read_text()
+
+        assert len(file_names) == 3
+        assert "cmake_example-0.0.1.dist-info" in file_names
+        file_names.remove("cmake_example-0.0.1.dist-info")
+        file_names.remove("LICENSE")
         (so_file,) = file_names
 
         assert so_file.startswith("cmake_example")
         print("SOFILE:", so_file)
 
         print(entry_points == ENTRYPOINTS)
         assert 'Requires-Dist: pytest>=6.0; extra == "test"' in metadata
```

### Comparing `scikit_build_core-0.3.3/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.0/tests/test_pyproject_pep518.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         assert file_names == {
             f"cmake-example-0.0.1/{x}"
             for x in (
                 "CMakeLists.txt",
                 "pyproject.toml",
                 "src/main.cpp",
                 "PKG-INFO",
+                "LICENSE",
             )
         }
         pkg_info = f.extractfile("cmake-example-0.0.1/PKG-INFO")
         assert pkg_info
         pkg_info_contents = pkg_info.read().decode()
         assert correct_metadata == pkg_info_contents
 
@@ -66,17 +67,18 @@
     (wheel,) = Path("dist").glob("cmake_example-0.0.1-*.whl")
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
 
-        assert len(file_names) == 2
+        assert len(file_names) == 3
         assert "cmake_example-0.0.1.dist-info" in file_names
         file_names.remove("cmake_example-0.0.1.dist-info")
+        file_names.remove("LICENSE")
         (so_file,) = file_names
 
         assert so_file.startswith("cmake_example")
         print("SOFILE:", so_file)
 
     isolated.install(wheel)
 
@@ -114,17 +116,18 @@
     (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
 
-        assert len(file_names) == 2
+        assert len(file_names) == 3
         assert "cmake_example-0.0.1.dist-info" in file_names
         file_names.remove("cmake_example-0.0.1.dist-info")
+        file_names.remove("LICENSE")
         (so_file,) = file_names
 
         assert so_file.startswith("cmake_example")
         print("SOFILE:", so_file)
 
     isolated.install(wheel)
```

### Comparing `scikit_build_core-0.3.3/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.0/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_settings.py` & `scikit_build_core-0.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.0/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.0/tests/test_setuptools_pep517.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,24 +36,26 @@
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
         assert file_names == {
             f"cmake-example-0.0.1/{x}"
             for x in (
                 # TODO: "CMakeLists.txt",
                 "PKG-INFO",
-                "cmake_example.egg-info",
-                "cmake_example.egg-info/PKG-INFO",
-                "cmake_example.egg-info/SOURCES.txt",
-                "cmake_example.egg-info/dependency_links.txt",
-                "cmake_example.egg-info/not-zip-safe",
-                "cmake_example.egg-info/requires.txt",
-                "cmake_example.egg-info/top_level.txt",
+                "src",
+                "src/cmake_example.egg-info",
+                "src/cmake_example.egg-info/PKG-INFO",
+                "src/cmake_example.egg-info/SOURCES.txt",
+                "src/cmake_example.egg-info/dependency_links.txt",
+                "src/cmake_example.egg-info/not-zip-safe",
+                "src/cmake_example.egg-info/requires.txt",
+                "src/cmake_example.egg-info/top_level.txt",
                 "pyproject.toml",
                 "setup.cfg",
                 "setup.py",
+                "LICENSE",
                 # TODO: "src/main.cpp",
             )
         } | {"cmake-example-0.0.1"}
         pkg_info = f.extractfile("cmake-example-0.0.1/PKG-INFO")
         assert pkg_info
         pkg_info_contents = set(pkg_info.read().decode().strip().splitlines())
         assert metadata_set <= pkg_info_contents
@@ -92,7 +94,37 @@
     version = virtualenv.execute(
         "import cmake_example; print(cmake_example.__version__)"
     )
     assert version.strip() == "0.0.1"
 
     add = virtualenv.execute("import cmake_example; print(cmake_example.add(1, 2))")
     assert add.strip() == "3"
+
+
+@pytest.mark.compile()
+@pytest.mark.configure()
+@pytest.mark.usefixtures("package_mixed_setuptools")
+def test_pep517_mixed_wheel(virtualenv):
+    dist = Path("dist")
+    out = build_wheel("dist")
+    (wheel,) = dist.glob("mixed_setuptools-3.1.4-*.whl")
+    assert wheel == dist / out
+
+    if sys.version_info >= (3, 8):
+        with wheel.open("rb") as f:
+            p = zipfile.Path(f)
+            file_names = [p.name for p in p.iterdir()]
+
+        assert len(file_names) == 2
+        assert "mixed_setuptools-3.1.4.dist-info" in file_names
+        file_names.remove("mixed_setuptools-3.1.4.dist-info")
+        (so_file,) = file_names
+
+        assert so_file.startswith("mixed_setuptools")
+        print("SOFILE:", so_file)
+
+    virtualenv.install(wheel)
+
+    add = virtualenv.execute(
+        "import mixed_setuptools; print(mixed_setuptools.add(1, 2))"
+    )
+    assert add.strip() == "3"
```

### Comparing `scikit_build_core-0.3.3/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.0/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_simple_pure.py` & `scikit_build_core-0.4.0/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_simplest_c.py` & `scikit_build_core-0.4.0/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.0/tests/test_skbuild_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,23 @@
     assert settings.ninja.minimum_version == "1.5"
     assert settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.15"
     assert settings.cmake.args == []
     assert settings.cmake.define == {}
     assert not settings.cmake.verbose
     assert settings.cmake.build_type == "Release"
+    assert not settings.cmake.source_dir
     assert settings.logging.level == "WARNING"
     assert settings.sdist.include == []
     assert settings.sdist.exclude == []
     assert settings.sdist.reproducible
     assert settings.wheel.packages is None
     assert settings.wheel.py_api == ""
     assert not settings.wheel.expand_macos_universal_tags
+    assert settings.wheel.license_files == ["LICENSE*", "COPYING*", "COPYRIGHT*"]
     assert settings.backport.find_python == "3.26.1"
     assert settings.strict_config
     assert not settings.experimental
     assert settings.minimum_version is None
     assert settings.build_dir == ""
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
@@ -54,21 +56,23 @@
 
     monkeypatch.setenv("SKBUILD_NINJA_MINIMUM_VERSION", "1.1")
     monkeypatch.setenv("SKBUILD_NINJA_MAKE_FALLBACK", "0")
     monkeypatch.setenv("SKBUILD_CMAKE_MINIMUM_VERSION", "3.16")
     monkeypatch.setenv("SKBUILD_CMAKE_ARGS", "-DFOO=BAR;-DBAR=FOO")
     monkeypatch.setenv("SKBUILD_CMAKE_DEFINE", "a=1;b=2")
     monkeypatch.setenv("SKBUILD_CMAKE_BUILD_TYPE", "Debug")
+    monkeypatch.setenv("SKBUILD_CMAKE_SOURCE_DIR", "a/b/c")
     monkeypatch.setenv("SKBUILD_LOGGING_LEVEL", "DEBUG")
     monkeypatch.setenv("SKBUILD_SDIST_INCLUDE", "a;b; c")
     monkeypatch.setenv("SKBUILD_SDIST_EXCLUDE", "d;e;f")
     monkeypatch.setenv("SKBUILD_SDIST_REPRODUCIBLE", "OFF")
     monkeypatch.setenv("SKBUILD_WHEEL_PACKAGES", "j; k; l")
     monkeypatch.setenv("SKBUILD_WHEEL_PY_API", "cp39")
     monkeypatch.setenv("SKBUILD_WHEEL_EXPAND_MACOS_UNIVERSAL_TAGS", "True")
+    monkeypatch.setenv("SKBUILD_WHEEL_LICENSE_FILES", "a;b;c")
     monkeypatch.setenv("SKBUILD_BACKPORT_FIND_PYTHON", "0")
     monkeypatch.setenv("SKBUILD_STRICT_CONFIG", "0")
     monkeypatch.setenv("SKBUILD_EXPERIMENTAL", "1")
     monkeypatch.setenv("SKBUILD_MINIMUM_VERSION", "0.1")
     monkeypatch.setenv("SKBUILD_CMAKE_VERBOSE", "TRUE")
     monkeypatch.setenv("SKBUILD_BUILD_DIR", "a/b/c")
     monkeypatch.setenv("SKBUILD_EDITABLE_REBUILD", "True")
@@ -85,22 +89,24 @@
 
     assert settings.ninja.minimum_version == "1.1"
     assert settings.cmake.minimum_version == "3.16"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
+    assert settings.cmake.source_dir == "a/b/c"
     assert not settings.ninja.make_fallback
     assert settings.logging.level == "DEBUG"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
+    assert settings.wheel.license_files == ["a", "b", "c"]
     assert settings.backport.find_python == "0"
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
@@ -121,21 +127,23 @@
         "ninja.make-fallback": "False",
         "cmake.minimum-version": "3.17",
         "cmake.args": ["-DFOO=BAR", "-DBAR=FOO"],
         "cmake.define.a": "1",
         "cmake.define.b": "2",
         "cmake.verbose": "true",
         "cmake.build-type": "Debug",
+        "cmake.source-dir": "a/b/c",
         "logging.level": "INFO",
         "sdist.include": ["a", "b", "c"],
         "sdist.exclude": "d;e;f",
         "sdist.reproducible": "false",
         "wheel.packages": ["j", "k", "l"],
         "wheel.py-api": "cp39",
         "wheel.expand-macos-universal-tags": "True",
+        "wheel.license-files": ["a", "b", "c"],
         "backport.find-python": "",
         "strict-config": "false",
         "experimental": "1",
         "minimum-version": "0.1",
         "build-dir": "a/b/c",
         "editable.mode": "redirect",
         "editable.rebuild": "True",
@@ -149,21 +157,23 @@
     assert settings.ninja.minimum_version == "1.2"
     assert not settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.17"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
+    assert settings.cmake.source_dir == "a/b/c"
     assert settings.logging.level == "INFO"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
+    assert settings.wheel.license_files == ["a", "b", "c"]
     assert settings.backport.find_python == ""
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {}
     assert settings.editable.mode == "redirect"
@@ -183,21 +193,23 @@
             ninja.minimum-version = "1.3"
             ninja.make-fallback = false
             cmake.minimum-version = "3.18"
             cmake.args = ["-DFOO=BAR", "-DBAR=FOO"]
             cmake.define = {a = "1", b = "2"}
             cmake.build-type = "Debug"
             cmake.verbose = true
+            cmake.source-dir = "a/b/c"
             logging.level = "ERROR"
             sdist.include = ["a", "b", "c"]
             sdist.exclude = ["d", "e", "f"]
             sdist.reproducible = false
             wheel.packages = ["j", "k", "l"]
             wheel.py-api = "cp39"
             wheel.expand-macos-universal-tags = true
+            wheel.license-files = ["a", "b", "c"]
             backport.find-python = "3.18"
             strict-config = false
             experimental = true
             minimum-version = "0.1"
             build-dir = "a/b/c"
             metadata.version.provider = "a"
             editable.mode = "redirect"
@@ -217,21 +229,23 @@
     assert settings.ninja.minimum_version == "1.3"
     assert not settings.ninja.make_fallback
     assert settings.cmake.minimum_version == "3.18"
     assert settings.cmake.args == ["-DFOO=BAR", "-DBAR=FOO"]
     assert settings.cmake.define == {"a": "1", "b": "2"}
     assert settings.cmake.verbose
     assert settings.cmake.build_type == "Debug"
+    assert settings.cmake.source_dir == "a/b/c"
     assert settings.logging.level == "ERROR"
     assert settings.sdist.include == ["a", "b", "c"]
     assert settings.sdist.exclude == ["d", "e", "f"]
     assert not settings.sdist.reproducible
     assert settings.wheel.packages == ["j", "k", "l"]
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
+    assert settings.wheel.license_files == ["a", "b", "c"]
     assert settings.backport.find_python == "3.18"
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
     assert settings.metadata == {"version": {"provider": "a"}}
     assert settings.editable.mode == "redirect"
```

### Comparing `scikit_build_core-0.3.3/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.0/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.0/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.0/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.0/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.0/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.0/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.0/tests/packages/fortran_example/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # setup project ###
-cmake_minimum_required(VERSION 3.15...3.24)
+cmake_minimum_required(VERSION 3.17.2...3.24)
 
 project(
   fibby
   VERSION 1.0
   DESCRIPTION "FIB module"
   LANGUAGES C Fortran)
```

### Comparing `scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.0/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.0/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.0/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/.gitignore` & `scikit_build_core-0.4.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 /src/scikit_build_core/_version.py
 
 # Common editor files
 *~
 *.swp
 
 # RPM spec file
-!/.distro/scikit-build-core.spec
+!/.distro/*.spec
 /.distro/*.tar.gz
 *.rpm
 
 # ruff
 .ruff_cache/
 
 # OS specific stuff
@@ -166,7 +166,11 @@
 ._*
 .Spotlight-V100
 .Trashes
 ehthumbs.db
 Thumbs.db
 
 .idea/
+# tmt setup
+/.distro/main.fmf
+/.distro/plans/main.fmf
+/.distro/tests/main.fmf
```

### Comparing `scikit_build_core-0.3.3/LICENSE` & `scikit_build_core-0.4.0/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.3/README.md` & `scikit_build_core-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,17 @@
 wheel.expand-macos-universal-tags = false
 
 # This allows you to change the install dir, such as to the package name. The
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
+# The licence file(s) to include in the wheel metadata directory.
+wheel.license-files = ["LICENSE*", "COPYING*", "COPYRIGHT*"]
+
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
 backport.find-python = "3.26.1"
 
 # This is the only editable mode currently
 editable.mode = "redirect"
```

### Comparing `scikit_build_core-0.3.3/pyproject.toml` & `scikit_build_core-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -81,18 +81,19 @@
     "sphinx_inline_tabs",
 ]
 
 [project.urls]
 Homepage = "https://github.com/scikit-build/scikit-build-core"
 Examples = "https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages"
 
-[project.entry-points."distutils.setup_keywords"]
-cmake_extensions = "scikit_build_core.setuptools.extension:cmake_extensions"
-cmake_source_dir = "scikit_build_core.setuptools.extension:cmake_source_dir"
-
+[project.entry-points]
+"distutils.commands".build_cmake = "scikit_build_core.setuptools.build_cmake:BuildCMake"
+"distutils.setup_keywords".cmake_source_dir = "scikit_build_core.setuptools.build_cmake:cmake_source_dir"
+"distutils.setup_keywords".cmake_args = "scikit_build_core.setuptools.build_cmake:cmake_args"
+"setuptools.finalize_distribution_options".scikit_build_entry = "scikit_build_core.setuptools.build_cmake:finalize_distribution_options"
 
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/scikit_build_core/_version.py"
 
 
 [tool.pytest.ini_options]
@@ -233,15 +234,15 @@
 "importlib_metadata".msg = "Use scikit_build_core._compat.importlib.metadata instead."
 "importlib.resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
 "importlib_resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
 
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
-"noxfile.py" = ["T20"]
+"noxfile.py" = ["T20", "TID251"]
 "src/scikit_build_core/resources/*.py" = ["PTH", "ARG002"]
 "src/scikit_build_core/_compat/**.py" = ["TID251"]
 "tests/conftest.py" = ["TID251"]
 
 
 [tool.check-sdist]
 sdist-only = ["src/scikit_build_core/_version.py"]
```

### Comparing `scikit_build_core-0.3.3/PKG-INFO` & `scikit_build_core-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.3.3
+Version: 0.4.0
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Examples, https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -227,14 +227,17 @@
 wheel.expand-macos-universal-tags = false
 
 # This allows you to change the install dir, such as to the package name. The
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
+# The licence file(s) to include in the wheel metadata directory.
+wheel.license-files = ["LICENSE*", "COPYING*", "COPYRIGHT*"]
+
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
 backport.find-python = "3.26.1"
 
 # This is the only editable mode currently
 editable.mode = "redirect"
```

