# Comparing `tmp/pyink-23.3.1.tar.gz` & `tmp/pyink-23.5.0.tar.gz`

## Comparing `pyink-23.3.1.tar` & `pyink-23.5.0.tar`

### file list

```diff
@@ -1,247 +1,247 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pyink-23.3.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyink-23.3.1/CHANGES.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pyink-23.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pyink-23.3.1/test_requirements.txt
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 pyink-23.3.1/tox.ini
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 pyink-23.3.1/.github/workflows/pypi_upload.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyink-23.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0    53351 2020-02-02 00:00:00.000000 pyink-23.3.1/patches/pyink.patch
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyink-23.3.1/src/_pyink_version.py
--rw-r--r--   0        0        0    50415 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/__main__.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/_width_table.py
--rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/brackets.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/cache.py
--rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/comments.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/concurrency.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/const.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/debug.py
--rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/files.py
--rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/handle_ipynb_magics.py
--rw-r--r--   0        0        0    13260 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/ink.py
--rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/ink_adjusted_lines.py
--rw-r--r--   0        0        0    64100 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/linegen.py
--rw-r--r--   0        0        0    38833 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/lines.py
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/mode.py
--rw-r--r--   0        0        0    25971 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/output.py
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/py.typed
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/rusty.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/strings.py
--rw-r--r--   0        0        0    91230 2020-02-02 00:00:00.000000 pyink-23.3.1/src/pyink/trans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/conftest.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/optional.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test.toml
--rw-r--r--   0        0        0   105128 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_black.py
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_format.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_ink_adjusted_lines.py
--rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_ipynb.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/test_trans.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11578 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33380 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45997 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/empty_lines.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/imports.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/indent.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/module_docstring_1.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/module_docstring_2.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/module_docstring_3.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/module_docstring_4.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/nested_brackets.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/nested_brackets_explodes.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/pragma_comments.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink/str_concat_in_func_args.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/disable.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/example.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/majority_quotes.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/majority_quotes.toml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/overrides.toml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/pyink_configs/tool_black.toml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11196 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyink-23.3.1/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pyink-23.3.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pyink-23.3.1/LICENSE
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 pyink-23.3.1/README.md
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 pyink-23.3.1/pyproject.toml
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 pyink-23.3.1/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pyink-23.5.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pyink-23.5.0/CHANGES.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pyink-23.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pyink-23.5.0/test_requirements.txt
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 pyink-23.5.0/tox.ini
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 pyink-23.5.0/.github/workflows/pypi_upload.yml
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyink-23.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0    54767 2020-02-02 00:00:00.000000 pyink-23.5.0/patches/pyink.patch
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyink-23.5.0/src/_pyink_version.py
+-rw-r--r--   0        0        0    50376 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/__main__.py
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/_width_table.py
+-rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/brackets.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/cache.py
+-rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/comments.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/concurrency.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/const.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/debug.py
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/files.py
+-rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/handle_ipynb_magics.py
+-rw-r--r--   0        0        0    13369 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/ink.py
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/ink_adjusted_lines.py
+-rw-r--r--   0        0        0    64347 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/linegen.py
+-rw-r--r--   0        0        0    38852 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/lines.py
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/mode.py
+-rw-r--r--   0        0        0    25986 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/numerics.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/output.py
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/py.typed
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/rusty.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/strings.py
+-rw-r--r--   0        0        0    92099 2020-02-02 00:00:00.000000 pyink-23.5.0/src/pyink/trans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/optional.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test.toml
+-rw-r--r--   0        0        0   105056 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_black.py
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_format.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_ink_adjusted_lines.py
+-rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/test_trans.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11578 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/empty_lines.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/imports.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/indent.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/module_docstring_1.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/module_docstring_2.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/module_docstring_3.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/module_docstring_4.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/nested_brackets.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/nested_brackets_explodes.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/pragma_comments.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink/str_concat_in_func_args.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/disable.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/example.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/majority_quotes.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/majority_quotes.toml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/overrides.toml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/pyink_configs/tool_black.toml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11196 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyink-23.5.0/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pyink-23.5.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pyink-23.5.0/LICENSE
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pyink-23.5.0/README.md
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 pyink-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10977 2020-02-02 00:00:00.000000 pyink-23.5.0/PKG-INFO
```

### Comparing `pyink-23.3.1/CHANGES.md` & `pyink-23.5.0/CHANGES.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 All notable changes to Pyink are recorded here.
 
 ## Unreleased
 
 * Nothing notable unreleased.
 
+## 23.5.0
+
+* Existing parentheses around strings are no longer removed if the content does
+  not fit on a single line. This is related to
+  https://github.com/psf/black/pull/3640 where we still want to keep the
+  parentheses around the implicitly concatenated strings if the code already
+  uses them, making it more obvious it's a single function argument.
+* `--pyink-lines=` now works with stdin inputs (#16).
+* Fixed compatibility issue on Python 3.7 (#13).
+
 ## 23.3.1
 
 * In multiline module docstrings, trailing quotes that are put on their own line
   are now kept on their own line. (#8)
 
 ## 23.3.0
```

### Comparing `pyink-23.3.1/CONTRIBUTING.md` & `pyink-23.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tox.ini` & `pyink-23.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/.github/workflows/pypi_upload.yml` & `pyink-23.5.0/.github/workflows/pypi_upload.yml`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/.github/workflows/test.yml` & `pyink-23.5.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
   contents: read
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.run_id }}
   cancel-in-progress: true
 
 jobs:
-  main:
+  test:
     if:
       github.event_name == 'push' || github.event.pull_request.head.repo.full_name !=
       github.repository
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11",]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11",]
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `pyink-23.3.1/patches/pyink.patch` & `pyink-23.5.0/patches/pyink.patch`

 * *Files 2% similar despite different names*

```diff
@@ -512,47 +512,67 @@
 -                docstring = normalize_string_quotes(docstring)
 +                docstring = normalize_string_quotes(
 +                    docstring, preferred_quote=self.mode.preferred_quote
 +                )
              else:
                  docstring = leaf.value
              prefix = get_string_prefix(docstring)
-@@ -411,7 +442,7 @@ class LineGenerator(Visitor[Line]):
+@@ -411,8 +442,9 @@ class LineGenerator(Visitor[Line]):
              quote_len = 1 if docstring[1] != quote_char else 3
              docstring = docstring[quote_len:-quote_len]
              docstring_started_empty = not docstring
 -            indent = " " * 4 * self.current_line.depth
 +            indent = " " * self.current_line.indentation_spaces()
  
++            original_has_trailing_newline = docstring.endswith("\n")
              if is_multiline_string(leaf):
                  docstring = fix_docstring(docstring, indent)
-@@ -453,7 +484,11 @@ class LineGenerator(Visitor[Line]):
+             else:
+@@ -453,7 +485,13 @@ class LineGenerator(Visitor[Line]):
                  # If docstring is one line, we don't put the closing quotes on a
                  # separate line because it looks ugly (#3320).
                  lines = docstring.splitlines()
 -                last_line_length = len(lines[-1]) if docstring else 0
 +                last_line_length = (
 +                    # When docstring ends with '\n' the last line is empty,
 +                    # not the last item from splitlines().
-+                    len(lines[-1]) if docstring and not docstring.endswith("\n") else 0
++                    len(lines[-1])
++                    if docstring and not docstring.endswith("\n")
++                    else 0
 +                )
  
                  # If adding closing quotes would cause the last line to exceed
                  # the maximum line length then put a line break before the
-@@ -492,7 +527,8 @@ class LineGenerator(Visitor[Line]):
+@@ -465,6 +503,15 @@ class LineGenerator(Visitor[Line]):
+                     and not has_trailing_backslash
+                 ):
+                     leaf.value = prefix + quote + docstring + "\n" + indent + quote
++                elif (
++                    not indent
++                    and len(lines) > 1
++                    and not docstring.endswith("\n")
++                    and original_has_trailing_newline
++                ):
++                    # Special case for module docstrings that put trailing quotes on
++                    # their own line.
++                    leaf.value = prefix + quote + docstring + "\n" + indent + quote
+                 else:
+                     leaf.value = prefix + quote + docstring + quote
+             else:
+@@ -492,7 +539,8 @@ class LineGenerator(Visitor[Line]):
          self.visit_classdef = partial(v, keywords={"class"}, parens=Ø)
          self.visit_expr_stmt = partial(v, keywords=Ø, parens=ASSIGNMENTS)
          self.visit_return_stmt = partial(v, keywords={"return"}, parens={"return"})
 -        self.visit_import_from = partial(v, keywords=Ø, parens={"import"})
 +        if not self.mode.is_pyink:
 +            self.visit_import_from = partial(v, keywords=Ø, parens={"import"})
          self.visit_del_stmt = partial(v, keywords=Ø, parens={"del"})
          self.visit_async_funcdef = self.visit_async_stmt
          self.visit_decorated = self.visit_decorators
-@@ -519,10 +555,11 @@ def transform_line(
+@@ -519,10 +567,11 @@ def transform_line(
  
      ll = mode.line_length
      sn = mode.string_normalization
 -    string_merge = StringMerger(ll, sn)
 -    string_paren_strip = StringParenStripper(ll, sn)
 -    string_split = StringSplitter(ll, sn)
 -    string_paren_wrap = StringParenWrapper(ll, sn)
@@ -560,25 +580,25 @@
 +    string_merge = StringMerger(ll, sn, preferred_quote=preferred_quote)
 +    string_paren_strip = StringParenStripper(ll, sn, preferred_quote=preferred_quote)
 +    string_split = StringSplitter(ll, sn, preferred_quote=preferred_quote)
 +    string_paren_wrap = StringParenWrapper(ll, sn, preferred_quote=preferred_quote)
  
      transformers: List[Transformer]
      if (
-@@ -697,8 +734,7 @@ def _first_right_hand_split(
+@@ -697,8 +746,7 @@ def _first_right_hand_split(
      omit: Collection[LeafID] = (),
  ) -> RHSResult:
      """Split the line into head, body, tail starting with the last bracket pair.
 -
 -    Note: this function should not have side effects. It's relied upon by
 +    Note: this function should not have side effects. It's replied upon by
      _maybe_split_omitting_optional_parens to get an opinion whether to prefer
      splitting on the right side of an assignment statement.
      """
-@@ -727,12 +763,53 @@ def _first_right_hand_split(
+@@ -727,12 +775,53 @@ def _first_right_hand_split(
      tail_leaves.reverse()
      body_leaves.reverse()
      head_leaves.reverse()
 +
 +    opening_brackets: List[Leaf] = [opening_bracket]
 +    closing_brackets: List[Leaf] = [closing_bracket]
 +    body: Optional[Line] = None
@@ -627,24 +647,24 @@
 +    if body is None:
 +        body = bracket_split_build_line(
 +            body_leaves, line, opening_bracket, component=_BracketSplitComponent.body
 +        )
      tail = bracket_split_build_line(
          tail_leaves, line, opening_bracket, component=_BracketSplitComponent.tail
      )
-@@ -891,7 +968,7 @@ def bracket_split_build_line(
+@@ -891,7 +980,7 @@ def bracket_split_build_line(
      result = Line(mode=original.mode, depth=original.depth)
      if component is _BracketSplitComponent.body:
          result.inside_brackets = True
 -        result.depth += 1
 +        result.depth = result.depth + (Indentation.CONTINUATION,)
          if leaves:
              # Since body is a new indent level, remove spurious leading whitespace.
              normalize_prefix(leaves[0], inside_brackets=True)
-@@ -1449,7 +1526,7 @@ def generate_trailers_to_omit(line: Line
+@@ -1449,7 +1538,7 @@ def generate_trailers_to_omit(line: Line
      if not line.magic_trailing_comma:
          yield omit
  
 -    length = 4 * line.depth
 +    length = line.indentation_spaces()
      opening_bracket: Optional[Leaf] = None
      closing_bracket: Optional[Leaf] = None
@@ -890,22 +910,29 @@
  from hashlib import sha256
  from operator import attrgetter
 -from typing import Dict, Set
 +from typing import Dict, Literal, Set
  from warnings import warn
  
  if sys.version_info < (3, 8):
-@@ -172,11 +172,26 @@ class Deprecated(UserWarning):
+@@ -172,11 +172,33 @@ class Deprecated(UserWarning):
      """Visible deprecation warning."""
  
  
 +class Quote(Enum):
 +    SINGLE = "'"
 +    DOUBLE = '"'
 +
++    def cache_key(self) -> str:
++        # On Windows, paths can't contain a double quote.
++        if self == Quote.SINGLE:
++            return "0"
++        else:
++            return "1"
++
 +
 +class QuoteStyle(Enum):
 +    SINGLE = auto()
 +    DOUBLE = auto()
 +    MAJORITY = auto()
 +
 +
@@ -917,29 +944,29 @@
 +    # No effect if string_normalization is False
 +    quote_style: QuoteStyle = QuoteStyle.DOUBLE
 +    # Overridden later when quote_style is MAJORITY
 +    majority_quote: Quote = Quote.DOUBLE
      is_pyi: bool = False
      is_ipynb: bool = False
      skip_source_first_line: bool = False
-@@ -184,6 +199,8 @@ class Mode:
+@@ -184,6 +206,8 @@ class Mode:
      experimental_string_processing: bool = False
      python_cell_magics: Set[str] = field(default_factory=set)
      preview: bool = False
 +    is_pyink: bool = False
 +    pyink_indentation: Literal[2, 4] = 4
  
      def __post_init__(self) -> None:
          if self.experimental_string_processing:
-@@ -218,12 +235,25 @@ class Mode:
+@@ -218,12 +242,25 @@ class Mode:
              version_str,
              str(self.line_length),
              str(int(self.string_normalization)),
 +            str(self.quote_style.value),
-+            self.majority_quote.value,
++            self.majority_quote.cache_key(),
              str(int(self.is_pyi)),
              str(int(self.is_ipynb)),
              str(int(self.skip_source_first_line)),
              str(int(self.magic_trailing_comma)),
              str(int(self.experimental_string_processing)),
              str(int(self.preview)),
 +            str(int(self.is_pyink)),
@@ -1174,53 +1201,58 @@
                  fast=True,
                  write_back=pyink.WriteBack.YES,
                  mode=replace(DEFAULT_MODE, is_ipynb=True),
 +                lines=None,
              )
              # __PYINK_STDIN_FILENAME__ should have been stripped
              report.done.assert_called_with(expected, pyink.Changed.YES)
-@@ -2459,6 +2461,113 @@ class TestFileCollection:
+@@ -2459,6 +2461,119 @@ class TestFileCollection:
              stdin_filename=stdin_filename,
          )
  
++    def decode_and_normalized(self, stdout: bytes) -> str:
++        # Make it easier to test on Windows. The test doesn't care about
++        # newlines.
++        return stdout.decode().replace("\r\n", "\n")
++
 +    def test_pyink_default(self) -> None:
 +        path = THIS_DIR / "data" / "pyink_configs"
 +        example = str(path / "example.py")
 +        config = str(THIS_DIR / "empty.toml")
 +        result = BlackRunner().invoke(
 +            pyink.main, ["--diff", "--config", config, example]
 +        )
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
-+        assert "- pass\n+    pass\n" in result.stdout_bytes.decode()
++        assert "- pass\n+    pass\n" in self.decode_and_normalized(result.stdout_bytes)
 +
 +    def test_pyink_overrides(self) -> None:
 +        path = THIS_DIR / "data" / "pyink_configs"
 +        example = str(path / "example.py")
 +        config = str(path / "overrides.toml")
 +        result = BlackRunner().invoke(
 +            pyink.main, ["--diff", "--config", config, example]
 +        )
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
-+        assert "- pass\n+  pass\n" in result.stdout_bytes.decode()
++        assert "- pass\n+  pass\n" in self.decode_and_normalized(result.stdout_bytes)
 +
 +    def test_pyink_disable(self) -> None:
 +        path = THIS_DIR / "data" / "pyink_configs"
 +        example = str(path / "example.py")
 +        config = str(path / "disable.toml")
 +        result = BlackRunner().invoke(
 +            pyink.main, ["--diff", "--config", config, example]
 +        )
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
-+        stdout = result.stdout_bytes.decode()
++        stdout = self.decode_and_normalized(result.stdout_bytes)
 +        assert (
 +            """\
 +-from very.long.package.path.my_org.my_very_long_project_name.awesome_backend.core_framework.util import my_long_module_name
 ++from very.long.package.path.my_org.my_very_long_project_name.awesome_backend.core_framework.util import (
 ++    my_long_module_name,
 ++)
 +"""
@@ -1234,15 +1266,15 @@
 +        config = str(path / "tool_black.toml")
 +        result = BlackRunner().invoke(
 +            pyink.main, ["--diff", "--config", config, example]
 +        )
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
-+        assert "- pass\n+    pass\n" in result.stdout_bytes.decode()
++        assert "- pass\n+    pass\n" in self.decode_and_normalized(result.stdout_bytes)
 +
 +    @pytest.mark.parametrize("values", [("7-7",), ("1-1", "7-7")])
 +    def test_pyink_lines(self, values) -> None:
 +        path = THIS_DIR / "data" / "pyink_configs"
 +        example = str(path / "example.py")
 +        pyink_lines_args = []
 +        for value in values:
@@ -1250,16 +1282,17 @@
 +        result = BlackRunner().invoke(
 +            pyink.main, pyink_lines_args + ["--diff", example]
 +        )
 +        assert result.stdout_bytes is not None
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
-+        assert "-from" not in result.stderr_bytes.decode()
-+        assert "- pass\n+    pass\n" in result.stdout_bytes.decode()
++        stdout = self.decode_and_normalized(result.stdout_bytes)
++        assert "-from" not in stdout
++        assert "- pass\n+    pass\n" in stdout
 +
 +    @pytest.mark.parametrize(
 +        "value,message",
 +        [
 +            ("1,2", "Incorrect --pyink-lines format, expect 'START-END'"),
 +            (
 +                "start-end",
@@ -1283,15 +1316,15 @@
 +        result = BlackRunner().invoke(
 +            pyink.main, ["--diff", "--config", config, example]
 +        )
 +        assert result.exit_code == 0
 +        assert result.stdout_bytes is not None
 +
 +        diff = """-_double = "Double"\n+_double = 'Double'\n"""
-+        assert diff in result.stdout_bytes.decode()
++        assert diff in self.decode_and_normalized(result.stdout_bytes)
 +
  
  try:
      with open(pyink.__file__, "r", encoding="utf-8") as _bf:
 --- a/tests/test_format.py
 +++ b/tests/test_format.py
 @@ -43,6 +43,15 @@ def test_preview_format(filename: str) -
```

### Comparing `pyink-23.3.1/src/pyink/__init__.py` & `pyink-23.5.0/src/pyink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,18 +542,16 @@
             out(f"Sources to be formatted: {srcs_string}", fg="blue")
 
         if config:
             config_source = ctx.get_parameter_source("config")
             user_level_config = str(find_user_pyproject_toml())
             if config == user_level_config:
                 out(
-                    (
-                        "Using configuration from user-level config at "
-                        f"'{user_level_config}'."
-                    ),
+                    "Using configuration from user-level config at "
+                    f"'{user_level_config}'.",
                     fg="blue",
                 )
             elif config_source in (
                 ParameterSource.DEFAULT,
                 ParameterSource.DEFAULT_MAP,
             ):
                 out("Using configuration from project root.", fg="blue")
@@ -961,15 +959,15 @@
     if content is None:
         src, encoding, newline = decode_bytes(sys.stdin.buffer.read())
     else:
         src, encoding, newline = content, "utf-8", ""
 
     dst = src
     try:
-        dst = format_file_contents(src, fast=fast, mode=mode)
+        dst = format_file_contents(src, fast=fast, mode=mode, lines=lines)
         return True
 
     except NothingChanged:
         return False
 
     finally:
         f = io.TextIOWrapper(
```

### Comparing `pyink-23.3.1/src/pyink/_width_table.py` & `pyink-23.5.0/src/pyink/_width_table.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/brackets.py` & `pyink-23.5.0/src/pyink/brackets.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/cache.py` & `pyink-23.5.0/src/pyink/cache.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/comments.py` & `pyink-23.5.0/src/pyink/comments.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/concurrency.py` & `pyink-23.5.0/src/pyink/concurrency.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/debug.py` & `pyink-23.5.0/src/pyink/debug.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/files.py` & `pyink-23.5.0/src/pyink/files.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/handle_ipynb_magics.py` & `pyink-23.5.0/src/pyink/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/ink.py` & `pyink-23.5.0/src/pyink/ink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Module that contains Pyink specific additions to Black.
 
 This is a separate module for easier patch management.
 """
 
+import sys
 from typing import (
     Collection,
     List,
-    Literal,
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
     Iterator,
 )
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Literal
+else:
+    from typing import Literal
+
 from blib2to3.pgen2.token import ASYNC, NEWLINE, STRING
 from blib2to3.pytree import type_repr
 from pyink.mode import Quote
 from pyink.nodes import LN, Leaf, Node, STANDALONE_COMMENT, syms, Visitor
 from pyink.strings import STRING_PREFIX_CHARS
```

### Comparing `pyink-23.3.1/src/pyink/ink_adjusted_lines.py` & `pyink-23.5.0/src/pyink/ink_adjusted_lines.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/linegen.py` & `pyink-23.5.0/src/pyink/linegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 Generating lines of code.
 """
 import sys
 from dataclasses import replace
 from enum import Enum, auto
 from functools import partial, wraps
-from typing import Collection, Iterator, List, Literal, Optional, Set, Union, cast
+from typing import Collection, Iterator, List, Optional, Set, Union, cast
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Final, Literal
+else:
+    from typing import Final, Literal
 
 from pyink.brackets import (
     COMMA_PRIORITY,
     DOT_PRIORITY,
     get_leaves_inside_matching_brackets,
     max_delimiter_priority_in_atom,
 )
@@ -555,18 +560,26 @@
         return
 
     line_str = line_to_string(line)
 
     ll = mode.line_length
     sn = mode.string_normalization
     preferred_quote = mode.preferred_quote
-    string_merge = StringMerger(ll, sn, preferred_quote=preferred_quote)
-    string_paren_strip = StringParenStripper(ll, sn, preferred_quote=preferred_quote)
-    string_split = StringSplitter(ll, sn, preferred_quote=preferred_quote)
-    string_paren_wrap = StringParenWrapper(ll, sn, preferred_quote=preferred_quote)
+    string_merge = StringMerger(
+        ll, sn, preferred_quote=preferred_quote, line_str=line_str
+    )
+    string_paren_strip = StringParenStripper(
+        ll, sn, preferred_quote=preferred_quote, line_str=line_str
+    )
+    string_split = StringSplitter(
+        ll, sn, preferred_quote=preferred_quote, line_str=line_str
+    )
+    string_paren_wrap = StringParenWrapper(
+        ll, sn, preferred_quote=preferred_quote, line_str=line_str
+    )
 
     transformers: List[Transformer]
     if (
         not line.contains_uncollapsable_type_comments()
         and not line.should_split_rhs
         and not line.magic_trailing_comma
         and (
```

### Comparing `pyink-23.3.1/src/pyink/lines.py` & `pyink-23.5.0/src/pyink/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,15 +848,15 @@
     # is needed to determine nesting level of the MLS.
     # Includes special case for trailing commas.
     commas: List[int] = []  # tracks number of commas per depth level
     multiline_string: Optional[Leaf] = None
     # store the leaves that contain parts of the MLS
     multiline_string_contexts: List[LN] = []
 
-    max_level_to_update = math.inf  # track the depth of the MLS
+    max_level_to_update: Union[int, float] = math.inf  # track the depth of the MLS
     for i, leaf in enumerate(line.leaves):
         if max_level_to_update == math.inf:
             had_comma: Optional[int] = None
             if leaf.bracket_depth + 1 > len(commas):
                 commas.append(0)
             elif leaf.bracket_depth + 1 < len(commas):
                 had_comma = commas.pop()
```

### Comparing `pyink-23.3.1/src/pyink/mode.py` & `pyink-23.5.0/src/pyink/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 """
 
 import sys
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from hashlib import sha256
 from operator import attrgetter
-from typing import Dict, Literal, Set
+from typing import Dict, Set
 from warnings import warn
 
 if sys.version_info < (3, 8):
-    from typing_extensions import Final
+    from typing_extensions import Final, Literal
 else:
-    from typing import Final
+    from typing import Final, Literal
 
 from pyink.const import DEFAULT_LINE_LENGTH
 
 
 class TargetVersion(Enum):
     PY33 = 3
     PY34 = 4
@@ -172,14 +172,21 @@
     """Visible deprecation warning."""
 
 
 class Quote(Enum):
     SINGLE = "'"
     DOUBLE = '"'
 
+    def cache_key(self) -> str:
+        # On Windows, paths can't contain a double quote.
+        if self == Quote.SINGLE:
+            return "0"
+        else:
+            return "1"
+
 
 class QuoteStyle(Enum):
     SINGLE = auto()
     DOUBLE = auto()
     MAJORITY = auto()
 
 
@@ -201,18 +208,16 @@
     preview: bool = False
     is_pyink: bool = False
     pyink_indentation: Literal[2, 4] = 4
 
     def __post_init__(self) -> None:
         if self.experimental_string_processing:
             warn(
-                (
-                    "`experimental string processing` has been included in `preview`"
-                    " and deprecated. Use `preview` instead."
-                ),
+                "`experimental string processing` has been included in `preview`"
+                " and deprecated. Use `preview` instead.",
                 Deprecated,
             )
 
     def __contains__(self, feature: Preview) -> bool:
         """
         Provide `Preview.FEATURE in Mode` syntax that mirrors the ``preview`` flag.
 
@@ -232,15 +237,15 @@
         else:
             version_str = "-"
         parts = [
             version_str,
             str(self.line_length),
             str(int(self.string_normalization)),
             str(self.quote_style.value),
-            self.majority_quote.value,
+            self.majority_quote.cache_key(),
             str(int(self.is_pyi)),
             str(int(self.is_ipynb)),
             str(int(self.skip_source_first_line)),
             str(int(self.magic_trailing_comma)),
             str(int(self.experimental_string_processing)),
             str(int(self.preview)),
             str(int(self.is_pyink)),
```

### Comparing `pyink-23.3.1/src/pyink/nodes.py` & `pyink-23.5.0/src/pyink/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
 
 def whitespace(leaf: Leaf, *, complex_subscript: bool) -> str:  # noqa: C901
     """Return whitespace prefix if needed for the given `leaf`.
 
     `complex_subscript` signals whether the given leaf is part of a subscription
     which has non-trivial arguments, like arithmetic expressions or function calls.
     """
-    NO: Final = ""
-    SPACE: Final = " "
-    DOUBLESPACE: Final = "  "
+    NO: Final[str] = ""
+    SPACE: Final[str] = " "
+    DOUBLESPACE: Final[str] = "  "
     t = leaf.type
     p = leaf.parent
     v = leaf.value
     if t in ALWAYS_NO_SPACE:
         return NO
 
     if t == token.COMMENT:
```

### Comparing `pyink-23.3.1/src/pyink/numerics.py` & `pyink-23.5.0/src/pyink/numerics.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/output.py` & `pyink-23.5.0/src/pyink/output.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/parsing.py` & `pyink-23.5.0/src/pyink/parsing.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/report.py` & `pyink-23.5.0/src/pyink/report.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/rusty.py` & `pyink-23.5.0/src/pyink/rusty.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/strings.py` & `pyink-23.5.0/src/pyink/strings.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/src/pyink/trans.py` & `pyink-23.5.0/src/pyink/trans.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,25 @@
     """
 
     __name__: Final = "StringTransformer"
 
     # Ideally this would be a dataclass, but unfortunately mypyc breaks when used with
     # `abc.ABC`.
     def __init__(
-        self, line_length: int, normalize_strings: bool, *, preferred_quote: Quote
+        self,
+        line_length: int,
+        normalize_strings: bool,
+        *,
+        preferred_quote: Quote,
+        line_str: str,
     ) -> None:
         self.line_length = line_length
         self.normalize_strings = normalize_strings
         self.preferred_quote = preferred_quote
+        self.line_str = line_str
 
     @abstractmethod
     def do_match(self, line: Line) -> TMatchResult:
         """
         Returns:
             * Ok(string_indices) such that for each index, `line.leaves[index]`
             is our target string if a match was able to be made. For
@@ -895,15 +901,21 @@
 
                 string_indices.append(string_idx)
                 idx = string_idx
                 while idx < len(LL) - 1 and LL[idx + 1].type == token.STRING:
                     idx += 1
 
         if string_indices:
-            return Ok(string_indices)
+            if (
+                not line.mode.is_pyink
+                or len(self.line_str) - len(string_indices) * 2 <= self.line_length
+            ):
+                return Ok(string_indices)
+            else:
+                return TErr("With parens stripped, the line is still too long.")
         return TErr("This line has no strings wrapped in parens.")
 
     def do_transform(
         self, line: Line, string_indices: List[int]
     ) -> Iterator[TResult[Line]]:
         LL = line.leaves
 
@@ -1187,27 +1199,41 @@
                 OR
             None, otherwise.
         """
         # The line must start with a string.
         if LL[0].type != token.STRING:
             return None
 
-        # If the string is surrounded by commas (or is the first/last child)...
-        prev_sibling = LL[0].prev_sibling
-        next_sibling = LL[0].next_sibling
-        if not prev_sibling and not next_sibling and parent_type(LL[0]) == syms.atom:
-            # If it's an atom string, we need to check the parent atom's siblings.
-            parent = LL[0].parent
-            assert parent is not None  # For type checkers.
-            prev_sibling = parent.prev_sibling
-            next_sibling = parent.next_sibling
-        if (not prev_sibling or prev_sibling.type == token.COMMA) and (
-            not next_sibling or next_sibling.type == token.COMMA
+        matching_nodes = [
+            syms.listmaker,
+            syms.dictsetmaker,
+            syms.testlist_gexp,
+        ]
+        # If the string is an immediate child of a list/set/tuple literal...
+        if (
+            parent_type(LL[0]) in matching_nodes
+            or parent_type(LL[0].parent) in matching_nodes
         ):
-            return 0
+            # And the string is surrounded by commas (or is the first/last child)...
+            prev_sibling = LL[0].prev_sibling
+            next_sibling = LL[0].next_sibling
+            if (
+                not prev_sibling
+                and not next_sibling
+                and parent_type(LL[0]) == syms.atom
+            ):
+                # If it's an atom string, we need to check the parent atom's siblings.
+                parent = LL[0].parent
+                assert parent is not None  # For type checkers.
+                prev_sibling = parent.prev_sibling
+                next_sibling = parent.next_sibling
+            if (not prev_sibling or prev_sibling.type == token.COMMA) and (
+                not next_sibling or next_sibling.type == token.COMMA
+            ):
+                return 0
 
         return None
 
 
 def iter_fexpr_spans(s: str) -> Iterator[Tuple[int, int]]:
     """
     Yields spans corresponding to expressions in a given f-string.
@@ -1814,16 +1840,17 @@
             OR
         * The line is a dictionary key assignment where some valid key is being
         assigned the value of some string.
             OR
         * The line is an lambda expression and the value is a string.
             OR
         * The line starts with an "atom" string that prefers to be wrapped in
-        parens. It's preferred to be wrapped when the string is surrounded by
-        commas (or is the first/last child).
+        parens. It's preferred to be wrapped when it's is an immediate child of
+        a list/set/tuple literal, AND the string is surrounded by commas (or is
+        the first/last child).
 
     Transformations:
         The chosen string is wrapped in parentheses and then split at the LPAR.
 
         We then have one line which ends with an LPAR and another line that
         starts with the chosen string. The latter line is then split again at
         the RPAR. This results in the RPAR (and possibly a trailing comma)
```

### Comparing `pyink-23.3.1/tests/optional.py` & `pyink-23.5.0/tests/optional.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/test_black.py` & `pyink-23.5.0/tests/test_black.py`

 * *Files 1% similar despite different names*

```diff
@@ -1407,5165 +1407,5160 @@
 000057e0: 696e 6573 5b2d 315d 2c20 2265 7272 6f72  ines[-1], "error
 000057f0: 3a20 6361 6e6e 6f74 2066 6f72 6d61 7420  : cannot format 
 00005800: 6531 3a20 626f 6f6d 2229 0a20 2020 2020  e1: boom").     
 00005810: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
 00005820: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
 00005830: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
 00005840: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
-00005850: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00005860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005870: 2020 2020 2022 3120 6669 6c65 2072 6566       "1 file ref
-00005880: 6f72 6d61 7474 6564 2c20 3220 6669 6c65  ormatted, 2 file
-00005890: 7320 6c65 6674 2075 6e63 6861 6e67 6564  s left unchanged
-000058a0: 2c20 3120 6669 6c65 2066 6169 6c65 6420  , 1 file failed 
-000058b0: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-000058c0: 2020 2020 2020 2020 2220 7265 666f 726d          " reform
-000058d0: 6174 2e22 0a20 2020 2020 2020 2020 2020  at.".           
-000058e0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-000058f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00005900: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00005910: 616c 2872 6570 6f72 742e 7265 7475 726e  al(report.return
-00005920: 5f63 6f64 652c 2031 3233 290a 2020 2020  _code, 123).    
-00005930: 2020 2020 2020 2020 7265 706f 7274 2e64          report.d
-00005940: 6f6e 6528 5061 7468 2822 6633 2229 2c20  one(Path("f3"), 
-00005950: 7079 696e 6b2e 4368 616e 6765 642e 5945  pyink.Changed.YE
-00005960: 5329 0a20 2020 2020 2020 2020 2020 2073  S).            s
-00005970: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00005980: 6c65 6e28 6f75 745f 6c69 6e65 7329 2c20  len(out_lines), 
-00005990: 3429 0a20 2020 2020 2020 2020 2020 2073  4).            s
-000059a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000059b0: 6c65 6e28 6572 725f 6c69 6e65 7329 2c20  len(err_lines), 
-000059c0: 3129 0a20 2020 2020 2020 2020 2020 2073  1).            s
-000059d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000059e0: 6f75 745f 6c69 6e65 735b 2d31 5d2c 2022  out_lines[-1], "
-000059f0: 7265 666f 726d 6174 7465 6420 6633 2229  reformatted f3")
-00005a00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005a10: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00005a30: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
-00005a40: 7429 292c 0a20 2020 2020 2020 2020 2020  t)),.           
-00005a50: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-00005a60: 2020 2020 2020 2020 2020 2022 3220 6669             "2 fi
-00005a70: 6c65 7320 7265 666f 726d 6174 7465 642c  les reformatted,
-00005a80: 2032 2066 696c 6573 206c 6566 7420 756e   2 files left un
-00005a90: 6368 616e 6765 642c 2031 2066 696c 6520  changed, 1 file 
-00005aa0: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005ac0: 2072 6566 6f72 6d61 742e 220a 2020 2020   reformat.".    
-00005ad0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00005ae0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00005af0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00005b00: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
-00005b10: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
-00005b20: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
-00005b30: 6570 6f72 742e 6661 696c 6564 2850 6174  eport.failed(Pat
-00005b40: 6828 2265 3222 292c 2022 626f 6f6d 2229  h("e2"), "boom")
-00005b50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005b60: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00005b70: 6e28 6f75 745f 6c69 6e65 7329 2c20 3429  n(out_lines), 4)
-00005b80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005b90: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00005ba0: 6e28 6572 725f 6c69 6e65 7329 2c20 3229  n(err_lines), 2)
-00005bb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005bc0: 662e 6173 7365 7274 4571 7561 6c28 6572  f.assertEqual(er
-00005bd0: 725f 6c69 6e65 735b 2d31 5d2c 2022 6572  r_lines[-1], "er
-00005be0: 726f 723a 2063 616e 6e6f 7420 666f 726d  ror: cannot form
-00005bf0: 6174 2065 323a 2062 6f6f 6d22 290a 2020  at e2: boom").  
-00005c00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00005c10: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00005c20: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00005c30: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00005c40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005c50: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00005c60: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00005c70: 2072 6566 6f72 6d61 7474 6564 2c20 3220   reformatted, 2 
-00005c80: 6669 6c65 7320 6c65 6674 2075 6e63 6861  files left uncha
-00005c90: 6e67 6564 2c20 3220 6669 6c65 7320 6661  nged, 2 files fa
-00005ca0: 696c 6564 2074 6f22 0a20 2020 2020 2020  iled to".       
-00005cb0: 2020 2020 2020 2020 2020 2020 2022 2072               " r
-00005cc0: 6566 6f72 6d61 742e 220a 2020 2020 2020  eformat.".      
-00005cd0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00005ce0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00005cf0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00005d00: 7274 4571 7561 6c28 7265 706f 7274 2e72  rtEqual(report.r
-00005d10: 6574 7572 6e5f 636f 6465 2c20 3132 3329  eturn_code, 123)
-00005d20: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00005d30: 6f72 742e 7061 7468 5f69 676e 6f72 6564  ort.path_ignored
-00005d40: 2850 6174 6828 2277 6174 2229 2c20 226e  (Path("wat"), "n
-00005d50: 6f20 6d61 7463 6822 290a 2020 2020 2020  o match").      
-00005d60: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00005d70: 7445 7175 616c 286c 656e 286f 7574 5f6c  tEqual(len(out_l
-00005d80: 696e 6573 292c 2035 290a 2020 2020 2020  ines), 5).      
-00005d90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00005da0: 7445 7175 616c 286c 656e 2865 7272 5f6c  tEqual(len(err_l
-00005db0: 696e 6573 292c 2032 290a 2020 2020 2020  ines), 2).      
-00005dc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00005dd0: 7445 7175 616c 286f 7574 5f6c 696e 6573  tEqual(out_lines
-00005de0: 5b2d 315d 2c20 2277 6174 2069 676e 6f72  [-1], "wat ignor
-00005df0: 6564 3a20 6e6f 206d 6174 6368 2229 0a20  ed: no match"). 
-00005e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005e10: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00005e20: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00005e30: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00005e40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00005e50: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-00005e60: 2020 2020 2020 2020 2022 3220 6669 6c65           "2 file
-00005e70: 7320 7265 666f 726d 6174 7465 642c 2032  s reformatted, 2
-00005e80: 2066 696c 6573 206c 6566 7420 756e 6368   files left unch
-00005e90: 616e 6765 642c 2032 2066 696c 6573 2066  anged, 2 files f
-00005ea0: 6169 6c65 6420 746f 220a 2020 2020 2020  ailed to".      
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-00005ec0: 7265 666f 726d 6174 2e22 0a20 2020 2020  reformat.".     
-00005ed0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00005ee0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00005ef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00005f00: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
-00005f10: 7265 7475 726e 5f63 6f64 652c 2031 3233  return_code, 123
-00005f20: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00005f30: 706f 7274 2e64 6f6e 6528 5061 7468 2822  port.done(Path("
-00005f40: 6634 2229 2c20 7079 696e 6b2e 4368 616e  f4"), pyink.Chan
-00005f50: 6765 642e 4e4f 290a 2020 2020 2020 2020  ged.NO).        
-00005f60: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00005f70: 7175 616c 286c 656e 286f 7574 5f6c 696e  qual(len(out_lin
-00005f80: 6573 292c 2036 290a 2020 2020 2020 2020  es), 6).        
-00005f90: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00005fa0: 7175 616c 286c 656e 2865 7272 5f6c 696e  qual(len(err_lin
-00005fb0: 6573 292c 2032 290a 2020 2020 2020 2020  es), 2).        
-00005fc0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00005fd0: 7175 616c 286f 7574 5f6c 696e 6573 5b2d  qual(out_lines[-
-00005fe0: 315d 2c20 2266 3420 616c 7265 6164 7920  1], "f4 already 
-00005ff0: 7765 6c6c 2066 6f72 6d61 7474 6564 2c20  well formatted, 
-00006000: 676f 6f64 206a 6f62 2e22 290a 2020 2020  good job.").    
-00006010: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00006020: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-00006030: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
-00006040: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006070: 2020 2020 2020 2232 2066 696c 6573 2072        "2 files r
-00006080: 6566 6f72 6d61 7474 6564 2c20 3320 6669  eformatted, 3 fi
-00006090: 6c65 7320 6c65 6674 2075 6e63 6861 6e67  les left unchang
-000060a0: 6564 2c20 3220 6669 6c65 7320 6661 696c  ed, 2 files fail
-000060b0: 6564 2074 6f22 0a20 2020 2020 2020 2020  ed to".         
-000060c0: 2020 2020 2020 2020 2020 2022 2072 6566             " ref
-000060d0: 6f72 6d61 742e 220a 2020 2020 2020 2020  ormat.".        
-000060e0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000060f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00006100: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006110: 4571 7561 6c28 7265 706f 7274 2e72 6574  Equal(report.ret
-00006120: 7572 6e5f 636f 6465 2c20 3132 3329 0a20  urn_code, 123). 
-00006130: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-00006140: 742e 6368 6563 6b20 3d20 5472 7565 0a20  t.check = True. 
-00006150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006160: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00006170: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00006180: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00006190: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000061a0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-000061b0: 2020 2020 2020 2020 2022 3220 6669 6c65           "2 file
-000061c0: 7320 776f 756c 6420 6265 2072 6566 6f72  s would be refor
-000061d0: 6d61 7474 6564 2c20 3320 6669 6c65 7320  matted, 3 files 
-000061e0: 776f 756c 6420 6265 206c 6566 7420 756e  would be left un
-000061f0: 6368 616e 6765 642c 2032 220a 2020 2020  changed, 2".    
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2220 6669 6c65 7320 776f 756c 6420 6661  " files would fa
-00006220: 696c 2074 6f20 7265 666f 726d 6174 2e22  il to reformat."
-00006230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006240: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00006250: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00006260: 706f 7274 2e63 6865 636b 203d 2046 616c  port.check = Fal
-00006270: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
-00006280: 6570 6f72 742e 6469 6666 203d 2054 7275  eport.diff = Tru
-00006290: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-000062a0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062c0: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
-000062d0: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
-000062e0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-000062f0: 2020 2020 2020 2020 2020 2020 2232 2066              "2 f
-00006300: 696c 6573 2077 6f75 6c64 2062 6520 7265  iles would be re
-00006310: 666f 726d 6174 7465 642c 2033 2066 696c  formatted, 3 fil
-00006320: 6573 2077 6f75 6c64 2062 6520 6c65 6674  es would be left
-00006330: 2075 6e63 6861 6e67 6564 2c20 3222 0a20   unchanged, 2". 
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2022 2066 696c 6573 2077 6f75 6c64     " files would
-00006360: 2066 6169 6c20 746f 2072 6566 6f72 6d61   fail to reforma
-00006370: 742e 220a 2020 2020 2020 2020 2020 2020  t.".            
-00006380: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00006390: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-000063a0: 7374 5f72 6570 6f72 745f 7175 6965 7428  st_report_quiet(
-000063b0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-000063c0: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
-000063d0: 5265 706f 7274 2871 7569 6574 3d54 7275  Report(quiet=Tru
-000063e0: 6529 0a20 2020 2020 2020 206f 7574 5f6c  e).        out_l
-000063f0: 696e 6573 203d 205b 5d0a 2020 2020 2020  ines = [].      
-00006400: 2020 6572 725f 6c69 6e65 7320 3d20 5b5d    err_lines = []
-00006410: 0a0a 2020 2020 2020 2020 6465 6620 6f75  ..        def ou
-00006420: 7428 6d73 673a 2073 7472 2c20 2a2a 6b77  t(msg: str, **kw
-00006430: 6172 6773 3a20 416e 7929 202d 3e20 4e6f  args: Any) -> No
-00006440: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006450: 6f75 745f 6c69 6e65 732e 6170 7065 6e64  out_lines.append
-00006460: 286d 7367 290a 0a20 2020 2020 2020 2064  (msg)..        d
-00006470: 6566 2065 7272 286d 7367 3a20 7374 722c  ef err(msg: str,
-00006480: 202a 2a6b 7761 7267 733a 2041 6e79 2920   **kwargs: Any) 
-00006490: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000064a0: 2020 2020 2065 7272 5f6c 696e 6573 2e61       err_lines.a
-000064b0: 7070 656e 6428 6d73 6729 0a0a 2020 2020  ppend(msg)..    
-000064c0: 2020 2020 7769 7468 2070 6174 6368 2822      with patch("
-000064d0: 7079 696e 6b2e 6f75 7470 7574 2e5f 6f75  pyink.output._ou
-000064e0: 7422 2c20 6f75 7429 2c20 7061 7463 6828  t", out), patch(
-000064f0: 2270 7969 6e6b 2e6f 7574 7075 742e 5f65  "pyink.output._e
-00006500: 7272 222c 2065 7272 293a 0a20 2020 2020  rr", err):.     
-00006510: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
-00006520: 6e65 2850 6174 6828 2266 3122 292c 2070  ne(Path("f1"), p
-00006530: 7969 6e6b 2e43 6861 6e67 6564 2e4e 4f29  yink.Changed.NO)
-00006540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006550: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00006560: 6e28 6f75 745f 6c69 6e65 7329 2c20 3029  n(out_lines), 0)
-00006570: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006580: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00006590: 6e28 6572 725f 6c69 6e65 7329 2c20 3029  n(err_lines), 0)
-000065a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000065b0: 662e 6173 7365 7274 4571 7561 6c28 756e  f.assertEqual(un
-000065c0: 7374 796c 6528 7374 7228 7265 706f 7274  style(str(report
-000065d0: 2929 2c20 2231 2066 696c 6520 6c65 6674  )), "1 file left
-000065e0: 2075 6e63 6861 6e67 6564 2e22 290a 2020   unchanged.").  
-000065f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006600: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-00006610: 742e 7265 7475 726e 5f63 6f64 652c 2030  t.return_code, 0
-00006620: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00006630: 706f 7274 2e64 6f6e 6528 5061 7468 2822  port.done(Path("
-00006640: 6632 2229 2c20 7079 696e 6b2e 4368 616e  f2"), pyink.Chan
-00006650: 6765 642e 5945 5329 0a20 2020 2020 2020  ged.YES).       
-00006660: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006670: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
-00006680: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
-00006690: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000066a0: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
-000066b0: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
-000066c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000066d0: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
-000066e0: 2020 2020 2020 2075 6e73 7479 6c65 2873         unstyle(s
-000066f0: 7472 2872 6570 6f72 7429 292c 2022 3120  tr(report)), "1 
-00006700: 6669 6c65 2072 6566 6f72 6d61 7474 6564  file reformatted
-00006710: 2c20 3120 6669 6c65 206c 6566 7420 756e  , 1 file left un
-00006720: 6368 616e 6765 642e 220a 2020 2020 2020  changed.".      
-00006730: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006740: 2020 2020 7265 706f 7274 2e64 6f6e 6528      report.done(
-00006750: 5061 7468 2822 6633 2229 2c20 7079 696e  Path("f3"), pyin
-00006760: 6b2e 4368 616e 6765 642e 4341 4348 4544  k.Changed.CACHED
-00006770: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006780: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00006790: 656e 286f 7574 5f6c 696e 6573 292c 2030  en(out_lines), 0
-000067a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000067b0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-000067c0: 656e 2865 7272 5f6c 696e 6573 292c 2030  en(err_lines), 0
-000067d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000067e0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
-00006810: 7274 2929 2c20 2231 2066 696c 6520 7265  rt)), "1 file re
-00006820: 666f 726d 6174 7465 642c 2032 2066 696c  formatted, 2 fil
-00006830: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
-00006840: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
-00006850: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006860: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
-00006870: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
-00006880: 652c 2030 290a 2020 2020 2020 2020 2020  e, 0).          
-00006890: 2020 7265 706f 7274 2e63 6865 636b 203d    report.check =
-000068a0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-000068b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000068c0: 616c 2872 6570 6f72 742e 7265 7475 726e  al(report.return
-000068d0: 5f63 6f64 652c 2031 290a 2020 2020 2020  _code, 1).      
-000068e0: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
-000068f0: 636b 203d 2046 616c 7365 0a20 2020 2020  ck = False.     
-00006900: 2020 2020 2020 2072 6570 6f72 742e 6661         report.fa
-00006910: 696c 6564 2850 6174 6828 2265 3122 292c  iled(Path("e1"),
-00006920: 2022 626f 6f6d 2229 0a20 2020 2020 2020   "boom").       
-00006930: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006940: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
-00006950: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
-00006960: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006970: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
-00006980: 6e65 7329 2c20 3129 0a20 2020 2020 2020  nes), 1).       
-00006990: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000069a0: 4571 7561 6c28 6572 725f 6c69 6e65 735b  Equal(err_lines[
-000069b0: 2d31 5d2c 2022 6572 726f 723a 2063 616e  -1], "error: can
-000069c0: 6e6f 7420 666f 726d 6174 2065 313a 2062  not format e1: b
-000069d0: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
-000069e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000069f0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00006a00: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
-00006a10: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
-00006a20: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2231 2066 696c 6520 7265 666f 726d 6174  "1 file reformat
-00006a50: 7465 642c 2032 2066 696c 6573 206c 6566  ted, 2 files lef
-00006a60: 7420 756e 6368 616e 6765 642c 2031 2066  t unchanged, 1 f
-00006a70: 696c 6520 6661 696c 6564 2074 6f22 0a20  ile failed to". 
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2022 2072 6566 6f72 6d61 742e 220a     " reformat.".
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-00006ac0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006ad0: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
-00006ae0: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
-00006af0: 2c20 3132 3329 0a20 2020 2020 2020 2020  , 123).         
-00006b00: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
-00006b10: 6174 6828 2266 3322 292c 2070 7969 6e6b  ath("f3"), pyink
-00006b20: 2e43 6861 6e67 6564 2e59 4553 290a 2020  .Changed.YES).  
-00006b30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006b40: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
-00006b50: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
-00006b60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006b70: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
-00006b80: 7272 5f6c 696e 6573 292c 2031 290a 2020  rr_lines), 1).  
-00006b90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006ba0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00006bb0: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00006bc0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00006bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006be0: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00006bf0: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00006c00: 2072 6566 6f72 6d61 7474 6564 2c20 3220   reformatted, 2 
-00006c10: 6669 6c65 7320 6c65 6674 2075 6e63 6861  files left uncha
-00006c20: 6e67 6564 2c20 3120 6669 6c65 2066 6169  nged, 1 file fai
-00006c30: 6c65 6420 746f 220a 2020 2020 2020 2020  led to".        
-00006c40: 2020 2020 2020 2020 2020 2020 2220 7265              " re
-00006c50: 666f 726d 6174 2e22 0a20 2020 2020 2020  format.".       
-00006c60: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00006c70: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006c80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00006c90: 7445 7175 616c 2872 6570 6f72 742e 7265  tEqual(report.re
-00006ca0: 7475 726e 5f63 6f64 652c 2031 3233 290a  turn_code, 123).
-00006cb0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00006cc0: 7274 2e66 6169 6c65 6428 5061 7468 2822  rt.failed(Path("
-00006cd0: 6532 2229 2c20 2262 6f6f 6d22 290a 2020  e2"), "boom").  
-00006ce0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006cf0: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
-00006d00: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
-00006d10: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006d20: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
-00006d30: 7272 5f6c 696e 6573 292c 2032 290a 2020  rr_lines), 2).  
-00006d40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00006d50: 7373 6572 7445 7175 616c 2865 7272 5f6c  ssertEqual(err_l
-00006d60: 696e 6573 5b2d 315d 2c20 2265 7272 6f72  ines[-1], "error
-00006d70: 3a20 6361 6e6e 6f74 2066 6f72 6d61 7420  : cannot format 
-00006d80: 6532 3a20 626f 6f6d 2229 0a20 2020 2020  e2: boom").     
-00006d90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00006da0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00006db0: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
-00006dc0: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006df0: 2020 2020 2022 3220 6669 6c65 7320 7265       "2 files re
-00006e00: 666f 726d 6174 7465 642c 2032 2066 696c  formatted, 2 fil
-00006e10: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
-00006e20: 642c 2032 2066 696c 6573 2066 6169 6c65  d, 2 files faile
-00006e30: 6420 746f 220a 2020 2020 2020 2020 2020  d to".          
-00006e40: 2020 2020 2020 2020 2020 2220 7265 666f            " refo
-00006e50: 726d 6174 2e22 0a20 2020 2020 2020 2020  rmat.".         
-00006e60: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00006e70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006e80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00006e90: 7175 616c 2872 6570 6f72 742e 7265 7475  qual(report.retu
-00006ea0: 726e 5f63 6f64 652c 2031 3233 290a 2020  rn_code, 123).  
-00006eb0: 2020 2020 2020 2020 2020 7265 706f 7274            report
-00006ec0: 2e70 6174 685f 6967 6e6f 7265 6428 5061  .path_ignored(Pa
-00006ed0: 7468 2822 7761 7422 292c 2022 6e6f 206d  th("wat"), "no m
-00006ee0: 6174 6368 2229 0a20 2020 2020 2020 2020  atch").         
-00006ef0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00006f00: 7561 6c28 6c65 6e28 6f75 745f 6c69 6e65  ual(len(out_line
-00006f10: 7329 2c20 3029 0a20 2020 2020 2020 2020  s), 0).         
-00006f20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00006f30: 7561 6c28 6c65 6e28 6572 725f 6c69 6e65  ual(len(err_line
-00006f40: 7329 2c20 3229 0a20 2020 2020 2020 2020  s), 2).         
-00006f50: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00006f60: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
-00006f70: 2020 2020 2075 6e73 7479 6c65 2873 7472       unstyle(str
-00006f80: 2872 6570 6f72 7429 292c 0a20 2020 2020  (report)),.     
-00006f90: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2022 3220 6669 6c65 7320 7265 666f 726d   "2 files reform
-00006fc0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
-00006fd0: 6566 7420 756e 6368 616e 6765 642c 2032  eft unchanged, 2
-00006fe0: 2066 696c 6573 2066 6169 6c65 6420 746f   files failed to
-00006ff0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00007000: 2020 2020 2020 2220 7265 666f 726d 6174        " reformat
-00007010: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-00007020: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00007030: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00007040: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00007050: 2872 6570 6f72 742e 7265 7475 726e 5f63  (report.return_c
-00007060: 6f64 652c 2031 3233 290a 2020 2020 2020  ode, 123).      
-00007070: 2020 2020 2020 7265 706f 7274 2e64 6f6e        report.don
-00007080: 6528 5061 7468 2822 6634 2229 2c20 7079  e(Path("f4"), py
-00007090: 696e 6b2e 4368 616e 6765 642e 4e4f 290a  ink.Changed.NO).
-000070a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000070b0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-000070c0: 286f 7574 5f6c 696e 6573 292c 2030 290a  (out_lines), 0).
-000070d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000070e0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-000070f0: 2865 7272 5f6c 696e 6573 292c 2032 290a  (err_lines), 2).
-00007100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007110: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-00007120: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00007130: 7374 796c 6528 7374 7228 7265 706f 7274  style(str(report
-00007140: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00007150: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00007160: 2020 2020 2020 2020 2020 2232 2066 696c            "2 fil
-00007170: 6573 2072 6566 6f72 6d61 7474 6564 2c20  es reformatted, 
-00007180: 3320 6669 6c65 7320 6c65 6674 2075 6e63  3 files left unc
-00007190: 6861 6e67 6564 2c20 3220 6669 6c65 7320  hanged, 2 files 
-000071a0: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000071c0: 2072 6566 6f72 6d61 742e 220a 2020 2020   reformat.".    
-000071d0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000071e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000071f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00007200: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
-00007210: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
-00007220: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
-00007230: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
-00007240: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00007250: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00007260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007270: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
-00007280: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
-00007290: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-000072a0: 2020 2020 2020 2020 2020 2020 2022 3220               "2 
-000072b0: 6669 6c65 7320 776f 756c 6420 6265 2072  files would be r
-000072c0: 6566 6f72 6d61 7474 6564 2c20 3320 6669  eformatted, 3 fi
-000072d0: 6c65 7320 776f 756c 6420 6265 206c 6566  les would be lef
-000072e0: 7420 756e 6368 616e 6765 642c 2032 220a  t unchanged, 2".
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 2220 6669 6c65 7320 776f 756c      " files woul
-00007310: 6420 6661 696c 2074 6f20 7265 666f 726d  d fail to reform
-00007320: 6174 2e22 0a20 2020 2020 2020 2020 2020  at.".           
-00007330: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00007340: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00007350: 2020 7265 706f 7274 2e63 6865 636b 203d    report.check =
-00007360: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00007370: 2020 2072 6570 6f72 742e 6469 6666 203d     report.diff =
-00007380: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00007390: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000073a0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-000073b0: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
-000073c0: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
-000073d0: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073f0: 2232 2066 696c 6573 2077 6f75 6c64 2062  "2 files would b
-00007400: 6520 7265 666f 726d 6174 7465 642c 2033  e reformatted, 3
-00007410: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
-00007420: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
-00007430: 3222 0a20 2020 2020 2020 2020 2020 2020  2".             
-00007440: 2020 2020 2020 2022 2066 696c 6573 2077         " files w
-00007450: 6f75 6c64 2066 6169 6c20 746f 2072 6566  ould fail to ref
-00007460: 6f72 6d61 742e 220a 2020 2020 2020 2020  ormat.".        
-00007470: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00007480: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00007490: 6620 7465 7374 5f72 6570 6f72 745f 6e6f  f test_report_no
-000074a0: 726d 616c 2873 656c 6629 202d 3e20 4e6f  rmal(self) -> No
-000074b0: 6e65 3a0a 2020 2020 2020 2020 7265 706f  ne:.        repo
-000074c0: 7274 203d 2070 7969 6e6b 2e52 6570 6f72  rt = pyink.Repor
-000074d0: 7428 290a 2020 2020 2020 2020 6f75 745f  t().        out_
-000074e0: 6c69 6e65 7320 3d20 5b5d 0a20 2020 2020  lines = [].     
-000074f0: 2020 2065 7272 5f6c 696e 6573 203d 205b     err_lines = [
-00007500: 5d0a 0a20 2020 2020 2020 2064 6566 206f  ]..        def o
-00007510: 7574 286d 7367 3a20 7374 722c 202a 2a6b  ut(msg: str, **k
-00007520: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
-00007530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007540: 206f 7574 5f6c 696e 6573 2e61 7070 656e   out_lines.appen
-00007550: 6428 6d73 6729 0a0a 2020 2020 2020 2020  d(msg)..        
-00007560: 6465 6620 6572 7228 6d73 673a 2073 7472  def err(msg: str
-00007570: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
-00007580: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00007590: 2020 2020 2020 6572 725f 6c69 6e65 732e        err_lines.
-000075a0: 6170 7065 6e64 286d 7367 290a 0a20 2020  append(msg)..   
-000075b0: 2020 2020 2077 6974 6820 7061 7463 6828       with patch(
-000075c0: 2270 7969 6e6b 2e6f 7574 7075 742e 5f6f  "pyink.output._o
-000075d0: 7574 222c 206f 7574 292c 2070 6174 6368  ut", out), patch
-000075e0: 2822 7079 696e 6b2e 6f75 7470 7574 2e5f  ("pyink.output._
-000075f0: 6572 7222 2c20 6572 7229 3a0a 2020 2020  err", err):.    
-00007600: 2020 2020 2020 2020 7265 706f 7274 2e64          report.d
-00007610: 6f6e 6528 5061 7468 2822 6631 2229 2c20  one(Path("f1"), 
-00007620: 7079 696e 6b2e 4368 616e 6765 642e 4e4f  pyink.Changed.NO
-00007630: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00007640: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00007650: 656e 286f 7574 5f6c 696e 6573 292c 2030  en(out_lines), 0
-00007660: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00007670: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00007680: 656e 2865 7272 5f6c 696e 6573 292c 2030  en(err_lines), 0
-00007690: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000076a0: 6c66 2e61 7373 6572 7445 7175 616c 2875  lf.assertEqual(u
-000076b0: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
-000076c0: 7429 292c 2022 3120 6669 6c65 206c 6566  t)), "1 file lef
-000076d0: 7420 756e 6368 616e 6765 642e 2229 0a20  t unchanged."). 
-000076e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000076f0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-00007700: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-00007710: 3029 0a20 2020 2020 2020 2020 2020 2072  0).            r
-00007720: 6570 6f72 742e 646f 6e65 2850 6174 6828  eport.done(Path(
-00007730: 2266 3222 292c 2070 7969 6e6b 2e43 6861  "f2"), pyink.Cha
-00007740: 6e67 6564 2e59 4553 290a 2020 2020 2020  nged.YES).      
-00007750: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00007760: 7445 7175 616c 286c 656e 286f 7574 5f6c  tEqual(len(out_l
-00007770: 696e 6573 292c 2031 290a 2020 2020 2020  ines), 1).      
-00007780: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00007790: 7445 7175 616c 286c 656e 2865 7272 5f6c  tEqual(len(err_l
-000077a0: 696e 6573 292c 2030 290a 2020 2020 2020  ines), 0).      
-000077b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000077c0: 7445 7175 616c 286f 7574 5f6c 696e 6573  tEqual(out_lines
-000077d0: 5b2d 315d 2c20 2272 6566 6f72 6d61 7474  [-1], "reformatt
-000077e0: 6564 2066 3222 290a 2020 2020 2020 2020  ed f2").        
-000077f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00007800: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00007810: 2020 2020 2020 756e 7374 796c 6528 7374        unstyle(st
-00007820: 7228 7265 706f 7274 2929 2c20 2231 2066  r(report)), "1 f
-00007830: 696c 6520 7265 666f 726d 6174 7465 642c  ile reformatted,
-00007840: 2031 2066 696c 6520 6c65 6674 2075 6e63   1 file left unc
-00007850: 6861 6e67 6564 2e22 0a20 2020 2020 2020  hanged.".       
-00007860: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007870: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
-00007880: 6174 6828 2266 3322 292c 2070 7969 6e6b  ath("f3"), pyink
-00007890: 2e43 6861 6e67 6564 2e43 4143 4845 4429  .Changed.CACHED)
-000078a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000078b0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-000078c0: 6e28 6f75 745f 6c69 6e65 7329 2c20 3129  n(out_lines), 1)
-000078d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000078e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-000078f0: 6e28 6572 725f 6c69 6e65 7329 2c20 3029  n(err_lines), 0)
-00007900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007910: 662e 6173 7365 7274 4571 7561 6c28 6f75  f.assertEqual(ou
-00007920: 745f 6c69 6e65 735b 2d31 5d2c 2022 7265  t_lines[-1], "re
-00007930: 666f 726d 6174 7465 6420 6632 2229 0a20  formatted f2"). 
-00007940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007950: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00007960: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
-00007970: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
-00007980: 292c 2022 3120 6669 6c65 2072 6566 6f72  ), "1 file refor
-00007990: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
-000079a0: 6c65 6674 2075 6e63 6861 6e67 6564 2e22  left unchanged."
-000079b0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000079c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000079d0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-000079e0: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-000079f0: 3029 0a20 2020 2020 2020 2020 2020 2072  0).            r
-00007a00: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
-00007a10: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
-00007a20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00007a30: 7265 706f 7274 2e72 6574 7572 6e5f 636f  report.return_co
-00007a40: 6465 2c20 3129 0a20 2020 2020 2020 2020  de, 1).         
-00007a50: 2020 2072 6570 6f72 742e 6368 6563 6b20     report.check 
-00007a60: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00007a70: 2020 2020 7265 706f 7274 2e66 6169 6c65      report.faile
-00007a80: 6428 5061 7468 2822 6531 2229 2c20 2262  d(Path("e1"), "b
-00007a90: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
-00007aa0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007ab0: 616c 286c 656e 286f 7574 5f6c 696e 6573  al(len(out_lines
-00007ac0: 292c 2031 290a 2020 2020 2020 2020 2020  ), 1).          
-00007ad0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007ae0: 616c 286c 656e 2865 7272 5f6c 696e 6573  al(len(err_lines
-00007af0: 292c 2031 290a 2020 2020 2020 2020 2020  ), 1).          
-00007b00: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007b10: 616c 2865 7272 5f6c 696e 6573 5b2d 315d  al(err_lines[-1]
-00007b20: 2c20 2265 7272 6f72 3a20 6361 6e6e 6f74  , "error: cannot
-00007b30: 2066 6f72 6d61 7420 6531 3a20 626f 6f6d   format e1: boom
-00007b40: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00007b50: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
-00007b80: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
-00007b90: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00007ba0: 2020 2020 2020 2020 2020 2020 2022 3120               "1 
-00007bb0: 6669 6c65 2072 6566 6f72 6d61 7474 6564  file reformatted
-00007bc0: 2c20 3220 6669 6c65 7320 6c65 6674 2075  , 2 files left u
-00007bd0: 6e63 6861 6e67 6564 2c20 3120 6669 6c65  nchanged, 1 file
-00007be0: 2066 6169 6c65 6420 746f 220a 2020 2020   failed to".    
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2220 7265 666f 726d 6174 2e22 0a20 2020  " reformat.".   
-00007c10: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00007c20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007c30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00007c40: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
-00007c50: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
-00007c60: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
-00007c70: 7265 706f 7274 2e64 6f6e 6528 5061 7468  report.done(Path
-00007c80: 2822 6633 2229 2c20 7079 696e 6b2e 4368  ("f3"), pyink.Ch
-00007c90: 616e 6765 642e 5945 5329 0a20 2020 2020  anged.YES).     
-00007ca0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007cb0: 7274 4571 7561 6c28 6c65 6e28 6f75 745f  rtEqual(len(out_
-00007cc0: 6c69 6e65 7329 2c20 3229 0a20 2020 2020  lines), 2).     
-00007cd0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007ce0: 7274 4571 7561 6c28 6c65 6e28 6572 725f  rtEqual(len(err_
-00007cf0: 6c69 6e65 7329 2c20 3129 0a20 2020 2020  lines), 1).     
-00007d00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007d10: 7274 4571 7561 6c28 6f75 745f 6c69 6e65  rtEqual(out_line
-00007d20: 735b 2d31 5d2c 2022 7265 666f 726d 6174  s[-1], "reformat
-00007d30: 7465 6420 6633 2229 0a20 2020 2020 2020  ted f3").       
-00007d40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00007d50: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
-00007d60: 2020 2020 2020 2075 6e73 7479 6c65 2873         unstyle(s
-00007d70: 7472 2872 6570 6f72 7429 292c 0a20 2020  tr(report)),.   
-00007d80: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
-00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
-00007db0: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
-00007dc0: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
-00007dd0: 2031 2066 696c 6520 6661 696c 6564 2074   1 file failed t
-00007de0: 6f22 0a20 2020 2020 2020 2020 2020 2020  o".             
-00007df0: 2020 2020 2020 2022 2072 6566 6f72 6d61         " reforma
-00007e00: 742e 220a 2020 2020 2020 2020 2020 2020  t.".            
-00007e10: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00007e20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00007e30: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00007e40: 6c28 7265 706f 7274 2e72 6574 7572 6e5f  l(report.return_
-00007e50: 636f 6465 2c20 3132 3329 0a20 2020 2020  code, 123).     
-00007e60: 2020 2020 2020 2072 6570 6f72 742e 6661         report.fa
-00007e70: 696c 6564 2850 6174 6828 2265 3222 292c  iled(Path("e2"),
-00007e80: 2022 626f 6f6d 2229 0a20 2020 2020 2020   "boom").       
-00007e90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00007ea0: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
-00007eb0: 6e65 7329 2c20 3229 0a20 2020 2020 2020  nes), 2).       
-00007ec0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00007ed0: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
-00007ee0: 6e65 7329 2c20 3229 0a20 2020 2020 2020  nes), 2).       
-00007ef0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00007f00: 4571 7561 6c28 6572 725f 6c69 6e65 735b  Equal(err_lines[
-00007f10: 2d31 5d2c 2022 6572 726f 723a 2063 616e  -1], "error: can
-00007f20: 6e6f 7420 666f 726d 6174 2065 323a 2062  not format e2: b
-00007f30: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
-00007f40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007f50: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00007f60: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
-00007f70: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
-00007f80: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
-00007fb0: 7474 6564 2c20 3220 6669 6c65 7320 6c65  tted, 2 files le
-00007fc0: 6674 2075 6e63 6861 6e67 6564 2c20 3220  ft unchanged, 2 
-00007fd0: 6669 6c65 7320 6661 696c 6564 2074 6f22  files failed to"
-00007fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ff0: 2020 2020 2022 2072 6566 6f72 6d61 742e       " reformat.
-00008000: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00008010: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00008020: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-00008030: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00008040: 7265 706f 7274 2e72 6574 7572 6e5f 636f  report.return_co
-00008050: 6465 2c20 3132 3329 0a20 2020 2020 2020  de, 123).       
-00008060: 2020 2020 2072 6570 6f72 742e 7061 7468       report.path
-00008070: 5f69 676e 6f72 6564 2850 6174 6828 2277  _ignored(Path("w
-00008080: 6174 2229 2c20 226e 6f20 6d61 7463 6822  at"), "no match"
-00008090: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000080a0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-000080b0: 656e 286f 7574 5f6c 696e 6573 292c 2032  en(out_lines), 2
-000080c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000080d0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-000080e0: 656e 2865 7272 5f6c 696e 6573 292c 2032  en(err_lines), 2
-000080f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00008100: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
-00008130: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
-00008140: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-00008150: 2020 2020 2020 2020 2020 2020 2232 2066              "2 f
-00008160: 696c 6573 2072 6566 6f72 6d61 7474 6564  iles reformatted
-00008170: 2c20 3220 6669 6c65 7320 6c65 6674 2075  , 2 files left u
-00008180: 6e63 6861 6e67 6564 2c20 3220 6669 6c65  nchanged, 2 file
-00008190: 7320 6661 696c 6564 2074 6f22 0a20 2020  s failed to".   
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2022 2072 6566 6f72 6d61 742e 220a 2020   " reformat.".  
-000081c0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000081d0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000081e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000081f0: 6173 7365 7274 4571 7561 6c28 7265 706f  assertEqual(repo
-00008200: 7274 2e72 6574 7572 6e5f 636f 6465 2c20  rt.return_code, 
-00008210: 3132 3329 0a20 2020 2020 2020 2020 2020  123).           
-00008220: 2072 6570 6f72 742e 646f 6e65 2850 6174   report.done(Pat
-00008230: 6828 2266 3422 292c 2070 7969 6e6b 2e43  h("f4"), pyink.C
-00008240: 6861 6e67 6564 2e4e 4f29 0a20 2020 2020  hanged.NO).     
-00008250: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00008260: 7274 4571 7561 6c28 6c65 6e28 6f75 745f  rtEqual(len(out_
-00008270: 6c69 6e65 7329 2c20 3229 0a20 2020 2020  lines), 2).     
-00008280: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00008290: 7274 4571 7561 6c28 6c65 6e28 6572 725f  rtEqual(len(err_
-000082a0: 6c69 6e65 7329 2c20 3229 0a20 2020 2020  lines), 2).     
-000082b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000082c0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-000082d0: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
-000082e0: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
-000082f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00008300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008310: 2020 2020 2022 3220 6669 6c65 7320 7265       "2 files re
-00008320: 666f 726d 6174 7465 642c 2033 2066 696c  formatted, 3 fil
-00008330: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
-00008340: 642c 2032 2066 696c 6573 2066 6169 6c65  d, 2 files faile
-00008350: 6420 746f 220a 2020 2020 2020 2020 2020  d to".          
-00008360: 2020 2020 2020 2020 2020 2220 7265 666f            " refo
-00008370: 726d 6174 2e22 0a20 2020 2020 2020 2020  rmat.".         
-00008380: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00008390: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000083a0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000083b0: 7175 616c 2872 6570 6f72 742e 7265 7475  qual(report.retu
-000083c0: 726e 5f63 6f64 652c 2031 3233 290a 2020  rn_code, 123).  
-000083d0: 2020 2020 2020 2020 2020 7265 706f 7274            report
-000083e0: 2e63 6865 636b 203d 2054 7275 650a 2020  .check = True.  
-000083f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00008400: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00008410: 2020 2020 2020 2020 2020 2020 756e 7374              unst
-00008420: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
-00008430: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008440: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00008450: 2020 2020 2020 2020 2232 2066 696c 6573          "2 files
-00008460: 2077 6f75 6c64 2062 6520 7265 666f 726d   would be reform
-00008470: 6174 7465 642c 2033 2066 696c 6573 2077  atted, 3 files w
-00008480: 6f75 6c64 2062 6520 6c65 6674 2075 6e63  ould be left unc
-00008490: 6861 6e67 6564 2c20 3222 0a20 2020 2020  hanged, 2".     
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000084b0: 2066 696c 6573 2077 6f75 6c64 2066 6169   files would fai
-000084c0: 6c20 746f 2072 6566 6f72 6d61 742e 220a  l to reformat.".
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-000084f0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00008500: 6f72 742e 6368 6563 6b20 3d20 4661 6c73  ort.check = Fals
-00008510: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
-00008520: 706f 7274 2e64 6966 6620 3d20 5472 7565  port.diff = True
-00008530: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008540: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
-00008550: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00008560: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
-00008570: 7429 292c 0a20 2020 2020 2020 2020 2020  t)),.           
-00008580: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-00008590: 2020 2020 2020 2020 2020 2022 3220 6669             "2 fi
-000085a0: 6c65 7320 776f 756c 6420 6265 2072 6566  les would be ref
-000085b0: 6f72 6d61 7474 6564 2c20 3320 6669 6c65  ormatted, 3 file
-000085c0: 7320 776f 756c 6420 6265 206c 6566 7420  s would be left 
-000085d0: 756e 6368 616e 6765 642c 2032 220a 2020  unchanged, 2".  
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2220 6669 6c65 7320 776f 756c 6420    " files would 
-00008600: 6661 696c 2074 6f20 7265 666f 726d 6174  fail to reformat
-00008610: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-00008620: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00008630: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
-00008640: 745f 6c69 6232 746f 335f 7061 7273 6528  t_lib2to3_parse(
-00008650: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00008660: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00008670: 2e61 7373 6572 7452 6169 7365 7328 7079  .assertRaises(py
-00008680: 696e 6b2e 496e 7661 6c69 6449 6e70 7574  ink.InvalidInput
-00008690: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-000086a0: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
-000086b0: 7365 2822 696e 7661 6c69 6420 7379 6e74  se("invalid synt
-000086c0: 6178 2229 0a0a 2020 2020 2020 2020 7374  ax")..        st
-000086d0: 7261 6464 6c69 6e67 203d 2022 7820 2b20  raddling = "x + 
-000086e0: 7922 0a20 2020 2020 2020 2070 7969 6e6b  y".        pyink
-000086f0: 2e6c 6962 3274 6f33 5f70 6172 7365 2873  .lib2to3_parse(s
-00008700: 7472 6164 646c 696e 6729 0a20 2020 2020  traddling).     
-00008710: 2020 2070 7969 6e6b 2e6c 6962 3274 6f33     pyink.lib2to3
-00008720: 5f70 6172 7365 2873 7472 6164 646c 696e  _parse(straddlin
-00008730: 672c 207b 5461 7267 6574 5665 7273 696f  g, {TargetVersio
-00008740: 6e2e 5059 3336 7d29 0a0a 2020 2020 2020  n.PY36})..      
-00008750: 2020 7079 325f 6f6e 6c79 203d 2022 7072    py2_only = "pr
-00008760: 696e 7420 7822 0a20 2020 2020 2020 2077  int x".        w
-00008770: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-00008780: 6169 7365 7328 7079 696e 6b2e 496e 7661  aises(pyink.Inva
-00008790: 6c69 6449 6e70 7574 293a 0a20 2020 2020  lidInput):.     
-000087a0: 2020 2020 2020 2070 7969 6e6b 2e6c 6962         pyink.lib
-000087b0: 3274 6f33 5f70 6172 7365 2870 7932 5f6f  2to3_parse(py2_o
-000087c0: 6e6c 792c 207b 5461 7267 6574 5665 7273  nly, {TargetVers
-000087d0: 696f 6e2e 5059 3336 7d29 0a0a 2020 2020  ion.PY36})..    
-000087e0: 2020 2020 7079 335f 6f6e 6c79 203d 2022      py3_only = "
-000087f0: 6578 6563 2878 2c20 656e 643d 7929 220a  exec(x, end=y)".
-00008800: 2020 2020 2020 2020 7079 696e 6b2e 6c69          pyink.li
-00008810: 6232 746f 335f 7061 7273 6528 7079 335f  b2to3_parse(py3_
-00008820: 6f6e 6c79 290a 2020 2020 2020 2020 7079  only).        py
-00008830: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
-00008840: 6528 7079 335f 6f6e 6c79 2c20 7b54 6172  e(py3_only, {Tar
-00008850: 6765 7456 6572 7369 6f6e 2e50 5933 367d  getVersion.PY36}
-00008860: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00008870: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00008880: 645f 6465 636f 7261 746f 7228 7365 6c66  d_decorator(self
-00008890: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000088a0: 2020 2023 2054 6573 7420 7468 6520 6665     # Test the fe
-000088b0: 6174 7572 6520 6465 7465 6374 696f 6e20  ature detection 
-000088c0: 6f66 206e 6577 2064 6563 6f72 6174 6f72  of new decorator
-000088d0: 2073 796e 7461 780a 2020 2020 2020 2020   syntax.        
-000088e0: 2320 7369 6e63 6520 7468 6973 206d 616b  # since this mak
-000088f0: 6573 2073 6f6d 6520 7465 7374 2063 6173  es some test cas
-00008900: 6573 206f 6620 7465 7374 5f67 6574 5f66  es of test_get_f
-00008910: 6561 7475 7265 735f 7573 6564 2829 0a20  eatures_used(). 
-00008920: 2020 2020 2020 2023 2066 6169 6c73 2069         # fails i
-00008930: 6620 6974 2066 6169 6c73 2c20 7468 6973  f it fails, this
-00008940: 2069 7320 7465 7374 6564 2066 6972 7374   is tested first
-00008950: 2073 6f20 7468 6174 2061 2075 7365 6675   so that a usefu
-00008960: 6c20 6361 7365 0a20 2020 2020 2020 2023  l case.        #
-00008970: 2069 7320 6964 656e 7469 6669 6564 0a20   is identified. 
-00008980: 2020 2020 2020 2073 696d 706c 6573 2c20         simples, 
-00008990: 7265 6c61 7865 6420 3d20 7265 6164 5f64  relaxed = read_d
-000089a0: 6174 6128 226d 6973 6365 6c6c 616e 656f  ata("miscellaneo
-000089b0: 7573 222c 2022 6465 636f 7261 746f 7273  us", "decorators
-000089c0: 2229 0a20 2020 2020 2020 2023 2073 6b69  ").        # ski
-000089d0: 7020 6578 706c 616e 6174 696f 6e20 636f  p explanation co
-000089e0: 6d6d 656e 7473 2061 7420 7468 6520 746f  mments at the to
-000089f0: 7020 6f66 2074 6865 2066 696c 650a 2020  p of the file.  
-00008a00: 2020 2020 2020 666f 7220 7369 6d70 6c65        for simple
-00008a10: 5f74 6573 7420 696e 2073 696d 706c 6573  _test in simples
-00008a20: 2e73 706c 6974 2822 2323 2229 5b31 3a5d  .split("##")[1:]
-00008a30: 3a0a 2020 2020 2020 2020 2020 2020 6e6f  :.            no
-00008a40: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
-00008a50: 6f33 5f70 6172 7365 2873 696d 706c 655f  o3_parse(simple_
-00008a60: 7465 7374 290a 2020 2020 2020 2020 2020  test).          
-00008a70: 2020 6465 636f 7261 746f 7220 3d20 7374    decorator = st
-00008a80: 7228 6e6f 6465 2e63 6869 6c64 7265 6e5b  r(node.children[
-00008a90: 305d 2e63 6869 6c64 7265 6e5b 305d 292e  0].children[0]).
-00008aa0: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
-00008ab0: 2020 2020 7365 6c66 2e61 7373 6572 744e      self.assertN
-00008ac0: 6f74 496e 280a 2020 2020 2020 2020 2020  otIn(.          
-00008ad0: 2020 2020 2020 4665 6174 7572 652e 5245        Feature.RE
-00008ae0: 4c41 5845 445f 4445 434f 5241 544f 5253  LAXED_DECORATORS
-00008af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008b00: 2020 7079 696e 6b2e 6765 745f 6665 6174    pyink.get_feat
-00008b10: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
-00008b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b30: 206d 7367 3d28 0a20 2020 2020 2020 2020   msg=(.         
-00008b40: 2020 2020 2020 2020 2020 2066 2264 6563             f"dec
-00008b50: 6f72 6174 6f72 2027 7b64 6563 6f72 6174  orator '{decorat
-00008b60: 6f72 7d27 2066 6f6c 6c6f 7773 2070 7974  or}' follows pyt
-00008b70: 686f 6e3c 3d33 2e38 2073 796e 7461 7822  hon<=3.8 syntax"
-00008b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b90: 2020 2020 2022 6275 7420 6973 2064 6574       "but is det
-00008ba0: 6563 7465 6420 6173 2033 2e39 2b22 0a20  ected as 3.9+". 
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bc0: 2020 2023 2066 2254 6865 2066 756c 6c20     # f"The full 
-00008bd0: 6e6f 6465 2069 735c 6e7b 6e6f 6465 2172  node is\n{node!r
-00008be0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00008bf0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00008c00: 2020 290a 2020 2020 2020 2020 2320 736b    ).        # sk
-00008c10: 6970 2074 6865 2027 2320 6f75 7470 7574  ip the '# output
-00008c20: 2720 636f 6d6d 656e 7420 6174 2074 6865  ' comment at the
-00008c30: 2074 6f70 206f 6620 7468 6520 6f75 7470   top of the outp
-00008c40: 7574 2070 6172 740a 2020 2020 2020 2020  ut part.        
-00008c50: 666f 7220 7265 6c61 7865 645f 7465 7374  for relaxed_test
-00008c60: 2069 6e20 7265 6c61 7865 642e 7370 6c69   in relaxed.spli
-00008c70: 7428 2223 2322 295b 313a 5d3a 0a20 2020  t("##")[1:]:.   
-00008c80: 2020 2020 2020 2020 206e 6f64 6520 3d20           node = 
-00008c90: 7079 696e 6b2e 6c69 6232 746f 335f 7061  pyink.lib2to3_pa
-00008ca0: 7273 6528 7265 6c61 7865 645f 7465 7374  rse(relaxed_test
-00008cb0: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-00008cc0: 636f 7261 746f 7220 3d20 7374 7228 6e6f  corator = str(no
-00008cd0: 6465 2e63 6869 6c64 7265 6e5b 305d 2e63  de.children[0].c
-00008ce0: 6869 6c64 7265 6e5b 305d 292e 7374 7269  hildren[0]).stri
-00008cf0: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
-00008d00: 7365 6c66 2e61 7373 6572 7449 6e28 0a20  self.assertIn(. 
-00008d10: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-00008d20: 6561 7475 7265 2e52 454c 4158 4544 5f44  eature.RELAXED_D
-00008d30: 4543 4f52 4154 4f52 532c 0a20 2020 2020  ECORATORS,.     
-00008d40: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
-00008d50: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
-00008d60: 6564 286e 6f64 6529 2c0a 2020 2020 2020  ed(node),.      
-00008d70: 2020 2020 2020 2020 2020 6d73 673d 280a            msg=(.
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 6622 6465 636f 7261 746f 7220      f"decorator 
-00008da0: 277b 6465 636f 7261 746f 727d 2720 7573  '{decorator}' us
-00008db0: 6573 2070 7974 686f 6e33 2e39 2b20 7379  es python3.9+ sy
-00008dc0: 6e74 6178 220a 2020 2020 2020 2020 2020  ntax".          
-00008dd0: 2020 2020 2020 2020 2020 2262 7574 2069            "but i
-00008de0: 7320 6465 7465 6374 6564 2061 7320 7079  s detected as py
-00008df0: 7468 6f6e 3c3d 332e 3822 0a20 2020 2020  thon<=3.8".     
-00008e00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008e10: 2066 2254 6865 2066 756c 6c20 6e6f 6465   f"The full node
-00008e20: 2069 735c 6e7b 6e6f 6465 2172 7d22 0a20   is\n{node!r}". 
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008e40: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00008e50: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-00008e60: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
-00008e70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00008e80: 2020 2020 2020 206e 6f64 6520 3d20 7079         node = py
-00008e90: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
-00008ea0: 6528 2264 6566 2066 282a 2c20 6172 6729  e("def f(*, arg)
-00008eb0: 3a20 2e2e 2e5c 6e22 290a 2020 2020 2020  : ...\n").      
-00008ec0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00008ed0: 616c 2870 7969 6e6b 2e67 6574 5f66 6561  al(pyink.get_fea
-00008ee0: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
-00008ef0: 2c20 7365 7428 2929 0a20 2020 2020 2020  , set()).       
-00008f00: 206e 6f64 6520 3d20 7079 696e 6b2e 6c69   node = pyink.li
-00008f10: 6232 746f 335f 7061 7273 6528 2264 6566  b2to3_parse("def
-00008f20: 2066 282a 2c20 6172 672c 293a 202e 2e2e   f(*, arg,): ...
-00008f30: 5c6e 2229 0a20 2020 2020 2020 2073 656c  \n").        sel
-00008f40: 662e 6173 7365 7274 4571 7561 6c28 7079  f.assertEqual(py
-00008f50: 696e 6b2e 6765 745f 6665 6174 7572 6573  ink.get_features
-00008f60: 5f75 7365 6428 6e6f 6465 292c 207b 4665  _used(node), {Fe
-00008f70: 6174 7572 652e 5452 4149 4c49 4e47 5f43  ature.TRAILING_C
-00008f80: 4f4d 4d41 5f49 4e5f 4445 467d 290a 2020  OMMA_IN_DEF}).  
-00008f90: 2020 2020 2020 6e6f 6465 203d 2070 7969        node = pyi
-00008fa0: 6e6b 2e6c 6962 3274 6f33 5f70 6172 7365  nk.lib2to3_parse
-00008fb0: 2822 6628 2a61 7267 2c29 5c6e 2229 0a20  ("f(*arg,)\n"). 
-00008fc0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00008fd0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00008fe0: 2020 2020 2070 7969 6e6b 2e67 6574 5f66       pyink.get_f
-00008ff0: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
-00009000: 6529 2c20 7b46 6561 7475 7265 2e54 5241  e), {Feature.TRA
-00009010: 494c 494e 475f 434f 4d4d 415f 494e 5f43  ILING_COMMA_IN_C
-00009020: 414c 4c7d 0a20 2020 2020 2020 2029 0a20  ALL}.        ). 
-00009030: 2020 2020 2020 206e 6f64 6520 3d20 7079         node = py
-00009040: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
-00009050: 6528 2264 6566 2066 282a 2c20 6172 6729  e("def f(*, arg)
-00009060: 3a20 6627 7374 7269 6e67 275c 6e22 290a  : f'string'\n").
-00009070: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00009080: 6572 7445 7175 616c 2870 7969 6e6b 2e67  ertEqual(pyink.g
-00009090: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
-000090a0: 286e 6f64 6529 2c20 7b46 6561 7475 7265  (node), {Feature
-000090b0: 2e46 5f53 5452 494e 4753 7d29 0a20 2020  .F_STRINGS}).   
-000090c0: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
-000090d0: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
-000090e0: 2231 3233 5f34 3536 5c6e 2229 0a20 2020  "123_456\n").   
-000090f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009100: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
-00009110: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009120: 6465 292c 207b 4665 6174 7572 652e 4e55  de), {Feature.NU
-00009130: 4d45 5249 435f 554e 4445 5253 434f 5245  MERIC_UNDERSCORE
-00009140: 537d 290a 2020 2020 2020 2020 6e6f 6465  S}).        node
-00009150: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-00009160: 5f70 6172 7365 2822 3132 3334 3536 5c6e  _parse("123456\n
-00009170: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009180: 6173 7365 7274 4571 7561 6c28 7079 696e  assertEqual(pyin
-00009190: 6b2e 6765 745f 6665 6174 7572 6573 5f75  k.get_features_u
-000091a0: 7365 6428 6e6f 6465 292c 2073 6574 2829  sed(node), set()
-000091b0: 290a 2020 2020 2020 2020 736f 7572 6365  ).        source
-000091c0: 2c20 6578 7065 6374 6564 203d 2072 6561  , expected = rea
-000091d0: 645f 6461 7461 2822 7369 6d70 6c65 5f63  d_data("simple_c
-000091e0: 6173 6573 222c 2022 6675 6e63 7469 6f6e  ases", "function
-000091f0: 2229 0a20 2020 2020 2020 206e 6f64 6520  ").        node 
-00009200: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
-00009210: 7061 7273 6528 736f 7572 6365 290a 2020  parse(source).  
-00009220: 2020 2020 2020 6578 7065 6374 6564 5f66        expected_f
-00009230: 6561 7475 7265 7320 3d20 7b0a 2020 2020  eatures = {.    
-00009240: 2020 2020 2020 2020 4665 6174 7572 652e          Feature.
-00009250: 5452 4149 4c49 4e47 5f43 4f4d 4d41 5f49  TRAILING_COMMA_I
-00009260: 4e5f 4341 4c4c 2c0a 2020 2020 2020 2020  N_CALL,.        
-00009270: 2020 2020 4665 6174 7572 652e 5452 4149      Feature.TRAI
-00009280: 4c49 4e47 5f43 4f4d 4d41 5f49 4e5f 4445  LING_COMMA_IN_DE
-00009290: 462c 0a20 2020 2020 2020 2020 2020 2046  F,.            F
-000092a0: 6561 7475 7265 2e46 5f53 5452 494e 4753  eature.F_STRINGS
-000092b0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-000092c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000092d0: 7175 616c 2870 7969 6e6b 2e67 6574 5f66  qual(pyink.get_f
-000092e0: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
-000092f0: 6529 2c20 6578 7065 6374 6564 5f66 6561  e), expected_fea
-00009300: 7475 7265 7329 0a20 2020 2020 2020 206e  tures).        n
-00009310: 6f64 6520 3d20 7079 696e 6b2e 6c69 6232  ode = pyink.lib2
-00009320: 746f 335f 7061 7273 6528 6578 7065 6374  to3_parse(expect
-00009330: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
-00009340: 2e61 7373 6572 7445 7175 616c 2870 7969  .assertEqual(pyi
-00009350: 6e6b 2e67 6574 5f66 6561 7475 7265 735f  nk.get_features_
-00009360: 7573 6564 286e 6f64 6529 2c20 6578 7065  used(node), expe
-00009370: 6374 6564 5f66 6561 7475 7265 7329 0a20  cted_features). 
-00009380: 2020 2020 2020 2073 6f75 7263 652c 2065         source, e
-00009390: 7870 6563 7465 6420 3d20 7265 6164 5f64  xpected = read_d
-000093a0: 6174 6128 2273 696d 706c 655f 6361 7365  ata("simple_case
-000093b0: 7322 2c20 2265 7870 7265 7373 696f 6e22  s", "expression"
-000093c0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-000093d0: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
-000093e0: 6172 7365 2873 6f75 7263 6529 0a20 2020  arse(source).   
-000093f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009400: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
-00009410: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009420: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
-00009430: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
-00009440: 2e6c 6962 3274 6f33 5f70 6172 7365 2865  .lib2to3_parse(e
-00009450: 7870 6563 7465 6429 0a20 2020 2020 2020  xpected).       
-00009460: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00009470: 6c28 7079 696e 6b2e 6765 745f 6665 6174  l(pyink.get_feat
-00009480: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
-00009490: 2073 6574 2829 290a 2020 2020 2020 2020   set()).        
-000094a0: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
-000094b0: 3274 6f33 5f70 6172 7365 2822 6c61 6d62  2to3_parse("lamb
-000094c0: 6461 2061 2c20 2f2c 2062 3a20 2e2e 2e22  da a, /, b: ..."
-000094d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000094e0: 7373 6572 7445 7175 616c 2870 7969 6e6b  ssertEqual(pyink
-000094f0: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
-00009500: 6564 286e 6f64 6529 2c20 7b46 6561 7475  ed(node), {Featu
-00009510: 7265 2e50 4f53 5f4f 4e4c 595f 4152 4755  re.POS_ONLY_ARGU
-00009520: 4d45 4e54 537d 290a 2020 2020 2020 2020  MENTS}).        
-00009530: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
-00009540: 3274 6f33 5f70 6172 7365 2822 6465 6620  2to3_parse("def 
-00009550: 666e 2861 2c20 2f2c 2062 293a 202e 2e2e  fn(a, /, b): ...
-00009560: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009570: 6173 7365 7274 4571 7561 6c28 7079 696e  assertEqual(pyin
-00009580: 6b2e 6765 745f 6665 6174 7572 6573 5f75  k.get_features_u
-00009590: 7365 6428 6e6f 6465 292c 207b 4665 6174  sed(node), {Feat
-000095a0: 7572 652e 504f 535f 4f4e 4c59 5f41 5247  ure.POS_ONLY_ARG
-000095b0: 554d 454e 5453 7d29 0a20 2020 2020 2020  UMENTS}).       
-000095c0: 206e 6f64 6520 3d20 7079 696e 6b2e 6c69   node = pyink.li
-000095d0: 6232 746f 335f 7061 7273 6528 2264 6566  b2to3_parse("def
-000095e0: 2066 6e28 293a 2079 6965 6c64 2061 2c20   fn(): yield a, 
-000095f0: 6222 290a 2020 2020 2020 2020 7365 6c66  b").        self
-00009600: 2e61 7373 6572 7445 7175 616c 2870 7969  .assertEqual(pyi
-00009610: 6e6b 2e67 6574 5f66 6561 7475 7265 735f  nk.get_features_
-00009620: 7573 6564 286e 6f64 6529 2c20 7365 7428  used(node), set(
-00009630: 2929 0a20 2020 2020 2020 206e 6f64 6520  )).        node 
-00009640: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
-00009650: 7061 7273 6528 2264 6566 2066 6e28 293a  parse("def fn():
-00009660: 2072 6574 7572 6e20 612c 2062 2229 0a20   return a, b"). 
-00009670: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00009680: 7274 4571 7561 6c28 7079 696e 6b2e 6765  rtEqual(pyink.ge
-00009690: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
-000096a0: 6e6f 6465 292c 2073 6574 2829 290a 2020  node), set()).  
-000096b0: 2020 2020 2020 6e6f 6465 203d 2070 7969        node = pyi
-000096c0: 6e6b 2e6c 6962 3274 6f33 5f70 6172 7365  nk.lib2to3_parse
-000096d0: 2822 6465 6620 666e 2829 3a20 7969 656c  ("def fn(): yiel
-000096e0: 6420 2a62 2c20 6322 290a 2020 2020 2020  d *b, c").      
-000096f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00009700: 616c 2870 7969 6e6b 2e67 6574 5f66 6561  al(pyink.get_fea
-00009710: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
-00009720: 2c20 7b46 6561 7475 7265 2e55 4e50 4143  , {Feature.UNPAC
-00009730: 4b49 4e47 5f4f 4e5f 464c 4f57 7d29 0a20  KING_ON_FLOW}). 
-00009740: 2020 2020 2020 206e 6f64 6520 3d20 7079         node = py
-00009750: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
-00009760: 6528 2264 6566 2066 6e28 293a 2072 6574  e("def fn(): ret
-00009770: 7572 6e20 612c 202a 622c 2063 2229 0a20  urn a, *b, c"). 
-00009780: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00009790: 7274 4571 7561 6c28 7079 696e 6b2e 6765  rtEqual(pyink.ge
-000097a0: 745f 6665 6174 7572 6573 5f75 7365 6428  t_features_used(
-000097b0: 6e6f 6465 292c 207b 4665 6174 7572 652e  node), {Feature.
-000097c0: 554e 5041 434b 494e 475f 4f4e 5f46 4c4f  UNPACKING_ON_FLO
-000097d0: 577d 290a 2020 2020 2020 2020 6e6f 6465  W}).        node
-000097e0: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-000097f0: 5f70 6172 7365 2822 7820 3d20 612c 202a  _parse("x = a, *
-00009800: 622c 2063 2229 0a20 2020 2020 2020 2073  b, c").        s
-00009810: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00009820: 7079 696e 6b2e 6765 745f 6665 6174 7572  pyink.get_featur
-00009830: 6573 5f75 7365 6428 6e6f 6465 292c 2073  es_used(node), s
-00009840: 6574 2829 290a 2020 2020 2020 2020 6e6f  et()).        no
-00009850: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
-00009860: 6f33 5f70 6172 7365 2822 783a 2041 6e79  o3_parse("x: Any
-00009870: 203d 2072 6567 756c 6172 2229 0a20 2020   = regular").   
-00009880: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009890: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
-000098a0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-000098b0: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
-000098c0: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
-000098d0: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
-000098e0: 783a 2041 6e79 203d 2028 7265 6775 6c61  x: Any = (regula
-000098f0: 722c 2072 6567 756c 6172 2922 290a 2020  r, regular)").  
-00009900: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00009910: 7445 7175 616c 2870 7969 6e6b 2e67 6574  tEqual(pyink.get
-00009920: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009930: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
-00009940: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
-00009950: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
-00009960: 2278 3a20 416e 7920 3d20 436f 6d70 6c65  "x: Any = Comple
-00009970: 7828 5479 7065 2831 2929 5b73 6f6d 6574  x(Type(1))[somet
-00009980: 6869 6e67 5d22 290a 2020 2020 2020 2020  hing]").        
-00009990: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000099a0: 2870 7969 6e6b 2e67 6574 5f66 6561 7475  (pyink.get_featu
-000099b0: 7265 735f 7573 6564 286e 6f64 6529 2c20  res_used(node), 
-000099c0: 7365 7428 2929 0a20 2020 2020 2020 206e  set()).        n
-000099d0: 6f64 6520 3d20 7079 696e 6b2e 6c69 6232  ode = pyink.lib2
-000099e0: 746f 335f 7061 7273 6528 2278 3a20 5475  to3_parse("x: Tu
-000099f0: 706c 655b 696e 742c 202e 2e2e 5d20 3d20  ple[int, ...] = 
-00009a00: 612c 2062 2c20 6322 290a 2020 2020 2020  a, b, c").      
-00009a10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00009a20: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-00009a30: 7079 696e 6b2e 6765 745f 6665 6174 7572  pyink.get_featur
-00009a40: 6573 5f75 7365 6428 6e6f 6465 292c 207b  es_used(node), {
-00009a50: 4665 6174 7572 652e 414e 4e5f 4153 5349  Feature.ANN_ASSI
-00009a60: 474e 5f45 5854 454e 4445 445f 5248 537d  GN_EXTENDED_RHS}
-00009a70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00009a80: 2020 206e 6f64 6520 3d20 7079 696e 6b2e     node = pyink.
-00009a90: 6c69 6232 746f 335f 7061 7273 6528 2274  lib2to3_parse("t
-00009aa0: 7279 3a20 7061 7373 5c6e 6578 6365 7074  ry: pass\nexcept
-00009ab0: 2053 6f6d 6574 6869 6e67 3a20 7061 7373   Something: pass
-00009ac0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009ad0: 6173 7365 7274 4571 7561 6c28 7079 696e  assertEqual(pyin
-00009ae0: 6b2e 6765 745f 6665 6174 7572 6573 5f75  k.get_features_u
-00009af0: 7365 6428 6e6f 6465 292c 2073 6574 2829  sed(node), set()
-00009b00: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-00009b10: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
-00009b20: 6172 7365 2822 7472 793a 2070 6173 735c  arse("try: pass\
-00009b30: 6e65 7863 6570 7420 282a 536f 6d65 7468  nexcept (*Someth
-00009b40: 696e 672c 293a 2070 6173 7322 290a 2020  ing,): pass").  
-00009b50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00009b60: 7445 7175 616c 2870 7969 6e6b 2e67 6574  tEqual(pyink.get
-00009b70: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
-00009b80: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
-00009b90: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
-00009ba0: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
-00009bb0: 2274 7279 3a20 7061 7373 5c6e 6578 6365  "try: pass\nexce
-00009bc0: 7074 202a 4772 6f75 703a 2070 6173 7322  pt *Group: pass"
-00009bd0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00009be0: 7373 6572 7445 7175 616c 2870 7969 6e6b  ssertEqual(pyink
-00009bf0: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
-00009c00: 6564 286e 6f64 6529 2c20 7b46 6561 7475  ed(node), {Featu
-00009c10: 7265 2e45 5843 4550 545f 5354 4152 7d29  re.EXCEPT_STAR})
-00009c20: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
-00009c30: 7079 696e 6b2e 6c69 6232 746f 335f 7061  pyink.lib2to3_pa
-00009c40: 7273 6528 2261 5b2a 625d 2229 0a20 2020  rse("a[*b]").   
-00009c50: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009c60: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
-00009c70: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009c80: 6465 292c 207b 4665 6174 7572 652e 5641  de), {Feature.VA
-00009c90: 5249 4144 4943 5f47 454e 4552 4943 537d  RIADIC_GENERICS}
-00009ca0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-00009cb0: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
-00009cc0: 6172 7365 2822 615b 782c 202a 7928 292c  arse("a[x, *y(),
-00009cd0: 207a 5d20 3d20 7422 290a 2020 2020 2020   z] = t").      
-00009ce0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00009cf0: 616c 2870 7969 6e6b 2e67 6574 5f66 6561  al(pyink.get_fea
-00009d00: 7475 7265 735f 7573 6564 286e 6f64 6529  tures_used(node)
-00009d10: 2c20 7b46 6561 7475 7265 2e56 4152 4941  , {Feature.VARIA
-00009d20: 4449 435f 4745 4e45 5249 4353 7d29 0a20  DIC_GENERICS}). 
-00009d30: 2020 2020 2020 206e 6f64 6520 3d20 7079         node = py
-00009d40: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
-00009d50: 6528 2264 6566 2066 6e28 2a61 7267 733a  e("def fn(*args:
-00009d60: 202a 5429 3a20 7061 7373 2229 0a20 2020   *T): pass").   
-00009d70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00009d80: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
-00009d90: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
-00009da0: 6465 292c 207b 4665 6174 7572 652e 5641  de), {Feature.VA
-00009db0: 5249 4144 4943 5f47 454e 4552 4943 537d  RIADIC_GENERICS}
-00009dc0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00009dd0: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
-00009de0: 645f 666f 725f 6675 7475 7265 5f66 6c61  d_for_future_fla
-00009df0: 6773 2873 656c 6629 202d 3e20 4e6f 6e65  gs(self) -> None
-00009e00: 3a0a 2020 2020 2020 2020 666f 7220 7372  :.        for sr
-00009e10: 632c 2066 6561 7475 7265 7320 696e 205b  c, features in [
-00009e20: 0a20 2020 2020 2020 2020 2020 2028 2266  .            ("f
-00009e30: 726f 6d20 5f5f 6675 7475 7265 5f5f 2069  rom __future__ i
-00009e40: 6d70 6f72 7420 616e 6e6f 7461 7469 6f6e  mport annotation
-00009e50: 7322 2c20 7b46 6561 7475 7265 2e46 5554  s", {Feature.FUT
-00009e60: 5552 455f 414e 4e4f 5441 5449 4f4e 537d  URE_ANNOTATIONS}
-00009e70: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00009e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e90: 2022 6672 6f6d 205f 5f66 7574 7572 655f   "from __future_
-00009ea0: 5f20 696d 706f 7274 2028 6f74 6865 722c  _ import (other,
-00009eb0: 2061 6e6e 6f74 6174 696f 6e73 2922 2c0a   annotations)",.
-00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 7b46 6561 7475 7265 2e46 5554 5552 455f  {Feature.FUTURE_
-00009ee0: 414e 4e4f 5441 5449 4f4e 537d 2c0a 2020  ANNOTATIONS},.  
-00009ef0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00009f00: 2020 2020 2020 2020 2028 2261 203d 2031           ("a = 1
-00009f10: 202b 2032 5c6e 6672 6f6d 2073 6f6d 6574   + 2\nfrom somet
-00009f20: 6869 6e67 2069 6d70 6f72 7420 616e 6e6f  hing import anno
-00009f30: 7461 7469 6f6e 7322 2c20 7365 7428 2929  tations", set())
-00009f40: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00009f50: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
-00009f60: 696d 706f 7274 2078 2c20 7922 2c20 7365  import x, y", se
-00009f70: 7428 2929 2c0a 2020 2020 2020 2020 5d3a  t()),.        ]:
-00009f80: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00009f90: 6820 7365 6c66 2e73 7562 5465 7374 2873  h self.subTest(s
-00009fa0: 7263 3d73 7263 2c20 6665 6174 7572 6573  rc=src, features
-00009fb0: 3d66 6561 7475 7265 7329 3a0a 2020 2020  =features):.    
-00009fc0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00009fd0: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-00009fe0: 5f70 6172 7365 2873 7263 290a 2020 2020  _parse(src).    
-00009ff0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000a000: 7265 5f69 6d70 6f72 7473 203d 2070 7969  re_imports = pyi
-0000a010: 6e6b 2e67 6574 5f66 7574 7572 655f 696d  nk.get_future_im
-0000a020: 706f 7274 7328 6e6f 6465 290a 2020 2020  ports(node).    
-0000a030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a040: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 7079 696e 6b2e 6765 745f 6665 6174    pyink.get_feat
-0000a070: 7572 6573 5f75 7365 6428 6e6f 6465 2c20  ures_used(node, 
-0000a080: 6675 7475 7265 5f69 6d70 6f72 7473 3d66  future_imports=f
-0000a090: 7574 7572 655f 696d 706f 7274 7329 2c0a  uture_imports),.
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 2020 6665 6174 7572 6573 2c0a 2020      features,.  
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000a0d0: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-0000a0e0: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
-0000a0f0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000a100: 2020 2020 2020 2020 6e6f 6465 203d 2070          node = p
-0000a110: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
-0000a120: 7365 2822 5c6e 2229 0a20 2020 2020 2020  se("\n").       
-0000a130: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000a140: 6c28 7365 7428 292c 2070 7969 6e6b 2e67  l(set(), pyink.g
-0000a150: 6574 5f66 7574 7572 655f 696d 706f 7274  et_future_import
-0000a160: 7328 6e6f 6465 2929 0a20 2020 2020 2020  s(node)).       
-0000a170: 206e 6f64 6520 3d20 7079 696e 6b2e 6c69   node = pyink.li
-0000a180: 6232 746f 335f 7061 7273 6528 2266 726f  b2to3_parse("fro
-0000a190: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
-0000a1a0: 6f72 7420 7079 696e 6b5c 6e22 290a 2020  ort pyink\n").  
-0000a1b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a1c0: 7445 7175 616c 287b 2270 7969 6e6b 227d  tEqual({"pyink"}
-0000a1d0: 2c20 7079 696e 6b2e 6765 745f 6675 7475  , pyink.get_futu
-0000a1e0: 7265 5f69 6d70 6f72 7473 286e 6f64 6529  re_imports(node)
-0000a1f0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-0000a200: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
-0000a210: 6172 7365 2822 6672 6f6d 205f 5f66 7574  arse("from __fut
-0000a220: 7572 655f 5f20 696d 706f 7274 206d 756c  ure__ import mul
-0000a230: 7469 706c 652c 2069 6d70 6f72 7473 5c6e  tiple, imports\n
-0000a240: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000a250: 6173 7365 7274 4571 7561 6c28 7b22 6d75  assertEqual({"mu
-0000a260: 6c74 6970 6c65 222c 2022 696d 706f 7274  ltiple", "import
-0000a270: 7322 7d2c 2070 7969 6e6b 2e67 6574 5f66  s"}, pyink.get_f
-0000a280: 7574 7572 655f 696d 706f 7274 7328 6e6f  uture_imports(no
-0000a290: 6465 2929 0a20 2020 2020 2020 206e 6f64  de)).        nod
-0000a2a0: 6520 3d20 7079 696e 6b2e 6c69 6232 746f  e = pyink.lib2to
-0000a2b0: 335f 7061 7273 6528 2266 726f 6d20 5f5f  3_parse("from __
-0000a2c0: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
-0000a2d0: 2870 6172 656e 7468 6573 697a 6564 2c20  (parenthesized, 
-0000a2e0: 696d 706f 7274 7329 5c6e 2229 0a20 2020  imports)\n").   
-0000a2f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000a300: 4571 7561 6c28 7b22 7061 7265 6e74 6865  Equal({"parenthe
-0000a310: 7369 7a65 6422 2c20 2269 6d70 6f72 7473  sized", "imports
-0000a320: 227d 2c20 7079 696e 6b2e 6765 745f 6675  "}, pyink.get_fu
-0000a330: 7475 7265 5f69 6d70 6f72 7473 286e 6f64  ture_imports(nod
-0000a340: 6529 290a 2020 2020 2020 2020 6e6f 6465  e)).        node
-0000a350: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-0000a360: 5f70 6172 7365 280a 2020 2020 2020 2020  _parse(.        
-0000a370: 2020 2020 2266 726f 6d20 5f5f 6675 7475      "from __futu
-0000a380: 7265 5f5f 2069 6d70 6f72 7420 6d75 6c74  re__ import mult
-0000a390: 6970 6c65 5c6e 6672 6f6d 205f 5f66 7574  iple\nfrom __fut
-0000a3a0: 7572 655f 5f20 696d 706f 7274 2069 6d70  ure__ import imp
-0000a3b0: 6f72 7473 5c6e 220a 2020 2020 2020 2020  orts\n".        
-0000a3c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000a3d0: 7373 6572 7445 7175 616c 287b 226d 756c  ssertEqual({"mul
-0000a3e0: 7469 706c 6522 2c20 2269 6d70 6f72 7473  tiple", "imports
-0000a3f0: 227d 2c20 7079 696e 6b2e 6765 745f 6675  "}, pyink.get_fu
-0000a400: 7475 7265 5f69 6d70 6f72 7473 286e 6f64  ture_imports(nod
-0000a410: 6529 290a 2020 2020 2020 2020 6e6f 6465  e)).        node
-0000a420: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-0000a430: 5f70 6172 7365 2822 2320 636f 6d6d 656e  _parse("# commen
-0000a440: 745c 6e66 726f 6d20 5f5f 6675 7475 7265  t\nfrom __future
-0000a450: 5f5f 2069 6d70 6f72 7420 7079 696e 6b5c  __ import pyink\
-0000a460: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
-0000a470: 2e61 7373 6572 7445 7175 616c 287b 2270  .assertEqual({"p
-0000a480: 7969 6e6b 227d 2c20 7079 696e 6b2e 6765  yink"}, pyink.ge
-0000a490: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
-0000a4a0: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
-0000a4b0: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
-0000a4c0: 3274 6f33 5f70 6172 7365 2827 2222 2264  2to3_parse('"""d
-0000a4d0: 6f63 7374 7269 6e67 2222 225c 6e66 726f  ocstring"""\nfro
-0000a4e0: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
-0000a4f0: 6f72 7420 7079 696e 6b5c 6e27 290a 2020  ort pyink\n').  
-0000a500: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a510: 7445 7175 616c 287b 2270 7969 6e6b 227d  tEqual({"pyink"}
-0000a520: 2c20 7079 696e 6b2e 6765 745f 6675 7475  , pyink.get_futu
-0000a530: 7265 5f69 6d70 6f72 7473 286e 6f64 6529  re_imports(node)
-0000a540: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
-0000a550: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
-0000a560: 6172 7365 2822 736f 6d65 286f 7468 6572  arse("some(other
-0000a570: 2c20 636f 6465 295c 6e66 726f 6d20 5f5f  , code)\nfrom __
-0000a580: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
-0000a590: 7079 696e 6b5c 6e22 290a 2020 2020 2020  pyink\n").      
-0000a5a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000a5b0: 616c 2873 6574 2829 2c20 7079 696e 6b2e  al(set(), pyink.
-0000a5c0: 6765 745f 6675 7475 7265 5f69 6d70 6f72  get_future_impor
-0000a5d0: 7473 286e 6f64 6529 290a 2020 2020 2020  ts(node)).      
-0000a5e0: 2020 6e6f 6465 203d 2070 7969 6e6b 2e6c    node = pyink.l
-0000a5f0: 6962 3274 6f33 5f70 6172 7365 2822 6672  ib2to3_parse("fr
-0000a600: 6f6d 2073 6f6d 652e 6d6f 6475 6c65 2069  om some.module i
-0000a610: 6d70 6f72 7420 7079 696e 6b5c 6e22 290a  mport pyink\n").
-0000a620: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000a630: 6572 7445 7175 616c 2873 6574 2829 2c20  ertEqual(set(), 
-0000a640: 7079 696e 6b2e 6765 745f 6675 7475 7265  pyink.get_future
-0000a650: 5f69 6d70 6f72 7473 286e 6f64 6529 290a  _imports(node)).
-0000a660: 2020 2020 2020 2020 6e6f 6465 203d 2070          node = p
-0000a670: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
-0000a680: 7365 280a 2020 2020 2020 2020 2020 2020  se(.            
-0000a690: 2266 726f 6d20 5f5f 6675 7475 7265 5f5f  "from __future__
-0000a6a0: 2069 6d70 6f72 7420 756e 6963 6f64 655f   import unicode_
-0000a6b0: 6c69 7465 7261 6c73 2061 7320 5f75 6e69  literals as _uni
-0000a6c0: 636f 6465 5f6c 6974 6572 616c 7322 0a20  code_literals". 
-0000a6d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a6e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000a6f0: 6c28 7b22 756e 6963 6f64 655f 6c69 7465  l({"unicode_lite
-0000a700: 7261 6c73 227d 2c20 7079 696e 6b2e 6765  rals"}, pyink.ge
-0000a710: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
-0000a720: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
-0000a730: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
-0000a740: 3274 6f33 5f70 6172 7365 280a 2020 2020  2to3_parse(.    
-0000a750: 2020 2020 2020 2020 2266 726f 6d20 5f5f          "from __
-0000a760: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
-0000a770: 756e 6963 6f64 655f 6c69 7465 7261 6c73  unicode_literals
-0000a780: 2061 7320 5f6c 6f6c 2c20 7072 696e 7422   as _lol, print"
-0000a790: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000a7a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000a7b0: 7561 6c28 7b22 756e 6963 6f64 655f 6c69  ual({"unicode_li
-0000a7c0: 7465 7261 6c73 222c 2022 7072 696e 7422  terals", "print"
-0000a7d0: 7d2c 2070 7969 6e6b 2e67 6574 5f66 7574  }, pyink.get_fut
-0000a7e0: 7572 655f 696d 706f 7274 7328 6e6f 6465  ure_imports(node
-0000a7f0: 2929 0a0a 2020 2020 4070 7974 6573 742e  ))..    @pytest.
-0000a800: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
-0000a810: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
-0000a820: 2064 6566 2074 6573 745f 6465 6275 675f   def test_debug_
-0000a830: 7669 7369 746f 7228 7365 6c66 2920 2d3e  visitor(self) ->
-0000a840: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-0000a850: 6f75 7263 652c 205f 203d 2072 6561 645f  ource, _ = read_
-0000a860: 6461 7461 2822 6d69 7363 656c 6c61 6e65  data("miscellane
-0000a870: 6f75 7322 2c20 2264 6562 7567 5f76 6973  ous", "debug_vis
-0000a880: 6974 6f72 2229 0a20 2020 2020 2020 2065  itor").        e
-0000a890: 7870 6563 7465 642c 205f 203d 2072 6561  xpected, _ = rea
-0000a8a0: 645f 6461 7461 2822 6d69 7363 656c 6c61  d_data("miscella
-0000a8b0: 6e65 6f75 7322 2c20 2264 6562 7567 5f76  neous", "debug_v
-0000a8c0: 6973 6974 6f72 2e6f 7574 2229 0a20 2020  isitor.out").   
-0000a8d0: 2020 2020 206f 7574 5f6c 696e 6573 203d       out_lines =
-0000a8e0: 205b 5d0a 2020 2020 2020 2020 6572 725f   [].        err_
-0000a8f0: 6c69 6e65 7320 3d20 5b5d 0a0a 2020 2020  lines = []..    
-0000a900: 2020 2020 6465 6620 6f75 7428 6d73 673a      def out(msg:
-0000a910: 2073 7472 2c20 2a2a 6b77 6172 6773 3a20   str, **kwargs: 
-0000a920: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
-0000a930: 2020 2020 2020 2020 2020 6f75 745f 6c69            out_li
-0000a940: 6e65 732e 6170 7065 6e64 286d 7367 290a  nes.append(msg).
-0000a950: 0a20 2020 2020 2020 2064 6566 2065 7272  .        def err
-0000a960: 286d 7367 3a20 7374 722c 202a 2a6b 7761  (msg: str, **kwa
-0000a970: 7267 733a 2041 6e79 2920 2d3e 204e 6f6e  rgs: Any) -> Non
-0000a980: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-0000a990: 7272 5f6c 696e 6573 2e61 7070 656e 6428  rr_lines.append(
-0000a9a0: 6d73 6729 0a0a 2020 2020 2020 2020 7769  msg)..        wi
-0000a9b0: 7468 2070 6174 6368 2822 7079 696e 6b2e  th patch("pyink.
-0000a9c0: 6465 6275 672e 6f75 7422 2c20 6f75 7429  debug.out", out)
-0000a9d0: 3a0a 2020 2020 2020 2020 2020 2020 4465  :.            De
-0000a9e0: 6275 6756 6973 6974 6f72 2e73 686f 7728  bugVisitor.show(
-0000a9f0: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
-0000aa00: 6163 7475 616c 203d 2022 5c6e 222e 6a6f  actual = "\n".jo
-0000aa10: 696e 286f 7574 5f6c 696e 6573 2920 2b20  in(out_lines) + 
-0000aa20: 225c 6e22 0a20 2020 2020 2020 206c 6f67  "\n".        log
-0000aa30: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
-0000aa40: 2020 2069 6620 6578 7065 6374 6564 2021     if expected !
-0000aa50: 3d20 6163 7475 616c 3a0a 2020 2020 2020  = actual:.      
-0000aa60: 2020 2020 2020 6c6f 675f 6e61 6d65 203d        log_name =
-0000aa70: 2070 7969 6e6b 2e64 756d 705f 746f 5f66   pyink.dump_to_f
-0000aa80: 696c 6528 2a6f 7574 5f6c 696e 6573 290a  ile(*out_lines).
-0000aa90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000aaa0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-0000aab0: 2020 2020 2020 6578 7065 6374 6564 2c0a        expected,.
-0000aac0: 2020 2020 2020 2020 2020 2020 6163 7475              actu
-0000aad0: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-0000aae0: 6622 4153 5420 7072 696e 7420 6f75 7420  f"AST print out 
-0000aaf0: 6973 2064 6966 6665 7265 6e74 2e20 4163  is different. Ac
-0000ab00: 7475 616c 2076 6572 7369 6f6e 2064 756d  tual version dum
-0000ab10: 7065 6420 746f 207b 6c6f 675f 6e61 6d65  ped to {log_name
-0000ab20: 7d22 2c0a 2020 2020 2020 2020 290a 0a20  }",.        ).. 
-0000ab30: 2020 2064 6566 2074 6573 745f 666f 726d     def test_form
-0000ab40: 6174 5f66 696c 655f 636f 6e74 656e 7473  at_file_contents
-0000ab50: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000ab60: 2020 2020 2020 2020 6d6f 6465 203d 2044          mode = D
-0000ab70: 4546 4155 4c54 5f4d 4f44 450a 2020 2020  EFAULT_MODE.    
-0000ab80: 2020 2020 656d 7074 7920 3d20 2222 0a20      empty = "". 
-0000ab90: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000aba0: 2e61 7373 6572 7452 6169 7365 7328 7079  .assertRaises(py
-0000abb0: 696e 6b2e 4e6f 7468 696e 6743 6861 6e67  ink.NothingChang
-0000abc0: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
-0000abd0: 2070 7969 6e6b 2e66 6f72 6d61 745f 6669   pyink.format_fi
-0000abe0: 6c65 5f63 6f6e 7465 6e74 7328 656d 7074  le_contents(empt
-0000abf0: 792c 206d 6f64 653d 6d6f 6465 2c20 6661  y, mode=mode, fa
-0000ac00: 7374 3d46 616c 7365 290a 2020 2020 2020  st=False).      
-0000ac10: 2020 6a75 7374 5f6e 6c20 3d20 225c 6e22    just_nl = "\n"
-0000ac20: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000ac30: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0000ac40: 7079 696e 6b2e 4e6f 7468 696e 6743 6861  pyink.NothingCha
-0000ac50: 6e67 6564 293a 0a20 2020 2020 2020 2020  nged):.         
-0000ac60: 2020 2070 7969 6e6b 2e66 6f72 6d61 745f     pyink.format_
-0000ac70: 6669 6c65 5f63 6f6e 7465 6e74 7328 6a75  file_contents(ju
-0000ac80: 7374 5f6e 6c2c 206d 6f64 653d 6d6f 6465  st_nl, mode=mode
-0000ac90: 2c20 6661 7374 3d46 616c 7365 290a 2020  , fast=False).  
-0000aca0: 2020 2020 2020 7361 6d65 203d 2022 6a20        same = "j 
-0000acb0: 3d20 5b31 2c20 322c 2033 5d5c 6e22 0a20  = [1, 2, 3]\n". 
-0000acc0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000acd0: 2e61 7373 6572 7452 6169 7365 7328 7079  .assertRaises(py
-0000ace0: 696e 6b2e 4e6f 7468 696e 6743 6861 6e67  ink.NothingChang
-0000acf0: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
-0000ad00: 2070 7969 6e6b 2e66 6f72 6d61 745f 6669   pyink.format_fi
-0000ad10: 6c65 5f63 6f6e 7465 6e74 7328 7361 6d65  le_contents(same
-0000ad20: 2c20 6d6f 6465 3d6d 6f64 652c 2066 6173  , mode=mode, fas
-0000ad30: 743d 4661 6c73 6529 0a20 2020 2020 2020  t=False).       
-0000ad40: 2064 6966 6665 7265 6e74 203d 2022 6a20   different = "j 
-0000ad50: 3d20 5b31 2c32 2c33 5d22 0a20 2020 2020  = [1,2,3]".     
-0000ad60: 2020 2065 7870 6563 7465 6420 3d20 7361     expected = sa
-0000ad70: 6d65 0a20 2020 2020 2020 2061 6374 7561  me.        actua
-0000ad80: 6c20 3d20 7079 696e 6b2e 666f 726d 6174  l = pyink.format
-0000ad90: 5f66 696c 655f 636f 6e74 656e 7473 2864  _file_contents(d
-0000ada0: 6966 6665 7265 6e74 2c20 6d6f 6465 3d6d  ifferent, mode=m
-0000adb0: 6f64 652c 2066 6173 743d 4661 6c73 6529  ode, fast=False)
-0000adc0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000add0: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000ade0: 6564 2c20 6163 7475 616c 290a 2020 2020  ed, actual).    
-0000adf0: 2020 2020 696e 7661 6c69 6420 3d20 2272      invalid = "r
-0000ae00: 6574 7572 6e20 6966 2079 6f75 2063 616e  eturn if you can
-0000ae10: 220a 2020 2020 2020 2020 7769 7468 2073  ".        with s
-0000ae20: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-0000ae30: 2870 7969 6e6b 2e49 6e76 616c 6964 496e  (pyink.InvalidIn
-0000ae40: 7075 7429 2061 7320 653a 0a20 2020 2020  put) as e:.     
-0000ae50: 2020 2020 2020 2070 7969 6e6b 2e66 6f72         pyink.for
-0000ae60: 6d61 745f 6669 6c65 5f63 6f6e 7465 6e74  mat_file_content
-0000ae70: 7328 696e 7661 6c69 642c 206d 6f64 653d  s(invalid, mode=
-0000ae80: 6d6f 6465 2c20 6661 7374 3d46 616c 7365  mode, fast=False
-0000ae90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000aea0: 7373 6572 7445 7175 616c 2873 7472 2865  ssertEqual(str(e
-0000aeb0: 2e65 7863 6570 7469 6f6e 292c 2022 4361  .exception), "Ca
-0000aec0: 6e6e 6f74 2070 6172 7365 3a20 313a 373a  nnot parse: 1:7:
-0000aed0: 2072 6574 7572 6e20 6966 2079 6f75 2063   return if you c
-0000aee0: 616e 2229 0a0a 2020 2020 2020 2020 6d6f  an")..        mo
-0000aef0: 6465 203d 2070 7969 6e6b 2e4d 6f64 6528  de = pyink.Mode(
-0000af00: 7072 6576 6965 773d 5472 7565 290a 2020  preview=True).  
-0000af10: 2020 2020 2020 6a75 7374 5f63 726c 6620        just_crlf 
-0000af20: 3d20 225c 725c 6e22 0a20 2020 2020 2020  = "\r\n".       
-0000af30: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-0000af40: 7452 6169 7365 7328 7079 696e 6b2e 4e6f  tRaises(pyink.No
-0000af50: 7468 696e 6743 6861 6e67 6564 293a 0a20  thingChanged):. 
-0000af60: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
-0000af70: 2e66 6f72 6d61 745f 6669 6c65 5f63 6f6e  .format_file_con
-0000af80: 7465 6e74 7328 6a75 7374 5f63 726c 662c  tents(just_crlf,
-0000af90: 206d 6f64 653d 6d6f 6465 2c20 6661 7374   mode=mode, fast
-0000afa0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-0000afb0: 6a75 7374 5f77 6869 7465 7370 6163 655f  just_whitespace_
-0000afc0: 6e6c 203d 2022 5c6e 5c74 5c6e 205c 6e5c  nl = "\n\t\n \n\
-0000afd0: 7420 5c6e 205c 745c 6e5c 6e22 0a20 2020  t \n \t\n\n".   
-0000afe0: 2020 2020 2061 6374 7561 6c20 3d20 7079       actual = py
-0000aff0: 696e 6b2e 666f 726d 6174 5f66 696c 655f  ink.format_file_
-0000b000: 636f 6e74 656e 7473 286a 7573 745f 7768  contents(just_wh
-0000b010: 6974 6573 7061 6365 5f6e 6c2c 206d 6f64  itespace_nl, mod
-0000b020: 653d 6d6f 6465 2c20 6661 7374 3d46 616c  e=mode, fast=Fal
-0000b030: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
-0000b040: 2e61 7373 6572 7445 7175 616c 2822 5c6e  .assertEqual("\n
-0000b050: 222c 2061 6374 7561 6c29 0a20 2020 2020  ", actual).     
-0000b060: 2020 206a 7573 745f 7768 6974 6573 7061     just_whitespa
-0000b070: 6365 5f63 726c 6620 3d20 225c 725c 6e5c  ce_crlf = "\r\n\
-0000b080: 745c 725c 6e20 5c72 5c6e 5c74 205c 725c  t\r\n \r\n\t \r\
-0000b090: 6e20 5c74 5c72 5c6e 5c72 5c6e 220a 2020  n \t\r\n\r\n".  
-0000b0a0: 2020 2020 2020 6163 7475 616c 203d 2070        actual = p
-0000b0b0: 7969 6e6b 2e66 6f72 6d61 745f 6669 6c65  yink.format_file
-0000b0c0: 5f63 6f6e 7465 6e74 7328 6a75 7374 5f77  _contents(just_w
-0000b0d0: 6869 7465 7370 6163 655f 6372 6c66 2c20  hitespace_crlf, 
-0000b0e0: 6d6f 6465 3d6d 6f64 652c 2066 6173 743d  mode=mode, fast=
-0000b0f0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0000b100: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000b110: 225c 725c 6e22 2c20 6163 7475 616c 290a  "\r\n", actual).
-0000b120: 0a20 2020 2064 6566 2074 6573 745f 656e  .    def test_en
-0000b130: 646d 6172 6b65 7228 7365 6c66 2920 2d3e  dmarker(self) ->
-0000b140: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
-0000b150: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
-0000b160: 5f70 6172 7365 2822 5c6e 2229 0a20 2020  _parse("\n").   
-0000b170: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b180: 4571 7561 6c28 6e2e 7479 7065 2c20 7079  Equal(n.type, py
-0000b190: 696e 6b2e 7379 6d73 2e66 696c 655f 696e  ink.syms.file_in
-0000b1a0: 7075 7429 0a20 2020 2020 2020 2073 656c  put).        sel
-0000b1b0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-0000b1c0: 6e28 6e2e 6368 696c 6472 656e 292c 2031  n(n.children), 1
-0000b1d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000b1e0: 7373 6572 7445 7175 616c 286e 2e63 6869  ssertEqual(n.chi
-0000b1f0: 6c64 7265 6e5b 305d 2e74 7970 652c 2070  ldren[0].type, p
-0000b200: 7969 6e6b 2e74 6f6b 656e 2e45 4e44 4d41  yink.token.ENDMA
-0000b210: 524b 4552 290a 0a20 2020 2040 7079 7465  RKER)..    @pyte
-0000b220: 7374 2e6d 6172 6b2e 696e 636f 6d70 6174  st.mark.incompat
-0000b230: 6962 6c65 5f77 6974 685f 6d79 7079 630a  ible_with_mypyc.
-0000b240: 2020 2020 4075 6e69 7474 6573 742e 736b      @unittest.sk
-0000b250: 6970 4966 286f 732e 656e 7669 726f 6e2e  ipIf(os.environ.
-0000b260: 6765 7428 2253 4b49 505f 4153 545f 5052  get("SKIP_AST_PR
-0000b270: 494e 5422 292c 2022 7573 6572 2073 6574  INT"), "user set
-0000b280: 2053 4b49 505f 4153 545f 5052 494e 5422   SKIP_AST_PRINT"
-0000b290: 290a 2020 2020 6465 6620 7465 7374 5f61  ).    def test_a
-0000b2a0: 7373 6572 7446 6f72 6d61 7445 7175 616c  ssertFormatEqual
-0000b2b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000b2c0: 2020 2020 2020 2020 6f75 745f 6c69 6e65          out_line
-0000b2d0: 7320 3d20 5b5d 0a20 2020 2020 2020 2065  s = [].        e
-0000b2e0: 7272 5f6c 696e 6573 203d 205b 5d0a 0a20  rr_lines = [].. 
-0000b2f0: 2020 2020 2020 2064 6566 206f 7574 286d         def out(m
-0000b300: 7367 3a20 7374 722c 202a 2a6b 7761 7267  sg: str, **kwarg
-0000b310: 733a 2041 6e79 2920 2d3e 204e 6f6e 653a  s: Any) -> None:
-0000b320: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-0000b330: 5f6c 696e 6573 2e61 7070 656e 6428 6d73  _lines.append(ms
-0000b340: 6729 0a0a 2020 2020 2020 2020 6465 6620  g)..        def 
-0000b350: 6572 7228 6d73 673a 2073 7472 2c20 2a2a  err(msg: str, **
-0000b360: 6b77 6172 6773 3a20 416e 7929 202d 3e20  kwargs: Any) -> 
-0000b370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b380: 2020 6572 725f 6c69 6e65 732e 6170 7065    err_lines.appe
-0000b390: 6e64 286d 7367 290a 0a20 2020 2020 2020  nd(msg)..       
-0000b3a0: 2077 6974 6820 7061 7463 6828 2270 7969   with patch("pyi
-0000b3b0: 6e6b 2e6f 7574 7075 742e 5f6f 7574 222c  nk.output._out",
-0000b3c0: 206f 7574 292c 2070 6174 6368 2822 7079   out), patch("py
-0000b3d0: 696e 6b2e 6f75 7470 7574 2e5f 6572 7222  ink.output._err"
-0000b3e0: 2c20 6572 7229 3a0a 2020 2020 2020 2020  , err):.        
-0000b3f0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-0000b400: 7365 7274 5261 6973 6573 2841 7373 6572  sertRaises(Asser
-0000b410: 7469 6f6e 4572 726f 7229 3a0a 2020 2020  tionError):.    
-0000b420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b430: 2e61 7373 6572 7446 6f72 6d61 7445 7175  .assertFormatEqu
-0000b440: 616c 2822 6a20 3d20 5b31 2c20 322c 2033  al("j = [1, 2, 3
-0000b450: 5d22 2c20 226a 203d 205b 312c 2032 2c20  ]", "j = [1, 2, 
-0000b460: 332c 5d22 290a 0a20 2020 2020 2020 206f  3,]")..        o
-0000b470: 7574 5f73 7472 203d 2022 222e 6a6f 696e  ut_str = "".join
-0000b480: 286f 7574 5f6c 696e 6573 290a 2020 2020  (out_lines).    
-0000b490: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-0000b4a0: 6e28 2245 7870 6563 7465 6420 7472 6565  n("Expected tree
-0000b4b0: 3a22 2c20 6f75 745f 7374 7229 0a20 2020  :", out_str).   
-0000b4c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000b4d0: 496e 2822 4163 7475 616c 2074 7265 653a  In("Actual tree:
-0000b4e0: 222c 206f 7574 5f73 7472 290a 2020 2020  ", out_str).    
-0000b4f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000b500: 7175 616c 2822 222e 6a6f 696e 2865 7272  qual("".join(err
-0000b510: 5f6c 696e 6573 292c 2022 2229 0a0a 2020  _lines), "")..  
-0000b520: 2020 4065 7665 6e74 5f6c 6f6f 7028 290a    @event_loop().
-0000b530: 2020 2020 4070 6174 6368 2822 636f 6e63      @patch("conc
-0000b540: 7572 7265 6e74 2e66 7574 7572 6573 2e50  urrent.futures.P
-0000b550: 726f 6365 7373 506f 6f6c 4578 6563 7574  rocessPoolExecut
-0000b560: 6f72 222c 204d 6167 6963 4d6f 636b 2873  or", MagicMock(s
-0000b570: 6964 655f 6566 6665 6374 3d4f 5345 7272  ide_effect=OSErr
-0000b580: 6f72 2929 0a20 2020 2064 6566 2074 6573  or)).    def tes
-0000b590: 745f 776f 726b 735f 696e 5f6d 6f6e 6f5f  t_works_in_mono_
-0000b5a0: 7072 6f63 6573 735f 6f6e 6c79 5f65 6e76  process_only_env
-0000b5b0: 6972 6f6e 6d65 6e74 2873 656c 6629 202d  ironment(self) -
-0000b5c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000b5d0: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
-0000b5e0: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
-0000b5f0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-0000b600: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-0000b610: 2020 2020 2020 2877 6f72 6b73 7061 6365        (workspace
-0000b620: 202f 2022 6f6e 652e 7079 2229 2e72 6573   / "one.py").res
-0000b630: 6f6c 7665 2829 2c0a 2020 2020 2020 2020  olve(),.        
-0000b640: 2020 2020 2020 2020 2877 6f72 6b73 7061          (workspa
-0000b650: 6365 202f 2022 7477 6f2e 7079 2229 2e72  ce / "two.py").r
-0000b660: 6573 6f6c 7665 2829 2c0a 2020 2020 2020  esolve(),.      
-0000b670: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
-0000b680: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-0000b690: 5f74 6578 7428 2770 7269 6e74 2822 6865  _text('print("he
-0000b6a0: 6c6c 6f22 295c 6e27 290a 2020 2020 2020  llo")\n').      
-0000b6b0: 2020 2020 2020 7365 6c66 2e69 6e76 6f6b        self.invok
-0000b6c0: 6542 6c61 636b 285b 7374 7228 776f 726b  eBlack([str(work
-0000b6d0: 7370 6163 6529 5d29 0a0a 2020 2020 4065  space)])..    @e
-0000b6e0: 7665 6e74 5f6c 6f6f 7028 290a 2020 2020  vent_loop().    
-0000b6f0: 6465 6620 7465 7374 5f63 6865 636b 5f64  def test_check_d
-0000b700: 6966 665f 7573 655f 746f 6765 7468 6572  iff_use_together
-0000b710: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000b720: 2020 2020 2020 2020 7769 7468 2063 6163          with cac
-0000b730: 6865 5f64 6972 2829 3a0a 2020 2020 2020  he_dir():.      
-0000b740: 2020 2020 2020 2320 4669 6c65 7320 7768        # Files wh
-0000b750: 6963 6820 7769 6c6c 2062 6520 7265 666f  ich will be refo
-0000b760: 726d 6174 7465 642e 0a20 2020 2020 2020  rmatted..       
-0000b770: 2020 2020 2073 7263 3120 3d20 6765 745f       src1 = get_
-0000b780: 6361 7365 5f70 6174 6828 226d 6973 6365  case_path("misce
-0000b790: 6c6c 616e 656f 7573 222c 2022 7374 7269  llaneous", "stri
-0000b7a0: 6e67 5f71 756f 7465 7322 290a 2020 2020  ng_quotes").    
-0000b7b0: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
-0000b7c0: 6f6b 6542 6c61 636b 285b 7374 7228 7372  okeBlack([str(sr
-0000b7d0: 6331 292c 2022 2d2d 6469 6666 222c 2022  c1), "--diff", "
-0000b7e0: 2d2d 6368 6563 6b22 5d2c 2065 7869 745f  --check"], exit_
-0000b7f0: 636f 6465 3d31 290a 2020 2020 2020 2020  code=1).        
-0000b800: 2020 2020 2320 4669 6c65 7320 7768 6963      # Files whic
-0000b810: 6820 7769 6c6c 206e 6f74 2062 6520 7265  h will not be re
-0000b820: 666f 726d 6174 7465 642e 0a20 2020 2020  formatted..     
-0000b830: 2020 2020 2020 2073 7263 3220 3d20 6765         src2 = ge
-0000b840: 745f 6361 7365 5f70 6174 6828 2273 696d  t_case_path("sim
-0000b850: 706c 655f 6361 7365 7322 2c20 2263 6f6d  ple_cases", "com
-0000b860: 706f 7369 7469 6f6e 2229 0a20 2020 2020  position").     
-0000b870: 2020 2020 2020 2073 656c 662e 696e 766f         self.invo
-0000b880: 6b65 426c 6163 6b28 5b73 7472 2873 7263  keBlack([str(src
-0000b890: 3229 2c20 222d 2d64 6966 6622 2c20 222d  2), "--diff", "-
-0000b8a0: 2d63 6865 636b 225d 290a 2020 2020 2020  -check"]).      
-0000b8b0: 2020 2020 2020 2320 4d75 6c74 6920 6669        # Multi fi
-0000b8c0: 6c65 2063 6f6d 6d61 6e64 2e0a 2020 2020  le command..    
-0000b8d0: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
-0000b8e0: 6f6b 6542 6c61 636b 285b 7374 7228 7372  okeBlack([str(sr
-0000b8f0: 6331 292c 2073 7472 2873 7263 3229 2c20  c1), str(src2), 
-0000b900: 222d 2d64 6966 6622 2c20 222d 2d63 6865  "--diff", "--che
-0000b910: 636b 225d 2c20 6578 6974 5f63 6f64 653d  ck"], exit_code=
-0000b920: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
-0000b930: 5f6e 6f5f 7372 635f 6661 696c 7328 7365  _no_src_fails(se
-0000b940: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000b950: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
-0000b960: 6469 7228 293a 0a20 2020 2020 2020 2020  dir():.         
-0000b970: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
-0000b980: 6163 6b28 5b5d 2c20 6578 6974 5f63 6f64  ack([], exit_cod
-0000b990: 653d 3129 0a0a 2020 2020 6465 6620 7465  e=1)..    def te
-0000b9a0: 7374 5f73 7263 5f61 6e64 5f63 6f64 655f  st_src_and_code_
-0000b9b0: 6661 696c 7328 7365 6c66 2920 2d3e 204e  fails(self) -> N
-0000b9c0: 6f6e 653a 0a20 2020 2020 2020 2077 6974  one:.        wit
-0000b9d0: 6820 6361 6368 655f 6469 7228 293a 0a20  h cache_dir():. 
-0000b9e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b9f0: 696e 766f 6b65 426c 6163 6b28 5b22 2e22  invokeBlack(["."
-0000ba00: 2c20 222d 6322 2c20 2230 225d 2c20 6578  , "-c", "0"], ex
-0000ba10: 6974 5f63 6f64 653d 3129 0a0a 2020 2020  it_code=1)..    
-0000ba20: 6465 6620 7465 7374 5f62 726f 6b65 6e5f  def test_broken_
-0000ba30: 7379 6d6c 696e 6b28 7365 6c66 2920 2d3e  symlink(self) ->
-0000ba40: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
-0000ba50: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
-0000ba60: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
-0000ba70: 2020 2020 2020 2020 2020 7379 6d6c 696e            symlin
-0000ba80: 6b20 3d20 776f 726b 7370 6163 6520 2f20  k = workspace / 
-0000ba90: 2262 726f 6b65 6e5f 6c69 6e6b 2e70 7922  "broken_link.py"
-0000baa0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000bab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bac0: 2020 7379 6d6c 696e 6b2e 7379 6d6c 696e    symlink.symlin
-0000bad0: 6b5f 746f 2822 6e6f 6e65 7869 7374 656e  k_to("nonexisten
-0000bae0: 742e 7079 2229 0a20 2020 2020 2020 2020  t.py").         
-0000baf0: 2020 2065 7863 6570 7420 284f 5345 7272     except (OSErr
-0000bb00: 6f72 2c20 4e6f 7449 6d70 6c65 6d65 6e74  or, NotImplement
-0000bb10: 6564 4572 726f 7229 2061 7320 653a 0a20  edError) as e:. 
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bb30: 656c 662e 736b 6970 5465 7374 2866 2243  elf.skipTest(f"C
-0000bb40: 616e 2774 2063 7265 6174 6520 7379 6d6c  an't create syml
-0000bb50: 696e 6b73 3a20 7b65 7d22 290a 2020 2020  inks: {e}").    
-0000bb60: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
-0000bb70: 6f6b 6542 6c61 636b 285b 7374 7228 776f  okeBlack([str(wo
-0000bb80: 726b 7370 6163 652e 7265 736f 6c76 6528  rkspace.resolve(
-0000bb90: 2929 5d29 0a0a 2020 2020 6465 6620 7465  ))])..    def te
-0000bba0: 7374 5f73 696e 676c 655f 6669 6c65 5f66  st_single_file_f
-0000bbb0: 6f72 6365 5f70 7969 2873 656c 6629 202d  orce_pyi(self) -
-0000bbc0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000bbd0: 7079 695f 6d6f 6465 203d 2072 6570 6c61  pyi_mode = repla
-0000bbe0: 6365 2844 4546 4155 4c54 5f4d 4f44 452c  ce(DEFAULT_MODE,
-0000bbf0: 2069 735f 7079 693d 5472 7565 290a 2020   is_pyi=True).  
-0000bc00: 2020 2020 2020 636f 6e74 656e 7473 2c20        contents, 
-0000bc10: 6578 7065 6374 6564 203d 2072 6561 645f  expected = read_
-0000bc20: 6461 7461 2822 6d69 7363 656c 6c61 6e65  data("miscellane
-0000bc30: 6f75 7322 2c20 2266 6f72 6365 5f70 7969  ous", "force_pyi
-0000bc40: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
-0000bc50: 6361 6368 655f 6469 7228 2920 6173 2077  cache_dir() as w
-0000bc60: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
-0000bc70: 2020 2020 2020 7061 7468 203d 2028 776f        path = (wo
-0000bc80: 726b 7370 6163 6520 2f20 2266 696c 652e  rkspace / "file.
-0000bc90: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
-0000bca0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000bcb0: 6f70 656e 2870 6174 682c 2022 7722 2920  open(path, "w") 
-0000bcc0: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
-0000bcd0: 2020 2020 2020 2066 682e 7772 6974 6528         fh.write(
-0000bce0: 636f 6e74 656e 7473 290a 2020 2020 2020  contents).      
-0000bcf0: 2020 2020 2020 7365 6c66 2e69 6e76 6f6b        self.invok
-0000bd00: 6542 6c61 636b 285b 7374 7228 7061 7468  eBlack([str(path
-0000bd10: 292c 2022 2d2d 7079 6922 5d29 0a20 2020  ), "--pyi"]).   
-0000bd20: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0000bd30: 656e 2870 6174 682c 2022 7222 2920 6173  en(path, "r") as
-0000bd40: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
-0000bd50: 2020 2020 2061 6374 7561 6c20 3d20 6668       actual = fh
-0000bd60: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
-0000bd70: 2020 2020 2320 7665 7269 6679 2063 6163      # verify cac
-0000bd80: 6865 2077 6974 6820 2d2d 7079 6920 6973  he with --pyi is
-0000bd90: 2073 6570 6172 6174 650a 2020 2020 2020   separate.      
-0000bda0: 2020 2020 2020 7079 695f 6361 6368 6520        pyi_cache 
-0000bdb0: 3d20 7079 696e 6b2e 7265 6164 5f63 6163  = pyink.read_cac
-0000bdc0: 6865 2870 7969 5f6d 6f64 6529 0a20 2020  he(pyi_mode).   
-0000bdd0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000bde0: 7365 7274 496e 2873 7472 2870 6174 6829  sertIn(str(path)
-0000bdf0: 2c20 7079 695f 6361 6368 6529 0a20 2020  , pyi_cache).   
-0000be00: 2020 2020 2020 2020 206e 6f72 6d61 6c5f           normal_
-0000be10: 6361 6368 6520 3d20 7079 696e 6b2e 7265  cache = pyink.re
-0000be20: 6164 5f63 6163 6865 2844 4546 4155 4c54  ad_cache(DEFAULT
-0000be30: 5f4d 4f44 4529 0a20 2020 2020 2020 2020  _MODE).         
-0000be40: 2020 2073 656c 662e 6173 7365 7274 4e6f     self.assertNo
-0000be50: 7449 6e28 7374 7228 7061 7468 292c 206e  tIn(str(path), n
-0000be60: 6f72 6d61 6c5f 6361 6368 6529 0a20 2020  ormal_cache).   
-0000be70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000be80: 466f 726d 6174 4571 7561 6c28 6578 7065  FormatEqual(expe
-0000be90: 6374 6564 2c20 6163 7475 616c 290a 2020  cted, actual).  
-0000bea0: 2020 2020 2020 7079 696e 6b2e 6173 7365        pyink.asse
-0000beb0: 7274 5f65 7175 6976 616c 656e 7428 636f  rt_equivalent(co
-0000bec0: 6e74 656e 7473 2c20 6163 7475 616c 290a  ntents, actual).
-0000bed0: 2020 2020 2020 2020 7079 696e 6b2e 6173          pyink.as
-0000bee0: 7365 7274 5f73 7461 626c 6528 636f 6e74  sert_stable(cont
-0000bef0: 656e 7473 2c20 6163 7475 616c 2c20 7079  ents, actual, py
-0000bf00: 695f 6d6f 6465 290a 0a20 2020 2040 6576  i_mode)..    @ev
-0000bf10: 656e 745f 6c6f 6f70 2829 0a20 2020 2064  ent_loop().    d
-0000bf20: 6566 2074 6573 745f 6d75 6c74 695f 6669  ef test_multi_fi
-0000bf30: 6c65 5f66 6f72 6365 5f70 7969 2873 656c  le_force_pyi(sel
-0000bf40: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000bf50: 2020 2020 7265 675f 6d6f 6465 203d 2044      reg_mode = D
-0000bf60: 4546 4155 4c54 5f4d 4f44 450a 2020 2020  EFAULT_MODE.    
-0000bf70: 2020 2020 7079 695f 6d6f 6465 203d 2072      pyi_mode = r
-0000bf80: 6570 6c61 6365 2844 4546 4155 4c54 5f4d  eplace(DEFAULT_M
-0000bf90: 4f44 452c 2069 735f 7079 693d 5472 7565  ODE, is_pyi=True
-0000bfa0: 290a 2020 2020 2020 2020 636f 6e74 656e  ).        conten
-0000bfb0: 7473 2c20 6578 7065 6374 6564 203d 2072  ts, expected = r
-0000bfc0: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
-0000bfd0: 6c61 6e65 6f75 7322 2c20 2266 6f72 6365  laneous", "force
-0000bfe0: 5f70 7969 2229 0a20 2020 2020 2020 2077  _pyi").        w
-0000bff0: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
-0000c000: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
-0000c010: 2020 2020 2020 2020 2020 7061 7468 7320            paths 
-0000c020: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0000c030: 2020 2020 2877 6f72 6b73 7061 6365 202f      (workspace /
-0000c040: 2022 6669 6c65 312e 7079 2229 2e72 6573   "file1.py").res
-0000c050: 6f6c 7665 2829 2c0a 2020 2020 2020 2020  olve(),.        
-0000c060: 2020 2020 2020 2020 2877 6f72 6b73 7061          (workspa
-0000c070: 6365 202f 2022 6669 6c65 322e 7079 2229  ce / "file2.py")
-0000c080: 2e72 6573 6f6c 7665 2829 2c0a 2020 2020  .resolve(),.    
-0000c090: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000c0a0: 2020 2020 2020 666f 7220 7061 7468 2069        for path i
-0000c0b0: 6e20 7061 7468 733a 0a20 2020 2020 2020  n paths:.       
-0000c0c0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0000c0d0: 656e 2870 6174 682c 2022 7722 2920 6173  en(path, "w") as
-0000c0e0: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
-0000c0f0: 2020 2020 2020 2020 2066 682e 7772 6974           fh.writ
-0000c100: 6528 636f 6e74 656e 7473 290a 2020 2020  e(contents).    
-0000c110: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
-0000c120: 6f6b 6542 6c61 636b 285b 7374 7228 7029  okeBlack([str(p)
-0000c130: 2066 6f72 2070 2069 6e20 7061 7468 735d   for p in paths]
-0000c140: 202b 205b 222d 2d70 7969 225d 290a 2020   + ["--pyi"]).  
-0000c150: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
-0000c160: 7468 2069 6e20 7061 7468 733a 0a20 2020  th in paths:.   
-0000c170: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000c180: 6820 6f70 656e 2870 6174 682c 2022 7222  h open(path, "r"
-0000c190: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
-0000c1a0: 2020 2020 2020 2020 2020 2020 2061 6374               act
-0000c1b0: 7561 6c20 3d20 6668 2e72 6561 6428 290a  ual = fh.read().
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000c1e0: 2861 6374 7561 6c2c 2065 7870 6563 7465  (actual, expecte
-0000c1f0: 6429 0a20 2020 2020 2020 2020 2020 2023  d).            #
-0000c200: 2076 6572 6966 7920 6361 6368 6520 7769   verify cache wi
-0000c210: 7468 202d 2d70 7969 2069 7320 7365 7061  th --pyi is sepa
-0000c220: 7261 7465 0a20 2020 2020 2020 2020 2020  rate.           
-0000c230: 2070 7969 5f63 6163 6865 203d 2070 7969   pyi_cache = pyi
-0000c240: 6e6b 2e72 6561 645f 6361 6368 6528 7079  nk.read_cache(py
-0000c250: 695f 6d6f 6465 290a 2020 2020 2020 2020  i_mode).        
-0000c260: 2020 2020 6e6f 726d 616c 5f63 6163 6865      normal_cache
-0000c270: 203d 2070 7969 6e6b 2e72 6561 645f 6361   = pyink.read_ca
-0000c280: 6368 6528 7265 675f 6d6f 6465 290a 2020  che(reg_mode).  
-0000c290: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
-0000c2a0: 7468 2069 6e20 7061 7468 733a 0a20 2020  th in paths:.   
-0000c2b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c2c0: 662e 6173 7365 7274 496e 2873 7472 2870  f.assertIn(str(p
-0000c2d0: 6174 6829 2c20 7079 695f 6361 6368 6529  ath), pyi_cache)
-0000c2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c2f0: 2073 656c 662e 6173 7365 7274 4e6f 7449   self.assertNotI
-0000c300: 6e28 7374 7228 7061 7468 292c 206e 6f72  n(str(path), nor
-0000c310: 6d61 6c5f 6361 6368 6529 0a0a 2020 2020  mal_cache)..    
-0000c320: 6465 6620 7465 7374 5f70 6970 655f 666f  def test_pipe_fo
-0000c330: 7263 655f 7079 6928 7365 6c66 2920 2d3e  rce_pyi(self) ->
-0000c340: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-0000c350: 6f75 7263 652c 2065 7870 6563 7465 6420  ource, expected 
-0000c360: 3d20 7265 6164 5f64 6174 6128 226d 6973  = read_data("mis
-0000c370: 6365 6c6c 616e 656f 7573 222c 2022 666f  cellaneous", "fo
-0000c380: 7263 655f 7079 6922 290a 2020 2020 2020  rce_pyi").      
-0000c390: 2020 7265 7375 6c74 203d 2043 6c69 5275    result = CliRu
-0000c3a0: 6e6e 6572 2829 2e69 6e76 6f6b 6528 0a20  nner().invoke(. 
-0000c3b0: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
-0000c3c0: 2e6d 6169 6e2c 205b 222d 222c 2022 2d71  .main, ["-", "-q
-0000c3d0: 222c 2022 2d2d 7079 6922 5d2c 2069 6e70  ", "--pyi"], inp
-0000c3e0: 7574 3d42 7974 6573 494f 2873 6f75 7263  ut=BytesIO(sourc
-0000c3f0: 652e 656e 636f 6465 2822 7574 6638 2229  e.encode("utf8")
-0000c400: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-0000c410: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000c420: 7175 616c 2872 6573 756c 742e 6578 6974  qual(result.exit
-0000c430: 5f63 6f64 652c 2030 290a 2020 2020 2020  _code, 0).      
-0000c440: 2020 6163 7475 616c 203d 2072 6573 756c    actual = resul
-0000c450: 742e 6f75 7470 7574 0a20 2020 2020 2020  t.output.       
-0000c460: 2073 656c 662e 6173 7365 7274 466f 726d   self.assertForm
-0000c470: 6174 4571 7561 6c28 6163 7475 616c 2c20  atEqual(actual, 
-0000c480: 6578 7065 6374 6564 290a 0a20 2020 2064  expected)..    d
-0000c490: 6566 2074 6573 745f 7369 6e67 6c65 5f66  ef test_single_f
-0000c4a0: 696c 655f 666f 7263 655f 7079 3336 2873  ile_force_py36(s
-0000c4b0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000c4c0: 2020 2020 2020 7265 675f 6d6f 6465 203d        reg_mode =
-0000c4d0: 2044 4546 4155 4c54 5f4d 4f44 450a 2020   DEFAULT_MODE.  
-0000c4e0: 2020 2020 2020 7079 3336 5f6d 6f64 6520        py36_mode 
-0000c4f0: 3d20 7265 706c 6163 6528 4445 4641 554c  = replace(DEFAUL
-0000c500: 545f 4d4f 4445 2c20 7461 7267 6574 5f76  T_MODE, target_v
-0000c510: 6572 7369 6f6e 733d 5059 3336 5f56 4552  ersions=PY36_VER
-0000c520: 5349 4f4e 5329 0a20 2020 2020 2020 2073  SIONS).        s
-0000c530: 6f75 7263 652c 2065 7870 6563 7465 6420  ource, expected 
-0000c540: 3d20 7265 6164 5f64 6174 6128 226d 6973  = read_data("mis
-0000c550: 6365 6c6c 616e 656f 7573 222c 2022 666f  cellaneous", "fo
-0000c560: 7263 655f 7079 3336 2229 0a20 2020 2020  rce_py36").     
-0000c570: 2020 2077 6974 6820 6361 6368 655f 6469     with cache_di
-0000c580: 7228 2920 6173 2077 6f72 6b73 7061 6365  r() as workspace
-0000c590: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-0000c5a0: 7468 203d 2028 776f 726b 7370 6163 6520  th = (workspace 
-0000c5b0: 2f20 2266 696c 652e 7079 2229 2e72 6573  / "file.py").res
-0000c5c0: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
-0000c5d0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-0000c5e0: 682c 2022 7722 2920 6173 2066 683a 0a20  h, "w") as fh:. 
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c600: 682e 7772 6974 6528 736f 7572 6365 290a  h.write(source).
-0000c610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c620: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
-0000c630: 7228 7061 7468 292c 202a 5059 3336 5f41  r(path), *PY36_A
-0000c640: 5247 535d 290a 2020 2020 2020 2020 2020  RGS]).          
-0000c650: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
-0000c660: 2c20 2272 2229 2061 7320 6668 3a0a 2020  , "r") as fh:.  
-0000c670: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-0000c680: 7475 616c 203d 2066 682e 7265 6164 2829  tual = fh.read()
-0000c690: 0a20 2020 2020 2020 2020 2020 2023 2076  .            # v
-0000c6a0: 6572 6966 7920 6361 6368 6520 7769 7468  erify cache with
-0000c6b0: 202d 2d74 6172 6765 742d 7665 7273 696f   --target-versio
-0000c6c0: 6e20 6973 2073 6570 6172 6174 650a 2020  n is separate.  
-0000c6d0: 2020 2020 2020 2020 2020 7079 3336 5f63            py36_c
-0000c6e0: 6163 6865 203d 2070 7969 6e6b 2e72 6561  ache = pyink.rea
-0000c6f0: 645f 6361 6368 6528 7079 3336 5f6d 6f64  d_cache(py36_mod
-0000c700: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-0000c710: 656c 662e 6173 7365 7274 496e 2873 7472  elf.assertIn(str
-0000c720: 2870 6174 6829 2c20 7079 3336 5f63 6163  (path), py36_cac
-0000c730: 6865 290a 2020 2020 2020 2020 2020 2020  he).            
-0000c740: 6e6f 726d 616c 5f63 6163 6865 203d 2070  normal_cache = p
-0000c750: 7969 6e6b 2e72 6561 645f 6361 6368 6528  yink.read_cache(
-0000c760: 7265 675f 6d6f 6465 290a 2020 2020 2020  reg_mode).      
-0000c770: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000c780: 744e 6f74 496e 2873 7472 2870 6174 6829  tNotIn(str(path)
-0000c790: 2c20 6e6f 726d 616c 5f63 6163 6865 290a  , normal_cache).
-0000c7a0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000c7b0: 6572 7445 7175 616c 2861 6374 7561 6c2c  ertEqual(actual,
-0000c7c0: 2065 7870 6563 7465 6429 0a0a 2020 2020   expected)..    
-0000c7d0: 4065 7665 6e74 5f6c 6f6f 7028 290a 2020  @event_loop().  
-0000c7e0: 2020 6465 6620 7465 7374 5f6d 756c 7469    def test_multi
-0000c7f0: 5f66 696c 655f 666f 7263 655f 7079 3336  _file_force_py36
-0000c800: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000c810: 2020 2020 2020 2020 7265 675f 6d6f 6465          reg_mode
-0000c820: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
-0000c830: 2020 2020 2020 2020 7079 3336 5f6d 6f64          py36_mod
-0000c840: 6520 3d20 7265 706c 6163 6528 4445 4641  e = replace(DEFA
-0000c850: 554c 545f 4d4f 4445 2c20 7461 7267 6574  ULT_MODE, target
-0000c860: 5f76 6572 7369 6f6e 733d 5059 3336 5f56  _versions=PY36_V
-0000c870: 4552 5349 4f4e 5329 0a20 2020 2020 2020  ERSIONS).       
-0000c880: 2073 6f75 7263 652c 2065 7870 6563 7465   source, expecte
-0000c890: 6420 3d20 7265 6164 5f64 6174 6128 226d  d = read_data("m
-0000c8a0: 6973 6365 6c6c 616e 656f 7573 222c 2022  iscellaneous", "
-0000c8b0: 666f 7263 655f 7079 3336 2229 0a20 2020  force_py36").   
-0000c8c0: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
-0000c8d0: 6469 7228 2920 6173 2077 6f72 6b73 7061  dir() as workspa
-0000c8e0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-0000c8f0: 7061 7468 7320 3d20 5b0a 2020 2020 2020  paths = [.      
-0000c900: 2020 2020 2020 2020 2020 2877 6f72 6b73            (works
-0000c910: 7061 6365 202f 2022 6669 6c65 312e 7079  pace / "file1.py
-0000c920: 2229 2e72 6573 6f6c 7665 2829 2c0a 2020  ").resolve(),.  
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2877                (w
-0000c940: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
-0000c950: 322e 7079 2229 2e72 6573 6f6c 7665 2829  2.py").resolve()
-0000c960: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
-0000c970: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000c980: 7061 7468 2069 6e20 7061 7468 733a 0a20  path in paths:. 
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000c9a0: 6974 6820 6f70 656e 2870 6174 682c 2022  ith open(path, "
-0000c9b0: 7722 2920 6173 2066 683a 0a20 2020 2020  w") as fh:.     
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c9d0: 682e 7772 6974 6528 736f 7572 6365 290a  h.write(source).
-0000c9e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c9f0: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
-0000ca00: 7228 7029 2066 6f72 2070 2069 6e20 7061  r(p) for p in pa
-0000ca10: 7468 735d 202b 2050 5933 365f 4152 4753  ths] + PY36_ARGS
-0000ca20: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000ca30: 7220 7061 7468 2069 6e20 7061 7468 733a  r path in paths:
-0000ca40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca50: 2077 6974 6820 6f70 656e 2870 6174 682c   with open(path,
-0000ca60: 2022 7222 2920 6173 2066 683a 0a20 2020   "r") as fh:.   
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2061 6374 7561 6c20 3d20 6668 2e72 6561   actual = fh.rea
-0000ca90: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000caa0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000cab0: 7175 616c 2861 6374 7561 6c2c 2065 7870  qual(actual, exp
-0000cac0: 6563 7465 6429 0a20 2020 2020 2020 2020  ected).         
-0000cad0: 2020 2023 2076 6572 6966 7920 6361 6368     # verify cach
-0000cae0: 6520 7769 7468 202d 2d74 6172 6765 742d  e with --target-
-0000caf0: 7665 7273 696f 6e20 6973 2073 6570 6172  version is separ
-0000cb00: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-0000cb10: 7079 695f 6361 6368 6520 3d20 7079 696e  pyi_cache = pyin
-0000cb20: 6b2e 7265 6164 5f63 6163 6865 2870 7933  k.read_cache(py3
-0000cb30: 365f 6d6f 6465 290a 2020 2020 2020 2020  6_mode).        
-0000cb40: 2020 2020 6e6f 726d 616c 5f63 6163 6865      normal_cache
-0000cb50: 203d 2070 7969 6e6b 2e72 6561 645f 6361   = pyink.read_ca
-0000cb60: 6368 6528 7265 675f 6d6f 6465 290a 2020  che(reg_mode).  
-0000cb70: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
-0000cb80: 7468 2069 6e20 7061 7468 733a 0a20 2020  th in paths:.   
-0000cb90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000cba0: 662e 6173 7365 7274 496e 2873 7472 2870  f.assertIn(str(p
-0000cbb0: 6174 6829 2c20 7079 695f 6361 6368 6529  ath), pyi_cache)
-0000cbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbd0: 2073 656c 662e 6173 7365 7274 4e6f 7449   self.assertNotI
-0000cbe0: 6e28 7374 7228 7061 7468 292c 206e 6f72  n(str(path), nor
-0000cbf0: 6d61 6c5f 6361 6368 6529 0a0a 2020 2020  mal_cache)..    
-0000cc00: 6465 6620 7465 7374 5f70 6970 655f 666f  def test_pipe_fo
-0000cc10: 7263 655f 7079 3336 2873 656c 6629 202d  rce_py36(self) -
-0000cc20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000cc30: 736f 7572 6365 2c20 6578 7065 6374 6564  source, expected
-0000cc40: 203d 2072 6561 645f 6461 7461 2822 6d69   = read_data("mi
-0000cc50: 7363 656c 6c61 6e65 6f75 7322 2c20 2266  scellaneous", "f
-0000cc60: 6f72 6365 5f70 7933 3622 290a 2020 2020  orce_py36").    
-0000cc70: 2020 2020 7265 7375 6c74 203d 2043 6c69      result = Cli
-0000cc80: 5275 6e6e 6572 2829 2e69 6e76 6f6b 6528  Runner().invoke(
-0000cc90: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
-0000cca0: 6e6b 2e6d 6169 6e2c 0a20 2020 2020 2020  nk.main,.       
-0000ccb0: 2020 2020 205b 222d 222c 2022 2d71 222c       ["-", "-q",
-0000ccc0: 2022 2d2d 7461 7267 6574 2d76 6572 7369   "--target-versi
-0000ccd0: 6f6e 3d70 7933 3622 5d2c 0a20 2020 2020  on=py36"],.     
-0000cce0: 2020 2020 2020 2069 6e70 7574 3d42 7974         input=Byt
-0000ccf0: 6573 494f 2873 6f75 7263 652e 656e 636f  esIO(source.enco
-0000cd00: 6465 2822 7574 6638 2229 292c 0a20 2020  de("utf8")),.   
-0000cd10: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0000cd20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000cd30: 7265 7375 6c74 2e65 7869 745f 636f 6465  result.exit_code
-0000cd40: 2c20 3029 0a20 2020 2020 2020 2061 6374  , 0).        act
-0000cd50: 7561 6c20 3d20 7265 7375 6c74 2e6f 7574  ual = result.out
-0000cd60: 7075 740a 2020 2020 2020 2020 7365 6c66  put.        self
-0000cd70: 2e61 7373 6572 7446 6f72 6d61 7445 7175  .assertFormatEqu
-0000cd80: 616c 2861 6374 7561 6c2c 2065 7870 6563  al(actual, expec
-0000cd90: 7465 6429 0a0a 2020 2020 4070 7974 6573  ted)..    @pytes
-0000cda0: 742e 6d61 726b 2e69 6e63 6f6d 7061 7469  t.mark.incompati
-0000cdb0: 626c 655f 7769 7468 5f6d 7970 7963 0a20  ble_with_mypyc. 
-0000cdc0: 2020 2064 6566 2074 6573 745f 7265 666f     def test_refo
-0000cdd0: 726d 6174 5f6f 6e65 5f77 6974 685f 7374  rmat_one_with_st
-0000cde0: 6469 6e28 7365 6c66 2920 2d3e 204e 6f6e  din(self) -> Non
-0000cdf0: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
-0000ce00: 7061 7463 6828 0a20 2020 2020 2020 2020  patch(.         
-0000ce10: 2020 2022 7079 696e 6b2e 666f 726d 6174     "pyink.format
-0000ce20: 5f73 7464 696e 5f74 6f5f 7374 646f 7574  _stdin_to_stdout
-0000ce30: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
-0000ce40: 6574 7572 6e5f 7661 6c75 653d 6c61 6d62  eturn_value=lamb
-0000ce50: 6461 202a 6172 6773 2c20 2a2a 6b77 6172  da *args, **kwar
-0000ce60: 6773 3a20 7079 696e 6b2e 4368 616e 6765  gs: pyink.Change
-0000ce70: 642e 5945 532c 0a20 2020 2020 2020 2029  d.YES,.        )
-0000ce80: 2061 7320 6673 7473 3a0a 2020 2020 2020   as fsts:.      
-0000ce90: 2020 2020 2020 7265 706f 7274 203d 204d        report = M
-0000cea0: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-0000ceb0: 2020 2020 2020 2070 6174 6820 3d20 5061         path = Pa
-0000cec0: 7468 2822 2d22 290a 2020 2020 2020 2020  th("-").        
-0000ced0: 2020 2020 7079 696e 6b2e 7265 666f 726d      pyink.reform
-0000cee0: 6174 5f6f 6e65 280a 2020 2020 2020 2020  at_one(.        
-0000cef0: 2020 2020 2020 2020 7061 7468 2c0a 2020          path,.  
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-0000cf10: 7374 3d54 7275 652c 0a20 2020 2020 2020  st=True,.       
-0000cf20: 2020 2020 2020 2020 2077 7269 7465 5f62           write_b
-0000cf30: 6163 6b3d 7079 696e 6b2e 5772 6974 6542  ack=pyink.WriteB
-0000cf40: 6163 6b2e 5945 532c 0a20 2020 2020 2020  ack.YES,.       
-0000cf50: 2020 2020 2020 2020 206d 6f64 653d 4445           mode=DE
-0000cf60: 4641 554c 545f 4d4f 4445 2c0a 2020 2020  FAULT_MODE,.    
-0000cf70: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-0000cf80: 7274 3d72 6570 6f72 742c 0a20 2020 2020  rt=report,.     
-0000cf90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000cfa0: 2020 2020 2066 7374 732e 6173 7365 7274       fsts.assert
-0000cfb0: 5f63 616c 6c65 645f 6f6e 6365 2829 0a20  _called_once(). 
-0000cfc0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-0000cfd0: 742e 646f 6e65 2e61 7373 6572 745f 6361  t.done.assert_ca
-0000cfe0: 6c6c 6564 5f77 6974 6828 7061 7468 2c20  lled_with(path, 
-0000cff0: 7079 696e 6b2e 4368 616e 6765 642e 5945  pyink.Changed.YE
-0000d000: 5329 0a0a 2020 2020 4070 7974 6573 742e  S)..    @pytest.
-0000d010: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
-0000d020: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
-0000d030: 2064 6566 2074 6573 745f 7265 666f 726d   def test_reform
-0000d040: 6174 5f6f 6e65 5f77 6974 685f 7374 6469  at_one_with_stdi
-0000d050: 6e5f 6669 6c65 6e61 6d65 2873 656c 6629  n_filename(self)
-0000d060: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000d070: 2020 7769 7468 2070 6174 6368 280a 2020    with patch(.  
-0000d080: 2020 2020 2020 2020 2020 2270 7969 6e6b            "pyink
-0000d090: 2e66 6f72 6d61 745f 7374 6469 6e5f 746f  .format_stdin_to
-0000d0a0: 5f73 7464 6f75 7422 2c0a 2020 2020 2020  _stdout",.      
-0000d0b0: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
-0000d0c0: 7565 3d6c 616d 6264 6120 2a61 7267 732c  ue=lambda *args,
-0000d0d0: 202a 2a6b 7761 7267 733a 2070 7969 6e6b   **kwargs: pyink
-0000d0e0: 2e43 6861 6e67 6564 2e59 4553 2c0a 2020  .Changed.YES,.  
-0000d0f0: 2020 2020 2020 2920 6173 2066 7374 733a        ) as fsts:
-0000d100: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000d110: 6f72 7420 3d20 4d61 6769 634d 6f63 6b28  ort = MagicMock(
-0000d120: 290a 2020 2020 2020 2020 2020 2020 7020  ).            p 
-0000d130: 3d20 2266 6f6f 2e70 7922 0a20 2020 2020  = "foo.py".     
-0000d140: 2020 2020 2020 2070 6174 6820 3d20 5061         path = Pa
-0000d150: 7468 2866 225f 5f50 5949 4e4b 5f53 5444  th(f"__PYINK_STD
-0000d160: 494e 5f46 494c 454e 414d 455f 5f7b 707d  IN_FILENAME__{p}
-0000d170: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000d180: 7870 6563 7465 6420 3d20 5061 7468 2870  xpected = Path(p
-0000d190: 290a 2020 2020 2020 2020 2020 2020 7079  ).            py
-0000d1a0: 696e 6b2e 7265 666f 726d 6174 5f6f 6e65  ink.reformat_one
-0000d1b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d1c0: 2020 7061 7468 2c0a 2020 2020 2020 2020    path,.        
-0000d1d0: 2020 2020 2020 2020 6661 7374 3d54 7275          fast=Tru
-0000d1e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000d1f0: 2020 2077 7269 7465 5f62 6163 6b3d 7079     write_back=py
-0000d200: 696e 6b2e 5772 6974 6542 6163 6b2e 5945  ink.WriteBack.YE
-0000d210: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
-0000d220: 2020 206d 6f64 653d 4445 4641 554c 545f     mode=DEFAULT_
-0000d230: 4d4f 4445 2c0a 2020 2020 2020 2020 2020  MODE,.          
-0000d240: 2020 2020 2020 7265 706f 7274 3d72 6570        report=rep
-0000d250: 6f72 742c 0a20 2020 2020 2020 2020 2020  ort,.           
-0000d260: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0000d270: 7374 732e 6173 7365 7274 5f63 616c 6c65  sts.assert_calle
-0000d280: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
-0000d290: 2020 2020 2020 2020 2020 2020 2066 6173               fas
-0000d2a0: 743d 5472 7565 2c20 7772 6974 655f 6261  t=True, write_ba
-0000d2b0: 636b 3d70 7969 6e6b 2e57 7269 7465 4261  ck=pyink.WriteBa
-0000d2c0: 636b 2e59 4553 2c20 6d6f 6465 3d44 4546  ck.YES, mode=DEF
-0000d2d0: 4155 4c54 5f4d 4f44 452c 206c 696e 6573  AULT_MODE, lines
-0000d2e0: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-0000d2f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000d300: 2320 5f5f 5059 494e 4b5f 5354 4449 4e5f  # __PYINK_STDIN_
-0000d310: 4649 4c45 4e41 4d45 5f5f 2073 686f 756c  FILENAME__ shoul
-0000d320: 6420 6861 7665 2062 6565 6e20 7374 7269  d have been stri
-0000d330: 7070 6564 0a20 2020 2020 2020 2020 2020  pped.           
-0000d340: 2072 6570 6f72 742e 646f 6e65 2e61 7373   report.done.ass
-0000d350: 6572 745f 6361 6c6c 6564 5f77 6974 6828  ert_called_with(
-0000d360: 6578 7065 6374 6564 2c20 7079 696e 6b2e  expected, pyink.
-0000d370: 4368 616e 6765 642e 5945 5329 0a0a 2020  Changed.YES)..  
-0000d380: 2020 4070 7974 6573 742e 6d61 726b 2e69    @pytest.mark.i
-0000d390: 6e63 6f6d 7061 7469 626c 655f 7769 7468  ncompatible_with
-0000d3a0: 5f6d 7970 7963 0a20 2020 2064 6566 2074  _mypyc.    def t
-0000d3b0: 6573 745f 7265 666f 726d 6174 5f6f 6e65  est_reformat_one
-0000d3c0: 5f77 6974 685f 7374 6469 6e5f 6669 6c65  _with_stdin_file
-0000d3d0: 6e61 6d65 5f70 7969 2873 656c 6629 202d  name_pyi(self) -
-0000d3e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000d3f0: 7769 7468 2070 6174 6368 280a 2020 2020  with patch(.    
-0000d400: 2020 2020 2020 2020 2270 7969 6e6b 2e66          "pyink.f
-0000d410: 6f72 6d61 745f 7374 6469 6e5f 746f 5f73  ormat_stdin_to_s
-0000d420: 7464 6f75 7422 2c0a 2020 2020 2020 2020  tdout",.        
-0000d430: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
-0000d440: 3d6c 616d 6264 6120 2a61 7267 732c 202a  =lambda *args, *
-0000d450: 2a6b 7761 7267 733a 2070 7969 6e6b 2e43  *kwargs: pyink.C
-0000d460: 6861 6e67 6564 2e59 4553 2c0a 2020 2020  hanged.YES,.    
-0000d470: 2020 2020 2920 6173 2066 7374 733a 0a20      ) as fsts:. 
-0000d480: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-0000d490: 7420 3d20 4d61 6769 634d 6f63 6b28 290a  t = MagicMock().
-0000d4a0: 2020 2020 2020 2020 2020 2020 7020 3d20              p = 
-0000d4b0: 2266 6f6f 2e70 7969 220a 2020 2020 2020  "foo.pyi".      
-0000d4c0: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
-0000d4d0: 6828 6622 5f5f 5059 494e 4b5f 5354 4449  h(f"__PYINK_STDI
-0000d4e0: 4e5f 4649 4c45 4e41 4d45 5f5f 7b70 7d22  N_FILENAME__{p}"
-0000d4f0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0000d500: 7065 6374 6564 203d 2050 6174 6828 7029  pected = Path(p)
-0000d510: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
-0000d520: 6e6b 2e72 6566 6f72 6d61 745f 6f6e 6528  nk.reformat_one(
-0000d530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d540: 2070 6174 682c 0a20 2020 2020 2020 2020   path,.         
-0000d550: 2020 2020 2020 2066 6173 743d 5472 7565         fast=True
-0000d560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d570: 2020 7772 6974 655f 6261 636b 3d70 7969    write_back=pyi
-0000d580: 6e6b 2e57 7269 7465 4261 636b 2e59 4553  nk.WriteBack.YES
-0000d590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d5a0: 2020 6d6f 6465 3d44 4546 4155 4c54 5f4d    mode=DEFAULT_M
-0000d5b0: 4f44 452c 0a20 2020 2020 2020 2020 2020  ODE,.           
-0000d5c0: 2020 2020 2072 6570 6f72 743d 7265 706f       report=repo
-0000d5d0: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
-0000d5e0: 290a 2020 2020 2020 2020 2020 2020 6673  ).            fs
-0000d5f0: 7473 2e61 7373 6572 745f 6361 6c6c 6564  ts.assert_called
-0000d600: 5f6f 6e63 655f 7769 7468 280a 2020 2020  _once_with(.    
-0000d610: 2020 2020 2020 2020 2020 2020 6661 7374              fast
-0000d620: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-0000d630: 2020 2020 2020 2077 7269 7465 5f62 6163         write_bac
-0000d640: 6b3d 7079 696e 6b2e 5772 6974 6542 6163  k=pyink.WriteBac
-0000d650: 6b2e 5945 532c 0a20 2020 2020 2020 2020  k.YES,.         
-0000d660: 2020 2020 2020 206d 6f64 653d 7265 706c         mode=repl
-0000d670: 6163 6528 4445 4641 554c 545f 4d4f 4445  ace(DEFAULT_MODE
-0000d680: 2c20 6973 5f70 7969 3d54 7275 6529 2c0a  , is_pyi=True),.
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6a0: 6c69 6e65 733d 4e6f 6e65 2c0a 2020 2020  lines=None,.    
-0000d6b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d6c0: 2020 2020 2020 2320 5f5f 5059 494e 4b5f        # __PYINK_
-0000d6d0: 5354 4449 4e5f 4649 4c45 4e41 4d45 5f5f  STDIN_FILENAME__
-0000d6e0: 2073 686f 756c 6420 6861 7665 2062 6565   should have bee
-0000d6f0: 6e20 7374 7269 7070 6564 0a20 2020 2020  n stripped.     
-0000d700: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
-0000d710: 6e65 2e61 7373 6572 745f 6361 6c6c 6564  ne.assert_called
-0000d720: 5f77 6974 6828 6578 7065 6374 6564 2c20  _with(expected, 
-0000d730: 7079 696e 6b2e 4368 616e 6765 642e 5945  pyink.Changed.YE
-0000d740: 5329 0a0a 2020 2020 4070 7974 6573 742e  S)..    @pytest.
-0000d750: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
-0000d760: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
-0000d770: 2064 6566 2074 6573 745f 7265 666f 726d   def test_reform
-0000d780: 6174 5f6f 6e65 5f77 6974 685f 7374 6469  at_one_with_stdi
-0000d790: 6e5f 6669 6c65 6e61 6d65 5f69 7079 6e62  n_filename_ipynb
-0000d7a0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000d7b0: 2020 2020 2020 2020 7769 7468 2070 6174          with pat
-0000d7c0: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
-0000d7d0: 2270 7969 6e6b 2e66 6f72 6d61 745f 7374  "pyink.format_st
-0000d7e0: 6469 6e5f 746f 5f73 7464 6f75 7422 2c0a  din_to_stdout",.
-0000d7f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d800: 726e 5f76 616c 7565 3d6c 616d 6264 6120  rn_value=lambda 
-0000d810: 2a61 7267 732c 202a 2a6b 7761 7267 733a  *args, **kwargs:
-0000d820: 2070 7969 6e6b 2e43 6861 6e67 6564 2e59   pyink.Changed.Y
-0000d830: 4553 2c0a 2020 2020 2020 2020 2920 6173  ES,.        ) as
-0000d840: 2066 7374 733a 0a20 2020 2020 2020 2020   fsts:.         
-0000d850: 2020 2072 6570 6f72 7420 3d20 4d61 6769     report = Magi
-0000d860: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
-0000d870: 2020 2020 7020 3d20 2266 6f6f 2e69 7079      p = "foo.ipy
-0000d880: 6e62 220a 2020 2020 2020 2020 2020 2020  nb".            
-0000d890: 7061 7468 203d 2050 6174 6828 6622 5f5f  path = Path(f"__
-0000d8a0: 5059 494e 4b5f 5354 4449 4e5f 4649 4c45  PYINK_STDIN_FILE
-0000d8b0: 4e41 4d45 5f5f 7b70 7d22 290a 2020 2020  NAME__{p}").    
-0000d8c0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0000d8d0: 203d 2050 6174 6828 7029 0a20 2020 2020   = Path(p).     
-0000d8e0: 2020 2020 2020 2070 7969 6e6b 2e72 6566         pyink.ref
-0000d8f0: 6f72 6d61 745f 6f6e 6528 0a20 2020 2020  ormat_one(.     
-0000d900: 2020 2020 2020 2020 2020 2070 6174 682c             path,
-0000d910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d920: 2066 6173 743d 5472 7565 2c0a 2020 2020   fast=True,.    
-0000d930: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-0000d940: 655f 6261 636b 3d70 7969 6e6b 2e57 7269  e_back=pyink.Wri
-0000d950: 7465 4261 636b 2e59 4553 2c0a 2020 2020  teBack.YES,.    
-0000d960: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0000d970: 3d44 4546 4155 4c54 5f4d 4f44 452c 0a20  =DEFAULT_MODE,. 
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d990: 6570 6f72 743d 7265 706f 7274 2c0a 2020  eport=report,.  
-0000d9a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d9b0: 2020 2020 2020 2020 6673 7473 2e61 7373          fsts.ass
-0000d9c0: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
-0000d9d0: 7769 7468 280a 2020 2020 2020 2020 2020  with(.          
-0000d9e0: 2020 2020 2020 6661 7374 3d54 7275 652c        fast=True,
-0000d9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da00: 2077 7269 7465 5f62 6163 6b3d 7079 696e   write_back=pyin
-0000da10: 6b2e 5772 6974 6542 6163 6b2e 5945 532c  k.WriteBack.YES,
-0000da20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da30: 206d 6f64 653d 7265 706c 6163 6528 4445   mode=replace(DE
-0000da40: 4641 554c 545f 4d4f 4445 2c20 6973 5f69  FAULT_MODE, is_i
-0000da50: 7079 6e62 3d54 7275 6529 2c0a 2020 2020  pynb=True),.    
-0000da60: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000da70: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0000da80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000da90: 2020 2320 5f5f 5059 494e 4b5f 5354 4449    # __PYINK_STDI
-0000daa0: 4e5f 4649 4c45 4e41 4d45 5f5f 2073 686f  N_FILENAME__ sho
-0000dab0: 756c 6420 6861 7665 2062 6565 6e20 7374  uld have been st
-0000dac0: 7269 7070 6564 0a20 2020 2020 2020 2020  ripped.         
-0000dad0: 2020 2072 6570 6f72 742e 646f 6e65 2e61     report.done.a
-0000dae0: 7373 6572 745f 6361 6c6c 6564 5f77 6974  ssert_called_wit
-0000daf0: 6828 6578 7065 6374 6564 2c20 7079 696e  h(expected, pyin
-0000db00: 6b2e 4368 616e 6765 642e 5945 5329 0a0a  k.Changed.YES)..
-0000db10: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000db20: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
-0000db30: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
-0000db40: 2074 6573 745f 7265 666f 726d 6174 5f6f   test_reformat_o
-0000db50: 6e65 5f77 6974 685f 7374 6469 6e5f 616e  ne_with_stdin_an
-0000db60: 645f 6578 6973 7469 6e67 5f70 6174 6828  d_existing_path(
-0000db70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000db80: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
-0000db90: 6828 0a20 2020 2020 2020 2020 2020 2022  h(.            "
-0000dba0: 7079 696e 6b2e 666f 726d 6174 5f73 7464  pyink.format_std
-0000dbb0: 696e 5f74 6f5f 7374 646f 7574 222c 0a20  in_to_stdout",. 
-0000dbc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dbd0: 6e5f 7661 6c75 653d 6c61 6d62 6461 202a  n_value=lambda *
-0000dbe0: 6172 6773 2c20 2a2a 6b77 6172 6773 3a20  args, **kwargs: 
-0000dbf0: 7079 696e 6b2e 4368 616e 6765 642e 5945  pyink.Changed.YE
-0000dc00: 532c 0a20 2020 2020 2020 2029 2061 7320  S,.        ) as 
-0000dc10: 6673 7473 3a0a 2020 2020 2020 2020 2020  fsts:.          
-0000dc20: 2020 7265 706f 7274 203d 204d 6167 6963    report = Magic
-0000dc30: 4d6f 636b 2829 0a20 2020 2020 2020 2020  Mock().         
-0000dc40: 2020 2023 2045 7665 6e20 7769 7468 2061     # Even with a
-0000dc50: 6e20 6578 6973 7469 6e67 2066 696c 652c  n existing file,
-0000dc60: 2073 696e 6365 2077 6520 6172 6520 666f   since we are fo
-0000dc70: 7263 696e 6720 7374 6469 6e2c 2062 6c61  rcing stdin, bla
-0000dc80: 636b 0a20 2020 2020 2020 2020 2020 2023  ck.            #
-0000dc90: 2073 686f 756c 6420 6f75 7470 7574 2074   should output t
-0000dca0: 6f20 7374 646f 7574 2061 6e64 206e 6f74  o stdout and not
-0000dcb0: 206d 6f64 6966 7920 7468 6520 6669 6c65   modify the file
-0000dcc0: 2069 6e70 6c61 6365 0a20 2020 2020 2020   inplace.       
-0000dcd0: 2020 2020 2070 203d 2054 4849 535f 4449       p = THIS_DI
-0000dce0: 5220 2f20 2264 6174 6122 202f 2022 7369  R / "data" / "si
-0000dcf0: 6d70 6c65 5f63 6173 6573 2220 2f20 2263  mple_cases" / "c
-0000dd00: 6f6c 6c65 6374 696f 6e73 2e70 7922 0a20  ollections.py". 
-0000dd10: 2020 2020 2020 2020 2020 2023 204d 616b             # Mak
-0000dd20: 6520 7375 7265 2069 735f 6669 6c65 2061  e sure is_file a
-0000dd30: 6374 7561 6c6c 7920 7265 7475 726e 7320  ctually returns 
-0000dd40: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000dd50: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0000dd60: 2870 2e69 735f 6669 6c65 2829 290a 2020  (p.is_file()).  
-0000dd70: 2020 2020 2020 2020 2020 7061 7468 203d            path =
-0000dd80: 2050 6174 6828 6622 5f5f 5059 494e 4b5f   Path(f"__PYINK_
-0000dd90: 5354 4449 4e5f 4649 4c45 4e41 4d45 5f5f  STDIN_FILENAME__
-0000dda0: 7b70 7d22 290a 2020 2020 2020 2020 2020  {p}").          
-0000ddb0: 2020 6578 7065 6374 6564 203d 2050 6174    expected = Pat
-0000ddc0: 6828 7029 0a20 2020 2020 2020 2020 2020  h(p).           
-0000ddd0: 2070 7969 6e6b 2e72 6566 6f72 6d61 745f   pyink.reformat_
-0000dde0: 6f6e 6528 0a20 2020 2020 2020 2020 2020  one(.           
-0000ddf0: 2020 2020 2070 6174 682c 0a20 2020 2020       path,.     
-0000de00: 2020 2020 2020 2020 2020 2066 6173 743d             fast=
-0000de10: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000de20: 2020 2020 2020 7772 6974 655f 6261 636b        write_back
-0000de30: 3d70 7969 6e6b 2e57 7269 7465 4261 636b  =pyink.WriteBack
-0000de40: 2e59 4553 2c0a 2020 2020 2020 2020 2020  .YES,.          
-0000de50: 2020 2020 2020 6d6f 6465 3d44 4546 4155        mode=DEFAU
-0000de60: 4c54 5f4d 4f44 452c 0a20 2020 2020 2020  LT_MODE,.       
-0000de70: 2020 2020 2020 2020 2072 6570 6f72 743d           report=
-0000de80: 7265 706f 7274 2c0a 2020 2020 2020 2020  report,.        
-0000de90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000dea0: 2020 6673 7473 2e61 7373 6572 745f 6361    fsts.assert_ca
-0000deb0: 6c6c 6564 5f6f 6e63 6528 290a 2020 2020  lled_once().    
-0000dec0: 2020 2020 2020 2020 2320 5f5f 5059 494e          # __PYIN
-0000ded0: 4b5f 5354 4449 4e5f 4649 4c45 4e41 4d45  K_STDIN_FILENAME
-0000dee0: 5f5f 2073 686f 756c 6420 6861 7665 2062  __ should have b
-0000def0: 6565 6e20 7374 7269 7070 6564 0a20 2020  een stripped.   
-0000df00: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
-0000df10: 646f 6e65 2e61 7373 6572 745f 6361 6c6c  done.assert_call
-0000df20: 6564 5f77 6974 6828 6578 7065 6374 6564  ed_with(expected
-0000df30: 2c20 7079 696e 6b2e 4368 616e 6765 642e  , pyink.Changed.
-0000df40: 5945 5329 0a0a 2020 2020 6465 6620 7465  YES)..    def te
-0000df50: 7374 5f72 6566 6f72 6d61 745f 6f6e 655f  st_reformat_one_
-0000df60: 7769 7468 5f73 7464 696e 5f65 6d70 7479  with_stdin_empty
-0000df70: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000df80: 2020 2020 2020 2020 6361 7365 7320 3d20          cases = 
-0000df90: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
-0000dfa0: 222c 2022 2229 2c0a 2020 2020 2020 2020  ", ""),.        
-0000dfb0: 2020 2020 2822 5c6e 222c 2022 5c6e 2229      ("\n", "\n")
-0000dfc0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-0000dfd0: 5c72 5c6e 222c 2022 5c72 5c6e 2229 2c0a  \r\n", "\r\n"),.
-0000dfe0: 2020 2020 2020 2020 2020 2020 2822 205c              (" \
-0000dff0: 7422 2c20 2222 292c 0a20 2020 2020 2020  t", ""),.       
-0000e000: 2020 2020 2028 2220 5c74 5c6e 5c74 2022       (" \t\n\t "
-0000e010: 2c20 225c 6e22 292c 0a20 2020 2020 2020  , "\n"),.       
-0000e020: 2020 2020 2028 2220 5c74 5c72 5c6e 5c74       (" \t\r\n\t
-0000e030: 2022 2c20 225c 725c 6e22 292c 0a20 2020   ", "\r\n"),.   
-0000e040: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
-0000e050: 6465 6620 5f6e 6577 5f77 7261 7070 6572  def _new_wrapper
-0000e060: 280a 2020 2020 2020 2020 2020 2020 6f75  (.            ou
-0000e070: 7470 7574 3a20 696f 2e53 7472 696e 6749  tput: io.StringI
-0000e080: 4f2c 2069 6f5f 5465 7874 494f 5772 6170  O, io_TextIOWrap
-0000e090: 7065 723a 2054 7970 655b 696f 2e54 6578  per: Type[io.Tex
-0000e0a0: 7449 4f57 7261 7070 6572 5d0a 2020 2020  tIOWrapper].    
-0000e0b0: 2020 2020 2920 2d3e 2043 616c 6c61 626c      ) -> Callabl
-0000e0c0: 655b 5b41 6e79 2c20 416e 795d 2c20 696f  e[[Any, Any], io
-0000e0d0: 2e54 6578 7449 4f57 7261 7070 6572 5d3a  .TextIOWrapper]:
-0000e0e0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-0000e0f0: 2067 6574 5f6f 7574 7075 7428 2a61 7267   get_output(*arg
-0000e100: 733a 2041 6e79 2c20 2a2a 6b77 6172 6773  s: Any, **kwargs
-0000e110: 3a20 416e 7929 202d 3e20 696f 2e54 6578  : Any) -> io.Tex
-0000e120: 7449 4f57 7261 7070 6572 3a0a 2020 2020  tIOWrapper:.    
-0000e130: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000e140: 7267 7320 3d3d 2028 7379 732e 7374 646f  rgs == (sys.stdo
-0000e150: 7574 2e62 7566 6665 722c 293a 0a20 2020  ut.buffer,):.   
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2023 2049 7427 7320 6066 6f72 6d61 745f   # It's `format_
-0000e180: 7374 6469 6e5f 746f 5f73 7464 6f75 7428  stdin_to_stdout(
-0000e190: 2960 2063 616c 6c69 6e67 2060 696f 2e54  )` calling `io.T
-0000e1a0: 6578 7449 4f57 7261 7070 6572 2829 602c  extIOWrapper()`,
-0000e1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e1c0: 2020 2020 2023 2072 6574 7572 6e20 6f75       # return ou
-0000e1d0: 7220 6d6f 636b 206f 626a 6563 742e 0a20  r mock object.. 
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
-0000e200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e210: 2023 2049 7427 7320 736f 6d65 7468 696e   # It's somethin
-0000e220: 6720 656c 7365 2028 692e 652e 2060 6465  g else (i.e. `de
-0000e230: 636f 6465 5f62 7974 6573 2829 6029 2063  code_bytes()`) c
-0000e240: 616c 6c69 6e67 0a20 2020 2020 2020 2020  alling.         
-0000e250: 2020 2020 2020 2023 2060 696f 2e54 6578         # `io.Tex
-0000e260: 7449 4f57 7261 7070 6572 2829 602c 2070  tIOWrapper()`, p
-0000e270: 6173 7320 7468 726f 7567 6820 746f 2074  ass through to t
-0000e280: 6865 206f 7269 6769 6e61 6c20 696d 706c  he original impl
-0000e290: 656d 656e 7461 7469 6f6e 2e0a 2020 2020  ementation..    
-0000e2a0: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
-0000e2b0: 6520 6469 7363 7573 7369 6f6e 2069 6e20  e discussion in 
-0000e2c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000e2d0: 6f6d 2f70 7366 2f62 6c61 636b 2f70 756c  om/psf/black/pul
-0000e2e0: 6c2f 3234 3839 0a20 2020 2020 2020 2020  l/2489.         
-0000e2f0: 2020 2020 2020 2072 6574 7572 6e20 696f         return io
-0000e300: 5f54 6578 7449 4f57 7261 7070 6572 282a  _TextIOWrapper(*
-0000e310: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-0000e320: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e330: 7572 6e20 6765 745f 6f75 7470 7574 0a0a  urn get_output..
-0000e340: 2020 2020 2020 2020 6d6f 6465 203d 2070          mode = p
-0000e350: 7969 6e6b 2e4d 6f64 6528 7072 6576 6965  yink.Mode(previe
-0000e360: 773d 5472 7565 290a 2020 2020 2020 2020  w=True).        
-0000e370: 666f 7220 636f 6e74 656e 742c 2065 7870  for content, exp
-0000e380: 6563 7465 6420 696e 2063 6173 6573 3a0a  ected in cases:.
-0000e390: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000e3a0: 7574 203d 2069 6f2e 5374 7269 6e67 494f  ut = io.StringIO
-0000e3b0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-0000e3c0: 6f5f 5465 7874 494f 5772 6170 7065 7220  o_TextIOWrapper 
-0000e3d0: 3d20 696f 2e54 6578 7449 4f57 7261 7070  = io.TextIOWrapp
-0000e3e0: 6572 0a0a 2020 2020 2020 2020 2020 2020  er..            
-0000e3f0: 7769 7468 2070 6174 6368 2822 696f 2e54  with patch("io.T
-0000e400: 6578 7449 4f57 7261 7070 6572 222c 205f  extIOWrapper", _
-0000e410: 6e65 775f 7772 6170 7065 7228 6f75 7470  new_wrapper(outp
-0000e420: 7574 2c20 696f 5f54 6578 7449 4f57 7261  ut, io_TextIOWra
-0000e430: 7070 6572 2929 3a0a 2020 2020 2020 2020  pper)):.        
-0000e440: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2070 7969 6e6b 2e66 6f72 6d61 745f 7374   pyink.format_st
-0000e470: 6469 6e5f 746f 5f73 7464 6f75 7428 0a20  din_to_stdout(. 
-0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e490: 2020 2020 2020 2066 6173 743d 5472 7565         fast=True
-0000e4a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e4b0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-0000e4c0: 743d 636f 6e74 656e 742c 0a20 2020 2020  t=content,.     
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4e0: 2020 2077 7269 7465 5f62 6163 6b3d 7079     write_back=py
-0000e4f0: 696e 6b2e 5772 6974 6542 6163 6b2e 5945  ink.WriteBack.YE
-0000e500: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
-0000e510: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
-0000e520: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
-0000e530: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e540: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000e550: 7074 2069 6f2e 556e 7375 7070 6f72 7465  pt io.Unsupporte
-0000e560: 644f 7065 7261 7469 6f6e 3a0a 2020 2020  dOperation:.    
-0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 7061 7373 2020 2320 5374 7269 6e67 494f  pass  # StringIO
-0000e590: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-0000e5a0: 7420 6465 7461 6368 0a20 2020 2020 2020  t detach.       
-0000e5b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000e5c0: 6f75 7470 7574 2e67 6574 7661 6c75 6528  output.getvalue(
-0000e5d0: 2920 3d3d 2065 7870 6563 7465 640a 0a20  ) == expected.. 
-0000e5e0: 2020 2020 2020 2023 2041 6e20 656d 7074         # An empt
-0000e5f0: 7920 7374 7269 6e67 2069 7320 7468 6520  y string is the 
-0000e600: 6f6e 6c79 2074 6573 7420 6361 7365 2066  only test case f
-0000e610: 6f72 2060 7072 6576 6965 773d 4661 6c73  or `preview=Fals
-0000e620: 6560 0a20 2020 2020 2020 206f 7574 7075  e`.        outpu
-0000e630: 7420 3d20 696f 2e53 7472 696e 6749 4f28  t = io.StringIO(
-0000e640: 290a 2020 2020 2020 2020 696f 5f54 6578  ).        io_Tex
-0000e650: 7449 4f57 7261 7070 6572 203d 2069 6f2e  tIOWrapper = io.
-0000e660: 5465 7874 494f 5772 6170 7065 720a 2020  TextIOWrapper.  
-0000e670: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
-0000e680: 2822 696f 2e54 6578 7449 4f57 7261 7070  ("io.TextIOWrapp
-0000e690: 6572 222c 205f 6e65 775f 7772 6170 7065  er", _new_wrappe
-0000e6a0: 7228 6f75 7470 7574 2c20 696f 5f54 6578  r(output, io_Tex
-0000e6b0: 7449 4f57 7261 7070 6572 2929 3a0a 2020  tIOWrapper)):.  
-0000e6c0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000e6e0: 7969 6e6b 2e66 6f72 6d61 745f 7374 6469  yink.format_stdi
-0000e6f0: 6e5f 746f 5f73 7464 6f75 7428 0a20 2020  n_to_stdout(.   
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 2066 6173 743d 5472 7565 2c0a 2020 2020   fast=True,.    
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e730: 636f 6e74 656e 743d 2222 2c0a 2020 2020  content="",.    
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 7772 6974 655f 6261 636b 3d70 7969 6e6b  write_back=pyink
-0000e760: 2e57 7269 7465 4261 636b 2e59 4553 2c0a  .WriteBack.YES,.
-0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 2020 2020 6d6f 6465 3d44 4546 4155 4c54      mode=DEFAULT
-0000e790: 5f4d 4f44 452c 0a20 2020 2020 2020 2020  _MODE,.         
-0000e7a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e7b0: 2020 2020 2065 7863 6570 7420 696f 2e55       except io.U
-0000e7c0: 6e73 7570 706f 7274 6564 4f70 6572 6174  nsupportedOperat
-0000e7d0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000e7e0: 2020 2020 2070 6173 7320 2023 2053 7472       pass  # Str
-0000e7f0: 696e 6749 4f20 646f 6573 206e 6f74 2073  ingIO does not s
-0000e800: 7570 706f 7274 2064 6574 6163 680a 2020  upport detach.  
-0000e810: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000e820: 206f 7574 7075 742e 6765 7476 616c 7565   output.getvalue
-0000e830: 2829 203d 3d20 2222 0a0a 2020 2020 6465  () == ""..    de
-0000e840: 6620 7465 7374 5f69 6e76 616c 6964 5f63  f test_invalid_c
-0000e850: 6c69 5f72 6567 6578 2873 656c 6629 202d  li_regex(self) -
-0000e860: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000e870: 666f 7220 6f70 7469 6f6e 2069 6e20 5b22  for option in ["
-0000e880: 2d2d 696e 636c 7564 6522 2c20 222d 2d65  --include", "--e
-0000e890: 7863 6c75 6465 222c 2022 2d2d 6578 7465  xclude", "--exte
-0000e8a0: 6e64 2d65 7863 6c75 6465 222c 2022 2d2d  nd-exclude", "--
-0000e8b0: 666f 7263 652d 6578 636c 7564 6522 5d3a  force-exclude"]:
-0000e8c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e8d0: 662e 696e 766f 6b65 426c 6163 6b28 5b22  f.invokeBlack(["
-0000e8e0: 2d22 2c20 6f70 7469 6f6e 2c20 222a 2a28  -", option, "**(
-0000e8f0: 2928 2121 2a29 225d 2c20 6578 6974 5f63  )(!!*)"], exit_c
-0000e900: 6f64 653d 3229 0a0a 2020 2020 6465 6620  ode=2)..    def 
-0000e910: 7465 7374 5f72 6571 7569 7265 645f 7665  test_required_ve
-0000e920: 7273 696f 6e5f 6d61 7463 6865 735f 7665  rsion_matches_ve
-0000e930: 7273 696f 6e28 7365 6c66 2920 2d3e 204e  rsion(self) -> N
-0000e940: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
-0000e950: 662e 696e 766f 6b65 426c 6163 6b28 0a20  f.invokeBlack(. 
-0000e960: 2020 2020 2020 2020 2020 205b 222d 2d72             ["--r
-0000e970: 6571 7569 7265 642d 7665 7273 696f 6e22  equired-version"
-0000e980: 2c20 7079 696e 6b2e 5f5f 7665 7273 696f  , pyink.__versio
-0000e990: 6e5f 5f2c 2022 2d63 222c 2022 3022 5d2c  n__, "-c", "0"],
-0000e9a0: 0a20 2020 2020 2020 2020 2020 2065 7869  .            exi
-0000e9b0: 745f 636f 6465 3d30 2c0a 2020 2020 2020  t_code=0,.      
-0000e9c0: 2020 2020 2020 6967 6e6f 7265 5f63 6f6e        ignore_con
-0000e9d0: 6669 673d 5472 7565 2c0a 2020 2020 2020  fig=True,.      
-0000e9e0: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
-0000e9f0: 745f 7265 7175 6972 6564 5f76 6572 7369  t_required_versi
-0000ea00: 6f6e 5f6d 6174 6368 6573 5f70 6172 7469  on_matches_parti
-0000ea10: 616c 5f76 6572 7369 6f6e 2873 656c 6629  al_version(self)
-0000ea20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000ea30: 2020 7365 6c66 2e69 6e76 6f6b 6542 6c61    self.invokeBla
-0000ea40: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
-0000ea50: 5b22 2d2d 7265 7175 6972 6564 2d76 6572  ["--required-ver
-0000ea60: 7369 6f6e 222c 2070 7969 6e6b 2e5f 5f76  sion", pyink.__v
-0000ea70: 6572 7369 6f6e 5f5f 2e73 706c 6974 2822  ersion__.split("
-0000ea80: 2e22 295b 305d 2c20 222d 6322 2c20 2230  .")[0], "-c", "0
-0000ea90: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0000eaa0: 6578 6974 5f63 6f64 653d 302c 0a20 2020  exit_code=0,.   
-0000eab0: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
-0000eac0: 636f 6e66 6967 3d54 7275 652c 0a20 2020  config=True,.   
-0000ead0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000eae0: 7465 7374 5f72 6571 7569 7265 645f 7665  test_required_ve
-0000eaf0: 7273 696f 6e5f 646f 6573 5f6e 6f74 5f6d  rsion_does_not_m
-0000eb00: 6174 6368 5f6f 6e5f 6d69 6e6f 725f 7665  atch_on_minor_ve
-0000eb10: 7273 696f 6e28 7365 6c66 2920 2d3e 204e  rsion(self) -> N
-0000eb20: 6f6e 653a 0a20 2020 2020 2020 2073 656c  one:.        sel
-0000eb30: 662e 696e 766f 6b65 426c 6163 6b28 0a20  f.invokeBlack(. 
-0000eb40: 2020 2020 2020 2020 2020 205b 222d 2d72             ["--r
-0000eb50: 6571 7569 7265 642d 7665 7273 696f 6e22  equired-version"
-0000eb60: 2c20 7079 696e 6b2e 5f5f 7665 7273 696f  , pyink.__versio
-0000eb70: 6e5f 5f2e 7370 6c69 7428 222e 2229 5b30  n__.split(".")[0
-0000eb80: 5d20 2b20 222e 3939 3922 2c20 222d 6322  ] + ".999", "-c"
-0000eb90: 2c20 2230 225d 2c0a 2020 2020 2020 2020  , "0"],.        
-0000eba0: 2020 2020 6578 6974 5f63 6f64 653d 312c      exit_code=1,
-0000ebb0: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-0000ebc0: 6f72 655f 636f 6e66 6967 3d54 7275 652c  ore_config=True,
-0000ebd0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000ebe0: 6465 6620 7465 7374 5f72 6571 7569 7265  def test_require
-0000ebf0: 645f 7665 7273 696f 6e5f 646f 6573 5f6e  d_version_does_n
-0000ec00: 6f74 5f6d 6174 6368 5f76 6572 7369 6f6e  ot_match_version
-0000ec10: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000ec20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000ec30: 2042 6c61 636b 5275 6e6e 6572 2829 2e69   BlackRunner().i
-0000ec40: 6e76 6f6b 6528 0a20 2020 2020 2020 2020  nvoke(.         
-0000ec50: 2020 2070 7969 6e6b 2e6d 6169 6e2c 0a20     pyink.main,. 
-0000ec60: 2020 2020 2020 2020 2020 205b 222d 2d72             ["--r
-0000ec70: 6571 7569 7265 642d 7665 7273 696f 6e22  equired-version"
-0000ec80: 2c20 2232 302e 3939 6222 2c20 222d 6322  , "20.99b", "-c"
-0000ec90: 2c20 2230 225d 2c0a 2020 2020 2020 2020  , "0"],.        
-0000eca0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000ecb0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-0000ecc0: 742e 6578 6974 5f63 6f64 652c 2031 290a  t.exit_code, 1).
-0000ecd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000ece0: 6572 7449 6e28 2272 6571 7569 7265 6420  ertIn("required 
-0000ecf0: 7665 7273 696f 6e22 2c20 7265 7375 6c74  version", result
-0000ed00: 2e73 7464 6572 7229 0a0a 2020 2020 6465  .stderr)..    de
-0000ed10: 6620 7465 7374 5f70 7265 7365 7276 6573  f test_preserves
-0000ed20: 5f6c 696e 655f 656e 6469 6e67 7328 7365  _line_endings(se
-0000ed30: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000ed40: 2020 2020 2077 6974 6820 5465 6d70 6f72       with Tempor
-0000ed50: 6172 7944 6972 6563 746f 7279 2829 2061  aryDirectory() a
-0000ed60: 7320 776f 726b 7370 6163 653a 0a20 2020  s workspace:.   
-0000ed70: 2020 2020 2020 2020 2074 6573 745f 6669           test_fi
-0000ed80: 6c65 203d 2050 6174 6828 776f 726b 7370  le = Path(worksp
-0000ed90: 6163 6529 202f 2022 7465 7374 2e70 7922  ace) / "test.py"
-0000eda0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000edb0: 206e 6c20 696e 205b 225c 6e22 2c20 225c   nl in ["\n", "\
-0000edc0: 725c 6e22 5d3a 0a20 2020 2020 2020 2020  r\n"]:.         
-0000edd0: 2020 2020 2020 2063 6f6e 7465 6e74 7320         contents 
-0000ede0: 3d20 6e6c 2e6a 6f69 6e28 5b22 6465 6620  = nl.join(["def 
-0000edf0: 6628 2020 293a 222c 2022 2020 2020 7061  f(  ):", "    pa
-0000ee00: 7373 225d 290a 2020 2020 2020 2020 2020  ss"]).          
-0000ee10: 2020 2020 2020 7465 7374 5f66 696c 652e        test_file.
-0000ee20: 7772 6974 655f 6279 7465 7328 636f 6e74  write_bytes(cont
-0000ee30: 656e 7473 2e65 6e63 6f64 6528 2929 0a20  ents.encode()). 
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ee50: 6628 7465 7374 5f66 696c 652c 2077 7269  f(test_file, wri
-0000ee60: 7465 5f62 6163 6b3d 7079 696e 6b2e 5772  te_back=pyink.Wr
-0000ee70: 6974 6542 6163 6b2e 5945 5329 0a20 2020  iteBack.YES).   
-0000ee80: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-0000ee90: 6174 6564 5f63 6f6e 7465 6e74 733a 2062  ated_contents: b
-0000eea0: 7974 6573 203d 2074 6573 745f 6669 6c65  ytes = test_file
-0000eeb0: 2e72 6561 645f 6279 7465 7328 290a 2020  .read_bytes().  
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000eed0: 6c66 2e61 7373 6572 7449 6e28 6e6c 2e65  lf.assertIn(nl.e
-0000eee0: 6e63 6f64 6528 292c 2075 7064 6174 6564  ncode(), updated
-0000eef0: 5f63 6f6e 7465 6e74 7329 0a20 2020 2020  _contents).     
-0000ef00: 2020 2020 2020 2020 2020 2069 6620 6e6c             if nl
-0000ef10: 203d 3d20 225c 6e22 3a0a 2020 2020 2020   == "\n":.      
-0000ef20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ef30: 6c66 2e61 7373 6572 744e 6f74 496e 2862  lf.assertNotIn(b
-0000ef40: 225c 725c 6e22 2c20 7570 6461 7465 645f  "\r\n", updated_
-0000ef50: 636f 6e74 656e 7473 290a 0a20 2020 2064  contents)..    d
-0000ef60: 6566 2074 6573 745f 7072 6573 6572 7665  ef test_preserve
-0000ef70: 735f 6c69 6e65 5f65 6e64 696e 6773 5f76  s_line_endings_v
-0000ef80: 6961 5f73 7464 696e 2873 656c 6629 202d  ia_stdin(self) -
-0000ef90: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000efa0: 666f 7220 6e6c 2069 6e20 5b22 5c6e 222c  for nl in ["\n",
-0000efb0: 2022 5c72 5c6e 225d 3a0a 2020 2020 2020   "\r\n"]:.      
-0000efc0: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
-0000efd0: 206e 6c2e 6a6f 696e 285b 2264 6566 2066   nl.join(["def f
-0000efe0: 2820 2029 3a22 2c20 2220 2020 2070 6173  (  ):", "    pas
-0000eff0: 7322 5d29 0a20 2020 2020 2020 2020 2020  s"]).           
-0000f000: 2072 756e 6e65 7220 3d20 426c 6163 6b52   runner = BlackR
-0000f010: 756e 6e65 7228 290a 2020 2020 2020 2020  unner().        
-0000f020: 2020 2020 7265 7375 6c74 203d 2072 756e      result = run
-0000f030: 6e65 722e 696e 766f 6b65 280a 2020 2020  ner.invoke(.    
-0000f040: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
-0000f050: 6b2e 6d61 696e 2c20 5b22 2d22 2c20 222d  k.main, ["-", "-
-0000f060: 2d66 6173 7422 5d2c 2069 6e70 7574 3d42  -fast"], input=B
-0000f070: 7974 6573 494f 2863 6f6e 7465 6e74 732e  ytesIO(contents.
-0000f080: 656e 636f 6465 2822 7574 6638 2229 290a  encode("utf8")).
-0000f090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000f0a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000f0b0: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-0000f0c0: 742e 6578 6974 5f63 6f64 652c 2030 290a  t.exit_code, 0).
-0000f0d0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000f0e0: 7574 203d 2072 6573 756c 742e 7374 646f  ut = result.stdo
-0000f0f0: 7574 5f62 7974 6573 0a20 2020 2020 2020  ut_bytes.       
-0000f100: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000f110: 496e 286e 6c2e 656e 636f 6465 2822 7574  In(nl.encode("ut
-0000f120: 6638 2229 2c20 6f75 7470 7574 290a 2020  f8"), output).  
-0000f130: 2020 2020 2020 2020 2020 6966 206e 6c20            if nl 
-0000f140: 3d3d 2022 5c6e 223a 0a20 2020 2020 2020  == "\n":.       
-0000f150: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000f160: 7365 7274 4e6f 7449 6e28 6222 5c72 5c6e  sertNotIn(b"\r\n
-0000f170: 222c 206f 7574 7075 7429 0a0a 2020 2020  ", output)..    
-0000f180: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
-0000f190: 7a65 5f6c 696e 655f 656e 6469 6e67 7328  ze_line_endings(
-0000f1a0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000f1b0: 2020 2020 2020 2077 6974 6820 5465 6d70         with Temp
-0000f1c0: 6f72 6172 7944 6972 6563 746f 7279 2829  oraryDirectory()
-0000f1d0: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
-0000f1e0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-0000f1f0: 6669 6c65 203d 2050 6174 6828 776f 726b  file = Path(work
-0000f200: 7370 6163 6529 202f 2022 7465 7374 2e70  space) / "test.p
-0000f210: 7922 0a20 2020 2020 2020 2020 2020 2066  y".            f
-0000f220: 6f72 2064 6174 612c 2065 7870 6563 7465  or data, expecte
-0000f230: 6420 696e 2028 0a20 2020 2020 2020 2020  d in (.         
-0000f240: 2020 2020 2020 2028 6222 635c 725c 6e63         (b"c\r\nc
-0000f250: 5c6e 2022 2c20 6222 635c 725c 6e63 5c72  \n ", b"c\r\nc\r
-0000f260: 5c6e 2229 2c0a 2020 2020 2020 2020 2020  \n"),.          
-0000f270: 2020 2020 2020 2862 226c 5c6e 6c5c 725c        (b"l\nl\r\
-0000f280: 6e20 222c 2062 226c 5c6e 6c5c 6e22 292c  n ", b"l\nl\n"),
-0000f290: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2b0: 7465 7374 5f66 696c 652e 7772 6974 655f  test_file.write_
-0000f2c0: 6279 7465 7328 6461 7461 290a 2020 2020  bytes(data).    
-0000f2d0: 2020 2020 2020 2020 2020 2020 6666 2874              ff(t
-0000f2e0: 6573 745f 6669 6c65 2c20 7772 6974 655f  est_file, write_
-0000f2f0: 6261 636b 3d70 7969 6e6b 2e57 7269 7465  back=pyink.Write
-0000f300: 4261 636b 2e59 4553 290a 2020 2020 2020  Back.YES).      
-0000f310: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000f320: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-0000f330: 6669 6c65 2e72 6561 645f 6279 7465 7328  file.read_bytes(
-0000f340: 292c 2065 7870 6563 7465 6429 0a0a 2020  ), expected)..  
-0000f350: 2020 6465 6620 7465 7374 5f61 7373 6572    def test_asser
-0000f360: 745f 6571 7569 7661 6c65 6e74 5f64 6966  t_equivalent_dif
-0000f370: 6665 7265 6e74 5f61 7374 7328 7365 6c66  ferent_asts(self
-0000f380: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000f390: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-0000f3a0: 6572 7452 6169 7365 7328 4173 7365 7274  ertRaises(Assert
-0000f3b0: 696f 6e45 7272 6f72 293a 0a20 2020 2020  ionError):.     
-0000f3c0: 2020 2020 2020 2070 7969 6e6b 2e61 7373         pyink.ass
-0000f3d0: 6572 745f 6571 7569 7661 6c65 6e74 2822  ert_equivalent("
-0000f3e0: 7b7d 222c 2022 4e6f 6e65 2229 0a0a 2020  {}", "None")..  
-0000f3f0: 2020 6465 6620 7465 7374 5f73 6868 685f    def test_shhh_
-0000f400: 636c 6963 6b28 7365 6c66 2920 2d3e 204e  click(self) -> N
-0000f410: 6f6e 653a 0a20 2020 2020 2020 2074 7279  one:.        try
-0000f420: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
-0000f430: 6f6d 2063 6c69 636b 2069 6d70 6f72 7420  om click import 
-0000f440: 5f75 6e69 636f 6465 6675 6e20 2023 2074  _unicodefun  # t
-0000f450: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0000f460: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
-0000f470: 7445 7272 6f72 3a0a 2020 2020 2020 2020  tError:.        
-0000f480: 2020 2020 7365 6c66 2e73 6b69 7054 6573      self.skipTes
-0000f490: 7428 2249 6e63 6f6d 7061 7469 626c 6520  t("Incompatible 
-0000f4a0: 436c 6963 6b20 7665 7273 696f 6e22 290a  Click version").
-0000f4b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f4c0: 6861 7361 7474 7228 5f75 6e69 636f 6465  hasattr(_unicode
-0000f4d0: 6675 6e2c 2022 5f76 6572 6966 795f 7079  fun, "_verify_py
-0000f4e0: 7468 6f6e 5f65 6e76 2229 3a0a 2020 2020  thon_env"):.    
-0000f4f0: 2020 2020 2020 2020 7365 6c66 2e73 6b69          self.ski
-0000f500: 7054 6573 7428 2249 6e63 6f6d 7061 7469  pTest("Incompati
-0000f510: 626c 6520 436c 6963 6b20 7665 7273 696f  ble Click versio
-0000f520: 6e22 290a 0a20 2020 2020 2020 2023 2046  n")..        # F
-0000f530: 6972 7374 2c20 6c65 7427 7320 7365 6520  irst, let's see 
-0000f540: 6966 2043 6c69 636b 2069 7320 6372 6173  if Click is cras
-0000f550: 6869 6e67 2077 6974 6820 6120 7072 6566  hing with a pref
-0000f560: 6572 7265 6420 4153 4349 4920 6368 6172  erred ASCII char
-0000f570: 7365 742e 0a20 2020 2020 2020 2077 6974  set..        wit
-0000f580: 6820 7061 7463 6828 226c 6f63 616c 652e  h patch("locale.
-0000f590: 6765 7470 7265 6665 7272 6564 656e 636f  getpreferredenco
-0000f5a0: 6469 6e67 2229 2061 7320 6770 653a 0a20  ding") as gpe:. 
-0000f5b0: 2020 2020 2020 2020 2020 2067 7065 2e72             gpe.r
-0000f5c0: 6574 7572 6e5f 7661 6c75 6520 3d20 2241  eturn_value = "A
-0000f5d0: 5343 4949 220a 2020 2020 2020 2020 2020  SCII".          
-0000f5e0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-0000f5f0: 7274 5261 6973 6573 2852 756e 7469 6d65  rtRaises(Runtime
-0000f600: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-0000f610: 2020 2020 2020 2020 5f75 6e69 636f 6465          _unicode
-0000f620: 6675 6e2e 5f76 6572 6966 795f 7079 7468  fun._verify_pyth
-0000f630: 6f6e 5f65 6e76 2829 0a20 2020 2020 2020  on_env().       
-0000f640: 2023 204e 6f77 2c20 6c65 7427 7320 7369   # Now, let's si
-0000f650: 6c65 6e63 6520 436c 6963 6b2e 2e2e 0a20  lence Click.... 
-0000f660: 2020 2020 2020 2070 7969 6e6b 2e70 6174         pyink.pat
-0000f670: 6368 5f63 6c69 636b 2829 0a20 2020 2020  ch_click().     
-0000f680: 2020 2023 202e 2e2e 616e 6420 636f 6e66     # ...and conf
-0000f690: 6972 6d20 6974 2773 2073 696c 656e 742e  irm it's silent.
-0000f6a0: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
-0000f6b0: 7463 6828 226c 6f63 616c 652e 6765 7470  tch("locale.getp
-0000f6c0: 7265 6665 7272 6564 656e 636f 6469 6e67  referredencoding
-0000f6d0: 2229 2061 7320 6770 653a 0a20 2020 2020  ") as gpe:.     
-0000f6e0: 2020 2020 2020 2067 7065 2e72 6574 7572         gpe.retur
-0000f6f0: 6e5f 7661 6c75 6520 3d20 2241 5343 4949  n_value = "ASCII
-0000f700: 220a 2020 2020 2020 2020 2020 2020 7472  ".            tr
-0000f710: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000f720: 2020 205f 756e 6963 6f64 6566 756e 2e5f     _unicodefun._
-0000f730: 7665 7269 6679 5f70 7974 686f 6e5f 656e  verify_python_en
-0000f740: 7628 290a 2020 2020 2020 2020 2020 2020  v().            
-0000f750: 6578 6365 7074 2052 756e 7469 6d65 4572  except RuntimeEr
-0000f760: 726f 7220 6173 2072 653a 0a20 2020 2020  ror as re:.     
-0000f770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f780: 6661 696c 2866 2260 7061 7463 685f 636c  fail(f"`patch_cl
-0000f790: 6963 6b28 2960 2066 6169 6c65 642c 2065  ick()` failed, e
-0000f7a0: 7863 6570 7469 6f6e 2073 7469 6c6c 2072  xception still r
-0000f7b0: 6169 7365 643a 207b 7265 7d22 290a 0a20  aised: {re}").. 
-0000f7c0: 2020 2064 6566 2074 6573 745f 726f 6f74     def test_root
-0000f7d0: 5f6c 6f67 6765 725f 6e6f 745f 7573 6564  _logger_not_used
-0000f7e0: 5f64 6972 6563 746c 7928 7365 6c66 2920  _directly(self) 
-0000f7f0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000f800: 2064 6566 2066 6169 6c28 2a61 7267 733a   def fail(*args:
-0000f810: 2041 6e79 2c20 2a2a 6b77 6172 6773 3a20   Any, **kwargs: 
-0000f820: 416e 7929 202d 3e20 4e6f 6e65 3a0a 2020  Any) -> None:.  
-0000f830: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000f840: 6169 6c28 2252 6563 6f72 6420 6372 6561  ail("Record crea
-0000f850: 7465 6420 7769 7468 2072 6f6f 7420 6c6f  ted with root lo
-0000f860: 6767 6572 2229 0a0a 2020 2020 2020 2020  gger")..        
-0000f870: 7769 7468 2070 6174 6368 2e6d 756c 7469  with patch.multi
-0000f880: 706c 6528 0a20 2020 2020 2020 2020 2020  ple(.           
-0000f890: 206c 6f67 6769 6e67 2e72 6f6f 742c 0a20   logging.root,. 
-0000f8a0: 2020 2020 2020 2020 2020 2064 6562 7567             debug
-0000f8b0: 3d66 6169 6c2c 0a20 2020 2020 2020 2020  =fail,.         
-0000f8c0: 2020 2069 6e66 6f3d 6661 696c 2c0a 2020     info=fail,.  
-0000f8d0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-0000f8e0: 673d 6661 696c 2c0a 2020 2020 2020 2020  g=fail,.        
-0000f8f0: 2020 2020 6572 726f 723d 6661 696c 2c0a      error=fail,.
-0000f900: 2020 2020 2020 2020 2020 2020 6372 6974              crit
-0000f910: 6963 616c 3d66 6169 6c2c 0a20 2020 2020  ical=fail,.     
-0000f920: 2020 2020 2020 206c 6f67 3d66 6169 6c2c         log=fail,
-0000f930: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0000f940: 2020 2020 2020 2020 6666 2854 4849 535f          ff(THIS_
-0000f950: 4449 5220 2f20 2275 7469 6c2e 7079 2229  DIR / "util.py")
-0000f960: 0a0a 2020 2020 6465 6620 7465 7374 5f69  ..    def test_i
-0000f970: 6e76 616c 6964 5f63 6f6e 6669 675f 7265  nvalid_config_re
-0000f980: 7475 726e 5f63 6f64 6528 7365 6c66 2920  turn_code(self) 
-0000f990: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000f9a0: 2074 6d70 5f66 696c 6520 3d20 5061 7468   tmp_file = Path
-0000f9b0: 2870 7969 6e6b 2e64 756d 705f 746f 5f66  (pyink.dump_to_f
-0000f9c0: 696c 6528 2929 0a20 2020 2020 2020 2074  ile()).        t
-0000f9d0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000f9e0: 746d 705f 636f 6e66 6967 203d 2050 6174  tmp_config = Pat
-0000f9f0: 6828 7079 696e 6b2e 6475 6d70 5f74 6f5f  h(pyink.dump_to_
-0000fa00: 6669 6c65 2829 290a 2020 2020 2020 2020  file()).        
-0000fa10: 2020 2020 746d 705f 636f 6e66 6967 2e75      tmp_config.u
-0000fa20: 6e6c 696e 6b28 290a 2020 2020 2020 2020  nlink().        
-0000fa30: 2020 2020 6172 6773 203d 205b 222d 2d63      args = ["--c
-0000fa40: 6f6e 6669 6722 2c20 7374 7228 746d 705f  onfig", str(tmp_
-0000fa50: 636f 6e66 6967 292c 2073 7472 2874 6d70  config), str(tmp
-0000fa60: 5f66 696c 6529 5d0a 2020 2020 2020 2020  _file)].        
-0000fa70: 2020 2020 7365 6c66 2e69 6e76 6f6b 6542      self.invokeB
-0000fa80: 6c61 636b 2861 7267 732c 2065 7869 745f  lack(args, exit_
-0000fa90: 636f 6465 3d32 2c20 6967 6e6f 7265 5f63  code=2, ignore_c
-0000faa0: 6f6e 6669 673d 4661 6c73 6529 0a20 2020  onfig=False).   
-0000fab0: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
-0000fac0: 2020 2020 2020 2020 2020 746d 705f 6669            tmp_fi
-0000fad0: 6c65 2e75 6e6c 696e 6b28 290a 0a20 2020  le.unlink()..   
-0000fae0: 2064 6566 2074 6573 745f 7061 7273 655f   def test_parse_
-0000faf0: 7079 7072 6f6a 6563 745f 746f 6d6c 2873  pyproject_toml(s
-0000fb00: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000fb10: 2020 2020 2020 7465 7374 5f74 6f6d 6c5f        test_toml_
-0000fb20: 6669 6c65 203d 2054 4849 535f 4449 5220  file = THIS_DIR 
-0000fb30: 2f20 2274 6573 742e 746f 6d6c 220a 2020  / "test.toml".  
-0000fb40: 2020 2020 2020 636f 6e66 6967 203d 2070        config = p
-0000fb50: 7969 6e6b 2e70 6172 7365 5f70 7970 726f  yink.parse_pypro
-0000fb60: 6a65 6374 5f74 6f6d 6c28 7374 7228 7465  ject_toml(str(te
-0000fb70: 7374 5f74 6f6d 6c5f 6669 6c65 2929 0a20  st_toml_file)). 
-0000fb80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fb90: 7274 4571 7561 6c28 636f 6e66 6967 5b22  rtEqual(config["
-0000fba0: 7665 7262 6f73 6522 5d2c 2031 290a 2020  verbose"], 1).  
-0000fbb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000fbc0: 7445 7175 616c 2863 6f6e 6669 675b 2263  tEqual(config["c
-0000fbd0: 6865 636b 225d 2c20 226e 6f22 290a 2020  heck"], "no").  
-0000fbe0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000fbf0: 7445 7175 616c 2863 6f6e 6669 675b 2264  tEqual(config["d
-0000fc00: 6966 6622 5d2c 2022 7922 290a 2020 2020  iff"], "y").    
-0000fc10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000fc20: 7175 616c 2863 6f6e 6669 675b 2263 6f6c  qual(config["col
-0000fc30: 6f72 225d 2c20 5472 7565 290a 2020 2020  or"], True).    
-0000fc40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000fc50: 7175 616c 2863 6f6e 6669 675b 226c 696e  qual(config["lin
-0000fc60: 655f 6c65 6e67 7468 225d 2c20 3739 290a  e_length"], 79).
-0000fc70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000fc80: 6572 7445 7175 616c 2863 6f6e 6669 675b  ertEqual(config[
-0000fc90: 2274 6172 6765 745f 7665 7273 696f 6e22  "target_version"
-0000fca0: 5d2c 205b 2270 7933 3622 2c20 2270 7933  ], ["py36", "py3
-0000fcb0: 3722 2c20 2270 7933 3822 5d29 0a20 2020  7", "py38"]).   
-0000fcc0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000fcd0: 4571 7561 6c28 636f 6e66 6967 5b22 7079  Equal(config["py
-0000fce0: 7468 6f6e 5f63 656c 6c5f 6d61 6769 6373  thon_cell_magics
-0000fcf0: 225d 2c20 5b22 6375 7374 6f6d 3122 2c20  "], ["custom1", 
-0000fd00: 2263 7573 746f 6d32 225d 290a 2020 2020  "custom2"]).    
-0000fd10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000fd20: 7175 616c 2863 6f6e 6669 675b 2265 7863  qual(config["exc
-0000fd30: 6c75 6465 225d 2c20 7222 5c2e 7079 693f  lude"], r"\.pyi?
-0000fd40: 2422 290a 2020 2020 2020 2020 7365 6c66  $").        self
-0000fd50: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
-0000fd60: 6669 675b 2269 6e63 6c75 6465 225d 2c20  fig["include"], 
-0000fd70: 7222 5c2e 7079 3f24 2229 0a0a 2020 2020  r"\.py?$")..    
-0000fd80: 6465 6620 7465 7374 5f70 6172 7365 5f70  def test_parse_p
-0000fd90: 7970 726f 6a65 6374 5f74 6f6d 6c5f 7072  yproject_toml_pr
-0000fda0: 6f6a 6563 745f 6d65 7461 6461 7461 2873  oject_metadata(s
-0000fdb0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000fdc0: 2020 2020 2020 666f 7220 7465 7374 5f74        for test_t
-0000fdd0: 6f6d 6c2c 2065 7870 6563 7465 6420 696e  oml, expected in
-0000fde0: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
-0000fdf0: 226f 6e6c 795f 626c 6163 6b5f 7079 7072  "only_black_pypr
-0000fe00: 6f6a 6563 742e 746f 6d6c 222c 205b 2270  oject.toml", ["p
-0000fe10: 7933 3130 225d 292c 0a20 2020 2020 2020  y310"]),.       
-0000fe20: 2020 2020 2028 226f 6e6c 795f 6d65 7461       ("only_meta
-0000fe30: 6461 7461 5f70 7970 726f 6a65 6374 2e74  data_pyproject.t
-0000fe40: 6f6d 6c22 2c20 5b22 7079 3337 222c 2022  oml", ["py37", "
-0000fe50: 7079 3338 222c 2022 7079 3339 222c 2022  py38", "py39", "
-0000fe60: 7079 3331 3022 5d29 2c0a 2020 2020 2020  py310"]),.      
-0000fe70: 2020 2020 2020 2822 6e65 6974 6865 725f        ("neither_
-0000fe80: 7079 7072 6f6a 6563 742e 746f 6d6c 222c  pyproject.toml",
-0000fe90: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
-0000fea0: 2020 2020 2822 626f 7468 5f70 7970 726f      ("both_pypro
-0000feb0: 6a65 6374 2e74 6f6d 6c22 2c20 5b22 7079  ject.toml", ["py
-0000fec0: 3331 3022 5d29 2c0a 2020 2020 2020 2020  310"]),.        
-0000fed0: 5d3a 0a20 2020 2020 2020 2020 2020 2074  ]:.            t
-0000fee0: 6573 745f 746f 6d6c 5f66 696c 6520 3d20  est_toml_file = 
-0000fef0: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
-0000ff00: 2220 2f20 2270 726f 6a65 6374 5f6d 6574  " / "project_met
-0000ff10: 6164 6174 6122 202f 2074 6573 745f 746f  adata" / test_to
-0000ff20: 6d6c 0a20 2020 2020 2020 2020 2020 2063  ml.            c
-0000ff30: 6f6e 6669 6720 3d20 7079 696e 6b2e 7061  onfig = pyink.pa
-0000ff40: 7273 655f 7079 7072 6f6a 6563 745f 746f  rse_pyproject_to
-0000ff50: 6d6c 2873 7472 2874 6573 745f 746f 6d6c  ml(str(test_toml
-0000ff60: 5f66 696c 6529 290a 2020 2020 2020 2020  _file)).        
-0000ff70: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000ff80: 7175 616c 2863 6f6e 6669 672e 6765 7428  qual(config.get(
-0000ff90: 2274 6172 6765 745f 7665 7273 696f 6e22  "target_version"
-0000ffa0: 292c 2065 7870 6563 7465 6429 0a0a 2020  ), expected)..  
-0000ffb0: 2020 6465 6620 7465 7374 5f69 6e66 6572    def test_infer
-0000ffc0: 5f74 6172 6765 745f 7665 7273 696f 6e28  _target_version(
-0000ffd0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000ffe0: 2020 2020 2020 2066 6f72 2076 6572 7369         for versi
-0000fff0: 6f6e 2c20 6578 7065 6374 6564 2069 6e20  on, expected in 
-00010000: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
-00010010: 332e 3622 2c20 5b54 6172 6765 7456 6572  3.6", [TargetVer
-00010020: 7369 6f6e 2e50 5933 365d 292c 0a20 2020  sion.PY36]),.   
-00010030: 2020 2020 2020 2020 2028 2233 2e31 312e           ("3.11.
-00010040: 3072 6331 222c 205b 5461 7267 6574 5665  0rc1", [TargetVe
-00010050: 7273 696f 6e2e 5059 3331 315d 292c 0a20  rsion.PY311]),. 
-00010060: 2020 2020 2020 2020 2020 2028 223e 3d33             (">=3
-00010070: 2e31 3022 2c20 5b54 6172 6765 7456 6572  .10", [TargetVer
-00010080: 7369 6f6e 2e50 5933 3130 2c20 5461 7267  sion.PY310, Targ
-00010090: 6574 5665 7273 696f 6e2e 5059 3331 315d  etVersion.PY311]
-000100a0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000100b0: 223e 3d33 2e31 302e 3622 2c20 5b54 6172  ">=3.10.6", [Tar
-000100c0: 6765 7456 6572 7369 6f6e 2e50 5933 3130  getVersion.PY310
-000100d0: 2c20 5461 7267 6574 5665 7273 696f 6e2e  , TargetVersion.
-000100e0: 5059 3331 315d 292c 0a20 2020 2020 2020  PY311]),.       
-000100f0: 2020 2020 2028 223c 332e 3622 2c20 5b54       ("<3.6", [T
-00010100: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-00010110: 332c 2054 6172 6765 7456 6572 7369 6f6e  3, TargetVersion
-00010120: 2e50 5933 342c 2054 6172 6765 7456 6572  .PY34, TargetVer
-00010130: 7369 6f6e 2e50 5933 355d 292c 0a20 2020  sion.PY35]),.   
-00010140: 2020 2020 2020 2020 2028 223e 332e 372c           (">3.7,
-00010150: 3c33 2e31 3022 2c20 5b54 6172 6765 7456  <3.10", [TargetV
-00010160: 6572 7369 6f6e 2e50 5933 382c 2054 6172  ersion.PY38, Tar
-00010170: 6765 7456 6572 7369 6f6e 2e50 5933 395d  getVersion.PY39]
-00010180: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00010190: 223e 332e 372c 213d 332e 382c 213d 332e  ">3.7,!=3.8,!=3.
-000101a0: 3922 2c20 5b54 6172 6765 7456 6572 7369  9", [TargetVersi
-000101b0: 6f6e 2e50 5933 3130 2c20 5461 7267 6574  on.PY310, Target
-000101c0: 5665 7273 696f 6e2e 5059 3331 315d 292c  Version.PY311]),
-000101d0: 0a20 2020 2020 2020 2020 2020 2028 0a20  .            (. 
-000101e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000101f0: 3e20 332e 392e 342c 2021 3d20 332e 3130  > 3.9.4, != 3.10
-00010200: 2e33 222c 0a20 2020 2020 2020 2020 2020  .3",.           
-00010210: 2020 2020 205b 5461 7267 6574 5665 7273       [TargetVers
-00010220: 696f 6e2e 5059 3339 2c20 5461 7267 6574  ion.PY39, Target
-00010230: 5665 7273 696f 6e2e 5059 3331 302c 2054  Version.PY310, T
-00010240: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-00010250: 3131 5d2c 0a20 2020 2020 2020 2020 2020  11],.           
-00010260: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00010270: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010280: 2020 2221 3d33 2e33 2c21 3d33 2e34 222c    "!=3.3,!=3.4",
-00010290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000102b0: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
-000102c0: 7369 6f6e 2e50 5933 352c 0a20 2020 2020  sion.PY35,.     
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000102e0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-000102f0: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
-00010300: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
-00010310: 7369 6f6e 2e50 5933 372c 0a20 2020 2020  sion.PY37,.     
-00010320: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00010330: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-00010340: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-00010350: 2020 2020 2020 2054 6172 6765 7456 6572         TargetVer
-00010360: 7369 6f6e 2e50 5933 392c 0a20 2020 2020  sion.PY39,.     
-00010370: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00010380: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
-00010390: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
-000103a0: 2020 2020 2020 2020 5461 7267 6574 5665          TargetVe
-000103b0: 7273 696f 6e2e 5059 3331 312c 0a20 2020  rsion.PY311,.   
-000103c0: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
-000103d0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000103e0: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-000103f0: 2020 2020 2020 2020 2020 2020 2022 3d3d               "==
-00010400: 332e 2a22 2c0a 2020 2020 2020 2020 2020  3.*",.          
-00010410: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00010420: 2020 2020 2020 2020 2020 2020 5461 7267              Targ
-00010430: 6574 5665 7273 696f 6e2e 5059 3333 2c0a  etVersion.PY33,.
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
-00010460: 6e2e 5059 3334 2c0a 2020 2020 2020 2020  n.PY34,.        
-00010470: 2020 2020 2020 2020 2020 2020 5461 7267              Targ
-00010480: 6574 5665 7273 696f 6e2e 5059 3335 2c0a  etVersion.PY35,.
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
-000104b0: 6e2e 5059 3336 2c0a 2020 2020 2020 2020  n.PY36,.        
-000104c0: 2020 2020 2020 2020 2020 2020 5461 7267              Targ
-000104d0: 6574 5665 7273 696f 6e2e 5059 3337 2c0a  etVersion.PY37,.
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
-00010500: 6e2e 5059 3338 2c0a 2020 2020 2020 2020  n.PY38,.        
-00010510: 2020 2020 2020 2020 2020 2020 5461 7267              Targ
-00010520: 6574 5665 7273 696f 6e2e 5059 3339 2c0a  etVersion.PY39,.
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2020 5461 7267 6574 5665 7273 696f      TargetVersio
-00010550: 6e2e 5059 3331 302c 0a20 2020 2020 2020  n.PY310,.       
-00010560: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
-00010570: 6765 7456 6572 7369 6f6e 2e50 5933 3131  getVersion.PY311
-00010580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010590: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-000105a0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-000105b0: 2822 3d3d 332e 382e 2a22 2c20 5b54 6172  ("==3.8.*", [Tar
-000105c0: 6765 7456 6572 7369 6f6e 2e50 5933 385d  getVersion.PY38]
-000105d0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000105e0: 4e6f 6e65 2c20 4e6f 6e65 292c 0a20 2020  None, None),.   
-000105f0: 2020 2020 2020 2020 2028 2222 2c20 4e6f           ("", No
-00010600: 6e65 292c 0a20 2020 2020 2020 2020 2020  ne),.           
-00010610: 2028 2269 6e76 616c 6964 222c 204e 6f6e   ("invalid", Non
-00010620: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00010630: 2822 3d3d 696e 7661 6c69 6422 2c20 4e6f  ("==invalid", No
-00010640: 6e65 292c 0a20 2020 2020 2020 2020 2020  ne),.           
-00010650: 2028 223e 332e 392c 213d 696e 7661 6c69   (">3.9,!=invali
-00010660: 6422 2c20 4e6f 6e65 292c 0a20 2020 2020  d", None),.     
-00010670: 2020 2020 2020 2028 2233 222c 204e 6f6e         ("3", Non
-00010680: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00010690: 2822 332e 3222 2c20 4e6f 6e65 292c 0a20  ("3.2", None),. 
-000106a0: 2020 2020 2020 2020 2020 2028 2232 2e37             ("2.7
-000106b0: 2e31 3822 2c20 4e6f 6e65 292c 0a20 2020  .18", None),.   
-000106c0: 2020 2020 2020 2020 2028 223d 3d32 2e37           ("==2.7
-000106d0: 222c 204e 6f6e 6529 2c0a 2020 2020 2020  ", None),.      
-000106e0: 2020 2020 2020 2822 3e33 2e31 302c 3c33        (">3.10,<3
-000106f0: 2e31 3122 2c20 4e6f 6e65 292c 0a20 2020  .11", None),.   
-00010700: 2020 2020 205d 3a0a 2020 2020 2020 2020       ]:.        
-00010710: 2020 2020 7465 7374 5f74 6f6d 6c20 3d20      test_toml = 
-00010720: 7b22 7072 6f6a 6563 7422 3a20 7b22 7265  {"project": {"re
-00010730: 7175 6972 6573 2d70 7974 686f 6e22 3a20  quires-python": 
-00010740: 7665 7273 696f 6e7d 7d0a 2020 2020 2020  version}}.      
-00010750: 2020 2020 2020 7265 7375 6c74 203d 2070        result = p
-00010760: 7969 6e6b 2e66 696c 6573 2e69 6e66 6572  yink.files.infer
-00010770: 5f74 6172 6765 745f 7665 7273 696f 6e28  _target_version(
-00010780: 7465 7374 5f74 6f6d 6c29 0a20 2020 2020  test_toml).     
-00010790: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000107a0: 7274 4571 7561 6c28 7265 7375 6c74 2c20  rtEqual(result, 
-000107b0: 6578 7065 6374 6564 290a 0a20 2020 2064  expected)..    d
-000107c0: 6566 2074 6573 745f 7265 6164 5f70 7970  ef test_read_pyp
-000107d0: 726f 6a65 6374 5f74 6f6d 6c28 7365 6c66  roject_toml(self
-000107e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000107f0: 2020 2074 6573 745f 746f 6d6c 5f66 696c     test_toml_fil
-00010800: 6520 3d20 5448 4953 5f44 4952 202f 2022  e = THIS_DIR / "
-00010810: 7465 7374 2e74 6f6d 6c22 0a20 2020 2020  test.toml".     
-00010820: 2020 2066 616b 655f 6374 7820 3d20 4661     fake_ctx = Fa
-00010830: 6b65 436f 6e74 6578 7428 290a 2020 2020  keContext().    
-00010840: 2020 2020 7079 696e 6b2e 7265 6164 5f70      pyink.read_p
-00010850: 7970 726f 6a65 6374 5f74 6f6d 6c28 6661  yproject_toml(fa
-00010860: 6b65 5f63 7478 2c20 4661 6b65 5061 7261  ke_ctx, FakePara
-00010870: 6d65 7465 7228 292c 2073 7472 2874 6573  meter(), str(tes
-00010880: 745f 746f 6d6c 5f66 696c 6529 290a 2020  t_toml_file)).  
-00010890: 2020 2020 2020 636f 6e66 6967 203d 2066        config = f
-000108a0: 616b 655f 6374 782e 6465 6661 756c 745f  ake_ctx.default_
-000108b0: 6d61 700a 2020 2020 2020 2020 7365 6c66  map.        self
-000108c0: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
-000108d0: 6669 675b 2276 6572 626f 7365 225d 2c20  fig["verbose"], 
-000108e0: 2231 2229 0a20 2020 2020 2020 2073 656c  "1").        sel
-000108f0: 662e 6173 7365 7274 4571 7561 6c28 636f  f.assertEqual(co
-00010900: 6e66 6967 5b22 6368 6563 6b22 5d2c 2022  nfig["check"], "
-00010910: 6e6f 2229 0a20 2020 2020 2020 2073 656c  no").        sel
-00010920: 662e 6173 7365 7274 4571 7561 6c28 636f  f.assertEqual(co
-00010930: 6e66 6967 5b22 6469 6666 225d 2c20 2279  nfig["diff"], "y
-00010940: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00010950: 6173 7365 7274 4571 7561 6c28 636f 6e66  assertEqual(conf
-00010960: 6967 5b22 636f 6c6f 7222 5d2c 2022 5472  ig["color"], "Tr
-00010970: 7565 2229 0a20 2020 2020 2020 2073 656c  ue").        sel
-00010980: 662e 6173 7365 7274 4571 7561 6c28 636f  f.assertEqual(co
-00010990: 6e66 6967 5b22 6c69 6e65 5f6c 656e 6774  nfig["line_lengt
-000109a0: 6822 5d2c 2022 3739 2229 0a20 2020 2020  h"], "79").     
-000109b0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000109c0: 7561 6c28 636f 6e66 6967 5b22 7461 7267  ual(config["targ
-000109d0: 6574 5f76 6572 7369 6f6e 225d 2c20 5b22  et_version"], ["
-000109e0: 7079 3336 222c 2022 7079 3337 222c 2022  py36", "py37", "
-000109f0: 7079 3338 225d 290a 2020 2020 2020 2020  py38"]).        
-00010a00: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00010a10: 2863 6f6e 6669 675b 2265 7863 6c75 6465  (config["exclude
-00010a20: 225d 2c20 7222 5c2e 7079 693f 2422 290a  "], r"\.pyi?$").
-00010a30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00010a40: 6572 7445 7175 616c 2863 6f6e 6669 675b  ertEqual(config[
-00010a50: 2269 6e63 6c75 6465 225d 2c20 7222 5c2e  "include"], r"\.
-00010a60: 7079 3f24 2229 0a0a 2020 2020 4070 7974  py?$")..    @pyt
-00010a70: 6573 742e 6d61 726b 2e69 6e63 6f6d 7061  est.mark.incompa
-00010a80: 7469 626c 655f 7769 7468 5f6d 7970 7963  tible_with_mypyc
-00010a90: 0a20 2020 2064 6566 2074 6573 745f 6669  .    def test_fi
-00010aa0: 6e64 5f70 726f 6a65 6374 5f72 6f6f 7428  nd_project_root(
-00010ab0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00010ac0: 2020 2020 2020 2077 6974 6820 5465 6d70         with Temp
-00010ad0: 6f72 6172 7944 6972 6563 746f 7279 2829  oraryDirectory()
-00010ae0: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
-00010af0: 2020 2020 2020 2020 2020 2072 6f6f 7420             root 
-00010b00: 3d20 5061 7468 2877 6f72 6b73 7061 6365  = Path(workspace
-00010b10: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
-00010b20: 7374 5f64 6972 203d 2072 6f6f 7420 2f20  st_dir = root / 
-00010b30: 2274 6573 7422 0a20 2020 2020 2020 2020  "test".         
-00010b40: 2020 2074 6573 745f 6469 722e 6d6b 6469     test_dir.mkdi
-00010b50: 7228 290a 0a20 2020 2020 2020 2020 2020  r()..           
-00010b60: 2073 7263 5f64 6972 203d 2072 6f6f 7420   src_dir = root 
-00010b70: 2f20 2273 7263 220a 2020 2020 2020 2020  / "src".        
-00010b80: 2020 2020 7372 635f 6469 722e 6d6b 6469      src_dir.mkdi
-00010b90: 7228 290a 0a20 2020 2020 2020 2020 2020  r()..           
-00010ba0: 2072 6f6f 745f 7079 7072 6f6a 6563 7420   root_pyproject 
-00010bb0: 3d20 726f 6f74 202f 2022 7079 7072 6f6a  = root / "pyproj
-00010bc0: 6563 742e 746f 6d6c 220a 2020 2020 2020  ect.toml".      
-00010bd0: 2020 2020 2020 726f 6f74 5f70 7970 726f        root_pypro
-00010be0: 6a65 6374 2e74 6f75 6368 2829 0a20 2020  ject.touch().   
-00010bf0: 2020 2020 2020 2020 2073 7263 5f70 7970           src_pyp
-00010c00: 726f 6a65 6374 203d 2073 7263 5f64 6972  roject = src_dir
-00010c10: 202f 2022 7079 7072 6f6a 6563 742e 746f   / "pyproject.to
-00010c20: 6d6c 220a 2020 2020 2020 2020 2020 2020  ml".            
-00010c30: 7372 635f 7079 7072 6f6a 6563 742e 746f  src_pyproject.to
-00010c40: 7563 6828 290a 2020 2020 2020 2020 2020  uch().          
-00010c50: 2020 7372 635f 7079 7468 6f6e 203d 2073    src_python = s
-00010c60: 7263 5f64 6972 202f 2022 666f 6f2e 7079  rc_dir / "foo.py
-00010c70: 220a 2020 2020 2020 2020 2020 2020 7372  ".            sr
-00010c80: 635f 7079 7468 6f6e 2e74 6f75 6368 2829  c_python.touch()
-00010c90: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00010ca0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cc0: 7079 696e 6b2e 6669 6e64 5f70 726f 6a65  pyink.find_proje
-00010cd0: 6374 5f72 6f6f 7428 2873 7263 5f64 6972  ct_root((src_dir
-00010ce0: 2c20 7465 7374 5f64 6972 2929 2c0a 2020  , test_dir)),.  
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2872                (r
-00010d00: 6f6f 742e 7265 736f 6c76 6528 292c 2022  oot.resolve(), "
-00010d10: 7079 7072 6f6a 6563 742e 746f 6d6c 2229  pyproject.toml")
-00010d20: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00010d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010d40: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-00010d50: 2020 2020 2020 2020 2020 2020 2020 7079                py
-00010d60: 696e 6b2e 6669 6e64 5f70 726f 6a65 6374  ink.find_project
-00010d70: 5f72 6f6f 7428 2873 7263 5f64 6972 2c29  _root((src_dir,)
-00010d80: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00010d90: 2020 2028 7372 635f 6469 722e 7265 736f     (src_dir.reso
-00010da0: 6c76 6528 292c 2022 7079 7072 6f6a 6563  lve(), "pyprojec
-00010db0: 742e 746f 6d6c 2229 2c0a 2020 2020 2020  t.toml"),.      
-00010dc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010dd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00010de0: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00010df0: 2020 2020 2020 7079 696e 6b2e 6669 6e64        pyink.find
-00010e00: 5f70 726f 6a65 6374 5f72 6f6f 7428 2873  _project_root((s
-00010e10: 7263 5f70 7974 686f 6e2c 2929 2c0a 2020  rc_python,)),.  
-00010e20: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-00010e30: 7263 5f64 6972 2e72 6573 6f6c 7665 2829  rc_dir.resolve()
-00010e40: 2c20 2270 7970 726f 6a65 6374 2e74 6f6d  , "pyproject.tom
-00010e50: 6c22 292c 0a20 2020 2020 2020 2020 2020  l"),.           
-00010e60: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00010e70: 7769 7468 2063 6861 6e67 655f 6469 7265  with change_dire
-00010e80: 6374 6f72 7928 7465 7374 5f64 6972 293a  ctory(test_dir):
-00010e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ea0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00010eb0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00010ec0: 2020 2020 2020 2070 7969 6e6b 2e66 696e         pyink.fin
-00010ed0: 645f 7072 6f6a 6563 745f 726f 6f74 2828  d_project_root((
-00010ee0: 222d 222c 292c 2073 7464 696e 5f66 696c  "-",), stdin_fil
-00010ef0: 656e 616d 653d 222e 2e2f 7372 632f 612e  ename="../src/a.
-00010f00: 7079 2229 2c0a 2020 2020 2020 2020 2020  py"),.          
-00010f10: 2020 2020 2020 2020 2020 2873 7263 5f64            (src_d
-00010f20: 6972 2e72 6573 6f6c 7665 2829 2c20 2270  ir.resolve(), "p
-00010f30: 7970 726f 6a65 6374 2e74 6f6d 6c22 292c  yproject.toml"),
-00010f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f50: 2029 0a0a 2020 2020 4070 6174 6368 280a   )..    @patch(.
-00010f60: 2020 2020 2020 2020 2270 7969 6e6b 2e66          "pyink.f
-00010f70: 696c 6573 2e66 696e 645f 7573 6572 5f70  iles.find_user_p
-00010f80: 7970 726f 6a65 6374 5f74 6f6d 6c22 2c0a  yproject_toml",.
-00010f90: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
-00010fa0: 7374 5f66 696e 645f 7079 7072 6f6a 6563  st_find_pyprojec
-00010fb0: 745f 746f 6d6c 2873 656c 662c 2066 696e  t_toml(self, fin
-00010fc0: 645f 7573 6572 5f70 7970 726f 6a65 6374  d_user_pyproject
-00010fd0: 5f74 6f6d 6c3a 204d 6167 6963 4d6f 636b  _toml: MagicMock
-00010fe0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00010ff0: 2020 2066 696e 645f 7573 6572 5f70 7970     find_user_pyp
-00011000: 726f 6a65 6374 5f74 6f6d 6c2e 7369 6465  roject_toml.side
-00011010: 5f65 6666 6563 7420 3d20 5275 6e74 696d  _effect = Runtim
-00011020: 6545 7272 6f72 2829 0a0a 2020 2020 2020  eError()..      
-00011030: 2020 7769 7468 2072 6564 6972 6563 745f    with redirect_
-00011040: 7374 6465 7272 2869 6f2e 5374 7269 6e67  stderr(io.String
-00011050: 494f 2829 2920 6173 2073 7464 6572 723a  IO()) as stderr:
-00011060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00011070: 756c 7420 3d20 7079 696e 6b2e 6669 6c65  ult = pyink.file
-00011080: 732e 6669 6e64 5f70 7970 726f 6a65 6374  s.find_pyproject
-00011090: 5f74 6f6d 6c28 0a20 2020 2020 2020 2020  _toml(.         
-000110a0: 2020 2020 2020 2070 6174 685f 7365 6172         path_sear
-000110b0: 6368 5f73 7461 7274 3d28 7374 7228 5061  ch_start=(str(Pa
-000110c0: 7468 2e63 7764 2829 2e72 6f6f 7429 2c29  th.cwd().root),)
-000110d0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000110e0: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-000110f0: 6573 756c 7420 6973 204e 6f6e 650a 2020  esult is None.  
-00011100: 2020 2020 2020 6572 7220 3d20 7374 6465        err = stde
-00011110: 7272 2e67 6574 7661 6c75 6528 290a 2020  rr.getvalue().  
-00011120: 2020 2020 2020 6173 7365 7274 2022 4967        assert "Ig
-00011130: 6e6f 7269 6e67 2075 7365 7220 636f 6e66  noring user conf
-00011140: 6967 7572 6174 696f 6e22 2069 6e20 6572  iguration" in er
-00011150: 720a 0a20 2020 2040 7061 7463 6828 0a20  r..    @patch(. 
-00011160: 2020 2020 2020 2022 7079 696e 6b2e 6669         "pyink.fi
-00011170: 6c65 732e 6669 6e64 5f75 7365 725f 7079  les.find_user_py
-00011180: 7072 6f6a 6563 745f 746f 6d6c 222c 0a20  project_toml",. 
-00011190: 2020 2020 2020 2070 7969 6e6b 2e66 696c         pyink.fil
-000111a0: 6573 2e66 696e 645f 7573 6572 5f70 7970  es.find_user_pyp
-000111b0: 726f 6a65 6374 5f74 6f6d 6c2e 5f5f 7772  roject_toml.__wr
-000111c0: 6170 7065 645f 5f2c 0a20 2020 2029 0a20  apped__,.    ). 
-000111d0: 2020 2064 6566 2074 6573 745f 6669 6e64     def test_find
-000111e0: 5f75 7365 725f 7079 7072 6f6a 6563 745f  _user_pyproject_
-000111f0: 746f 6d6c 5f6c 696e 7578 2873 656c 6629  toml_linux(self)
-00011200: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00011210: 2020 6966 2073 7973 7465 6d28 2920 3d3d    if system() ==
-00011220: 2022 5769 6e64 6f77 7322 3a0a 2020 2020   "Windows":.    
-00011230: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00011240: 2020 2020 2020 2020 2320 5465 7374 2069          # Test i
-00011250: 6620 5844 475f 434f 4e46 4947 5f48 4f4d  f XDG_CONFIG_HOM
-00011260: 4520 6973 2063 6865 636b 6564 0a20 2020  E is checked.   
-00011270: 2020 2020 2077 6974 6820 5465 6d70 6f72       with Tempor
-00011280: 6172 7944 6972 6563 746f 7279 2829 2061  aryDirectory() a
-00011290: 7320 776f 726b 7370 6163 653a 0a20 2020  s workspace:.   
-000112a0: 2020 2020 2020 2020 2074 6d70 5f75 7365           tmp_use
-000112b0: 725f 636f 6e66 6967 203d 2050 6174 6828  r_config = Path(
-000112c0: 776f 726b 7370 6163 6529 202f 2022 7079  workspace) / "py
-000112d0: 696e 6b22 0a20 2020 2020 2020 2020 2020  ink".           
-000112e0: 2077 6974 6820 7061 7463 682e 6469 6374   with patch.dict
-000112f0: 2822 6f73 2e65 6e76 6972 6f6e 222c 207b  ("os.environ", {
-00011300: 2258 4447 5f43 4f4e 4649 475f 484f 4d45  "XDG_CONFIG_HOME
-00011310: 223a 2077 6f72 6b73 7061 6365 7d29 3a0a  ": workspace}):.
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00011340: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011350: 2020 2020 2020 7079 696e 6b2e 6669 6c65        pyink.file
-00011360: 732e 6669 6e64 5f75 7365 725f 7079 7072  s.find_user_pypr
-00011370: 6f6a 6563 745f 746f 6d6c 2829 2c20 746d  oject_toml(), tm
-00011380: 705f 7573 6572 5f63 6f6e 6669 672e 7265  p_user_config.re
-00011390: 736f 6c76 6528 290a 2020 2020 2020 2020  solve().        
-000113a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000113b0: 2020 2023 2054 6573 7420 6661 6c6c 6261     # Test fallba
-000113c0: 636b 2066 6f72 2058 4447 5f43 4f4e 4649  ck for XDG_CONFI
-000113d0: 475f 484f 4d45 0a20 2020 2020 2020 2077  G_HOME.        w
-000113e0: 6974 6820 7061 7463 682e 6469 6374 2822  ith patch.dict("
-000113f0: 6f73 2e65 6e76 6972 6f6e 2229 3a0a 2020  os.environ"):.  
-00011400: 2020 2020 2020 2020 2020 6f73 2e65 6e76            os.env
-00011410: 6972 6f6e 2e70 6f70 2822 5844 475f 434f  iron.pop("XDG_CO
-00011420: 4e46 4947 5f48 4f4d 4522 2c20 4e6f 6e65  NFIG_HOME", None
-00011430: 290a 2020 2020 2020 2020 2020 2020 6661  ).            fa
-00011440: 6c6c 6261 636b 5f75 7365 725f 636f 6e66  llback_user_conf
-00011450: 6967 203d 2050 6174 6828 227e 2f2e 636f  ig = Path("~/.co
-00011460: 6e66 6967 2229 2e65 7870 616e 6475 7365  nfig").expanduse
-00011470: 7228 2920 2f20 2270 7969 6e6b 220a 2020  r() / "pyink".  
-00011480: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00011490: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-000114a0: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
-000114b0: 6b2e 6669 6c65 732e 6669 6e64 5f75 7365  k.files.find_use
-000114c0: 725f 7079 7072 6f6a 6563 745f 746f 6d6c  r_pyproject_toml
-000114d0: 2829 2c20 6661 6c6c 6261 636b 5f75 7365  (), fallback_use
-000114e0: 725f 636f 6e66 6967 2e72 6573 6f6c 7665  r_config.resolve
-000114f0: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
-00011500: 0a0a 2020 2020 6465 6620 7465 7374 5f66  ..    def test_f
-00011510: 696e 645f 7573 6572 5f70 7970 726f 6a65  ind_user_pyproje
-00011520: 6374 5f74 6f6d 6c5f 7769 6e64 6f77 7328  ct_toml_windows(
-00011530: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00011540: 2020 2020 2020 2069 6620 7379 7374 656d         if system
-00011550: 2829 2021 3d20 2257 696e 646f 7773 223a  () != "Windows":
-00011560: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00011570: 7572 6e0a 0a20 2020 2020 2020 2075 7365  urn..        use
-00011580: 725f 636f 6e66 6967 5f70 6174 6820 3d20  r_config_path = 
-00011590: 5061 7468 2e68 6f6d 6528 2920 2f20 222e  Path.home() / ".
-000115a0: 7079 696e 6b22 0a20 2020 2020 2020 2073  pyink".        s
-000115b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000115c0: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
-000115d0: 6e6b 2e66 696c 6573 2e66 696e 645f 7573  nk.files.find_us
-000115e0: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
-000115f0: 6c28 292c 2075 7365 725f 636f 6e66 6967  l(), user_config
-00011600: 5f70 6174 682e 7265 736f 6c76 6528 290a  _path.resolve().
-00011610: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00011620: 6566 2074 6573 745f 6270 6f5f 3333 3636  ef test_bpo_3366
-00011630: 305f 776f 726b 6172 6f75 6e64 2873 656c  0_workaround(sel
-00011640: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00011650: 2020 2020 6966 2073 7973 7465 6d28 2920      if system() 
-00011660: 3d3d 2022 5769 6e64 6f77 7322 3a0a 2020  == "Windows":.  
-00011670: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011680: 0a0a 2020 2020 2020 2020 2320 6874 7470  ..        # http
-00011690: 733a 2f2f 6275 6773 2e70 7974 686f 6e2e  s://bugs.python.
-000116a0: 6f72 672f 6973 7375 6533 3336 3630 0a20  org/issue33660. 
-000116b0: 2020 2020 2020 2072 6f6f 7420 3d20 5061         root = Pa
-000116c0: 7468 2822 2f22 290a 2020 2020 2020 2020  th("/").        
-000116d0: 7769 7468 2063 6861 6e67 655f 6469 7265  with change_dire
-000116e0: 6374 6f72 7928 726f 6f74 293a 0a20 2020  ctory(root):.   
-000116f0: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-00011700: 5061 7468 2822 776f 726b 7370 6163 6522  Path("workspace"
-00011710: 2920 2f20 2270 726f 6a65 6374 220a 2020  ) / "project".  
-00011720: 2020 2020 2020 2020 2020 7265 706f 7274            report
-00011730: 203d 2070 7969 6e6b 2e52 6570 6f72 7428   = pyink.Report(
-00011740: 7665 7262 6f73 653d 5472 7565 290a 2020  verbose=True).  
-00011750: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
-00011760: 697a 6564 5f70 6174 6820 3d20 7079 696e  ized_path = pyin
-00011770: 6b2e 6e6f 726d 616c 697a 655f 7061 7468  k.normalize_path
-00011780: 5f6d 6179 6265 5f69 676e 6f72 6528 7061  _maybe_ignore(pa
-00011790: 7468 2c20 726f 6f74 2c20 7265 706f 7274  th, root, report
-000117a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000117b0: 6c66 2e61 7373 6572 7445 7175 616c 286e  lf.assertEqual(n
-000117c0: 6f72 6d61 6c69 7a65 645f 7061 7468 2c20  ormalized_path, 
-000117d0: 2277 6f72 6b73 7061 6365 2f70 726f 6a65  "workspace/proje
-000117e0: 6374 2229 0a0a 2020 2020 6465 6620 7465  ct")..    def te
-000117f0: 7374 5f6e 6f72 6d61 6c69 7a65 5f70 6174  st_normalize_pat
-00011800: 685f 6967 6e6f 7265 5f77 696e 646f 7773  h_ignore_windows
-00011810: 5f6a 756e 6374 696f 6e73 5f6f 7574 7369  _junctions_outsi
-00011820: 6465 5f6f 665f 726f 6f74 2873 656c 6629  de_of_root(self)
-00011830: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00011840: 2020 6966 2073 7973 7465 6d28 2920 213d    if system() !=
-00011850: 2022 5769 6e64 6f77 7322 3a0a 2020 2020   "Windows":.    
-00011860: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00011870: 2020 2020 2020 2020 7769 7468 2054 656d          with Tem
-00011880: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-00011890: 2920 6173 2077 6f72 6b73 7061 6365 3a0a  ) as workspace:.
-000118a0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-000118b0: 203d 2050 6174 6828 776f 726b 7370 6163   = Path(workspac
-000118c0: 6529 0a20 2020 2020 2020 2020 2020 206a  e).            j
-000118d0: 756e 6374 696f 6e5f 6469 7220 3d20 726f  unction_dir = ro
-000118e0: 6f74 202f 2022 6a75 6e63 7469 6f6e 220a  ot / "junction".
-000118f0: 2020 2020 2020 2020 2020 2020 6a75 6e63              junc
-00011900: 7469 6f6e 5f74 6172 6765 745f 6f75 7473  tion_target_outs
-00011910: 6964 655f 6f66 5f72 6f6f 7420 3d20 726f  ide_of_root = ro
-00011920: 6f74 202f 2022 2e2e 220a 2020 2020 2020  ot / "..".      
-00011930: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
-00011940: 6622 6d6b 6c69 6e6b 202f 4a20 7b6a 756e  f"mklink /J {jun
-00011950: 6374 696f 6e5f 6469 727d 207b 6a75 6e63  ction_dir} {junc
-00011960: 7469 6f6e 5f74 6172 6765 745f 6f75 7473  tion_target_outs
-00011970: 6964 655f 6f66 5f72 6f6f 747d 2229 0a0a  ide_of_root}")..
-00011980: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00011990: 7274 203d 2070 7969 6e6b 2e52 6570 6f72  rt = pyink.Repor
-000119a0: 7428 7665 7262 6f73 653d 5472 7565 290a  t(verbose=True).
-000119b0: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-000119c0: 616c 697a 6564 5f70 6174 6820 3d20 7079  alized_path = py
-000119d0: 696e 6b2e 6e6f 726d 616c 697a 655f 7061  ink.normalize_pa
-000119e0: 7468 5f6d 6179 6265 5f69 676e 6f72 6528  th_maybe_ignore(
-000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a00: 206a 756e 6374 696f 6e5f 6469 722c 2072   junction_dir, r
-00011a10: 6f6f 742c 2072 6570 6f72 740a 2020 2020  oot, report.    
-00011a20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011a30: 2020 2020 2020 2320 4d61 6e75 616c 6c79        # Manually
-00011a40: 2064 656c 6574 6520 666f 7220 5079 7468   delete for Pyth
-00011a50: 6f6e 203c 2033 2e38 0a20 2020 2020 2020  on < 3.8.       
-00011a60: 2020 2020 206f 732e 7379 7374 656d 2866       os.system(f
-00011a70: 2272 6d64 6972 207b 6a75 6e63 7469 6f6e  "rmdir {junction
-00011a80: 5f64 6972 7d22 290a 0a20 2020 2020 2020  _dir}")..       
-00011a90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00011aa0: 4571 7561 6c28 6e6f 726d 616c 697a 6564  Equal(normalized
-00011ab0: 5f70 6174 682c 204e 6f6e 6529 0a0a 2020  _path, None)..  
-00011ac0: 2020 6465 6620 7465 7374 5f6e 6577 6c69    def test_newli
-00011ad0: 6e65 5f63 6f6d 6d65 6e74 5f69 6e74 6572  ne_comment_inter
-00011ae0: 6163 7469 6f6e 2873 656c 6629 202d 3e20  action(self) -> 
-00011af0: 4e6f 6e65 3a0a 2020 2020 2020 2020 736f  None:.        so
-00011b00: 7572 6365 203d 2022 636c 6173 7320 413a  urce = "class A:
-00011b10: 5c5c 5c72 5c6e 2320 7479 7065 3a20 6967  \\\r\n# type: ig
-00011b20: 6e6f 7265 5c6e 2070 6173 735c 6e22 0a20  nore\n pass\n". 
-00011b30: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-00011b40: 7079 696e 6b2e 666f 726d 6174 5f73 7472  pyink.format_str
-00011b50: 2873 6f75 7263 652c 206d 6f64 653d 4445  (source, mode=DE
-00011b60: 4641 554c 545f 4d4f 4445 290a 2020 2020  FAULT_MODE).    
-00011b70: 2020 2020 7079 696e 6b2e 6173 7365 7274      pyink.assert
-00011b80: 5f73 7461 626c 6528 736f 7572 6365 2c20  _stable(source, 
-00011b90: 6f75 7470 7574 2c20 6d6f 6465 3d44 4546  output, mode=DEF
-00011ba0: 4155 4c54 5f4d 4f44 4529 0a0a 2020 2020  AULT_MODE)..    
-00011bb0: 6465 6620 7465 7374 5f62 706f 5f32 3134  def test_bpo_214
-00011bc0: 325f 776f 726b 6172 6f75 6e64 2873 656c  2_workaround(sel
-00011bd0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00011be0: 2020 2020 2320 6874 7470 733a 2f2f 6275      # https://bu
-00011bf0: 6773 2e70 7974 686f 6e2e 6f72 672f 6973  gs.python.org/is
-00011c00: 7375 6532 3134 320a 0a20 2020 2020 2020  sue2142..       
-00011c10: 2073 6f75 7263 652c 205f 203d 2072 6561   source, _ = rea
-00011c20: 645f 6461 7461 2822 6d69 7363 656c 6c61  d_data("miscella
-00011c30: 6e65 6f75 7322 2c20 226d 6973 7369 6e67  neous", "missing
-00011c40: 5f66 696e 616c 5f6e 6577 6c69 6e65 2229  _final_newline")
-00011c50: 0a20 2020 2020 2020 2023 2072 6561 645f  .        # read_
-00011c60: 6461 7461 2061 6464 7320 6120 7472 6169  data adds a trai
-00011c70: 6c69 6e67 206e 6577 6c69 6e65 0a20 2020  ling newline.   
-00011c80: 2020 2020 2073 6f75 7263 6520 3d20 736f       source = so
-00011c90: 7572 6365 2e72 7374 7269 7028 290a 2020  urce.rstrip().  
-00011ca0: 2020 2020 2020 6578 7065 6374 6564 2c20        expected, 
-00011cb0: 5f20 3d20 7265 6164 5f64 6174 6128 226d  _ = read_data("m
-00011cc0: 6973 6365 6c6c 616e 656f 7573 222c 2022  iscellaneous", "
-00011cd0: 6d69 7373 696e 675f 6669 6e61 6c5f 6e65  missing_final_ne
-00011ce0: 776c 696e 652e 6469 6666 2229 0a20 2020  wline.diff").   
-00011cf0: 2020 2020 2074 6d70 5f66 696c 6520 3d20       tmp_file = 
-00011d00: 5061 7468 2870 7969 6e6b 2e64 756d 705f  Path(pyink.dump_
-00011d10: 746f 5f66 696c 6528 736f 7572 6365 2c20  to_file(source, 
-00011d20: 656e 7375 7265 5f66 696e 616c 5f6e 6577  ensure_final_new
-00011d30: 6c69 6e65 3d46 616c 7365 2929 0a20 2020  line=False)).   
-00011d40: 2020 2020 2064 6966 665f 6865 6164 6572       diff_header
-00011d50: 203d 2072 652e 636f 6d70 696c 6528 0a20   = re.compile(. 
-00011d60: 2020 2020 2020 2020 2020 2072 6622 7b72             rf"{r
-00011d70: 652e 6573 6361 7065 2873 7472 2874 6d70  e.escape(str(tmp
-00011d80: 5f66 696c 6529 297d 5c74 5c64 5c64 5c64  _file))}\t\d\d\d
-00011d90: 5c64 2d5c 645c 642d 5c64 5c64 2022 0a20  \d-\d\d-\d\d ". 
-00011da0: 2020 2020 2020 2020 2020 2072 225c 645c             r"\d\
-00011db0: 643a 5c64 5c64 3a5c 645c 645c 2e5c 645c  d:\d\d:\d\d\.\d\
-00011dc0: 645c 645c 645c 645c 6420 5c2b 5c64 5c64  d\d\d\d\d \+\d\d
-00011dd0: 5c64 5c64 220a 2020 2020 2020 2020 290a  \d\d".        ).
-00011de0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00011df0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00011e00: 3d20 426c 6163 6b52 756e 6e65 7228 292e  = BlackRunner().
-00011e10: 696e 766f 6b65 2870 7969 6e6b 2e6d 6169  invoke(pyink.mai
-00011e20: 6e2c 205b 222d 2d64 6966 6622 2c20 7374  n, ["--diff", st
-00011e30: 7228 746d 705f 6669 6c65 295d 290a 2020  r(tmp_file)]).  
-00011e40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00011e50: 7373 6572 7445 7175 616c 2872 6573 756c  ssertEqual(resul
-00011e60: 742e 6578 6974 5f63 6f64 652c 2030 290a  t.exit_code, 0).
-00011e70: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
-00011e80: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-00011e90: 756e 6c69 6e6b 2874 6d70 5f66 696c 6529  unlink(tmp_file)
-00011ea0: 0a20 2020 2020 2020 2061 6374 7561 6c20  .        actual 
-00011eb0: 3d20 7265 7375 6c74 2e6f 7574 7075 740a  = result.output.
-00011ec0: 2020 2020 2020 2020 6163 7475 616c 203d          actual =
-00011ed0: 2064 6966 665f 6865 6164 6572 2e73 7562   diff_header.sub
-00011ee0: 2844 4554 4552 4d49 4e49 5354 4943 5f48  (DETERMINISTIC_H
-00011ef0: 4541 4445 522c 2061 6374 7561 6c29 0a20  EADER, actual). 
-00011f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011f10: 7274 4571 7561 6c28 6163 7475 616c 2c20  rtEqual(actual, 
-00011f20: 6578 7065 6374 6564 290a 0a20 2020 2040  expected)..    @
-00011f30: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00011f40: 2064 6566 2063 6f6d 7061 7265 5f72 6573   def compare_res
-00011f50: 756c 7473 280a 2020 2020 2020 2020 7265  ults(.        re
-00011f60: 7375 6c74 3a20 636c 6963 6b2e 7465 7374  sult: click.test
-00011f70: 696e 672e 5265 7375 6c74 2c20 6578 7065  ing.Result, expe
-00011f80: 6374 6564 5f76 616c 7565 3a20 7374 722c  cted_value: str,
-00011f90: 2065 7870 6563 7465 645f 6578 6974 5f63   expected_exit_c
-00011fa0: 6f64 653a 2069 6e74 0a20 2020 2029 202d  ode: int.    ) -
-00011fb0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011fc0: 2222 2248 656c 7065 7220 6d65 7468 6f64  """Helper method
-00011fd0: 2074 6f20 7465 7374 2074 6865 2076 616c   to test the val
-00011fe0: 7565 2061 6e64 2065 7869 7420 636f 6465  ue and exit code
-00011ff0: 206f 6620 6120 636c 6963 6b20 5265 7375   of a click Resu
-00012000: 6c74 2e22 2222 0a20 2020 2020 2020 2061  lt.""".        a
-00012010: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-00012020: 2020 2020 7265 7375 6c74 2e6f 7574 7075      result.outpu
-00012030: 7420 3d3d 2065 7870 6563 7465 645f 7661  t == expected_va
-00012040: 6c75 650a 2020 2020 2020 2020 292c 2022  lue.        ), "
-00012050: 5468 6520 6f75 7470 7574 2064 6964 206e  The output did n
-00012060: 6f74 206d 6174 6368 2074 6865 2065 7870  ot match the exp
-00012070: 6563 7465 6420 7661 6c75 652e 220a 2020  ected value.".  
-00012080: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
-00012090: 756c 742e 6578 6974 5f63 6f64 6520 3d3d  ult.exit_code ==
-000120a0: 2065 7870 6563 7465 645f 6578 6974 5f63   expected_exit_c
-000120b0: 6f64 652c 2022 5468 6520 6578 6974 2063  ode, "The exit c
-000120c0: 6f64 6520 6973 2069 6e63 6f72 7265 6374  ode is incorrect
-000120d0: 2e22 0a0a 2020 2020 6465 6620 7465 7374  ."..    def test
-000120e0: 5f63 6f64 655f 6f70 7469 6f6e 2873 656c  _code_option(sel
-000120f0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00012100: 2020 2020 2222 2254 6573 7420 7468 6520      """Test the 
-00012110: 636f 6465 206f 7074 696f 6e20 7769 7468  code option with
-00012120: 206e 6f20 6368 616e 6765 732e 2222 220a   no changes.""".
-00012130: 2020 2020 2020 2020 636f 6465 203d 2027          code = '
-00012140: 7072 696e 7428 2248 656c 6c6f 2077 6f72  print("Hello wor
-00012150: 6c64 2229 5c6e 270a 2020 2020 2020 2020  ld")\n'.        
-00012160: 6172 6773 203d 205b 222d 2d63 6f64 6522  args = ["--code"
-00012170: 2c20 636f 6465 5d0a 2020 2020 2020 2020  , code].        
-00012180: 7265 7375 6c74 203d 2043 6c69 5275 6e6e  result = CliRunn
-00012190: 6572 2829 2e69 6e76 6f6b 6528 7079 696e  er().invoke(pyin
-000121a0: 6b2e 6d61 696e 2c20 6172 6773 290a 0a20  k.main, args).. 
-000121b0: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-000121c0: 6172 655f 7265 7375 6c74 7328 7265 7375  are_results(resu
-000121d0: 6c74 2c20 636f 6465 2c20 3029 0a0a 2020  lt, code, 0)..  
-000121e0: 2020 6465 6620 7465 7374 5f63 6f64 655f    def test_code_
-000121f0: 6f70 7469 6f6e 5f63 6861 6e67 6564 2873  option_changed(s
-00012200: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00012210: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-00012220: 6520 636f 6465 206f 7074 696f 6e20 7768  e code option wh
-00012230: 656e 2063 6861 6e67 6573 2061 7265 2072  en changes are r
-00012240: 6571 7569 7265 642e 2222 220a 2020 2020  equired.""".    
-00012250: 2020 2020 636f 6465 203d 2022 7072 696e      code = "prin
-00012260: 7428 2768 656c 6c6f 2077 6f72 6c64 2729  t('hello world')
-00012270: 220a 2020 2020 2020 2020 666f 726d 6174  ".        format
-00012280: 7465 6420 3d20 7079 696e 6b2e 666f 726d  ted = pyink.form
-00012290: 6174 5f73 7472 2863 6f64 652c 206d 6f64  at_str(code, mod
-000122a0: 653d 4445 4641 554c 545f 4d4f 4445 290a  e=DEFAULT_MODE).
-000122b0: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-000122c0: 5b22 2d2d 636f 6465 222c 2063 6f64 655d  ["--code", code]
-000122d0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000122e0: 3d20 436c 6952 756e 6e65 7228 292e 696e  = CliRunner().in
-000122f0: 766f 6b65 2870 7969 6e6b 2e6d 6169 6e2c  voke(pyink.main,
-00012300: 2061 7267 7329 0a0a 2020 2020 2020 2020   args)..        
-00012310: 7365 6c66 2e63 6f6d 7061 7265 5f72 6573  self.compare_res
-00012320: 756c 7473 2872 6573 756c 742c 2066 6f72  ults(result, for
-00012330: 6d61 7474 6564 2c20 3029 0a0a 2020 2020  matted, 0)..    
-00012340: 6465 6620 7465 7374 5f63 6f64 655f 6f70  def test_code_op
-00012350: 7469 6f6e 5f63 6865 636b 2873 656c 6629  tion_check(self)
-00012360: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00012370: 2020 2222 2254 6573 7420 7468 6520 636f    """Test the co
-00012380: 6465 206f 7074 696f 6e20 7768 656e 2063  de option when c
-00012390: 6865 636b 2069 7320 7061 7373 6564 2e22  heck is passed."
-000123a0: 2222 0a20 2020 2020 2020 2061 7267 7320  "".        args 
-000123b0: 3d20 5b22 2d2d 6368 6563 6b22 2c20 222d  = ["--check", "-
-000123c0: 2d63 6f64 6522 2c20 2770 7269 6e74 2822  -code", 'print("
-000123d0: 4865 6c6c 6f20 776f 726c 6422 295c 6e27  Hello world")\n'
-000123e0: 5d0a 2020 2020 2020 2020 7265 7375 6c74  ].        result
-000123f0: 203d 2043 6c69 5275 6e6e 6572 2829 2e69   = CliRunner().i
-00012400: 6e76 6f6b 6528 7079 696e 6b2e 6d61 696e  nvoke(pyink.main
-00012410: 2c20 6172 6773 290a 2020 2020 2020 2020  , args).        
-00012420: 7365 6c66 2e63 6f6d 7061 7265 5f72 6573  self.compare_res
-00012430: 756c 7473 2872 6573 756c 742c 2022 222c  ults(result, "",
-00012440: 2030 290a 0a20 2020 2064 6566 2074 6573   0)..    def tes
-00012450: 745f 636f 6465 5f6f 7074 696f 6e5f 6368  t_code_option_ch
-00012460: 6563 6b5f 6368 616e 6765 6428 7365 6c66  eck_changed(self
-00012470: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012480: 2020 2022 2222 5465 7374 2074 6865 2063     """Test the c
-00012490: 6f64 6520 6f70 7469 6f6e 2077 6865 6e20  ode option when 
-000124a0: 6368 616e 6765 7320 6172 6520 7265 7175  changes are requ
-000124b0: 6972 6564 2c20 616e 6420 6368 6563 6b20  ired, and check 
-000124c0: 6973 2070 6173 7365 642e 2222 220a 2020  is passed.""".  
-000124d0: 2020 2020 2020 6172 6773 203d 205b 222d        args = ["-
-000124e0: 2d63 6865 636b 222c 2022 2d2d 636f 6465  -check", "--code
-000124f0: 222c 2022 7072 696e 7428 2768 656c 6c6f  ", "print('hello
-00012500: 2077 6f72 6c64 2729 225d 0a20 2020 2020   world')"].     
-00012510: 2020 2072 6573 756c 7420 3d20 436c 6952     result = CliR
-00012520: 756e 6e65 7228 292e 696e 766f 6b65 2870  unner().invoke(p
-00012530: 7969 6e6b 2e6d 6169 6e2c 2061 7267 7329  yink.main, args)
-00012540: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00012550: 6d70 6172 655f 7265 7375 6c74 7328 7265  mpare_results(re
-00012560: 7375 6c74 2c20 2222 2c20 3129 0a0a 2020  sult, "", 1)..  
-00012570: 2020 6465 6620 7465 7374 5f63 6f64 655f    def test_code_
-00012580: 6f70 7469 6f6e 5f64 6966 6628 7365 6c66  option_diff(self
-00012590: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000125a0: 2020 2022 2222 5465 7374 2074 6865 2063     """Test the c
-000125b0: 6f64 6520 6f70 7469 6f6e 2077 6865 6e20  ode option when 
-000125c0: 6469 6666 2069 7320 7061 7373 6564 2e22  diff is passed."
-000125d0: 2222 0a20 2020 2020 2020 2063 6f64 6520  "".        code 
-000125e0: 3d20 2270 7269 6e74 2827 6865 6c6c 6f20  = "print('hello 
-000125f0: 776f 726c 6427 2922 0a20 2020 2020 2020  world')".       
-00012600: 2066 6f72 6d61 7474 6564 203d 2070 7969   formatted = pyi
-00012610: 6e6b 2e66 6f72 6d61 745f 7374 7228 636f  nk.format_str(co
-00012620: 6465 2c20 6d6f 6465 3d44 4546 4155 4c54  de, mode=DEFAULT
-00012630: 5f4d 4f44 4529 0a20 2020 2020 2020 2072  _MODE).        r
-00012640: 6573 756c 745f 6469 6666 203d 2064 6966  esult_diff = dif
-00012650: 6628 636f 6465 2c20 666f 726d 6174 7465  f(code, formatte
-00012660: 642c 2022 5354 4449 4e22 2c20 2253 5444  d, "STDIN", "STD
-00012670: 4f55 5422 290a 0a20 2020 2020 2020 2061  OUT")..        a
-00012680: 7267 7320 3d20 5b22 2d2d 6469 6666 222c  rgs = ["--diff",
-00012690: 2022 2d2d 636f 6465 222c 2063 6f64 655d   "--code", code]
-000126a0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000126b0: 3d20 436c 6952 756e 6e65 7228 292e 696e  = CliRunner().in
-000126c0: 766f 6b65 2870 7969 6e6b 2e6d 6169 6e2c  voke(pyink.main,
-000126d0: 2061 7267 7329 0a0a 2020 2020 2020 2020   args)..        
-000126e0: 2320 5265 6d6f 7665 2074 696d 6520 6672  # Remove time fr
-000126f0: 6f6d 2064 6966 660a 2020 2020 2020 2020  om diff.        
-00012700: 6f75 7470 7574 203d 2044 4946 465f 5449  output = DIFF_TI
-00012710: 4d45 2e73 7562 2822 222c 2072 6573 756c  ME.sub("", resul
-00012720: 742e 6f75 7470 7574 290a 0a20 2020 2020  t.output)..     
-00012730: 2020 2061 7373 6572 7420 6f75 7470 7574     assert output
-00012740: 203d 3d20 7265 7375 6c74 5f64 6966 662c   == result_diff,
-00012750: 2022 5468 6520 6f75 7470 7574 2064 6964   "The output did
-00012760: 206e 6f74 206d 6174 6368 2074 6865 2065   not match the e
-00012770: 7870 6563 7465 6420 7661 6c75 652e 220a  xpected value.".
-00012780: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-00012790: 6573 756c 742e 6578 6974 5f63 6f64 6520  esult.exit_code 
-000127a0: 3d3d 2030 2c20 2254 6865 2065 7869 7420  == 0, "The exit 
-000127b0: 636f 6465 2069 7320 696e 636f 7272 6563  code is incorrec
-000127c0: 742e 220a 0a20 2020 2064 6566 2074 6573  t."..    def tes
-000127d0: 745f 636f 6465 5f6f 7074 696f 6e5f 636f  t_code_option_co
-000127e0: 6c6f 725f 6469 6666 2873 656c 6629 202d  lor_diff(self) -
-000127f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00012800: 2222 2254 6573 7420 7468 6520 636f 6465  """Test the code
-00012810: 206f 7074 696f 6e20 7768 656e 2063 6f6c   option when col
-00012820: 6f72 2061 6e64 2064 6966 6620 6172 6520  or and diff are 
-00012830: 7061 7373 6564 2e22 2222 0a20 2020 2020  passed.""".     
-00012840: 2020 2063 6f64 6520 3d20 2270 7269 6e74     code = "print
-00012850: 2827 6865 6c6c 6f20 776f 726c 6427 2922  ('hello world')"
-00012860: 0a20 2020 2020 2020 2066 6f72 6d61 7474  .        formatt
-00012870: 6564 203d 2070 7969 6e6b 2e66 6f72 6d61  ed = pyink.forma
-00012880: 745f 7374 7228 636f 6465 2c20 6d6f 6465  t_str(code, mode
-00012890: 3d44 4546 4155 4c54 5f4d 4f44 4529 0a0a  =DEFAULT_MODE)..
-000128a0: 2020 2020 2020 2020 7265 7375 6c74 5f64          result_d
-000128b0: 6966 6620 3d20 6469 6666 2863 6f64 652c  iff = diff(code,
-000128c0: 2066 6f72 6d61 7474 6564 2c20 2253 5444   formatted, "STD
-000128d0: 494e 222c 2022 5354 444f 5554 2229 0a20  IN", "STDOUT"). 
-000128e0: 2020 2020 2020 2072 6573 756c 745f 6469         result_di
-000128f0: 6666 203d 2063 6f6c 6f72 5f64 6966 6628  ff = color_diff(
-00012900: 7265 7375 6c74 5f64 6966 6629 0a0a 2020  result_diff)..  
-00012910: 2020 2020 2020 6172 6773 203d 205b 222d        args = ["-
-00012920: 2d64 6966 6622 2c20 222d 2d63 6f6c 6f72  -diff", "--color
-00012930: 222c 2022 2d2d 636f 6465 222c 2063 6f64  ", "--code", cod
-00012940: 655d 0a20 2020 2020 2020 2072 6573 756c  e].        resul
-00012950: 7420 3d20 436c 6952 756e 6e65 7228 292e  t = CliRunner().
-00012960: 696e 766f 6b65 2870 7969 6e6b 2e6d 6169  invoke(pyink.mai
-00012970: 6e2c 2061 7267 7329 0a0a 2020 2020 2020  n, args)..      
-00012980: 2020 2320 5265 6d6f 7665 2074 696d 6520    # Remove time 
-00012990: 6672 6f6d 2064 6966 660a 2020 2020 2020  from diff.      
-000129a0: 2020 6f75 7470 7574 203d 2044 4946 465f    output = DIFF_
-000129b0: 5449 4d45 2e73 7562 2822 222c 2072 6573  TIME.sub("", res
-000129c0: 756c 742e 6f75 7470 7574 290a 0a20 2020  ult.output)..   
-000129d0: 2020 2020 2061 7373 6572 7420 6f75 7470       assert outp
-000129e0: 7574 203d 3d20 7265 7375 6c74 5f64 6966  ut == result_dif
-000129f0: 662c 2022 5468 6520 6f75 7470 7574 2064  f, "The output d
-00012a00: 6964 206e 6f74 206d 6174 6368 2074 6865  id not match the
-00012a10: 2065 7870 6563 7465 6420 7661 6c75 652e   expected value.
-00012a20: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00012a30: 2072 6573 756c 742e 6578 6974 5f63 6f64   result.exit_cod
-00012a40: 6520 3d3d 2030 2c20 2254 6865 2065 7869  e == 0, "The exi
-00012a50: 7420 636f 6465 2069 7320 696e 636f 7272  t code is incorr
-00012a60: 6563 742e 220a 0a20 2020 2040 7079 7465  ect."..    @pyte
-00012a70: 7374 2e6d 6172 6b2e 696e 636f 6d70 6174  st.mark.incompat
-00012a80: 6962 6c65 5f77 6974 685f 6d79 7079 630a  ible_with_mypyc.
-00012a90: 2020 2020 6465 6620 7465 7374 5f63 6f64      def test_cod
-00012aa0: 655f 6f70 7469 6f6e 5f73 6166 6528 7365  e_option_safe(se
-00012ab0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00012ac0: 2020 2020 2022 2222 5465 7374 2074 6861       """Test tha
-00012ad0: 7420 7468 6520 636f 6465 206f 7074 696f  t the code optio
-00012ae0: 6e20 7468 726f 7773 2061 6e20 6572 726f  n throws an erro
-00012af0: 7220 7768 656e 2074 6865 2073 616e 6974  r when the sanit
-00012b00: 7920 6368 6563 6b73 2066 6169 6c2e 2222  y checks fail.""
-00012b10: 220a 2020 2020 2020 2020 2320 5061 7463  ".        # Patc
-00012b20: 6820 7079 696e 6b2e 6173 7365 7274 5f65  h pyink.assert_e
-00012b30: 7175 6976 616c 656e 7420 746f 2065 6e73  quivalent to ens
-00012b40: 7572 6520 7468 6520 7361 6e69 7479 2063  ure the sanity c
-00012b50: 6865 636b 7320 6661 696c 0a20 2020 2020  hecks fail.     
-00012b60: 2020 2077 6974 6820 7061 7463 682e 6f62     with patch.ob
-00012b70: 6a65 6374 2870 7969 6e6b 2c20 2261 7373  ject(pyink, "ass
-00012b80: 6572 745f 6571 7569 7661 6c65 6e74 222c  ert_equivalent",
-00012b90: 2073 6964 655f 6566 6665 6374 3d41 7373   side_effect=Ass
-00012ba0: 6572 7469 6f6e 4572 726f 7229 3a0a 2020  ertionError):.  
-00012bb0: 2020 2020 2020 2020 2020 636f 6465 203d            code =
-00012bc0: 2027 7072 696e 7428 2248 656c 6c6f 2077   'print("Hello w
-00012bd0: 6f72 6c64 2229 270a 2020 2020 2020 2020  orld")'.        
-00012be0: 2020 2020 6572 726f 725f 6d73 6720 3d20      error_msg = 
-00012bf0: 6622 7b63 6f64 657d 5c6e 6572 726f 723a  f"{code}\nerror:
-00012c00: 2063 616e 6e6f 7420 666f 726d 6174 203c   cannot format <
-00012c10: 7374 7269 6e67 3e3a 205c 6e22 0a0a 2020  string>: \n"..  
-00012c20: 2020 2020 2020 2020 2020 6172 6773 203d            args =
-00012c30: 205b 222d 2d73 6166 6522 2c20 222d 2d63   ["--safe", "--c
-00012c40: 6f64 6522 2c20 636f 6465 5d0a 2020 2020  ode", code].    
-00012c50: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00012c60: 2043 6c69 5275 6e6e 6572 2829 2e69 6e76   CliRunner().inv
-00012c70: 6f6b 6528 7079 696e 6b2e 6d61 696e 2c20  oke(pyink.main, 
-00012c80: 6172 6773 290a 0a20 2020 2020 2020 2020  args)..         
-00012c90: 2020 2073 656c 662e 636f 6d70 6172 655f     self.compare_
-00012ca0: 7265 7375 6c74 7328 7265 7375 6c74 2c20  results(result, 
-00012cb0: 6572 726f 725f 6d73 672c 2031 3233 290a  error_msg, 123).
-00012cc0: 0a20 2020 2064 6566 2074 6573 745f 636f  .    def test_co
-00012cd0: 6465 5f6f 7074 696f 6e5f 6661 7374 2873  de_option_fast(s
-00012ce0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00012cf0: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-00012d00: 6174 2074 6865 2063 6f64 6520 6f70 7469  at the code opti
-00012d10: 6f6e 2069 676e 6f72 6573 2065 7272 6f72  on ignores error
-00012d20: 7320 7768 656e 2074 6865 2073 616e 6974  s when the sanit
-00012d30: 7920 6368 6563 6b73 2066 6169 6c2e 2222  y checks fail.""
-00012d40: 220a 2020 2020 2020 2020 2320 5061 7463  ".        # Patc
-00012d50: 6820 7079 696e 6b2e 6173 7365 7274 5f65  h pyink.assert_e
-00012d60: 7175 6976 616c 656e 7420 746f 2065 6e73  quivalent to ens
-00012d70: 7572 6520 7468 6520 7361 6e69 7479 2063  ure the sanity c
-00012d80: 6865 636b 7320 6661 696c 0a20 2020 2020  hecks fail.     
-00012d90: 2020 2077 6974 6820 7061 7463 682e 6f62     with patch.ob
-00012da0: 6a65 6374 2870 7969 6e6b 2c20 2261 7373  ject(pyink, "ass
-00012db0: 6572 745f 6571 7569 7661 6c65 6e74 222c  ert_equivalent",
-00012dc0: 2073 6964 655f 6566 6665 6374 3d41 7373   side_effect=Ass
-00012dd0: 6572 7469 6f6e 4572 726f 7229 3a0a 2020  ertionError):.  
-00012de0: 2020 2020 2020 2020 2020 636f 6465 203d            code =
-00012df0: 2027 7072 696e 7428 2248 656c 6c6f 2077   'print("Hello w
-00012e00: 6f72 6c64 2229 270a 2020 2020 2020 2020  orld")'.        
-00012e10: 2020 2020 666f 726d 6174 7465 6420 3d20      formatted = 
-00012e20: 7079 696e 6b2e 666f 726d 6174 5f73 7472  pyink.format_str
-00012e30: 2863 6f64 652c 206d 6f64 653d 4445 4641  (code, mode=DEFA
-00012e40: 554c 545f 4d4f 4445 290a 0a20 2020 2020  ULT_MODE)..     
-00012e50: 2020 2020 2020 2061 7267 7320 3d20 5b22         args = ["
-00012e60: 2d2d 6661 7374 222c 2022 2d2d 636f 6465  --fast", "--code
-00012e70: 222c 2063 6f64 655d 0a20 2020 2020 2020  ", code].       
-00012e80: 2020 2020 2072 6573 756c 7420 3d20 436c       result = Cl
-00012e90: 6952 756e 6e65 7228 292e 696e 766f 6b65  iRunner().invoke
-00012ea0: 2870 7969 6e6b 2e6d 6169 6e2c 2061 7267  (pyink.main, arg
-00012eb0: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
-00012ec0: 7365 6c66 2e63 6f6d 7061 7265 5f72 6573  self.compare_res
-00012ed0: 756c 7473 2872 6573 756c 742c 2066 6f72  ults(result, for
-00012ee0: 6d61 7474 6564 2c20 3029 0a0a 2020 2020  matted, 0)..    
-00012ef0: 4070 7974 6573 742e 6d61 726b 2e69 6e63  @pytest.mark.inc
-00012f00: 6f6d 7061 7469 626c 655f 7769 7468 5f6d  ompatible_with_m
-00012f10: 7970 7963 0a20 2020 2064 6566 2074 6573  ypyc.    def tes
-00012f20: 745f 636f 6465 5f6f 7074 696f 6e5f 636f  t_code_option_co
-00012f30: 6e66 6967 2873 656c 6629 202d 3e20 4e6f  nfig(self) -> No
-00012f40: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00012f50: 2020 2020 2020 2020 5465 7374 2074 6861          Test tha
-00012f60: 7420 7468 6520 636f 6465 206f 7074 696f  t the code optio
-00012f70: 6e20 6669 6e64 7320 7468 6520 7079 7072  n finds the pypr
-00012f80: 6f6a 6563 742e 746f 6d6c 2069 6e20 7468  oject.toml in th
-00012f90: 6520 6375 7272 656e 7420 6469 7265 6374  e current direct
-00012fa0: 6f72 792e 0a20 2020 2020 2020 2022 2222  ory..        """
-00012fb0: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
-00012fc0: 7463 682e 6f62 6a65 6374 2870 7969 6e6b  tch.object(pyink
-00012fd0: 2c20 2270 6172 7365 5f70 7970 726f 6a65  , "parse_pyproje
-00012fe0: 6374 5f74 6f6d 6c22 2c20 7265 7475 726e  ct_toml", return
-00012ff0: 5f76 616c 7565 3d7b 7d29 2061 7320 7061  _value={}) as pa
-00013000: 7273 653a 0a20 2020 2020 2020 2020 2020  rse:.           
-00013010: 2061 7267 7320 3d20 5b22 2d2d 636f 6465   args = ["--code
-00013020: 222c 2022 7072 696e 7422 5d0a 2020 2020  ", "print"].    
-00013030: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
-00013040: 7320 7468 6520 6f6e 6c79 2064 6972 6563  s the only direc
-00013050: 746f 7279 206b 6e6f 776e 2074 6f20 636f  tory known to co
-00013060: 6e74 6169 6e20 6120 7079 7072 6f6a 6563  ntain a pyprojec
-00013070: 742e 746f 6d6c 0a20 2020 2020 2020 2020  t.toml.         
-00013080: 2020 2077 6974 6820 6368 616e 6765 5f64     with change_d
-00013090: 6972 6563 746f 7279 2850 524f 4a45 4354  irectory(PROJECT
-000130a0: 5f52 4f4f 5429 3a0a 2020 2020 2020 2020  _ROOT):.        
-000130b0: 2020 2020 2020 2020 436c 6952 756e 6e65          CliRunne
-000130c0: 7228 292e 696e 766f 6b65 2870 7969 6e6b  r().invoke(pyink
-000130d0: 2e6d 6169 6e2c 2061 7267 7329 0a20 2020  .main, args).   
-000130e0: 2020 2020 2020 2020 2020 2020 2070 7970               pyp
-000130f0: 726f 6a65 6374 5f70 6174 6820 3d20 5061  roject_path = Pa
-00013100: 7468 2850 6174 682e 6377 6428 292c 2022  th(Path.cwd(), "
-00013110: 7079 7072 6f6a 6563 742e 746f 6d6c 2229  pyproject.toml")
-00013120: 2e72 6573 6f6c 7665 2829 0a0a 2020 2020  .resolve()..    
-00013130: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
-00013140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013150: 206c 656e 2870 6172 7365 2e6d 6f63 6b5f   len(parse.mock_
-00013160: 6361 6c6c 7329 203e 3d20 310a 2020 2020  calls) >= 1.    
-00013170: 2020 2020 2020 2020 292c 2022 4578 7065          ), "Expe
-00013180: 6374 6564 2063 6f6e 6669 6720 7061 7273  cted config pars
-00013190: 6520 746f 2062 6520 6361 6c6c 6564 2077  e to be called w
-000131a0: 6974 6820 7468 6520 6375 7272 656e 7420  ith the current 
-000131b0: 6469 7265 6374 6f72 792e 220a 0a20 2020  directory."..   
-000131c0: 2020 2020 2020 2020 205f 2c20 6361 6c6c           _, call
-000131d0: 5f61 7267 732c 205f 203d 2070 6172 7365  _args, _ = parse
-000131e0: 2e6d 6f63 6b5f 6361 6c6c 735b 305d 0a20  .mock_calls[0]. 
-000131f0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00013200: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
-00013210: 2020 2020 6361 6c6c 5f61 7267 735b 305d      call_args[0]
-00013220: 2e6c 6f77 6572 2829 203d 3d20 7374 7228  .lower() == str(
-00013230: 7079 7072 6f6a 6563 745f 7061 7468 292e  pyproject_path).
-00013240: 6c6f 7765 7228 290a 2020 2020 2020 2020  lower().        
-00013250: 2020 2020 292c 2022 496e 636f 7272 6563      ), "Incorrec
-00013260: 7420 636f 6e66 6967 206c 6f61 6465 642e  t config loaded.
-00013270: 220a 0a20 2020 2040 7079 7465 7374 2e6d  "..    @pytest.m
-00013280: 6172 6b2e 696e 636f 6d70 6174 6962 6c65  ark.incompatible
-00013290: 5f77 6974 685f 6d79 7079 630a 2020 2020  _with_mypyc.    
-000132a0: 6465 6620 7465 7374 5f63 6f64 655f 6f70  def test_code_op
-000132b0: 7469 6f6e 5f70 6172 656e 745f 636f 6e66  tion_parent_conf
-000132c0: 6967 2873 656c 6629 202d 3e20 4e6f 6e65  ig(self) -> None
-000132d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000132e0: 2020 2020 2020 5465 7374 2074 6861 7420        Test that 
-000132f0: 7468 6520 636f 6465 206f 7074 696f 6e20  the code option 
-00013300: 6669 6e64 7320 7468 6520 7079 7072 6f6a  finds the pyproj
-00013310: 6563 742e 746f 6d6c 2069 6e20 7468 6520  ect.toml in the 
-00013320: 7061 7265 6e74 2064 6972 6563 746f 7279  parent directory
-00013330: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00013340: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
-00013350: 2e6f 626a 6563 7428 7079 696e 6b2c 2022  .object(pyink, "
-00013360: 7061 7273 655f 7079 7072 6f6a 6563 745f  parse_pyproject_
-00013370: 746f 6d6c 222c 2072 6574 7572 6e5f 7661  toml", return_va
-00013380: 6c75 653d 7b7d 2920 6173 2070 6172 7365  lue={}) as parse
-00013390: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-000133a0: 7468 2063 6861 6e67 655f 6469 7265 6374  th change_direct
-000133b0: 6f72 7928 5448 4953 5f44 4952 293a 0a20  ory(THIS_DIR):. 
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000133d0: 7267 7320 3d20 5b22 2d2d 636f 6465 222c  rgs = ["--code",
-000133e0: 2022 7072 696e 7422 5d0a 2020 2020 2020   "print"].      
-000133f0: 2020 2020 2020 2020 2020 436c 6952 756e            CliRun
-00013400: 6e65 7228 292e 696e 766f 6b65 2870 7969  ner().invoke(pyi
-00013410: 6e6b 2e6d 6169 6e2c 2061 7267 7329 0a0a  nk.main, args)..
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 7079 7072 6f6a 6563 745f 7061 7468 203d  pyproject_path =
-00013440: 2050 6174 6828 5061 7468 2829 2e63 7764   Path(Path().cwd
-00013450: 2829 2e70 6172 656e 742c 2022 7079 7072  ().parent, "pypr
-00013460: 6f6a 6563 742e 746f 6d6c 2229 2e72 6573  oject.toml").res
-00013470: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
-00013480: 2020 2020 2020 2061 7373 6572 7420 280a         assert (.
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 2020 6c65 6e28 7061 7273 652e 6d6f      len(parse.mo
-000134b0: 636b 5f63 616c 6c73 2920 3e3d 2031 0a20  ck_calls) >= 1. 
-000134c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000134d0: 2c20 2245 7870 6563 7465 6420 636f 6e66  , "Expected conf
-000134e0: 6967 2070 6172 7365 2074 6f20 6265 2063  ig parse to be c
-000134f0: 616c 6c65 6420 7769 7468 2074 6865 2063  alled with the c
-00013500: 7572 7265 6e74 2064 6972 6563 746f 7279  urrent directory
-00013510: 2e22 0a0a 2020 2020 2020 2020 2020 2020  ."..            
-00013520: 2020 2020 5f2c 2063 616c 6c5f 6172 6773      _, call_args
-00013530: 2c20 5f20 3d20 7061 7273 652e 6d6f 636b  , _ = parse.mock
-00013540: 5f63 616c 6c73 5b30 5d0a 2020 2020 2020  _calls[0].      
-00013550: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00013560: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00013570: 2020 2020 2020 2063 616c 6c5f 6172 6773         call_args
-00013580: 5b30 5d2e 6c6f 7765 7228 2920 3d3d 2073  [0].lower() == s
-00013590: 7472 2870 7970 726f 6a65 6374 5f70 6174  tr(pyproject_pat
-000135a0: 6829 2e6c 6f77 6572 2829 0a20 2020 2020  h).lower().     
-000135b0: 2020 2020 2020 2020 2020 2029 2c20 2249             ), "I
-000135c0: 6e63 6f72 7265 6374 2063 6f6e 6669 6720  ncorrect config 
-000135d0: 6c6f 6164 6564 2e22 0a0a 2020 2020 6465  loaded."..    de
-000135e0: 6620 7465 7374 5f66 6f72 5f68 616e 646c  f test_for_handl
-000135f0: 6564 5f75 6e65 7870 6563 7465 645f 656f  ed_unexpected_eo
-00013600: 665f 6572 726f 7228 7365 6c66 2920 2d3e  f_error(self) ->
-00013610: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00013620: 2222 0a20 2020 2020 2020 2054 6573 7420  "".        Test 
-00013630: 7468 6174 2061 6e20 756e 6578 7065 6374  that an unexpect
-00013640: 6564 2045 4f46 2053 796e 7461 7845 7272  ed EOF SyntaxErr
-00013650: 6f72 2069 7320 6e69 6365 6c79 2070 7265  or is nicely pre
-00013660: 7365 6e74 6564 2e0a 2020 2020 2020 2020  sented..        
-00013670: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
-00013680: 2070 7974 6573 742e 7261 6973 6573 2870   pytest.raises(p
-00013690: 7969 6e6b 2e70 6172 7369 6e67 2e49 6e76  yink.parsing.Inv
-000136a0: 616c 6964 496e 7075 7429 2061 7320 6578  alidInput) as ex
-000136b0: 635f 696e 666f 3a0a 2020 2020 2020 2020  c_info:.        
-000136c0: 2020 2020 7079 696e 6b2e 6c69 6232 746f      pyink.lib2to
-000136d0: 335f 7061 7273 6528 2270 7269 6e74 2822  3_parse("print("
-000136e0: 2c20 7b7d 290a 0a20 2020 2020 2020 2065  , {})..        e
-000136f0: 7863 5f69 6e66 6f2e 6d61 7463 6828 2243  xc_info.match("C
-00013700: 616e 6e6f 7420 7061 7273 653a 2032 3a30  annot parse: 2:0
-00013710: 3a20 454f 4620 696e 206d 756c 7469 2d6c  : EOF in multi-l
-00013720: 696e 6520 7374 6174 656d 656e 7422 290a  ine statement").
-00013730: 0a20 2020 2064 6566 2074 6573 745f 6571  .    def test_eq
-00013740: 7569 7661 6c65 6e63 795f 6173 745f 7061  uivalency_ast_pa
-00013750: 7273 655f 6661 696c 7572 655f 696e 636c  rse_failure_incl
-00013760: 7564 6573 5f65 7272 6f72 2873 656c 6629  udes_error(self)
-00013770: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00013780: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
-00013790: 6973 6573 2841 7373 6572 7469 6f6e 4572  ises(AssertionEr
-000137a0: 726f 7229 2061 7320 6572 723a 0a20 2020  ror) as err:.   
-000137b0: 2020 2020 2020 2020 2070 7969 6e6b 2e61           pyink.a
-000137c0: 7373 6572 745f 6571 7569 7661 6c65 6e74  ssert_equivalent
-000137d0: 2822 61c2 abc2 bb61 2020 3d20 3122 2c20  ("a....a  = 1", 
-000137e0: 2261 c2ab c2bb 6120 203d 2031 2229 0a0a  "a....a  = 1")..
-000137f0: 2020 2020 2020 2020 6572 722e 6d61 7463          err.matc
-00013800: 6828 222d 2d73 6166 6522 290a 2020 2020  h("--safe").    
-00013810: 2020 2020 2320 556e 666f 7274 756e 6174      # Unfortunat
-00013820: 656c 7920 7468 6520 5379 6e74 6178 4572  ely the SyntaxEr
-00013830: 726f 7220 6d65 7373 6167 6520 6861 7320  ror message has 
-00013840: 6368 616e 6765 6420 696e 206e 6577 6572  changed in newer
-00013850: 2076 6572 7369 6f6e 7320 736f 2077 650a   versions so we.
-00013860: 2020 2020 2020 2020 2320 6361 6e27 7420          # can't 
-00013870: 6d61 7463 6820 6974 2064 6972 6563 746c  match it directl
-00013880: 792e 0a20 2020 2020 2020 2065 7272 2e6d  y..        err.m
-00013890: 6174 6368 2822 696e 7661 6c69 6420 6368  atch("invalid ch
-000138a0: 6172 6163 7465 7222 290a 2020 2020 2020  aracter").      
-000138b0: 2020 6572 722e 6d61 7463 6828 7222 5c28    err.match(r"\(
-000138c0: 3c75 6e6b 6e6f 776e 3e2c 206c 696e 6520  <unknown>, line 
-000138d0: 315c 2922 290a 0a0a 636c 6173 7320 5465  1\)")...class Te
-000138e0: 7374 4361 6368 696e 673a 0a20 2020 2064  stCaching:.    d
-000138f0: 6566 2074 6573 745f 6765 745f 6361 6368  ef test_get_cach
-00013900: 655f 6469 7228 0a20 2020 2020 2020 2073  e_dir(.        s
-00013910: 656c 662c 0a20 2020 2020 2020 2074 6d70  elf,.        tmp
-00013920: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
-00013930: 2020 2020 206d 6f6e 6b65 7970 6174 6368       monkeypatch
-00013940: 3a20 7079 7465 7374 2e4d 6f6e 6b65 7950  : pytest.MonkeyP
-00013950: 6174 6368 2c0a 2020 2020 2920 2d3e 204e  atch,.    ) -> N
-00013960: 6f6e 653a 0a20 2020 2020 2020 2023 2043  one:.        # C
-00013970: 7265 6174 6520 6d75 6c74 6970 6c65 2063  reate multiple c
-00013980: 6163 6865 2064 6972 6563 746f 7269 6573  ache directories
-00013990: 0a20 2020 2020 2020 2077 6f72 6b73 7061  .        workspa
-000139a0: 6365 3120 3d20 746d 705f 7061 7468 202f  ce1 = tmp_path /
-000139b0: 2022 7773 3122 0a20 2020 2020 2020 2077   "ws1".        w
-000139c0: 6f72 6b73 7061 6365 312e 6d6b 6469 7228  orkspace1.mkdir(
-000139d0: 290a 2020 2020 2020 2020 776f 726b 7370  ).        worksp
-000139e0: 6163 6532 203d 2074 6d70 5f70 6174 6820  ace2 = tmp_path 
-000139f0: 2f20 2277 7332 220a 2020 2020 2020 2020  / "ws2".        
-00013a00: 776f 726b 7370 6163 6532 2e6d 6b64 6972  workspace2.mkdir
-00013a10: 2829 0a0a 2020 2020 2020 2020 2320 466f  ()..        # Fo
-00013a20: 7263 6520 7573 6572 5f63 6163 6865 5f64  rce user_cache_d
-00013a30: 6972 2074 6f20 7573 6520 7468 6520 7465  ir to use the te
-00013a40: 6d70 6f72 6172 7920 6469 7265 6374 6f72  mporary director
-00013a50: 7920 666f 7220 6561 7369 6572 2061 7373  y for easier ass
-00013a60: 6572 7469 6f6e 730a 2020 2020 2020 2020  ertions.        
-00013a70: 7061 7463 685f 7573 6572 5f63 6163 6865  patch_user_cache
-00013a80: 5f64 6972 203d 2070 6174 6368 280a 2020  _dir = patch(.  
-00013a90: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00013aa0: 3d22 7079 696e 6b2e 6361 6368 652e 7573  ="pyink.cache.us
-00013ab0: 6572 5f63 6163 6865 5f64 6972 222c 0a20  er_cache_dir",. 
-00013ac0: 2020 2020 2020 2020 2020 2061 7574 6f73             autos
-00013ad0: 7065 633d 5472 7565 2c0a 2020 2020 2020  pec=True,.      
-00013ae0: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
-00013af0: 7565 3d73 7472 2877 6f72 6b73 7061 6365  ue=str(workspace
-00013b00: 3129 2c0a 2020 2020 2020 2020 290a 0a20  1),.        ).. 
-00013b10: 2020 2020 2020 2023 2049 6620 5059 494e         # If PYIN
-00013b20: 4b5f 4341 4348 455f 4449 5220 6973 206e  K_CACHE_DIR is n
-00013b30: 6f74 2073 6574 2c20 7573 6520 7573 6572  ot set, use user
-00013b40: 5f63 6163 6865 5f64 6972 0a20 2020 2020  _cache_dir.     
-00013b50: 2020 206d 6f6e 6b65 7970 6174 6368 2e64     monkeypatch.d
-00013b60: 656c 656e 7628 2250 5949 4e4b 5f43 4143  elenv("PYINK_CAC
-00013b70: 4845 5f44 4952 222c 2072 6169 7369 6e67  HE_DIR", raising
-00013b80: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00013b90: 7769 7468 2070 6174 6368 5f75 7365 725f  with patch_user_
-00013ba0: 6361 6368 655f 6469 723a 0a20 2020 2020  cache_dir:.     
-00013bb0: 2020 2020 2020 2061 7373 6572 7420 6765         assert ge
-00013bc0: 745f 6361 6368 655f 6469 7228 2920 3d3d  t_cache_dir() ==
-00013bd0: 2077 6f72 6b73 7061 6365 310a 0a20 2020   workspace1..   
-00013be0: 2020 2020 2023 2049 6620 6974 2069 7320       # If it is 
-00013bf0: 7365 742c 2075 7365 2074 6865 2070 6174  set, use the pat
-00013c00: 6820 7072 6f76 6964 6564 2069 6e20 7468  h provided in th
-00013c10: 6520 656e 7620 7661 722e 0a20 2020 2020  e env var..     
-00013c20: 2020 206d 6f6e 6b65 7970 6174 6368 2e73     monkeypatch.s
-00013c30: 6574 656e 7628 2250 5949 4e4b 5f43 4143  etenv("PYINK_CAC
-00013c40: 4845 5f44 4952 222c 2073 7472 2877 6f72  HE_DIR", str(wor
-00013c50: 6b73 7061 6365 3229 290a 2020 2020 2020  kspace2)).      
-00013c60: 2020 6173 7365 7274 2067 6574 5f63 6163    assert get_cac
-00013c70: 6865 5f64 6972 2829 203d 3d20 776f 726b  he_dir() == work
-00013c80: 7370 6163 6532 0a0a 2020 2020 6465 6620  space2..    def 
-00013c90: 7465 7374 5f63 6163 6865 5f62 726f 6b65  test_cache_broke
-00013ca0: 6e5f 6669 6c65 2873 656c 6629 202d 3e20  n_file(self) -> 
-00013cb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6d6f  None:.        mo
-00013cc0: 6465 203d 2044 4546 4155 4c54 5f4d 4f44  de = DEFAULT_MOD
-00013cd0: 450a 2020 2020 2020 2020 7769 7468 2063  E.        with c
-00013ce0: 6163 6865 5f64 6972 2829 2061 7320 776f  ache_dir() as wo
-00013cf0: 726b 7370 6163 653a 0a20 2020 2020 2020  rkspace:.       
-00013d00: 2020 2020 2063 6163 6865 5f66 696c 6520       cache_file 
-00013d10: 3d20 6765 745f 6361 6368 655f 6669 6c65  = get_cache_file
-00013d20: 286d 6f64 6529 0a20 2020 2020 2020 2020  (mode).         
-00013d30: 2020 2063 6163 6865 5f66 696c 652e 7772     cache_file.wr
-00013d40: 6974 655f 7465 7874 2822 7468 6973 2069  ite_text("this i
-00013d50: 7320 6e6f 7420 6120 7069 636b 6c65 2229  s not a pickle")
-00013d60: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00013d70: 6572 7420 7079 696e 6b2e 7265 6164 5f63  ert pyink.read_c
-00013d80: 6163 6865 286d 6f64 6529 203d 3d20 7b7d  ache(mode) == {}
+00005850: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005860: 3120 6669 6c65 2072 6566 6f72 6d61 7474  1 file reformatt
+00005870: 6564 2c20 3220 6669 6c65 7320 6c65 6674  ed, 2 files left
+00005880: 2075 6e63 6861 6e67 6564 2c20 3120 6669   unchanged, 1 fi
+00005890: 6c65 2066 6169 6c65 6420 746f 220a 2020  le failed to".  
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+000058b0: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+000058c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000058d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000058e0: 7445 7175 616c 2872 6570 6f72 742e 7265  tEqual(report.re
+000058f0: 7475 726e 5f63 6f64 652c 2031 3233 290a  turn_code, 123).
+00005900: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00005910: 7274 2e64 6f6e 6528 5061 7468 2822 6633  rt.done(Path("f3
+00005920: 2229 2c20 7079 696e 6b2e 4368 616e 6765  "), pyink.Change
+00005930: 642e 5945 5329 0a20 2020 2020 2020 2020  d.YES).         
+00005940: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005950: 7561 6c28 6c65 6e28 6f75 745f 6c69 6e65  ual(len(out_line
+00005960: 7329 2c20 3429 0a20 2020 2020 2020 2020  s), 4).         
+00005970: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005980: 7561 6c28 6c65 6e28 6572 725f 6c69 6e65  ual(len(err_line
+00005990: 7329 2c20 3129 0a20 2020 2020 2020 2020  s), 1).         
+000059a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000059b0: 7561 6c28 6f75 745f 6c69 6e65 735b 2d31  ual(out_lines[-1
+000059c0: 5d2c 2022 7265 666f 726d 6174 7465 6420  ], "reformatted 
+000059d0: 6633 2229 0a20 2020 2020 2020 2020 2020  f3").           
+000059e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000059f0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00005a00: 2020 2075 6e73 7479 6c65 2873 7472 2872     unstyle(str(r
+00005a10: 6570 6f72 7429 292c 0a20 2020 2020 2020  eport)),.       
+00005a20: 2020 2020 2020 2020 2022 3220 6669 6c65           "2 file
+00005a30: 7320 7265 666f 726d 6174 7465 642c 2032  s reformatted, 2
+00005a40: 2066 696c 6573 206c 6566 7420 756e 6368   files left unch
+00005a50: 616e 6765 642c 2031 2066 696c 6520 6661  anged, 1 file fa
+00005a60: 696c 6564 2074 6f22 0a20 2020 2020 2020  iled to".       
+00005a70: 2020 2020 2020 2020 2022 2072 6566 6f72           " refor
+00005a80: 6d61 742e 222c 0a20 2020 2020 2020 2020  mat.",.         
+00005a90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00005aa0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00005ab0: 6c28 7265 706f 7274 2e72 6574 7572 6e5f  l(report.return_
+00005ac0: 636f 6465 2c20 3132 3329 0a20 2020 2020  code, 123).     
+00005ad0: 2020 2020 2020 2072 6570 6f72 742e 6661         report.fa
+00005ae0: 696c 6564 2850 6174 6828 2265 3222 292c  iled(Path("e2"),
+00005af0: 2022 626f 6f6d 2229 0a20 2020 2020 2020   "boom").       
+00005b00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00005b10: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
+00005b20: 6e65 7329 2c20 3429 0a20 2020 2020 2020  nes), 4).       
+00005b30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00005b40: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
+00005b50: 6e65 7329 2c20 3229 0a20 2020 2020 2020  nes), 2).       
+00005b60: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00005b70: 4571 7561 6c28 6572 725f 6c69 6e65 735b  Equal(err_lines[
+00005b80: 2d31 5d2c 2022 6572 726f 723a 2063 616e  -1], "error: can
+00005b90: 6e6f 7420 666f 726d 6174 2065 323a 2062  not format e2: b
+00005ba0: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
+00005bb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005bc0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00005bd0: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
+00005be0: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
+00005bf0: 2020 2020 2020 2020 2020 2232 2066 696c            "2 fil
+00005c00: 6573 2072 6566 6f72 6d61 7474 6564 2c20  es reformatted, 
+00005c10: 3220 6669 6c65 7320 6c65 6674 2075 6e63  2 files left unc
+00005c20: 6861 6e67 6564 2c20 3220 6669 6c65 7320  hanged, 2 files 
+00005c30: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
+00005c40: 2020 2020 2020 2020 2020 2022 2072 6566             " ref
+00005c50: 6f72 6d61 742e 222c 0a20 2020 2020 2020  ormat.",.       
+00005c60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005c70: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005c80: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
+00005c90: 6e5f 636f 6465 2c20 3132 3329 0a20 2020  n_code, 123).   
+00005ca0: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
+00005cb0: 7061 7468 5f69 676e 6f72 6564 2850 6174  path_ignored(Pat
+00005cc0: 6828 2277 6174 2229 2c20 226e 6f20 6d61  h("wat"), "no ma
+00005cd0: 7463 6822 290a 2020 2020 2020 2020 2020  tch").          
+00005ce0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005cf0: 616c 286c 656e 286f 7574 5f6c 696e 6573  al(len(out_lines
+00005d00: 292c 2035 290a 2020 2020 2020 2020 2020  ), 5).          
+00005d10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005d20: 616c 286c 656e 2865 7272 5f6c 696e 6573  al(len(err_lines
+00005d30: 292c 2032 290a 2020 2020 2020 2020 2020  ), 2).          
+00005d40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00005d50: 616c 286f 7574 5f6c 696e 6573 5b2d 315d  al(out_lines[-1]
+00005d60: 2c20 2277 6174 2069 676e 6f72 6564 3a20  , "wat ignored: 
+00005d70: 6e6f 206d 6174 6368 2229 0a20 2020 2020  no match").     
+00005d80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00005d90: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00005da0: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
+00005db0: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005dd0: 3220 6669 6c65 7320 7265 666f 726d 6174  2 files reformat
+00005de0: 7465 642c 2032 2066 696c 6573 206c 6566  ted, 2 files lef
+00005df0: 7420 756e 6368 616e 6765 642c 2032 2066  t unchanged, 2 f
+00005e00: 696c 6573 2066 6169 6c65 6420 746f 220a  iles failed to".
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2220 7265 666f 726d 6174 2e22 2c0a 2020  " reformat.",.  
+00005e30: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00005e40: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00005e50: 6572 7445 7175 616c 2872 6570 6f72 742e  ertEqual(report.
+00005e60: 7265 7475 726e 5f63 6f64 652c 2031 3233  return_code, 123
+00005e70: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00005e80: 706f 7274 2e64 6f6e 6528 5061 7468 2822  port.done(Path("
+00005e90: 6634 2229 2c20 7079 696e 6b2e 4368 616e  f4"), pyink.Chan
+00005ea0: 6765 642e 4e4f 290a 2020 2020 2020 2020  ged.NO).        
+00005eb0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00005ec0: 7175 616c 286c 656e 286f 7574 5f6c 696e  qual(len(out_lin
+00005ed0: 6573 292c 2036 290a 2020 2020 2020 2020  es), 6).        
+00005ee0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00005ef0: 7175 616c 286c 656e 2865 7272 5f6c 696e  qual(len(err_lin
+00005f00: 6573 292c 2032 290a 2020 2020 2020 2020  es), 2).        
+00005f10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00005f20: 7175 616c 286f 7574 5f6c 696e 6573 5b2d  qual(out_lines[-
+00005f30: 315d 2c20 2266 3420 616c 7265 6164 7920  1], "f4 already 
+00005f40: 7765 6c6c 2066 6f72 6d61 7474 6564 2c20  well formatted, 
+00005f50: 676f 6f64 206a 6f62 2e22 290a 2020 2020  good job.").    
+00005f60: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00005f70: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00005f80: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00005f90: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
+00005fc0: 7474 6564 2c20 3320 6669 6c65 7320 6c65  tted, 3 files le
+00005fd0: 6674 2075 6e63 6861 6e67 6564 2c20 3220  ft unchanged, 2 
+00005fe0: 6669 6c65 7320 6661 696c 6564 2074 6f22  files failed to"
+00005ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006000: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
+00006010: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006020: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006030: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00006040: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
+00006050: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
+00006060: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
+00006070: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+00006080: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00006090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060a0: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+000060b0: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+000060c0: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+000060d0: 776f 756c 6420 6265 2072 6566 6f72 6d61  would be reforma
+000060e0: 7474 6564 2c20 3320 6669 6c65 7320 776f  tted, 3 files wo
+000060f0: 756c 6420 6265 206c 6566 7420 756e 6368  uld be left unch
+00006100: 616e 6765 642c 2032 220a 2020 2020 2020  anged, 2".      
+00006110: 2020 2020 2020 2020 2020 2220 6669 6c65            " file
+00006120: 7320 776f 756c 6420 6661 696c 2074 6f20  s would fail to 
+00006130: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+00006140: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00006150: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
+00006160: 636b 203d 2046 616c 7365 0a20 2020 2020  ck = False.     
+00006170: 2020 2020 2020 2072 6570 6f72 742e 6469         report.di
+00006180: 6666 203d 2054 7275 650a 2020 2020 2020  ff = True.      
+00006190: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000061a0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+000061b0: 2020 2020 2020 2020 756e 7374 796c 6528          unstyle(
+000061c0: 7374 7228 7265 706f 7274 2929 2c0a 2020  str(report)),.  
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2232                "2
+000061e0: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
+000061f0: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
+00006200: 696c 6573 2077 6f75 6c64 2062 6520 6c65  iles would be le
+00006210: 6674 2075 6e63 6861 6e67 6564 2c20 3222  ft unchanged, 2"
+00006220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006230: 2022 2066 696c 6573 2077 6f75 6c64 2066   " files would f
+00006240: 6169 6c20 746f 2072 6566 6f72 6d61 742e  ail to reformat.
+00006250: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00006260: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
+00006270: 6570 6f72 745f 7175 6965 7428 7365 6c66  eport_quiet(self
+00006280: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00006290: 2020 2072 6570 6f72 7420 3d20 5265 706f     report = Repo
+000062a0: 7274 2871 7569 6574 3d54 7275 6529 0a20  rt(quiet=True). 
+000062b0: 2020 2020 2020 206f 7574 5f6c 696e 6573         out_lines
+000062c0: 203d 205b 5d0a 2020 2020 2020 2020 6572   = [].        er
+000062d0: 725f 6c69 6e65 7320 3d20 5b5d 0a0a 2020  r_lines = []..  
+000062e0: 2020 2020 2020 6465 6620 6f75 7428 6d73        def out(ms
+000062f0: 673a 2073 7472 2c20 2a2a 6b77 6172 6773  g: str, **kwargs
+00006300: 3a20 416e 7929 202d 3e20 4e6f 6e65 3a0a  : Any) -> None:.
+00006310: 2020 2020 2020 2020 2020 2020 6f75 745f              out_
+00006320: 6c69 6e65 732e 6170 7065 6e64 286d 7367  lines.append(msg
+00006330: 290a 0a20 2020 2020 2020 2064 6566 2065  )..        def e
+00006340: 7272 286d 7367 3a20 7374 722c 202a 2a6b  rr(msg: str, **k
+00006350: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+00006360: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006370: 2065 7272 5f6c 696e 6573 2e61 7070 656e   err_lines.appen
+00006380: 6428 6d73 6729 0a0a 2020 2020 2020 2020  d(msg)..        
+00006390: 7769 7468 2070 6174 6368 2822 7079 696e  with patch("pyin
+000063a0: 6b2e 6f75 7470 7574 2e5f 6f75 7422 2c20  k.output._out", 
+000063b0: 6f75 7429 2c20 7061 7463 6828 2270 7969  out), patch("pyi
+000063c0: 6e6b 2e6f 7574 7075 742e 5f65 7272 222c  nk.output._err",
+000063d0: 2065 7272 293a 0a20 2020 2020 2020 2020   err):.         
+000063e0: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
+000063f0: 6174 6828 2266 3122 292c 2070 7969 6e6b  ath("f1"), pyink
+00006400: 2e43 6861 6e67 6564 2e4e 4f29 0a20 2020  .Changed.NO).   
+00006410: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006420: 7365 7274 4571 7561 6c28 6c65 6e28 6f75  sertEqual(len(ou
+00006430: 745f 6c69 6e65 7329 2c20 3029 0a20 2020  t_lines), 0).   
+00006440: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006450: 7365 7274 4571 7561 6c28 6c65 6e28 6572  sertEqual(len(er
+00006460: 725f 6c69 6e65 7329 2c20 3029 0a20 2020  r_lines), 0).   
+00006470: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006480: 7365 7274 4571 7561 6c28 756e 7374 796c  sertEqual(unstyl
+00006490: 6528 7374 7228 7265 706f 7274 2929 2c20  e(str(report)), 
+000064a0: 2231 2066 696c 6520 6c65 6674 2075 6e63  "1 file left unc
+000064b0: 6861 6e67 6564 2e22 290a 2020 2020 2020  hanged.").      
+000064c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000064d0: 7445 7175 616c 2872 6570 6f72 742e 7265  tEqual(report.re
+000064e0: 7475 726e 5f63 6f64 652c 2030 290a 2020  turn_code, 0).  
+000064f0: 2020 2020 2020 2020 2020 7265 706f 7274            report
+00006500: 2e64 6f6e 6528 5061 7468 2822 6632 2229  .done(Path("f2")
+00006510: 2c20 7079 696e 6b2e 4368 616e 6765 642e  , pyink.Changed.
+00006520: 5945 5329 0a20 2020 2020 2020 2020 2020  YES).           
+00006530: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00006540: 6c28 6c65 6e28 6f75 745f 6c69 6e65 7329  l(len(out_lines)
+00006550: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+00006560: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00006570: 6c28 6c65 6e28 6572 725f 6c69 6e65 7329  l(len(err_lines)
+00006580: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+00006590: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000065a0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+000065b0: 2020 2075 6e73 7479 6c65 2873 7472 2872     unstyle(str(r
+000065c0: 6570 6f72 7429 292c 2022 3120 6669 6c65  eport)), "1 file
+000065d0: 2072 6566 6f72 6d61 7474 6564 2c20 3120   reformatted, 1 
+000065e0: 6669 6c65 206c 6566 7420 756e 6368 616e  file left unchan
+000065f0: 6765 642e 220a 2020 2020 2020 2020 2020  ged.".          
+00006600: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00006610: 7265 706f 7274 2e64 6f6e 6528 5061 7468  report.done(Path
+00006620: 2822 6633 2229 2c20 7079 696e 6b2e 4368  ("f3"), pyink.Ch
+00006630: 616e 6765 642e 4341 4348 4544 290a 2020  anged.CACHED).  
+00006640: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006650: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00006660: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
+00006670: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006680: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00006690: 7272 5f6c 696e 6573 292c 2030 290a 2020  rr_lines), 0).  
+000066a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000066b0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+000066c0: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+000066d0: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+000066e0: 2c20 2231 2066 696c 6520 7265 666f 726d  , "1 file reform
+000066f0: 6174 7465 642c 2032 2066 696c 6573 206c  atted, 2 files l
+00006700: 6566 7420 756e 6368 616e 6765 642e 220a  eft unchanged.".
+00006710: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006720: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006730: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
+00006740: 742e 7265 7475 726e 5f63 6f64 652c 2030  t.return_code, 0
+00006750: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00006760: 706f 7274 2e63 6865 636b 203d 2054 7275  port.check = Tru
+00006770: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00006780: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
+00006790: 6570 6f72 742e 7265 7475 726e 5f63 6f64  eport.return_cod
+000067a0: 652c 2031 290a 2020 2020 2020 2020 2020  e, 1).          
+000067b0: 2020 7265 706f 7274 2e63 6865 636b 203d    report.check =
+000067c0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+000067d0: 2020 2072 6570 6f72 742e 6661 696c 6564     report.failed
+000067e0: 2850 6174 6828 2265 3122 292c 2022 626f  (Path("e1"), "bo
+000067f0: 6f6d 2229 0a20 2020 2020 2020 2020 2020  om").           
+00006800: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00006810: 6c28 6c65 6e28 6f75 745f 6c69 6e65 7329  l(len(out_lines)
+00006820: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+00006830: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00006840: 6c28 6c65 6e28 6572 725f 6c69 6e65 7329  l(len(err_lines)
+00006850: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
+00006860: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00006870: 6c28 6572 725f 6c69 6e65 735b 2d31 5d2c  l(err_lines[-1],
+00006880: 2022 6572 726f 723a 2063 616e 6e6f 7420   "error: cannot 
+00006890: 666f 726d 6174 2065 313a 2062 6f6f 6d22  format e1: boom"
+000068a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000068b0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 756e 7374 796c 6528 7374 7228 7265 706f  unstyle(str(repo
+000068e0: 7274 2929 2c0a 2020 2020 2020 2020 2020  rt)),.          
+000068f0: 2020 2020 2020 2231 2066 696c 6520 7265        "1 file re
+00006900: 666f 726d 6174 7465 642c 2032 2066 696c  formatted, 2 fil
+00006910: 6573 206c 6566 7420 756e 6368 616e 6765  es left unchange
+00006920: 642c 2031 2066 696c 6520 6661 696c 6564  d, 1 file failed
+00006930: 2074 6f22 0a20 2020 2020 2020 2020 2020   to".           
+00006940: 2020 2020 2022 2072 6566 6f72 6d61 742e       " reformat.
+00006950: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00006960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006970: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00006980: 706f 7274 2e72 6574 7572 6e5f 636f 6465  port.return_code
+00006990: 2c20 3132 3329 0a20 2020 2020 2020 2020  , 123).         
+000069a0: 2020 2072 6570 6f72 742e 646f 6e65 2850     report.done(P
+000069b0: 6174 6828 2266 3322 292c 2070 7969 6e6b  ath("f3"), pyink
+000069c0: 2e43 6861 6e67 6564 2e59 4553 290a 2020  .Changed.YES).  
+000069d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000069e0: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+000069f0: 7574 5f6c 696e 6573 292c 2030 290a 2020  ut_lines), 0).  
+00006a00: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006a10: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00006a20: 7272 5f6c 696e 6573 292c 2031 290a 2020  rr_lines), 1).  
+00006a30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006a40: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00006a50: 2020 2020 2020 2020 2020 2020 756e 7374              unst
+00006a60: 796c 6528 7374 7228 7265 706f 7274 2929  yle(str(report))
+00006a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006a80: 2020 2232 2066 696c 6573 2072 6566 6f72    "2 files refor
+00006a90: 6d61 7474 6564 2c20 3220 6669 6c65 7320  matted, 2 files 
+00006aa0: 6c65 6674 2075 6e63 6861 6e67 6564 2c20  left unchanged, 
+00006ab0: 3120 6669 6c65 2066 6169 6c65 6420 746f  1 file failed to
+00006ac0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00006ad0: 2020 2220 7265 666f 726d 6174 2e22 2c0a    " reformat.",.
+00006ae0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006af0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00006b00: 7373 6572 7445 7175 616c 2872 6570 6f72  ssertEqual(repor
+00006b10: 742e 7265 7475 726e 5f63 6f64 652c 2031  t.return_code, 1
+00006b20: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+00006b30: 7265 706f 7274 2e66 6169 6c65 6428 5061  report.failed(Pa
+00006b40: 7468 2822 6532 2229 2c20 2262 6f6f 6d22  th("e2"), "boom"
+00006b50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00006b60: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00006b70: 656e 286f 7574 5f6c 696e 6573 292c 2030  en(out_lines), 0
+00006b80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00006b90: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00006ba0: 656e 2865 7272 5f6c 696e 6573 292c 2032  en(err_lines), 2
+00006bb0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00006bc0: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+00006bd0: 7272 5f6c 696e 6573 5b2d 315d 2c20 2265  rr_lines[-1], "e
+00006be0: 7272 6f72 3a20 6361 6e6e 6f74 2066 6f72  rror: cannot for
+00006bf0: 6d61 7420 6532 3a20 626f 6f6d 2229 0a20  mat e2: boom"). 
+00006c00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006c10: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
+00006c20: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
+00006c30: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
+00006c40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00006c50: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
+00006c60: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
+00006c70: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
+00006c80: 2032 2066 696c 6573 2066 6169 6c65 6420   2 files failed 
+00006c90: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
+00006ca0: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
+00006cb0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00006cc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006cd0: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
+00006ce0: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
+00006cf0: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
+00006d00: 2020 7265 706f 7274 2e70 6174 685f 6967    report.path_ig
+00006d10: 6e6f 7265 6428 5061 7468 2822 7761 7422  nored(Path("wat"
+00006d20: 292c 2022 6e6f 206d 6174 6368 2229 0a20  ), "no match"). 
+00006d30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006d40: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00006d50: 6f75 745f 6c69 6e65 7329 2c20 3029 0a20  out_lines), 0). 
+00006d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006d70: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+00006d80: 6572 725f 6c69 6e65 7329 2c20 3229 0a20  err_lines), 2). 
+00006d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006da0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
+00006db0: 2020 2020 2020 2020 2020 2020 2075 6e73               uns
+00006dc0: 7479 6c65 2873 7472 2872 6570 6f72 7429  tyle(str(report)
+00006dd0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00006de0: 2020 2022 3220 6669 6c65 7320 7265 666f     "2 files refo
+00006df0: 726d 6174 7465 642c 2032 2066 696c 6573  rmatted, 2 files
+00006e00: 206c 6566 7420 756e 6368 616e 6765 642c   left unchanged,
+00006e10: 2032 2066 696c 6573 2066 6169 6c65 6420   2 files failed 
+00006e20: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
+00006e30: 2020 2020 2220 7265 666f 726d 6174 2e22      " reformat."
+00006e40: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00006e50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006e60: 2e61 7373 6572 7445 7175 616c 2872 6570  .assertEqual(rep
+00006e70: 6f72 742e 7265 7475 726e 5f63 6f64 652c  ort.return_code,
+00006e80: 2031 3233 290a 2020 2020 2020 2020 2020   123).          
+00006e90: 2020 7265 706f 7274 2e64 6f6e 6528 5061    report.done(Pa
+00006ea0: 7468 2822 6634 2229 2c20 7079 696e 6b2e  th("f4"), pyink.
+00006eb0: 4368 616e 6765 642e 4e4f 290a 2020 2020  Changed.NO).    
+00006ec0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006ed0: 6572 7445 7175 616c 286c 656e 286f 7574  ertEqual(len(out
+00006ee0: 5f6c 696e 6573 292c 2030 290a 2020 2020  _lines), 0).    
+00006ef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006f00: 6572 7445 7175 616c 286c 656e 2865 7272  ertEqual(len(err
+00006f10: 5f6c 696e 6573 292c 2032 290a 2020 2020  _lines), 2).    
+00006f20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00006f30: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00006f40: 2020 2020 2020 2020 2020 756e 7374 796c            unstyl
+00006f50: 6528 7374 7228 7265 706f 7274 2929 2c0a  e(str(report)),.
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2232 2066 696c 6573 2072 6566 6f72 6d61  "2 files reforma
+00006f80: 7474 6564 2c20 3320 6669 6c65 7320 6c65  tted, 3 files le
+00006f90: 6674 2075 6e63 6861 6e67 6564 2c20 3220  ft unchanged, 2 
+00006fa0: 6669 6c65 7320 6661 696c 6564 2074 6f22  files failed to"
+00006fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006fc0: 2022 2072 6566 6f72 6d61 742e 222c 0a20   " reformat.",. 
+00006fd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006fe0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00006ff0: 7365 7274 4571 7561 6c28 7265 706f 7274  sertEqual(report
+00007000: 2e72 6574 7572 6e5f 636f 6465 2c20 3132  .return_code, 12
+00007010: 3329 0a20 2020 2020 2020 2020 2020 2072  3).            r
+00007020: 6570 6f72 742e 6368 6563 6b20 3d20 5472  eport.check = Tr
+00007030: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+00007040: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007060: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+00007070: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+00007080: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+00007090: 776f 756c 6420 6265 2072 6566 6f72 6d61  would be reforma
+000070a0: 7474 6564 2c20 3320 6669 6c65 7320 776f  tted, 3 files wo
+000070b0: 756c 6420 6265 206c 6566 7420 756e 6368  uld be left unch
+000070c0: 616e 6765 642c 2032 220a 2020 2020 2020  anged, 2".      
+000070d0: 2020 2020 2020 2020 2020 2220 6669 6c65            " file
+000070e0: 7320 776f 756c 6420 6661 696c 2074 6f20  s would fail to 
+000070f0: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+00007100: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00007110: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
+00007120: 636b 203d 2046 616c 7365 0a20 2020 2020  ck = False.     
+00007130: 2020 2020 2020 2072 6570 6f72 742e 6469         report.di
+00007140: 6666 203d 2054 7275 650a 2020 2020 2020  ff = True.      
+00007150: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00007160: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+00007170: 2020 2020 2020 2020 756e 7374 796c 6528          unstyle(
+00007180: 7374 7228 7265 706f 7274 2929 2c0a 2020  str(report)),.  
+00007190: 2020 2020 2020 2020 2020 2020 2020 2232                "2
+000071a0: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
+000071b0: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
+000071c0: 696c 6573 2077 6f75 6c64 2062 6520 6c65  iles would be le
+000071d0: 6674 2075 6e63 6861 6e67 6564 2c20 3222  ft unchanged, 2"
+000071e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000071f0: 2022 2066 696c 6573 2077 6f75 6c64 2066   " files would f
+00007200: 6169 6c20 746f 2072 6566 6f72 6d61 742e  ail to reformat.
+00007210: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00007220: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
+00007230: 6570 6f72 745f 6e6f 726d 616c 2873 656c  eport_normal(sel
+00007240: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00007250: 2020 2020 7265 706f 7274 203d 2070 7969      report = pyi
+00007260: 6e6b 2e52 6570 6f72 7428 290a 2020 2020  nk.Report().    
+00007270: 2020 2020 6f75 745f 6c69 6e65 7320 3d20      out_lines = 
+00007280: 5b5d 0a20 2020 2020 2020 2065 7272 5f6c  [].        err_l
+00007290: 696e 6573 203d 205b 5d0a 0a20 2020 2020  ines = []..     
+000072a0: 2020 2064 6566 206f 7574 286d 7367 3a20     def out(msg: 
+000072b0: 7374 722c 202a 2a6b 7761 7267 733a 2041  str, **kwargs: A
+000072c0: 6e79 2920 2d3e 204e 6f6e 653a 0a20 2020  ny) -> None:.   
+000072d0: 2020 2020 2020 2020 206f 7574 5f6c 696e           out_lin
+000072e0: 6573 2e61 7070 656e 6428 6d73 6729 0a0a  es.append(msg)..
+000072f0: 2020 2020 2020 2020 6465 6620 6572 7228          def err(
+00007300: 6d73 673a 2073 7472 2c20 2a2a 6b77 6172  msg: str, **kwar
+00007310: 6773 3a20 416e 7929 202d 3e20 4e6f 6e65  gs: Any) -> None
+00007320: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
+00007330: 725f 6c69 6e65 732e 6170 7065 6e64 286d  r_lines.append(m
+00007340: 7367 290a 0a20 2020 2020 2020 2077 6974  sg)..        wit
+00007350: 6820 7061 7463 6828 2270 7969 6e6b 2e6f  h patch("pyink.o
+00007360: 7574 7075 742e 5f6f 7574 222c 206f 7574  utput._out", out
+00007370: 292c 2070 6174 6368 2822 7079 696e 6b2e  ), patch("pyink.
+00007380: 6f75 7470 7574 2e5f 6572 7222 2c20 6572  output._err", er
+00007390: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000073a0: 7265 706f 7274 2e64 6f6e 6528 5061 7468  report.done(Path
+000073b0: 2822 6631 2229 2c20 7079 696e 6b2e 4368  ("f1"), pyink.Ch
+000073c0: 616e 6765 642e 4e4f 290a 2020 2020 2020  anged.NO).      
+000073d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000073e0: 7445 7175 616c 286c 656e 286f 7574 5f6c  tEqual(len(out_l
+000073f0: 696e 6573 292c 2030 290a 2020 2020 2020  ines), 0).      
+00007400: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00007410: 7445 7175 616c 286c 656e 2865 7272 5f6c  tEqual(len(err_l
+00007420: 696e 6573 292c 2030 290a 2020 2020 2020  ines), 0).      
+00007430: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00007440: 7445 7175 616c 2875 6e73 7479 6c65 2873  tEqual(unstyle(s
+00007450: 7472 2872 6570 6f72 7429 292c 2022 3120  tr(report)), "1 
+00007460: 6669 6c65 206c 6566 7420 756e 6368 616e  file left unchan
+00007470: 6765 642e 2229 0a20 2020 2020 2020 2020  ged.").         
+00007480: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007490: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
+000074a0: 6e5f 636f 6465 2c20 3029 0a20 2020 2020  n_code, 0).     
+000074b0: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
+000074c0: 6e65 2850 6174 6828 2266 3222 292c 2070  ne(Path("f2"), p
+000074d0: 7969 6e6b 2e43 6861 6e67 6564 2e59 4553  yink.Changed.YES
+000074e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000074f0: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00007500: 656e 286f 7574 5f6c 696e 6573 292c 2031  en(out_lines), 1
+00007510: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00007520: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00007530: 656e 2865 7272 5f6c 696e 6573 292c 2030  en(err_lines), 0
+00007540: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00007550: 6c66 2e61 7373 6572 7445 7175 616c 286f  lf.assertEqual(o
+00007560: 7574 5f6c 696e 6573 5b2d 315d 2c20 2272  ut_lines[-1], "r
+00007570: 6566 6f72 6d61 7474 6564 2066 3222 290a  eformatted f2").
+00007580: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007590: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
+000075a0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000075b0: 7374 796c 6528 7374 7228 7265 706f 7274  style(str(report
+000075c0: 2929 2c20 2231 2066 696c 6520 7265 666f  )), "1 file refo
+000075d0: 726d 6174 7465 642c 2031 2066 696c 6520  rmatted, 1 file 
+000075e0: 6c65 6674 2075 6e63 6861 6e67 6564 2e22  left unchanged."
+000075f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007600: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+00007610: 742e 646f 6e65 2850 6174 6828 2266 3322  t.done(Path("f3"
+00007620: 292c 2070 7969 6e6b 2e43 6861 6e67 6564  ), pyink.Changed
+00007630: 2e43 4143 4845 4429 0a20 2020 2020 2020  .CACHED).       
+00007640: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007650: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
+00007660: 6e65 7329 2c20 3129 0a20 2020 2020 2020  nes), 1).       
+00007670: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007680: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
+00007690: 6e65 7329 2c20 3029 0a20 2020 2020 2020  nes), 0).       
+000076a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000076b0: 4571 7561 6c28 6f75 745f 6c69 6e65 735b  Equal(out_lines[
+000076c0: 2d31 5d2c 2022 7265 666f 726d 6174 7465  -1], "reformatte
+000076d0: 6420 6632 2229 0a20 2020 2020 2020 2020  d f2").         
+000076e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000076f0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+00007700: 2020 2020 2075 6e73 7479 6c65 2873 7472       unstyle(str
+00007710: 2872 6570 6f72 7429 292c 2022 3120 6669  (report)), "1 fi
+00007720: 6c65 2072 6566 6f72 6d61 7474 6564 2c20  le reformatted, 
+00007730: 3220 6669 6c65 7320 6c65 6674 2075 6e63  2 files left unc
+00007740: 6861 6e67 6564 2e22 0a20 2020 2020 2020  hanged.".       
+00007750: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00007760: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007770: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
+00007780: 6e5f 636f 6465 2c20 3029 0a20 2020 2020  n_code, 0).     
+00007790: 2020 2020 2020 2072 6570 6f72 742e 6368         report.ch
+000077a0: 6563 6b20 3d20 5472 7565 0a20 2020 2020  eck = True.     
+000077b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000077c0: 7274 4571 7561 6c28 7265 706f 7274 2e72  rtEqual(report.r
+000077d0: 6574 7572 6e5f 636f 6465 2c20 3129 0a20  eturn_code, 1). 
+000077e0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+000077f0: 742e 6368 6563 6b20 3d20 4661 6c73 650a  t.check = False.
+00007800: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00007810: 7274 2e66 6169 6c65 6428 5061 7468 2822  rt.failed(Path("
+00007820: 6531 2229 2c20 2262 6f6f 6d22 290a 2020  e1"), "boom").  
+00007830: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007840: 7373 6572 7445 7175 616c 286c 656e 286f  ssertEqual(len(o
+00007850: 7574 5f6c 696e 6573 292c 2031 290a 2020  ut_lines), 1).  
+00007860: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00007870: 7373 6572 7445 7175 616c 286c 656e 2865  ssertEqual(len(e
+00007880: 7272 5f6c 696e 6573 292c 2031 290a 2020  rr_lines), 1).  
+00007890: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000078a0: 7373 6572 7445 7175 616c 2865 7272 5f6c  ssertEqual(err_l
+000078b0: 696e 6573 5b2d 315d 2c20 2265 7272 6f72  ines[-1], "error
+000078c0: 3a20 6361 6e6e 6f74 2066 6f72 6d61 7420  : cannot format 
+000078d0: 6531 3a20 626f 6f6d 2229 0a20 2020 2020  e1: boom").     
+000078e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000078f0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00007900: 2020 2020 2020 2020 2075 6e73 7479 6c65           unstyle
+00007910: 2873 7472 2872 6570 6f72 7429 292c 0a20  (str(report)),. 
+00007920: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007930: 3120 6669 6c65 2072 6566 6f72 6d61 7474  1 file reformatt
+00007940: 6564 2c20 3220 6669 6c65 7320 6c65 6674  ed, 2 files left
+00007950: 2075 6e63 6861 6e67 6564 2c20 3120 6669   unchanged, 1 fi
+00007960: 6c65 2066 6169 6c65 6420 746f 220a 2020  le failed to".  
+00007970: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+00007980: 7265 666f 726d 6174 2e22 2c0a 2020 2020  reformat.",.    
+00007990: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000079a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000079b0: 7445 7175 616c 2872 6570 6f72 742e 7265  tEqual(report.re
+000079c0: 7475 726e 5f63 6f64 652c 2031 3233 290a  turn_code, 123).
+000079d0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+000079e0: 7274 2e64 6f6e 6528 5061 7468 2822 6633  rt.done(Path("f3
+000079f0: 2229 2c20 7079 696e 6b2e 4368 616e 6765  "), pyink.Change
+00007a00: 642e 5945 5329 0a20 2020 2020 2020 2020  d.YES).         
+00007a10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007a20: 7561 6c28 6c65 6e28 6f75 745f 6c69 6e65  ual(len(out_line
+00007a30: 7329 2c20 3229 0a20 2020 2020 2020 2020  s), 2).         
+00007a40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007a50: 7561 6c28 6c65 6e28 6572 725f 6c69 6e65  ual(len(err_line
+00007a60: 7329 2c20 3129 0a20 2020 2020 2020 2020  s), 1).         
+00007a70: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007a80: 7561 6c28 6f75 745f 6c69 6e65 735b 2d31  ual(out_lines[-1
+00007a90: 5d2c 2022 7265 666f 726d 6174 7465 6420  ], "reformatted 
+00007aa0: 6633 2229 0a20 2020 2020 2020 2020 2020  f3").           
+00007ab0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00007ac0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00007ad0: 2020 2075 6e73 7479 6c65 2873 7472 2872     unstyle(str(r
+00007ae0: 6570 6f72 7429 292c 0a20 2020 2020 2020  eport)),.       
+00007af0: 2020 2020 2020 2020 2022 3220 6669 6c65           "2 file
+00007b00: 7320 7265 666f 726d 6174 7465 642c 2032  s reformatted, 2
+00007b10: 2066 696c 6573 206c 6566 7420 756e 6368   files left unch
+00007b20: 616e 6765 642c 2031 2066 696c 6520 6661  anged, 1 file fa
+00007b30: 696c 6564 2074 6f22 0a20 2020 2020 2020  iled to".       
+00007b40: 2020 2020 2020 2020 2022 2072 6566 6f72           " refor
+00007b50: 6d61 742e 222c 0a20 2020 2020 2020 2020  mat.",.         
+00007b60: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00007b70: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00007b80: 6c28 7265 706f 7274 2e72 6574 7572 6e5f  l(report.return_
+00007b90: 636f 6465 2c20 3132 3329 0a20 2020 2020  code, 123).     
+00007ba0: 2020 2020 2020 2072 6570 6f72 742e 6661         report.fa
+00007bb0: 696c 6564 2850 6174 6828 2265 3222 292c  iled(Path("e2"),
+00007bc0: 2022 626f 6f6d 2229 0a20 2020 2020 2020   "boom").       
+00007bd0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007be0: 4571 7561 6c28 6c65 6e28 6f75 745f 6c69  Equal(len(out_li
+00007bf0: 6e65 7329 2c20 3229 0a20 2020 2020 2020  nes), 2).       
+00007c00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007c10: 4571 7561 6c28 6c65 6e28 6572 725f 6c69  Equal(len(err_li
+00007c20: 6e65 7329 2c20 3229 0a20 2020 2020 2020  nes), 2).       
+00007c30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007c40: 4571 7561 6c28 6572 725f 6c69 6e65 735b  Equal(err_lines[
+00007c50: 2d31 5d2c 2022 6572 726f 723a 2063 616e  -1], "error: can
+00007c60: 6e6f 7420 666f 726d 6174 2065 323a 2062  not format e2: b
+00007c70: 6f6f 6d22 290a 2020 2020 2020 2020 2020  oom").          
+00007c80: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007c90: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00007ca0: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
+00007cb0: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
+00007cc0: 2020 2020 2020 2020 2020 2232 2066 696c            "2 fil
+00007cd0: 6573 2072 6566 6f72 6d61 7474 6564 2c20  es reformatted, 
+00007ce0: 3220 6669 6c65 7320 6c65 6674 2075 6e63  2 files left unc
+00007cf0: 6861 6e67 6564 2c20 3220 6669 6c65 7320  hanged, 2 files 
+00007d00: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
+00007d10: 2020 2020 2020 2020 2020 2022 2072 6566             " ref
+00007d20: 6f72 6d61 742e 222c 0a20 2020 2020 2020  ormat.",.       
+00007d30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00007d40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007d50: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
+00007d60: 6e5f 636f 6465 2c20 3132 3329 0a20 2020  n_code, 123).   
+00007d70: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
+00007d80: 7061 7468 5f69 676e 6f72 6564 2850 6174  path_ignored(Pat
+00007d90: 6828 2277 6174 2229 2c20 226e 6f20 6d61  h("wat"), "no ma
+00007da0: 7463 6822 290a 2020 2020 2020 2020 2020  tch").          
+00007db0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007dc0: 616c 286c 656e 286f 7574 5f6c 696e 6573  al(len(out_lines
+00007dd0: 292c 2032 290a 2020 2020 2020 2020 2020  ), 2).          
+00007de0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007df0: 616c 286c 656e 2865 7272 5f6c 696e 6573  al(len(err_lines
+00007e00: 292c 2032 290a 2020 2020 2020 2020 2020  ), 2).          
+00007e10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00007e20: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00007e30: 2020 2020 756e 7374 796c 6528 7374 7228      unstyle(str(
+00007e40: 7265 706f 7274 2929 2c0a 2020 2020 2020  report)),.      
+00007e50: 2020 2020 2020 2020 2020 2232 2066 696c            "2 fil
+00007e60: 6573 2072 6566 6f72 6d61 7474 6564 2c20  es reformatted, 
+00007e70: 3220 6669 6c65 7320 6c65 6674 2075 6e63  2 files left unc
+00007e80: 6861 6e67 6564 2c20 3220 6669 6c65 7320  hanged, 2 files 
+00007e90: 6661 696c 6564 2074 6f22 0a20 2020 2020  failed to".     
+00007ea0: 2020 2020 2020 2020 2020 2022 2072 6566             " ref
+00007eb0: 6f72 6d61 742e 222c 0a20 2020 2020 2020  ormat.",.       
+00007ec0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00007ed0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00007ee0: 7561 6c28 7265 706f 7274 2e72 6574 7572  ual(report.retur
+00007ef0: 6e5f 636f 6465 2c20 3132 3329 0a20 2020  n_code, 123).   
+00007f00: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
+00007f10: 646f 6e65 2850 6174 6828 2266 3422 292c  done(Path("f4"),
+00007f20: 2070 7969 6e6b 2e43 6861 6e67 6564 2e4e   pyink.Changed.N
+00007f30: 4f29 0a20 2020 2020 2020 2020 2020 2073  O).            s
+00007f40: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007f50: 6c65 6e28 6f75 745f 6c69 6e65 7329 2c20  len(out_lines), 
+00007f60: 3229 0a20 2020 2020 2020 2020 2020 2073  2).            s
+00007f70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007f80: 6c65 6e28 6572 725f 6c69 6e65 7329 2c20  len(err_lines), 
+00007f90: 3229 0a20 2020 2020 2020 2020 2020 2073  2).            s
+00007fa0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007fc0: 2075 6e73 7479 6c65 2873 7472 2872 6570   unstyle(str(rep
+00007fd0: 6f72 7429 292c 0a20 2020 2020 2020 2020  ort)),.         
+00007fe0: 2020 2020 2020 2022 3220 6669 6c65 7320         "2 files 
+00007ff0: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
+00008000: 696c 6573 206c 6566 7420 756e 6368 616e  iles left unchan
+00008010: 6765 642c 2032 2066 696c 6573 2066 6169  ged, 2 files fai
+00008020: 6c65 6420 746f 220a 2020 2020 2020 2020  led to".        
+00008030: 2020 2020 2020 2020 2220 7265 666f 726d          " reform
+00008040: 6174 2e22 2c0a 2020 2020 2020 2020 2020  at.",.          
+00008050: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00008060: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008070: 2872 6570 6f72 742e 7265 7475 726e 5f63  (report.return_c
+00008080: 6f64 652c 2031 3233 290a 2020 2020 2020  ode, 123).      
+00008090: 2020 2020 2020 7265 706f 7274 2e63 6865        report.che
+000080a0: 636b 203d 2054 7275 650a 2020 2020 2020  ck = True.      
+000080b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000080c0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+000080d0: 2020 2020 2020 2020 756e 7374 796c 6528          unstyle(
+000080e0: 7374 7228 7265 706f 7274 2929 2c0a 2020  str(report)),.  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2232                "2
+00008100: 2066 696c 6573 2077 6f75 6c64 2062 6520   files would be 
+00008110: 7265 666f 726d 6174 7465 642c 2033 2066  reformatted, 3 f
+00008120: 696c 6573 2077 6f75 6c64 2062 6520 6c65  iles would be le
+00008130: 6674 2075 6e63 6861 6e67 6564 2c20 3222  ft unchanged, 2"
+00008140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008150: 2022 2066 696c 6573 2077 6f75 6c64 2066   " files would f
+00008160: 6169 6c20 746f 2072 6566 6f72 6d61 742e  ail to reformat.
+00008170: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00008180: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00008190: 6f72 742e 6368 6563 6b20 3d20 4661 6c73  ort.check = Fals
+000081a0: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+000081b0: 706f 7274 2e64 6966 6620 3d20 5472 7565  port.diff = True
+000081c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000081d0: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000081f0: 6e73 7479 6c65 2873 7472 2872 6570 6f72  nstyle(str(repor
+00008200: 7429 292c 0a20 2020 2020 2020 2020 2020  t)),.           
+00008210: 2020 2020 2022 3220 6669 6c65 7320 776f       "2 files wo
+00008220: 756c 6420 6265 2072 6566 6f72 6d61 7474  uld be reformatt
+00008230: 6564 2c20 3320 6669 6c65 7320 776f 756c  ed, 3 files woul
+00008240: 6420 6265 206c 6566 7420 756e 6368 616e  d be left unchan
+00008250: 6765 642c 2032 220a 2020 2020 2020 2020  ged, 2".        
+00008260: 2020 2020 2020 2020 2220 6669 6c65 7320          " files 
+00008270: 776f 756c 6420 6661 696c 2074 6f20 7265  would fail to re
+00008280: 666f 726d 6174 2e22 2c0a 2020 2020 2020  format.",.      
+00008290: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+000082a0: 2074 6573 745f 6c69 6232 746f 335f 7061   test_lib2to3_pa
+000082b0: 7273 6528 7365 6c66 2920 2d3e 204e 6f6e  rse(self) -> Non
+000082c0: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
+000082d0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+000082e0: 7328 7079 696e 6b2e 496e 7661 6c69 6449  s(pyink.InvalidI
+000082f0: 6e70 7574 293a 0a20 2020 2020 2020 2020  nput):.         
+00008300: 2020 2070 7969 6e6b 2e6c 6962 3274 6f33     pyink.lib2to3
+00008310: 5f70 6172 7365 2822 696e 7661 6c69 6420  _parse("invalid 
+00008320: 7379 6e74 6178 2229 0a0a 2020 2020 2020  syntax")..      
+00008330: 2020 7374 7261 6464 6c69 6e67 203d 2022    straddling = "
+00008340: 7820 2b20 7922 0a20 2020 2020 2020 2070  x + y".        p
+00008350: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
+00008360: 7365 2873 7472 6164 646c 696e 6729 0a20  se(straddling). 
+00008370: 2020 2020 2020 2070 7969 6e6b 2e6c 6962         pyink.lib
+00008380: 3274 6f33 5f70 6172 7365 2873 7472 6164  2to3_parse(strad
+00008390: 646c 696e 672c 207b 5461 7267 6574 5665  dling, {TargetVe
+000083a0: 7273 696f 6e2e 5059 3336 7d29 0a0a 2020  rsion.PY36})..  
+000083b0: 2020 2020 2020 7079 325f 6f6e 6c79 203d        py2_only =
+000083c0: 2022 7072 696e 7420 7822 0a20 2020 2020   "print x".     
+000083d0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+000083e0: 6572 7452 6169 7365 7328 7079 696e 6b2e  ertRaises(pyink.
+000083f0: 496e 7661 6c69 6449 6e70 7574 293a 0a20  InvalidInput):. 
+00008400: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
+00008410: 2e6c 6962 3274 6f33 5f70 6172 7365 2870  .lib2to3_parse(p
+00008420: 7932 5f6f 6e6c 792c 207b 5461 7267 6574  y2_only, {Target
+00008430: 5665 7273 696f 6e2e 5059 3336 7d29 0a0a  Version.PY36})..
+00008440: 2020 2020 2020 2020 7079 335f 6f6e 6c79          py3_only
+00008450: 203d 2022 6578 6563 2878 2c20 656e 643d   = "exec(x, end=
+00008460: 7929 220a 2020 2020 2020 2020 7079 696e  y)".        pyin
+00008470: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
+00008480: 7079 335f 6f6e 6c79 290a 2020 2020 2020  py3_only).      
+00008490: 2020 7079 696e 6b2e 6c69 6232 746f 335f    pyink.lib2to3_
+000084a0: 7061 7273 6528 7079 335f 6f6e 6c79 2c20  parse(py3_only, 
+000084b0: 7b54 6172 6765 7456 6572 7369 6f6e 2e50  {TargetVersion.P
+000084c0: 5933 367d 290a 0a20 2020 2064 6566 2074  Y36})..    def t
+000084d0: 6573 745f 6765 745f 6665 6174 7572 6573  est_get_features
+000084e0: 5f75 7365 645f 6465 636f 7261 746f 7228  _used_decorator(
+000084f0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00008500: 2020 2020 2020 2023 2054 6573 7420 7468         # Test th
+00008510: 6520 6665 6174 7572 6520 6465 7465 6374  e feature detect
+00008520: 696f 6e20 6f66 206e 6577 2064 6563 6f72  ion of new decor
+00008530: 6174 6f72 2073 796e 7461 780a 2020 2020  ator syntax.    
+00008540: 2020 2020 2320 7369 6e63 6520 7468 6973      # since this
+00008550: 206d 616b 6573 2073 6f6d 6520 7465 7374   makes some test
+00008560: 2063 6173 6573 206f 6620 7465 7374 5f67   cases of test_g
+00008570: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00008580: 2829 0a20 2020 2020 2020 2023 2066 6169  ().        # fai
+00008590: 6c73 2069 6620 6974 2066 6169 6c73 2c20  ls if it fails, 
+000085a0: 7468 6973 2069 7320 7465 7374 6564 2066  this is tested f
+000085b0: 6972 7374 2073 6f20 7468 6174 2061 2075  irst so that a u
+000085c0: 7365 6675 6c20 6361 7365 0a20 2020 2020  seful case.     
+000085d0: 2020 2023 2069 7320 6964 656e 7469 6669     # is identifi
+000085e0: 6564 0a20 2020 2020 2020 2073 696d 706c  ed.        simpl
+000085f0: 6573 2c20 7265 6c61 7865 6420 3d20 7265  es, relaxed = re
+00008600: 6164 5f64 6174 6128 226d 6973 6365 6c6c  ad_data("miscell
+00008610: 616e 656f 7573 222c 2022 6465 636f 7261  aneous", "decora
+00008620: 746f 7273 2229 0a20 2020 2020 2020 2023  tors").        #
+00008630: 2073 6b69 7020 6578 706c 616e 6174 696f   skip explanatio
+00008640: 6e20 636f 6d6d 656e 7473 2061 7420 7468  n comments at th
+00008650: 6520 746f 7020 6f66 2074 6865 2066 696c  e top of the fil
+00008660: 650a 2020 2020 2020 2020 666f 7220 7369  e.        for si
+00008670: 6d70 6c65 5f74 6573 7420 696e 2073 696d  mple_test in sim
+00008680: 706c 6573 2e73 706c 6974 2822 2323 2229  ples.split("##")
+00008690: 5b31 3a5d 3a0a 2020 2020 2020 2020 2020  [1:]:.          
+000086a0: 2020 6e6f 6465 203d 2070 7969 6e6b 2e6c    node = pyink.l
+000086b0: 6962 3274 6f33 5f70 6172 7365 2873 696d  ib2to3_parse(sim
+000086c0: 706c 655f 7465 7374 290a 2020 2020 2020  ple_test).      
+000086d0: 2020 2020 2020 6465 636f 7261 746f 7220        decorator 
+000086e0: 3d20 7374 7228 6e6f 6465 2e63 6869 6c64  = str(node.child
+000086f0: 7265 6e5b 305d 2e63 6869 6c64 7265 6e5b  ren[0].children[
+00008700: 305d 292e 7374 7269 7028 290a 2020 2020  0]).strip().    
+00008710: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008720: 6572 744e 6f74 496e 280a 2020 2020 2020  ertNotIn(.      
+00008730: 2020 2020 2020 2020 2020 4665 6174 7572            Featur
+00008740: 652e 5245 4c41 5845 445f 4445 434f 5241  e.RELAXED_DECORA
+00008750: 544f 5253 2c0a 2020 2020 2020 2020 2020  TORS,.          
+00008760: 2020 2020 2020 7079 696e 6b2e 6765 745f        pyink.get_
+00008770: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+00008780: 6465 292c 0a20 2020 2020 2020 2020 2020  de),.           
+00008790: 2020 2020 206d 7367 3d28 0a20 2020 2020       msg=(.     
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000087b0: 2264 6563 6f72 6174 6f72 2027 7b64 6563  "decorator '{dec
+000087c0: 6f72 6174 6f72 7d27 2066 6f6c 6c6f 7773  orator}' follows
+000087d0: 2070 7974 686f 6e3c 3d33 2e38 2073 796e   python<=3.8 syn
+000087e0: 7461 7822 0a20 2020 2020 2020 2020 2020  tax".           
+000087f0: 2020 2020 2020 2020 2022 6275 7420 6973           "but is
+00008800: 2064 6574 6563 7465 6420 6173 2033 2e39   detected as 3.9
+00008810: 2b22 0a20 2020 2020 2020 2020 2020 2020  +".             
+00008820: 2020 2020 2020 2023 2066 2254 6865 2066         # f"The f
+00008830: 756c 6c20 6e6f 6465 2069 735c 6e7b 6e6f  ull node is\n{no
+00008840: 6465 2172 7d22 0a20 2020 2020 2020 2020  de!r}".         
+00008850: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00008860: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008870: 2320 736b 6970 2074 6865 2027 2320 6f75  # skip the '# ou
+00008880: 7470 7574 2720 636f 6d6d 656e 7420 6174  tput' comment at
+00008890: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
+000088a0: 6f75 7470 7574 2070 6172 740a 2020 2020  output part.    
+000088b0: 2020 2020 666f 7220 7265 6c61 7865 645f      for relaxed_
+000088c0: 7465 7374 2069 6e20 7265 6c61 7865 642e  test in relaxed.
+000088d0: 7370 6c69 7428 2223 2322 295b 313a 5d3a  split("##")[1:]:
+000088e0: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
+000088f0: 6520 3d20 7079 696e 6b2e 6c69 6232 746f  e = pyink.lib2to
+00008900: 335f 7061 7273 6528 7265 6c61 7865 645f  3_parse(relaxed_
+00008910: 7465 7374 290a 2020 2020 2020 2020 2020  test).          
+00008920: 2020 6465 636f 7261 746f 7220 3d20 7374    decorator = st
+00008930: 7228 6e6f 6465 2e63 6869 6c64 7265 6e5b  r(node.children[
+00008940: 305d 2e63 6869 6c64 7265 6e5b 305d 292e  0].children[0]).
+00008950: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
+00008960: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+00008970: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00008980: 2020 2046 6561 7475 7265 2e52 454c 4158     Feature.RELAX
+00008990: 4544 5f44 4543 4f52 4154 4f52 532c 0a20  ED_DECORATORS,. 
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000089b0: 7969 6e6b 2e67 6574 5f66 6561 7475 7265  yink.get_feature
+000089c0: 735f 7573 6564 286e 6f64 6529 2c0a 2020  s_used(node),.  
+000089d0: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+000089e0: 673d 280a 2020 2020 2020 2020 2020 2020  g=(.            
+000089f0: 2020 2020 2020 2020 6622 6465 636f 7261          f"decora
+00008a00: 746f 7220 277b 6465 636f 7261 746f 727d  tor '{decorator}
+00008a10: 2720 7573 6573 2070 7974 686f 6e33 2e39  ' uses python3.9
+00008a20: 2b20 7379 6e74 6178 220a 2020 2020 2020  + syntax".      
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00008a40: 7574 2069 7320 6465 7465 6374 6564 2061  ut is detected a
+00008a50: 7320 7079 7468 6f6e 3c3d 332e 3822 0a20  s python<=3.8". 
+00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a70: 2020 2023 2066 2254 6865 2066 756c 6c20     # f"The full 
+00008a80: 6e6f 6465 2069 735c 6e7b 6e6f 6465 2172  node is\n{node!r
+00008a90: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00008aa0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00008ab0: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+00008ac0: 745f 6765 745f 6665 6174 7572 6573 5f75  t_get_features_u
+00008ad0: 7365 6428 7365 6c66 2920 2d3e 204e 6f6e  sed(self) -> Non
+00008ae0: 653a 0a20 2020 2020 2020 206e 6f64 6520  e:.        node 
+00008af0: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
+00008b00: 7061 7273 6528 2264 6566 2066 282a 2c20  parse("def f(*, 
+00008b10: 6172 6729 3a20 2e2e 2e5c 6e22 290a 2020  arg): ...\n").  
+00008b20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008b30: 7445 7175 616c 2870 7969 6e6b 2e67 6574  tEqual(pyink.get
+00008b40: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
+00008b50: 6f64 6529 2c20 7365 7428 2929 0a20 2020  ode), set()).   
+00008b60: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
+00008b70: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
+00008b80: 2264 6566 2066 282a 2c20 6172 672c 293a  "def f(*, arg,):
+00008b90: 202e 2e2e 5c6e 2229 0a20 2020 2020 2020   ...\n").       
+00008ba0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00008bb0: 6c28 7079 696e 6b2e 6765 745f 6665 6174  l(pyink.get_feat
+00008bc0: 7572 6573 5f75 7365 6428 6e6f 6465 292c  ures_used(node),
+00008bd0: 207b 4665 6174 7572 652e 5452 4149 4c49   {Feature.TRAILI
+00008be0: 4e47 5f43 4f4d 4d41 5f49 4e5f 4445 467d  NG_COMMA_IN_DEF}
+00008bf0: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
+00008c00: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
+00008c10: 6172 7365 2822 6628 2a61 7267 2c29 5c6e  arse("f(*arg,)\n
+00008c20: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00008c30: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
+00008c40: 2020 2020 2020 2020 2070 7969 6e6b 2e67           pyink.g
+00008c50: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00008c60: 286e 6f64 6529 2c20 7b46 6561 7475 7265  (node), {Feature
+00008c70: 2e54 5241 494c 494e 475f 434f 4d4d 415f  .TRAILING_COMMA_
+00008c80: 494e 5f43 414c 4c7d 0a20 2020 2020 2020  IN_CALL}.       
+00008c90: 2029 0a20 2020 2020 2020 206e 6f64 6520   ).        node 
+00008ca0: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
+00008cb0: 7061 7273 6528 2264 6566 2066 282a 2c20  parse("def f(*, 
+00008cc0: 6172 6729 3a20 6627 7374 7269 6e67 275c  arg): f'string'\
+00008cd0: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
+00008ce0: 2e61 7373 6572 7445 7175 616c 2870 7969  .assertEqual(pyi
+00008cf0: 6e6b 2e67 6574 5f66 6561 7475 7265 735f  nk.get_features_
+00008d00: 7573 6564 286e 6f64 6529 2c20 7b46 6561  used(node), {Fea
+00008d10: 7475 7265 2e46 5f53 5452 494e 4753 7d29  ture.F_STRINGS})
+00008d20: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+00008d30: 7079 696e 6b2e 6c69 6232 746f 335f 7061  pyink.lib2to3_pa
+00008d40: 7273 6528 2231 3233 5f34 3536 5c6e 2229  rse("123_456\n")
+00008d50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00008d60: 7365 7274 4571 7561 6c28 7079 696e 6b2e  sertEqual(pyink.
+00008d70: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+00008d80: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
+00008d90: 652e 4e55 4d45 5249 435f 554e 4445 5253  e.NUMERIC_UNDERS
+00008da0: 434f 5245 537d 290a 2020 2020 2020 2020  CORES}).        
+00008db0: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
+00008dc0: 3274 6f33 5f70 6172 7365 2822 3132 3334  2to3_parse("1234
+00008dd0: 3536 5c6e 2229 0a20 2020 2020 2020 2073  56\n").        s
+00008de0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00008df0: 7079 696e 6b2e 6765 745f 6665 6174 7572  pyink.get_featur
+00008e00: 6573 5f75 7365 6428 6e6f 6465 292c 2073  es_used(node), s
+00008e10: 6574 2829 290a 2020 2020 2020 2020 736f  et()).        so
+00008e20: 7572 6365 2c20 6578 7065 6374 6564 203d  urce, expected =
+00008e30: 2072 6561 645f 6461 7461 2822 7369 6d70   read_data("simp
+00008e40: 6c65 5f63 6173 6573 222c 2022 6675 6e63  le_cases", "func
+00008e50: 7469 6f6e 2229 0a20 2020 2020 2020 206e  tion").        n
+00008e60: 6f64 6520 3d20 7079 696e 6b2e 6c69 6232  ode = pyink.lib2
+00008e70: 746f 335f 7061 7273 6528 736f 7572 6365  to3_parse(source
+00008e80: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+00008e90: 6564 5f66 6561 7475 7265 7320 3d20 7b0a  ed_features = {.
+00008ea0: 2020 2020 2020 2020 2020 2020 4665 6174              Feat
+00008eb0: 7572 652e 5452 4149 4c49 4e47 5f43 4f4d  ure.TRAILING_COM
+00008ec0: 4d41 5f49 4e5f 4341 4c4c 2c0a 2020 2020  MA_IN_CALL,.    
+00008ed0: 2020 2020 2020 2020 4665 6174 7572 652e          Feature.
+00008ee0: 5452 4149 4c49 4e47 5f43 4f4d 4d41 5f49  TRAILING_COMMA_I
+00008ef0: 4e5f 4445 462c 0a20 2020 2020 2020 2020  N_DEF,.         
+00008f00: 2020 2046 6561 7475 7265 2e46 5f53 5452     Feature.F_STR
+00008f10: 494e 4753 2c0a 2020 2020 2020 2020 7d0a  INGS,.        }.
+00008f20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008f30: 6572 7445 7175 616c 2870 7969 6e6b 2e67  ertEqual(pyink.g
+00008f40: 6574 5f66 6561 7475 7265 735f 7573 6564  et_features_used
+00008f50: 286e 6f64 6529 2c20 6578 7065 6374 6564  (node), expected
+00008f60: 5f66 6561 7475 7265 7329 0a20 2020 2020  _features).     
+00008f70: 2020 206e 6f64 6520 3d20 7079 696e 6b2e     node = pyink.
+00008f80: 6c69 6232 746f 335f 7061 7273 6528 6578  lib2to3_parse(ex
+00008f90: 7065 6374 6564 290a 2020 2020 2020 2020  pected).        
+00008fa0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008fb0: 2870 7969 6e6b 2e67 6574 5f66 6561 7475  (pyink.get_featu
+00008fc0: 7265 735f 7573 6564 286e 6f64 6529 2c20  res_used(node), 
+00008fd0: 6578 7065 6374 6564 5f66 6561 7475 7265  expected_feature
+00008fe0: 7329 0a20 2020 2020 2020 2073 6f75 7263  s).        sourc
+00008ff0: 652c 2065 7870 6563 7465 6420 3d20 7265  e, expected = re
+00009000: 6164 5f64 6174 6128 2273 696d 706c 655f  ad_data("simple_
+00009010: 6361 7365 7322 2c20 2265 7870 7265 7373  cases", "express
+00009020: 696f 6e22 290a 2020 2020 2020 2020 6e6f  ion").        no
+00009030: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
+00009040: 6f33 5f70 6172 7365 2873 6f75 7263 6529  o3_parse(source)
+00009050: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009060: 7365 7274 4571 7561 6c28 7079 696e 6b2e  sertEqual(pyink.
+00009070: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+00009080: 6428 6e6f 6465 292c 2073 6574 2829 290a  d(node), set()).
+00009090: 2020 2020 2020 2020 6e6f 6465 203d 2070          node = p
+000090a0: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
+000090b0: 7365 2865 7870 6563 7465 6429 0a20 2020  se(expected).   
+000090c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000090d0: 4571 7561 6c28 7079 696e 6b2e 6765 745f  Equal(pyink.get_
+000090e0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+000090f0: 6465 292c 2073 6574 2829 290a 2020 2020  de), set()).    
+00009100: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
+00009110: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
+00009120: 6c61 6d62 6461 2061 2c20 2f2c 2062 3a20  lambda a, /, b: 
+00009130: 2e2e 2e22 290a 2020 2020 2020 2020 7365  ...").        se
+00009140: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
+00009150: 7969 6e6b 2e67 6574 5f66 6561 7475 7265  yink.get_feature
+00009160: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
+00009170: 6561 7475 7265 2e50 4f53 5f4f 4e4c 595f  eature.POS_ONLY_
+00009180: 4152 4755 4d45 4e54 537d 290a 2020 2020  ARGUMENTS}).    
+00009190: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
+000091a0: 2e6c 6962 3274 6f33 5f70 6172 7365 2822  .lib2to3_parse("
+000091b0: 6465 6620 666e 2861 2c20 2f2c 2062 293a  def fn(a, /, b):
+000091c0: 202e 2e2e 2229 0a20 2020 2020 2020 2073   ...").        s
+000091d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000091e0: 7079 696e 6b2e 6765 745f 6665 6174 7572  pyink.get_featur
+000091f0: 6573 5f75 7365 6428 6e6f 6465 292c 207b  es_used(node), {
+00009200: 4665 6174 7572 652e 504f 535f 4f4e 4c59  Feature.POS_ONLY
+00009210: 5f41 5247 554d 454e 5453 7d29 0a20 2020  _ARGUMENTS}).   
+00009220: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
+00009230: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
+00009240: 2264 6566 2066 6e28 293a 2079 6965 6c64  "def fn(): yield
+00009250: 2061 2c20 6222 290a 2020 2020 2020 2020   a, b").        
+00009260: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00009270: 2870 7969 6e6b 2e67 6574 5f66 6561 7475  (pyink.get_featu
+00009280: 7265 735f 7573 6564 286e 6f64 6529 2c20  res_used(node), 
+00009290: 7365 7428 2929 0a20 2020 2020 2020 206e  set()).        n
+000092a0: 6f64 6520 3d20 7079 696e 6b2e 6c69 6232  ode = pyink.lib2
+000092b0: 746f 335f 7061 7273 6528 2264 6566 2066  to3_parse("def f
+000092c0: 6e28 293a 2072 6574 7572 6e20 612c 2062  n(): return a, b
+000092d0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000092e0: 6173 7365 7274 4571 7561 6c28 7079 696e  assertEqual(pyin
+000092f0: 6b2e 6765 745f 6665 6174 7572 6573 5f75  k.get_features_u
+00009300: 7365 6428 6e6f 6465 292c 2073 6574 2829  sed(node), set()
+00009310: 290a 2020 2020 2020 2020 6e6f 6465 203d  ).        node =
+00009320: 2070 7969 6e6b 2e6c 6962 3274 6f33 5f70   pyink.lib2to3_p
+00009330: 6172 7365 2822 6465 6620 666e 2829 3a20  arse("def fn(): 
+00009340: 7969 656c 6420 2a62 2c20 6322 290a 2020  yield *b, c").  
+00009350: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009360: 7445 7175 616c 2870 7969 6e6b 2e67 6574  tEqual(pyink.get
+00009370: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
+00009380: 6f64 6529 2c20 7b46 6561 7475 7265 2e55  ode), {Feature.U
+00009390: 4e50 4143 4b49 4e47 5f4f 4e5f 464c 4f57  NPACKING_ON_FLOW
+000093a0: 7d29 0a20 2020 2020 2020 206e 6f64 6520  }).        node 
+000093b0: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
+000093c0: 7061 7273 6528 2264 6566 2066 6e28 293a  parse("def fn():
+000093d0: 2072 6574 7572 6e20 612c 202a 622c 2063   return a, *b, c
+000093e0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000093f0: 6173 7365 7274 4571 7561 6c28 7079 696e  assertEqual(pyin
+00009400: 6b2e 6765 745f 6665 6174 7572 6573 5f75  k.get_features_u
+00009410: 7365 6428 6e6f 6465 292c 207b 4665 6174  sed(node), {Feat
+00009420: 7572 652e 554e 5041 434b 494e 475f 4f4e  ure.UNPACKING_ON
+00009430: 5f46 4c4f 577d 290a 2020 2020 2020 2020  _FLOW}).        
+00009440: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
+00009450: 3274 6f33 5f70 6172 7365 2822 7820 3d20  2to3_parse("x = 
+00009460: 612c 202a 622c 2063 2229 0a20 2020 2020  a, *b, c").     
+00009470: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00009480: 7561 6c28 7079 696e 6b2e 6765 745f 6665  ual(pyink.get_fe
+00009490: 6174 7572 6573 5f75 7365 6428 6e6f 6465  atures_used(node
+000094a0: 292c 2073 6574 2829 290a 2020 2020 2020  ), set()).      
+000094b0: 2020 6e6f 6465 203d 2070 7969 6e6b 2e6c    node = pyink.l
+000094c0: 6962 3274 6f33 5f70 6172 7365 2822 783a  ib2to3_parse("x:
+000094d0: 2041 6e79 203d 2072 6567 756c 6172 2229   Any = regular")
+000094e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000094f0: 7365 7274 4571 7561 6c28 7079 696e 6b2e  sertEqual(pyink.
+00009500: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+00009510: 6428 6e6f 6465 292c 2073 6574 2829 290a  d(node), set()).
+00009520: 2020 2020 2020 2020 6e6f 6465 203d 2070          node = p
+00009530: 7969 6e6b 2e6c 6962 3274 6f33 5f70 6172  yink.lib2to3_par
+00009540: 7365 2822 783a 2041 6e79 203d 2028 7265  se("x: Any = (re
+00009550: 6775 6c61 722c 2072 6567 756c 6172 2922  gular, regular)"
+00009560: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00009570: 7373 6572 7445 7175 616c 2870 7969 6e6b  ssertEqual(pyink
+00009580: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
+00009590: 6564 286e 6f64 6529 2c20 7365 7428 2929  ed(node), set())
+000095a0: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+000095b0: 7079 696e 6b2e 6c69 6232 746f 335f 7061  pyink.lib2to3_pa
+000095c0: 7273 6528 2278 3a20 416e 7920 3d20 436f  rse("x: Any = Co
+000095d0: 6d70 6c65 7828 5479 7065 2831 2929 5b73  mplex(Type(1))[s
+000095e0: 6f6d 6574 6869 6e67 5d22 290a 2020 2020  omething]").    
+000095f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00009600: 7175 616c 2870 7969 6e6b 2e67 6574 5f66  qual(pyink.get_f
+00009610: 6561 7475 7265 735f 7573 6564 286e 6f64  eatures_used(nod
+00009620: 6529 2c20 7365 7428 2929 0a20 2020 2020  e), set()).     
+00009630: 2020 206e 6f64 6520 3d20 7079 696e 6b2e     node = pyink.
+00009640: 6c69 6232 746f 335f 7061 7273 6528 2278  lib2to3_parse("x
+00009650: 3a20 5475 706c 655b 696e 742c 202e 2e2e  : Tuple[int, ...
+00009660: 5d20 3d20 612c 2062 2c20 6322 290a 2020  ] = a, b, c").  
+00009670: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009680: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+00009690: 2020 2020 7079 696e 6b2e 6765 745f 6665      pyink.get_fe
+000096a0: 6174 7572 6573 5f75 7365 6428 6e6f 6465  atures_used(node
+000096b0: 292c 207b 4665 6174 7572 652e 414e 4e5f  ), {Feature.ANN_
+000096c0: 4153 5349 474e 5f45 5854 454e 4445 445f  ASSIGN_EXTENDED_
+000096d0: 5248 537d 0a20 2020 2020 2020 2029 0a20  RHS}.        ). 
+000096e0: 2020 2020 2020 206e 6f64 6520 3d20 7079         node = py
+000096f0: 696e 6b2e 6c69 6232 746f 335f 7061 7273  ink.lib2to3_pars
+00009700: 6528 2274 7279 3a20 7061 7373 5c6e 6578  e("try: pass\nex
+00009710: 6365 7074 2053 6f6d 6574 6869 6e67 3a20  cept Something: 
+00009720: 7061 7373 2229 0a20 2020 2020 2020 2073  pass").        s
+00009730: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00009740: 7079 696e 6b2e 6765 745f 6665 6174 7572  pyink.get_featur
+00009750: 6573 5f75 7365 6428 6e6f 6465 292c 2073  es_used(node), s
+00009760: 6574 2829 290a 2020 2020 2020 2020 6e6f  et()).        no
+00009770: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
+00009780: 6f33 5f70 6172 7365 2822 7472 793a 2070  o3_parse("try: p
+00009790: 6173 735c 6e65 7863 6570 7420 282a 536f  ass\nexcept (*So
+000097a0: 6d65 7468 696e 672c 293a 2070 6173 7322  mething,): pass"
+000097b0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000097c0: 7373 6572 7445 7175 616c 2870 7969 6e6b  ssertEqual(pyink
+000097d0: 2e67 6574 5f66 6561 7475 7265 735f 7573  .get_features_us
+000097e0: 6564 286e 6f64 6529 2c20 7365 7428 2929  ed(node), set())
+000097f0: 0a20 2020 2020 2020 206e 6f64 6520 3d20  .        node = 
+00009800: 7079 696e 6b2e 6c69 6232 746f 335f 7061  pyink.lib2to3_pa
+00009810: 7273 6528 2274 7279 3a20 7061 7373 5c6e  rse("try: pass\n
+00009820: 6578 6365 7074 202a 4772 6f75 703a 2070  except *Group: p
+00009830: 6173 7322 290a 2020 2020 2020 2020 7365  ass").        se
+00009840: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
+00009850: 7969 6e6b 2e67 6574 5f66 6561 7475 7265  yink.get_feature
+00009860: 735f 7573 6564 286e 6f64 6529 2c20 7b46  s_used(node), {F
+00009870: 6561 7475 7265 2e45 5843 4550 545f 5354  eature.EXCEPT_ST
+00009880: 4152 7d29 0a20 2020 2020 2020 206e 6f64  AR}).        nod
+00009890: 6520 3d20 7079 696e 6b2e 6c69 6232 746f  e = pyink.lib2to
+000098a0: 335f 7061 7273 6528 2261 5b2a 625d 2229  3_parse("a[*b]")
+000098b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000098c0: 7365 7274 4571 7561 6c28 7079 696e 6b2e  sertEqual(pyink.
+000098d0: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+000098e0: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
+000098f0: 652e 5641 5249 4144 4943 5f47 454e 4552  e.VARIADIC_GENER
+00009900: 4943 537d 290a 2020 2020 2020 2020 6e6f  ICS}).        no
+00009910: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
+00009920: 6f33 5f70 6172 7365 2822 615b 782c 202a  o3_parse("a[x, *
+00009930: 7928 292c 207a 5d20 3d20 7422 290a 2020  y(), z] = t").  
+00009940: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009950: 7445 7175 616c 2870 7969 6e6b 2e67 6574  tEqual(pyink.get
+00009960: 5f66 6561 7475 7265 735f 7573 6564 286e  _features_used(n
+00009970: 6f64 6529 2c20 7b46 6561 7475 7265 2e56  ode), {Feature.V
+00009980: 4152 4941 4449 435f 4745 4e45 5249 4353  ARIADIC_GENERICS
+00009990: 7d29 0a20 2020 2020 2020 206e 6f64 6520  }).        node 
+000099a0: 3d20 7079 696e 6b2e 6c69 6232 746f 335f  = pyink.lib2to3_
+000099b0: 7061 7273 6528 2264 6566 2066 6e28 2a61  parse("def fn(*a
+000099c0: 7267 733a 202a 5429 3a20 7061 7373 2229  rgs: *T): pass")
+000099d0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000099e0: 7365 7274 4571 7561 6c28 7079 696e 6b2e  sertEqual(pyink.
+000099f0: 6765 745f 6665 6174 7572 6573 5f75 7365  get_features_use
+00009a00: 6428 6e6f 6465 292c 207b 4665 6174 7572  d(node), {Featur
+00009a10: 652e 5641 5249 4144 4943 5f47 454e 4552  e.VARIADIC_GENER
+00009a20: 4943 537d 290a 0a20 2020 2064 6566 2074  ICS})..    def t
+00009a30: 6573 745f 6765 745f 6665 6174 7572 6573  est_get_features
+00009a40: 5f75 7365 645f 666f 725f 6675 7475 7265  _used_for_future
+00009a50: 5f66 6c61 6773 2873 656c 6629 202d 3e20  _flags(self) -> 
+00009a60: 4e6f 6e65 3a0a 2020 2020 2020 2020 666f  None:.        fo
+00009a70: 7220 7372 632c 2066 6561 7475 7265 7320  r src, features 
+00009a80: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
+00009a90: 2028 2266 726f 6d20 5f5f 6675 7475 7265   ("from __future
+00009aa0: 5f5f 2069 6d70 6f72 7420 616e 6e6f 7461  __ import annota
+00009ab0: 7469 6f6e 7322 2c20 7b46 6561 7475 7265  tions", {Feature
+00009ac0: 2e46 5554 5552 455f 414e 4e4f 5441 5449  .FUTURE_ANNOTATI
+00009ad0: 4f4e 537d 292c 0a20 2020 2020 2020 2020  ONS}),.         
+00009ae0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00009af0: 2020 2020 2022 6672 6f6d 205f 5f66 7574       "from __fut
+00009b00: 7572 655f 5f20 696d 706f 7274 2028 6f74  ure__ import (ot
+00009b10: 6865 722c 2061 6e6e 6f74 6174 696f 6e73  her, annotations
+00009b20: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+00009b30: 2020 2020 7b46 6561 7475 7265 2e46 5554      {Feature.FUT
+00009b40: 5552 455f 414e 4e4f 5441 5449 4f4e 537d  URE_ANNOTATIONS}
+00009b50: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
+00009b60: 0a20 2020 2020 2020 2020 2020 2028 2261  .            ("a
+00009b70: 203d 2031 202b 2032 5c6e 6672 6f6d 2073   = 1 + 2\nfrom s
+00009b80: 6f6d 6574 6869 6e67 2069 6d70 6f72 7420  omething import 
+00009b90: 616e 6e6f 7461 7469 6f6e 7322 2c20 7365  annotations", se
+00009ba0: 7428 2929 2c0a 2020 2020 2020 2020 2020  t()),.          
+00009bb0: 2020 2822 6672 6f6d 205f 5f66 7574 7572    ("from __futur
+00009bc0: 655f 5f20 696d 706f 7274 2078 2c20 7922  e__ import x, y"
+00009bd0: 2c20 7365 7428 2929 2c0a 2020 2020 2020  , set()),.      
+00009be0: 2020 5d3a 0a20 2020 2020 2020 2020 2020    ]:.           
+00009bf0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00009c00: 7374 2873 7263 3d73 7263 2c20 6665 6174  st(src=src, feat
+00009c10: 7572 6573 3d66 6561 7475 7265 7329 3a0a  ures=features):.
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
+00009c40: 3274 6f33 5f70 6172 7365 2873 7263 290a  2to3_parse(src).
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 6675 7475 7265 5f69 6d70 6f72 7473 203d  future_imports =
+00009c70: 2070 7969 6e6b 2e67 6574 5f66 7574 7572   pyink.get_futur
+00009c80: 655f 696d 706f 7274 7328 6e6f 6465 290a  e_imports(node).
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00009cb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009cc0: 2020 2020 2020 7079 696e 6b2e 6765 745f        pyink.get_
+00009cd0: 6665 6174 7572 6573 5f75 7365 6428 6e6f  features_used(no
+00009ce0: 6465 2c20 6675 7475 7265 5f69 6d70 6f72  de, future_impor
+00009cf0: 7473 3d66 7574 7572 655f 696d 706f 7274  ts=future_import
+00009d00: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00009d10: 2020 2020 2020 2020 6665 6174 7572 6573          features
+00009d20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009d30: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+00009d40: 745f 6765 745f 6675 7475 7265 5f69 6d70  t_get_future_imp
+00009d50: 6f72 7473 2873 656c 6629 202d 3e20 4e6f  orts(self) -> No
+00009d60: 6e65 3a0a 2020 2020 2020 2020 6e6f 6465  ne:.        node
+00009d70: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
+00009d80: 5f70 6172 7365 2822 5c6e 2229 0a20 2020  _parse("\n").   
+00009d90: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00009da0: 4571 7561 6c28 7365 7428 292c 2070 7969  Equal(set(), pyi
+00009db0: 6e6b 2e67 6574 5f66 7574 7572 655f 696d  nk.get_future_im
+00009dc0: 706f 7274 7328 6e6f 6465 2929 0a20 2020  ports(node)).   
+00009dd0: 2020 2020 206e 6f64 6520 3d20 7079 696e       node = pyin
+00009de0: 6b2e 6c69 6232 746f 335f 7061 7273 6528  k.lib2to3_parse(
+00009df0: 2266 726f 6d20 5f5f 6675 7475 7265 5f5f  "from __future__
+00009e00: 2069 6d70 6f72 7420 7079 696e 6b5c 6e22   import pyink\n"
+00009e10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00009e20: 7373 6572 7445 7175 616c 287b 2270 7969  ssertEqual({"pyi
+00009e30: 6e6b 227d 2c20 7079 696e 6b2e 6765 745f  nk"}, pyink.get_
+00009e40: 6675 7475 7265 5f69 6d70 6f72 7473 286e  future_imports(n
+00009e50: 6f64 6529 290a 2020 2020 2020 2020 6e6f  ode)).        no
+00009e60: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
+00009e70: 6f33 5f70 6172 7365 2822 6672 6f6d 205f  o3_parse("from _
+00009e80: 5f66 7574 7572 655f 5f20 696d 706f 7274  _future__ import
+00009e90: 206d 756c 7469 706c 652c 2069 6d70 6f72   multiple, impor
+00009ea0: 7473 5c6e 2229 0a20 2020 2020 2020 2073  ts\n").        s
+00009eb0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00009ec0: 7b22 6d75 6c74 6970 6c65 222c 2022 696d  {"multiple", "im
+00009ed0: 706f 7274 7322 7d2c 2070 7969 6e6b 2e67  ports"}, pyink.g
+00009ee0: 6574 5f66 7574 7572 655f 696d 706f 7274  et_future_import
+00009ef0: 7328 6e6f 6465 2929 0a20 2020 2020 2020  s(node)).       
+00009f00: 206e 6f64 6520 3d20 7079 696e 6b2e 6c69   node = pyink.li
+00009f10: 6232 746f 335f 7061 7273 6528 2266 726f  b2to3_parse("fro
+00009f20: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
+00009f30: 6f72 7420 2870 6172 656e 7468 6573 697a  ort (parenthesiz
+00009f40: 6564 2c20 696d 706f 7274 7329 5c6e 2229  ed, imports)\n")
+00009f50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009f60: 7365 7274 4571 7561 6c28 7b22 7061 7265  sertEqual({"pare
+00009f70: 6e74 6865 7369 7a65 6422 2c20 2269 6d70  nthesized", "imp
+00009f80: 6f72 7473 227d 2c20 7079 696e 6b2e 6765  orts"}, pyink.ge
+00009f90: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
+00009fa0: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
+00009fb0: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
+00009fc0: 3274 6f33 5f70 6172 7365 280a 2020 2020  2to3_parse(.    
+00009fd0: 2020 2020 2020 2020 2266 726f 6d20 5f5f          "from __
+00009fe0: 6675 7475 7265 5f5f 2069 6d70 6f72 7420  future__ import 
+00009ff0: 6d75 6c74 6970 6c65 5c6e 6672 6f6d 205f  multiple\nfrom _
+0000a000: 5f66 7574 7572 655f 5f20 696d 706f 7274  _future__ import
+0000a010: 2069 6d70 6f72 7473 5c6e 220a 2020 2020   imports\n".    
+0000a020: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0000a030: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
+0000a040: 226d 756c 7469 706c 6522 2c20 2269 6d70  "multiple", "imp
+0000a050: 6f72 7473 227d 2c20 7079 696e 6b2e 6765  orts"}, pyink.ge
+0000a060: 745f 6675 7475 7265 5f69 6d70 6f72 7473  t_future_imports
+0000a070: 286e 6f64 6529 290a 2020 2020 2020 2020  (node)).        
+0000a080: 6e6f 6465 203d 2070 7969 6e6b 2e6c 6962  node = pyink.lib
+0000a090: 3274 6f33 5f70 6172 7365 2822 2320 636f  2to3_parse("# co
+0000a0a0: 6d6d 656e 745c 6e66 726f 6d20 5f5f 6675  mment\nfrom __fu
+0000a0b0: 7475 7265 5f5f 2069 6d70 6f72 7420 7079  ture__ import py
+0000a0c0: 696e 6b5c 6e22 290a 2020 2020 2020 2020  ink\n").        
+0000a0d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000a0e0: 287b 2270 7969 6e6b 227d 2c20 7079 696e  ({"pyink"}, pyin
+0000a0f0: 6b2e 6765 745f 6675 7475 7265 5f69 6d70  k.get_future_imp
+0000a100: 6f72 7473 286e 6f64 6529 290a 2020 2020  orts(node)).    
+0000a110: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
+0000a120: 2e6c 6962 3274 6f33 5f70 6172 7365 2827  .lib2to3_parse('
+0000a130: 2222 2264 6f63 7374 7269 6e67 2222 225c  """docstring"""\
+0000a140: 6e66 726f 6d20 5f5f 6675 7475 7265 5f5f  nfrom __future__
+0000a150: 2069 6d70 6f72 7420 7079 696e 6b5c 6e27   import pyink\n'
+0000a160: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000a170: 7373 6572 7445 7175 616c 287b 2270 7969  ssertEqual({"pyi
+0000a180: 6e6b 227d 2c20 7079 696e 6b2e 6765 745f  nk"}, pyink.get_
+0000a190: 6675 7475 7265 5f69 6d70 6f72 7473 286e  future_imports(n
+0000a1a0: 6f64 6529 290a 2020 2020 2020 2020 6e6f  ode)).        no
+0000a1b0: 6465 203d 2070 7969 6e6b 2e6c 6962 3274  de = pyink.lib2t
+0000a1c0: 6f33 5f70 6172 7365 2822 736f 6d65 286f  o3_parse("some(o
+0000a1d0: 7468 6572 2c20 636f 6465 295c 6e66 726f  ther, code)\nfro
+0000a1e0: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
+0000a1f0: 6f72 7420 7079 696e 6b5c 6e22 290a 2020  ort pyink\n").  
+0000a200: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000a210: 7445 7175 616c 2873 6574 2829 2c20 7079  tEqual(set(), py
+0000a220: 696e 6b2e 6765 745f 6675 7475 7265 5f69  ink.get_future_i
+0000a230: 6d70 6f72 7473 286e 6f64 6529 290a 2020  mports(node)).  
+0000a240: 2020 2020 2020 6e6f 6465 203d 2070 7969        node = pyi
+0000a250: 6e6b 2e6c 6962 3274 6f33 5f70 6172 7365  nk.lib2to3_parse
+0000a260: 2822 6672 6f6d 2073 6f6d 652e 6d6f 6475  ("from some.modu
+0000a270: 6c65 2069 6d70 6f72 7420 7079 696e 6b5c  le import pyink\
+0000a280: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
+0000a290: 2e61 7373 6572 7445 7175 616c 2873 6574  .assertEqual(set
+0000a2a0: 2829 2c20 7079 696e 6b2e 6765 745f 6675  (), pyink.get_fu
+0000a2b0: 7475 7265 5f69 6d70 6f72 7473 286e 6f64  ture_imports(nod
+0000a2c0: 6529 290a 2020 2020 2020 2020 6e6f 6465  e)).        node
+0000a2d0: 203d 2070 7969 6e6b 2e6c 6962 3274 6f33   = pyink.lib2to3
+0000a2e0: 5f70 6172 7365 280a 2020 2020 2020 2020  _parse(.        
+0000a2f0: 2020 2020 2266 726f 6d20 5f5f 6675 7475      "from __futu
+0000a300: 7265 5f5f 2069 6d70 6f72 7420 756e 6963  re__ import unic
+0000a310: 6f64 655f 6c69 7465 7261 6c73 2061 7320  ode_literals as 
+0000a320: 5f75 6e69 636f 6465 5f6c 6974 6572 616c  _unicode_literal
+0000a330: 7322 0a20 2020 2020 2020 2029 0a20 2020  s".        ).   
+0000a340: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000a350: 4571 7561 6c28 7b22 756e 6963 6f64 655f  Equal({"unicode_
+0000a360: 6c69 7465 7261 6c73 227d 2c20 7079 696e  literals"}, pyin
+0000a370: 6b2e 6765 745f 6675 7475 7265 5f69 6d70  k.get_future_imp
+0000a380: 6f72 7473 286e 6f64 6529 290a 2020 2020  orts(node)).    
+0000a390: 2020 2020 6e6f 6465 203d 2070 7969 6e6b      node = pyink
+0000a3a0: 2e6c 6962 3274 6f33 5f70 6172 7365 280a  .lib2to3_parse(.
+0000a3b0: 2020 2020 2020 2020 2020 2020 2266 726f              "fro
+0000a3c0: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
+0000a3d0: 6f72 7420 756e 6963 6f64 655f 6c69 7465  ort unicode_lite
+0000a3e0: 7261 6c73 2061 7320 5f6c 6f6c 2c20 7072  rals as _lol, pr
+0000a3f0: 696e 7422 0a20 2020 2020 2020 2029 0a20  int".        ). 
+0000a400: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000a410: 7274 4571 7561 6c28 7b22 756e 6963 6f64  rtEqual({"unicod
+0000a420: 655f 6c69 7465 7261 6c73 222c 2022 7072  e_literals", "pr
+0000a430: 696e 7422 7d2c 2070 7969 6e6b 2e67 6574  int"}, pyink.get
+0000a440: 5f66 7574 7572 655f 696d 706f 7274 7328  _future_imports(
+0000a450: 6e6f 6465 2929 0a0a 2020 2020 4070 7974  node))..    @pyt
+0000a460: 6573 742e 6d61 726b 2e69 6e63 6f6d 7061  est.mark.incompa
+0000a470: 7469 626c 655f 7769 7468 5f6d 7970 7963  tible_with_mypyc
+0000a480: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
+0000a490: 6275 675f 7669 7369 746f 7228 7365 6c66  bug_visitor(self
+0000a4a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000a4b0: 2020 2073 6f75 7263 652c 205f 203d 2072     source, _ = r
+0000a4c0: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
+0000a4d0: 6c61 6e65 6f75 7322 2c20 2264 6562 7567  laneous", "debug
+0000a4e0: 5f76 6973 6974 6f72 2229 0a20 2020 2020  _visitor").     
+0000a4f0: 2020 2065 7870 6563 7465 642c 205f 203d     expected, _ =
+0000a500: 2072 6561 645f 6461 7461 2822 6d69 7363   read_data("misc
+0000a510: 656c 6c61 6e65 6f75 7322 2c20 2264 6562  ellaneous", "deb
+0000a520: 7567 5f76 6973 6974 6f72 2e6f 7574 2229  ug_visitor.out")
+0000a530: 0a20 2020 2020 2020 206f 7574 5f6c 696e  .        out_lin
+0000a540: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+0000a550: 6572 725f 6c69 6e65 7320 3d20 5b5d 0a0a  err_lines = []..
+0000a560: 2020 2020 2020 2020 6465 6620 6f75 7428          def out(
+0000a570: 6d73 673a 2073 7472 2c20 2a2a 6b77 6172  msg: str, **kwar
+0000a580: 6773 3a20 416e 7929 202d 3e20 4e6f 6e65  gs: Any) -> None
+0000a590: 3a0a 2020 2020 2020 2020 2020 2020 6f75  :.            ou
+0000a5a0: 745f 6c69 6e65 732e 6170 7065 6e64 286d  t_lines.append(m
+0000a5b0: 7367 290a 0a20 2020 2020 2020 2064 6566  sg)..        def
+0000a5c0: 2065 7272 286d 7367 3a20 7374 722c 202a   err(msg: str, *
+0000a5d0: 2a6b 7761 7267 733a 2041 6e79 2920 2d3e  *kwargs: Any) ->
+0000a5e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a5f0: 2020 2065 7272 5f6c 696e 6573 2e61 7070     err_lines.app
+0000a600: 656e 6428 6d73 6729 0a0a 2020 2020 2020  end(msg)..      
+0000a610: 2020 7769 7468 2070 6174 6368 2822 7079    with patch("py
+0000a620: 696e 6b2e 6465 6275 672e 6f75 7422 2c20  ink.debug.out", 
+0000a630: 6f75 7429 3a0a 2020 2020 2020 2020 2020  out):.          
+0000a640: 2020 4465 6275 6756 6973 6974 6f72 2e73    DebugVisitor.s
+0000a650: 686f 7728 736f 7572 6365 290a 2020 2020  how(source).    
+0000a660: 2020 2020 6163 7475 616c 203d 2022 5c6e      actual = "\n
+0000a670: 222e 6a6f 696e 286f 7574 5f6c 696e 6573  ".join(out_lines
+0000a680: 2920 2b20 225c 6e22 0a20 2020 2020 2020  ) + "\n".       
+0000a690: 206c 6f67 5f6e 616d 6520 3d20 2222 0a20   log_name = "". 
+0000a6a0: 2020 2020 2020 2069 6620 6578 7065 6374         if expect
+0000a6b0: 6564 2021 3d20 6163 7475 616c 3a0a 2020  ed != actual:.  
+0000a6c0: 2020 2020 2020 2020 2020 6c6f 675f 6e61            log_na
+0000a6d0: 6d65 203d 2070 7969 6e6b 2e64 756d 705f  me = pyink.dump_
+0000a6e0: 746f 5f66 696c 6528 2a6f 7574 5f6c 696e  to_file(*out_lin
+0000a6f0: 6573 290a 2020 2020 2020 2020 7365 6c66  es).        self
+0000a700: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
+0000a710: 2020 2020 2020 2020 2020 6578 7065 6374            expect
+0000a720: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+0000a730: 6163 7475 616c 2c0a 2020 2020 2020 2020  actual,.        
+0000a740: 2020 2020 6622 4153 5420 7072 696e 7420      f"AST print 
+0000a750: 6f75 7420 6973 2064 6966 6665 7265 6e74  out is different
+0000a760: 2e20 4163 7475 616c 2076 6572 7369 6f6e  . Actual version
+0000a770: 2064 756d 7065 6420 746f 207b 6c6f 675f   dumped to {log_
+0000a780: 6e61 6d65 7d22 2c0a 2020 2020 2020 2020  name}",.        
+0000a790: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000a7a0: 666f 726d 6174 5f66 696c 655f 636f 6e74  format_file_cont
+0000a7b0: 656e 7473 2873 656c 6629 202d 3e20 4e6f  ents(self) -> No
+0000a7c0: 6e65 3a0a 2020 2020 2020 2020 6d6f 6465  ne:.        mode
+0000a7d0: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
+0000a7e0: 2020 2020 2020 2020 656d 7074 7920 3d20          empty = 
+0000a7f0: 2222 0a20 2020 2020 2020 2077 6974 6820  "".        with 
+0000a800: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+0000a810: 7328 7079 696e 6b2e 4e6f 7468 696e 6743  s(pyink.NothingC
+0000a820: 6861 6e67 6564 293a 0a20 2020 2020 2020  hanged):.       
+0000a830: 2020 2020 2070 7969 6e6b 2e66 6f72 6d61       pyink.forma
+0000a840: 745f 6669 6c65 5f63 6f6e 7465 6e74 7328  t_file_contents(
+0000a850: 656d 7074 792c 206d 6f64 653d 6d6f 6465  empty, mode=mode
+0000a860: 2c20 6661 7374 3d46 616c 7365 290a 2020  , fast=False).  
+0000a870: 2020 2020 2020 6a75 7374 5f6e 6c20 3d20        just_nl = 
+0000a880: 225c 6e22 0a20 2020 2020 2020 2077 6974  "\n".        wit
+0000a890: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+0000a8a0: 7365 7328 7079 696e 6b2e 4e6f 7468 696e  ses(pyink.Nothin
+0000a8b0: 6743 6861 6e67 6564 293a 0a20 2020 2020  gChanged):.     
+0000a8c0: 2020 2020 2020 2070 7969 6e6b 2e66 6f72         pyink.for
+0000a8d0: 6d61 745f 6669 6c65 5f63 6f6e 7465 6e74  mat_file_content
+0000a8e0: 7328 6a75 7374 5f6e 6c2c 206d 6f64 653d  s(just_nl, mode=
+0000a8f0: 6d6f 6465 2c20 6661 7374 3d46 616c 7365  mode, fast=False
+0000a900: 290a 2020 2020 2020 2020 7361 6d65 203d  ).        same =
+0000a910: 2022 6a20 3d20 5b31 2c20 322c 2033 5d5c   "j = [1, 2, 3]\
+0000a920: 6e22 0a20 2020 2020 2020 2077 6974 6820  n".        with 
+0000a930: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+0000a940: 7328 7079 696e 6b2e 4e6f 7468 696e 6743  s(pyink.NothingC
+0000a950: 6861 6e67 6564 293a 0a20 2020 2020 2020  hanged):.       
+0000a960: 2020 2020 2070 7969 6e6b 2e66 6f72 6d61       pyink.forma
+0000a970: 745f 6669 6c65 5f63 6f6e 7465 6e74 7328  t_file_contents(
+0000a980: 7361 6d65 2c20 6d6f 6465 3d6d 6f64 652c  same, mode=mode,
+0000a990: 2066 6173 743d 4661 6c73 6529 0a20 2020   fast=False).   
+0000a9a0: 2020 2020 2064 6966 6665 7265 6e74 203d       different =
+0000a9b0: 2022 6a20 3d20 5b31 2c32 2c33 5d22 0a20   "j = [1,2,3]". 
+0000a9c0: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
+0000a9d0: 3d20 7361 6d65 0a20 2020 2020 2020 2061  = same.        a
+0000a9e0: 6374 7561 6c20 3d20 7079 696e 6b2e 666f  ctual = pyink.fo
+0000a9f0: 726d 6174 5f66 696c 655f 636f 6e74 656e  rmat_file_conten
+0000aa00: 7473 2864 6966 6665 7265 6e74 2c20 6d6f  ts(different, mo
+0000aa10: 6465 3d6d 6f64 652c 2066 6173 743d 4661  de=mode, fast=Fa
+0000aa20: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
+0000aa30: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+0000aa40: 7065 6374 6564 2c20 6163 7475 616c 290a  pected, actual).
+0000aa50: 2020 2020 2020 2020 696e 7661 6c69 6420          invalid 
+0000aa60: 3d20 2272 6574 7572 6e20 6966 2079 6f75  = "return if you
+0000aa70: 2063 616e 220a 2020 2020 2020 2020 7769   can".        wi
+0000aa80: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0000aa90: 6973 6573 2870 7969 6e6b 2e49 6e76 616c  ises(pyink.Inval
+0000aaa0: 6964 496e 7075 7429 2061 7320 653a 0a20  idInput) as e:. 
+0000aab0: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
+0000aac0: 2e66 6f72 6d61 745f 6669 6c65 5f63 6f6e  .format_file_con
+0000aad0: 7465 6e74 7328 696e 7661 6c69 642c 206d  tents(invalid, m
+0000aae0: 6f64 653d 6d6f 6465 2c20 6661 7374 3d46  ode=mode, fast=F
+0000aaf0: 616c 7365 290a 2020 2020 2020 2020 7365  alse).        se
+0000ab00: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+0000ab10: 7472 2865 2e65 7863 6570 7469 6f6e 292c  tr(e.exception),
+0000ab20: 2022 4361 6e6e 6f74 2070 6172 7365 3a20   "Cannot parse: 
+0000ab30: 313a 373a 2072 6574 7572 6e20 6966 2079  1:7: return if y
+0000ab40: 6f75 2063 616e 2229 0a0a 2020 2020 2020  ou can")..      
+0000ab50: 2020 6d6f 6465 203d 2070 7969 6e6b 2e4d    mode = pyink.M
+0000ab60: 6f64 6528 7072 6576 6965 773d 5472 7565  ode(preview=True
+0000ab70: 290a 2020 2020 2020 2020 6a75 7374 5f63  ).        just_c
+0000ab80: 726c 6620 3d20 225c 725c 6e22 0a20 2020  rlf = "\r\n".   
+0000ab90: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+0000aba0: 7373 6572 7452 6169 7365 7328 7079 696e  ssertRaises(pyin
+0000abb0: 6b2e 4e6f 7468 696e 6743 6861 6e67 6564  k.NothingChanged
+0000abc0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+0000abd0: 7969 6e6b 2e66 6f72 6d61 745f 6669 6c65  yink.format_file
+0000abe0: 5f63 6f6e 7465 6e74 7328 6a75 7374 5f63  _contents(just_c
+0000abf0: 726c 662c 206d 6f64 653d 6d6f 6465 2c20  rlf, mode=mode, 
+0000ac00: 6661 7374 3d46 616c 7365 290a 2020 2020  fast=False).    
+0000ac10: 2020 2020 6a75 7374 5f77 6869 7465 7370      just_whitesp
+0000ac20: 6163 655f 6e6c 203d 2022 5c6e 5c74 5c6e  ace_nl = "\n\t\n
+0000ac30: 205c 6e5c 7420 5c6e 205c 745c 6e5c 6e22   \n\t \n \t\n\n"
+0000ac40: 0a20 2020 2020 2020 2061 6374 7561 6c20  .        actual 
+0000ac50: 3d20 7079 696e 6b2e 666f 726d 6174 5f66  = pyink.format_f
+0000ac60: 696c 655f 636f 6e74 656e 7473 286a 7573  ile_contents(jus
+0000ac70: 745f 7768 6974 6573 7061 6365 5f6e 6c2c  t_whitespace_nl,
+0000ac80: 206d 6f64 653d 6d6f 6465 2c20 6661 7374   mode=mode, fast
+0000ac90: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+0000aca0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000acb0: 2822 5c6e 222c 2061 6374 7561 6c29 0a20  ("\n", actual). 
+0000acc0: 2020 2020 2020 206a 7573 745f 7768 6974         just_whit
+0000acd0: 6573 7061 6365 5f63 726c 6620 3d20 225c  espace_crlf = "\
+0000ace0: 725c 6e5c 745c 725c 6e20 5c72 5c6e 5c74  r\n\t\r\n \r\n\t
+0000acf0: 205c 725c 6e20 5c74 5c72 5c6e 5c72 5c6e   \r\n \t\r\n\r\n
+0000ad00: 220a 2020 2020 2020 2020 6163 7475 616c  ".        actual
+0000ad10: 203d 2070 7969 6e6b 2e66 6f72 6d61 745f   = pyink.format_
+0000ad20: 6669 6c65 5f63 6f6e 7465 6e74 7328 6a75  file_contents(ju
+0000ad30: 7374 5f77 6869 7465 7370 6163 655f 6372  st_whitespace_cr
+0000ad40: 6c66 2c20 6d6f 6465 3d6d 6f64 652c 2066  lf, mode=mode, f
+0000ad50: 6173 743d 4661 6c73 6529 0a20 2020 2020  ast=False).     
+0000ad60: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000ad70: 7561 6c28 225c 725c 6e22 2c20 6163 7475  ual("\r\n", actu
+0000ad80: 616c 290a 0a20 2020 2064 6566 2074 6573  al)..    def tes
+0000ad90: 745f 656e 646d 6172 6b65 7228 7365 6c66  t_endmarker(self
+0000ada0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000adb0: 2020 206e 203d 2070 7969 6e6b 2e6c 6962     n = pyink.lib
+0000adc0: 3274 6f33 5f70 6172 7365 2822 5c6e 2229  2to3_parse("\n")
+0000add0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000ade0: 7365 7274 4571 7561 6c28 6e2e 7479 7065  sertEqual(n.type
+0000adf0: 2c20 7079 696e 6b2e 7379 6d73 2e66 696c  , pyink.syms.fil
+0000ae00: 655f 696e 7075 7429 0a20 2020 2020 2020  e_input).       
+0000ae10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000ae20: 6c28 6c65 6e28 6e2e 6368 696c 6472 656e  l(len(n.children
+0000ae30: 292c 2031 290a 2020 2020 2020 2020 7365  ), 1).        se
+0000ae40: 6c66 2e61 7373 6572 7445 7175 616c 286e  lf.assertEqual(n
+0000ae50: 2e63 6869 6c64 7265 6e5b 305d 2e74 7970  .children[0].typ
+0000ae60: 652c 2070 7969 6e6b 2e74 6f6b 656e 2e45  e, pyink.token.E
+0000ae70: 4e44 4d41 524b 4552 290a 0a20 2020 2040  NDMARKER)..    @
+0000ae80: 7079 7465 7374 2e6d 6172 6b2e 696e 636f  pytest.mark.inco
+0000ae90: 6d70 6174 6962 6c65 5f77 6974 685f 6d79  mpatible_with_my
+0000aea0: 7079 630a 2020 2020 4075 6e69 7474 6573  pyc.    @unittes
+0000aeb0: 742e 736b 6970 4966 286f 732e 656e 7669  t.skipIf(os.envi
+0000aec0: 726f 6e2e 6765 7428 2253 4b49 505f 4153  ron.get("SKIP_AS
+0000aed0: 545f 5052 494e 5422 292c 2022 7573 6572  T_PRINT"), "user
+0000aee0: 2073 6574 2053 4b49 505f 4153 545f 5052   set SKIP_AST_PR
+0000aef0: 494e 5422 290a 2020 2020 6465 6620 7465  INT").    def te
+0000af00: 7374 5f61 7373 6572 7446 6f72 6d61 7445  st_assertFormatE
+0000af10: 7175 616c 2873 656c 6629 202d 3e20 4e6f  qual(self) -> No
+0000af20: 6e65 3a0a 2020 2020 2020 2020 6f75 745f  ne:.        out_
+0000af30: 6c69 6e65 7320 3d20 5b5d 0a20 2020 2020  lines = [].     
+0000af40: 2020 2065 7272 5f6c 696e 6573 203d 205b     err_lines = [
+0000af50: 5d0a 0a20 2020 2020 2020 2064 6566 206f  ]..        def o
+0000af60: 7574 286d 7367 3a20 7374 722c 202a 2a6b  ut(msg: str, **k
+0000af70: 7761 7267 733a 2041 6e79 2920 2d3e 204e  wargs: Any) -> N
+0000af80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000af90: 206f 7574 5f6c 696e 6573 2e61 7070 656e   out_lines.appen
+0000afa0: 6428 6d73 6729 0a0a 2020 2020 2020 2020  d(msg)..        
+0000afb0: 6465 6620 6572 7228 6d73 673a 2073 7472  def err(msg: str
+0000afc0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
+0000afd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000afe0: 2020 2020 2020 6572 725f 6c69 6e65 732e        err_lines.
+0000aff0: 6170 7065 6e64 286d 7367 290a 0a20 2020  append(msg)..   
+0000b000: 2020 2020 2077 6974 6820 7061 7463 6828       with patch(
+0000b010: 2270 7969 6e6b 2e6f 7574 7075 742e 5f6f  "pyink.output._o
+0000b020: 7574 222c 206f 7574 292c 2070 6174 6368  ut", out), patch
+0000b030: 2822 7079 696e 6b2e 6f75 7470 7574 2e5f  ("pyink.output._
+0000b040: 6572 7222 2c20 6572 7229 3a0a 2020 2020  err", err):.    
+0000b050: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000b060: 662e 6173 7365 7274 5261 6973 6573 2841  f.assertRaises(A
+0000b070: 7373 6572 7469 6f6e 4572 726f 7229 3a0a  ssertionError):.
+0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b090: 7365 6c66 2e61 7373 6572 7446 6f72 6d61  self.assertForma
+0000b0a0: 7445 7175 616c 2822 6a20 3d20 5b31 2c20  tEqual("j = [1, 
+0000b0b0: 322c 2033 5d22 2c20 226a 203d 205b 312c  2, 3]", "j = [1,
+0000b0c0: 2032 2c20 332c 5d22 290a 0a20 2020 2020   2, 3,]")..     
+0000b0d0: 2020 206f 7574 5f73 7472 203d 2022 222e     out_str = "".
+0000b0e0: 6a6f 696e 286f 7574 5f6c 696e 6573 290a  join(out_lines).
+0000b0f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000b100: 6572 7449 6e28 2245 7870 6563 7465 6420  ertIn("Expected 
+0000b110: 7472 6565 3a22 2c20 6f75 745f 7374 7229  tree:", out_str)
+0000b120: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000b130: 7365 7274 496e 2822 4163 7475 616c 2074  sertIn("Actual t
+0000b140: 7265 653a 222c 206f 7574 5f73 7472 290a  ree:", out_str).
+0000b150: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000b160: 6572 7445 7175 616c 2822 222e 6a6f 696e  ertEqual("".join
+0000b170: 2865 7272 5f6c 696e 6573 292c 2022 2229  (err_lines), "")
+0000b180: 0a0a 2020 2020 4065 7665 6e74 5f6c 6f6f  ..    @event_loo
+0000b190: 7028 290a 2020 2020 4070 6174 6368 2822  p().    @patch("
+0000b1a0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+0000b1b0: 6573 2e50 726f 6365 7373 506f 6f6c 4578  es.ProcessPoolEx
+0000b1c0: 6563 7574 6f72 222c 204d 6167 6963 4d6f  ecutor", MagicMo
+0000b1d0: 636b 2873 6964 655f 6566 6665 6374 3d4f  ck(side_effect=O
+0000b1e0: 5345 7272 6f72 2929 0a20 2020 2064 6566  SError)).    def
+0000b1f0: 2074 6573 745f 776f 726b 735f 696e 5f6d   test_works_in_m
+0000b200: 6f6e 6f5f 7072 6f63 6573 735f 6f6e 6c79  ono_process_only
+0000b210: 5f65 6e76 6972 6f6e 6d65 6e74 2873 656c  _environment(sel
+0000b220: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000b230: 2020 2020 7769 7468 2063 6163 6865 5f64      with cache_d
+0000b240: 6972 2829 2061 7320 776f 726b 7370 6163  ir() as workspac
+0000b250: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0000b260: 6f72 2066 2069 6e20 5b0a 2020 2020 2020  or f in [.      
+0000b270: 2020 2020 2020 2020 2020 2877 6f72 6b73            (works
+0000b280: 7061 6365 202f 2022 6f6e 652e 7079 2229  pace / "one.py")
+0000b290: 2e72 6573 6f6c 7665 2829 2c0a 2020 2020  .resolve(),.    
+0000b2a0: 2020 2020 2020 2020 2020 2020 2877 6f72              (wor
+0000b2b0: 6b73 7061 6365 202f 2022 7477 6f2e 7079  kspace / "two.py
+0000b2c0: 2229 2e72 6573 6f6c 7665 2829 2c0a 2020  ").resolve(),.  
+0000b2d0: 2020 2020 2020 2020 2020 5d3a 0a20 2020            ]:.   
+0000b2e0: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
+0000b2f0: 7269 7465 5f74 6578 7428 2770 7269 6e74  rite_text('print
+0000b300: 2822 6865 6c6c 6f22 295c 6e27 290a 2020  ("hello")\n').  
+0000b310: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+0000b320: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
+0000b330: 776f 726b 7370 6163 6529 5d29 0a0a 2020  workspace)])..  
+0000b340: 2020 4065 7665 6e74 5f6c 6f6f 7028 290a    @event_loop().
+0000b350: 2020 2020 6465 6620 7465 7374 5f63 6865      def test_che
+0000b360: 636b 5f64 6966 665f 7573 655f 746f 6765  ck_diff_use_toge
+0000b370: 7468 6572 2873 656c 6629 202d 3e20 4e6f  ther(self) -> No
+0000b380: 6e65 3a0a 2020 2020 2020 2020 7769 7468  ne:.        with
+0000b390: 2063 6163 6865 5f64 6972 2829 3a0a 2020   cache_dir():.  
+0000b3a0: 2020 2020 2020 2020 2020 2320 4669 6c65            # File
+0000b3b0: 7320 7768 6963 6820 7769 6c6c 2062 6520  s which will be 
+0000b3c0: 7265 666f 726d 6174 7465 642e 0a20 2020  reformatted..   
+0000b3d0: 2020 2020 2020 2020 2073 7263 3120 3d20           src1 = 
+0000b3e0: 6765 745f 6361 7365 5f70 6174 6828 226d  get_case_path("m
+0000b3f0: 6973 6365 6c6c 616e 656f 7573 222c 2022  iscellaneous", "
+0000b400: 7374 7269 6e67 5f71 756f 7465 7322 290a  string_quotes").
+0000b410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b420: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+0000b430: 7228 7372 6331 292c 2022 2d2d 6469 6666  r(src1), "--diff
+0000b440: 222c 2022 2d2d 6368 6563 6b22 5d2c 2065  ", "--check"], e
+0000b450: 7869 745f 636f 6465 3d31 290a 2020 2020  xit_code=1).    
+0000b460: 2020 2020 2020 2020 2320 4669 6c65 7320          # Files 
+0000b470: 7768 6963 6820 7769 6c6c 206e 6f74 2062  which will not b
+0000b480: 6520 7265 666f 726d 6174 7465 642e 0a20  e reformatted.. 
+0000b490: 2020 2020 2020 2020 2020 2073 7263 3220             src2 
+0000b4a0: 3d20 6765 745f 6361 7365 5f70 6174 6828  = get_case_path(
+0000b4b0: 2273 696d 706c 655f 6361 7365 7322 2c20  "simple_cases", 
+0000b4c0: 2263 6f6d 706f 7369 7469 6f6e 2229 0a20  "composition"). 
+0000b4d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b4e0: 696e 766f 6b65 426c 6163 6b28 5b73 7472  invokeBlack([str
+0000b4f0: 2873 7263 3229 2c20 222d 2d64 6966 6622  (src2), "--diff"
+0000b500: 2c20 222d 2d63 6865 636b 225d 290a 2020  , "--check"]).  
+0000b510: 2020 2020 2020 2020 2020 2320 4d75 6c74            # Mult
+0000b520: 6920 6669 6c65 2063 6f6d 6d61 6e64 2e0a  i file command..
+0000b530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b540: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+0000b550: 7228 7372 6331 292c 2073 7472 2873 7263  r(src1), str(src
+0000b560: 3229 2c20 222d 2d64 6966 6622 2c20 222d  2), "--diff", "-
+0000b570: 2d63 6865 636b 225d 2c20 6578 6974 5f63  -check"], exit_c
+0000b580: 6f64 653d 3129 0a0a 2020 2020 6465 6620  ode=1)..    def 
+0000b590: 7465 7374 5f6e 6f5f 7372 635f 6661 696c  test_no_src_fail
+0000b5a0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
+0000b5b0: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
+0000b5c0: 6368 655f 6469 7228 293a 0a20 2020 2020  che_dir():.     
+0000b5d0: 2020 2020 2020 2073 656c 662e 696e 766f         self.invo
+0000b5e0: 6b65 426c 6163 6b28 5b5d 2c20 6578 6974  keBlack([], exit
+0000b5f0: 5f63 6f64 653d 3129 0a0a 2020 2020 6465  _code=1)..    de
+0000b600: 6620 7465 7374 5f73 7263 5f61 6e64 5f63  f test_src_and_c
+0000b610: 6f64 655f 6661 696c 7328 7365 6c66 2920  ode_fails(self) 
+0000b620: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000b630: 2077 6974 6820 6361 6368 655f 6469 7228   with cache_dir(
+0000b640: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000b650: 656c 662e 696e 766f 6b65 426c 6163 6b28  elf.invokeBlack(
+0000b660: 5b22 2e22 2c20 222d 6322 2c20 2230 225d  [".", "-c", "0"]
+0000b670: 2c20 6578 6974 5f63 6f64 653d 3129 0a0a  , exit_code=1)..
+0000b680: 2020 2020 6465 6620 7465 7374 5f62 726f      def test_bro
+0000b690: 6b65 6e5f 7379 6d6c 696e 6b28 7365 6c66  ken_symlink(self
+0000b6a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000b6b0: 2020 2077 6974 6820 6361 6368 655f 6469     with cache_di
+0000b6c0: 7228 2920 6173 2077 6f72 6b73 7061 6365  r() as workspace
+0000b6d0: 3a0a 2020 2020 2020 2020 2020 2020 7379  :.            sy
+0000b6e0: 6d6c 696e 6b20 3d20 776f 726b 7370 6163  mlink = workspac
+0000b6f0: 6520 2f20 2262 726f 6b65 6e5f 6c69 6e6b  e / "broken_link
+0000b700: 2e70 7922 0a20 2020 2020 2020 2020 2020  .py".           
+0000b710: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000b720: 2020 2020 2020 7379 6d6c 696e 6b2e 7379        symlink.sy
+0000b730: 6d6c 696e 6b5f 746f 2822 6e6f 6e65 7869  mlink_to("nonexi
+0000b740: 7374 656e 742e 7079 2229 0a20 2020 2020  stent.py").     
+0000b750: 2020 2020 2020 2065 7863 6570 7420 284f         except (O
+0000b760: 5345 7272 6f72 2c20 4e6f 7449 6d70 6c65  SError, NotImple
+0000b770: 6d65 6e74 6564 4572 726f 7229 2061 7320  mentedError) as 
+0000b780: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000b790: 2020 2073 656c 662e 736b 6970 5465 7374     self.skipTest
+0000b7a0: 2866 2243 616e 2774 2063 7265 6174 6520  (f"Can't create 
+0000b7b0: 7379 6d6c 696e 6b73 3a20 7b65 7d22 290a  symlinks: {e}").
+0000b7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b7d0: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+0000b7e0: 7228 776f 726b 7370 6163 652e 7265 736f  r(workspace.reso
+0000b7f0: 6c76 6528 2929 5d29 0a0a 2020 2020 6465  lve())])..    de
+0000b800: 6620 7465 7374 5f73 696e 676c 655f 6669  f test_single_fi
+0000b810: 6c65 5f66 6f72 6365 5f70 7969 2873 656c  le_force_pyi(sel
+0000b820: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000b830: 2020 2020 7079 695f 6d6f 6465 203d 2072      pyi_mode = r
+0000b840: 6570 6c61 6365 2844 4546 4155 4c54 5f4d  eplace(DEFAULT_M
+0000b850: 4f44 452c 2069 735f 7079 693d 5472 7565  ODE, is_pyi=True
+0000b860: 290a 2020 2020 2020 2020 636f 6e74 656e  ).        conten
+0000b870: 7473 2c20 6578 7065 6374 6564 203d 2072  ts, expected = r
+0000b880: 6561 645f 6461 7461 2822 6d69 7363 656c  ead_data("miscel
+0000b890: 6c61 6e65 6f75 7322 2c20 2266 6f72 6365  laneous", "force
+0000b8a0: 5f70 7969 2229 0a20 2020 2020 2020 2077  _pyi").        w
+0000b8b0: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
+0000b8c0: 6173 2077 6f72 6b73 7061 6365 3a0a 2020  as workspace:.  
+0000b8d0: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+0000b8e0: 2028 776f 726b 7370 6163 6520 2f20 2266   (workspace / "f
+0000b8f0: 696c 652e 7079 2229 2e72 6573 6f6c 7665  ile.py").resolve
+0000b900: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
+0000b910: 6974 6820 6f70 656e 2870 6174 682c 2022  ith open(path, "
+0000b920: 7722 2920 6173 2066 683a 0a20 2020 2020  w") as fh:.     
+0000b930: 2020 2020 2020 2020 2020 2066 682e 7772             fh.wr
+0000b940: 6974 6528 636f 6e74 656e 7473 290a 2020  ite(contents).  
+0000b950: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+0000b960: 6e76 6f6b 6542 6c61 636b 285b 7374 7228  nvokeBlack([str(
+0000b970: 7061 7468 292c 2022 2d2d 7079 6922 5d29  path), "--pyi"])
+0000b980: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000b990: 6820 6f70 656e 2870 6174 682c 2022 7222  h open(path, "r"
+0000b9a0: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
+0000b9b0: 2020 2020 2020 2020 2061 6374 7561 6c20           actual 
+0000b9c0: 3d20 6668 2e72 6561 6428 290a 2020 2020  = fh.read().    
+0000b9d0: 2020 2020 2020 2020 2320 7665 7269 6679          # verify
+0000b9e0: 2063 6163 6865 2077 6974 6820 2d2d 7079   cache with --py
+0000b9f0: 6920 6973 2073 6570 6172 6174 650a 2020  i is separate.  
+0000ba00: 2020 2020 2020 2020 2020 7079 695f 6361            pyi_ca
+0000ba10: 6368 6520 3d20 7079 696e 6b2e 7265 6164  che = pyink.read
+0000ba20: 5f63 6163 6865 2870 7969 5f6d 6f64 6529  _cache(pyi_mode)
+0000ba30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ba40: 662e 6173 7365 7274 496e 2873 7472 2870  f.assertIn(str(p
+0000ba50: 6174 6829 2c20 7079 695f 6361 6368 6529  ath), pyi_cache)
+0000ba60: 0a20 2020 2020 2020 2020 2020 206e 6f72  .            nor
+0000ba70: 6d61 6c5f 6361 6368 6520 3d20 7079 696e  mal_cache = pyin
+0000ba80: 6b2e 7265 6164 5f63 6163 6865 2844 4546  k.read_cache(DEF
+0000ba90: 4155 4c54 5f4d 4f44 4529 0a20 2020 2020  AULT_MODE).     
+0000baa0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000bab0: 7274 4e6f 7449 6e28 7374 7228 7061 7468  rtNotIn(str(path
+0000bac0: 292c 206e 6f72 6d61 6c5f 6361 6368 6529  ), normal_cache)
+0000bad0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000bae0: 7365 7274 466f 726d 6174 4571 7561 6c28  sertFormatEqual(
+0000baf0: 6578 7065 6374 6564 2c20 6163 7475 616c  expected, actual
+0000bb00: 290a 2020 2020 2020 2020 7079 696e 6b2e  ).        pyink.
+0000bb10: 6173 7365 7274 5f65 7175 6976 616c 656e  assert_equivalen
+0000bb20: 7428 636f 6e74 656e 7473 2c20 6163 7475  t(contents, actu
+0000bb30: 616c 290a 2020 2020 2020 2020 7079 696e  al).        pyin
+0000bb40: 6b2e 6173 7365 7274 5f73 7461 626c 6528  k.assert_stable(
+0000bb50: 636f 6e74 656e 7473 2c20 6163 7475 616c  contents, actual
+0000bb60: 2c20 7079 695f 6d6f 6465 290a 0a20 2020  , pyi_mode)..   
+0000bb70: 2040 6576 656e 745f 6c6f 6f70 2829 0a20   @event_loop(). 
+0000bb80: 2020 2064 6566 2074 6573 745f 6d75 6c74     def test_mult
+0000bb90: 695f 6669 6c65 5f66 6f72 6365 5f70 7969  i_file_force_pyi
+0000bba0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000bbb0: 2020 2020 2020 2020 7265 675f 6d6f 6465          reg_mode
+0000bbc0: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
+0000bbd0: 2020 2020 2020 2020 7079 695f 6d6f 6465          pyi_mode
+0000bbe0: 203d 2072 6570 6c61 6365 2844 4546 4155   = replace(DEFAU
+0000bbf0: 4c54 5f4d 4f44 452c 2069 735f 7079 693d  LT_MODE, is_pyi=
+0000bc00: 5472 7565 290a 2020 2020 2020 2020 636f  True).        co
+0000bc10: 6e74 656e 7473 2c20 6578 7065 6374 6564  ntents, expected
+0000bc20: 203d 2072 6561 645f 6461 7461 2822 6d69   = read_data("mi
+0000bc30: 7363 656c 6c61 6e65 6f75 7322 2c20 2266  scellaneous", "f
+0000bc40: 6f72 6365 5f70 7969 2229 0a20 2020 2020  orce_pyi").     
+0000bc50: 2020 2077 6974 6820 6361 6368 655f 6469     with cache_di
+0000bc60: 7228 2920 6173 2077 6f72 6b73 7061 6365  r() as workspace
+0000bc70: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000bc80: 7468 7320 3d20 5b0a 2020 2020 2020 2020  ths = [.        
+0000bc90: 2020 2020 2020 2020 2877 6f72 6b73 7061          (workspa
+0000bca0: 6365 202f 2022 6669 6c65 312e 7079 2229  ce / "file1.py")
+0000bcb0: 2e72 6573 6f6c 7665 2829 2c0a 2020 2020  .resolve(),.    
+0000bcc0: 2020 2020 2020 2020 2020 2020 2877 6f72              (wor
+0000bcd0: 6b73 7061 6365 202f 2022 6669 6c65 322e  kspace / "file2.
+0000bce0: 7079 2229 2e72 6573 6f6c 7665 2829 2c0a  py").resolve(),.
+0000bcf0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+0000bd00: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
+0000bd10: 7468 2069 6e20 7061 7468 733a 0a20 2020  th in paths:.   
+0000bd20: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000bd30: 6820 6f70 656e 2870 6174 682c 2022 7722  h open(path, "w"
+0000bd40: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
+0000bd50: 2020 2020 2020 2020 2020 2020 2066 682e               fh.
+0000bd60: 7772 6974 6528 636f 6e74 656e 7473 290a  write(contents).
+0000bd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bd80: 2e69 6e76 6f6b 6542 6c61 636b 285b 7374  .invokeBlack([st
+0000bd90: 7228 7029 2066 6f72 2070 2069 6e20 7061  r(p) for p in pa
+0000bda0: 7468 735d 202b 205b 222d 2d70 7969 225d  ths] + ["--pyi"]
+0000bdb0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000bdc0: 7220 7061 7468 2069 6e20 7061 7468 733a  r path in paths:
+0000bdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bde0: 2077 6974 6820 6f70 656e 2870 6174 682c   with open(path,
+0000bdf0: 2022 7222 2920 6173 2066 683a 0a20 2020   "r") as fh:.   
+0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be10: 2061 6374 7561 6c20 3d20 6668 2e72 6561   actual = fh.rea
+0000be20: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+0000be30: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000be40: 7175 616c 2861 6374 7561 6c2c 2065 7870  qual(actual, exp
+0000be50: 6563 7465 6429 0a20 2020 2020 2020 2020  ected).         
+0000be60: 2020 2023 2076 6572 6966 7920 6361 6368     # verify cach
+0000be70: 6520 7769 7468 202d 2d70 7969 2069 7320  e with --pyi is 
+0000be80: 7365 7061 7261 7465 0a20 2020 2020 2020  separate.       
+0000be90: 2020 2020 2070 7969 5f63 6163 6865 203d       pyi_cache =
+0000bea0: 2070 7969 6e6b 2e72 6561 645f 6361 6368   pyink.read_cach
+0000beb0: 6528 7079 695f 6d6f 6465 290a 2020 2020  e(pyi_mode).    
+0000bec0: 2020 2020 2020 2020 6e6f 726d 616c 5f63          normal_c
+0000bed0: 6163 6865 203d 2070 7969 6e6b 2e72 6561  ache = pyink.rea
+0000bee0: 645f 6361 6368 6528 7265 675f 6d6f 6465  d_cache(reg_mode
+0000bef0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000bf00: 7220 7061 7468 2069 6e20 7061 7468 733a  r path in paths:
+0000bf10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf20: 2073 656c 662e 6173 7365 7274 496e 2873   self.assertIn(s
+0000bf30: 7472 2870 6174 6829 2c20 7079 695f 6361  tr(path), pyi_ca
+0000bf40: 6368 6529 0a20 2020 2020 2020 2020 2020  che).           
+0000bf50: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000bf60: 4e6f 7449 6e28 7374 7228 7061 7468 292c  NotIn(str(path),
+0000bf70: 206e 6f72 6d61 6c5f 6361 6368 6529 0a0a   normal_cache)..
+0000bf80: 2020 2020 6465 6620 7465 7374 5f70 6970      def test_pip
+0000bf90: 655f 666f 7263 655f 7079 6928 7365 6c66  e_force_pyi(self
+0000bfa0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000bfb0: 2020 2073 6f75 7263 652c 2065 7870 6563     source, expec
+0000bfc0: 7465 6420 3d20 7265 6164 5f64 6174 6128  ted = read_data(
+0000bfd0: 226d 6973 6365 6c6c 616e 656f 7573 222c  "miscellaneous",
+0000bfe0: 2022 666f 7263 655f 7079 6922 290a 2020   "force_pyi").  
+0000bff0: 2020 2020 2020 7265 7375 6c74 203d 2043        result = C
+0000c000: 6c69 5275 6e6e 6572 2829 2e69 6e76 6f6b  liRunner().invok
+0000c010: 6528 0a20 2020 2020 2020 2020 2020 2070  e(.            p
+0000c020: 7969 6e6b 2e6d 6169 6e2c 205b 222d 222c  yink.main, ["-",
+0000c030: 2022 2d71 222c 2022 2d2d 7079 6922 5d2c   "-q", "--pyi"],
+0000c040: 2069 6e70 7574 3d42 7974 6573 494f 2873   input=BytesIO(s
+0000c050: 6f75 7263 652e 656e 636f 6465 2822 7574  ource.encode("ut
+0000c060: 6638 2229 290a 2020 2020 2020 2020 290a  f8")).        ).
+0000c070: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c080: 6572 7445 7175 616c 2872 6573 756c 742e  ertEqual(result.
+0000c090: 6578 6974 5f63 6f64 652c 2030 290a 2020  exit_code, 0).  
+0000c0a0: 2020 2020 2020 6163 7475 616c 203d 2072        actual = r
+0000c0b0: 6573 756c 742e 6f75 7470 7574 0a20 2020  esult.output.   
+0000c0c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c0d0: 466f 726d 6174 4571 7561 6c28 6163 7475  FormatEqual(actu
+0000c0e0: 616c 2c20 6578 7065 6374 6564 290a 0a20  al, expected).. 
+0000c0f0: 2020 2064 6566 2074 6573 745f 7369 6e67     def test_sing
+0000c100: 6c65 5f66 696c 655f 666f 7263 655f 7079  le_file_force_py
+0000c110: 3336 2873 656c 6629 202d 3e20 4e6f 6e65  36(self) -> None
+0000c120: 3a0a 2020 2020 2020 2020 7265 675f 6d6f  :.        reg_mo
+0000c130: 6465 203d 2044 4546 4155 4c54 5f4d 4f44  de = DEFAULT_MOD
+0000c140: 450a 2020 2020 2020 2020 7079 3336 5f6d  E.        py36_m
+0000c150: 6f64 6520 3d20 7265 706c 6163 6528 4445  ode = replace(DE
+0000c160: 4641 554c 545f 4d4f 4445 2c20 7461 7267  FAULT_MODE, targ
+0000c170: 6574 5f76 6572 7369 6f6e 733d 5059 3336  et_versions=PY36
+0000c180: 5f56 4552 5349 4f4e 5329 0a20 2020 2020  _VERSIONS).     
+0000c190: 2020 2073 6f75 7263 652c 2065 7870 6563     source, expec
+0000c1a0: 7465 6420 3d20 7265 6164 5f64 6174 6128  ted = read_data(
+0000c1b0: 226d 6973 6365 6c6c 616e 656f 7573 222c  "miscellaneous",
+0000c1c0: 2022 666f 7263 655f 7079 3336 2229 0a20   "force_py36"). 
+0000c1d0: 2020 2020 2020 2077 6974 6820 6361 6368         with cach
+0000c1e0: 655f 6469 7228 2920 6173 2077 6f72 6b73  e_dir() as works
+0000c1f0: 7061 6365 3a0a 2020 2020 2020 2020 2020  pace:.          
+0000c200: 2020 7061 7468 203d 2028 776f 726b 7370    path = (worksp
+0000c210: 6163 6520 2f20 2266 696c 652e 7079 2229  ace / "file.py")
+0000c220: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+0000c230: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+0000c240: 2870 6174 682c 2022 7722 2920 6173 2066  (path, "w") as f
+0000c250: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+0000c260: 2020 2066 682e 7772 6974 6528 736f 7572     fh.write(sour
+0000c270: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
+0000c280: 7365 6c66 2e69 6e76 6f6b 6542 6c61 636b  self.invokeBlack
+0000c290: 285b 7374 7228 7061 7468 292c 202a 5059  ([str(path), *PY
+0000c2a0: 3336 5f41 5247 535d 290a 2020 2020 2020  36_ARGS]).      
+0000c2b0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0000c2c0: 7061 7468 2c20 2272 2229 2061 7320 6668  path, "r") as fh
+0000c2d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c2e0: 2020 6163 7475 616c 203d 2066 682e 7265    actual = fh.re
+0000c2f0: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+0000c300: 2023 2076 6572 6966 7920 6361 6368 6520   # verify cache 
+0000c310: 7769 7468 202d 2d74 6172 6765 742d 7665  with --target-ve
+0000c320: 7273 696f 6e20 6973 2073 6570 6172 6174  rsion is separat
+0000c330: 650a 2020 2020 2020 2020 2020 2020 7079  e.            py
+0000c340: 3336 5f63 6163 6865 203d 2070 7969 6e6b  36_cache = pyink
+0000c350: 2e72 6561 645f 6361 6368 6528 7079 3336  .read_cache(py36
+0000c360: 5f6d 6f64 6529 0a20 2020 2020 2020 2020  _mode).         
+0000c370: 2020 2073 656c 662e 6173 7365 7274 496e     self.assertIn
+0000c380: 2873 7472 2870 6174 6829 2c20 7079 3336  (str(path), py36
+0000c390: 5f63 6163 6865 290a 2020 2020 2020 2020  _cache).        
+0000c3a0: 2020 2020 6e6f 726d 616c 5f63 6163 6865      normal_cache
+0000c3b0: 203d 2070 7969 6e6b 2e72 6561 645f 6361   = pyink.read_ca
+0000c3c0: 6368 6528 7265 675f 6d6f 6465 290a 2020  che(reg_mode).  
+0000c3d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c3e0: 7373 6572 744e 6f74 496e 2873 7472 2870  ssertNotIn(str(p
+0000c3f0: 6174 6829 2c20 6e6f 726d 616c 5f63 6163  ath), normal_cac
+0000c400: 6865 290a 2020 2020 2020 2020 7365 6c66  he).        self
+0000c410: 2e61 7373 6572 7445 7175 616c 2861 6374  .assertEqual(act
+0000c420: 7561 6c2c 2065 7870 6563 7465 6429 0a0a  ual, expected)..
+0000c430: 2020 2020 4065 7665 6e74 5f6c 6f6f 7028      @event_loop(
+0000c440: 290a 2020 2020 6465 6620 7465 7374 5f6d  ).    def test_m
+0000c450: 756c 7469 5f66 696c 655f 666f 7263 655f  ulti_file_force_
+0000c460: 7079 3336 2873 656c 6629 202d 3e20 4e6f  py36(self) -> No
+0000c470: 6e65 3a0a 2020 2020 2020 2020 7265 675f  ne:.        reg_
+0000c480: 6d6f 6465 203d 2044 4546 4155 4c54 5f4d  mode = DEFAULT_M
+0000c490: 4f44 450a 2020 2020 2020 2020 7079 3336  ODE.        py36
+0000c4a0: 5f6d 6f64 6520 3d20 7265 706c 6163 6528  _mode = replace(
+0000c4b0: 4445 4641 554c 545f 4d4f 4445 2c20 7461  DEFAULT_MODE, ta
+0000c4c0: 7267 6574 5f76 6572 7369 6f6e 733d 5059  rget_versions=PY
+0000c4d0: 3336 5f56 4552 5349 4f4e 5329 0a20 2020  36_VERSIONS).   
+0000c4e0: 2020 2020 2073 6f75 7263 652c 2065 7870       source, exp
+0000c4f0: 6563 7465 6420 3d20 7265 6164 5f64 6174  ected = read_dat
+0000c500: 6128 226d 6973 6365 6c6c 616e 656f 7573  a("miscellaneous
+0000c510: 222c 2022 666f 7263 655f 7079 3336 2229  ", "force_py36")
+0000c520: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
+0000c530: 6368 655f 6469 7228 2920 6173 2077 6f72  che_dir() as wor
+0000c540: 6b73 7061 6365 3a0a 2020 2020 2020 2020  kspace:.        
+0000c550: 2020 2020 7061 7468 7320 3d20 5b0a 2020      paths = [.  
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2877                (w
+0000c570: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
+0000c580: 312e 7079 2229 2e72 6573 6f6c 7665 2829  1.py").resolve()
+0000c590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c5a0: 2020 2877 6f72 6b73 7061 6365 202f 2022    (workspace / "
+0000c5b0: 6669 6c65 322e 7079 2229 2e72 6573 6f6c  file2.py").resol
+0000c5c0: 7665 2829 2c0a 2020 2020 2020 2020 2020  ve(),.          
+0000c5d0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000c5e0: 666f 7220 7061 7468 2069 6e20 7061 7468  for path in path
+0000c5f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000c600: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
+0000c610: 682c 2022 7722 2920 6173 2066 683a 0a20  h, "w") as fh:. 
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c630: 2020 2066 682e 7772 6974 6528 736f 7572     fh.write(sour
+0000c640: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
+0000c650: 7365 6c66 2e69 6e76 6f6b 6542 6c61 636b  self.invokeBlack
+0000c660: 285b 7374 7228 7029 2066 6f72 2070 2069  ([str(p) for p i
+0000c670: 6e20 7061 7468 735d 202b 2050 5933 365f  n paths] + PY36_
+0000c680: 4152 4753 290a 2020 2020 2020 2020 2020  ARGS).          
+0000c690: 2020 666f 7220 7061 7468 2069 6e20 7061    for path in pa
+0000c6a0: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
+0000c6b0: 2020 2020 2077 6974 6820 6f70 656e 2870       with open(p
+0000c6c0: 6174 682c 2022 7222 2920 6173 2066 683a  ath, "r") as fh:
+0000c6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c6e0: 2020 2020 2061 6374 7561 6c20 3d20 6668       actual = fh
+0000c6f0: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
+0000c700: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000c710: 6572 7445 7175 616c 2861 6374 7561 6c2c  ertEqual(actual,
+0000c720: 2065 7870 6563 7465 6429 0a20 2020 2020   expected).     
+0000c730: 2020 2020 2020 2023 2076 6572 6966 7920         # verify 
+0000c740: 6361 6368 6520 7769 7468 202d 2d74 6172  cache with --tar
+0000c750: 6765 742d 7665 7273 696f 6e20 6973 2073  get-version is s
+0000c760: 6570 6172 6174 650a 2020 2020 2020 2020  eparate.        
+0000c770: 2020 2020 7079 695f 6361 6368 6520 3d20      pyi_cache = 
+0000c780: 7079 696e 6b2e 7265 6164 5f63 6163 6865  pyink.read_cache
+0000c790: 2870 7933 365f 6d6f 6465 290a 2020 2020  (py36_mode).    
+0000c7a0: 2020 2020 2020 2020 6e6f 726d 616c 5f63          normal_c
+0000c7b0: 6163 6865 203d 2070 7969 6e6b 2e72 6561  ache = pyink.rea
+0000c7c0: 645f 6361 6368 6528 7265 675f 6d6f 6465  d_cache(reg_mode
+0000c7d0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000c7e0: 7220 7061 7468 2069 6e20 7061 7468 733a  r path in paths:
+0000c7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c800: 2073 656c 662e 6173 7365 7274 496e 2873   self.assertIn(s
+0000c810: 7472 2870 6174 6829 2c20 7079 695f 6361  tr(path), pyi_ca
+0000c820: 6368 6529 0a20 2020 2020 2020 2020 2020  che).           
+0000c830: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c840: 4e6f 7449 6e28 7374 7228 7061 7468 292c  NotIn(str(path),
+0000c850: 206e 6f72 6d61 6c5f 6361 6368 6529 0a0a   normal_cache)..
+0000c860: 2020 2020 6465 6620 7465 7374 5f70 6970      def test_pip
+0000c870: 655f 666f 7263 655f 7079 3336 2873 656c  e_force_py36(sel
+0000c880: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000c890: 2020 2020 736f 7572 6365 2c20 6578 7065      source, expe
+0000c8a0: 6374 6564 203d 2072 6561 645f 6461 7461  cted = read_data
+0000c8b0: 2822 6d69 7363 656c 6c61 6e65 6f75 7322  ("miscellaneous"
+0000c8c0: 2c20 2266 6f72 6365 5f70 7933 3622 290a  , "force_py36").
+0000c8d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000c8e0: 2043 6c69 5275 6e6e 6572 2829 2e69 6e76   CliRunner().inv
+0000c8f0: 6f6b 6528 0a20 2020 2020 2020 2020 2020  oke(.           
+0000c900: 2070 7969 6e6b 2e6d 6169 6e2c 0a20 2020   pyink.main,.   
+0000c910: 2020 2020 2020 2020 205b 222d 222c 2022           ["-", "
+0000c920: 2d71 222c 2022 2d2d 7461 7267 6574 2d76  -q", "--target-v
+0000c930: 6572 7369 6f6e 3d70 7933 3622 5d2c 0a20  ersion=py36"],. 
+0000c940: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000c950: 3d42 7974 6573 494f 2873 6f75 7263 652e  =BytesIO(source.
+0000c960: 656e 636f 6465 2822 7574 6638 2229 292c  encode("utf8")),
+0000c970: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000c980: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000c990: 7561 6c28 7265 7375 6c74 2e65 7869 745f  ual(result.exit_
+0000c9a0: 636f 6465 2c20 3029 0a20 2020 2020 2020  code, 0).       
+0000c9b0: 2061 6374 7561 6c20 3d20 7265 7375 6c74   actual = result
+0000c9c0: 2e6f 7574 7075 740a 2020 2020 2020 2020  .output.        
+0000c9d0: 7365 6c66 2e61 7373 6572 7446 6f72 6d61  self.assertForma
+0000c9e0: 7445 7175 616c 2861 6374 7561 6c2c 2065  tEqual(actual, e
+0000c9f0: 7870 6563 7465 6429 0a0a 2020 2020 4070  xpected)..    @p
+0000ca00: 7974 6573 742e 6d61 726b 2e69 6e63 6f6d  ytest.mark.incom
+0000ca10: 7061 7469 626c 655f 7769 7468 5f6d 7970  patible_with_myp
+0000ca20: 7963 0a20 2020 2064 6566 2074 6573 745f  yc.    def test_
+0000ca30: 7265 666f 726d 6174 5f6f 6e65 5f77 6974  reformat_one_wit
+0000ca40: 685f 7374 6469 6e28 7365 6c66 2920 2d3e  h_stdin(self) ->
+0000ca50: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
+0000ca60: 6974 6820 7061 7463 6828 0a20 2020 2020  ith patch(.     
+0000ca70: 2020 2020 2020 2022 7079 696e 6b2e 666f         "pyink.fo
+0000ca80: 726d 6174 5f73 7464 696e 5f74 6f5f 7374  rmat_stdin_to_st
+0000ca90: 646f 7574 222c 0a20 2020 2020 2020 2020  dout",.         
+0000caa0: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
+0000cab0: 6c61 6d62 6461 202a 6172 6773 2c20 2a2a  lambda *args, **
+0000cac0: 6b77 6172 6773 3a20 7079 696e 6b2e 4368  kwargs: pyink.Ch
+0000cad0: 616e 6765 642e 5945 532c 0a20 2020 2020  anged.YES,.     
+0000cae0: 2020 2029 2061 7320 6673 7473 3a0a 2020     ) as fsts:.  
+0000caf0: 2020 2020 2020 2020 2020 7265 706f 7274            report
+0000cb00: 203d 204d 6167 6963 4d6f 636b 2829 0a20   = MagicMock(). 
+0000cb10: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+0000cb20: 3d20 5061 7468 2822 2d22 290a 2020 2020  = Path("-").    
+0000cb30: 2020 2020 2020 2020 7079 696e 6b2e 7265          pyink.re
+0000cb40: 666f 726d 6174 5f6f 6e65 280a 2020 2020  format_one(.    
+0000cb50: 2020 2020 2020 2020 2020 2020 7061 7468              path
+0000cb60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cb70: 2020 6661 7374 3d54 7275 652c 0a20 2020    fast=True,.   
+0000cb80: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+0000cb90: 7465 5f62 6163 6b3d 7079 696e 6b2e 5772  te_back=pyink.Wr
+0000cba0: 6974 6542 6163 6b2e 5945 532c 0a20 2020  iteBack.YES,.   
+0000cbb0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0000cbc0: 653d 4445 4641 554c 545f 4d4f 4445 2c0a  e=DEFAULT_MODE,.
+0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbe0: 7265 706f 7274 3d72 6570 6f72 742c 0a20  report=report,. 
+0000cbf0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000cc00: 2020 2020 2020 2020 2066 7374 732e 6173           fsts.as
+0000cc10: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+0000cc20: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+0000cc30: 6570 6f72 742e 646f 6e65 2e61 7373 6572  eport.done.asser
+0000cc40: 745f 6361 6c6c 6564 5f77 6974 6828 7061  t_called_with(pa
+0000cc50: 7468 2c20 7079 696e 6b2e 4368 616e 6765  th, pyink.Change
+0000cc60: 642e 5945 5329 0a0a 2020 2020 4070 7974  d.YES)..    @pyt
+0000cc70: 6573 742e 6d61 726b 2e69 6e63 6f6d 7061  est.mark.incompa
+0000cc80: 7469 626c 655f 7769 7468 5f6d 7970 7963  tible_with_mypyc
+0000cc90: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+0000cca0: 666f 726d 6174 5f6f 6e65 5f77 6974 685f  format_one_with_
+0000ccb0: 7374 6469 6e5f 6669 6c65 6e61 6d65 2873  stdin_filename(s
+0000ccc0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000ccd0: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
+0000cce0: 280a 2020 2020 2020 2020 2020 2020 2270  (.            "p
+0000ccf0: 7969 6e6b 2e66 6f72 6d61 745f 7374 6469  yink.format_stdi
+0000cd00: 6e5f 746f 5f73 7464 6f75 7422 2c0a 2020  n_to_stdout",.  
+0000cd10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000cd20: 5f76 616c 7565 3d6c 616d 6264 6120 2a61  _value=lambda *a
+0000cd30: 7267 732c 202a 2a6b 7761 7267 733a 2070  rgs, **kwargs: p
+0000cd40: 7969 6e6b 2e43 6861 6e67 6564 2e59 4553  yink.Changed.YES
+0000cd50: 2c0a 2020 2020 2020 2020 2920 6173 2066  ,.        ) as f
+0000cd60: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
+0000cd70: 2072 6570 6f72 7420 3d20 4d61 6769 634d   report = MagicM
+0000cd80: 6f63 6b28 290a 2020 2020 2020 2020 2020  ock().          
+0000cd90: 2020 7020 3d20 2266 6f6f 2e70 7922 0a20    p = "foo.py". 
+0000cda0: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+0000cdb0: 3d20 5061 7468 2866 225f 5f50 5949 4e4b  = Path(f"__PYINK
+0000cdc0: 5f53 5444 494e 5f46 494c 454e 414d 455f  _STDIN_FILENAME_
+0000cdd0: 5f7b 707d 2229 0a20 2020 2020 2020 2020  _{p}").         
+0000cde0: 2020 2065 7870 6563 7465 6420 3d20 5061     expected = Pa
+0000cdf0: 7468 2870 290a 2020 2020 2020 2020 2020  th(p).          
+0000ce00: 2020 7079 696e 6b2e 7265 666f 726d 6174    pyink.reformat
+0000ce10: 5f6f 6e65 280a 2020 2020 2020 2020 2020  _one(.          
+0000ce20: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
+0000ce30: 2020 2020 2020 2020 2020 2020 6661 7374              fast
+0000ce40: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000ce50: 2020 2020 2020 2077 7269 7465 5f62 6163         write_bac
+0000ce60: 6b3d 7079 696e 6b2e 5772 6974 6542 6163  k=pyink.WriteBac
+0000ce70: 6b2e 5945 532c 0a20 2020 2020 2020 2020  k.YES,.         
+0000ce80: 2020 2020 2020 206d 6f64 653d 4445 4641         mode=DEFA
+0000ce90: 554c 545f 4d4f 4445 2c0a 2020 2020 2020  ULT_MODE,.      
+0000cea0: 2020 2020 2020 2020 2020 7265 706f 7274            report
+0000ceb0: 3d72 6570 6f72 742c 0a20 2020 2020 2020  =report,.       
+0000cec0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000ced0: 2020 2066 7374 732e 6173 7365 7274 5f63     fsts.assert_c
+0000cee0: 616c 6c65 645f 6f6e 6365 5f77 6974 6828  alled_once_with(
+0000cef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf00: 2066 6173 743d 5472 7565 2c20 7772 6974   fast=True, writ
+0000cf10: 655f 6261 636b 3d70 7969 6e6b 2e57 7269  e_back=pyink.Wri
+0000cf20: 7465 4261 636b 2e59 4553 2c20 6d6f 6465  teBack.YES, mode
+0000cf30: 3d44 4546 4155 4c54 5f4d 4f44 452c 206c  =DEFAULT_MODE, l
+0000cf40: 696e 6573 3d4e 6f6e 650a 2020 2020 2020  ines=None.      
+0000cf50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000cf60: 2020 2020 2320 5f5f 5059 494e 4b5f 5354      # __PYINK_ST
+0000cf70: 4449 4e5f 4649 4c45 4e41 4d45 5f5f 2073  DIN_FILENAME__ s
+0000cf80: 686f 756c 6420 6861 7665 2062 6565 6e20  hould have been 
+0000cf90: 7374 7269 7070 6564 0a20 2020 2020 2020  stripped.       
+0000cfa0: 2020 2020 2072 6570 6f72 742e 646f 6e65       report.done
+0000cfb0: 2e61 7373 6572 745f 6361 6c6c 6564 5f77  .assert_called_w
+0000cfc0: 6974 6828 6578 7065 6374 6564 2c20 7079  ith(expected, py
+0000cfd0: 696e 6b2e 4368 616e 6765 642e 5945 5329  ink.Changed.YES)
+0000cfe0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0000cff0: 726b 2e69 6e63 6f6d 7061 7469 626c 655f  rk.incompatible_
+0000d000: 7769 7468 5f6d 7970 7963 0a20 2020 2064  with_mypyc.    d
+0000d010: 6566 2074 6573 745f 7265 666f 726d 6174  ef test_reformat
+0000d020: 5f6f 6e65 5f77 6974 685f 7374 6469 6e5f  _one_with_stdin_
+0000d030: 6669 6c65 6e61 6d65 5f70 7969 2873 656c  filename_pyi(sel
+0000d040: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000d050: 2020 2020 7769 7468 2070 6174 6368 280a      with patch(.
+0000d060: 2020 2020 2020 2020 2020 2020 2270 7969              "pyi
+0000d070: 6e6b 2e66 6f72 6d61 745f 7374 6469 6e5f  nk.format_stdin_
+0000d080: 746f 5f73 7464 6f75 7422 2c0a 2020 2020  to_stdout",.    
+0000d090: 2020 2020 2020 2020 7265 7475 726e 5f76          return_v
+0000d0a0: 616c 7565 3d6c 616d 6264 6120 2a61 7267  alue=lambda *arg
+0000d0b0: 732c 202a 2a6b 7761 7267 733a 2070 7969  s, **kwargs: pyi
+0000d0c0: 6e6b 2e43 6861 6e67 6564 2e59 4553 2c0a  nk.Changed.YES,.
+0000d0d0: 2020 2020 2020 2020 2920 6173 2066 7374          ) as fst
+0000d0e0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0000d0f0: 6570 6f72 7420 3d20 4d61 6769 634d 6f63  eport = MagicMoc
+0000d100: 6b28 290a 2020 2020 2020 2020 2020 2020  k().            
+0000d110: 7020 3d20 2266 6f6f 2e70 7969 220a 2020  p = "foo.pyi".  
+0000d120: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+0000d130: 2050 6174 6828 6622 5f5f 5059 494e 4b5f   Path(f"__PYINK_
+0000d140: 5354 4449 4e5f 4649 4c45 4e41 4d45 5f5f  STDIN_FILENAME__
+0000d150: 7b70 7d22 290a 2020 2020 2020 2020 2020  {p}").          
+0000d160: 2020 6578 7065 6374 6564 203d 2050 6174    expected = Pat
+0000d170: 6828 7029 0a20 2020 2020 2020 2020 2020  h(p).           
+0000d180: 2070 7969 6e6b 2e72 6566 6f72 6d61 745f   pyink.reformat_
+0000d190: 6f6e 6528 0a20 2020 2020 2020 2020 2020  one(.           
+0000d1a0: 2020 2020 2070 6174 682c 0a20 2020 2020       path,.     
+0000d1b0: 2020 2020 2020 2020 2020 2066 6173 743d             fast=
+0000d1c0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0000d1d0: 2020 2020 2020 7772 6974 655f 6261 636b        write_back
+0000d1e0: 3d70 7969 6e6b 2e57 7269 7465 4261 636b  =pyink.WriteBack
+0000d1f0: 2e59 4553 2c0a 2020 2020 2020 2020 2020  .YES,.          
+0000d200: 2020 2020 2020 6d6f 6465 3d44 4546 4155        mode=DEFAU
+0000d210: 4c54 5f4d 4f44 452c 0a20 2020 2020 2020  LT_MODE,.       
+0000d220: 2020 2020 2020 2020 2072 6570 6f72 743d           report=
+0000d230: 7265 706f 7274 2c0a 2020 2020 2020 2020  report,.        
+0000d240: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000d250: 2020 6673 7473 2e61 7373 6572 745f 6361    fsts.assert_ca
+0000d260: 6c6c 6564 5f6f 6e63 655f 7769 7468 280a  lled_once_with(.
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 6661 7374 3d54 7275 652c 0a20 2020 2020  fast=True,.     
+0000d290: 2020 2020 2020 2020 2020 2077 7269 7465             write
+0000d2a0: 5f62 6163 6b3d 7079 696e 6b2e 5772 6974  _back=pyink.Writ
+0000d2b0: 6542 6163 6b2e 5945 532c 0a20 2020 2020  eBack.YES,.     
+0000d2c0: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
+0000d2d0: 7265 706c 6163 6528 4445 4641 554c 545f  replace(DEFAULT_
+0000d2e0: 4d4f 4445 2c20 6973 5f70 7969 3d54 7275  MODE, is_pyi=Tru
+0000d2f0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000d300: 2020 2020 6c69 6e65 733d 4e6f 6e65 2c0a      lines=None,.
+0000d310: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000d320: 2020 2020 2020 2020 2020 2320 5f5f 5059            # __PY
+0000d330: 494e 4b5f 5354 4449 4e5f 4649 4c45 4e41  INK_STDIN_FILENA
+0000d340: 4d45 5f5f 2073 686f 756c 6420 6861 7665  ME__ should have
+0000d350: 2062 6565 6e20 7374 7269 7070 6564 0a20   been stripped. 
+0000d360: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+0000d370: 742e 646f 6e65 2e61 7373 6572 745f 6361  t.done.assert_ca
+0000d380: 6c6c 6564 5f77 6974 6828 6578 7065 6374  lled_with(expect
+0000d390: 6564 2c20 7079 696e 6b2e 4368 616e 6765  ed, pyink.Change
+0000d3a0: 642e 5945 5329 0a0a 2020 2020 4070 7974  d.YES)..    @pyt
+0000d3b0: 6573 742e 6d61 726b 2e69 6e63 6f6d 7061  est.mark.incompa
+0000d3c0: 7469 626c 655f 7769 7468 5f6d 7970 7963  tible_with_mypyc
+0000d3d0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+0000d3e0: 666f 726d 6174 5f6f 6e65 5f77 6974 685f  format_one_with_
+0000d3f0: 7374 6469 6e5f 6669 6c65 6e61 6d65 5f69  stdin_filename_i
+0000d400: 7079 6e62 2873 656c 6629 202d 3e20 4e6f  pynb(self) -> No
+0000d410: 6e65 3a0a 2020 2020 2020 2020 7769 7468  ne:.        with
+0000d420: 2070 6174 6368 280a 2020 2020 2020 2020   patch(.        
+0000d430: 2020 2020 2270 7969 6e6b 2e66 6f72 6d61      "pyink.forma
+0000d440: 745f 7374 6469 6e5f 746f 5f73 7464 6f75  t_stdin_to_stdou
+0000d450: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+0000d460: 7265 7475 726e 5f76 616c 7565 3d6c 616d  return_value=lam
+0000d470: 6264 6120 2a61 7267 732c 202a 2a6b 7761  bda *args, **kwa
+0000d480: 7267 733a 2070 7969 6e6b 2e43 6861 6e67  rgs: pyink.Chang
+0000d490: 6564 2e59 4553 2c0a 2020 2020 2020 2020  ed.YES,.        
+0000d4a0: 2920 6173 2066 7374 733a 0a20 2020 2020  ) as fsts:.     
+0000d4b0: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
+0000d4c0: 4d61 6769 634d 6f63 6b28 290a 2020 2020  MagicMock().    
+0000d4d0: 2020 2020 2020 2020 7020 3d20 2266 6f6f          p = "foo
+0000d4e0: 2e69 7079 6e62 220a 2020 2020 2020 2020  .ipynb".        
+0000d4f0: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
+0000d500: 6622 5f5f 5059 494e 4b5f 5354 4449 4e5f  f"__PYINK_STDIN_
+0000d510: 4649 4c45 4e41 4d45 5f5f 7b70 7d22 290a  FILENAME__{p}").
+0000d520: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+0000d530: 6374 6564 203d 2050 6174 6828 7029 0a20  cted = Path(p). 
+0000d540: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
+0000d550: 2e72 6566 6f72 6d61 745f 6f6e 6528 0a20  .reformat_one(. 
+0000d560: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d570: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000d580: 2020 2020 2066 6173 743d 5472 7565 2c0a       fast=True,.
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 7772 6974 655f 6261 636b 3d70 7969 6e6b  write_back=pyink
+0000d5b0: 2e57 7269 7465 4261 636b 2e59 4553 2c0a  .WriteBack.YES,.
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5d0: 6d6f 6465 3d44 4546 4155 4c54 5f4d 4f44  mode=DEFAULT_MOD
+0000d5e0: 452c 0a20 2020 2020 2020 2020 2020 2020  E,.             
+0000d5f0: 2020 2072 6570 6f72 743d 7265 706f 7274     report=report
+0000d600: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000d610: 2020 2020 2020 2020 2020 2020 6673 7473              fsts
+0000d620: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
+0000d630: 6e63 655f 7769 7468 280a 2020 2020 2020  nce_with(.      
+0000d640: 2020 2020 2020 2020 2020 6661 7374 3d54            fast=T
+0000d650: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000d660: 2020 2020 2077 7269 7465 5f62 6163 6b3d       write_back=
+0000d670: 7079 696e 6b2e 5772 6974 6542 6163 6b2e  pyink.WriteBack.
+0000d680: 5945 532c 0a20 2020 2020 2020 2020 2020  YES,.           
+0000d690: 2020 2020 206d 6f64 653d 7265 706c 6163       mode=replac
+0000d6a0: 6528 4445 4641 554c 545f 4d4f 4445 2c20  e(DEFAULT_MODE, 
+0000d6b0: 6973 5f69 7079 6e62 3d54 7275 6529 2c0a  is_ipynb=True),.
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 6c69 6e65 733d 4e6f 6e65 2c0a 2020 2020  lines=None,.    
+0000d6e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d6f0: 2020 2020 2020 2320 5f5f 5059 494e 4b5f        # __PYINK_
+0000d700: 5354 4449 4e5f 4649 4c45 4e41 4d45 5f5f  STDIN_FILENAME__
+0000d710: 2073 686f 756c 6420 6861 7665 2062 6565   should have bee
+0000d720: 6e20 7374 7269 7070 6564 0a20 2020 2020  n stripped.     
+0000d730: 2020 2020 2020 2072 6570 6f72 742e 646f         report.do
+0000d740: 6e65 2e61 7373 6572 745f 6361 6c6c 6564  ne.assert_called
+0000d750: 5f77 6974 6828 6578 7065 6374 6564 2c20  _with(expected, 
+0000d760: 7079 696e 6b2e 4368 616e 6765 642e 5945  pyink.Changed.YE
+0000d770: 5329 0a0a 2020 2020 4070 7974 6573 742e  S)..    @pytest.
+0000d780: 6d61 726b 2e69 6e63 6f6d 7061 7469 626c  mark.incompatibl
+0000d790: 655f 7769 7468 5f6d 7970 7963 0a20 2020  e_with_mypyc.   
+0000d7a0: 2064 6566 2074 6573 745f 7265 666f 726d   def test_reform
+0000d7b0: 6174 5f6f 6e65 5f77 6974 685f 7374 6469  at_one_with_stdi
+0000d7c0: 6e5f 616e 645f 6578 6973 7469 6e67 5f70  n_and_existing_p
+0000d7d0: 6174 6828 7365 6c66 2920 2d3e 204e 6f6e  ath(self) -> Non
+0000d7e0: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
+0000d7f0: 7061 7463 6828 0a20 2020 2020 2020 2020  patch(.         
+0000d800: 2020 2022 7079 696e 6b2e 666f 726d 6174     "pyink.format
+0000d810: 5f73 7464 696e 5f74 6f5f 7374 646f 7574  _stdin_to_stdout
+0000d820: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
+0000d830: 6574 7572 6e5f 7661 6c75 653d 6c61 6d62  eturn_value=lamb
+0000d840: 6461 202a 6172 6773 2c20 2a2a 6b77 6172  da *args, **kwar
+0000d850: 6773 3a20 7079 696e 6b2e 4368 616e 6765  gs: pyink.Change
+0000d860: 642e 5945 532c 0a20 2020 2020 2020 2029  d.YES,.        )
+0000d870: 2061 7320 6673 7473 3a0a 2020 2020 2020   as fsts:.      
+0000d880: 2020 2020 2020 7265 706f 7274 203d 204d        report = M
+0000d890: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
+0000d8a0: 2020 2020 2020 2023 2045 7665 6e20 7769         # Even wi
+0000d8b0: 7468 2061 6e20 6578 6973 7469 6e67 2066  th an existing f
+0000d8c0: 696c 652c 2073 696e 6365 2077 6520 6172  ile, since we ar
+0000d8d0: 6520 666f 7263 696e 6720 7374 6469 6e2c  e forcing stdin,
+0000d8e0: 2062 6c61 636b 0a20 2020 2020 2020 2020   black.         
+0000d8f0: 2020 2023 2073 686f 756c 6420 6f75 7470     # should outp
+0000d900: 7574 2074 6f20 7374 646f 7574 2061 6e64  ut to stdout and
+0000d910: 206e 6f74 206d 6f64 6966 7920 7468 6520   not modify the 
+0000d920: 6669 6c65 2069 6e70 6c61 6365 0a20 2020  file inplace.   
+0000d930: 2020 2020 2020 2020 2070 203d 2054 4849           p = THI
+0000d940: 535f 4449 5220 2f20 2264 6174 6122 202f  S_DIR / "data" /
+0000d950: 2022 7369 6d70 6c65 5f63 6173 6573 2220   "simple_cases" 
+0000d960: 2f20 2263 6f6c 6c65 6374 696f 6e73 2e70  / "collections.p
+0000d970: 7922 0a20 2020 2020 2020 2020 2020 2023  y".            #
+0000d980: 204d 616b 6520 7375 7265 2069 735f 6669   Make sure is_fi
+0000d990: 6c65 2061 6374 7561 6c6c 7920 7265 7475  le actually retu
+0000d9a0: 726e 7320 5472 7565 0a20 2020 2020 2020  rns True.       
+0000d9b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000d9c0: 5472 7565 2870 2e69 735f 6669 6c65 2829  True(p.is_file()
+0000d9d0: 290a 2020 2020 2020 2020 2020 2020 7061  ).            pa
+0000d9e0: 7468 203d 2050 6174 6828 6622 5f5f 5059  th = Path(f"__PY
+0000d9f0: 494e 4b5f 5354 4449 4e5f 4649 4c45 4e41  INK_STDIN_FILENA
+0000da00: 4d45 5f5f 7b70 7d22 290a 2020 2020 2020  ME__{p}").      
+0000da10: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+0000da20: 2050 6174 6828 7029 0a20 2020 2020 2020   Path(p).       
+0000da30: 2020 2020 2070 7969 6e6b 2e72 6566 6f72       pyink.refor
+0000da40: 6d61 745f 6f6e 6528 0a20 2020 2020 2020  mat_one(.       
+0000da50: 2020 2020 2020 2020 2070 6174 682c 0a20           path,. 
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000da70: 6173 743d 5472 7565 2c0a 2020 2020 2020  ast=True,.      
+0000da80: 2020 2020 2020 2020 2020 7772 6974 655f            write_
+0000da90: 6261 636b 3d70 7969 6e6b 2e57 7269 7465  back=pyink.Write
+0000daa0: 4261 636b 2e59 4553 2c0a 2020 2020 2020  Back.YES,.      
+0000dab0: 2020 2020 2020 2020 2020 6d6f 6465 3d44            mode=D
+0000dac0: 4546 4155 4c54 5f4d 4f44 452c 0a20 2020  EFAULT_MODE,.   
+0000dad0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+0000dae0: 6f72 743d 7265 706f 7274 2c0a 2020 2020  ort=report,.    
+0000daf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000db00: 2020 2020 2020 6673 7473 2e61 7373 6572        fsts.asser
+0000db10: 745f 6361 6c6c 6564 5f6f 6e63 6528 290a  t_called_once().
+0000db20: 2020 2020 2020 2020 2020 2020 2320 5f5f              # __
+0000db30: 5059 494e 4b5f 5354 4449 4e5f 4649 4c45  PYINK_STDIN_FILE
+0000db40: 4e41 4d45 5f5f 2073 686f 756c 6420 6861  NAME__ should ha
+0000db50: 7665 2062 6565 6e20 7374 7269 7070 6564  ve been stripped
+0000db60: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+0000db70: 6f72 742e 646f 6e65 2e61 7373 6572 745f  ort.done.assert_
+0000db80: 6361 6c6c 6564 5f77 6974 6828 6578 7065  called_with(expe
+0000db90: 6374 6564 2c20 7079 696e 6b2e 4368 616e  cted, pyink.Chan
+0000dba0: 6765 642e 5945 5329 0a0a 2020 2020 6465  ged.YES)..    de
+0000dbb0: 6620 7465 7374 5f72 6566 6f72 6d61 745f  f test_reformat_
+0000dbc0: 6f6e 655f 7769 7468 5f73 7464 696e 5f65  one_with_stdin_e
+0000dbd0: 6d70 7479 2873 656c 6629 202d 3e20 4e6f  mpty(self) -> No
+0000dbe0: 6e65 3a0a 2020 2020 2020 2020 6361 7365  ne:.        case
+0000dbf0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+0000dc00: 2020 2822 222c 2022 2229 2c0a 2020 2020    ("", ""),.    
+0000dc10: 2020 2020 2020 2020 2822 5c6e 222c 2022          ("\n", "
+0000dc20: 5c6e 2229 2c0a 2020 2020 2020 2020 2020  \n"),.          
+0000dc30: 2020 2822 5c72 5c6e 222c 2022 5c72 5c6e    ("\r\n", "\r\n
+0000dc40: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0000dc50: 2822 205c 7422 2c20 2222 292c 0a20 2020  (" \t", ""),.   
+0000dc60: 2020 2020 2020 2020 2028 2220 5c74 5c6e           (" \t\n
+0000dc70: 5c74 2022 2c20 225c 6e22 292c 0a20 2020  \t ", "\n"),.   
+0000dc80: 2020 2020 2020 2020 2028 2220 5c74 5c72           (" \t\r
+0000dc90: 5c6e 5c74 2022 2c20 225c 725c 6e22 292c  \n\t ", "\r\n"),
+0000dca0: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+0000dcb0: 2020 2020 6465 6620 5f6e 6577 5f77 7261      def _new_wra
+0000dcc0: 7070 6572 280a 2020 2020 2020 2020 2020  pper(.          
+0000dcd0: 2020 6f75 7470 7574 3a20 696f 2e53 7472    output: io.Str
+0000dce0: 696e 6749 4f2c 2069 6f5f 5465 7874 494f  ingIO, io_TextIO
+0000dcf0: 5772 6170 7065 723a 2054 7970 655b 696f  Wrapper: Type[io
+0000dd00: 2e54 6578 7449 4f57 7261 7070 6572 5d0a  .TextIOWrapper].
+0000dd10: 2020 2020 2020 2020 2920 2d3e 2043 616c          ) -> Cal
+0000dd20: 6c61 626c 655b 5b41 6e79 2c20 416e 795d  lable[[Any, Any]
+0000dd30: 2c20 696f 2e54 6578 7449 4f57 7261 7070  , io.TextIOWrapp
+0000dd40: 6572 5d3a 0a20 2020 2020 2020 2020 2020  er]:.           
+0000dd50: 2064 6566 2067 6574 5f6f 7574 7075 7428   def get_output(
+0000dd60: 2a61 7267 733a 2041 6e79 2c20 2a2a 6b77  *args: Any, **kw
+0000dd70: 6172 6773 3a20 416e 7929 202d 3e20 696f  args: Any) -> io
+0000dd80: 2e54 6578 7449 4f57 7261 7070 6572 3a0a  .TextIOWrapper:.
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 6966 2061 7267 7320 3d3d 2028 7379 732e  if args == (sys.
+0000ddb0: 7374 646f 7574 2e62 7566 6665 722c 293a  stdout.buffer,):
+0000ddc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ddd0: 2020 2020 2023 2049 7427 7320 6066 6f72       # It's `for
+0000dde0: 6d61 745f 7374 6469 6e5f 746f 5f73 7464  mat_stdin_to_std
+0000ddf0: 6f75 7428 2960 2063 616c 6c69 6e67 2060  out()` calling `
+0000de00: 696f 2e54 6578 7449 4f57 7261 7070 6572  io.TextIOWrapper
+0000de10: 2829 602c 0a20 2020 2020 2020 2020 2020  ()`,.           
+0000de20: 2020 2020 2020 2020 2023 2072 6574 7572           # retur
+0000de30: 6e20 6f75 7220 6d6f 636b 206f 626a 6563  n our mock objec
+0000de40: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000de50: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
+0000de60: 7470 7574 0a20 2020 2020 2020 2020 2020  tput.           
+0000de70: 2020 2020 2023 2049 7427 7320 736f 6d65       # It's some
+0000de80: 7468 696e 6720 656c 7365 2028 692e 652e  thing else (i.e.
+0000de90: 2060 6465 636f 6465 5f62 7974 6573 2829   `decode_bytes()
+0000dea0: 6029 2063 616c 6c69 6e67 0a20 2020 2020  `) calling.     
+0000deb0: 2020 2020 2020 2020 2020 2023 2060 696f             # `io
+0000dec0: 2e54 6578 7449 4f57 7261 7070 6572 2829  .TextIOWrapper()
+0000ded0: 602c 2070 6173 7320 7468 726f 7567 6820  `, pass through 
+0000dee0: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+0000def0: 696d 706c 656d 656e 7461 7469 6f6e 2e0a  implementation..
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df10: 2320 5365 6520 6469 7363 7573 7369 6f6e  # See discussion
+0000df20: 2069 6e20 6874 7470 733a 2f2f 6769 7468   in https://gith
+0000df30: 7562 2e63 6f6d 2f70 7366 2f62 6c61 636b  ub.com/psf/black
+0000df40: 2f70 756c 6c2f 3234 3839 0a20 2020 2020  /pull/2489.     
+0000df50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000df60: 6e20 696f 5f54 6578 7449 4f57 7261 7070  n io_TextIOWrapp
+0000df70: 6572 282a 6172 6773 2c20 2a2a 6b77 6172  er(*args, **kwar
+0000df80: 6773 290a 0a20 2020 2020 2020 2020 2020  gs)..           
+0000df90: 2072 6574 7572 6e20 6765 745f 6f75 7470   return get_outp
+0000dfa0: 7574 0a0a 2020 2020 2020 2020 6d6f 6465  ut..        mode
+0000dfb0: 203d 2070 7969 6e6b 2e4d 6f64 6528 7072   = pyink.Mode(pr
+0000dfc0: 6576 6965 773d 5472 7565 290a 2020 2020  eview=True).    
+0000dfd0: 2020 2020 666f 7220 636f 6e74 656e 742c      for content,
+0000dfe0: 2065 7870 6563 7465 6420 696e 2063 6173   expected in cas
+0000dff0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000e000: 6f75 7470 7574 203d 2069 6f2e 5374 7269  output = io.Stri
+0000e010: 6e67 494f 2829 0a20 2020 2020 2020 2020  ngIO().         
+0000e020: 2020 2069 6f5f 5465 7874 494f 5772 6170     io_TextIOWrap
+0000e030: 7065 7220 3d20 696f 2e54 6578 7449 4f57  per = io.TextIOW
+0000e040: 7261 7070 6572 0a0a 2020 2020 2020 2020  rapper..        
+0000e050: 2020 2020 7769 7468 2070 6174 6368 2822      with patch("
+0000e060: 696f 2e54 6578 7449 4f57 7261 7070 6572  io.TextIOWrapper
+0000e070: 222c 205f 6e65 775f 7772 6170 7065 7228  ", _new_wrapper(
+0000e080: 6f75 7470 7574 2c20 696f 5f54 6578 7449  output, io_TextI
+0000e090: 4f57 7261 7070 6572 2929 3a0a 2020 2020  OWrapper)):.    
+0000e0a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000e0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e0c0: 2020 2020 2070 7969 6e6b 2e66 6f72 6d61       pyink.forma
+0000e0d0: 745f 7374 6469 6e5f 746f 5f73 7464 6f75  t_stdin_to_stdou
+0000e0e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000e0f0: 2020 2020 2020 2020 2020 2066 6173 743d             fast=
+0000e100: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0000e110: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000e120: 6e74 656e 743d 636f 6e74 656e 742c 0a20  ntent=content,. 
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e140: 2020 2020 2020 2077 7269 7465 5f62 6163         write_bac
+0000e150: 6b3d 7079 696e 6b2e 5772 6974 6542 6163  k=pyink.WriteBac
+0000e160: 6b2e 5945 532c 0a20 2020 2020 2020 2020  k.YES,.         
+0000e170: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000e180: 6f64 653d 6d6f 6465 2c0a 2020 2020 2020  ode=mode,.      
+0000e190: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1b0: 6578 6365 7074 2069 6f2e 556e 7375 7070  except io.Unsupp
+0000e1c0: 6f72 7465 644f 7065 7261 7469 6f6e 3a0a  ortedOperation:.
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1e0: 2020 2020 7061 7373 2020 2320 5374 7269      pass  # Stri
+0000e1f0: 6e67 494f 2064 6f65 7320 6e6f 7420 7375  ngIO does not su
+0000e200: 7070 6f72 7420 6465 7461 6368 0a20 2020  pport detach.   
+0000e210: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+0000e220: 6572 7420 6f75 7470 7574 2e67 6574 7661  ert output.getva
+0000e230: 6c75 6528 2920 3d3d 2065 7870 6563 7465  lue() == expecte
+0000e240: 640a 0a20 2020 2020 2020 2023 2041 6e20  d..        # An 
+0000e250: 656d 7074 7920 7374 7269 6e67 2069 7320  empty string is 
+0000e260: 7468 6520 6f6e 6c79 2074 6573 7420 6361  the only test ca
+0000e270: 7365 2066 6f72 2060 7072 6576 6965 773d  se for `preview=
+0000e280: 4661 6c73 6560 0a20 2020 2020 2020 206f  False`.        o
+0000e290: 7574 7075 7420 3d20 696f 2e53 7472 696e  utput = io.Strin
+0000e2a0: 6749 4f28 290a 2020 2020 2020 2020 696f  gIO().        io
+0000e2b0: 5f54 6578 7449 4f57 7261 7070 6572 203d  _TextIOWrapper =
+0000e2c0: 2069 6f2e 5465 7874 494f 5772 6170 7065   io.TextIOWrappe
+0000e2d0: 720a 2020 2020 2020 2020 7769 7468 2070  r.        with p
+0000e2e0: 6174 6368 2822 696f 2e54 6578 7449 4f57  atch("io.TextIOW
+0000e2f0: 7261 7070 6572 222c 205f 6e65 775f 7772  rapper", _new_wr
+0000e300: 6170 7065 7228 6f75 7470 7574 2c20 696f  apper(output, io
+0000e310: 5f54 6578 7449 4f57 7261 7070 6572 2929  _TextIOWrapper))
+0000e320: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+0000e330: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000e340: 2020 2070 7969 6e6b 2e66 6f72 6d61 745f     pyink.format_
+0000e350: 7374 6469 6e5f 746f 5f73 7464 6f75 7428  stdin_to_stdout(
+0000e360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e370: 2020 2020 2066 6173 743d 5472 7565 2c0a       fast=True,.
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 2020 2020 636f 6e74 656e 743d 2222 2c0a      content="",.
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3b0: 2020 2020 7772 6974 655f 6261 636b 3d70      write_back=p
+0000e3c0: 7969 6e6b 2e57 7269 7465 4261 636b 2e59  yink.WriteBack.Y
+0000e3d0: 4553 2c0a 2020 2020 2020 2020 2020 2020  ES,.            
+0000e3e0: 2020 2020 2020 2020 6d6f 6465 3d44 4546          mode=DEF
+0000e3f0: 4155 4c54 5f4d 4f44 452c 0a20 2020 2020  AULT_MODE,.     
+0000e400: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000e410: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0000e420: 696f 2e55 6e73 7570 706f 7274 6564 4f70  io.UnsupportedOp
+0000e430: 6572 6174 696f 6e3a 0a20 2020 2020 2020  eration:.       
+0000e440: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
+0000e450: 2053 7472 696e 6749 4f20 646f 6573 206e   StringIO does n
+0000e460: 6f74 2073 7570 706f 7274 2064 6574 6163  ot support detac
+0000e470: 680a 2020 2020 2020 2020 2020 2020 6173  h.            as
+0000e480: 7365 7274 206f 7574 7075 742e 6765 7476  sert output.getv
+0000e490: 616c 7565 2829 203d 3d20 2222 0a0a 2020  alue() == ""..  
+0000e4a0: 2020 6465 6620 7465 7374 5f66 6f72 6d61    def test_forma
+0000e4b0: 745f 7374 6469 6e5f 746f 5f73 7464 6f75  t_stdin_to_stdou
+0000e4c0: 745f 7769 7468 5f6c 696e 6573 2873 656c  t_with_lines(sel
+0000e4d0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000e4e0: 2020 2020 636f 6e74 656e 7473 203d 2022      contents = "
+0000e4f0: 2222 5c0a 6465 6620 6675 6e63 3128 293a  ""\.def func1():
+0000e500: 2070 6173 730a 6465 6620 6675 6e63 3228   pass.def func2(
+0000e510: 293a 2070 6173 730a 2222 220a 2020 2020  ): pass.""".    
+0000e520: 2020 2020 666f 726d 6174 7465 6420 3d20      formatted = 
+0000e530: 2222 225c 0a64 6566 2066 756e 6331 2829  """\.def func1()
+0000e540: 3a0a 2020 2020 7061 7373 0a0a 0a64 6566  :.    pass...def
+0000e550: 2066 756e 6332 2829 3a20 7061 7373 0a22   func2(): pass."
+0000e560: 2222 0a20 2020 2020 2020 2072 756e 6e65  "".        runne
+0000e570: 7220 3d20 426c 6163 6b52 756e 6e65 7228  r = BlackRunner(
+0000e580: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+0000e590: 203d 2072 756e 6e65 722e 696e 766f 6b65   = runner.invoke
+0000e5a0: 280a 2020 2020 2020 2020 2020 2020 7079  (.            py
+0000e5b0: 696e 6b2e 6d61 696e 2c0a 2020 2020 2020  ink.main,.      
+0000e5c0: 2020 2020 2020 5b22 2d22 2c20 222d 2d66        ["-", "--f
+0000e5d0: 6173 7422 2c20 222d 2d70 7969 6e6b 2d6c  ast", "--pyink-l
+0000e5e0: 696e 6573 3d31 2d31 225d 2c0a 2020 2020  ines=1-1"],.    
+0000e5f0: 2020 2020 2020 2020 696e 7075 743d 4279          input=By
+0000e600: 7465 7349 4f28 636f 6e74 656e 7473 2e65  tesIO(contents.e
+0000e610: 6e63 6f64 6528 2275 7466 3822 2929 2c0a  ncode("utf8")),.
+0000e620: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e630: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000e640: 616c 2872 6573 756c 742e 6578 6974 5f63  al(result.exit_c
+0000e650: 6f64 652c 2030 290a 2020 2020 2020 2020  ode, 0).        
+0000e660: 6f75 7470 7574 203d 2072 6573 756c 742e  output = result.
+0000e670: 7374 646f 7574 5f62 7974 6573 2e64 6563  stdout_bytes.dec
+0000e680: 6f64 6528 2275 7466 3822 290a 2020 2020  ode("utf8").    
+0000e690: 2020 2020 6173 7365 7274 206f 7574 7075      assert outpu
+0000e6a0: 7420 3d3d 2066 6f72 6d61 7474 6564 0a0a  t == formatted..
+0000e6b0: 2020 2020 6465 6620 7465 7374 5f69 6e76      def test_inv
+0000e6c0: 616c 6964 5f63 6c69 5f72 6567 6578 2873  alid_cli_regex(s
+0000e6d0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000e6e0: 2020 2020 2020 666f 7220 6f70 7469 6f6e        for option
+0000e6f0: 2069 6e20 5b22 2d2d 696e 636c 7564 6522   in ["--include"
+0000e700: 2c20 222d 2d65 7863 6c75 6465 222c 2022  , "--exclude", "
+0000e710: 2d2d 6578 7465 6e64 2d65 7863 6c75 6465  --extend-exclude
+0000e720: 222c 2022 2d2d 666f 7263 652d 6578 636c  ", "--force-excl
+0000e730: 7564 6522 5d3a 0a20 2020 2020 2020 2020  ude"]:.         
+0000e740: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
+0000e750: 6163 6b28 5b22 2d22 2c20 6f70 7469 6f6e  ack(["-", option
+0000e760: 2c20 222a 2a28 2928 2121 2a29 225d 2c20  , "**()(!!*)"], 
+0000e770: 6578 6974 5f63 6f64 653d 3229 0a0a 2020  exit_code=2)..  
+0000e780: 2020 6465 6620 7465 7374 5f72 6571 7569    def test_requi
+0000e790: 7265 645f 7665 7273 696f 6e5f 6d61 7463  red_version_matc
+0000e7a0: 6865 735f 7665 7273 696f 6e28 7365 6c66  hes_version(self
+0000e7b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000e7c0: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
+0000e7d0: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
+0000e7e0: 205b 222d 2d72 6571 7569 7265 642d 7665   ["--required-ve
+0000e7f0: 7273 696f 6e22 2c20 7079 696e 6b2e 5f5f  rsion", pyink.__
+0000e800: 7665 7273 696f 6e5f 5f2c 2022 2d63 222c  version__, "-c",
+0000e810: 2022 3022 5d2c 0a20 2020 2020 2020 2020   "0"],.         
+0000e820: 2020 2065 7869 745f 636f 6465 3d30 2c0a     exit_code=0,.
+0000e830: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
+0000e840: 7265 5f63 6f6e 6669 673d 5472 7565 2c0a  re_config=True,.
+0000e850: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000e860: 6566 2074 6573 745f 7265 7175 6972 6564  ef test_required
+0000e870: 5f76 6572 7369 6f6e 5f6d 6174 6368 6573  _version_matches
+0000e880: 5f70 6172 7469 616c 5f76 6572 7369 6f6e  _partial_version
+0000e890: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000e8a0: 2020 2020 2020 2020 7365 6c66 2e69 6e76          self.inv
+0000e8b0: 6f6b 6542 6c61 636b 280a 2020 2020 2020  okeBlack(.      
+0000e8c0: 2020 2020 2020 5b22 2d2d 7265 7175 6972        ["--requir
+0000e8d0: 6564 2d76 6572 7369 6f6e 222c 2070 7969  ed-version", pyi
+0000e8e0: 6e6b 2e5f 5f76 6572 7369 6f6e 5f5f 2e73  nk.__version__.s
+0000e8f0: 706c 6974 2822 2e22 295b 305d 2c20 222d  plit(".")[0], "-
+0000e900: 6322 2c20 2230 225d 2c0a 2020 2020 2020  c", "0"],.      
+0000e910: 2020 2020 2020 6578 6974 5f63 6f64 653d        exit_code=
+0000e920: 302c 0a20 2020 2020 2020 2020 2020 2069  0,.            i
+0000e930: 676e 6f72 655f 636f 6e66 6967 3d54 7275  gnore_config=Tru
+0000e940: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+0000e950: 2020 6465 6620 7465 7374 5f72 6571 7569    def test_requi
+0000e960: 7265 645f 7665 7273 696f 6e5f 646f 6573  red_version_does
+0000e970: 5f6e 6f74 5f6d 6174 6368 5f6f 6e5f 6d69  _not_match_on_mi
+0000e980: 6e6f 725f 7665 7273 696f 6e28 7365 6c66  nor_version(self
+0000e990: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000e9a0: 2020 2073 656c 662e 696e 766f 6b65 426c     self.invokeBl
+0000e9b0: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
+0000e9c0: 205b 222d 2d72 6571 7569 7265 642d 7665   ["--required-ve
+0000e9d0: 7273 696f 6e22 2c20 7079 696e 6b2e 5f5f  rsion", pyink.__
+0000e9e0: 7665 7273 696f 6e5f 5f2e 7370 6c69 7428  version__.split(
+0000e9f0: 222e 2229 5b30 5d20 2b20 222e 3939 3922  ".")[0] + ".999"
+0000ea00: 2c20 222d 6322 2c20 2230 225d 2c0a 2020  , "-c", "0"],.  
+0000ea10: 2020 2020 2020 2020 2020 6578 6974 5f63            exit_c
+0000ea20: 6f64 653d 312c 0a20 2020 2020 2020 2020  ode=1,.         
+0000ea30: 2020 2069 676e 6f72 655f 636f 6e66 6967     ignore_config
+0000ea40: 3d54 7275 652c 0a20 2020 2020 2020 2029  =True,.        )
+0000ea50: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
+0000ea60: 6571 7569 7265 645f 7665 7273 696f 6e5f  equired_version_
+0000ea70: 646f 6573 5f6e 6f74 5f6d 6174 6368 5f76  does_not_match_v
+0000ea80: 6572 7369 6f6e 2873 656c 6629 202d 3e20  ersion(self) -> 
+0000ea90: 4e6f 6e65 3a0a 2020 2020 2020 2020 7265  None:.        re
+0000eaa0: 7375 6c74 203d 2042 6c61 636b 5275 6e6e  sult = BlackRunn
+0000eab0: 6572 2829 2e69 6e76 6f6b 6528 0a20 2020  er().invoke(.   
+0000eac0: 2020 2020 2020 2020 2070 7969 6e6b 2e6d           pyink.m
+0000ead0: 6169 6e2c 0a20 2020 2020 2020 2020 2020  ain,.           
+0000eae0: 205b 222d 2d72 6571 7569 7265 642d 7665   ["--required-ve
+0000eaf0: 7273 696f 6e22 2c20 2232 302e 3939 6222  rsion", "20.99b"
+0000eb00: 2c20 222d 6322 2c20 2230 225d 2c0a 2020  , "-c", "0"],.  
+0000eb10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000eb20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000eb30: 2872 6573 756c 742e 6578 6974 5f63 6f64  (result.exit_cod
+0000eb40: 652c 2031 290a 2020 2020 2020 2020 7365  e, 1).        se
+0000eb50: 6c66 2e61 7373 6572 7449 6e28 2272 6571  lf.assertIn("req
+0000eb60: 7569 7265 6420 7665 7273 696f 6e22 2c20  uired version", 
+0000eb70: 7265 7375 6c74 2e73 7464 6572 7229 0a0a  result.stderr)..
+0000eb80: 2020 2020 6465 6620 7465 7374 5f70 7265      def test_pre
+0000eb90: 7365 7276 6573 5f6c 696e 655f 656e 6469  serves_line_endi
+0000eba0: 6e67 7328 7365 6c66 2920 2d3e 204e 6f6e  ngs(self) -> Non
+0000ebb0: 653a 0a20 2020 2020 2020 2077 6974 6820  e:.        with 
+0000ebc0: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+0000ebd0: 7279 2829 2061 7320 776f 726b 7370 6163  ry() as workspac
+0000ebe0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0000ebf0: 6573 745f 6669 6c65 203d 2050 6174 6828  est_file = Path(
+0000ec00: 776f 726b 7370 6163 6529 202f 2022 7465  workspace) / "te
+0000ec10: 7374 2e70 7922 0a20 2020 2020 2020 2020  st.py".         
+0000ec20: 2020 2066 6f72 206e 6c20 696e 205b 225c     for nl in ["\
+0000ec30: 6e22 2c20 225c 725c 6e22 5d3a 0a20 2020  n", "\r\n"]:.   
+0000ec40: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000ec50: 7465 6e74 7320 3d20 6e6c 2e6a 6f69 6e28  tents = nl.join(
+0000ec60: 5b22 6465 6620 6628 2020 293a 222c 2022  ["def f(  ):", "
+0000ec70: 2020 2020 7061 7373 225d 290a 2020 2020      pass"]).    
+0000ec80: 2020 2020 2020 2020 2020 2020 7465 7374              test
+0000ec90: 5f66 696c 652e 7772 6974 655f 6279 7465  _file.write_byte
+0000eca0: 7328 636f 6e74 656e 7473 2e65 6e63 6f64  s(contents.encod
+0000ecb0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+0000ecc0: 2020 2020 2066 6628 7465 7374 5f66 696c       ff(test_fil
+0000ecd0: 652c 2077 7269 7465 5f62 6163 6b3d 7079  e, write_back=py
+0000ece0: 696e 6b2e 5772 6974 6542 6163 6b2e 5945  ink.WriteBack.YE
+0000ecf0: 5329 0a20 2020 2020 2020 2020 2020 2020  S).             
+0000ed00: 2020 2075 7064 6174 6564 5f63 6f6e 7465     updated_conte
+0000ed10: 6e74 733a 2062 7974 6573 203d 2074 6573  nts: bytes = tes
+0000ed20: 745f 6669 6c65 2e72 6561 645f 6279 7465  t_file.read_byte
+0000ed30: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0000ed40: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+0000ed50: 6e28 6e6c 2e65 6e63 6f64 6528 292c 2075  n(nl.encode(), u
+0000ed60: 7064 6174 6564 5f63 6f6e 7465 6e74 7329  pdated_contents)
+0000ed70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ed80: 2069 6620 6e6c 203d 3d20 225c 6e22 3a0a   if nl == "\n":.
+0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eda0: 2020 2020 7365 6c66 2e61 7373 6572 744e      self.assertN
+0000edb0: 6f74 496e 2862 225c 725c 6e22 2c20 7570  otIn(b"\r\n", up
+0000edc0: 6461 7465 645f 636f 6e74 656e 7473 290a  dated_contents).
+0000edd0: 0a20 2020 2064 6566 2074 6573 745f 7072  .    def test_pr
+0000ede0: 6573 6572 7665 735f 6c69 6e65 5f65 6e64  eserves_line_end
+0000edf0: 696e 6773 5f76 6961 5f73 7464 696e 2873  ings_via_stdin(s
+0000ee00: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000ee10: 2020 2020 2020 666f 7220 6e6c 2069 6e20        for nl in 
+0000ee20: 5b22 5c6e 222c 2022 5c72 5c6e 225d 3a0a  ["\n", "\r\n"]:.
+0000ee30: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000ee40: 656e 7473 203d 206e 6c2e 6a6f 696e 285b  ents = nl.join([
+0000ee50: 2264 6566 2066 2820 2029 3a22 2c20 2220  "def f(  ):", " 
+0000ee60: 2020 2070 6173 7322 5d29 0a20 2020 2020     pass"]).     
+0000ee70: 2020 2020 2020 2072 756e 6e65 7220 3d20         runner = 
+0000ee80: 426c 6163 6b52 756e 6e65 7228 290a 2020  BlackRunner().  
+0000ee90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000eea0: 203d 2072 756e 6e65 722e 696e 766f 6b65   = runner.invoke
+0000eeb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000eec0: 2020 7079 696e 6b2e 6d61 696e 2c20 5b22    pyink.main, ["
+0000eed0: 2d22 2c20 222d 2d66 6173 7422 5d2c 2069  -", "--fast"], i
+0000eee0: 6e70 7574 3d42 7974 6573 494f 2863 6f6e  nput=BytesIO(con
+0000eef0: 7465 6e74 732e 656e 636f 6465 2822 7574  tents.encode("ut
+0000ef00: 6638 2229 290a 2020 2020 2020 2020 2020  f8")).          
+0000ef10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ef20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000ef30: 2872 6573 756c 742e 6578 6974 5f63 6f64  (result.exit_cod
+0000ef40: 652c 2030 290a 2020 2020 2020 2020 2020  e, 0).          
+0000ef50: 2020 6f75 7470 7574 203d 2072 6573 756c    output = resul
+0000ef60: 742e 7374 646f 7574 5f62 7974 6573 0a20  t.stdout_bytes. 
+0000ef70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ef80: 6173 7365 7274 496e 286e 6c2e 656e 636f  assertIn(nl.enco
+0000ef90: 6465 2822 7574 6638 2229 2c20 6f75 7470  de("utf8"), outp
+0000efa0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+0000efb0: 6966 206e 6c20 3d3d 2022 5c6e 223a 0a20  if nl == "\n":. 
+0000efc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000efd0: 656c 662e 6173 7365 7274 4e6f 7449 6e28  elf.assertNotIn(
+0000efe0: 6222 5c72 5c6e 222c 206f 7574 7075 7429  b"\r\n", output)
+0000eff0: 0a0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
+0000f000: 6f72 6d61 6c69 7a65 5f6c 696e 655f 656e  ormalize_line_en
+0000f010: 6469 6e67 7328 7365 6c66 2920 2d3e 204e  dings(self) -> N
+0000f020: 6f6e 653a 0a20 2020 2020 2020 2077 6974  one:.        wit
+0000f030: 6820 5465 6d70 6f72 6172 7944 6972 6563  h TemporaryDirec
+0000f040: 746f 7279 2829 2061 7320 776f 726b 7370  tory() as worksp
+0000f050: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
+0000f060: 2074 6573 745f 6669 6c65 203d 2050 6174   test_file = Pat
+0000f070: 6828 776f 726b 7370 6163 6529 202f 2022  h(workspace) / "
+0000f080: 7465 7374 2e70 7922 0a20 2020 2020 2020  test.py".       
+0000f090: 2020 2020 2066 6f72 2064 6174 612c 2065       for data, e
+0000f0a0: 7870 6563 7465 6420 696e 2028 0a20 2020  xpected in (.   
+0000f0b0: 2020 2020 2020 2020 2020 2020 2028 6222               (b"
+0000f0c0: 635c 725c 6e63 5c6e 2022 2c20 6222 635c  c\r\nc\n ", b"c\
+0000f0d0: 725c 6e63 5c72 5c6e 2229 2c0a 2020 2020  r\nc\r\n"),.    
+0000f0e0: 2020 2020 2020 2020 2020 2020 2862 226c              (b"l
+0000f0f0: 5c6e 6c5c 725c 6e20 222c 2062 226c 5c6e  \nl\r\n ", b"l\n
+0000f100: 6c5c 6e22 292c 0a20 2020 2020 2020 2020  l\n"),.         
+0000f110: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000f120: 2020 2020 2020 7465 7374 5f66 696c 652e        test_file.
+0000f130: 7772 6974 655f 6279 7465 7328 6461 7461  write_bytes(data
+0000f140: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f150: 2020 6666 2874 6573 745f 6669 6c65 2c20    ff(test_file, 
+0000f160: 7772 6974 655f 6261 636b 3d70 7969 6e6b  write_back=pyink
+0000f170: 2e57 7269 7465 4261 636b 2e59 4553 290a  .WriteBack.YES).
+0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f190: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000f1a0: 2874 6573 745f 6669 6c65 2e72 6561 645f  (test_file.read_
+0000f1b0: 6279 7465 7328 292c 2065 7870 6563 7465  bytes(), expecte
+0000f1c0: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
+0000f1d0: 5f61 7373 6572 745f 6571 7569 7661 6c65  _assert_equivale
+0000f1e0: 6e74 5f64 6966 6665 7265 6e74 5f61 7374  nt_different_ast
+0000f1f0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
+0000f200: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000f210: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+0000f220: 4173 7365 7274 696f 6e45 7272 6f72 293a  AssertionError):
+0000f230: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
+0000f240: 6e6b 2e61 7373 6572 745f 6571 7569 7661  nk.assert_equiva
+0000f250: 6c65 6e74 2822 7b7d 222c 2022 4e6f 6e65  lent("{}", "None
+0000f260: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+0000f270: 5f73 6868 685f 636c 6963 6b28 7365 6c66  _shhh_click(self
+0000f280: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f290: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000f2a0: 2020 2020 6672 6f6d 2063 6c69 636b 2069      from click i
+0000f2b0: 6d70 6f72 7420 5f75 6e69 636f 6465 6675  mport _unicodefu
+0000f2c0: 6e20 2023 2074 7970 653a 2069 676e 6f72  n  # type: ignor
+0000f2d0: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
+0000f2e0: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
+0000f2f0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f300: 6b69 7054 6573 7428 2249 6e63 6f6d 7061  kipTest("Incompa
+0000f310: 7469 626c 6520 436c 6963 6b20 7665 7273  tible Click vers
+0000f320: 696f 6e22 290a 0a20 2020 2020 2020 2069  ion")..        i
+0000f330: 6620 6e6f 7420 6861 7361 7474 7228 5f75  f not hasattr(_u
+0000f340: 6e69 636f 6465 6675 6e2c 2022 5f76 6572  nicodefun, "_ver
+0000f350: 6966 795f 7079 7468 6f6e 5f65 6e76 2229  ify_python_env")
+0000f360: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f370: 6c66 2e73 6b69 7054 6573 7428 2249 6e63  lf.skipTest("Inc
+0000f380: 6f6d 7061 7469 626c 6520 436c 6963 6b20  ompatible Click 
+0000f390: 7665 7273 696f 6e22 290a 0a20 2020 2020  version")..     
+0000f3a0: 2020 2023 2046 6972 7374 2c20 6c65 7427     # First, let'
+0000f3b0: 7320 7365 6520 6966 2043 6c69 636b 2069  s see if Click i
+0000f3c0: 7320 6372 6173 6869 6e67 2077 6974 6820  s crashing with 
+0000f3d0: 6120 7072 6566 6572 7265 6420 4153 4349  a preferred ASCI
+0000f3e0: 4920 6368 6172 7365 742e 0a20 2020 2020  I charset..     
+0000f3f0: 2020 2077 6974 6820 7061 7463 6828 226c     with patch("l
+0000f400: 6f63 616c 652e 6765 7470 7265 6665 7272  ocale.getpreferr
+0000f410: 6564 656e 636f 6469 6e67 2229 2061 7320  edencoding") as 
+0000f420: 6770 653a 0a20 2020 2020 2020 2020 2020  gpe:.           
+0000f430: 2067 7065 2e72 6574 7572 6e5f 7661 6c75   gpe.return_valu
+0000f440: 6520 3d20 2241 5343 4949 220a 2020 2020  e = "ASCII".    
+0000f450: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000f460: 662e 6173 7365 7274 5261 6973 6573 2852  f.assertRaises(R
+0000f470: 756e 7469 6d65 4572 726f 7229 3a0a 2020  untimeError):.  
+0000f480: 2020 2020 2020 2020 2020 2020 2020 5f75                _u
+0000f490: 6e69 636f 6465 6675 6e2e 5f76 6572 6966  nicodefun._verif
+0000f4a0: 795f 7079 7468 6f6e 5f65 6e76 2829 0a20  y_python_env(). 
+0000f4b0: 2020 2020 2020 2023 204e 6f77 2c20 6c65         # Now, le
+0000f4c0: 7427 7320 7369 6c65 6e63 6520 436c 6963  t's silence Clic
+0000f4d0: 6b2e 2e2e 0a20 2020 2020 2020 2070 7969  k....        pyi
+0000f4e0: 6e6b 2e70 6174 6368 5f63 6c69 636b 2829  nk.patch_click()
+0000f4f0: 0a20 2020 2020 2020 2023 202e 2e2e 616e  .        # ...an
+0000f500: 6420 636f 6e66 6972 6d20 6974 2773 2073  d confirm it's s
+0000f510: 696c 656e 742e 0a20 2020 2020 2020 2077  ilent..        w
+0000f520: 6974 6820 7061 7463 6828 226c 6f63 616c  ith patch("local
+0000f530: 652e 6765 7470 7265 6665 7272 6564 656e  e.getpreferreden
+0000f540: 636f 6469 6e67 2229 2061 7320 6770 653a  coding") as gpe:
+0000f550: 0a20 2020 2020 2020 2020 2020 2067 7065  .            gpe
+0000f560: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+0000f570: 2241 5343 4949 220a 2020 2020 2020 2020  "ASCII".        
+0000f580: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000f590: 2020 2020 2020 2020 205f 756e 6963 6f64           _unicod
+0000f5a0: 6566 756e 2e5f 7665 7269 6679 5f70 7974  efun._verify_pyt
+0000f5b0: 686f 6e5f 656e 7628 290a 2020 2020 2020  hon_env().      
+0000f5c0: 2020 2020 2020 6578 6365 7074 2052 756e        except Run
+0000f5d0: 7469 6d65 4572 726f 7220 6173 2072 653a  timeError as re:
+0000f5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f5f0: 2073 656c 662e 6661 696c 2866 2260 7061   self.fail(f"`pa
+0000f600: 7463 685f 636c 6963 6b28 2960 2066 6169  tch_click()` fai
+0000f610: 6c65 642c 2065 7863 6570 7469 6f6e 2073  led, exception s
+0000f620: 7469 6c6c 2072 6169 7365 643a 207b 7265  till raised: {re
+0000f630: 7d22 290a 0a20 2020 2064 6566 2074 6573  }")..    def tes
+0000f640: 745f 726f 6f74 5f6c 6f67 6765 725f 6e6f  t_root_logger_no
+0000f650: 745f 7573 6564 5f64 6972 6563 746c 7928  t_used_directly(
+0000f660: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000f670: 2020 2020 2020 2064 6566 2066 6169 6c28         def fail(
+0000f680: 2a61 7267 733a 2041 6e79 2c20 2a2a 6b77  *args: Any, **kw
+0000f690: 6172 6773 3a20 416e 7929 202d 3e20 4e6f  args: Any) -> No
+0000f6a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f6b0: 7365 6c66 2e66 6169 6c28 2252 6563 6f72  self.fail("Recor
+0000f6c0: 6420 6372 6561 7465 6420 7769 7468 2072  d created with r
+0000f6d0: 6f6f 7420 6c6f 6767 6572 2229 0a0a 2020  oot logger")..  
+0000f6e0: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
+0000f6f0: 2e6d 756c 7469 706c 6528 0a20 2020 2020  .multiple(.     
+0000f700: 2020 2020 2020 206c 6f67 6769 6e67 2e72         logging.r
+0000f710: 6f6f 742c 0a20 2020 2020 2020 2020 2020  oot,.           
+0000f720: 2064 6562 7567 3d66 6169 6c2c 0a20 2020   debug=fail,.   
+0000f730: 2020 2020 2020 2020 2069 6e66 6f3d 6661           info=fa
+0000f740: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
+0000f750: 7761 726e 696e 673d 6661 696c 2c0a 2020  warning=fail,.  
+0000f760: 2020 2020 2020 2020 2020 6572 726f 723d            error=
+0000f770: 6661 696c 2c0a 2020 2020 2020 2020 2020  fail,.          
+0000f780: 2020 6372 6974 6963 616c 3d66 6169 6c2c    critical=fail,
+0000f790: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000f7a0: 3d66 6169 6c2c 0a20 2020 2020 2020 2029  =fail,.        )
+0000f7b0: 3a0a 2020 2020 2020 2020 2020 2020 6666  :.            ff
+0000f7c0: 2854 4849 535f 4449 5220 2f20 2275 7469  (THIS_DIR / "uti
+0000f7d0: 6c2e 7079 2229 0a0a 2020 2020 6465 6620  l.py")..    def 
+0000f7e0: 7465 7374 5f69 6e76 616c 6964 5f63 6f6e  test_invalid_con
+0000f7f0: 6669 675f 7265 7475 726e 5f63 6f64 6528  fig_return_code(
+0000f800: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000f810: 2020 2020 2020 2074 6d70 5f66 696c 6520         tmp_file 
+0000f820: 3d20 5061 7468 2870 7969 6e6b 2e64 756d  = Path(pyink.dum
+0000f830: 705f 746f 5f66 696c 6528 2929 0a20 2020  p_to_file()).   
+0000f840: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000f850: 2020 2020 2020 746d 705f 636f 6e66 6967        tmp_config
+0000f860: 203d 2050 6174 6828 7079 696e 6b2e 6475   = Path(pyink.du
+0000f870: 6d70 5f74 6f5f 6669 6c65 2829 290a 2020  mp_to_file()).  
+0000f880: 2020 2020 2020 2020 2020 746d 705f 636f            tmp_co
+0000f890: 6e66 6967 2e75 6e6c 696e 6b28 290a 2020  nfig.unlink().  
+0000f8a0: 2020 2020 2020 2020 2020 6172 6773 203d            args =
+0000f8b0: 205b 222d 2d63 6f6e 6669 6722 2c20 7374   ["--config", st
+0000f8c0: 7228 746d 705f 636f 6e66 6967 292c 2073  r(tmp_config), s
+0000f8d0: 7472 2874 6d70 5f66 696c 6529 5d0a 2020  tr(tmp_file)].  
+0000f8e0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+0000f8f0: 6e76 6f6b 6542 6c61 636b 2861 7267 732c  nvokeBlack(args,
+0000f900: 2065 7869 745f 636f 6465 3d32 2c20 6967   exit_code=2, ig
+0000f910: 6e6f 7265 5f63 6f6e 6669 673d 4661 6c73  nore_config=Fals
+0000f920: 6529 0a20 2020 2020 2020 2066 696e 616c  e).        final
+0000f930: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
+0000f940: 746d 705f 6669 6c65 2e75 6e6c 696e 6b28  tmp_file.unlink(
+0000f950: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000f960: 7061 7273 655f 7079 7072 6f6a 6563 745f  parse_pyproject_
+0000f970: 746f 6d6c 2873 656c 6629 202d 3e20 4e6f  toml(self) -> No
+0000f980: 6e65 3a0a 2020 2020 2020 2020 7465 7374  ne:.        test
+0000f990: 5f74 6f6d 6c5f 6669 6c65 203d 2054 4849  _toml_file = THI
+0000f9a0: 535f 4449 5220 2f20 2274 6573 742e 746f  S_DIR / "test.to
+0000f9b0: 6d6c 220a 2020 2020 2020 2020 636f 6e66  ml".        conf
+0000f9c0: 6967 203d 2070 7969 6e6b 2e70 6172 7365  ig = pyink.parse
+0000f9d0: 5f70 7970 726f 6a65 6374 5f74 6f6d 6c28  _pyproject_toml(
+0000f9e0: 7374 7228 7465 7374 5f74 6f6d 6c5f 6669  str(test_toml_fi
+0000f9f0: 6c65 2929 0a20 2020 2020 2020 2073 656c  le)).        sel
+0000fa00: 662e 6173 7365 7274 4571 7561 6c28 636f  f.assertEqual(co
+0000fa10: 6e66 6967 5b22 7665 7262 6f73 6522 5d2c  nfig["verbose"],
+0000fa20: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
+0000fa30: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
+0000fa40: 6669 675b 2263 6865 636b 225d 2c20 226e  fig["check"], "n
+0000fa50: 6f22 290a 2020 2020 2020 2020 7365 6c66  o").        self
+0000fa60: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
+0000fa70: 6669 675b 2264 6966 6622 5d2c 2022 7922  fig["diff"], "y"
+0000fa80: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000fa90: 7373 6572 7445 7175 616c 2863 6f6e 6669  ssertEqual(confi
+0000faa0: 675b 2263 6f6c 6f72 225d 2c20 5472 7565  g["color"], True
+0000fab0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000fac0: 7373 6572 7445 7175 616c 2863 6f6e 6669  ssertEqual(confi
+0000fad0: 675b 226c 696e 655f 6c65 6e67 7468 225d  g["line_length"]
+0000fae0: 2c20 3739 290a 2020 2020 2020 2020 7365  , 79).        se
+0000faf0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+0000fb00: 6f6e 6669 675b 2274 6172 6765 745f 7665  onfig["target_ve
+0000fb10: 7273 696f 6e22 5d2c 205b 2270 7933 3622  rsion"], ["py36"
+0000fb20: 2c20 2270 7933 3722 2c20 2270 7933 3822  , "py37", "py38"
+0000fb30: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+0000fb40: 6173 7365 7274 4571 7561 6c28 636f 6e66  assertEqual(conf
+0000fb50: 6967 5b22 7079 7468 6f6e 5f63 656c 6c5f  ig["python_cell_
+0000fb60: 6d61 6769 6373 225d 2c20 5b22 6375 7374  magics"], ["cust
+0000fb70: 6f6d 3122 2c20 2263 7573 746f 6d32 225d  om1", "custom2"]
+0000fb80: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000fb90: 7373 6572 7445 7175 616c 2863 6f6e 6669  ssertEqual(confi
+0000fba0: 675b 2265 7863 6c75 6465 225d 2c20 7222  g["exclude"], r"
+0000fbb0: 5c2e 7079 693f 2422 290a 2020 2020 2020  \.pyi?$").      
+0000fbc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000fbd0: 616c 2863 6f6e 6669 675b 2269 6e63 6c75  al(config["inclu
+0000fbe0: 6465 225d 2c20 7222 5c2e 7079 3f24 2229  de"], r"\.py?$")
+0000fbf0: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+0000fc00: 6172 7365 5f70 7970 726f 6a65 6374 5f74  arse_pyproject_t
+0000fc10: 6f6d 6c5f 7072 6f6a 6563 745f 6d65 7461  oml_project_meta
+0000fc20: 6461 7461 2873 656c 6629 202d 3e20 4e6f  data(self) -> No
+0000fc30: 6e65 3a0a 2020 2020 2020 2020 666f 7220  ne:.        for 
+0000fc40: 7465 7374 5f74 6f6d 6c2c 2065 7870 6563  test_toml, expec
+0000fc50: 7465 6420 696e 205b 0a20 2020 2020 2020  ted in [.       
+0000fc60: 2020 2020 2028 226f 6e6c 795f 626c 6163       ("only_blac
+0000fc70: 6b5f 7079 7072 6f6a 6563 742e 746f 6d6c  k_pyproject.toml
+0000fc80: 222c 205b 2270 7933 3130 225d 292c 0a20  ", ["py310"]),. 
+0000fc90: 2020 2020 2020 2020 2020 2028 226f 6e6c             ("onl
+0000fca0: 795f 6d65 7461 6461 7461 5f70 7970 726f  y_metadata_pypro
+0000fcb0: 6a65 6374 2e74 6f6d 6c22 2c20 5b22 7079  ject.toml", ["py
+0000fcc0: 3337 222c 2022 7079 3338 222c 2022 7079  37", "py38", "py
+0000fcd0: 3339 222c 2022 7079 3331 3022 5d29 2c0a  39", "py310"]),.
+0000fce0: 2020 2020 2020 2020 2020 2020 2822 6e65              ("ne
+0000fcf0: 6974 6865 725f 7079 7072 6f6a 6563 742e  ither_pyproject.
+0000fd00: 746f 6d6c 222c 204e 6f6e 6529 2c0a 2020  toml", None),.  
+0000fd10: 2020 2020 2020 2020 2020 2822 626f 7468            ("both
+0000fd20: 5f70 7970 726f 6a65 6374 2e74 6f6d 6c22  _pyproject.toml"
+0000fd30: 2c20 5b22 7079 3331 3022 5d29 2c0a 2020  , ["py310"]),.  
+0000fd40: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
+0000fd50: 2020 2020 2074 6573 745f 746f 6d6c 5f66       test_toml_f
+0000fd60: 696c 6520 3d20 5448 4953 5f44 4952 202f  ile = THIS_DIR /
+0000fd70: 2022 6461 7461 2220 2f20 2270 726f 6a65   "data" / "proje
+0000fd80: 6374 5f6d 6574 6164 6174 6122 202f 2074  ct_metadata" / t
+0000fd90: 6573 745f 746f 6d6c 0a20 2020 2020 2020  est_toml.       
+0000fda0: 2020 2020 2063 6f6e 6669 6720 3d20 7079       config = py
+0000fdb0: 696e 6b2e 7061 7273 655f 7079 7072 6f6a  ink.parse_pyproj
+0000fdc0: 6563 745f 746f 6d6c 2873 7472 2874 6573  ect_toml(str(tes
+0000fdd0: 745f 746f 6d6c 5f66 696c 6529 290a 2020  t_toml_file)).  
+0000fde0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fdf0: 7373 6572 7445 7175 616c 2863 6f6e 6669  ssertEqual(confi
+0000fe00: 672e 6765 7428 2274 6172 6765 745f 7665  g.get("target_ve
+0000fe10: 7273 696f 6e22 292c 2065 7870 6563 7465  rsion"), expecte
+0000fe20: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
+0000fe30: 5f69 6e66 6572 5f74 6172 6765 745f 7665  _infer_target_ve
+0000fe40: 7273 696f 6e28 7365 6c66 2920 2d3e 204e  rsion(self) -> N
+0000fe50: 6f6e 653a 0a20 2020 2020 2020 2066 6f72  one:.        for
+0000fe60: 2076 6572 7369 6f6e 2c20 6578 7065 6374   version, expect
+0000fe70: 6564 2069 6e20 5b0a 2020 2020 2020 2020  ed in [.        
+0000fe80: 2020 2020 2822 332e 3622 2c20 5b54 6172      ("3.6", [Tar
+0000fe90: 6765 7456 6572 7369 6f6e 2e50 5933 365d  getVersion.PY36]
+0000fea0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0000feb0: 2233 2e31 312e 3072 6331 222c 205b 5461  "3.11.0rc1", [Ta
+0000fec0: 7267 6574 5665 7273 696f 6e2e 5059 3331  rgetVersion.PY31
+0000fed0: 315d 292c 0a20 2020 2020 2020 2020 2020  1]),.           
+0000fee0: 2028 223e 3d33 2e31 3022 2c20 5b54 6172   (">=3.10", [Tar
+0000fef0: 6765 7456 6572 7369 6f6e 2e50 5933 3130  getVersion.PY310
+0000ff00: 2c20 5461 7267 6574 5665 7273 696f 6e2e  , TargetVersion.
+0000ff10: 5059 3331 315d 292c 0a20 2020 2020 2020  PY311]),.       
+0000ff20: 2020 2020 2028 223e 3d33 2e31 302e 3622       (">=3.10.6"
+0000ff30: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
+0000ff40: 2e50 5933 3130 2c20 5461 7267 6574 5665  .PY310, TargetVe
+0000ff50: 7273 696f 6e2e 5059 3331 315d 292c 0a20  rsion.PY311]),. 
+0000ff60: 2020 2020 2020 2020 2020 2028 223c 332e             ("<3.
+0000ff70: 3622 2c20 5b54 6172 6765 7456 6572 7369  6", [TargetVersi
+0000ff80: 6f6e 2e50 5933 332c 2054 6172 6765 7456  on.PY33, TargetV
+0000ff90: 6572 7369 6f6e 2e50 5933 342c 2054 6172  ersion.PY34, Tar
+0000ffa0: 6765 7456 6572 7369 6f6e 2e50 5933 355d  getVersion.PY35]
+0000ffb0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0000ffc0: 223e 332e 372c 3c33 2e31 3022 2c20 5b54  ">3.7,<3.10", [T
+0000ffd0: 6172 6765 7456 6572 7369 6f6e 2e50 5933  argetVersion.PY3
+0000ffe0: 382c 2054 6172 6765 7456 6572 7369 6f6e  8, TargetVersion
+0000fff0: 2e50 5933 395d 292c 0a20 2020 2020 2020  .PY39]),.       
+00010000: 2020 2020 2028 223e 332e 372c 213d 332e       (">3.7,!=3.
+00010010: 382c 213d 332e 3922 2c20 5b54 6172 6765  8,!=3.9", [Targe
+00010020: 7456 6572 7369 6f6e 2e50 5933 3130 2c20  tVersion.PY310, 
+00010030: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
+00010040: 3331 315d 292c 0a20 2020 2020 2020 2020  311]),.         
+00010050: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00010060: 2020 2020 2022 3e20 332e 392e 342c 2021       "> 3.9.4, !
+00010070: 3d20 332e 3130 2e33 222c 0a20 2020 2020  = 3.10.3",.     
+00010080: 2020 2020 2020 2020 2020 205b 5461 7267             [Targ
+00010090: 6574 5665 7273 696f 6e2e 5059 3339 2c20  etVersion.PY39, 
+000100a0: 5461 7267 6574 5665 7273 696f 6e2e 5059  TargetVersion.PY
+000100b0: 3331 302c 2054 6172 6765 7456 6572 7369  310, TargetVersi
+000100c0: 6f6e 2e50 5933 3131 5d2c 0a20 2020 2020  on.PY311],.     
+000100d0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000100e0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+000100f0: 2020 2020 2020 2020 2221 3d33 2e33 2c21          "!=3.3,!
+00010100: 3d33 2e34 222c 0a20 2020 2020 2020 2020  =3.4",.         
+00010110: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00010120: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+00010130: 6765 7456 6572 7369 6f6e 2e50 5933 352c  getVersion.PY35,
+00010140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010150: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+00010160: 6f6e 2e50 5933 362c 0a20 2020 2020 2020  on.PY36,.       
+00010170: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+00010180: 6765 7456 6572 7369 6f6e 2e50 5933 372c  getVersion.PY37,
+00010190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101a0: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+000101b0: 6f6e 2e50 5933 382c 0a20 2020 2020 2020  on.PY38,.       
+000101c0: 2020 2020 2020 2020 2020 2020 2054 6172               Tar
+000101d0: 6765 7456 6572 7369 6f6e 2e50 5933 392c  getVersion.PY39,
+000101e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101f0: 2020 2020 2054 6172 6765 7456 6572 7369       TargetVersi
+00010200: 6f6e 2e50 5933 3130 2c0a 2020 2020 2020  on.PY310,.      
+00010210: 2020 2020 2020 2020 2020 2020 2020 5461                Ta
+00010220: 7267 6574 5665 7273 696f 6e2e 5059 3331  rgetVersion.PY31
+00010230: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00010240: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00010250: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00010260: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00010270: 2020 2022 3d3d 332e 2a22 2c0a 2020 2020     "==3.*",.    
+00010280: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 5461 7267 6574 5665 7273 696f 6e2e    TargetVersion.
+000102b0: 5059 3333 2c0a 2020 2020 2020 2020 2020  PY33,.          
+000102c0: 2020 2020 2020 2020 2020 5461 7267 6574            Target
+000102d0: 5665 7273 696f 6e2e 5059 3334 2c0a 2020  Version.PY34,.  
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 5461 7267 6574 5665 7273 696f 6e2e    TargetVersion.
+00010300: 5059 3335 2c0a 2020 2020 2020 2020 2020  PY35,.          
+00010310: 2020 2020 2020 2020 2020 5461 7267 6574            Target
+00010320: 5665 7273 696f 6e2e 5059 3336 2c0a 2020  Version.PY36,.  
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2020 5461 7267 6574 5665 7273 696f 6e2e    TargetVersion.
+00010350: 5059 3337 2c0a 2020 2020 2020 2020 2020  PY37,.          
+00010360: 2020 2020 2020 2020 2020 5461 7267 6574            Target
+00010370: 5665 7273 696f 6e2e 5059 3338 2c0a 2020  Version.PY38,.  
+00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010390: 2020 5461 7267 6574 5665 7273 696f 6e2e    TargetVersion.
+000103a0: 5059 3339 2c0a 2020 2020 2020 2020 2020  PY39,.          
+000103b0: 2020 2020 2020 2020 2020 5461 7267 6574            Target
+000103c0: 5665 7273 696f 6e2e 5059 3331 302c 0a20  Version.PY310,. 
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2054 6172 6765 7456 6572 7369 6f6e     TargetVersion
+000103f0: 2e50 5933 3131 2c0a 2020 2020 2020 2020  .PY311,.        
+00010400: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00010410: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00010420: 2020 2020 2020 2822 3d3d 332e 382e 2a22        ("==3.8.*"
+00010430: 2c20 5b54 6172 6765 7456 6572 7369 6f6e  , [TargetVersion
+00010440: 2e50 5933 385d 292c 0a20 2020 2020 2020  .PY38]),.       
+00010450: 2020 2020 2028 4e6f 6e65 2c20 4e6f 6e65       (None, None
+00010460: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00010470: 2222 2c20 4e6f 6e65 292c 0a20 2020 2020  "", None),.     
+00010480: 2020 2020 2020 2028 2269 6e76 616c 6964         ("invalid
+00010490: 222c 204e 6f6e 6529 2c0a 2020 2020 2020  ", None),.      
+000104a0: 2020 2020 2020 2822 3d3d 696e 7661 6c69        ("==invali
+000104b0: 6422 2c20 4e6f 6e65 292c 0a20 2020 2020  d", None),.     
+000104c0: 2020 2020 2020 2028 223e 332e 392c 213d         (">3.9,!=
+000104d0: 696e 7661 6c69 6422 2c20 4e6f 6e65 292c  invalid", None),
+000104e0: 0a20 2020 2020 2020 2020 2020 2028 2233  .            ("3
+000104f0: 222c 204e 6f6e 6529 2c0a 2020 2020 2020  ", None),.      
+00010500: 2020 2020 2020 2822 332e 3222 2c20 4e6f        ("3.2", No
+00010510: 6e65 292c 0a20 2020 2020 2020 2020 2020  ne),.           
+00010520: 2028 2232 2e37 2e31 3822 2c20 4e6f 6e65   ("2.7.18", None
+00010530: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00010540: 223d 3d32 2e37 222c 204e 6f6e 6529 2c0a  "==2.7", None),.
+00010550: 2020 2020 2020 2020 2020 2020 2822 3e33              (">3
+00010560: 2e31 302c 3c33 2e31 3122 2c20 4e6f 6e65  .10,<3.11", None
+00010570: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
+00010580: 2020 2020 2020 2020 2020 7465 7374 5f74            test_t
+00010590: 6f6d 6c20 3d20 7b22 7072 6f6a 6563 7422  oml = {"project"
+000105a0: 3a20 7b22 7265 7175 6972 6573 2d70 7974  : {"requires-pyt
+000105b0: 686f 6e22 3a20 7665 7273 696f 6e7d 7d0a  hon": version}}.
+000105c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000105d0: 6c74 203d 2070 7969 6e6b 2e66 696c 6573  lt = pyink.files
+000105e0: 2e69 6e66 6572 5f74 6172 6765 745f 7665  .infer_target_ve
+000105f0: 7273 696f 6e28 7465 7374 5f74 6f6d 6c29  rsion(test_toml)
+00010600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010610: 662e 6173 7365 7274 4571 7561 6c28 7265  f.assertEqual(re
+00010620: 7375 6c74 2c20 6578 7065 6374 6564 290a  sult, expected).
+00010630: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+00010640: 6164 5f70 7970 726f 6a65 6374 5f74 6f6d  ad_pyproject_tom
+00010650: 6c28 7365 6c66 2920 2d3e 204e 6f6e 653a  l(self) -> None:
+00010660: 0a20 2020 2020 2020 2074 6573 745f 746f  .        test_to
+00010670: 6d6c 5f66 696c 6520 3d20 5448 4953 5f44  ml_file = THIS_D
+00010680: 4952 202f 2022 7465 7374 2e74 6f6d 6c22  IR / "test.toml"
+00010690: 0a20 2020 2020 2020 2066 616b 655f 6374  .        fake_ct
+000106a0: 7820 3d20 4661 6b65 436f 6e74 6578 7428  x = FakeContext(
+000106b0: 290a 2020 2020 2020 2020 7079 696e 6b2e  ).        pyink.
+000106c0: 7265 6164 5f70 7970 726f 6a65 6374 5f74  read_pyproject_t
+000106d0: 6f6d 6c28 6661 6b65 5f63 7478 2c20 4661  oml(fake_ctx, Fa
+000106e0: 6b65 5061 7261 6d65 7465 7228 292c 2073  keParameter(), s
+000106f0: 7472 2874 6573 745f 746f 6d6c 5f66 696c  tr(test_toml_fil
+00010700: 6529 290a 2020 2020 2020 2020 636f 6e66  e)).        conf
+00010710: 6967 203d 2066 616b 655f 6374 782e 6465  ig = fake_ctx.de
+00010720: 6661 756c 745f 6d61 700a 2020 2020 2020  fault_map.      
+00010730: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00010740: 616c 2863 6f6e 6669 675b 2276 6572 626f  al(config["verbo
+00010750: 7365 225d 2c20 2231 2229 0a20 2020 2020  se"], "1").     
+00010760: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00010770: 7561 6c28 636f 6e66 6967 5b22 6368 6563  ual(config["chec
+00010780: 6b22 5d2c 2022 6e6f 2229 0a20 2020 2020  k"], "no").     
+00010790: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000107a0: 7561 6c28 636f 6e66 6967 5b22 6469 6666  ual(config["diff
+000107b0: 225d 2c20 2279 2229 0a20 2020 2020 2020  "], "y").       
+000107c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000107d0: 6c28 636f 6e66 6967 5b22 636f 6c6f 7222  l(config["color"
+000107e0: 5d2c 2022 5472 7565 2229 0a20 2020 2020  ], "True").     
+000107f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00010800: 7561 6c28 636f 6e66 6967 5b22 6c69 6e65  ual(config["line
+00010810: 5f6c 656e 6774 6822 5d2c 2022 3739 2229  _length"], "79")
+00010820: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00010830: 7365 7274 4571 7561 6c28 636f 6e66 6967  sertEqual(config
+00010840: 5b22 7461 7267 6574 5f76 6572 7369 6f6e  ["target_version
+00010850: 225d 2c20 5b22 7079 3336 222c 2022 7079  "], ["py36", "py
+00010860: 3337 222c 2022 7079 3338 225d 290a 2020  37", "py38"]).  
+00010870: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00010880: 7445 7175 616c 2863 6f6e 6669 675b 2265  tEqual(config["e
+00010890: 7863 6c75 6465 225d 2c20 7222 5c2e 7079  xclude"], r"\.py
+000108a0: 693f 2422 290a 2020 2020 2020 2020 7365  i?$").        se
+000108b0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
+000108c0: 6f6e 6669 675b 2269 6e63 6c75 6465 225d  onfig["include"]
+000108d0: 2c20 7222 5c2e 7079 3f24 2229 0a0a 2020  , r"\.py?$")..  
+000108e0: 2020 4070 7974 6573 742e 6d61 726b 2e69    @pytest.mark.i
+000108f0: 6e63 6f6d 7061 7469 626c 655f 7769 7468  ncompatible_with
+00010900: 5f6d 7970 7963 0a20 2020 2064 6566 2074  _mypyc.    def t
+00010910: 6573 745f 6669 6e64 5f70 726f 6a65 6374  est_find_project
+00010920: 5f72 6f6f 7428 7365 6c66 2920 2d3e 204e  _root(self) -> N
+00010930: 6f6e 653a 0a20 2020 2020 2020 2077 6974  one:.        wit
+00010940: 6820 5465 6d70 6f72 6172 7944 6972 6563  h TemporaryDirec
+00010950: 746f 7279 2829 2061 7320 776f 726b 7370  tory() as worksp
+00010960: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
+00010970: 2072 6f6f 7420 3d20 5061 7468 2877 6f72   root = Path(wor
+00010980: 6b73 7061 6365 290a 2020 2020 2020 2020  kspace).        
+00010990: 2020 2020 7465 7374 5f64 6972 203d 2072      test_dir = r
+000109a0: 6f6f 7420 2f20 2274 6573 7422 0a20 2020  oot / "test".   
+000109b0: 2020 2020 2020 2020 2074 6573 745f 6469           test_di
+000109c0: 722e 6d6b 6469 7228 290a 0a20 2020 2020  r.mkdir()..     
+000109d0: 2020 2020 2020 2073 7263 5f64 6972 203d         src_dir =
+000109e0: 2072 6f6f 7420 2f20 2273 7263 220a 2020   root / "src".  
+000109f0: 2020 2020 2020 2020 2020 7372 635f 6469            src_di
+00010a00: 722e 6d6b 6469 7228 290a 0a20 2020 2020  r.mkdir()..     
+00010a10: 2020 2020 2020 2072 6f6f 745f 7079 7072         root_pypr
+00010a20: 6f6a 6563 7420 3d20 726f 6f74 202f 2022  oject = root / "
+00010a30: 7079 7072 6f6a 6563 742e 746f 6d6c 220a  pyproject.toml".
+00010a40: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00010a50: 5f70 7970 726f 6a65 6374 2e74 6f75 6368  _pyproject.touch
+00010a60: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00010a70: 7263 5f70 7970 726f 6a65 6374 203d 2073  rc_pyproject = s
+00010a80: 7263 5f64 6972 202f 2022 7079 7072 6f6a  rc_dir / "pyproj
+00010a90: 6563 742e 746f 6d6c 220a 2020 2020 2020  ect.toml".      
+00010aa0: 2020 2020 2020 7372 635f 7079 7072 6f6a        src_pyproj
+00010ab0: 6563 742e 746f 7563 6828 290a 2020 2020  ect.touch().    
+00010ac0: 2020 2020 2020 2020 7372 635f 7079 7468          src_pyth
+00010ad0: 6f6e 203d 2073 7263 5f64 6972 202f 2022  on = src_dir / "
+00010ae0: 666f 6f2e 7079 220a 2020 2020 2020 2020  foo.py".        
+00010af0: 2020 2020 7372 635f 7079 7468 6f6e 2e74      src_python.t
+00010b00: 6f75 6368 2829 0a0a 2020 2020 2020 2020  ouch()..        
+00010b10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00010b20: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
+00010b30: 2020 2020 2020 7079 696e 6b2e 6669 6e64        pyink.find
+00010b40: 5f70 726f 6a65 6374 5f72 6f6f 7428 2873  _project_root((s
+00010b50: 7263 5f64 6972 2c20 7465 7374 5f64 6972  rc_dir, test_dir
+00010b60: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00010b70: 2020 2020 2872 6f6f 742e 7265 736f 6c76      (root.resolv
+00010b80: 6528 292c 2022 7079 7072 6f6a 6563 742e  e(), "pyproject.
+00010b90: 746f 6d6c 2229 2c0a 2020 2020 2020 2020  toml"),.        
+00010ba0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010bb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00010bc0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00010bd0: 2020 2020 7079 696e 6b2e 6669 6e64 5f70      pyink.find_p
+00010be0: 726f 6a65 6374 5f72 6f6f 7428 2873 7263  roject_root((src
+00010bf0: 5f64 6972 2c29 292c 0a20 2020 2020 2020  _dir,)),.       
+00010c00: 2020 2020 2020 2020 2028 7372 635f 6469           (src_di
+00010c10: 722e 7265 736f 6c76 6528 292c 2022 7079  r.resolve(), "py
+00010c20: 7072 6f6a 6563 742e 746f 6d6c 2229 2c0a  project.toml"),.
+00010c30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010c40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00010c50: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00010c60: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
+00010c70: 6b2e 6669 6e64 5f70 726f 6a65 6374 5f72  k.find_project_r
+00010c80: 6f6f 7428 2873 7263 5f70 7974 686f 6e2c  oot((src_python,
+00010c90: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00010ca0: 2020 2020 2873 7263 5f64 6972 2e72 6573      (src_dir.res
+00010cb0: 6f6c 7665 2829 2c20 2270 7970 726f 6a65  olve(), "pyproje
+00010cc0: 6374 2e74 6f6d 6c22 292c 0a20 2020 2020  ct.toml"),.     
+00010cd0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00010ce0: 2020 2020 2020 7769 7468 2063 6861 6e67        with chang
+00010cf0: 655f 6469 7265 6374 6f72 7928 7465 7374  e_directory(test
+00010d00: 5f64 6972 293a 0a20 2020 2020 2020 2020  _dir):.         
+00010d10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010d20: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00010d30: 2020 2020 2020 2020 2020 2020 2070 7969               pyi
+00010d40: 6e6b 2e66 696e 645f 7072 6f6a 6563 745f  nk.find_project_
+00010d50: 726f 6f74 2828 222d 222c 292c 2073 7464  root(("-",), std
+00010d60: 696e 5f66 696c 656e 616d 653d 222e 2e2f  in_filename="../
+00010d70: 7372 632f 612e 7079 2229 2c0a 2020 2020  src/a.py"),.    
+00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d90: 2873 7263 5f64 6972 2e72 6573 6f6c 7665  (src_dir.resolve
+00010da0: 2829 2c20 2270 7970 726f 6a65 6374 2e74  (), "pyproject.t
+00010db0: 6f6d 6c22 292c 0a20 2020 2020 2020 2020  oml"),.         
+00010dc0: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
+00010dd0: 6174 6368 280a 2020 2020 2020 2020 2270  atch(.        "p
+00010de0: 7969 6e6b 2e66 696c 6573 2e66 696e 645f  yink.files.find_
+00010df0: 7573 6572 5f70 7970 726f 6a65 6374 5f74  user_pyproject_t
+00010e00: 6f6d 6c22 2c0a 2020 2020 290a 2020 2020  oml",.    ).    
+00010e10: 6465 6620 7465 7374 5f66 696e 645f 7079  def test_find_py
+00010e20: 7072 6f6a 6563 745f 746f 6d6c 2873 656c  project_toml(sel
+00010e30: 662c 2066 696e 645f 7573 6572 5f70 7970  f, find_user_pyp
+00010e40: 726f 6a65 6374 5f74 6f6d 6c3a 204d 6167  roject_toml: Mag
+00010e50: 6963 4d6f 636b 2920 2d3e 204e 6f6e 653a  icMock) -> None:
+00010e60: 0a20 2020 2020 2020 2066 696e 645f 7573  .        find_us
+00010e70: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
+00010e80: 6c2e 7369 6465 5f65 6666 6563 7420 3d20  l.side_effect = 
+00010e90: 5275 6e74 696d 6545 7272 6f72 2829 0a0a  RuntimeError()..
+00010ea0: 2020 2020 2020 2020 7769 7468 2072 6564          with red
+00010eb0: 6972 6563 745f 7374 6465 7272 2869 6f2e  irect_stderr(io.
+00010ec0: 5374 7269 6e67 494f 2829 2920 6173 2073  StringIO()) as s
+00010ed0: 7464 6572 723a 0a20 2020 2020 2020 2020  tderr:.         
+00010ee0: 2020 2072 6573 756c 7420 3d20 7079 696e     result = pyin
+00010ef0: 6b2e 6669 6c65 732e 6669 6e64 5f70 7970  k.files.find_pyp
+00010f00: 726f 6a65 6374 5f74 6f6d 6c28 0a20 2020  roject_toml(.   
+00010f10: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+00010f20: 685f 7365 6172 6368 5f73 7461 7274 3d28  h_search_start=(
+00010f30: 7374 7228 5061 7468 2e63 7764 2829 2e72  str(Path.cwd().r
+00010f40: 6f6f 7429 2c29 0a20 2020 2020 2020 2020  oot),).         
+00010f50: 2020 2029 0a0a 2020 2020 2020 2020 6173     )..        as
+00010f60: 7365 7274 2072 6573 756c 7420 6973 204e  sert result is N
+00010f70: 6f6e 650a 2020 2020 2020 2020 6572 7220  one.        err 
+00010f80: 3d20 7374 6465 7272 2e67 6574 7661 6c75  = stderr.getvalu
+00010f90: 6528 290a 2020 2020 2020 2020 6173 7365  e().        asse
+00010fa0: 7274 2022 4967 6e6f 7269 6e67 2075 7365  rt "Ignoring use
+00010fb0: 7220 636f 6e66 6967 7572 6174 696f 6e22  r configuration"
+00010fc0: 2069 6e20 6572 720a 0a20 2020 2040 7061   in err..    @pa
+00010fd0: 7463 6828 0a20 2020 2020 2020 2022 7079  tch(.        "py
+00010fe0: 696e 6b2e 6669 6c65 732e 6669 6e64 5f75  ink.files.find_u
+00010ff0: 7365 725f 7079 7072 6f6a 6563 745f 746f  ser_pyproject_to
+00011000: 6d6c 222c 0a20 2020 2020 2020 2070 7969  ml",.        pyi
+00011010: 6e6b 2e66 696c 6573 2e66 696e 645f 7573  nk.files.find_us
+00011020: 6572 5f70 7970 726f 6a65 6374 5f74 6f6d  er_pyproject_tom
+00011030: 6c2e 5f5f 7772 6170 7065 645f 5f2c 0a20  l.__wrapped__,. 
+00011040: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
+00011050: 745f 6669 6e64 5f75 7365 725f 7079 7072  t_find_user_pypr
+00011060: 6f6a 6563 745f 746f 6d6c 5f6c 696e 7578  oject_toml_linux
+00011070: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00011080: 2020 2020 2020 2020 6966 2073 7973 7465          if syste
+00011090: 6d28 2920 3d3d 2022 5769 6e64 6f77 7322  m() == "Windows"
+000110a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000110b0: 7475 726e 0a0a 2020 2020 2020 2020 2320  turn..        # 
+000110c0: 5465 7374 2069 6620 5844 475f 434f 4e46  Test if XDG_CONF
+000110d0: 4947 5f48 4f4d 4520 6973 2063 6865 636b  IG_HOME is check
+000110e0: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
+000110f0: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+00011100: 7279 2829 2061 7320 776f 726b 7370 6163  ry() as workspac
+00011110: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00011120: 6d70 5f75 7365 725f 636f 6e66 6967 203d  mp_user_config =
+00011130: 2050 6174 6828 776f 726b 7370 6163 6529   Path(workspace)
+00011140: 202f 2022 7079 696e 6b22 0a20 2020 2020   / "pyink".     
+00011150: 2020 2020 2020 2077 6974 6820 7061 7463         with patc
+00011160: 682e 6469 6374 2822 6f73 2e65 6e76 6972  h.dict("os.envir
+00011170: 6f6e 222c 207b 2258 4447 5f43 4f4e 4649  on", {"XDG_CONFI
+00011180: 475f 484f 4d45 223a 2077 6f72 6b73 7061  G_HOME": workspa
+00011190: 6365 7d29 3a0a 2020 2020 2020 2020 2020  ce}):.          
+000111a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000111b0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+000111c0: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
+000111d0: 6b2e 6669 6c65 732e 6669 6e64 5f75 7365  k.files.find_use
+000111e0: 725f 7079 7072 6f6a 6563 745f 746f 6d6c  r_pyproject_toml
+000111f0: 2829 2c20 746d 705f 7573 6572 5f63 6f6e  (), tmp_user_con
+00011200: 6669 672e 7265 736f 6c76 6528 290a 2020  fig.resolve().  
+00011210: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00011220: 0a20 2020 2020 2020 2023 2054 6573 7420  .        # Test 
+00011230: 6661 6c6c 6261 636b 2066 6f72 2058 4447  fallback for XDG
+00011240: 5f43 4f4e 4649 475f 484f 4d45 0a20 2020  _CONFIG_HOME.   
+00011250: 2020 2020 2077 6974 6820 7061 7463 682e       with patch.
+00011260: 6469 6374 2822 6f73 2e65 6e76 6972 6f6e  dict("os.environ
+00011270: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00011280: 6f73 2e65 6e76 6972 6f6e 2e70 6f70 2822  os.environ.pop("
+00011290: 5844 475f 434f 4e46 4947 5f48 4f4d 4522  XDG_CONFIG_HOME"
+000112a0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+000112b0: 2020 2020 6661 6c6c 6261 636b 5f75 7365      fallback_use
+000112c0: 725f 636f 6e66 6967 203d 2050 6174 6828  r_config = Path(
+000112d0: 227e 2f2e 636f 6e66 6967 2229 2e65 7870  "~/.config").exp
+000112e0: 616e 6475 7365 7228 2920 2f20 2270 7969  anduser() / "pyi
+000112f0: 6e6b 220a 2020 2020 2020 2020 2020 2020  nk".            
+00011300: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00011310: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011320: 2020 7079 696e 6b2e 6669 6c65 732e 6669    pyink.files.fi
+00011330: 6e64 5f75 7365 725f 7079 7072 6f6a 6563  nd_user_pyprojec
+00011340: 745f 746f 6d6c 2829 2c20 6661 6c6c 6261  t_toml(), fallba
+00011350: 636b 5f75 7365 725f 636f 6e66 6967 2e72  ck_user_config.r
+00011360: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
+00011370: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00011380: 7465 7374 5f66 696e 645f 7573 6572 5f70  test_find_user_p
+00011390: 7970 726f 6a65 6374 5f74 6f6d 6c5f 7769  yproject_toml_wi
+000113a0: 6e64 6f77 7328 7365 6c66 2920 2d3e 204e  ndows(self) -> N
+000113b0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+000113c0: 7379 7374 656d 2829 2021 3d20 2257 696e  system() != "Win
+000113d0: 646f 7773 223a 0a20 2020 2020 2020 2020  dows":.         
+000113e0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+000113f0: 2020 2075 7365 725f 636f 6e66 6967 5f70     user_config_p
+00011400: 6174 6820 3d20 5061 7468 2e68 6f6d 6528  ath = Path.home(
+00011410: 2920 2f20 222e 7079 696e 6b22 0a20 2020  ) / ".pyink".   
+00011420: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00011430: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+00011440: 2020 2070 7969 6e6b 2e66 696c 6573 2e66     pyink.files.f
+00011450: 696e 645f 7573 6572 5f70 7970 726f 6a65  ind_user_pyproje
+00011460: 6374 5f74 6f6d 6c28 292c 2075 7365 725f  ct_toml(), user_
+00011470: 636f 6e66 6967 5f70 6174 682e 7265 736f  config_path.reso
+00011480: 6c76 6528 290a 2020 2020 2020 2020 290a  lve().        ).
+00011490: 0a20 2020 2064 6566 2074 6573 745f 6270  .    def test_bp
+000114a0: 6f5f 3333 3636 305f 776f 726b 6172 6f75  o_33660_workarou
+000114b0: 6e64 2873 656c 6629 202d 3e20 4e6f 6e65  nd(self) -> None
+000114c0: 3a0a 2020 2020 2020 2020 6966 2073 7973  :.        if sys
+000114d0: 7465 6d28 2920 3d3d 2022 5769 6e64 6f77  tem() == "Window
+000114e0: 7322 3a0a 2020 2020 2020 2020 2020 2020  s":.            
+000114f0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+00011500: 2320 6874 7470 733a 2f2f 6275 6773 2e70  # https://bugs.p
+00011510: 7974 686f 6e2e 6f72 672f 6973 7375 6533  ython.org/issue3
+00011520: 3336 3630 0a20 2020 2020 2020 2072 6f6f  3660.        roo
+00011530: 7420 3d20 5061 7468 2822 2f22 290a 2020  t = Path("/").  
+00011540: 2020 2020 2020 7769 7468 2063 6861 6e67        with chang
+00011550: 655f 6469 7265 6374 6f72 7928 726f 6f74  e_directory(root
+00011560: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+00011570: 6174 6820 3d20 5061 7468 2822 776f 726b  ath = Path("work
+00011580: 7370 6163 6522 2920 2f20 2270 726f 6a65  space") / "proje
+00011590: 6374 220a 2020 2020 2020 2020 2020 2020  ct".            
+000115a0: 7265 706f 7274 203d 2070 7969 6e6b 2e52  report = pyink.R
+000115b0: 6570 6f72 7428 7665 7262 6f73 653d 5472  eport(verbose=Tr
+000115c0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+000115d0: 6e6f 726d 616c 697a 6564 5f70 6174 6820  normalized_path 
+000115e0: 3d20 7079 696e 6b2e 6e6f 726d 616c 697a  = pyink.normaliz
+000115f0: 655f 7061 7468 5f6d 6179 6265 5f69 676e  e_path_maybe_ign
+00011600: 6f72 6528 7061 7468 2c20 726f 6f74 2c20  ore(path, root, 
+00011610: 7265 706f 7274 290a 2020 2020 2020 2020  report).        
+00011620: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00011630: 7175 616c 286e 6f72 6d61 6c69 7a65 645f  qual(normalized_
+00011640: 7061 7468 2c20 2277 6f72 6b73 7061 6365  path, "workspace
+00011650: 2f70 726f 6a65 6374 2229 0a0a 2020 2020  /project")..    
+00011660: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
+00011670: 7a65 5f70 6174 685f 6967 6e6f 7265 5f77  ze_path_ignore_w
+00011680: 696e 646f 7773 5f6a 756e 6374 696f 6e73  indows_junctions
+00011690: 5f6f 7574 7369 6465 5f6f 665f 726f 6f74  _outside_of_root
+000116a0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000116b0: 2020 2020 2020 2020 6966 2073 7973 7465          if syste
+000116c0: 6d28 2920 213d 2022 5769 6e64 6f77 7322  m() != "Windows"
+000116d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000116e0: 7475 726e 0a0a 2020 2020 2020 2020 7769  turn..        wi
+000116f0: 7468 2054 656d 706f 7261 7279 4469 7265  th TemporaryDire
+00011700: 6374 6f72 7928 2920 6173 2077 6f72 6b73  ctory() as works
+00011710: 7061 6365 3a0a 2020 2020 2020 2020 2020  pace:.          
+00011720: 2020 726f 6f74 203d 2050 6174 6828 776f    root = Path(wo
+00011730: 726b 7370 6163 6529 0a20 2020 2020 2020  rkspace).       
+00011740: 2020 2020 206a 756e 6374 696f 6e5f 6469       junction_di
+00011750: 7220 3d20 726f 6f74 202f 2022 6a75 6e63  r = root / "junc
+00011760: 7469 6f6e 220a 2020 2020 2020 2020 2020  tion".          
+00011770: 2020 6a75 6e63 7469 6f6e 5f74 6172 6765    junction_targe
+00011780: 745f 6f75 7473 6964 655f 6f66 5f72 6f6f  t_outside_of_roo
+00011790: 7420 3d20 726f 6f74 202f 2022 2e2e 220a  t = root / "..".
+000117a0: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
+000117b0: 7973 7465 6d28 6622 6d6b 6c69 6e6b 202f  ystem(f"mklink /
+000117c0: 4a20 7b6a 756e 6374 696f 6e5f 6469 727d  J {junction_dir}
+000117d0: 207b 6a75 6e63 7469 6f6e 5f74 6172 6765   {junction_targe
+000117e0: 745f 6f75 7473 6964 655f 6f66 5f72 6f6f  t_outside_of_roo
+000117f0: 747d 2229 0a0a 2020 2020 2020 2020 2020  t}")..          
+00011800: 2020 7265 706f 7274 203d 2070 7969 6e6b    report = pyink
+00011810: 2e52 6570 6f72 7428 7665 7262 6f73 653d  .Report(verbose=
+00011820: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00011830: 2020 6e6f 726d 616c 697a 6564 5f70 6174    normalized_pat
+00011840: 6820 3d20 7079 696e 6b2e 6e6f 726d 616c  h = pyink.normal
+00011850: 697a 655f 7061 7468 5f6d 6179 6265 5f69  ize_path_maybe_i
+00011860: 676e 6f72 6528 0a20 2020 2020 2020 2020  gnore(.         
+00011870: 2020 2020 2020 206a 756e 6374 696f 6e5f         junction_
+00011880: 6469 722c 2072 6f6f 742c 2072 6570 6f72  dir, root, repor
+00011890: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
+000118a0: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+000118b0: 6e75 616c 6c79 2064 656c 6574 6520 666f  nually delete fo
+000118c0: 7220 5079 7468 6f6e 203c 2033 2e38 0a20  r Python < 3.8. 
+000118d0: 2020 2020 2020 2020 2020 206f 732e 7379             os.sy
+000118e0: 7374 656d 2866 2272 6d64 6972 207b 6a75  stem(f"rmdir {ju
+000118f0: 6e63 7469 6f6e 5f64 6972 7d22 290a 0a20  nction_dir}").. 
+00011900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011910: 6173 7365 7274 4571 7561 6c28 6e6f 726d  assertEqual(norm
+00011920: 616c 697a 6564 5f70 6174 682c 204e 6f6e  alized_path, Non
+00011930: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
+00011940: 5f6e 6577 6c69 6e65 5f63 6f6d 6d65 6e74  _newline_comment
+00011950: 5f69 6e74 6572 6163 7469 6f6e 2873 656c  _interaction(sel
+00011960: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00011970: 2020 2020 736f 7572 6365 203d 2022 636c      source = "cl
+00011980: 6173 7320 413a 5c5c 5c72 5c6e 2320 7479  ass A:\\\r\n# ty
+00011990: 7065 3a20 6967 6e6f 7265 5c6e 2070 6173  pe: ignore\n pas
+000119a0: 735c 6e22 0a20 2020 2020 2020 206f 7574  s\n".        out
+000119b0: 7075 7420 3d20 7079 696e 6b2e 666f 726d  put = pyink.form
+000119c0: 6174 5f73 7472 2873 6f75 7263 652c 206d  at_str(source, m
+000119d0: 6f64 653d 4445 4641 554c 545f 4d4f 4445  ode=DEFAULT_MODE
+000119e0: 290a 2020 2020 2020 2020 7079 696e 6b2e  ).        pyink.
+000119f0: 6173 7365 7274 5f73 7461 626c 6528 736f  assert_stable(so
+00011a00: 7572 6365 2c20 6f75 7470 7574 2c20 6d6f  urce, output, mo
+00011a10: 6465 3d44 4546 4155 4c54 5f4d 4f44 4529  de=DEFAULT_MODE)
+00011a20: 0a0a 2020 2020 6465 6620 7465 7374 5f62  ..    def test_b
+00011a30: 706f 5f32 3134 325f 776f 726b 6172 6f75  po_2142_workarou
+00011a40: 6e64 2873 656c 6629 202d 3e20 4e6f 6e65  nd(self) -> None
+00011a50: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
+00011a60: 733a 2f2f 6275 6773 2e70 7974 686f 6e2e  s://bugs.python.
+00011a70: 6f72 672f 6973 7375 6532 3134 320a 0a20  org/issue2142.. 
+00011a80: 2020 2020 2020 2073 6f75 7263 652c 205f         source, _
+00011a90: 203d 2072 6561 645f 6461 7461 2822 6d69   = read_data("mi
+00011aa0: 7363 656c 6c61 6e65 6f75 7322 2c20 226d  scellaneous", "m
+00011ab0: 6973 7369 6e67 5f66 696e 616c 5f6e 6577  issing_final_new
+00011ac0: 6c69 6e65 2229 0a20 2020 2020 2020 2023  line").        #
+00011ad0: 2072 6561 645f 6461 7461 2061 6464 7320   read_data adds 
+00011ae0: 6120 7472 6169 6c69 6e67 206e 6577 6c69  a trailing newli
+00011af0: 6e65 0a20 2020 2020 2020 2073 6f75 7263  ne.        sourc
+00011b00: 6520 3d20 736f 7572 6365 2e72 7374 7269  e = source.rstri
+00011b10: 7028 290a 2020 2020 2020 2020 6578 7065  p().        expe
+00011b20: 6374 6564 2c20 5f20 3d20 7265 6164 5f64  cted, _ = read_d
+00011b30: 6174 6128 226d 6973 6365 6c6c 616e 656f  ata("miscellaneo
+00011b40: 7573 222c 2022 6d69 7373 696e 675f 6669  us", "missing_fi
+00011b50: 6e61 6c5f 6e65 776c 696e 652e 6469 6666  nal_newline.diff
+00011b60: 2229 0a20 2020 2020 2020 2074 6d70 5f66  ").        tmp_f
+00011b70: 696c 6520 3d20 5061 7468 2870 7969 6e6b  ile = Path(pyink
+00011b80: 2e64 756d 705f 746f 5f66 696c 6528 736f  .dump_to_file(so
+00011b90: 7572 6365 2c20 656e 7375 7265 5f66 696e  urce, ensure_fin
+00011ba0: 616c 5f6e 6577 6c69 6e65 3d46 616c 7365  al_newline=False
+00011bb0: 2929 0a20 2020 2020 2020 2064 6966 665f  )).        diff_
+00011bc0: 6865 6164 6572 203d 2072 652e 636f 6d70  header = re.comp
+00011bd0: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+00011be0: 2072 6622 7b72 652e 6573 6361 7065 2873   rf"{re.escape(s
+00011bf0: 7472 2874 6d70 5f66 696c 6529 297d 5c74  tr(tmp_file))}\t
+00011c00: 5c64 5c64 5c64 5c64 2d5c 645c 642d 5c64  \d\d\d\d-\d\d-\d
+00011c10: 5c64 2022 0a20 2020 2020 2020 2020 2020  \d ".           
+00011c20: 2072 225c 645c 643a 5c64 5c64 3a5c 645c   r"\d\d:\d\d:\d\
+00011c30: 645c 2e5c 645c 645c 645c 645c 645c 6420  d\.\d\d\d\d\d\d 
+00011c40: 5c2b 5c64 5c64 5c64 5c64 220a 2020 2020  \+\d\d\d\d".    
+00011c50: 2020 2020 290a 2020 2020 2020 2020 7472      ).        tr
+00011c60: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+00011c70: 6573 756c 7420 3d20 426c 6163 6b52 756e  esult = BlackRun
+00011c80: 6e65 7228 292e 696e 766f 6b65 2870 7969  ner().invoke(pyi
+00011c90: 6e6b 2e6d 6169 6e2c 205b 222d 2d64 6966  nk.main, ["--dif
+00011ca0: 6622 2c20 7374 7228 746d 705f 6669 6c65  f", str(tmp_file
+00011cb0: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
+00011cc0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00011cd0: 2872 6573 756c 742e 6578 6974 5f63 6f64  (result.exit_cod
+00011ce0: 652c 2030 290a 2020 2020 2020 2020 6669  e, 0).        fi
+00011cf0: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+00011d00: 2020 206f 732e 756e 6c69 6e6b 2874 6d70     os.unlink(tmp
+00011d10: 5f66 696c 6529 0a20 2020 2020 2020 2061  _file).        a
+00011d20: 6374 7561 6c20 3d20 7265 7375 6c74 2e6f  ctual = result.o
+00011d30: 7574 7075 740a 2020 2020 2020 2020 6163  utput.        ac
+00011d40: 7475 616c 203d 2064 6966 665f 6865 6164  tual = diff_head
+00011d50: 6572 2e73 7562 2844 4554 4552 4d49 4e49  er.sub(DETERMINI
+00011d60: 5354 4943 5f48 4541 4445 522c 2061 6374  STIC_HEADER, act
+00011d70: 7561 6c29 0a20 2020 2020 2020 2073 656c  ual).        sel
+00011d80: 662e 6173 7365 7274 4571 7561 6c28 6163  f.assertEqual(ac
+00011d90: 7475 616c 2c20 6578 7065 6374 6564 290a  tual, expected).
+00011da0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00011db0: 6f64 0a20 2020 2064 6566 2063 6f6d 7061  od.    def compa
+00011dc0: 7265 5f72 6573 756c 7473 280a 2020 2020  re_results(.    
+00011dd0: 2020 2020 7265 7375 6c74 3a20 636c 6963      result: clic
+00011de0: 6b2e 7465 7374 696e 672e 5265 7375 6c74  k.testing.Result
+00011df0: 2c20 6578 7065 6374 6564 5f76 616c 7565  , expected_value
+00011e00: 3a20 7374 722c 2065 7870 6563 7465 645f  : str, expected_
+00011e10: 6578 6974 5f63 6f64 653a 2069 6e74 0a20  exit_code: int. 
+00011e20: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00011e30: 2020 2020 2020 2222 2248 656c 7065 7220        """Helper 
+00011e40: 6d65 7468 6f64 2074 6f20 7465 7374 2074  method to test t
+00011e50: 6865 2076 616c 7565 2061 6e64 2065 7869  he value and exi
+00011e60: 7420 636f 6465 206f 6620 6120 636c 6963  t code of a clic
+00011e70: 6b20 5265 7375 6c74 2e22 2222 0a20 2020  k Result.""".   
+00011e80: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
+00011e90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00011ea0: 2e6f 7574 7075 7420 3d3d 2065 7870 6563  .output == expec
+00011eb0: 7465 645f 7661 6c75 650a 2020 2020 2020  ted_value.      
+00011ec0: 2020 292c 2022 5468 6520 6f75 7470 7574    ), "The output
+00011ed0: 2064 6964 206e 6f74 206d 6174 6368 2074   did not match t
+00011ee0: 6865 2065 7870 6563 7465 6420 7661 6c75  he expected valu
+00011ef0: 652e 220a 2020 2020 2020 2020 6173 7365  e.".        asse
+00011f00: 7274 2072 6573 756c 742e 6578 6974 5f63  rt result.exit_c
+00011f10: 6f64 6520 3d3d 2065 7870 6563 7465 645f  ode == expected_
+00011f20: 6578 6974 5f63 6f64 652c 2022 5468 6520  exit_code, "The 
+00011f30: 6578 6974 2063 6f64 6520 6973 2069 6e63  exit code is inc
+00011f40: 6f72 7265 6374 2e22 0a0a 2020 2020 6465  orrect."..    de
+00011f50: 6620 7465 7374 5f63 6f64 655f 6f70 7469  f test_code_opti
+00011f60: 6f6e 2873 656c 6629 202d 3e20 4e6f 6e65  on(self) -> None
+00011f70: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
+00011f80: 7420 7468 6520 636f 6465 206f 7074 696f  t the code optio
+00011f90: 6e20 7769 7468 206e 6f20 6368 616e 6765  n with no change
+00011fa0: 732e 2222 220a 2020 2020 2020 2020 636f  s.""".        co
+00011fb0: 6465 203d 2027 7072 696e 7428 2248 656c  de = 'print("Hel
+00011fc0: 6c6f 2077 6f72 6c64 2229 5c6e 270a 2020  lo world")\n'.  
+00011fd0: 2020 2020 2020 6172 6773 203d 205b 222d        args = ["-
+00011fe0: 2d63 6f64 6522 2c20 636f 6465 5d0a 2020  -code", code].  
+00011ff0: 2020 2020 2020 7265 7375 6c74 203d 2043        result = C
+00012000: 6c69 5275 6e6e 6572 2829 2e69 6e76 6f6b  liRunner().invok
+00012010: 6528 7079 696e 6b2e 6d61 696e 2c20 6172  e(pyink.main, ar
+00012020: 6773 290a 0a20 2020 2020 2020 2073 656c  gs)..        sel
+00012030: 662e 636f 6d70 6172 655f 7265 7375 6c74  f.compare_result
+00012040: 7328 7265 7375 6c74 2c20 636f 6465 2c20  s(result, code, 
+00012050: 3029 0a0a 2020 2020 6465 6620 7465 7374  0)..    def test
+00012060: 5f63 6f64 655f 6f70 7469 6f6e 5f63 6861  _code_option_cha
+00012070: 6e67 6564 2873 656c 6629 202d 3e20 4e6f  nged(self) -> No
+00012080: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
+00012090: 6573 7420 7468 6520 636f 6465 206f 7074  est the code opt
+000120a0: 696f 6e20 7768 656e 2063 6861 6e67 6573  ion when changes
+000120b0: 2061 7265 2072 6571 7569 7265 642e 2222   are required.""
+000120c0: 220a 2020 2020 2020 2020 636f 6465 203d  ".        code =
+000120d0: 2022 7072 696e 7428 2768 656c 6c6f 2077   "print('hello w
+000120e0: 6f72 6c64 2729 220a 2020 2020 2020 2020  orld')".        
+000120f0: 666f 726d 6174 7465 6420 3d20 7079 696e  formatted = pyin
+00012100: 6b2e 666f 726d 6174 5f73 7472 2863 6f64  k.format_str(cod
+00012110: 652c 206d 6f64 653d 4445 4641 554c 545f  e, mode=DEFAULT_
+00012120: 4d4f 4445 290a 0a20 2020 2020 2020 2061  MODE)..        a
+00012130: 7267 7320 3d20 5b22 2d2d 636f 6465 222c  rgs = ["--code",
+00012140: 2063 6f64 655d 0a20 2020 2020 2020 2072   code].        r
+00012150: 6573 756c 7420 3d20 436c 6952 756e 6e65  esult = CliRunne
+00012160: 7228 292e 696e 766f 6b65 2870 7969 6e6b  r().invoke(pyink
+00012170: 2e6d 6169 6e2c 2061 7267 7329 0a0a 2020  .main, args)..  
+00012180: 2020 2020 2020 7365 6c66 2e63 6f6d 7061        self.compa
+00012190: 7265 5f72 6573 756c 7473 2872 6573 756c  re_results(resul
+000121a0: 742c 2066 6f72 6d61 7474 6564 2c20 3029  t, formatted, 0)
+000121b0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+000121c0: 6f64 655f 6f70 7469 6f6e 5f63 6865 636b  ode_option_check
+000121d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000121e0: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
+000121f0: 7468 6520 636f 6465 206f 7074 696f 6e20  the code option 
+00012200: 7768 656e 2063 6865 636b 2069 7320 7061  when check is pa
+00012210: 7373 6564 2e22 2222 0a20 2020 2020 2020  ssed.""".       
+00012220: 2061 7267 7320 3d20 5b22 2d2d 6368 6563   args = ["--chec
+00012230: 6b22 2c20 222d 2d63 6f64 6522 2c20 2770  k", "--code", 'p
+00012240: 7269 6e74 2822 4865 6c6c 6f20 776f 726c  rint("Hello worl
+00012250: 6422 295c 6e27 5d0a 2020 2020 2020 2020  d")\n'].        
+00012260: 7265 7375 6c74 203d 2043 6c69 5275 6e6e  result = CliRunn
+00012270: 6572 2829 2e69 6e76 6f6b 6528 7079 696e  er().invoke(pyin
+00012280: 6b2e 6d61 696e 2c20 6172 6773 290a 2020  k.main, args).  
+00012290: 2020 2020 2020 7365 6c66 2e63 6f6d 7061        self.compa
+000122a0: 7265 5f72 6573 756c 7473 2872 6573 756c  re_results(resul
+000122b0: 742c 2022 222c 2030 290a 0a20 2020 2064  t, "", 0)..    d
+000122c0: 6566 2074 6573 745f 636f 6465 5f6f 7074  ef test_code_opt
+000122d0: 696f 6e5f 6368 6563 6b5f 6368 616e 6765  ion_check_change
+000122e0: 6428 7365 6c66 2920 2d3e 204e 6f6e 653a  d(self) -> None:
+000122f0: 0a20 2020 2020 2020 2022 2222 5465 7374  .        """Test
+00012300: 2074 6865 2063 6f64 6520 6f70 7469 6f6e   the code option
+00012310: 2077 6865 6e20 6368 616e 6765 7320 6172   when changes ar
+00012320: 6520 7265 7175 6972 6564 2c20 616e 6420  e required, and 
+00012330: 6368 6563 6b20 6973 2070 6173 7365 642e  check is passed.
+00012340: 2222 220a 2020 2020 2020 2020 6172 6773  """.        args
+00012350: 203d 205b 222d 2d63 6865 636b 222c 2022   = ["--check", "
+00012360: 2d2d 636f 6465 222c 2022 7072 696e 7428  --code", "print(
+00012370: 2768 656c 6c6f 2077 6f72 6c64 2729 225d  'hello world')"]
+00012380: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00012390: 3d20 436c 6952 756e 6e65 7228 292e 696e  = CliRunner().in
+000123a0: 766f 6b65 2870 7969 6e6b 2e6d 6169 6e2c  voke(pyink.main,
+000123b0: 2061 7267 7329 0a20 2020 2020 2020 2073   args).        s
+000123c0: 656c 662e 636f 6d70 6172 655f 7265 7375  elf.compare_resu
+000123d0: 6c74 7328 7265 7375 6c74 2c20 2222 2c20  lts(result, "", 
+000123e0: 3129 0a0a 2020 2020 6465 6620 7465 7374  1)..    def test
+000123f0: 5f63 6f64 655f 6f70 7469 6f6e 5f64 6966  _code_option_dif
+00012400: 6628 7365 6c66 2920 2d3e 204e 6f6e 653a  f(self) -> None:
+00012410: 0a20 2020 2020 2020 2022 2222 5465 7374  .        """Test
+00012420: 2074 6865 2063 6f64 6520 6f70 7469 6f6e   the code option
+00012430: 2077 6865 6e20 6469 6666 2069 7320 7061   when diff is pa
+00012440: 7373 6564 2e22 2222 0a20 2020 2020 2020  ssed.""".       
+00012450: 2063 6f64 6520 3d20 2270 7269 6e74 2827   code = "print('
+00012460: 6865 6c6c 6f20 776f 726c 6427 2922 0a20  hello world')". 
+00012470: 2020 2020 2020 2066 6f72 6d61 7474 6564         formatted
+00012480: 203d 2070 7969 6e6b 2e66 6f72 6d61 745f   = pyink.format_
+00012490: 7374 7228 636f 6465 2c20 6d6f 6465 3d44  str(code, mode=D
+000124a0: 4546 4155 4c54 5f4d 4f44 4529 0a20 2020  EFAULT_MODE).   
+000124b0: 2020 2020 2072 6573 756c 745f 6469 6666       result_diff
+000124c0: 203d 2064 6966 6628 636f 6465 2c20 666f   = diff(code, fo
+000124d0: 726d 6174 7465 642c 2022 5354 4449 4e22  rmatted, "STDIN"
+000124e0: 2c20 2253 5444 4f55 5422 290a 0a20 2020  , "STDOUT")..   
+000124f0: 2020 2020 2061 7267 7320 3d20 5b22 2d2d       args = ["--
+00012500: 6469 6666 222c 2022 2d2d 636f 6465 222c  diff", "--code",
+00012510: 2063 6f64 655d 0a20 2020 2020 2020 2072   code].        r
+00012520: 6573 756c 7420 3d20 436c 6952 756e 6e65  esult = CliRunne
+00012530: 7228 292e 696e 766f 6b65 2870 7969 6e6b  r().invoke(pyink
+00012540: 2e6d 6169 6e2c 2061 7267 7329 0a0a 2020  .main, args)..  
+00012550: 2020 2020 2020 2320 5265 6d6f 7665 2074        # Remove t
+00012560: 696d 6520 6672 6f6d 2064 6966 660a 2020  ime from diff.  
+00012570: 2020 2020 2020 6f75 7470 7574 203d 2044        output = D
+00012580: 4946 465f 5449 4d45 2e73 7562 2822 222c  IFF_TIME.sub("",
+00012590: 2072 6573 756c 742e 6f75 7470 7574 290a   result.output).
+000125a0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000125b0: 6f75 7470 7574 203d 3d20 7265 7375 6c74  output == result
+000125c0: 5f64 6966 662c 2022 5468 6520 6f75 7470  _diff, "The outp
+000125d0: 7574 2064 6964 206e 6f74 206d 6174 6368  ut did not match
+000125e0: 2074 6865 2065 7870 6563 7465 6420 7661   the expected va
+000125f0: 6c75 652e 220a 2020 2020 2020 2020 6173  lue.".        as
+00012600: 7365 7274 2072 6573 756c 742e 6578 6974  sert result.exit
+00012610: 5f63 6f64 6520 3d3d 2030 2c20 2254 6865  _code == 0, "The
+00012620: 2065 7869 7420 636f 6465 2069 7320 696e   exit code is in
+00012630: 636f 7272 6563 742e 220a 0a20 2020 2064  correct."..    d
+00012640: 6566 2074 6573 745f 636f 6465 5f6f 7074  ef test_code_opt
+00012650: 696f 6e5f 636f 6c6f 725f 6469 6666 2873  ion_color_diff(s
+00012660: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00012670: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
+00012680: 6520 636f 6465 206f 7074 696f 6e20 7768  e code option wh
+00012690: 656e 2063 6f6c 6f72 2061 6e64 2064 6966  en color and dif
+000126a0: 6620 6172 6520 7061 7373 6564 2e22 2222  f are passed."""
+000126b0: 0a20 2020 2020 2020 2063 6f64 6520 3d20  .        code = 
+000126c0: 2270 7269 6e74 2827 6865 6c6c 6f20 776f  "print('hello wo
+000126d0: 726c 6427 2922 0a20 2020 2020 2020 2066  rld')".        f
+000126e0: 6f72 6d61 7474 6564 203d 2070 7969 6e6b  ormatted = pyink
+000126f0: 2e66 6f72 6d61 745f 7374 7228 636f 6465  .format_str(code
+00012700: 2c20 6d6f 6465 3d44 4546 4155 4c54 5f4d  , mode=DEFAULT_M
+00012710: 4f44 4529 0a0a 2020 2020 2020 2020 7265  ODE)..        re
+00012720: 7375 6c74 5f64 6966 6620 3d20 6469 6666  sult_diff = diff
+00012730: 2863 6f64 652c 2066 6f72 6d61 7474 6564  (code, formatted
+00012740: 2c20 2253 5444 494e 222c 2022 5354 444f  , "STDIN", "STDO
+00012750: 5554 2229 0a20 2020 2020 2020 2072 6573  UT").        res
+00012760: 756c 745f 6469 6666 203d 2063 6f6c 6f72  ult_diff = color
+00012770: 5f64 6966 6628 7265 7375 6c74 5f64 6966  _diff(result_dif
+00012780: 6629 0a0a 2020 2020 2020 2020 6172 6773  f)..        args
+00012790: 203d 205b 222d 2d64 6966 6622 2c20 222d   = ["--diff", "-
+000127a0: 2d63 6f6c 6f72 222c 2022 2d2d 636f 6465  -color", "--code
+000127b0: 222c 2063 6f64 655d 0a20 2020 2020 2020  ", code].       
+000127c0: 2072 6573 756c 7420 3d20 436c 6952 756e   result = CliRun
+000127d0: 6e65 7228 292e 696e 766f 6b65 2870 7969  ner().invoke(pyi
+000127e0: 6e6b 2e6d 6169 6e2c 2061 7267 7329 0a0a  nk.main, args)..
+000127f0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+00012800: 2074 696d 6520 6672 6f6d 2064 6966 660a   time from diff.
+00012810: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00012820: 2044 4946 465f 5449 4d45 2e73 7562 2822   DIFF_TIME.sub("
+00012830: 222c 2072 6573 756c 742e 6f75 7470 7574  ", result.output
+00012840: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00012850: 7420 6f75 7470 7574 203d 3d20 7265 7375  t output == resu
+00012860: 6c74 5f64 6966 662c 2022 5468 6520 6f75  lt_diff, "The ou
+00012870: 7470 7574 2064 6964 206e 6f74 206d 6174  tput did not mat
+00012880: 6368 2074 6865 2065 7870 6563 7465 6420  ch the expected 
+00012890: 7661 6c75 652e 220a 2020 2020 2020 2020  value.".        
+000128a0: 6173 7365 7274 2072 6573 756c 742e 6578  assert result.ex
+000128b0: 6974 5f63 6f64 6520 3d3d 2030 2c20 2254  it_code == 0, "T
+000128c0: 6865 2065 7869 7420 636f 6465 2069 7320  he exit code is 
+000128d0: 696e 636f 7272 6563 742e 220a 0a20 2020  incorrect."..   
+000128e0: 2040 7079 7465 7374 2e6d 6172 6b2e 696e   @pytest.mark.in
+000128f0: 636f 6d70 6174 6962 6c65 5f77 6974 685f  compatible_with_
+00012900: 6d79 7079 630a 2020 2020 6465 6620 7465  mypyc.    def te
+00012910: 7374 5f63 6f64 655f 6f70 7469 6f6e 5f73  st_code_option_s
+00012920: 6166 6528 7365 6c66 2920 2d3e 204e 6f6e  afe(self) -> Non
+00012930: 653a 0a20 2020 2020 2020 2022 2222 5465  e:.        """Te
+00012940: 7374 2074 6861 7420 7468 6520 636f 6465  st that the code
+00012950: 206f 7074 696f 6e20 7468 726f 7773 2061   option throws a
+00012960: 6e20 6572 726f 7220 7768 656e 2074 6865  n error when the
+00012970: 2073 616e 6974 7920 6368 6563 6b73 2066   sanity checks f
+00012980: 6169 6c2e 2222 220a 2020 2020 2020 2020  ail.""".        
+00012990: 2320 5061 7463 6820 7079 696e 6b2e 6173  # Patch pyink.as
+000129a0: 7365 7274 5f65 7175 6976 616c 656e 7420  sert_equivalent 
+000129b0: 746f 2065 6e73 7572 6520 7468 6520 7361  to ensure the sa
+000129c0: 6e69 7479 2063 6865 636b 7320 6661 696c  nity checks fail
+000129d0: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
+000129e0: 7463 682e 6f62 6a65 6374 2870 7969 6e6b  tch.object(pyink
+000129f0: 2c20 2261 7373 6572 745f 6571 7569 7661  , "assert_equiva
+00012a00: 6c65 6e74 222c 2073 6964 655f 6566 6665  lent", side_effe
+00012a10: 6374 3d41 7373 6572 7469 6f6e 4572 726f  ct=AssertionErro
+00012a20: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012a30: 636f 6465 203d 2027 7072 696e 7428 2248  code = 'print("H
+00012a40: 656c 6c6f 2077 6f72 6c64 2229 270a 2020  ello world")'.  
+00012a50: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+00012a60: 6d73 6720 3d20 6622 7b63 6f64 657d 5c6e  msg = f"{code}\n
+00012a70: 6572 726f 723a 2063 616e 6e6f 7420 666f  error: cannot fo
+00012a80: 726d 6174 203c 7374 7269 6e67 3e3a 205c  rmat <string>: \
+00012a90: 6e22 0a0a 2020 2020 2020 2020 2020 2020  n"..            
+00012aa0: 6172 6773 203d 205b 222d 2d73 6166 6522  args = ["--safe"
+00012ab0: 2c20 222d 2d63 6f64 6522 2c20 636f 6465  , "--code", code
+00012ac0: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+00012ad0: 7375 6c74 203d 2043 6c69 5275 6e6e 6572  sult = CliRunner
+00012ae0: 2829 2e69 6e76 6f6b 6528 7079 696e 6b2e  ().invoke(pyink.
+00012af0: 6d61 696e 2c20 6172 6773 290a 0a20 2020  main, args)..   
+00012b00: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00012b10: 6d70 6172 655f 7265 7375 6c74 7328 7265  mpare_results(re
+00012b20: 7375 6c74 2c20 6572 726f 725f 6d73 672c  sult, error_msg,
+00012b30: 2031 3233 290a 0a20 2020 2064 6566 2074   123)..    def t
+00012b40: 6573 745f 636f 6465 5f6f 7074 696f 6e5f  est_code_option_
+00012b50: 6661 7374 2873 656c 6629 202d 3e20 4e6f  fast(self) -> No
+00012b60: 6e65 3a0a 2020 2020 2020 2020 2222 2254  ne:.        """T
+00012b70: 6573 7420 7468 6174 2074 6865 2063 6f64  est that the cod
+00012b80: 6520 6f70 7469 6f6e 2069 676e 6f72 6573  e option ignores
+00012b90: 2065 7272 6f72 7320 7768 656e 2074 6865   errors when the
+00012ba0: 2073 616e 6974 7920 6368 6563 6b73 2066   sanity checks f
+00012bb0: 6169 6c2e 2222 220a 2020 2020 2020 2020  ail.""".        
+00012bc0: 2320 5061 7463 6820 7079 696e 6b2e 6173  # Patch pyink.as
+00012bd0: 7365 7274 5f65 7175 6976 616c 656e 7420  sert_equivalent 
+00012be0: 746f 2065 6e73 7572 6520 7468 6520 7361  to ensure the sa
+00012bf0: 6e69 7479 2063 6865 636b 7320 6661 696c  nity checks fail
+00012c00: 0a20 2020 2020 2020 2077 6974 6820 7061  .        with pa
+00012c10: 7463 682e 6f62 6a65 6374 2870 7969 6e6b  tch.object(pyink
+00012c20: 2c20 2261 7373 6572 745f 6571 7569 7661  , "assert_equiva
+00012c30: 6c65 6e74 222c 2073 6964 655f 6566 6665  lent", side_effe
+00012c40: 6374 3d41 7373 6572 7469 6f6e 4572 726f  ct=AssertionErro
+00012c50: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012c60: 636f 6465 203d 2027 7072 696e 7428 2248  code = 'print("H
+00012c70: 656c 6c6f 2077 6f72 6c64 2229 270a 2020  ello world")'.  
+00012c80: 2020 2020 2020 2020 2020 666f 726d 6174            format
+00012c90: 7465 6420 3d20 7079 696e 6b2e 666f 726d  ted = pyink.form
+00012ca0: 6174 5f73 7472 2863 6f64 652c 206d 6f64  at_str(code, mod
+00012cb0: 653d 4445 4641 554c 545f 4d4f 4445 290a  e=DEFAULT_MODE).
+00012cc0: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00012cd0: 7320 3d20 5b22 2d2d 6661 7374 222c 2022  s = ["--fast", "
+00012ce0: 2d2d 636f 6465 222c 2063 6f64 655d 0a20  --code", code]. 
+00012cf0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00012d00: 7420 3d20 436c 6952 756e 6e65 7228 292e  t = CliRunner().
+00012d10: 696e 766f 6b65 2870 7969 6e6b 2e6d 6169  invoke(pyink.mai
+00012d20: 6e2c 2061 7267 7329 0a0a 2020 2020 2020  n, args)..      
+00012d30: 2020 2020 2020 7365 6c66 2e63 6f6d 7061        self.compa
+00012d40: 7265 5f72 6573 756c 7473 2872 6573 756c  re_results(resul
+00012d50: 742c 2066 6f72 6d61 7474 6564 2c20 3029  t, formatted, 0)
+00012d60: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00012d70: 726b 2e69 6e63 6f6d 7061 7469 626c 655f  rk.incompatible_
+00012d80: 7769 7468 5f6d 7970 7963 0a20 2020 2064  with_mypyc.    d
+00012d90: 6566 2074 6573 745f 636f 6465 5f6f 7074  ef test_code_opt
+00012da0: 696f 6e5f 636f 6e66 6967 2873 656c 6629  ion_config(self)
+00012db0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00012dc0: 2020 2222 220a 2020 2020 2020 2020 5465    """.        Te
+00012dd0: 7374 2074 6861 7420 7468 6520 636f 6465  st that the code
+00012de0: 206f 7074 696f 6e20 6669 6e64 7320 7468   option finds th
+00012df0: 6520 7079 7072 6f6a 6563 742e 746f 6d6c  e pyproject.toml
+00012e00: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00012e10: 6469 7265 6374 6f72 792e 0a20 2020 2020  directory..     
+00012e20: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
+00012e30: 6974 6820 7061 7463 682e 6f62 6a65 6374  ith patch.object
+00012e40: 2870 7969 6e6b 2c20 2270 6172 7365 5f70  (pyink, "parse_p
+00012e50: 7970 726f 6a65 6374 5f74 6f6d 6c22 2c20  yproject_toml", 
+00012e60: 7265 7475 726e 5f76 616c 7565 3d7b 7d29  return_value={})
+00012e70: 2061 7320 7061 7273 653a 0a20 2020 2020   as parse:.     
+00012e80: 2020 2020 2020 2061 7267 7320 3d20 5b22         args = ["
+00012e90: 2d2d 636f 6465 222c 2022 7072 696e 7422  --code", "print"
+00012ea0: 5d0a 2020 2020 2020 2020 2020 2020 2320  ].            # 
+00012eb0: 5468 6973 2069 7320 7468 6520 6f6e 6c79  This is the only
+00012ec0: 2064 6972 6563 746f 7279 206b 6e6f 776e   directory known
+00012ed0: 2074 6f20 636f 6e74 6169 6e20 6120 7079   to contain a py
+00012ee0: 7072 6f6a 6563 742e 746f 6d6c 0a20 2020  project.toml.   
+00012ef0: 2020 2020 2020 2020 2077 6974 6820 6368           with ch
+00012f00: 616e 6765 5f64 6972 6563 746f 7279 2850  ange_directory(P
+00012f10: 524f 4a45 4354 5f52 4f4f 5429 3a0a 2020  ROJECT_ROOT):.  
+00012f20: 2020 2020 2020 2020 2020 2020 2020 436c                Cl
+00012f30: 6952 756e 6e65 7228 292e 696e 766f 6b65  iRunner().invoke
+00012f40: 2870 7969 6e6b 2e6d 6169 6e2c 2061 7267  (pyink.main, arg
+00012f50: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00012f60: 2020 2070 7970 726f 6a65 6374 5f70 6174     pyproject_pat
+00012f70: 6820 3d20 5061 7468 2850 6174 682e 6377  h = Path(Path.cw
+00012f80: 6428 292c 2022 7079 7072 6f6a 6563 742e  d(), "pyproject.
+00012f90: 746f 6d6c 2229 2e72 6573 6f6c 7665 2829  toml").resolve()
+00012fa0: 0a0a 2020 2020 2020 2020 2020 2020 6173  ..            as
+00012fb0: 7365 7274 2028 0a20 2020 2020 2020 2020  sert (.         
+00012fc0: 2020 2020 2020 206c 656e 2870 6172 7365         len(parse
+00012fd0: 2e6d 6f63 6b5f 6361 6c6c 7329 203e 3d20  .mock_calls) >= 
+00012fe0: 310a 2020 2020 2020 2020 2020 2020 292c  1.            ),
+00012ff0: 2022 4578 7065 6374 6564 2063 6f6e 6669   "Expected confi
+00013000: 6720 7061 7273 6520 746f 2062 6520 6361  g parse to be ca
+00013010: 6c6c 6564 2077 6974 6820 7468 6520 6375  lled with the cu
+00013020: 7272 656e 7420 6469 7265 6374 6f72 792e  rrent directory.
+00013030: 220a 0a20 2020 2020 2020 2020 2020 205f  "..            _
+00013040: 2c20 6361 6c6c 5f61 7267 732c 205f 203d  , call_args, _ =
+00013050: 2070 6172 7365 2e6d 6f63 6b5f 6361 6c6c   parse.mock_call
+00013060: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
+00013070: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+00013080: 2020 2020 2020 2020 2020 6361 6c6c 5f61            call_a
+00013090: 7267 735b 305d 2e6c 6f77 6572 2829 203d  rgs[0].lower() =
+000130a0: 3d20 7374 7228 7079 7072 6f6a 6563 745f  = str(pyproject_
+000130b0: 7061 7468 292e 6c6f 7765 7228 290a 2020  path).lower().  
+000130c0: 2020 2020 2020 2020 2020 292c 2022 496e            ), "In
+000130d0: 636f 7272 6563 7420 636f 6e66 6967 206c  correct config l
+000130e0: 6f61 6465 642e 220a 0a20 2020 2040 7079  oaded."..    @py
+000130f0: 7465 7374 2e6d 6172 6b2e 696e 636f 6d70  test.mark.incomp
+00013100: 6174 6962 6c65 5f77 6974 685f 6d79 7079  atible_with_mypy
+00013110: 630a 2020 2020 6465 6620 7465 7374 5f63  c.    def test_c
+00013120: 6f64 655f 6f70 7469 6f6e 5f70 6172 656e  ode_option_paren
+00013130: 745f 636f 6e66 6967 2873 656c 6629 202d  t_config(self) -
+00013140: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00013150: 2222 220a 2020 2020 2020 2020 5465 7374  """.        Test
+00013160: 2074 6861 7420 7468 6520 636f 6465 206f   that the code o
+00013170: 7074 696f 6e20 6669 6e64 7320 7468 6520  ption finds the 
+00013180: 7079 7072 6f6a 6563 742e 746f 6d6c 2069  pyproject.toml i
+00013190: 6e20 7468 6520 7061 7265 6e74 2064 6972  n the parent dir
+000131a0: 6563 746f 7279 2e0a 2020 2020 2020 2020  ectory..        
+000131b0: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
+000131c0: 2070 6174 6368 2e6f 626a 6563 7428 7079   patch.object(py
+000131d0: 696e 6b2c 2022 7061 7273 655f 7079 7072  ink, "parse_pypr
+000131e0: 6f6a 6563 745f 746f 6d6c 222c 2072 6574  oject_toml", ret
+000131f0: 7572 6e5f 7661 6c75 653d 7b7d 2920 6173  urn_value={}) as
+00013200: 2070 6172 7365 3a0a 2020 2020 2020 2020   parse:.        
+00013210: 2020 2020 7769 7468 2063 6861 6e67 655f      with change_
+00013220: 6469 7265 6374 6f72 7928 5448 4953 5f44  directory(THIS_D
+00013230: 4952 293a 0a20 2020 2020 2020 2020 2020  IR):.           
+00013240: 2020 2020 2061 7267 7320 3d20 5b22 2d2d       args = ["--
+00013250: 636f 6465 222c 2022 7072 696e 7422 5d0a  code", "print"].
+00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013270: 436c 6952 756e 6e65 7228 292e 696e 766f  CliRunner().invo
+00013280: 6b65 2870 7969 6e6b 2e6d 6169 6e2c 2061  ke(pyink.main, a
+00013290: 7267 7329 0a0a 2020 2020 2020 2020 2020  rgs)..          
+000132a0: 2020 2020 2020 7079 7072 6f6a 6563 745f        pyproject_
+000132b0: 7061 7468 203d 2050 6174 6828 5061 7468  path = Path(Path
+000132c0: 2829 2e63 7764 2829 2e70 6172 656e 742c  ().cwd().parent,
+000132d0: 2022 7079 7072 6f6a 6563 742e 746f 6d6c   "pyproject.toml
+000132e0: 2229 2e72 6573 6f6c 7665 2829 0a20 2020  ").resolve().   
+000132f0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00013300: 6572 7420 280a 2020 2020 2020 2020 2020  ert (.          
+00013310: 2020 2020 2020 2020 2020 6c65 6e28 7061            len(pa
+00013320: 7273 652e 6d6f 636b 5f63 616c 6c73 2920  rse.mock_calls) 
+00013330: 3e3d 2031 0a20 2020 2020 2020 2020 2020  >= 1.           
+00013340: 2020 2020 2029 2c20 2245 7870 6563 7465       ), "Expecte
+00013350: 6420 636f 6e66 6967 2070 6172 7365 2074  d config parse t
+00013360: 6f20 6265 2063 616c 6c65 6420 7769 7468  o be called with
+00013370: 2074 6865 2063 7572 7265 6e74 2064 6972   the current dir
+00013380: 6563 746f 7279 2e22 0a0a 2020 2020 2020  ectory."..      
+00013390: 2020 2020 2020 2020 2020 5f2c 2063 616c            _, cal
+000133a0: 6c5f 6172 6773 2c20 5f20 3d20 7061 7273  l_args, _ = pars
+000133b0: 652e 6d6f 636b 5f63 616c 6c73 5b30 5d0a  e.mock_calls[0].
+000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133d0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+000133e0: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+000133f0: 6c5f 6172 6773 5b30 5d2e 6c6f 7765 7228  l_args[0].lower(
+00013400: 2920 3d3d 2073 7472 2870 7970 726f 6a65  ) == str(pyproje
+00013410: 6374 5f70 6174 6829 2e6c 6f77 6572 2829  ct_path).lower()
+00013420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013430: 2029 2c20 2249 6e63 6f72 7265 6374 2063   ), "Incorrect c
+00013440: 6f6e 6669 6720 6c6f 6164 6564 2e22 0a0a  onfig loaded."..
+00013450: 2020 2020 6465 6620 7465 7374 5f66 6f72      def test_for
+00013460: 5f68 616e 646c 6564 5f75 6e65 7870 6563  _handled_unexpec
+00013470: 7465 645f 656f 665f 6572 726f 7228 7365  ted_eof_error(se
+00013480: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00013490: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000134a0: 2054 6573 7420 7468 6174 2061 6e20 756e   Test that an un
+000134b0: 6578 7065 6374 6564 2045 4f46 2053 796e  expected EOF Syn
+000134c0: 7461 7845 7272 6f72 2069 7320 6e69 6365  taxError is nice
+000134d0: 6c79 2070 7265 7365 6e74 6564 2e0a 2020  ly presented..  
+000134e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000134f0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00013500: 6973 6573 2870 7969 6e6b 2e70 6172 7369  ises(pyink.parsi
+00013510: 6e67 2e49 6e76 616c 6964 496e 7075 7429  ng.InvalidInput)
+00013520: 2061 7320 6578 635f 696e 666f 3a0a 2020   as exc_info:.  
+00013530: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
+00013540: 6c69 6232 746f 335f 7061 7273 6528 2270  lib2to3_parse("p
+00013550: 7269 6e74 2822 2c20 7b7d 290a 0a20 2020  rint(", {})..   
+00013560: 2020 2020 2065 7863 5f69 6e66 6f2e 6d61       exc_info.ma
+00013570: 7463 6828 2243 616e 6e6f 7420 7061 7273  tch("Cannot pars
+00013580: 653a 2032 3a30 3a20 454f 4620 696e 206d  e: 2:0: EOF in m
+00013590: 756c 7469 2d6c 696e 6520 7374 6174 656d  ulti-line statem
+000135a0: 656e 7422 290a 0a20 2020 2064 6566 2074  ent")..    def t
+000135b0: 6573 745f 6571 7569 7661 6c65 6e63 795f  est_equivalency_
+000135c0: 6173 745f 7061 7273 655f 6661 696c 7572  ast_parse_failur
+000135d0: 655f 696e 636c 7564 6573 5f65 7272 6f72  e_includes_error
+000135e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+000135f0: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+00013600: 6573 742e 7261 6973 6573 2841 7373 6572  est.raises(Asser
+00013610: 7469 6f6e 4572 726f 7229 2061 7320 6572  tionError) as er
+00013620: 723a 0a20 2020 2020 2020 2020 2020 2070  r:.            p
+00013630: 7969 6e6b 2e61 7373 6572 745f 6571 7569  yink.assert_equi
+00013640: 7661 6c65 6e74 2822 61c2 abc2 bb61 2020  valent("a....a  
+00013650: 3d20 3122 2c20 2261 c2ab c2bb 6120 203d  = 1", "a....a  =
+00013660: 2031 2229 0a0a 2020 2020 2020 2020 6572   1")..        er
+00013670: 722e 6d61 7463 6828 222d 2d73 6166 6522  r.match("--safe"
+00013680: 290a 2020 2020 2020 2020 2320 556e 666f  ).        # Unfo
+00013690: 7274 756e 6174 656c 7920 7468 6520 5379  rtunately the Sy
+000136a0: 6e74 6178 4572 726f 7220 6d65 7373 6167  ntaxError messag
+000136b0: 6520 6861 7320 6368 616e 6765 6420 696e  e has changed in
+000136c0: 206e 6577 6572 2076 6572 7369 6f6e 7320   newer versions 
+000136d0: 736f 2077 650a 2020 2020 2020 2020 2320  so we.        # 
+000136e0: 6361 6e27 7420 6d61 7463 6820 6974 2064  can't match it d
+000136f0: 6972 6563 746c 792e 0a20 2020 2020 2020  irectly..       
+00013700: 2065 7272 2e6d 6174 6368 2822 696e 7661   err.match("inva
+00013710: 6c69 6420 6368 6172 6163 7465 7222 290a  lid character").
+00013720: 2020 2020 2020 2020 6572 722e 6d61 7463          err.matc
+00013730: 6828 7222 5c28 3c75 6e6b 6e6f 776e 3e2c  h(r"\(<unknown>,
+00013740: 206c 696e 6520 315c 2922 290a 0a0a 636c   line 1\)")...cl
+00013750: 6173 7320 5465 7374 4361 6368 696e 673a  ass TestCaching:
+00013760: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
+00013770: 745f 6361 6368 655f 6469 7228 0a20 2020  t_cache_dir(.   
+00013780: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00013790: 2020 2074 6d70 5f70 6174 683a 2050 6174     tmp_path: Pat
+000137a0: 682c 0a20 2020 2020 2020 206d 6f6e 6b65  h,.        monke
+000137b0: 7970 6174 6368 3a20 7079 7465 7374 2e4d  ypatch: pytest.M
+000137c0: 6f6e 6b65 7950 6174 6368 2c0a 2020 2020  onkeyPatch,.    
+000137d0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000137e0: 2020 2023 2043 7265 6174 6520 6d75 6c74     # Create mult
+000137f0: 6970 6c65 2063 6163 6865 2064 6972 6563  iple cache direc
+00013800: 746f 7269 6573 0a20 2020 2020 2020 2077  tories.        w
+00013810: 6f72 6b73 7061 6365 3120 3d20 746d 705f  orkspace1 = tmp_
+00013820: 7061 7468 202f 2022 7773 3122 0a20 2020  path / "ws1".   
+00013830: 2020 2020 2077 6f72 6b73 7061 6365 312e       workspace1.
+00013840: 6d6b 6469 7228 290a 2020 2020 2020 2020  mkdir().        
+00013850: 776f 726b 7370 6163 6532 203d 2074 6d70  workspace2 = tmp
+00013860: 5f70 6174 6820 2f20 2277 7332 220a 2020  _path / "ws2".  
+00013870: 2020 2020 2020 776f 726b 7370 6163 6532        workspace2
+00013880: 2e6d 6b64 6972 2829 0a0a 2020 2020 2020  .mkdir()..      
+00013890: 2020 2320 466f 7263 6520 7573 6572 5f63    # Force user_c
+000138a0: 6163 6865 5f64 6972 2074 6f20 7573 6520  ache_dir to use 
+000138b0: 7468 6520 7465 6d70 6f72 6172 7920 6469  the temporary di
+000138c0: 7265 6374 6f72 7920 666f 7220 6561 7369  rectory for easi
+000138d0: 6572 2061 7373 6572 7469 6f6e 730a 2020  er assertions.  
+000138e0: 2020 2020 2020 7061 7463 685f 7573 6572        patch_user
+000138f0: 5f63 6163 6865 5f64 6972 203d 2070 6174  _cache_dir = pat
+00013900: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
+00013910: 7461 7267 6574 3d22 7079 696e 6b2e 6361  target="pyink.ca
+00013920: 6368 652e 7573 6572 5f63 6163 6865 5f64  che.user_cache_d
+00013930: 6972 222c 0a20 2020 2020 2020 2020 2020  ir",.           
+00013940: 2061 7574 6f73 7065 633d 5472 7565 2c0a   autospec=True,.
+00013950: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013960: 726e 5f76 616c 7565 3d73 7472 2877 6f72  rn_value=str(wor
+00013970: 6b73 7061 6365 3129 2c0a 2020 2020 2020  kspace1),.      
+00013980: 2020 290a 0a20 2020 2020 2020 2023 2049    )..        # I
+00013990: 6620 5059 494e 4b5f 4341 4348 455f 4449  f PYINK_CACHE_DI
+000139a0: 5220 6973 206e 6f74 2073 6574 2c20 7573  R is not set, us
+000139b0: 6520 7573 6572 5f63 6163 6865 5f64 6972  e user_cache_dir
+000139c0: 0a20 2020 2020 2020 206d 6f6e 6b65 7970  .        monkeyp
+000139d0: 6174 6368 2e64 656c 656e 7628 2250 5949  atch.delenv("PYI
+000139e0: 4e4b 5f43 4143 4845 5f44 4952 222c 2072  NK_CACHE_DIR", r
+000139f0: 6169 7369 6e67 3d46 616c 7365 290a 2020  aising=False).  
+00013a00: 2020 2020 2020 7769 7468 2070 6174 6368        with patch
+00013a10: 5f75 7365 725f 6361 6368 655f 6469 723a  _user_cache_dir:
+00013a20: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00013a30: 6572 7420 6765 745f 6361 6368 655f 6469  ert get_cache_di
+00013a40: 7228 2920 3d3d 2077 6f72 6b73 7061 6365  r() == workspace
+00013a50: 310a 0a20 2020 2020 2020 2023 2049 6620  1..        # If 
+00013a60: 6974 2069 7320 7365 742c 2075 7365 2074  it is set, use t
+00013a70: 6865 2070 6174 6820 7072 6f76 6964 6564  he path provided
+00013a80: 2069 6e20 7468 6520 656e 7620 7661 722e   in the env var.
+00013a90: 0a20 2020 2020 2020 206d 6f6e 6b65 7970  .        monkeyp
+00013aa0: 6174 6368 2e73 6574 656e 7628 2250 5949  atch.setenv("PYI
+00013ab0: 4e4b 5f43 4143 4845 5f44 4952 222c 2073  NK_CACHE_DIR", s
+00013ac0: 7472 2877 6f72 6b73 7061 6365 3229 290a  tr(workspace2)).
+00013ad0: 2020 2020 2020 2020 6173 7365 7274 2067          assert g
+00013ae0: 6574 5f63 6163 6865 5f64 6972 2829 203d  et_cache_dir() =
+00013af0: 3d20 776f 726b 7370 6163 6532 0a0a 2020  = workspace2..  
+00013b00: 2020 6465 6620 7465 7374 5f63 6163 6865    def test_cache
+00013b10: 5f62 726f 6b65 6e5f 6669 6c65 2873 656c  _broken_file(sel
+00013b20: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00013b30: 2020 2020 6d6f 6465 203d 2044 4546 4155      mode = DEFAU
+00013b40: 4c54 5f4d 4f44 450a 2020 2020 2020 2020  LT_MODE.        
+00013b50: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
+00013b60: 2061 7320 776f 726b 7370 6163 653a 0a20   as workspace:. 
+00013b70: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00013b80: 5f66 696c 6520 3d20 6765 745f 6361 6368  _file = get_cach
+00013b90: 655f 6669 6c65 286d 6f64 6529 0a20 2020  e_file(mode).   
+00013ba0: 2020 2020 2020 2020 2063 6163 6865 5f66           cache_f
+00013bb0: 696c 652e 7772 6974 655f 7465 7874 2822  ile.write_text("
+00013bc0: 7468 6973 2069 7320 6e6f 7420 6120 7069  this is not a pi
+00013bd0: 636b 6c65 2229 0a20 2020 2020 2020 2020  ckle").         
+00013be0: 2020 2061 7373 6572 7420 7079 696e 6b2e     assert pyink.
+00013bf0: 7265 6164 5f63 6163 6865 286d 6f64 6529  read_cache(mode)
+00013c00: 203d 3d20 7b7d 0a20 2020 2020 2020 2020   == {}.         
+00013c10: 2020 2073 7263 203d 2028 776f 726b 7370     src = (worksp
+00013c20: 6163 6520 2f20 2274 6573 742e 7079 2229  ace / "test.py")
+00013c30: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
+00013c40: 2020 2020 2020 2073 7263 2e77 7269 7465         src.write
+00013c50: 5f74 6578 7428 2270 7269 6e74 2827 6865  _text("print('he
+00013c60: 6c6c 6f27 2922 290a 2020 2020 2020 2020  llo')").        
+00013c70: 2020 2020 696e 766f 6b65 426c 6163 6b28      invokeBlack(
+00013c80: 5b73 7472 2873 7263 295d 290a 2020 2020  [str(src)]).    
+00013c90: 2020 2020 2020 2020 6361 6368 6520 3d20          cache = 
+00013ca0: 7079 696e 6b2e 7265 6164 5f63 6163 6865  pyink.read_cache
+00013cb0: 286d 6f64 6529 0a20 2020 2020 2020 2020  (mode).         
+00013cc0: 2020 2061 7373 6572 7420 7374 7228 7372     assert str(sr
+00013cd0: 6329 2069 6e20 6361 6368 650a 0a20 2020  c) in cache..   
+00013ce0: 2064 6566 2074 6573 745f 6361 6368 655f   def test_cache_
+00013cf0: 7369 6e67 6c65 5f66 696c 655f 616c 7265  single_file_alre
+00013d00: 6164 795f 6361 6368 6564 2873 656c 6629  ady_cached(self)
+00013d10: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00013d20: 2020 6d6f 6465 203d 2044 4546 4155 4c54    mode = DEFAULT
+00013d30: 5f4d 4f44 450a 2020 2020 2020 2020 7769  _MODE.        wi
+00013d40: 7468 2063 6163 6865 5f64 6972 2829 2061  th cache_dir() a
+00013d50: 7320 776f 726b 7370 6163 653a 0a20 2020  s workspace:.   
+00013d60: 2020 2020 2020 2020 2073 7263 203d 2028           src = (
+00013d70: 776f 726b 7370 6163 6520 2f20 2274 6573  workspace / "tes
+00013d80: 742e 7079 2229 2e72 6573 6f6c 7665 2829  t.py").resolve()
 00013d90: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00013da0: 203d 2028 776f 726b 7370 6163 6520 2f20   = (workspace / 
-00013db0: 2274 6573 742e 7079 2229 2e72 6573 6f6c  "test.py").resol
-00013dc0: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
-00013dd0: 2073 7263 2e77 7269 7465 5f74 6578 7428   src.write_text(
-00013de0: 2270 7269 6e74 2827 6865 6c6c 6f27 2922  "print('hello')"
-00013df0: 290a 2020 2020 2020 2020 2020 2020 696e  ).            in
-00013e00: 766f 6b65 426c 6163 6b28 5b73 7472 2873  vokeBlack([str(s
-00013e10: 7263 295d 290a 2020 2020 2020 2020 2020  rc)]).          
-00013e20: 2020 6361 6368 6520 3d20 7079 696e 6b2e    cache = pyink.
-00013e30: 7265 6164 5f63 6163 6865 286d 6f64 6529  read_cache(mode)
-00013e40: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00013e50: 6572 7420 7374 7228 7372 6329 2069 6e20  ert str(src) in 
-00013e60: 6361 6368 650a 0a20 2020 2064 6566 2074  cache..    def t
-00013e70: 6573 745f 6361 6368 655f 7369 6e67 6c65  est_cache_single
-00013e80: 5f66 696c 655f 616c 7265 6164 795f 6361  _file_already_ca
-00013e90: 6368 6564 2873 656c 6629 202d 3e20 4e6f  ched(self) -> No
-00013ea0: 6e65 3a0a 2020 2020 2020 2020 6d6f 6465  ne:.        mode
-00013eb0: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
-00013ec0: 2020 2020 2020 2020 7769 7468 2063 6163          with cac
-00013ed0: 6865 5f64 6972 2829 2061 7320 776f 726b  he_dir() as work
-00013ee0: 7370 6163 653a 0a20 2020 2020 2020 2020  space:.         
-00013ef0: 2020 2073 7263 203d 2028 776f 726b 7370     src = (worksp
-00013f00: 6163 6520 2f20 2274 6573 742e 7079 2229  ace / "test.py")
-00013f10: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
-00013f20: 2020 2020 2020 2073 7263 2e77 7269 7465         src.write
-00013f30: 5f74 6578 7428 2270 7269 6e74 2827 6865  _text("print('he
-00013f40: 6c6c 6f27 2922 290a 2020 2020 2020 2020  llo')").        
-00013f50: 2020 2020 7079 696e 6b2e 7772 6974 655f      pyink.write_
-00013f60: 6361 6368 6528 7b7d 2c20 5b73 7263 5d2c  cache({}, [src],
-00013f70: 206d 6f64 6529 0a20 2020 2020 2020 2020   mode).         
-00013f80: 2020 2069 6e76 6f6b 6542 6c61 636b 285b     invokeBlack([
-00013f90: 7374 7228 7372 6329 5d29 0a20 2020 2020  str(src)]).     
-00013fa0: 2020 2020 2020 2061 7373 6572 7420 7372         assert sr
-00013fb0: 632e 7265 6164 5f74 6578 7428 2920 3d3d  c.read_text() ==
-00013fc0: 2022 7072 696e 7428 2768 656c 6c6f 2729   "print('hello')
-00013fd0: 220a 0a20 2020 2040 6576 656e 745f 6c6f  "..    @event_lo
-00013fe0: 6f70 2829 0a20 2020 2064 6566 2074 6573  op().    def tes
-00013ff0: 745f 6361 6368 655f 6d75 6c74 6970 6c65  t_cache_multiple
-00014000: 5f66 696c 6573 2873 656c 6629 202d 3e20  _files(self) -> 
-00014010: 4e6f 6e65 3a0a 2020 2020 2020 2020 6d6f  None:.        mo
-00014020: 6465 203d 2044 4546 4155 4c54 5f4d 4f44  de = DEFAULT_MOD
-00014030: 450a 2020 2020 2020 2020 7769 7468 2063  E.        with c
-00014040: 6163 6865 5f64 6972 2829 2061 7320 776f  ache_dir() as wo
-00014050: 726b 7370 6163 652c 2070 6174 6368 280a  rkspace, patch(.
-00014060: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00014070: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-00014080: 5072 6f63 6573 7350 6f6f 6c45 7865 6375  ProcessPoolExecu
-00014090: 746f 7222 2c20 6e65 773d 5468 7265 6164  tor", new=Thread
-000140a0: 506f 6f6c 4578 6563 7574 6f72 0a20 2020  PoolExecutor.   
-000140b0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-000140c0: 2020 2020 6f6e 6520 3d20 2877 6f72 6b73      one = (works
-000140d0: 7061 6365 202f 2022 6f6e 652e 7079 2229  pace / "one.py")
-000140e0: 2e72 6573 6f6c 7665 2829 0a20 2020 2020  .resolve().     
-000140f0: 2020 2020 2020 2077 6974 6820 6f6e 652e         with one.
-00014100: 6f70 656e 2822 7722 2920 6173 2066 6f62  open("w") as fob
-00014110: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
-00014120: 2020 2066 6f62 6a2e 7772 6974 6528 2270     fobj.write("p
-00014130: 7269 6e74 2827 6865 6c6c 6f27 2922 290a  rint('hello')").
-00014140: 2020 2020 2020 2020 2020 2020 7477 6f20              two 
-00014150: 3d20 2877 6f72 6b73 7061 6365 202f 2022  = (workspace / "
-00014160: 7477 6f2e 7079 2229 2e72 6573 6f6c 7665  two.py").resolve
-00014170: 2829 0a20 2020 2020 2020 2020 2020 2077  ().            w
-00014180: 6974 6820 7477 6f2e 6f70 656e 2822 7722  ith two.open("w"
-00014190: 2920 6173 2066 6f62 6a3a 0a20 2020 2020  ) as fobj:.     
-000141a0: 2020 2020 2020 2020 2020 2066 6f62 6a2e             fobj.
-000141b0: 7772 6974 6528 2270 7269 6e74 2827 6865  write("print('he
-000141c0: 6c6c 6f27 2922 290a 2020 2020 2020 2020  llo')").        
-000141d0: 2020 2020 7079 696e 6b2e 7772 6974 655f      pyink.write_
-000141e0: 6361 6368 6528 7b7d 2c20 5b6f 6e65 5d2c  cache({}, [one],
-000141f0: 206d 6f64 6529 0a20 2020 2020 2020 2020   mode).         
-00014200: 2020 2069 6e76 6f6b 6542 6c61 636b 285b     invokeBlack([
-00014210: 7374 7228 776f 726b 7370 6163 6529 5d29  str(workspace)])
-00014220: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00014230: 6820 6f6e 652e 6f70 656e 2822 7222 2920  h one.open("r") 
-00014240: 6173 2066 6f62 6a3a 0a20 2020 2020 2020  as fobj:.       
-00014250: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00014260: 666f 626a 2e72 6561 6428 2920 3d3d 2022  fobj.read() == "
-00014270: 7072 696e 7428 2768 656c 6c6f 2729 220a  print('hello')".
-00014280: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00014290: 2074 776f 2e6f 7065 6e28 2272 2229 2061   two.open("r") a
-000142a0: 7320 666f 626a 3a0a 2020 2020 2020 2020  s fobj:.        
-000142b0: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
-000142c0: 6f62 6a2e 7265 6164 2829 203d 3d20 2770  obj.read() == 'p
-000142d0: 7269 6e74 2822 6865 6c6c 6f22 295c 6e27  rint("hello")\n'
-000142e0: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
-000142f0: 6865 203d 2070 7969 6e6b 2e72 6561 645f  he = pyink.read_
-00014300: 6361 6368 6528 6d6f 6465 290a 2020 2020  cache(mode).    
-00014310: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00014320: 7472 286f 6e65 2920 696e 2063 6163 6865  tr(one) in cache
-00014330: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00014340: 6572 7420 7374 7228 7477 6f29 2069 6e20  ert str(two) in 
-00014350: 6361 6368 650a 0a20 2020 2040 7079 7465  cache..    @pyte
-00014360: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-00014370: 697a 6528 2263 6f6c 6f72 222c 205b 4661  ize("color", [Fa
-00014380: 6c73 652c 2054 7275 655d 2c20 6964 733d  lse, True], ids=
-00014390: 5b22 6e6f 2d63 6f6c 6f72 222c 2022 7769  ["no-color", "wi
-000143a0: 7468 2d63 6f6c 6f72 225d 290a 2020 2020  th-color"]).    
-000143b0: 6465 6620 7465 7374 5f6e 6f5f 6361 6368  def test_no_cach
-000143c0: 655f 7768 656e 5f77 7269 7465 6261 636b  e_when_writeback
-000143d0: 5f64 6966 6628 7365 6c66 2c20 636f 6c6f  _diff(self, colo
-000143e0: 723a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  r: bool) -> None
-000143f0: 3a0a 2020 2020 2020 2020 6d6f 6465 203d  :.        mode =
-00014400: 2044 4546 4155 4c54 5f4d 4f44 450a 2020   DEFAULT_MODE.  
-00014410: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
-00014420: 5f64 6972 2829 2061 7320 776f 726b 7370  _dir() as worksp
-00014430: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
-00014440: 2073 7263 203d 2028 776f 726b 7370 6163   src = (workspac
-00014450: 6520 2f20 2274 6573 742e 7079 2229 2e72  e / "test.py").r
-00014460: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
-00014470: 2020 2020 2077 6974 6820 7372 632e 6f70       with src.op
-00014480: 656e 2822 7722 2920 6173 2066 6f62 6a3a  en("w") as fobj:
-00014490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000144a0: 2066 6f62 6a2e 7772 6974 6528 2270 7269   fobj.write("pri
-000144b0: 6e74 2827 6865 6c6c 6f27 2922 290a 2020  nt('hello')").  
-000144c0: 2020 2020 2020 2020 2020 7769 7468 2070            with p
-000144d0: 6174 6368 2822 7079 696e 6b2e 7265 6164  atch("pyink.read
-000144e0: 5f63 6163 6865 2229 2061 7320 7265 6164  _cache") as read
-000144f0: 5f63 6163 6865 2c20 7061 7463 6828 0a20  _cache, patch(. 
-00014500: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014510: 7079 696e 6b2e 7772 6974 655f 6361 6368  pyink.write_cach
-00014520: 6522 0a20 2020 2020 2020 2020 2020 2029  e".            )
-00014530: 2061 7320 7772 6974 655f 6361 6368 653a   as write_cache:
-00014540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014550: 2063 6d64 203d 205b 7374 7228 7372 6329   cmd = [str(src)
-00014560: 2c20 222d 2d64 6966 6622 5d0a 2020 2020  , "--diff"].    
-00014570: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00014580: 6f6c 6f72 3a0a 2020 2020 2020 2020 2020  olor:.          
-00014590: 2020 2020 2020 2020 2020 636d 642e 6170            cmd.ap
-000145a0: 7065 6e64 2822 2d2d 636f 6c6f 7222 290a  pend("--color").
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 696e 766f 6b65 426c 6163 6b28 636d 6429  invokeBlack(cmd)
-000145d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000145e0: 2063 6163 6865 5f66 696c 6520 3d20 6765   cache_file = ge
-000145f0: 745f 6361 6368 655f 6669 6c65 286d 6f64  t_cache_file(mod
-00014600: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00014610: 2020 2061 7373 6572 7420 6361 6368 655f     assert cache_
-00014620: 6669 6c65 2e65 7869 7374 7328 2920 6973  file.exists() is
-00014630: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00014640: 2020 2020 2020 2077 7269 7465 5f63 6163         write_cac
-00014650: 6865 2e61 7373 6572 745f 6e6f 745f 6361  he.assert_not_ca
-00014660: 6c6c 6564 2829 0a20 2020 2020 2020 2020  lled().         
-00014670: 2020 2020 2020 2072 6561 645f 6361 6368         read_cach
-00014680: 652e 6173 7365 7274 5f6e 6f74 5f63 616c  e.assert_not_cal
-00014690: 6c65 6428 290a 0a20 2020 2040 7079 7465  led()..    @pyte
-000146a0: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-000146b0: 697a 6528 2263 6f6c 6f72 222c 205b 4661  ize("color", [Fa
-000146c0: 6c73 652c 2054 7275 655d 2c20 6964 733d  lse, True], ids=
-000146d0: 5b22 6e6f 2d63 6f6c 6f72 222c 2022 7769  ["no-color", "wi
-000146e0: 7468 2d63 6f6c 6f72 225d 290a 2020 2020  th-color"]).    
-000146f0: 4065 7665 6e74 5f6c 6f6f 7028 290a 2020  @event_loop().  
-00014700: 2020 6465 6620 7465 7374 5f6f 7574 7075    def test_outpu
-00014710: 745f 6c6f 636b 696e 675f 7768 656e 5f77  t_locking_when_w
-00014720: 7269 7465 6261 636b 5f64 6966 6628 7365  riteback_diff(se
-00014730: 6c66 2c20 636f 6c6f 723a 2062 6f6f 6c29  lf, color: bool)
-00014740: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00014750: 2020 7769 7468 2063 6163 6865 5f64 6972    with cache_dir
-00014760: 2829 2061 7320 776f 726b 7370 6163 653a  () as workspace:
-00014770: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00014780: 2074 6167 2069 6e20 7261 6e67 6528 302c   tag in range(0,
-00014790: 2034 293a 0a20 2020 2020 2020 2020 2020   4):.           
-000147a0: 2020 2020 2073 7263 203d 2028 776f 726b       src = (work
-000147b0: 7370 6163 6520 2f20 6622 7465 7374 7b74  space / f"test{t
-000147c0: 6167 7d2e 7079 2229 2e72 6573 6f6c 7665  ag}.py").resolve
-000147d0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000147e0: 2020 2077 6974 6820 7372 632e 6f70 656e     with src.open
-000147f0: 2822 7722 2920 6173 2066 6f62 6a3a 0a20  ("w") as fobj:. 
-00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014810: 2020 2066 6f62 6a2e 7772 6974 6528 2270     fobj.write("p
-00014820: 7269 6e74 2827 6865 6c6c 6f27 2922 290a  rint('hello')").
-00014830: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00014840: 2070 6174 6368 280a 2020 2020 2020 2020   patch(.        
-00014850: 2020 2020 2020 2020 2270 7969 6e6b 2e63          "pyink.c
-00014860: 6f6e 6375 7272 656e 6379 2e4d 616e 6167  oncurrency.Manag
-00014870: 6572 222c 2077 7261 7073 3d6d 756c 7469  er", wraps=multi
-00014880: 7072 6f63 6573 7369 6e67 2e4d 616e 6167  processing.Manag
-00014890: 6572 0a20 2020 2020 2020 2020 2020 2029  er.            )
-000148a0: 2061 7320 6d67 723a 0a20 2020 2020 2020   as mgr:.       
-000148b0: 2020 2020 2020 2020 2063 6d64 203d 205b           cmd = [
-000148c0: 222d 2d64 6966 6622 2c20 7374 7228 776f  "--diff", str(wo
-000148d0: 726b 7370 6163 6529 5d0a 2020 2020 2020  rkspace)].      
-000148e0: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-000148f0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00014900: 2020 2020 2020 2020 636d 642e 6170 7065          cmd.appe
-00014910: 6e64 2822 2d2d 636f 6c6f 7222 290a 2020  nd("--color").  
-00014920: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00014930: 766f 6b65 426c 6163 6b28 636d 642c 2065  vokeBlack(cmd, e
-00014940: 7869 745f 636f 6465 3d30 290a 2020 2020  xit_code=0).    
-00014950: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-00014960: 6973 2069 736e 2774 2071 7569 7465 2064  is isn't quite d
-00014970: 6f69 6e67 2077 6861 7420 7765 2077 616e  oing what we wan
-00014980: 742c 2062 7574 2069 6620 6974 205f 6973  t, but if it _is
-00014990: 6e27 745f 0a20 2020 2020 2020 2020 2020  n't_.           
-000149a0: 2020 2020 2023 2063 616c 6c65 6420 7468       # called th
-000149b0: 656e 2077 6520 6361 6e6e 6f74 2062 6520  en we cannot be 
-000149c0: 7573 696e 6720 7468 6520 6c6f 636b 2069  using the lock i
-000149d0: 7420 7072 6f76 6964 6573 0a20 2020 2020  t provides.     
-000149e0: 2020 2020 2020 2020 2020 206d 6772 2e61             mgr.a
-000149f0: 7373 6572 745f 6361 6c6c 6564 2829 0a0a  ssert_called()..
-00014a00: 2020 2020 6465 6620 7465 7374 5f6e 6f5f      def test_no_
-00014a10: 6361 6368 655f 7768 656e 5f73 7464 696e  cache_when_stdin
-00014a20: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00014a30: 2020 2020 2020 2020 6d6f 6465 203d 2044          mode = D
-00014a40: 4546 4155 4c54 5f4d 4f44 450a 2020 2020  EFAULT_MODE.    
-00014a50: 2020 2020 7769 7468 2063 6163 6865 5f64      with cache_d
-00014a60: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
-00014a70: 2020 7265 7375 6c74 203d 2043 6c69 5275    result = CliRu
-00014a80: 6e6e 6572 2829 2e69 6e76 6f6b 6528 0a20  nner().invoke(. 
-00014a90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00014aa0: 7969 6e6b 2e6d 6169 6e2c 205b 222d 225d  yink.main, ["-"]
-00014ab0: 2c20 696e 7075 743d 4279 7465 7349 4f28  , input=BytesIO(
-00014ac0: 6222 7072 696e 7428 2768 656c 6c6f 2729  b"print('hello')
-00014ad0: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
-00014ae0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00014af0: 6572 7420 6e6f 7420 7265 7375 6c74 2e65  ert not result.e
-00014b00: 7869 745f 636f 6465 0a20 2020 2020 2020  xit_code.       
-00014b10: 2020 2020 2063 6163 6865 5f66 696c 6520       cache_file 
-00014b20: 3d20 6765 745f 6361 6368 655f 6669 6c65  = get_cache_file
-00014b30: 286d 6f64 6529 0a20 2020 2020 2020 2020  (mode).         
-00014b40: 2020 2061 7373 6572 7420 6e6f 7420 6361     assert not ca
-00014b50: 6368 655f 6669 6c65 2e65 7869 7374 7328  che_file.exists(
-00014b60: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00014b70: 7265 6164 5f63 6163 6865 5f6e 6f5f 6361  read_cache_no_ca
-00014b80: 6368 6566 696c 6528 7365 6c66 2920 2d3e  chefile(self) ->
-00014b90: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
-00014ba0: 6f64 6520 3d20 4445 4641 554c 545f 4d4f  ode = DEFAULT_MO
-00014bb0: 4445 0a20 2020 2020 2020 2077 6974 6820  DE.        with 
-00014bc0: 6361 6368 655f 6469 7228 293a 0a20 2020  cache_dir():.   
-00014bd0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00014be0: 7079 696e 6b2e 7265 6164 5f63 6163 6865  pyink.read_cache
-00014bf0: 286d 6f64 6529 203d 3d20 7b7d 0a0a 2020  (mode) == {}..  
-00014c00: 2020 6465 6620 7465 7374 5f77 7269 7465    def test_write
-00014c10: 5f63 6163 6865 5f72 6561 645f 6361 6368  _cache_read_cach
-00014c20: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-00014c30: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
-00014c40: 4445 4641 554c 545f 4d4f 4445 0a20 2020  DEFAULT_MODE.   
-00014c50: 2020 2020 2077 6974 6820 6361 6368 655f       with cache_
-00014c60: 6469 7228 2920 6173 2077 6f72 6b73 7061  dir() as workspa
-00014c70: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00014c80: 7372 6320 3d20 2877 6f72 6b73 7061 6365  src = (workspace
-00014c90: 202f 2022 7465 7374 2e70 7922 292e 7265   / "test.py").re
+00013da0: 2e77 7269 7465 5f74 6578 7428 2270 7269  .write_text("pri
+00013db0: 6e74 2827 6865 6c6c 6f27 2922 290a 2020  nt('hello')").  
+00013dc0: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
+00013dd0: 7772 6974 655f 6361 6368 6528 7b7d 2c20  write_cache({}, 
+00013de0: 5b73 7263 5d2c 206d 6f64 6529 0a20 2020  [src], mode).   
+00013df0: 2020 2020 2020 2020 2069 6e76 6f6b 6542           invokeB
+00013e00: 6c61 636b 285b 7374 7228 7372 6329 5d29  lack([str(src)])
+00013e10: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00013e20: 6572 7420 7372 632e 7265 6164 5f74 6578  ert src.read_tex
+00013e30: 7428 2920 3d3d 2022 7072 696e 7428 2768  t() == "print('h
+00013e40: 656c 6c6f 2729 220a 0a20 2020 2040 6576  ello')"..    @ev
+00013e50: 656e 745f 6c6f 6f70 2829 0a20 2020 2064  ent_loop().    d
+00013e60: 6566 2074 6573 745f 6361 6368 655f 6d75  ef test_cache_mu
+00013e70: 6c74 6970 6c65 5f66 696c 6573 2873 656c  ltiple_files(sel
+00013e80: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00013e90: 2020 2020 6d6f 6465 203d 2044 4546 4155      mode = DEFAU
+00013ea0: 4c54 5f4d 4f44 450a 2020 2020 2020 2020  LT_MODE.        
+00013eb0: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
+00013ec0: 2061 7320 776f 726b 7370 6163 652c 2070   as workspace, p
+00013ed0: 6174 6368 280a 2020 2020 2020 2020 2020  atch(.          
+00013ee0: 2020 2263 6f6e 6375 7272 656e 742e 6675    "concurrent.fu
+00013ef0: 7475 7265 732e 5072 6f63 6573 7350 6f6f  tures.ProcessPoo
+00013f00: 6c45 7865 6375 746f 7222 2c20 6e65 773d  lExecutor", new=
+00013f10: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+00013f20: 6f72 0a20 2020 2020 2020 2029 3a0a 2020  or.        ):.  
+00013f30: 2020 2020 2020 2020 2020 6f6e 6520 3d20            one = 
+00013f40: 2877 6f72 6b73 7061 6365 202f 2022 6f6e  (workspace / "on
+00013f50: 652e 7079 2229 2e72 6573 6f6c 7665 2829  e.py").resolve()
+00013f60: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00013f70: 6820 6f6e 652e 6f70 656e 2822 7722 2920  h one.open("w") 
+00013f80: 6173 2066 6f62 6a3a 0a20 2020 2020 2020  as fobj:.       
+00013f90: 2020 2020 2020 2020 2066 6f62 6a2e 7772           fobj.wr
+00013fa0: 6974 6528 2270 7269 6e74 2827 6865 6c6c  ite("print('hell
+00013fb0: 6f27 2922 290a 2020 2020 2020 2020 2020  o')").          
+00013fc0: 2020 7477 6f20 3d20 2877 6f72 6b73 7061    two = (workspa
+00013fd0: 6365 202f 2022 7477 6f2e 7079 2229 2e72  ce / "two.py").r
+00013fe0: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
+00013ff0: 2020 2020 2077 6974 6820 7477 6f2e 6f70       with two.op
+00014000: 656e 2822 7722 2920 6173 2066 6f62 6a3a  en("w") as fobj:
+00014010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014020: 2066 6f62 6a2e 7772 6974 6528 2270 7269   fobj.write("pri
+00014030: 6e74 2827 6865 6c6c 6f27 2922 290a 2020  nt('hello')").  
+00014040: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
+00014050: 7772 6974 655f 6361 6368 6528 7b7d 2c20  write_cache({}, 
+00014060: 5b6f 6e65 5d2c 206d 6f64 6529 0a20 2020  [one], mode).   
+00014070: 2020 2020 2020 2020 2069 6e76 6f6b 6542           invokeB
+00014080: 6c61 636b 285b 7374 7228 776f 726b 7370  lack([str(worksp
+00014090: 6163 6529 5d29 0a20 2020 2020 2020 2020  ace)]).         
+000140a0: 2020 2077 6974 6820 6f6e 652e 6f70 656e     with one.open
+000140b0: 2822 7222 2920 6173 2066 6f62 6a3a 0a20  ("r") as fobj:. 
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000140d0: 7373 6572 7420 666f 626a 2e72 6561 6428  ssert fobj.read(
+000140e0: 2920 3d3d 2022 7072 696e 7428 2768 656c  ) == "print('hel
+000140f0: 6c6f 2729 220a 2020 2020 2020 2020 2020  lo')".          
+00014100: 2020 7769 7468 2074 776f 2e6f 7065 6e28    with two.open(
+00014110: 2272 2229 2061 7320 666f 626a 3a0a 2020  "r") as fobj:.  
+00014120: 2020 2020 2020 2020 2020 2020 2020 6173                as
+00014130: 7365 7274 2066 6f62 6a2e 7265 6164 2829  sert fobj.read()
+00014140: 203d 3d20 2770 7269 6e74 2822 6865 6c6c   == 'print("hell
+00014150: 6f22 295c 6e27 0a20 2020 2020 2020 2020  o")\n'.         
+00014160: 2020 2063 6163 6865 203d 2070 7969 6e6b     cache = pyink
+00014170: 2e72 6561 645f 6361 6368 6528 6d6f 6465  .read_cache(mode
+00014180: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
+00014190: 7365 7274 2073 7472 286f 6e65 2920 696e  sert str(one) in
+000141a0: 2063 6163 6865 0a20 2020 2020 2020 2020   cache.         
+000141b0: 2020 2061 7373 6572 7420 7374 7228 7477     assert str(tw
+000141c0: 6f29 2069 6e20 6361 6368 650a 0a20 2020  o) in cache..   
+000141d0: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
+000141e0: 7261 6d65 7472 697a 6528 2263 6f6c 6f72  rametrize("color
+000141f0: 222c 205b 4661 6c73 652c 2054 7275 655d  ", [False, True]
+00014200: 2c20 6964 733d 5b22 6e6f 2d63 6f6c 6f72  , ids=["no-color
+00014210: 222c 2022 7769 7468 2d63 6f6c 6f72 225d  ", "with-color"]
+00014220: 290a 2020 2020 6465 6620 7465 7374 5f6e  ).    def test_n
+00014230: 6f5f 6361 6368 655f 7768 656e 5f77 7269  o_cache_when_wri
+00014240: 7465 6261 636b 5f64 6966 6628 7365 6c66  teback_diff(self
+00014250: 2c20 636f 6c6f 723a 2062 6f6f 6c29 202d  , color: bool) -
+00014260: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00014270: 6d6f 6465 203d 2044 4546 4155 4c54 5f4d  mode = DEFAULT_M
+00014280: 4f44 450a 2020 2020 2020 2020 7769 7468  ODE.        with
+00014290: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
+000142a0: 776f 726b 7370 6163 653a 0a20 2020 2020  workspace:.     
+000142b0: 2020 2020 2020 2073 7263 203d 2028 776f         src = (wo
+000142c0: 726b 7370 6163 6520 2f20 2274 6573 742e  rkspace / "test.
+000142d0: 7079 2229 2e72 6573 6f6c 7665 2829 0a20  py").resolve(). 
+000142e0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000142f0: 7372 632e 6f70 656e 2822 7722 2920 6173  src.open("w") as
+00014300: 2066 6f62 6a3a 0a20 2020 2020 2020 2020   fobj:.         
+00014310: 2020 2020 2020 2066 6f62 6a2e 7772 6974         fobj.writ
+00014320: 6528 2270 7269 6e74 2827 6865 6c6c 6f27  e("print('hello'
+00014330: 2922 290a 2020 2020 2020 2020 2020 2020  )").            
+00014340: 7769 7468 2070 6174 6368 2822 7079 696e  with patch("pyin
+00014350: 6b2e 7265 6164 5f63 6163 6865 2229 2061  k.read_cache") a
+00014360: 7320 7265 6164 5f63 6163 6865 2c20 7061  s read_cache, pa
+00014370: 7463 6828 0a20 2020 2020 2020 2020 2020  tch(.           
+00014380: 2020 2020 2022 7079 696e 6b2e 7772 6974       "pyink.writ
+00014390: 655f 6361 6368 6522 0a20 2020 2020 2020  e_cache".       
+000143a0: 2020 2020 2029 2061 7320 7772 6974 655f       ) as write_
+000143b0: 6361 6368 653a 0a20 2020 2020 2020 2020  cache:.         
+000143c0: 2020 2020 2020 2063 6d64 203d 205b 7374         cmd = [st
+000143d0: 7228 7372 6329 2c20 222d 2d64 6966 6622  r(src), "--diff"
+000143e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000143f0: 2020 6966 2063 6f6c 6f72 3a0a 2020 2020    if color:.    
+00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014410: 636d 642e 6170 7065 6e64 2822 2d2d 636f  cmd.append("--co
+00014420: 6c6f 7222 290a 2020 2020 2020 2020 2020  lor").          
+00014430: 2020 2020 2020 696e 766f 6b65 426c 6163        invokeBlac
+00014440: 6b28 636d 6429 0a20 2020 2020 2020 2020  k(cmd).         
+00014450: 2020 2020 2020 2063 6163 6865 5f66 696c         cache_fil
+00014460: 6520 3d20 6765 745f 6361 6368 655f 6669  e = get_cache_fi
+00014470: 6c65 286d 6f64 6529 0a20 2020 2020 2020  le(mode).       
+00014480: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00014490: 6361 6368 655f 6669 6c65 2e65 7869 7374  cache_file.exist
+000144a0: 7328 2920 6973 2046 616c 7365 0a20 2020  s() is False.   
+000144b0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+000144c0: 7465 5f63 6163 6865 2e61 7373 6572 745f  te_cache.assert_
+000144d0: 6e6f 745f 6361 6c6c 6564 2829 0a20 2020  not_called().   
+000144e0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+000144f0: 645f 6361 6368 652e 6173 7365 7274 5f6e  d_cache.assert_n
+00014500: 6f74 5f63 616c 6c65 6428 290a 0a20 2020  ot_called()..   
+00014510: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
+00014520: 7261 6d65 7472 697a 6528 2263 6f6c 6f72  rametrize("color
+00014530: 222c 205b 4661 6c73 652c 2054 7275 655d  ", [False, True]
+00014540: 2c20 6964 733d 5b22 6e6f 2d63 6f6c 6f72  , ids=["no-color
+00014550: 222c 2022 7769 7468 2d63 6f6c 6f72 225d  ", "with-color"]
+00014560: 290a 2020 2020 4065 7665 6e74 5f6c 6f6f  ).    @event_loo
+00014570: 7028 290a 2020 2020 6465 6620 7465 7374  p().    def test
+00014580: 5f6f 7574 7075 745f 6c6f 636b 696e 675f  _output_locking_
+00014590: 7768 656e 5f77 7269 7465 6261 636b 5f64  when_writeback_d
+000145a0: 6966 6628 7365 6c66 2c20 636f 6c6f 723a  iff(self, color:
+000145b0: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+000145c0: 2020 2020 2020 2020 7769 7468 2063 6163          with cac
+000145d0: 6865 5f64 6972 2829 2061 7320 776f 726b  he_dir() as work
+000145e0: 7370 6163 653a 0a20 2020 2020 2020 2020  space:.         
+000145f0: 2020 2066 6f72 2074 6167 2069 6e20 7261     for tag in ra
+00014600: 6e67 6528 302c 2034 293a 0a20 2020 2020  nge(0, 4):.     
+00014610: 2020 2020 2020 2020 2020 2073 7263 203d             src =
+00014620: 2028 776f 726b 7370 6163 6520 2f20 6622   (workspace / f"
+00014630: 7465 7374 7b74 6167 7d2e 7079 2229 2e72  test{tag}.py").r
+00014640: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
+00014650: 2020 2020 2020 2020 2077 6974 6820 7372           with sr
+00014660: 632e 6f70 656e 2822 7722 2920 6173 2066  c.open("w") as f
+00014670: 6f62 6a3a 0a20 2020 2020 2020 2020 2020  obj:.           
+00014680: 2020 2020 2020 2020 2066 6f62 6a2e 7772           fobj.wr
+00014690: 6974 6528 2270 7269 6e74 2827 6865 6c6c  ite("print('hell
+000146a0: 6f27 2922 290a 2020 2020 2020 2020 2020  o')").          
+000146b0: 2020 7769 7468 2070 6174 6368 280a 2020    with patch(.  
+000146c0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000146d0: 7969 6e6b 2e63 6f6e 6375 7272 656e 6379  yink.concurrency
+000146e0: 2e4d 616e 6167 6572 222c 2077 7261 7073  .Manager", wraps
+000146f0: 3d6d 756c 7469 7072 6f63 6573 7369 6e67  =multiprocessing
+00014700: 2e4d 616e 6167 6572 0a20 2020 2020 2020  .Manager.       
+00014710: 2020 2020 2029 2061 7320 6d67 723a 0a20       ) as mgr:. 
+00014720: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014730: 6d64 203d 205b 222d 2d64 6966 6622 2c20  md = ["--diff", 
+00014740: 7374 7228 776f 726b 7370 6163 6529 5d0a  str(workspace)].
+00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014760: 6966 2063 6f6c 6f72 3a0a 2020 2020 2020  if color:.      
+00014770: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00014780: 642e 6170 7065 6e64 2822 2d2d 636f 6c6f  d.append("--colo
+00014790: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
+000147a0: 2020 2020 696e 766f 6b65 426c 6163 6b28      invokeBlack(
+000147b0: 636d 642c 2065 7869 745f 636f 6465 3d30  cmd, exit_code=0
+000147c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000147d0: 2020 2320 7468 6973 2069 736e 2774 2071    # this isn't q
+000147e0: 7569 7465 2064 6f69 6e67 2077 6861 7420  uite doing what 
+000147f0: 7765 2077 616e 742c 2062 7574 2069 6620  we want, but if 
+00014800: 6974 205f 6973 6e27 745f 0a20 2020 2020  it _isn't_.     
+00014810: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
+00014820: 6c65 6420 7468 656e 2077 6520 6361 6e6e  led then we cann
+00014830: 6f74 2062 6520 7573 696e 6720 7468 6520  ot be using the 
+00014840: 6c6f 636b 2069 7420 7072 6f76 6964 6573  lock it provides
+00014850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014860: 206d 6772 2e61 7373 6572 745f 6361 6c6c   mgr.assert_call
+00014870: 6564 2829 0a0a 2020 2020 6465 6620 7465  ed()..    def te
+00014880: 7374 5f6e 6f5f 6361 6368 655f 7768 656e  st_no_cache_when
+00014890: 5f73 7464 696e 2873 656c 6629 202d 3e20  _stdin(self) -> 
+000148a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6d6f  None:.        mo
+000148b0: 6465 203d 2044 4546 4155 4c54 5f4d 4f44  de = DEFAULT_MOD
+000148c0: 450a 2020 2020 2020 2020 7769 7468 2063  E.        with c
+000148d0: 6163 6865 5f64 6972 2829 3a0a 2020 2020  ache_dir():.    
+000148e0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000148f0: 2043 6c69 5275 6e6e 6572 2829 2e69 6e76   CliRunner().inv
+00014900: 6f6b 6528 0a20 2020 2020 2020 2020 2020  oke(.           
+00014910: 2020 2020 2070 7969 6e6b 2e6d 6169 6e2c       pyink.main,
+00014920: 205b 222d 225d 2c20 696e 7075 743d 4279   ["-"], input=By
+00014930: 7465 7349 4f28 6222 7072 696e 7428 2768  tesIO(b"print('h
+00014940: 656c 6c6f 2729 2229 0a20 2020 2020 2020  ello')").       
+00014950: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014960: 2020 2061 7373 6572 7420 6e6f 7420 7265     assert not re
+00014970: 7375 6c74 2e65 7869 745f 636f 6465 0a20  sult.exit_code. 
+00014980: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00014990: 5f66 696c 6520 3d20 6765 745f 6361 6368  _file = get_cach
+000149a0: 655f 6669 6c65 286d 6f64 6529 0a20 2020  e_file(mode).   
+000149b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000149c0: 6e6f 7420 6361 6368 655f 6669 6c65 2e65  not cache_file.e
+000149d0: 7869 7374 7328 290a 0a20 2020 2064 6566  xists()..    def
+000149e0: 2074 6573 745f 7265 6164 5f63 6163 6865   test_read_cache
+000149f0: 5f6e 6f5f 6361 6368 6566 696c 6528 7365  _no_cachefile(se
+00014a00: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00014a10: 2020 2020 206d 6f64 6520 3d20 4445 4641       mode = DEFA
+00014a20: 554c 545f 4d4f 4445 0a20 2020 2020 2020  ULT_MODE.       
+00014a30: 2077 6974 6820 6361 6368 655f 6469 7228   with cache_dir(
+00014a40: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00014a50: 7373 6572 7420 7079 696e 6b2e 7265 6164  ssert pyink.read
+00014a60: 5f63 6163 6865 286d 6f64 6529 203d 3d20  _cache(mode) == 
+00014a70: 7b7d 0a0a 2020 2020 6465 6620 7465 7374  {}..    def test
+00014a80: 5f77 7269 7465 5f63 6163 6865 5f72 6561  _write_cache_rea
+00014a90: 645f 6361 6368 6528 7365 6c66 2920 2d3e  d_cache(self) ->
+00014aa0: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
+00014ab0: 6f64 6520 3d20 4445 4641 554c 545f 4d4f  ode = DEFAULT_MO
+00014ac0: 4445 0a20 2020 2020 2020 2077 6974 6820  DE.        with 
+00014ad0: 6361 6368 655f 6469 7228 2920 6173 2077  cache_dir() as w
+00014ae0: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
+00014af0: 2020 2020 2020 7372 6320 3d20 2877 6f72        src = (wor
+00014b00: 6b73 7061 6365 202f 2022 7465 7374 2e70  kspace / "test.p
+00014b10: 7922 292e 7265 736f 6c76 6528 290a 2020  y").resolve().  
+00014b20: 2020 2020 2020 2020 2020 7372 632e 746f            src.to
+00014b30: 7563 6828 290a 2020 2020 2020 2020 2020  uch().          
+00014b40: 2020 7079 696e 6b2e 7772 6974 655f 6361    pyink.write_ca
+00014b50: 6368 6528 7b7d 2c20 5b73 7263 5d2c 206d  che({}, [src], m
+00014b60: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
+00014b70: 2063 6163 6865 203d 2070 7969 6e6b 2e72   cache = pyink.r
+00014b80: 6561 645f 6361 6368 6528 6d6f 6465 290a  ead_cache(mode).
+00014b90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00014ba0: 7274 2073 7472 2873 7263 2920 696e 2063  rt str(src) in c
+00014bb0: 6163 6865 0a20 2020 2020 2020 2020 2020  ache.           
+00014bc0: 2061 7373 6572 7420 6361 6368 655b 7374   assert cache[st
+00014bd0: 7228 7372 6329 5d20 3d3d 2070 7969 6e6b  r(src)] == pyink
+00014be0: 2e67 6574 5f63 6163 6865 5f69 6e66 6f28  .get_cache_info(
+00014bf0: 7372 6329 0a0a 2020 2020 6465 6620 7465  src)..    def te
+00014c00: 7374 5f66 696c 7465 725f 6361 6368 6564  st_filter_cached
+00014c10: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00014c20: 2020 2020 2020 2020 7769 7468 2054 656d          with Tem
+00014c30: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
+00014c40: 2920 6173 2077 6f72 6b73 7061 6365 3a0a  ) as workspace:.
+00014c50: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00014c60: 203d 2050 6174 6828 776f 726b 7370 6163   = Path(workspac
+00014c70: 6529 0a20 2020 2020 2020 2020 2020 2075  e).            u
+00014c80: 6e63 6163 6865 6420 3d20 2870 6174 6820  ncached = (path 
+00014c90: 2f20 2275 6e63 6163 6865 6422 292e 7265  / "uncached").re
 00014ca0: 736f 6c76 6528 290a 2020 2020 2020 2020  solve().        
-00014cb0: 2020 2020 7372 632e 746f 7563 6828 290a      src.touch().
-00014cc0: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
-00014cd0: 6b2e 7772 6974 655f 6361 6368 6528 7b7d  k.write_cache({}
-00014ce0: 2c20 5b73 7263 5d2c 206d 6f64 6529 0a20  , [src], mode). 
-00014cf0: 2020 2020 2020 2020 2020 2063 6163 6865             cache
-00014d00: 203d 2070 7969 6e6b 2e72 6561 645f 6361   = pyink.read_ca
-00014d10: 6368 6528 6d6f 6465 290a 2020 2020 2020  che(mode).      
-00014d20: 2020 2020 2020 6173 7365 7274 2073 7472        assert str
-00014d30: 2873 7263 2920 696e 2063 6163 6865 0a20  (src) in cache. 
-00014d40: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00014d50: 7420 6361 6368 655b 7374 7228 7372 6329  t cache[str(src)
-00014d60: 5d20 3d3d 2070 7969 6e6b 2e67 6574 5f63  ] == pyink.get_c
-00014d70: 6163 6865 5f69 6e66 6f28 7372 6329 0a0a  ache_info(src)..
-00014d80: 2020 2020 6465 6620 7465 7374 5f66 696c      def test_fil
-00014d90: 7465 725f 6361 6368 6564 2873 656c 6629  ter_cached(self)
-00014da0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00014db0: 2020 7769 7468 2054 656d 706f 7261 7279    with Temporary
-00014dc0: 4469 7265 6374 6f72 7928 2920 6173 2077  Directory() as w
-00014dd0: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
-00014de0: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
-00014df0: 6828 776f 726b 7370 6163 6529 0a20 2020  h(workspace).   
-00014e00: 2020 2020 2020 2020 2075 6e63 6163 6865           uncache
-00014e10: 6420 3d20 2870 6174 6820 2f20 2275 6e63  d = (path / "unc
-00014e20: 6163 6865 6422 292e 7265 736f 6c76 6528  ached").resolve(
-00014e30: 290a 2020 2020 2020 2020 2020 2020 6361  ).            ca
-00014e40: 6368 6564 203d 2028 7061 7468 202f 2022  ched = (path / "
-00014e50: 6361 6368 6564 2229 2e72 6573 6f6c 7665  cached").resolve
-00014e60: 2829 0a20 2020 2020 2020 2020 2020 2063  ().            c
-00014e70: 6163 6865 645f 6275 745f 6368 616e 6765  ached_but_change
-00014e80: 6420 3d20 2870 6174 6820 2f20 2263 6861  d = (path / "cha
-00014e90: 6e67 6564 2229 2e72 6573 6f6c 7665 2829  nged").resolve()
-00014ea0: 0a20 2020 2020 2020 2020 2020 2075 6e63  .            unc
-00014eb0: 6163 6865 642e 746f 7563 6828 290a 2020  ached.touch().  
-00014ec0: 2020 2020 2020 2020 2020 6361 6368 6564            cached
-00014ed0: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
-00014ee0: 2020 2020 2063 6163 6865 645f 6275 745f       cached_but_
-00014ef0: 6368 616e 6765 642e 746f 7563 6828 290a  changed.touch().
-00014f00: 2020 2020 2020 2020 2020 2020 6361 6368              cach
-00014f10: 6520 3d20 7b0a 2020 2020 2020 2020 2020  e = {.          
-00014f20: 2020 2020 2020 7374 7228 6361 6368 6564        str(cached
-00014f30: 293a 2070 7969 6e6b 2e67 6574 5f63 6163  ): pyink.get_cac
-00014f40: 6865 5f69 6e66 6f28 6361 6368 6564 292c  he_info(cached),
-00014f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f60: 2073 7472 2863 6163 6865 645f 6275 745f   str(cached_but_
-00014f70: 6368 616e 6765 6429 3a20 2830 2e30 2c20  changed): (0.0, 
-00014f80: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-00014f90: 7d0a 2020 2020 2020 2020 2020 2020 746f  }.            to
-00014fa0: 646f 2c20 646f 6e65 203d 2070 7969 6e6b  do, done = pyink
-00014fb0: 2e63 6163 6865 2e66 696c 7465 725f 6361  .cache.filter_ca
-00014fc0: 6368 6564 280a 2020 2020 2020 2020 2020  ched(.          
-00014fd0: 2020 2020 2020 6361 6368 652c 207b 756e        cache, {un
-00014fe0: 6361 6368 6564 2c20 6361 6368 6564 2c20  cached, cached, 
-00014ff0: 6361 6368 6564 5f62 7574 5f63 6861 6e67  cached_but_chang
-00015000: 6564 7d0a 2020 2020 2020 2020 2020 2020  ed}.            
-00015010: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-00015020: 7365 7274 2074 6f64 6f20 3d3d 207b 756e  sert todo == {un
-00015030: 6361 6368 6564 2c20 6361 6368 6564 5f62  cached, cached_b
-00015040: 7574 5f63 6861 6e67 6564 7d0a 2020 2020  ut_changed}.    
-00015050: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00015060: 6f6e 6520 3d3d 207b 6361 6368 6564 7d0a  one == {cached}.
-00015070: 0a20 2020 2064 6566 2074 6573 745f 7772  .    def test_wr
-00015080: 6974 655f 6361 6368 655f 6372 6561 7465  ite_cache_create
-00015090: 735f 6469 7265 6374 6f72 795f 6966 5f6e  s_directory_if_n
-000150a0: 6565 6465 6428 7365 6c66 2920 2d3e 204e  eeded(self) -> N
-000150b0: 6f6e 653a 0a20 2020 2020 2020 206d 6f64  one:.        mod
-000150c0: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
-000150d0: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
-000150e0: 6368 655f 6469 7228 6578 6973 7473 3d46  che_dir(exists=F
-000150f0: 616c 7365 2920 6173 2077 6f72 6b73 7061  alse) as workspa
-00015100: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-00015110: 6173 7365 7274 206e 6f74 2077 6f72 6b73  assert not works
-00015120: 7061 6365 2e65 7869 7374 7328 290a 2020  pace.exists().  
-00015130: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
-00015140: 7772 6974 655f 6361 6368 6528 7b7d 2c20  write_cache({}, 
-00015150: 5b5d 2c20 6d6f 6465 290a 2020 2020 2020  [], mode).      
-00015160: 2020 2020 2020 6173 7365 7274 2077 6f72        assert wor
-00015170: 6b73 7061 6365 2e65 7869 7374 7328 290a  kspace.exists().
-00015180: 0a20 2020 2040 6576 656e 745f 6c6f 6f70  .    @event_loop
-00015190: 2829 0a20 2020 2064 6566 2074 6573 745f  ().    def test_
-000151a0: 6661 696c 6564 5f66 6f72 6d61 7474 696e  failed_formattin
-000151b0: 675f 646f 6573 5f6e 6f74 5f67 6574 5f63  g_does_not_get_c
-000151c0: 6163 6865 6428 7365 6c66 2920 2d3e 204e  ached(self) -> N
-000151d0: 6f6e 653a 0a20 2020 2020 2020 206d 6f64  one:.        mod
-000151e0: 6520 3d20 4445 4641 554c 545f 4d4f 4445  e = DEFAULT_MODE
-000151f0: 0a20 2020 2020 2020 2077 6974 6820 6361  .        with ca
-00015200: 6368 655f 6469 7228 2920 6173 2077 6f72  che_dir() as wor
-00015210: 6b73 7061 6365 2c20 7061 7463 6828 0a20  kspace, patch(. 
-00015220: 2020 2020 2020 2020 2020 2022 636f 6e63             "conc
-00015230: 7572 7265 6e74 2e66 7574 7572 6573 2e50  urrent.futures.P
-00015240: 726f 6365 7373 506f 6f6c 4578 6563 7574  rocessPoolExecut
-00015250: 6f72 222c 206e 6577 3d54 6872 6561 6450  or", new=ThreadP
-00015260: 6f6f 6c45 7865 6375 746f 720a 2020 2020  oolExecutor.    
-00015270: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00015280: 2020 2066 6169 6c69 6e67 203d 2028 776f     failing = (wo
-00015290: 726b 7370 6163 6520 2f20 2266 6169 6c69  rkspace / "faili
-000152a0: 6e67 2e70 7922 292e 7265 736f 6c76 6528  ng.py").resolve(
-000152b0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-000152c0: 7468 2066 6169 6c69 6e67 2e6f 7065 6e28  th failing.open(
-000152d0: 2277 2229 2061 7320 666f 626a 3a0a 2020  "w") as fobj:.  
-000152e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000152f0: 626a 2e77 7269 7465 2822 6e6f 7420 6163  bj.write("not ac
-00015300: 7475 616c 6c79 2070 7974 686f 6e22 290a  tually python").
-00015310: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-00015320: 6e20 3d20 2877 6f72 6b73 7061 6365 202f  n = (workspace /
-00015330: 2022 636c 6561 6e2e 7079 2229 2e72 6573   "clean.py").res
-00015340: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
-00015350: 2020 2077 6974 6820 636c 6561 6e2e 6f70     with clean.op
-00015360: 656e 2822 7722 2920 6173 2066 6f62 6a3a  en("w") as fobj:
-00015370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015380: 2066 6f62 6a2e 7772 6974 6528 2770 7269   fobj.write('pri
-00015390: 6e74 2822 6865 6c6c 6f22 295c 6e27 290a  nt("hello")\n').
-000153a0: 2020 2020 2020 2020 2020 2020 696e 766f              invo
-000153b0: 6b65 426c 6163 6b28 5b73 7472 2877 6f72  keBlack([str(wor
-000153c0: 6b73 7061 6365 295d 2c20 6578 6974 5f63  kspace)], exit_c
-000153d0: 6f64 653d 3132 3329 0a20 2020 2020 2020  ode=123).       
-000153e0: 2020 2020 2063 6163 6865 203d 2070 7969       cache = pyi
-000153f0: 6e6b 2e72 6561 645f 6361 6368 6528 6d6f  nk.read_cache(mo
-00015400: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-00015410: 6173 7365 7274 2073 7472 2866 6169 6c69  assert str(faili
-00015420: 6e67 2920 6e6f 7420 696e 2063 6163 6865  ng) not in cache
-00015430: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00015440: 6572 7420 7374 7228 636c 6561 6e29 2069  ert str(clean) i
-00015450: 6e20 6361 6368 650a 0a20 2020 2064 6566  n cache..    def
-00015460: 2074 6573 745f 7772 6974 655f 6361 6368   test_write_cach
-00015470: 655f 7772 6974 655f 6661 696c 2873 656c  e_write_fail(sel
-00015480: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00015490: 2020 2020 6d6f 6465 203d 2044 4546 4155      mode = DEFAU
-000154a0: 4c54 5f4d 4f44 450a 2020 2020 2020 2020  LT_MODE.        
-000154b0: 7769 7468 2063 6163 6865 5f64 6972 2829  with cache_dir()
-000154c0: 2c20 7061 7463 682e 6f62 6a65 6374 2850  , patch.object(P
-000154d0: 6174 682c 2022 6f70 656e 2229 2061 7320  ath, "open") as 
-000154e0: 6d6f 636b 3a0a 2020 2020 2020 2020 2020  mock:.          
-000154f0: 2020 6d6f 636b 2e73 6964 655f 6566 6665    mock.side_effe
-00015500: 6374 203d 204f 5345 7272 6f72 0a20 2020  ct = OSError.   
-00015510: 2020 2020 2020 2020 2070 7969 6e6b 2e77           pyink.w
-00015520: 7269 7465 5f63 6163 6865 287b 7d2c 205b  rite_cache({}, [
-00015530: 5d2c 206d 6f64 6529 0a0a 2020 2020 6465  ], mode)..    de
-00015540: 6620 7465 7374 5f72 6561 645f 6361 6368  f test_read_cach
-00015550: 655f 6c69 6e65 5f6c 656e 6774 6873 2873  e_line_lengths(s
-00015560: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00015570: 2020 2020 2020 6d6f 6465 203d 2044 4546        mode = DEF
-00015580: 4155 4c54 5f4d 4f44 450a 2020 2020 2020  AULT_MODE.      
-00015590: 2020 7368 6f72 745f 6d6f 6465 203d 2072    short_mode = r
-000155a0: 6570 6c61 6365 2844 4546 4155 4c54 5f4d  eplace(DEFAULT_M
-000155b0: 4f44 452c 206c 696e 655f 6c65 6e67 7468  ODE, line_length
-000155c0: 3d31 290a 2020 2020 2020 2020 7769 7468  =1).        with
-000155d0: 2063 6163 6865 5f64 6972 2829 2061 7320   cache_dir() as 
-000155e0: 776f 726b 7370 6163 653a 0a20 2020 2020  workspace:.     
-000155f0: 2020 2020 2020 2070 6174 6820 3d20 2877         path = (w
-00015600: 6f72 6b73 7061 6365 202f 2022 6669 6c65  orkspace / "file
-00015610: 2e70 7922 292e 7265 736f 6c76 6528 290a  .py").resolve().
-00015620: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00015630: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
-00015640: 2020 2020 2070 7969 6e6b 2e77 7269 7465       pyink.write
-00015650: 5f63 6163 6865 287b 7d2c 205b 7061 7468  _cache({}, [path
-00015660: 5d2c 206d 6f64 6529 0a20 2020 2020 2020  ], mode).       
-00015670: 2020 2020 206f 6e65 203d 2070 7969 6e6b       one = pyink
-00015680: 2e72 6561 645f 6361 6368 6528 6d6f 6465  .read_cache(mode
-00015690: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-000156a0: 7365 7274 2073 7472 2870 6174 6829 2069  sert str(path) i
-000156b0: 6e20 6f6e 650a 2020 2020 2020 2020 2020  n one.          
-000156c0: 2020 7477 6f20 3d20 7079 696e 6b2e 7265    two = pyink.re
-000156d0: 6164 5f63 6163 6865 2873 686f 7274 5f6d  ad_cache(short_m
-000156e0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
-000156f0: 2061 7373 6572 7420 7374 7228 7061 7468   assert str(path
-00015700: 2920 6e6f 7420 696e 2074 776f 0a0a 0a64  ) not in two...d
-00015710: 6566 2061 7373 6572 745f 636f 6c6c 6563  ef assert_collec
-00015720: 7465 645f 736f 7572 6365 7328 0a20 2020  ted_sources(.   
-00015730: 2073 7263 3a20 5365 7175 656e 6365 5b55   src: Sequence[U
-00015740: 6e69 6f6e 5b73 7472 2c20 5061 7468 5d5d  nion[str, Path]]
-00015750: 2c0a 2020 2020 6578 7065 6374 6564 3a20  ,.    expected: 
-00015760: 5365 7175 656e 6365 5b55 6e69 6f6e 5b73  Sequence[Union[s
-00015770: 7472 2c20 5061 7468 5d5d 2c0a 2020 2020  tr, Path]],.    
-00015780: 2a2c 0a20 2020 2063 7478 3a20 4f70 7469  *,.    ctx: Opti
-00015790: 6f6e 616c 5b46 616b 6543 6f6e 7465 7874  onal[FakeContext
-000157a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
-000157b0: 636c 7564 653a 204f 7074 696f 6e61 6c5b  clude: Optional[
-000157c0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000157d0: 2069 6e63 6c75 6465 3a20 4f70 7469 6f6e   include: Option
-000157e0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-000157f0: 2020 2020 6578 7465 6e64 5f65 7863 6c75      extend_exclu
-00015800: 6465 3a20 4f70 7469 6f6e 616c 5b73 7472  de: Optional[str
-00015810: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 666f  ] = None,.    fo
-00015820: 7263 655f 6578 636c 7564 653a 204f 7074  rce_exclude: Opt
-00015830: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00015840: 652c 0a20 2020 2073 7464 696e 5f66 696c  e,.    stdin_fil
-00015850: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
-00015860: 7374 725d 203d 204e 6f6e 652c 0a29 202d  str] = None,.) -
-00015870: 3e20 4e6f 6e65 3a0a 2020 2020 6773 5f73  > None:.    gs_s
-00015880: 7263 203d 2074 7570 6c65 2873 7472 2850  rc = tuple(str(P
-00015890: 6174 6828 7329 2920 666f 7220 7320 696e  ath(s)) for s in
-000158a0: 2073 7263 290a 2020 2020 6773 5f65 7870   src).    gs_exp
-000158b0: 6563 7465 6420 3d20 5b50 6174 6828 7329  ected = [Path(s)
-000158c0: 2066 6f72 2073 2069 6e20 6578 7065 6374   for s in expect
-000158d0: 6564 5d0a 2020 2020 6773 5f65 7863 6c75  ed].    gs_exclu
-000158e0: 6465 203d 204e 6f6e 6520 6966 2065 7863  de = None if exc
-000158f0: 6c75 6465 2069 7320 4e6f 6e65 2065 6c73  lude is None els
-00015900: 6520 636f 6d70 696c 655f 7061 7474 6572  e compile_patter
-00015910: 6e28 6578 636c 7564 6529 0a20 2020 2067  n(exclude).    g
-00015920: 735f 696e 636c 7564 6520 3d20 4445 4641  s_include = DEFA
-00015930: 554c 545f 494e 434c 5544 4520 6966 2069  ULT_INCLUDE if i
-00015940: 6e63 6c75 6465 2069 7320 4e6f 6e65 2065  nclude is None e
-00015950: 6c73 6520 636f 6d70 696c 655f 7061 7474  lse compile_patt
-00015960: 6572 6e28 696e 636c 7564 6529 0a20 2020  ern(include).   
-00015970: 2067 735f 6578 7465 6e64 5f65 7863 6c75   gs_extend_exclu
-00015980: 6465 203d 2028 0a20 2020 2020 2020 204e  de = (.        N
-00015990: 6f6e 6520 6966 2065 7874 656e 645f 6578  one if extend_ex
-000159a0: 636c 7564 6520 6973 204e 6f6e 6520 656c  clude is None el
-000159b0: 7365 2063 6f6d 7069 6c65 5f70 6174 7465  se compile_patte
-000159c0: 726e 2865 7874 656e 645f 6578 636c 7564  rn(extend_exclud
-000159d0: 6529 0a20 2020 2029 0a20 2020 2067 735f  e).    ).    gs_
-000159e0: 666f 7263 655f 6578 636c 7564 6520 3d20  force_exclude = 
-000159f0: 4e6f 6e65 2069 6620 666f 7263 655f 6578  None if force_ex
-00015a00: 636c 7564 6520 6973 204e 6f6e 6520 656c  clude is None el
-00015a10: 7365 2063 6f6d 7069 6c65 5f70 6174 7465  se compile_patte
-00015a20: 726e 2866 6f72 6365 5f65 7863 6c75 6465  rn(force_exclude
-00015a30: 290a 2020 2020 636f 6c6c 6563 7465 6420  ).    collected 
-00015a40: 3d20 7079 696e 6b2e 6765 745f 736f 7572  = pyink.get_sour
-00015a50: 6365 7328 0a20 2020 2020 2020 2063 7478  ces(.        ctx
-00015a60: 3d63 7478 206f 7220 4661 6b65 436f 6e74  =ctx or FakeCont
-00015a70: 6578 7428 292c 0a20 2020 2020 2020 2073  ext(),.        s
-00015a80: 7263 3d67 735f 7372 632c 0a20 2020 2020  rc=gs_src,.     
-00015a90: 2020 2071 7569 6574 3d46 616c 7365 2c0a     quiet=False,.
-00015aa0: 2020 2020 2020 2020 7665 7262 6f73 653d          verbose=
-00015ab0: 4661 6c73 652c 0a20 2020 2020 2020 2069  False,.        i
-00015ac0: 6e63 6c75 6465 3d67 735f 696e 636c 7564  nclude=gs_includ
-00015ad0: 652c 0a20 2020 2020 2020 2065 7863 6c75  e,.        exclu
-00015ae0: 6465 3d67 735f 6578 636c 7564 652c 0a20  de=gs_exclude,. 
-00015af0: 2020 2020 2020 2065 7874 656e 645f 6578         extend_ex
-00015b00: 636c 7564 653d 6773 5f65 7874 656e 645f  clude=gs_extend_
-00015b10: 6578 636c 7564 652c 0a20 2020 2020 2020  exclude,.       
-00015b20: 2066 6f72 6365 5f65 7863 6c75 6465 3d67   force_exclude=g
-00015b30: 735f 666f 7263 655f 6578 636c 7564 652c  s_force_exclude,
-00015b40: 0a20 2020 2020 2020 2072 6570 6f72 743d  .        report=
-00015b50: 7079 696e 6b2e 5265 706f 7274 2829 2c0a  pyink.Report(),.
-00015b60: 2020 2020 2020 2020 7374 6469 6e5f 6669          stdin_fi
-00015b70: 6c65 6e61 6d65 3d73 7464 696e 5f66 696c  lename=stdin_fil
-00015b80: 656e 616d 652c 0a20 2020 2029 0a20 2020  ename,.    ).   
-00015b90: 2061 7373 6572 7420 736f 7274 6564 2863   assert sorted(c
-00015ba0: 6f6c 6c65 6374 6564 2920 3d3d 2073 6f72  ollected) == sor
-00015bb0: 7465 6428 6773 5f65 7870 6563 7465 6429  ted(gs_expected)
-00015bc0: 0a0a 0a63 6c61 7373 2054 6573 7446 696c  ...class TestFil
-00015bd0: 6543 6f6c 6c65 6374 696f 6e3a 0a20 2020  eCollection:.   
-00015be0: 2064 6566 2074 6573 745f 696e 636c 7564   def test_includ
-00015bf0: 655f 6578 636c 7564 6528 7365 6c66 2920  e_exclude(self) 
-00015c00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015c10: 2070 6174 6820 3d20 5448 4953 5f44 4952   path = THIS_DIR
-00015c20: 202f 2022 6461 7461 2220 2f20 2269 6e63   / "data" / "inc
-00015c30: 6c75 6465 5f65 7863 6c75 6465 5f74 6573  lude_exclude_tes
-00015c40: 7473 220a 2020 2020 2020 2020 7372 6320  ts".        src 
-00015c50: 3d20 5b70 6174 685d 0a20 2020 2020 2020  = [path].       
-00015c60: 2065 7870 6563 7465 6420 3d20 5b0a 2020   expected = [.  
-00015c70: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
-00015c80: 6174 6820 2f20 2262 2f64 6f6e 745f 6578  ath / "b/dont_ex
-00015c90: 636c 7564 652f 612e 7079 2229 2c0a 2020  clude/a.py"),.  
-00015ca0: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
-00015cb0: 6174 6820 2f20 2262 2f64 6f6e 745f 6578  ath / "b/dont_ex
-00015cc0: 636c 7564 652f 612e 7079 6922 292c 0a20  clude/a.pyi"),. 
-00015cd0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00015ce0: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00015cf0: 645f 736f 7572 6365 7328 0a20 2020 2020  d_sources(.     
-00015d00: 2020 2020 2020 2073 7263 2c0a 2020 2020         src,.    
-00015d10: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00015d20: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-00015d30: 636c 7564 653d 7222 5c2e 7079 693f 2422  clude=r"\.pyi?$"
-00015d40: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-00015d50: 636c 7564 653d 7222 2f65 7863 6c75 6465  clude=r"/exclude
-00015d60: 2f7c 2f5c 2e64 6566 696e 6974 656c 795f  /|/\.definitely_
-00015d70: 6578 636c 7564 652f 222c 0a20 2020 2020  exclude/",.     
-00015d80: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-00015d90: 7374 5f67 6974 6967 6e6f 7265 5f75 7365  st_gitignore_use
-00015da0: 645f 6173 5f64 6566 6175 6c74 2873 656c  d_as_default(sel
-00015db0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00015dc0: 2020 2020 6261 7365 203d 2050 6174 6828      base = Path(
-00015dd0: 4441 5441 5f44 4952 202f 2022 696e 636c  DATA_DIR / "incl
-00015de0: 7564 655f 6578 636c 7564 655f 7465 7374  ude_exclude_test
-00015df0: 7322 290a 2020 2020 2020 2020 6578 7065  s").        expe
-00015e00: 6374 6564 203d 205b 0a20 2020 2020 2020  cted = [.       
-00015e10: 2020 2020 2062 6173 6520 2f20 2262 2f2e       base / "b/.
-00015e20: 6465 6669 6e69 7465 6c79 5f65 7863 6c75  definitely_exclu
-00015e30: 6465 2f61 2e70 7922 2c0a 2020 2020 2020  de/a.py",.      
-00015e40: 2020 2020 2020 6261 7365 202f 2022 622f        base / "b/
-00015e50: 2e64 6566 696e 6974 656c 795f 6578 636c  .definitely_excl
-00015e60: 7564 652f 612e 7079 6922 2c0a 2020 2020  ude/a.pyi",.    
-00015e70: 2020 2020 5d0a 2020 2020 2020 2020 7372      ].        sr
-00015e80: 6320 3d20 5b62 6173 6520 2f20 2262 2f22  c = [base / "b/"
-00015e90: 5d0a 2020 2020 2020 2020 6374 7820 3d20  ].        ctx = 
-00015ea0: 4661 6b65 436f 6e74 6578 7428 290a 2020  FakeContext().  
-00015eb0: 2020 2020 2020 6374 782e 6f62 6a5b 2272        ctx.obj["r
-00015ec0: 6f6f 7422 5d20 3d20 6261 7365 0a20 2020  oot"] = base.   
-00015ed0: 2020 2020 2061 7373 6572 745f 636f 6c6c       assert_coll
-00015ee0: 6563 7465 645f 736f 7572 6365 7328 7372  ected_sources(sr
-00015ef0: 632c 2065 7870 6563 7465 642c 2063 7478  c, expected, ctx
-00015f00: 3d63 7478 2c20 6578 7465 6e64 5f65 7863  =ctx, extend_exc
-00015f10: 6c75 6465 3d72 222f 6578 636c 7564 652f  lude=r"/exclude/
-00015f20: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-00015f30: 5f67 6974 6967 6e6f 7265 5f75 7365 645f  _gitignore_used_
-00015f40: 6f6e 5f6d 756c 7469 706c 655f 736f 7572  on_multiple_sour
-00015f50: 6365 7328 7365 6c66 2920 2d3e 204e 6f6e  ces(self) -> Non
-00015f60: 653a 0a20 2020 2020 2020 2072 6f6f 7420  e:.        root 
-00015f70: 3d20 5061 7468 2844 4154 415f 4449 5220  = Path(DATA_DIR 
-00015f80: 2f20 2267 6974 6967 6e6f 7265 5f75 7365  / "gitignore_use
-00015f90: 645f 6f6e 5f6d 756c 7469 706c 655f 736f  d_on_multiple_so
-00015fa0: 7572 6365 7322 290a 2020 2020 2020 2020  urces").        
-00015fb0: 6578 7065 6374 6564 203d 205b 0a20 2020  expected = [.   
-00015fc0: 2020 2020 2020 2020 2072 6f6f 7420 2f20           root / 
-00015fd0: 2264 6972 3122 202f 2022 622e 7079 222c  "dir1" / "b.py",
-00015fe0: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
-00015ff0: 7420 2f20 2264 6972 3222 202f 2022 622e  t / "dir2" / "b.
-00016000: 7079 222c 0a20 2020 2020 2020 205d 0a20  py",.        ]. 
-00016010: 2020 2020 2020 2063 7478 203d 2046 616b         ctx = Fak
-00016020: 6543 6f6e 7465 7874 2829 0a20 2020 2020  eContext().     
-00016030: 2020 2063 7478 2e6f 626a 5b22 726f 6f74     ctx.obj["root
-00016040: 225d 203d 2072 6f6f 740a 2020 2020 2020  "] = root.      
-00016050: 2020 7372 6320 3d20 5b72 6f6f 7420 2f20    src = [root / 
-00016060: 2264 6972 3122 2c20 726f 6f74 202f 2022  "dir1", root / "
-00016070: 6469 7232 225d 0a20 2020 2020 2020 2061  dir2"].        a
-00016080: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
-00016090: 736f 7572 6365 7328 7372 632c 2065 7870  sources(src, exp
-000160a0: 6563 7465 642c 2063 7478 3d63 7478 290a  ected, ctx=ctx).
-000160b0: 0a20 2020 2040 7061 7463 6828 2270 7969  .    @patch("pyi
-000160c0: 6e6b 2e66 696e 645f 7072 6f6a 6563 745f  nk.find_project_
-000160d0: 726f 6f74 222c 206c 616d 6264 6120 2a61  root", lambda *a
-000160e0: 7267 733a 2028 5448 4953 5f44 4952 2e72  rgs: (THIS_DIR.r
-000160f0: 6573 6f6c 7665 2829 2c20 4e6f 6e65 2929  esolve(), None))
-00016100: 0a20 2020 2064 6566 2074 6573 745f 6578  .    def test_ex
-00016110: 636c 7564 655f 666f 725f 6973 7375 655f  clude_for_issue_
-00016120: 3135 3732 2873 656c 6629 202d 3e20 4e6f  1572(self) -> No
-00016130: 6e65 3a0a 2020 2020 2020 2020 2320 4578  ne:.        # Ex
-00016140: 636c 7564 6520 7368 6f75 6c64 6e27 7420  clude shouldn't 
-00016150: 746f 7563 6820 6669 6c65 7320 7468 6174  touch files that
-00016160: 2077 6572 6520 6578 706c 6963 6974 6c79   were explicitly
-00016170: 2067 6976 656e 2074 6f20 426c 6163 6b20   given to Black 
-00016180: 7468 726f 7567 6820 7468 650a 2020 2020  through the.    
-00016190: 2020 2020 2320 434c 492e 2045 7863 6c75      # CLI. Exclu
-000161a0: 6465 2069 7320 7375 7070 6f73 6564 2074  de is supposed t
-000161b0: 6f20 6f6e 6c79 2061 7070 6c79 2074 6f20  o only apply to 
-000161c0: 7468 6520 7265 6375 7273 6976 6520 6469  the recursive di
-000161d0: 7363 6f76 6572 7920 6f66 2066 696c 6573  scovery of files
-000161e0: 2e0a 2020 2020 2020 2020 2320 6874 7470  ..        # http
-000161f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00016200: 7366 2f62 6c61 636b 2f69 7373 7565 732f  sf/black/issues/
-00016210: 3135 3732 0a20 2020 2020 2020 2070 6174  1572.        pat
-00016220: 6820 3d20 4441 5441 5f44 4952 202f 2022  h = DATA_DIR / "
-00016230: 696e 636c 7564 655f 6578 636c 7564 655f  include_exclude_
-00016240: 7465 7374 7322 0a20 2020 2020 2020 2073  tests".        s
-00016250: 7263 203d 205b 7061 7468 202f 2022 622f  rc = [path / "b/
-00016260: 6578 636c 7564 652f 612e 7079 225d 0a20  exclude/a.py"]. 
-00016270: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
-00016280: 3d20 5b70 6174 6820 2f20 2262 2f65 7863  = [path / "b/exc
-00016290: 6c75 6465 2f61 2e70 7922 5d0a 2020 2020  lude/a.py"].    
-000162a0: 2020 2020 6173 7365 7274 5f63 6f6c 6c65      assert_colle
-000162b0: 6374 6564 5f73 6f75 7263 6573 2873 7263  cted_sources(src
-000162c0: 2c20 6578 7065 6374 6564 2c20 696e 636c  , expected, incl
-000162d0: 7564 653d 2222 2c20 6578 636c 7564 653d  ude="", exclude=
-000162e0: 7222 2f65 7863 6c75 6465 2f7c 615c 2e70  r"/exclude/|a\.p
-000162f0: 7922 290a 0a20 2020 2064 6566 2074 6573  y")..    def tes
-00016300: 745f 6769 7469 676e 6f72 655f 6578 636c  t_gitignore_excl
-00016310: 7564 6528 7365 6c66 2920 2d3e 204e 6f6e  ude(self) -> Non
-00016320: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
-00016330: 3d20 5448 4953 5f44 4952 202f 2022 6461  = THIS_DIR / "da
-00016340: 7461 2220 2f20 2269 6e63 6c75 6465 5f65  ta" / "include_e
-00016350: 7863 6c75 6465 5f74 6573 7473 220a 2020  xclude_tests".  
-00016360: 2020 2020 2020 696e 636c 7564 6520 3d20        include = 
-00016370: 7265 2e63 6f6d 7069 6c65 2872 225c 2e70  re.compile(r"\.p
-00016380: 7969 3f24 2229 0a20 2020 2020 2020 2065  yi?$").        e
-00016390: 7863 6c75 6465 203d 2072 652e 636f 6d70  xclude = re.comp
-000163a0: 696c 6528 7222 2229 0a20 2020 2020 2020  ile(r"").       
-000163b0: 2072 6570 6f72 7420 3d20 7079 696e 6b2e   report = pyink.
-000163c0: 5265 706f 7274 2829 0a20 2020 2020 2020  Report().       
-000163d0: 2067 6974 6967 6e6f 7265 203d 2050 6174   gitignore = Pat
-000163e0: 6853 7065 632e 6672 6f6d 5f6c 696e 6573  hSpec.from_lines
-000163f0: 280a 2020 2020 2020 2020 2020 2020 2267  (.            "g
-00016400: 6974 7769 6c64 6d61 7463 6822 2c20 5b22  itwildmatch", ["
-00016410: 6578 636c 7564 652f 222c 2022 2e64 6566  exclude/", ".def
-00016420: 696e 6974 656c 795f 6578 636c 7564 6522  initely_exclude"
-00016430: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-00016440: 2020 2020 736f 7572 6365 733a 204c 6973      sources: Lis
-00016450: 745b 5061 7468 5d20 3d20 5b5d 0a20 2020  t[Path] = [].   
-00016460: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
-00016470: 5b0a 2020 2020 2020 2020 2020 2020 5061  [.            Pa
-00016480: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
-00016490: 745f 6578 636c 7564 652f 612e 7079 2229  t_exclude/a.py")
-000164a0: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
-000164b0: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
-000164c0: 745f 6578 636c 7564 652f 612e 7079 6922  t_exclude/a.pyi"
-000164d0: 292c 0a20 2020 2020 2020 205d 0a20 2020  ),.        ].   
-000164e0: 2020 2020 2074 6869 735f 6162 7320 3d20       this_abs = 
-000164f0: 5448 4953 5f44 4952 2e72 6573 6f6c 7665  THIS_DIR.resolve
-00016500: 2829 0a20 2020 2020 2020 2073 6f75 7263  ().        sourc
-00016510: 6573 2e65 7874 656e 6428 0a20 2020 2020  es.extend(.     
-00016520: 2020 2020 2020 2070 7969 6e6b 2e67 656e         pyink.gen
-00016530: 5f70 7974 686f 6e5f 6669 6c65 7328 0a20  _python_files(. 
-00016540: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00016550: 6174 682e 6974 6572 6469 7228 292c 0a20  ath.iterdir(),. 
-00016560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00016570: 6869 735f 6162 732c 0a20 2020 2020 2020  his_abs,.       
-00016580: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00016590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000165a0: 2020 6578 636c 7564 652c 0a20 2020 2020    exclude,.     
-000165b0: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-000165c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165d0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000165e0: 2020 2020 2020 2072 6570 6f72 742c 0a20         report,. 
-000165f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00016600: 7061 7468 3a20 6769 7469 676e 6f72 657d  path: gitignore}
-00016610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016620: 2020 7665 7262 6f73 653d 4661 6c73 652c    verbose=False,
-00016630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016640: 2071 7569 6574 3d46 616c 7365 2c0a 2020   quiet=False,.  
-00016650: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00016660: 2020 2020 290a 2020 2020 2020 2020 6173      ).        as
-00016670: 7365 7274 2073 6f72 7465 6428 6578 7065  sert sorted(expe
-00016680: 6374 6564 2920 3d3d 2073 6f72 7465 6428  cted) == sorted(
-00016690: 736f 7572 6365 7329 0a0a 2020 2020 6465  sources)..    de
-000166a0: 6620 7465 7374 5f6e 6573 7465 645f 6769  f test_nested_gi
-000166b0: 7469 676e 6f72 6528 7365 6c66 2920 2d3e  tignore(self) ->
-000166c0: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-000166d0: 6174 6820 3d20 5061 7468 2854 4849 535f  ath = Path(THIS_
-000166e0: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
-000166f0: 6e65 7374 6564 5f67 6974 6967 6e6f 7265  nested_gitignore
-00016700: 5f74 6573 7473 2229 0a20 2020 2020 2020  _tests").       
-00016710: 2069 6e63 6c75 6465 203d 2072 652e 636f   include = re.co
-00016720: 6d70 696c 6528 7222 5c2e 7079 693f 2422  mpile(r"\.pyi?$"
-00016730: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
-00016740: 6520 3d20 7265 2e63 6f6d 7069 6c65 2872  e = re.compile(r
-00016750: 2222 290a 2020 2020 2020 2020 726f 6f74  "").        root
-00016760: 5f67 6974 6967 6e6f 7265 203d 2070 7969  _gitignore = pyi
-00016770: 6e6b 2e66 696c 6573 2e67 6574 5f67 6974  nk.files.get_git
-00016780: 6967 6e6f 7265 2870 6174 6829 0a20 2020  ignore(path).   
-00016790: 2020 2020 2072 6570 6f72 7420 3d20 7079       report = py
-000167a0: 696e 6b2e 5265 706f 7274 2829 0a20 2020  ink.Report().   
-000167b0: 2020 2020 2065 7870 6563 7465 643a 204c       expected: L
-000167c0: 6973 745b 5061 7468 5d20 3d20 5b0a 2020  ist[Path] = [.  
-000167d0: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
-000167e0: 6174 6820 2f20 2278 2e70 7922 292c 0a20  ath / "x.py"),. 
-000167f0: 2020 2020 2020 2020 2020 2050 6174 6828             Path(
-00016800: 7061 7468 202f 2022 726f 6f74 2f62 2e70  path / "root/b.p
-00016810: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
-00016820: 2050 6174 6828 7061 7468 202f 2022 726f   Path(path / "ro
-00016830: 6f74 2f63 2e70 7922 292c 0a20 2020 2020  ot/c.py"),.     
-00016840: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
-00016850: 202f 2022 726f 6f74 2f63 6869 6c64 2f63   / "root/child/c
-00016860: 2e70 7922 292c 0a20 2020 2020 2020 205d  .py"),.        ]
-00016870: 0a20 2020 2020 2020 2074 6869 735f 6162  .        this_ab
-00016880: 7320 3d20 5448 4953 5f44 4952 2e72 6573  s = THIS_DIR.res
-00016890: 6f6c 7665 2829 0a20 2020 2020 2020 2073  olve().        s
-000168a0: 6f75 7263 6573 203d 206c 6973 7428 0a20  ources = list(. 
-000168b0: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
-000168c0: 2e67 656e 5f70 7974 686f 6e5f 6669 6c65  .gen_python_file
-000168d0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-000168e0: 2020 2070 6174 682e 6974 6572 6469 7228     path.iterdir(
-000168f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00016900: 2020 2074 6869 735f 6162 732c 0a20 2020     this_abs,.   
-00016910: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
-00016920: 6c75 6465 2c0a 2020 2020 2020 2020 2020  lude,.          
-00016930: 2020 2020 2020 6578 636c 7564 652c 0a20        exclude,. 
-00016940: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00016950: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00016960: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
-00016970: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-00016980: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00016990: 2020 207b 7061 7468 3a20 726f 6f74 5f67     {path: root_g
-000169a0: 6974 6967 6e6f 7265 7d2c 0a20 2020 2020  itignore},.     
-000169b0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
-000169c0: 7365 3d46 616c 7365 2c0a 2020 2020 2020  se=False,.      
-000169d0: 2020 2020 2020 2020 2020 7175 6965 743d            quiet=
-000169e0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000169f0: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
-00016a00: 2020 2020 2020 2061 7373 6572 7420 736f         assert so
-00016a10: 7274 6564 2865 7870 6563 7465 6429 203d  rted(expected) =
-00016a20: 3d20 736f 7274 6564 2873 6f75 7263 6573  = sorted(sources
-00016a30: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00016a40: 6e65 7374 6564 5f67 6974 6967 6e6f 7265  nested_gitignore
-00016a50: 5f64 6972 6563 746c 795f 696e 5f73 6f75  _directly_in_sou
-00016a60: 7263 655f 6469 7265 6374 6f72 7928 7365  rce_directory(se
-00016a70: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00016a80: 2020 2020 2023 2068 7474 7073 3a2f 2f67       # https://g
-00016a90: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00016aa0: 6163 6b2f 6973 7375 6573 2f32 3539 380a  ack/issues/2598.
-00016ab0: 2020 2020 2020 2020 7061 7468 203d 2050          path = P
-00016ac0: 6174 6828 4441 5441 5f44 4952 202f 2022  ath(DATA_DIR / "
-00016ad0: 6e65 7374 6564 5f67 6974 6967 6e6f 7265  nested_gitignore
-00016ae0: 5f74 6573 7473 2229 0a20 2020 2020 2020  _tests").       
-00016af0: 2073 7263 203d 2050 6174 6828 7061 7468   src = Path(path
-00016b00: 202f 2022 726f 6f74 2220 2f20 2263 6869   / "root" / "chi
-00016b10: 6c64 2229 0a20 2020 2020 2020 2065 7870  ld").        exp
-00016b20: 6563 7465 6420 3d20 5b73 7263 202f 2022  ected = [src / "
-00016b30: 612e 7079 222c 2073 7263 202f 2022 632e  a.py", src / "c.
-00016b40: 7079 225d 0a20 2020 2020 2020 2061 7373  py"].        ass
-00016b50: 6572 745f 636f 6c6c 6563 7465 645f 736f  ert_collected_so
-00016b60: 7572 6365 7328 5b73 7263 5d2c 2065 7870  urces([src], exp
-00016b70: 6563 7465 6429 0a0a 2020 2020 6465 6620  ected)..    def 
-00016b80: 7465 7374 5f69 6e76 616c 6964 5f67 6974  test_invalid_git
-00016b90: 6967 6e6f 7265 2873 656c 6629 202d 3e20  ignore(self) -> 
-00016ba0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7061  None:.        pa
-00016bb0: 7468 203d 2054 4849 535f 4449 5220 2f20  th = THIS_DIR / 
-00016bc0: 2264 6174 6122 202f 2022 696e 7661 6c69  "data" / "invali
-00016bd0: 645f 6769 7469 676e 6f72 655f 7465 7374  d_gitignore_test
-00016be0: 7322 0a20 2020 2020 2020 2065 6d70 7479  s".        empty
-00016bf0: 5f63 6f6e 6669 6720 3d20 7061 7468 202f  _config = path /
-00016c00: 2022 7079 7072 6f6a 6563 742e 746f 6d6c   "pyproject.toml
-00016c10: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
-00016c20: 203d 2042 6c61 636b 5275 6e6e 6572 2829   = BlackRunner()
-00016c30: 2e69 6e76 6f6b 6528 0a20 2020 2020 2020  .invoke(.       
-00016c40: 2020 2020 2070 7969 6e6b 2e6d 6169 6e2c       pyink.main,
-00016c50: 205b 222d 2d76 6572 626f 7365 222c 2022   ["--verbose", "
-00016c60: 2d2d 636f 6e66 6967 222c 2073 7472 2865  --config", str(e
-00016c70: 6d70 7479 5f63 6f6e 6669 6729 2c20 7374  mpty_config), st
-00016c80: 7228 7061 7468 295d 0a20 2020 2020 2020  r(path)].       
-00016c90: 2029 0a20 2020 2020 2020 2061 7373 6572   ).        asser
-00016ca0: 7420 7265 7375 6c74 2e65 7869 745f 636f  t result.exit_co
-00016cb0: 6465 203d 3d20 310a 2020 2020 2020 2020  de == 1.        
-00016cc0: 6173 7365 7274 2072 6573 756c 742e 7374  assert result.st
-00016cd0: 6465 7272 5f62 7974 6573 2069 7320 6e6f  derr_bytes is no
-00016ce0: 7420 4e6f 6e65 0a0a 2020 2020 2020 2020  t None..        
-00016cf0: 6769 7469 676e 6f72 6520 3d20 7061 7468  gitignore = path
-00016d00: 202f 2022 2e67 6974 6967 6e6f 7265 220a   / ".gitignore".
-00016d10: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
-00016d20: 2243 6f75 6c64 206e 6f74 2070 6172 7365  "Could not parse
-00016d30: 207b 6769 7469 676e 6f72 657d 2220 696e   {gitignore}" in
-00016d40: 2072 6573 756c 742e 7374 6465 7272 5f62   result.stderr_b
-00016d50: 7974 6573 2e64 6563 6f64 6528 290a 0a20  ytes.decode().. 
-00016d60: 2020 2064 6566 2074 6573 745f 696e 7661     def test_inva
-00016d70: 6c69 645f 6e65 7374 6564 5f67 6974 6967  lid_nested_gitig
-00016d80: 6e6f 7265 2873 656c 6629 202d 3e20 4e6f  nore(self) -> No
-00016d90: 6e65 3a0a 2020 2020 2020 2020 7061 7468  ne:.        path
-00016da0: 203d 2054 4849 535f 4449 5220 2f20 2264   = THIS_DIR / "d
-00016db0: 6174 6122 202f 2022 696e 7661 6c69 645f  ata" / "invalid_
-00016dc0: 6e65 7374 6564 5f67 6974 6967 6e6f 7265  nested_gitignore
-00016dd0: 5f74 6573 7473 220a 2020 2020 2020 2020  _tests".        
-00016de0: 656d 7074 795f 636f 6e66 6967 203d 2070  empty_config = p
-00016df0: 6174 6820 2f20 2270 7970 726f 6a65 6374  ath / "pyproject
-00016e00: 2e74 6f6d 6c22 0a20 2020 2020 2020 2072  .toml".        r
-00016e10: 6573 756c 7420 3d20 426c 6163 6b52 756e  esult = BlackRun
-00016e20: 6e65 7228 292e 696e 766f 6b65 280a 2020  ner().invoke(.  
-00016e30: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
-00016e40: 6d61 696e 2c20 5b22 2d2d 7665 7262 6f73  main, ["--verbos
-00016e50: 6522 2c20 222d 2d63 6f6e 6669 6722 2c20  e", "--config", 
-00016e60: 7374 7228 656d 7074 795f 636f 6e66 6967  str(empty_config
-00016e70: 292c 2073 7472 2870 6174 6829 5d0a 2020  ), str(path)].  
-00016e80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00016e90: 6173 7365 7274 2072 6573 756c 742e 6578  assert result.ex
-00016ea0: 6974 5f63 6f64 6520 3d3d 2031 0a20 2020  it_code == 1.   
-00016eb0: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
-00016ec0: 6c74 2e73 7464 6572 725f 6279 7465 7320  lt.stderr_bytes 
-00016ed0: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
-00016ee0: 2020 2020 2067 6974 6967 6e6f 7265 203d       gitignore =
-00016ef0: 2070 6174 6820 2f20 2261 2220 2f20 222e   path / "a" / ".
-00016f00: 6769 7469 676e 6f72 6522 0a20 2020 2020  gitignore".     
-00016f10: 2020 2061 7373 6572 7420 6622 436f 756c     assert f"Coul
-00016f20: 6420 6e6f 7420 7061 7273 6520 7b67 6974  d not parse {git
-00016f30: 6967 6e6f 7265 7d22 2069 6e20 7265 7375  ignore}" in resu
-00016f40: 6c74 2e73 7464 6572 725f 6279 7465 732e  lt.stderr_bytes.
-00016f50: 6465 636f 6465 2829 0a0a 2020 2020 6465  decode()..    de
-00016f60: 6620 7465 7374 5f67 6974 6967 6e6f 7265  f test_gitignore
-00016f70: 5f74 6861 745f 6967 6e6f 7265 735f 7375  _that_ignores_su
-00016f80: 6266 6f6c 6465 7273 2873 656c 6629 202d  bfolders(self) -
-00016f90: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00016fa0: 2320 4966 2067 6974 6967 6e6f 7265 2077  # If gitignore w
-00016fb0: 6974 6820 2a2f 2a20 6973 2069 6e20 726f  ith */* is in ro
-00016fc0: 6f74 0a20 2020 2020 2020 2072 6f6f 7420  ot.        root 
-00016fd0: 3d20 5061 7468 2844 4154 415f 4449 5220  = Path(DATA_DIR 
-00016fe0: 2f20 2269 676e 6f72 655f 7375 6266 6f6c  / "ignore_subfol
-00016ff0: 6465 7273 5f67 6974 6967 6e6f 7265 5f74  ders_gitignore_t
-00017000: 6573 7473 2220 2f20 2273 7562 6469 7222  ests" / "subdir"
-00017010: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
-00017020: 6564 203d 205b 726f 6f74 202f 2022 622e  ed = [root / "b.
-00017030: 7079 225d 0a20 2020 2020 2020 2063 7478  py"].        ctx
-00017040: 203d 2046 616b 6543 6f6e 7465 7874 2829   = FakeContext()
-00017050: 0a20 2020 2020 2020 2063 7478 2e6f 626a  .        ctx.obj
-00017060: 5b22 726f 6f74 225d 203d 2072 6f6f 740a  ["root"] = root.
-00017070: 2020 2020 2020 2020 6173 7365 7274 5f63          assert_c
-00017080: 6f6c 6c65 6374 6564 5f73 6f75 7263 6573  ollected_sources
-00017090: 285b 726f 6f74 5d2c 2065 7870 6563 7465  ([root], expecte
-000170a0: 642c 2063 7478 3d63 7478 290a 0a20 2020  d, ctx=ctx)..   
-000170b0: 2020 2020 2023 2049 6620 2e67 6974 6967       # If .gitig
-000170c0: 6e6f 7265 2077 6974 6820 2a2f 2a20 6973  nore with */* is
-000170d0: 206e 6573 7465 640a 2020 2020 2020 2020   nested.        
-000170e0: 726f 6f74 203d 2050 6174 6828 4441 5441  root = Path(DATA
-000170f0: 5f44 4952 202f 2022 6967 6e6f 7265 5f73  _DIR / "ignore_s
-00017100: 7562 666f 6c64 6572 735f 6769 7469 676e  ubfolders_gitign
-00017110: 6f72 655f 7465 7374 7322 290a 2020 2020  ore_tests").    
-00017120: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
-00017130: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
-00017140: 7420 2f20 2261 2e70 7922 2c0a 2020 2020  t / "a.py",.    
-00017150: 2020 2020 2020 2020 726f 6f74 202f 2022          root / "
-00017160: 7375 6264 6972 2220 2f20 2262 2e70 7922  subdir" / "b.py"
-00017170: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
-00017180: 2020 2020 6374 7820 3d20 4661 6b65 436f      ctx = FakeCo
-00017190: 6e74 6578 7428 290a 2020 2020 2020 2020  ntext().        
-000171a0: 6374 782e 6f62 6a5b 2272 6f6f 7422 5d20  ctx.obj["root"] 
-000171b0: 3d20 726f 6f74 0a20 2020 2020 2020 2061  = root.        a
-000171c0: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
-000171d0: 736f 7572 6365 7328 5b72 6f6f 745d 2c20  sources([root], 
-000171e0: 6578 7065 6374 6564 2c20 6374 783d 6374  expected, ctx=ct
-000171f0: 7829 0a0a 2020 2020 2020 2020 2320 4966  x)..        # If
-00017200: 2063 6f6d 6d61 6e64 2069 7320 6578 6563   command is exec
-00017210: 7574 6564 2066 726f 6d20 6f75 7465 7220  uted from outer 
-00017220: 6469 720a 2020 2020 2020 2020 726f 6f74  dir.        root
-00017230: 203d 2050 6174 6828 4441 5441 5f44 4952   = Path(DATA_DIR
-00017240: 202f 2022 6967 6e6f 7265 5f73 7562 666f   / "ignore_subfo
-00017250: 6c64 6572 735f 6769 7469 676e 6f72 655f  lders_gitignore_
-00017260: 7465 7374 7322 290a 2020 2020 2020 2020  tests").        
-00017270: 7461 7267 6574 203d 2072 6f6f 7420 2f20  target = root / 
-00017280: 2273 7562 6469 7222 0a20 2020 2020 2020  "subdir".       
-00017290: 2065 7870 6563 7465 6420 3d20 5b74 6172   expected = [tar
-000172a0: 6765 7420 2f20 2262 2e70 7922 5d0a 2020  get / "b.py"].  
-000172b0: 2020 2020 2020 6374 7820 3d20 4661 6b65        ctx = Fake
-000172c0: 436f 6e74 6578 7428 290a 2020 2020 2020  Context().      
-000172d0: 2020 6374 782e 6f62 6a5b 2272 6f6f 7422    ctx.obj["root"
-000172e0: 5d20 3d20 726f 6f74 0a20 2020 2020 2020  ] = root.       
-000172f0: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00017300: 645f 736f 7572 6365 7328 5b74 6172 6765  d_sources([targe
-00017310: 745d 2c20 6578 7065 6374 6564 2c20 6374  t], expected, ct
-00017320: 783d 6374 7829 0a0a 2020 2020 6465 6620  x=ctx)..    def 
-00017330: 7465 7374 5f65 6d70 7479 5f69 6e63 6c75  test_empty_inclu
-00017340: 6465 2873 656c 6629 202d 3e20 4e6f 6e65  de(self) -> None
-00017350: 3a0a 2020 2020 2020 2020 7061 7468 203d  :.        path =
-00017360: 2044 4154 415f 4449 5220 2f20 2269 6e63   DATA_DIR / "inc
-00017370: 6c75 6465 5f65 7863 6c75 6465 5f74 6573  lude_exclude_tes
-00017380: 7473 220a 2020 2020 2020 2020 7372 6320  ts".        src 
-00017390: 3d20 5b70 6174 685d 0a20 2020 2020 2020  = [path].       
-000173a0: 2065 7870 6563 7465 6420 3d20 5b0a 2020   expected = [.  
-000173b0: 2020 2020 2020 2020 2020 5061 7468 2870            Path(p
-000173c0: 6174 6820 2f20 2262 2f65 7863 6c75 6465  ath / "b/exclude
-000173d0: 2f61 2e70 6965 2229 2c0a 2020 2020 2020  /a.pie"),.      
-000173e0: 2020 2020 2020 5061 7468 2870 6174 6820        Path(path 
-000173f0: 2f20 2262 2f65 7863 6c75 6465 2f61 2e70  / "b/exclude/a.p
-00017400: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
-00017410: 2050 6174 6828 7061 7468 202f 2022 622f   Path(path / "b/
-00017420: 6578 636c 7564 652f 612e 7079 6922 292c  exclude/a.pyi"),
-00017430: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
-00017440: 6828 7061 7468 202f 2022 622f 646f 6e74  h(path / "b/dont
-00017450: 5f65 7863 6c75 6465 2f61 2e70 6965 2229  _exclude/a.pie")
-00017460: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
-00017470: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
-00017480: 745f 6578 636c 7564 652f 612e 7079 2229  t_exclude/a.py")
-00017490: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
-000174a0: 7468 2870 6174 6820 2f20 2262 2f64 6f6e  th(path / "b/don
-000174b0: 745f 6578 636c 7564 652f 612e 7079 6922  t_exclude/a.pyi"
-000174c0: 292c 0a20 2020 2020 2020 2020 2020 2050  ),.            P
-000174d0: 6174 6828 7061 7468 202f 2022 622f 2e64  ath(path / "b/.d
-000174e0: 6566 696e 6974 656c 795f 6578 636c 7564  efinitely_exclud
-000174f0: 652f 612e 7069 6522 292c 0a20 2020 2020  e/a.pie"),.     
-00017500: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
-00017510: 202f 2022 622f 2e64 6566 696e 6974 656c   / "b/.definitel
-00017520: 795f 6578 636c 7564 652f 612e 7079 2229  y_exclude/a.py")
-00017530: 2c0a 2020 2020 2020 2020 2020 2020 5061  ,.            Pa
-00017540: 7468 2870 6174 6820 2f20 2262 2f2e 6465  th(path / "b/.de
-00017550: 6669 6e69 7465 6c79 5f65 7863 6c75 6465  finitely_exclude
-00017560: 2f61 2e70 7969 2229 2c0a 2020 2020 2020  /a.pyi"),.      
-00017570: 2020 2020 2020 5061 7468 2870 6174 6820        Path(path 
-00017580: 2f20 222e 6769 7469 676e 6f72 6522 292c  / ".gitignore"),
-00017590: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
-000175a0: 6828 7061 7468 202f 2022 7079 7072 6f6a  h(path / "pyproj
-000175b0: 6563 742e 746f 6d6c 2229 2c0a 2020 2020  ect.toml"),.    
-000175c0: 2020 2020 5d0a 2020 2020 2020 2020 2320      ].        # 
-000175d0: 5365 7474 696e 6720 6578 636c 7564 6520  Setting exclude 
-000175e0: 6578 706c 6963 6974 6c79 2074 6f20 616e  explicitly to an
-000175f0: 2065 6d70 7479 2073 7472 696e 6720 746f   empty string to
-00017600: 2062 6c6f 636b 202e 6769 7469 676e 6f72   block .gitignor
-00017610: 6520 7573 6167 652e 0a20 2020 2020 2020  e usage..       
-00017620: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00017630: 645f 736f 7572 6365 7328 7372 632c 2065  d_sources(src, e
-00017640: 7870 6563 7465 642c 2069 6e63 6c75 6465  xpected, include
-00017650: 3d22 222c 2065 7863 6c75 6465 3d22 2229  ="", exclude="")
-00017660: 0a0a 2020 2020 6465 6620 7465 7374 5f65  ..    def test_e
-00017670: 7874 656e 645f 6578 636c 7564 6528 7365  xtend_exclude(se
-00017680: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00017690: 2020 2020 2070 6174 6820 3d20 4441 5441       path = DATA
-000176a0: 5f44 4952 202f 2022 696e 636c 7564 655f  _DIR / "include_
-000176b0: 6578 636c 7564 655f 7465 7374 7322 0a20  exclude_tests". 
-000176c0: 2020 2020 2020 2073 7263 203d 205b 7061         src = [pa
-000176d0: 7468 5d0a 2020 2020 2020 2020 6578 7065  th].        expe
-000176e0: 6374 6564 203d 205b 0a20 2020 2020 2020  cted = [.       
-000176f0: 2020 2020 2050 6174 6828 7061 7468 202f       Path(path /
-00017700: 2022 622f 6578 636c 7564 652f 612e 7079   "b/exclude/a.py
-00017710: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00017720: 5061 7468 2870 6174 6820 2f20 2262 2f64  Path(path / "b/d
-00017730: 6f6e 745f 6578 636c 7564 652f 612e 7079  ont_exclude/a.py
-00017740: 2229 2c0a 2020 2020 2020 2020 5d0a 2020  "),.        ].  
-00017750: 2020 2020 2020 6173 7365 7274 5f63 6f6c        assert_col
-00017760: 6c65 6374 6564 5f73 6f75 7263 6573 280a  lected_sources(.
-00017770: 2020 2020 2020 2020 2020 2020 7372 632c              src,
-00017780: 2065 7870 6563 7465 642c 2065 7863 6c75   expected, exclu
-00017790: 6465 3d72 225c 2e70 7969 2422 2c20 6578  de=r"\.pyi$", ex
-000177a0: 7465 6e64 5f65 7863 6c75 6465 3d72 225c  tend_exclude=r"\
-000177b0: 2e64 6566 696e 6974 656c 795f 6578 636c  .definitely_excl
-000177c0: 7564 6522 0a20 2020 2020 2020 2029 0a0a  ude".        )..
-000177d0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-000177e0: 2e69 6e63 6f6d 7061 7469 626c 655f 7769  .incompatible_wi
-000177f0: 7468 5f6d 7970 7963 0a20 2020 2064 6566  th_mypyc.    def
-00017800: 2074 6573 745f 7379 6d6c 696e 6b5f 6f75   test_symlink_ou
-00017810: 745f 6f66 5f72 6f6f 745f 6469 7265 6374  t_of_root_direct
-00017820: 6f72 7928 7365 6c66 2920 2d3e 204e 6f6e  ory(self) -> Non
-00017830: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
-00017840: 3d20 4d61 6769 634d 6f63 6b28 290a 2020  = MagicMock().  
-00017850: 2020 2020 2020 726f 6f74 203d 2054 4849        root = THI
-00017860: 535f 4449 522e 7265 736f 6c76 6528 290a  S_DIR.resolve().
-00017870: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
-00017880: 4d61 6769 634d 6f63 6b28 290a 2020 2020  MagicMock().    
-00017890: 2020 2020 696e 636c 7564 6520 3d20 7265      include = re
-000178a0: 2e63 6f6d 7069 6c65 2870 7969 6e6b 2e44  .compile(pyink.D
-000178b0: 4546 4155 4c54 5f49 4e43 4c55 4445 5329  EFAULT_INCLUDES)
-000178c0: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-000178d0: 203d 2072 652e 636f 6d70 696c 6528 7079   = re.compile(py
-000178e0: 696e 6b2e 4445 4641 554c 545f 4558 434c  ink.DEFAULT_EXCL
-000178f0: 5544 4553 290a 2020 2020 2020 2020 7265  UDES).        re
-00017900: 706f 7274 203d 2070 7969 6e6b 2e52 6570  port = pyink.Rep
-00017910: 6f72 7428 290a 2020 2020 2020 2020 6769  ort().        gi
-00017920: 7469 676e 6f72 6520 3d20 5061 7468 5370  tignore = PathSp
-00017930: 6563 2e66 726f 6d5f 6c69 6e65 7328 2267  ec.from_lines("g
-00017940: 6974 7769 6c64 6d61 7463 6822 2c20 5b5d  itwildmatch", []
-00017950: 290a 2020 2020 2020 2020 2320 6063 6869  ).        # `chi
-00017960: 6c64 6020 7368 6f75 6c64 2062 6568 6176  ld` should behav
-00017970: 6520 6c69 6b65 2061 2073 796d 6c69 6e6b  e like a symlink
-00017980: 2077 6869 6368 2072 6573 6f6c 7665 6420   which resolved 
-00017990: 7061 7468 2069 7320 636c 6561 726c 790a  path is clearly.
-000179a0: 2020 2020 2020 2020 2320 6f75 7473 6964          # outsid
-000179b0: 6520 6f66 2074 6865 2060 726f 6f74 6020  e of the `root` 
-000179c0: 6469 7265 6374 6f72 792e 0a20 2020 2020  directory..     
-000179d0: 2020 2070 6174 682e 6974 6572 6469 722e     path.iterdir.
-000179e0: 7265 7475 726e 5f76 616c 7565 203d 205b  return_value = [
-000179f0: 6368 696c 645d 0a20 2020 2020 2020 2063  child].        c
-00017a00: 6869 6c64 2e72 6573 6f6c 7665 2e72 6574  hild.resolve.ret
-00017a10: 7572 6e5f 7661 6c75 6520 3d20 5061 7468  urn_value = Path
-00017a20: 2822 2f61 2f62 2f63 2229 0a20 2020 2020  ("/a/b/c").     
-00017a30: 2020 2063 6869 6c64 2e61 735f 706f 7369     child.as_posi
-00017a40: 782e 7265 7475 726e 5f76 616c 7565 203d  x.return_value =
-00017a50: 2022 2f61 2f62 2f63 220a 2020 2020 2020   "/a/b/c".      
-00017a60: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00017a70: 2020 206c 6973 7428 0a20 2020 2020 2020     list(.       
-00017a80: 2020 2020 2020 2020 2070 7969 6e6b 2e67           pyink.g
-00017a90: 656e 5f70 7974 686f 6e5f 6669 6c65 7328  en_python_files(
-00017aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ab0: 2020 2020 2070 6174 682e 6974 6572 6469       path.iterdi
-00017ac0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
-00017ad0: 2020 2020 2020 2020 2072 6f6f 742c 0a20           root,. 
-00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017af0: 2020 2069 6e63 6c75 6465 2c0a 2020 2020     include,.    
-00017b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b10: 6578 636c 7564 652c 0a20 2020 2020 2020  exclude,.       
-00017b20: 2020 2020 2020 2020 2020 2020 204e 6f6e               Non
-00017b30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00017b40: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b60: 2072 6570 6f72 742c 0a20 2020 2020 2020   report,.       
-00017b70: 2020 2020 2020 2020 2020 2020 207b 7061               {pa
-00017b80: 7468 3a20 6769 7469 676e 6f72 657d 2c0a  th: gitignore},.
-00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ba0: 2020 2020 7665 7262 6f73 653d 4661 6c73      verbose=Fals
-00017bb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00017bc0: 2020 2020 2020 2071 7569 6574 3d46 616c         quiet=Fal
-00017bd0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00017be0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017bf0: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
-00017c00: 7074 2056 616c 7565 4572 726f 7220 6173  pt ValueError as
-00017c10: 2076 653a 0a20 2020 2020 2020 2020 2020   ve:.           
-00017c20: 2070 7974 6573 742e 6661 696c 2866 2260   pytest.fail(f"`
-00017c30: 6765 745f 7079 7468 6f6e 5f66 696c 6573  get_python_files
-00017c40: 5f69 6e5f 6469 7228 2960 2066 6169 6c65  _in_dir()` faile
-00017c50: 643a 207b 7665 7d22 290a 2020 2020 2020  d: {ve}").      
-00017c60: 2020 7061 7468 2e69 7465 7264 6972 2e61    path.iterdir.a
-00017c70: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
-00017c80: 6528 290a 2020 2020 2020 2020 6368 696c  e().        chil
-00017c90: 642e 7265 736f 6c76 652e 6173 7365 7274  d.resolve.assert
-00017ca0: 5f63 616c 6c65 645f 6f6e 6365 2829 0a0a  _called_once()..
-00017cb0: 2020 2020 4070 6174 6368 2822 7079 696e      @patch("pyin
-00017cc0: 6b2e 6669 6e64 5f70 726f 6a65 6374 5f72  k.find_project_r
-00017cd0: 6f6f 7422 2c20 6c61 6d62 6461 202a 6172  oot", lambda *ar
-00017ce0: 6773 3a20 2854 4849 535f 4449 522e 7265  gs: (THIS_DIR.re
-00017cf0: 736f 6c76 6528 292c 204e 6f6e 6529 290a  solve(), None)).
-00017d00: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-00017d10: 5f73 6f75 7263 6573 5f77 6974 685f 7374  _sources_with_st
-00017d20: 6469 6e28 7365 6c66 2920 2d3e 204e 6f6e  din(self) -> Non
-00017d30: 653a 0a20 2020 2020 2020 2073 7263 203d  e:.        src =
-00017d40: 205b 222d 225d 0a20 2020 2020 2020 2065   ["-"].        e
-00017d50: 7870 6563 7465 6420 3d20 5b22 2d22 5d0a  xpected = ["-"].
-00017d60: 2020 2020 2020 2020 6173 7365 7274 5f63          assert_c
-00017d70: 6f6c 6c65 6374 6564 5f73 6f75 7263 6573  ollected_sources
-00017d80: 2873 7263 2c20 6578 7065 6374 6564 2c20  (src, expected, 
-00017d90: 696e 636c 7564 653d 2222 2c20 6578 636c  include="", excl
-00017da0: 7564 653d 7222 2f65 7863 6c75 6465 2f7c  ude=r"/exclude/|
-00017db0: 615c 2e70 7922 290a 0a20 2020 2040 7061  a\.py")..    @pa
-00017dc0: 7463 6828 2270 7969 6e6b 2e66 696e 645f  tch("pyink.find_
-00017dd0: 7072 6f6a 6563 745f 726f 6f74 222c 206c  project_root", l
-00017de0: 616d 6264 6120 2a61 7267 733a 2028 5448  ambda *args: (TH
-00017df0: 4953 5f44 4952 2e72 6573 6f6c 7665 2829  IS_DIR.resolve()
-00017e00: 2c20 4e6f 6e65 2929 0a20 2020 2064 6566  , None)).    def
-00017e10: 2074 6573 745f 6765 745f 736f 7572 6365   test_get_source
-00017e20: 735f 7769 7468 5f73 7464 696e 5f66 696c  s_with_stdin_fil
-00017e30: 656e 616d 6528 7365 6c66 2920 2d3e 204e  ename(self) -> N
-00017e40: 6f6e 653a 0a20 2020 2020 2020 2073 7263  one:.        src
-00017e50: 203d 205b 222d 225d 0a20 2020 2020 2020   = ["-"].       
-00017e60: 2073 7464 696e 5f66 696c 656e 616d 6520   stdin_filename 
-00017e70: 3d20 7374 7228 5448 4953 5f44 4952 202f  = str(THIS_DIR /
-00017e80: 2022 6461 7461 2f63 6f6c 6c65 6374 696f   "data/collectio
-00017e90: 6e73 2e70 7922 290a 2020 2020 2020 2020  ns.py").        
-00017ea0: 6578 7065 6374 6564 203d 205b 6622 5f5f  expected = [f"__
-00017eb0: 5059 494e 4b5f 5354 4449 4e5f 4649 4c45  PYINK_STDIN_FILE
-00017ec0: 4e41 4d45 5f5f 7b73 7464 696e 5f66 696c  NAME__{stdin_fil
-00017ed0: 656e 616d 657d 225d 0a20 2020 2020 2020  ename}"].       
-00017ee0: 2061 7373 6572 745f 636f 6c6c 6563 7465   assert_collecte
-00017ef0: 645f 736f 7572 6365 7328 0a20 2020 2020  d_sources(.     
-00017f00: 2020 2020 2020 2073 7263 2c0a 2020 2020         src,.    
-00017f10: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00017f20: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-00017f30: 636c 7564 653d 7222 2f65 7863 6c75 6465  clude=r"/exclude
-00017f40: 2f61 5c2e 7079 222c 0a20 2020 2020 2020  /a\.py",.       
-00017f50: 2020 2020 2073 7464 696e 5f66 696c 656e       stdin_filen
-00017f60: 616d 653d 7374 6469 6e5f 6669 6c65 6e61  ame=stdin_filena
-00017f70: 6d65 2c0a 2020 2020 2020 2020 290a 0a20  me,.        ).. 
-00017f80: 2020 2040 7061 7463 6828 2270 7969 6e6b     @patch("pyink
-00017f90: 2e66 696e 645f 7072 6f6a 6563 745f 726f  .find_project_ro
-00017fa0: 6f74 222c 206c 616d 6264 6120 2a61 7267  ot", lambda *arg
-00017fb0: 733a 2028 5448 4953 5f44 4952 2e72 6573  s: (THIS_DIR.res
-00017fc0: 6f6c 7665 2829 2c20 4e6f 6e65 2929 0a20  olve(), None)). 
-00017fd0: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
-00017fe0: 736f 7572 6365 735f 7769 7468 5f73 7464  sources_with_std
-00017ff0: 696e 5f66 696c 656e 616d 655f 616e 645f  in_filename_and_
-00018000: 6578 636c 7564 6528 7365 6c66 2920 2d3e  exclude(self) ->
-00018010: 204e 6f6e 653a 0a20 2020 2020 2020 2023   None:.        #
-00018020: 2045 7863 6c75 6465 2073 686f 756c 646e   Exclude shouldn
-00018030: 2774 2065 7863 6c75 6465 2073 7464 696e  't exclude stdin
-00018040: 5f66 696c 656e 616d 6520 7369 6e63 6520  _filename since 
-00018050: 6974 2069 7320 6d69 6d69 636b 696e 6720  it is mimicking 
-00018060: 7468 650a 2020 2020 2020 2020 2320 6669  the.        # fi
-00018070: 6c65 2062 6569 6e67 2070 6173 7365 6420  le being passed 
-00018080: 6469 7265 6374 6c79 2e20 5468 6973 2069  directly. This i
-00018090: 7320 7468 6520 7361 6d65 2061 730a 2020  s the same as.  
-000180a0: 2020 2020 2020 2320 7465 7374 5f65 7863        # test_exc
-000180b0: 6c75 6465 5f66 6f72 5f69 7373 7565 5f31  lude_for_issue_1
-000180c0: 3537 320a 2020 2020 2020 2020 7061 7468  572.        path
-000180d0: 203d 2044 4154 415f 4449 5220 2f20 2269   = DATA_DIR / "i
-000180e0: 6e63 6c75 6465 5f65 7863 6c75 6465 5f74  nclude_exclude_t
-000180f0: 6573 7473 220a 2020 2020 2020 2020 7372  ests".        sr
-00018100: 6320 3d20 5b22 2d22 5d0a 2020 2020 2020  c = ["-"].      
-00018110: 2020 7374 6469 6e5f 6669 6c65 6e61 6d65    stdin_filename
-00018120: 203d 2073 7472 2870 6174 6820 2f20 2262   = str(path / "b
-00018130: 2f65 7863 6c75 6465 2f61 2e70 7922 290a  /exclude/a.py").
-00018140: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00018150: 203d 205b 6622 5f5f 5059 494e 4b5f 5354   = [f"__PYINK_ST
-00018160: 4449 4e5f 4649 4c45 4e41 4d45 5f5f 7b73  DIN_FILENAME__{s
-00018170: 7464 696e 5f66 696c 656e 616d 657d 225d  tdin_filename}"]
-00018180: 0a20 2020 2020 2020 2061 7373 6572 745f  .        assert_
-00018190: 636f 6c6c 6563 7465 645f 736f 7572 6365  collected_source
-000181a0: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
-000181b0: 7263 2c0a 2020 2020 2020 2020 2020 2020  rc,.            
-000181c0: 6578 7065 6374 6564 2c0a 2020 2020 2020  expected,.      
-000181d0: 2020 2020 2020 6578 636c 7564 653d 7222        exclude=r"
-000181e0: 2f65 7863 6c75 6465 2f7c 615c 2e70 7922  /exclude/|a\.py"
-000181f0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-00018200: 6469 6e5f 6669 6c65 6e61 6d65 3d73 7464  din_filename=std
-00018210: 696e 5f66 696c 656e 616d 652c 0a20 2020  in_filename,.   
-00018220: 2020 2020 2029 0a0a 2020 2020 4070 6174       )..    @pat
-00018230: 6368 2822 7079 696e 6b2e 6669 6e64 5f70  ch("pyink.find_p
-00018240: 726f 6a65 6374 5f72 6f6f 7422 2c20 6c61  roject_root", la
-00018250: 6d62 6461 202a 6172 6773 3a20 2854 4849  mbda *args: (THI
-00018260: 535f 4449 522e 7265 736f 6c76 6528 292c  S_DIR.resolve(),
-00018270: 204e 6f6e 6529 290a 2020 2020 6465 6620   None)).    def 
-00018280: 7465 7374 5f67 6574 5f73 6f75 7263 6573  test_get_sources
-00018290: 5f77 6974 685f 7374 6469 6e5f 6669 6c65  _with_stdin_file
-000182a0: 6e61 6d65 5f61 6e64 5f65 7874 656e 645f  name_and_extend_
-000182b0: 6578 636c 7564 6528 7365 6c66 2920 2d3e  exclude(self) ->
-000182c0: 204e 6f6e 653a 0a20 2020 2020 2020 2023   None:.        #
-000182d0: 2045 7874 656e 6420 6578 636c 7564 6520   Extend exclude 
-000182e0: 7368 6f75 6c64 6e27 7420 6578 636c 7564  shouldn't exclud
-000182f0: 6520 7374 6469 6e5f 6669 6c65 6e61 6d65  e stdin_filename
-00018300: 2073 696e 6365 2069 7420 6973 206d 696d   since it is mim
-00018310: 6963 6b69 6e67 2074 6865 0a20 2020 2020  icking the.     
-00018320: 2020 2023 2066 696c 6520 6265 696e 6720     # file being 
-00018330: 7061 7373 6564 2064 6972 6563 746c 792e  passed directly.
-00018340: 2054 6869 7320 6973 2074 6865 2073 616d   This is the sam
-00018350: 6520 6173 0a20 2020 2020 2020 2023 2074  e as.        # t
-00018360: 6573 745f 6578 636c 7564 655f 666f 725f  est_exclude_for_
-00018370: 6973 7375 655f 3135 3732 0a20 2020 2020  issue_1572.     
-00018380: 2020 2073 7263 203d 205b 222d 225d 0a20     src = ["-"]. 
-00018390: 2020 2020 2020 2070 6174 6820 3d20 5448         path = TH
-000183a0: 4953 5f44 4952 202f 2022 6461 7461 2220  IS_DIR / "data" 
-000183b0: 2f20 2269 6e63 6c75 6465 5f65 7863 6c75  / "include_exclu
-000183c0: 6465 5f74 6573 7473 220a 2020 2020 2020  de_tests".      
-000183d0: 2020 7374 6469 6e5f 6669 6c65 6e61 6d65    stdin_filename
-000183e0: 203d 2073 7472 2870 6174 6820 2f20 2262   = str(path / "b
-000183f0: 2f65 7863 6c75 6465 2f61 2e70 7922 290a  /exclude/a.py").
-00018400: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00018410: 203d 205b 6622 5f5f 5059 494e 4b5f 5354   = [f"__PYINK_ST
-00018420: 4449 4e5f 4649 4c45 4e41 4d45 5f5f 7b73  DIN_FILENAME__{s
-00018430: 7464 696e 5f66 696c 656e 616d 657d 225d  tdin_filename}"]
-00018440: 0a20 2020 2020 2020 2061 7373 6572 745f  .        assert_
-00018450: 636f 6c6c 6563 7465 645f 736f 7572 6365  collected_source
-00018460: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
-00018470: 7263 2c0a 2020 2020 2020 2020 2020 2020  rc,.            
-00018480: 6578 7065 6374 6564 2c0a 2020 2020 2020  expected,.      
-00018490: 2020 2020 2020 6578 7465 6e64 5f65 7863        extend_exc
-000184a0: 6c75 6465 3d72 222f 6578 636c 7564 652f  lude=r"/exclude/
-000184b0: 7c61 5c2e 7079 222c 0a20 2020 2020 2020  |a\.py",.       
-000184c0: 2020 2020 2073 7464 696e 5f66 696c 656e       stdin_filen
-000184d0: 616d 653d 7374 6469 6e5f 6669 6c65 6e61  ame=stdin_filena
-000184e0: 6d65 2c0a 2020 2020 2020 2020 290a 0a20  me,.        ).. 
-000184f0: 2020 2040 7061 7463 6828 2270 7969 6e6b     @patch("pyink
-00018500: 2e66 696e 645f 7072 6f6a 6563 745f 726f  .find_project_ro
-00018510: 6f74 222c 206c 616d 6264 6120 2a61 7267  ot", lambda *arg
-00018520: 733a 2028 5448 4953 5f44 4952 2e72 6573  s: (THIS_DIR.res
-00018530: 6f6c 7665 2829 2c20 4e6f 6e65 2929 0a20  olve(), None)). 
-00018540: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
-00018550: 736f 7572 6365 735f 7769 7468 5f73 7464  sources_with_std
-00018560: 696e 5f66 696c 656e 616d 655f 616e 645f  in_filename_and_
-00018570: 666f 7263 655f 6578 636c 7564 6528 7365  force_exclude(se
-00018580: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00018590: 2020 2020 2023 2046 6f72 6365 2065 7863       # Force exc
-000185a0: 6c75 6465 2073 686f 756c 6420 6578 636c  lude should excl
-000185b0: 7564 6520 7468 6520 6669 6c65 2077 6865  ude the file whe
-000185c0: 6e20 7061 7373 696e 6720 6974 2074 6872  n passing it thr
-000185d0: 6f75 6768 0a20 2020 2020 2020 2023 2073  ough.        # s
-000185e0: 7464 696e 5f66 696c 656e 616d 650a 2020  tdin_filename.  
-000185f0: 2020 2020 2020 7061 7468 203d 2054 4849        path = THI
-00018600: 535f 4449 5220 2f20 2264 6174 6122 202f  S_DIR / "data" /
-00018610: 2022 696e 636c 7564 655f 6578 636c 7564   "include_exclud
-00018620: 655f 7465 7374 7322 0a20 2020 2020 2020  e_tests".       
-00018630: 2073 7464 696e 5f66 696c 656e 616d 6520   stdin_filename 
-00018640: 3d20 7374 7228 7061 7468 202f 2022 622f  = str(path / "b/
-00018650: 6578 636c 7564 652f 612e 7079 2229 0a20  exclude/a.py"). 
-00018660: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
-00018670: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
-00018680: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00018690: 3d5b 222d 225d 2c0a 2020 2020 2020 2020  =["-"],.        
-000186a0: 2020 2020 6578 7065 6374 6564 3d5b 5d2c      expected=[],
-000186b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000186c0: 6365 5f65 7863 6c75 6465 3d72 222f 6578  ce_exclude=r"/ex
-000186d0: 636c 7564 652f 7c61 5c2e 7079 222c 0a20  clude/|a\.py",. 
-000186e0: 2020 2020 2020 2020 2020 2073 7464 696e             stdin
-000186f0: 5f66 696c 656e 616d 653d 7374 6469 6e5f  _filename=stdin_
-00018700: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
-00018710: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
-00018720: 745f 7079 696e 6b5f 6465 6661 756c 7428  t_pyink_default(
-00018730: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00018740: 2020 2020 2020 2070 6174 6820 3d20 5448         path = TH
-00018750: 4953 5f44 4952 202f 2022 6461 7461 2220  IS_DIR / "data" 
-00018760: 2f20 2270 7969 6e6b 5f63 6f6e 6669 6773  / "pyink_configs
-00018770: 220a 2020 2020 2020 2020 6578 616d 706c  ".        exampl
-00018780: 6520 3d20 7374 7228 7061 7468 202f 2022  e = str(path / "
-00018790: 6578 616d 706c 652e 7079 2229 0a20 2020  example.py").   
-000187a0: 2020 2020 2063 6f6e 6669 6720 3d20 7374       config = st
-000187b0: 7228 5448 4953 5f44 4952 202f 2022 656d  r(THIS_DIR / "em
-000187c0: 7074 792e 746f 6d6c 2229 0a20 2020 2020  pty.toml").     
-000187d0: 2020 2072 6573 756c 7420 3d20 426c 6163     result = Blac
-000187e0: 6b52 756e 6e65 7228 292e 696e 766f 6b65  kRunner().invoke
-000187f0: 280a 2020 2020 2020 2020 2020 2020 7079  (.            py
-00018800: 696e 6b2e 6d61 696e 2c20 5b22 2d2d 6469  ink.main, ["--di
-00018810: 6666 222c 2022 2d2d 636f 6e66 6967 222c  ff", "--config",
-00018820: 2063 6f6e 6669 672c 2065 7861 6d70 6c65   config, example
-00018830: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-00018840: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
-00018850: 742e 6578 6974 5f63 6f64 6520 3d3d 2030  t.exit_code == 0
-00018860: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00018870: 7265 7375 6c74 2e73 7464 6f75 745f 6279  result.stdout_by
-00018880: 7465 7320 6973 206e 6f74 204e 6f6e 650a  tes is not None.
-00018890: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000188a0: 222d 2070 6173 735c 6e2b 2020 2020 7061  "- pass\n+    pa
-000188b0: 7373 5c6e 2220 696e 2072 6573 756c 742e  ss\n" in result.
-000188c0: 7374 646f 7574 5f62 7974 6573 2e64 6563  stdout_bytes.dec
-000188d0: 6f64 6528 290a 0a20 2020 2064 6566 2074  ode()..    def t
-000188e0: 6573 745f 7079 696e 6b5f 6f76 6572 7269  est_pyink_overri
-000188f0: 6465 7328 7365 6c66 2920 2d3e 204e 6f6e  des(self) -> Non
-00018900: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
-00018910: 3d20 5448 4953 5f44 4952 202f 2022 6461  = THIS_DIR / "da
-00018920: 7461 2220 2f20 2270 7969 6e6b 5f63 6f6e  ta" / "pyink_con
-00018930: 6669 6773 220a 2020 2020 2020 2020 6578  figs".        ex
-00018940: 616d 706c 6520 3d20 7374 7228 7061 7468  ample = str(path
-00018950: 202f 2022 6578 616d 706c 652e 7079 2229   / "example.py")
-00018960: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
-00018970: 3d20 7374 7228 7061 7468 202f 2022 6f76  = str(path / "ov
-00018980: 6572 7269 6465 732e 746f 6d6c 2229 0a20  errides.toml"). 
-00018990: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000189a0: 426c 6163 6b52 756e 6e65 7228 292e 696e  BlackRunner().in
-000189b0: 766f 6b65 280a 2020 2020 2020 2020 2020  voke(.          
-000189c0: 2020 7079 696e 6b2e 6d61 696e 2c20 5b22    pyink.main, ["
-000189d0: 2d2d 6469 6666 222c 2022 2d2d 636f 6e66  --diff", "--conf
-000189e0: 6967 222c 2063 6f6e 6669 672c 2065 7861  ig", config, exa
-000189f0: 6d70 6c65 5d0a 2020 2020 2020 2020 290a  mple].        ).
-00018a00: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-00018a10: 6573 756c 742e 6578 6974 5f63 6f64 6520  esult.exit_code 
-00018a20: 3d3d 2030 0a20 2020 2020 2020 2061 7373  == 0.        ass
-00018a30: 6572 7420 7265 7375 6c74 2e73 7464 6f75  ert result.stdou
-00018a40: 745f 6279 7465 7320 6973 206e 6f74 204e  t_bytes is not N
-00018a50: 6f6e 650a 0a20 2020 2020 2020 2061 7373  one..        ass
-00018a60: 6572 7420 222d 2070 6173 735c 6e2b 2020  ert "- pass\n+  
-00018a70: 7061 7373 5c6e 2220 696e 2072 6573 756c  pass\n" in resul
-00018a80: 742e 7374 646f 7574 5f62 7974 6573 2e64  t.stdout_bytes.d
-00018a90: 6563 6f64 6528 290a 0a20 2020 2064 6566  ecode()..    def
-00018aa0: 2074 6573 745f 7079 696e 6b5f 6469 7361   test_pyink_disa
-00018ab0: 626c 6528 7365 6c66 2920 2d3e 204e 6f6e  ble(self) -> Non
-00018ac0: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
-00018ad0: 3d20 5448 4953 5f44 4952 202f 2022 6461  = THIS_DIR / "da
-00018ae0: 7461 2220 2f20 2270 7969 6e6b 5f63 6f6e  ta" / "pyink_con
-00018af0: 6669 6773 220a 2020 2020 2020 2020 6578  figs".        ex
-00018b00: 616d 706c 6520 3d20 7374 7228 7061 7468  ample = str(path
-00018b10: 202f 2022 6578 616d 706c 652e 7079 2229   / "example.py")
-00018b20: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
-00018b30: 3d20 7374 7228 7061 7468 202f 2022 6469  = str(path / "di
-00018b40: 7361 626c 652e 746f 6d6c 2229 0a20 2020  sable.toml").   
-00018b50: 2020 2020 2072 6573 756c 7420 3d20 426c       result = Bl
-00018b60: 6163 6b52 756e 6e65 7228 292e 696e 766f  ackRunner().invo
-00018b70: 6b65 280a 2020 2020 2020 2020 2020 2020  ke(.            
-00018b80: 7079 696e 6b2e 6d61 696e 2c20 5b22 2d2d  pyink.main, ["--
-00018b90: 6469 6666 222c 2022 2d2d 636f 6e66 6967  diff", "--config
-00018ba0: 222c 2063 6f6e 6669 672c 2065 7861 6d70  ", config, examp
-00018bb0: 6c65 5d0a 2020 2020 2020 2020 290a 2020  le].        ).  
-00018bc0: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
-00018bd0: 756c 742e 6578 6974 5f63 6f64 6520 3d3d  ult.exit_code ==
-00018be0: 2030 0a20 2020 2020 2020 2061 7373 6572   0.        asser
-00018bf0: 7420 7265 7375 6c74 2e73 7464 6f75 745f  t result.stdout_
-00018c00: 6279 7465 7320 6973 206e 6f74 204e 6f6e  bytes is not Non
-00018c10: 650a 0a20 2020 2020 2020 2073 7464 6f75  e..        stdou
-00018c20: 7420 3d20 7265 7375 6c74 2e73 7464 6f75  t = result.stdou
-00018c30: 745f 6279 7465 732e 6465 636f 6465 2829  t_bytes.decode()
-00018c40: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00018c50: 280a 2020 2020 2020 2020 2020 2020 2222  (.            ""
-00018c60: 225c 0a2d 6672 6f6d 2076 6572 792e 6c6f  "\.-from very.lo
-00018c70: 6e67 2e70 6163 6b61 6765 2e70 6174 682e  ng.package.path.
-00018c80: 6d79 5f6f 7267 2e6d 795f 7665 7279 5f6c  my_org.my_very_l
-00018c90: 6f6e 675f 7072 6f6a 6563 745f 6e61 6d65  ong_project_name
-00018ca0: 2e61 7765 736f 6d65 5f62 6163 6b65 6e64  .awesome_backend
-00018cb0: 2e63 6f72 655f 6672 616d 6577 6f72 6b2e  .core_framework.
-00018cc0: 7574 696c 2069 6d70 6f72 7420 6d79 5f6c  util import my_l
-00018cd0: 6f6e 675f 6d6f 6475 6c65 5f6e 616d 650a  ong_module_name.
-00018ce0: 2b66 726f 6d20 7665 7279 2e6c 6f6e 672e  +from very.long.
-00018cf0: 7061 636b 6167 652e 7061 7468 2e6d 795f  package.path.my_
-00018d00: 6f72 672e 6d79 5f76 6572 795f 6c6f 6e67  org.my_very_long
-00018d10: 5f70 726f 6a65 6374 5f6e 616d 652e 6177  _project_name.aw
-00018d20: 6573 6f6d 655f 6261 636b 656e 642e 636f  esome_backend.co
-00018d30: 7265 5f66 7261 6d65 776f 726b 2e75 7469  re_framework.uti
-00018d40: 6c20 696d 706f 7274 2028 0a2b 2020 2020  l import (.+    
-00018d50: 6d79 5f6c 6f6e 675f 6d6f 6475 6c65 5f6e  my_long_module_n
-00018d60: 616d 652c 0a2b 290a 2222 220a 2020 2020  ame,.+).""".    
-00018d70: 2020 2020 2020 2020 696e 2073 7464 6f75          in stdou
-00018d80: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
-00018d90: 2020 2020 6173 7365 7274 2022 2d20 7061      assert "- pa
-00018da0: 7373 5c6e 2b20 2020 2070 6173 735c 6e22  ss\n+    pass\n"
-00018db0: 2069 6e20 7374 646f 7574 0a0a 2020 2020   in stdout..    
-00018dc0: 6465 6620 7465 7374 5f70 7969 6e6b 5f69  def test_pyink_i
-00018dd0: 6e5f 746f 6f6c 5f62 6c61 636b 2873 656c  n_tool_black(sel
-00018de0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00018df0: 2020 2020 7061 7468 203d 2054 4849 535f      path = THIS_
-00018e00: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
-00018e10: 7079 696e 6b5f 636f 6e66 6967 7322 0a20  pyink_configs". 
-00018e20: 2020 2020 2020 2065 7861 6d70 6c65 203d         example =
-00018e30: 2073 7472 2870 6174 6820 2f20 2265 7861   str(path / "exa
-00018e40: 6d70 6c65 2e70 7922 290a 2020 2020 2020  mple.py").      
-00018e50: 2020 636f 6e66 6967 203d 2073 7472 2870    config = str(p
-00018e60: 6174 6820 2f20 2274 6f6f 6c5f 626c 6163  ath / "tool_blac
-00018e70: 6b2e 746f 6d6c 2229 0a20 2020 2020 2020  k.toml").       
-00018e80: 2072 6573 756c 7420 3d20 426c 6163 6b52   result = BlackR
-00018e90: 756e 6e65 7228 292e 696e 766f 6b65 280a  unner().invoke(.
-00018ea0: 2020 2020 2020 2020 2020 2020 7079 696e              pyin
-00018eb0: 6b2e 6d61 696e 2c20 5b22 2d2d 6469 6666  k.main, ["--diff
-00018ec0: 222c 2022 2d2d 636f 6e66 6967 222c 2063  ", "--config", c
-00018ed0: 6f6e 6669 672c 2065 7861 6d70 6c65 5d0a  onfig, example].
-00018ee0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00018ef0: 2020 6173 7365 7274 2072 6573 756c 742e    assert result.
-00018f00: 6578 6974 5f63 6f64 6520 3d3d 2030 0a20  exit_code == 0. 
-00018f10: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-00018f20: 7375 6c74 2e73 7464 6f75 745f 6279 7465  sult.stdout_byte
-00018f30: 7320 6973 206e 6f74 204e 6f6e 650a 0a20  s is not None.. 
-00018f40: 2020 2020 2020 2061 7373 6572 7420 222d         assert "-
-00018f50: 2070 6173 735c 6e2b 2020 2020 7061 7373   pass\n+    pass
-00018f60: 5c6e 2220 696e 2072 6573 756c 742e 7374  \n" in result.st
-00018f70: 646f 7574 5f62 7974 6573 2e64 6563 6f64  dout_bytes.decod
-00018f80: 6528 290a 0a20 2020 2040 7079 7465 7374  e()..    @pytest
-00018f90: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-00018fa0: 6528 2276 616c 7565 7322 2c20 5b28 2237  e("values", [("7
-00018fb0: 2d37 222c 292c 2028 2231 2d31 222c 2022  -7",), ("1-1", "
-00018fc0: 372d 3722 295d 290a 2020 2020 6465 6620  7-7")]).    def 
-00018fd0: 7465 7374 5f70 7969 6e6b 5f6c 696e 6573  test_pyink_lines
-00018fe0: 2873 656c 662c 2076 616c 7565 7329 202d  (self, values) -
-00018ff0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00019000: 7061 7468 203d 2054 4849 535f 4449 5220  path = THIS_DIR 
-00019010: 2f20 2264 6174 6122 202f 2022 7079 696e  / "data" / "pyin
-00019020: 6b5f 636f 6e66 6967 7322 0a20 2020 2020  k_configs".     
-00019030: 2020 2065 7861 6d70 6c65 203d 2073 7472     example = str
-00019040: 2870 6174 6820 2f20 2265 7861 6d70 6c65  (path / "example
-00019050: 2e70 7922 290a 2020 2020 2020 2020 7079  .py").        py
-00019060: 696e 6b5f 6c69 6e65 735f 6172 6773 203d  ink_lines_args =
-00019070: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-00019080: 7661 6c75 6520 696e 2076 616c 7565 733a  value in values:
-00019090: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
-000190a0: 6e6b 5f6c 696e 6573 5f61 7267 732e 6170  nk_lines_args.ap
-000190b0: 7065 6e64 2866 222d 2d70 7969 6e6b 2d6c  pend(f"--pyink-l
-000190c0: 696e 6573 3d7b 7661 6c75 657d 2229 0a20  ines={value}"). 
-000190d0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000190e0: 426c 6163 6b52 756e 6e65 7228 292e 696e  BlackRunner().in
-000190f0: 766f 6b65 280a 2020 2020 2020 2020 2020  voke(.          
-00019100: 2020 7079 696e 6b2e 6d61 696e 2c20 7079    pyink.main, py
-00019110: 696e 6b5f 6c69 6e65 735f 6172 6773 202b  ink_lines_args +
-00019120: 205b 222d 2d64 6966 6622 2c20 6578 616d   ["--diff", exam
-00019130: 706c 655d 0a20 2020 2020 2020 2029 0a20  ple].        ). 
-00019140: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-00019150: 7375 6c74 2e73 7464 6f75 745f 6279 7465  sult.stdout_byte
-00019160: 7320 6973 206e 6f74 204e 6f6e 650a 2020  s is not None.  
-00019170: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
-00019180: 756c 742e 6578 6974 5f63 6f64 6520 3d3d  ult.exit_code ==
-00019190: 2030 0a20 2020 2020 2020 2061 7373 6572   0.        asser
-000191a0: 7420 7265 7375 6c74 2e73 7464 6f75 745f  t result.stdout_
-000191b0: 6279 7465 7320 6973 206e 6f74 204e 6f6e  bytes is not Non
-000191c0: 650a 0a20 2020 2020 2020 2061 7373 6572  e..        asser
-000191d0: 7420 222d 6672 6f6d 2220 6e6f 7420 696e  t "-from" not in
-000191e0: 2072 6573 756c 742e 7374 6465 7272 5f62   result.stderr_b
-000191f0: 7974 6573 2e64 6563 6f64 6528 290a 2020  ytes.decode().  
-00019200: 2020 2020 2020 6173 7365 7274 2022 2d20        assert "- 
-00019210: 7061 7373 5c6e 2b20 2020 2070 6173 735c  pass\n+    pass\
-00019220: 6e22 2069 6e20 7265 7375 6c74 2e73 7464  n" in result.std
-00019230: 6f75 745f 6279 7465 732e 6465 636f 6465  out_bytes.decode
-00019240: 2829 0a0a 2020 2020 4070 7974 6573 742e  ()..    @pytest.
-00019250: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00019260: 280a 2020 2020 2020 2020 2276 616c 7565  (.        "value
-00019270: 2c6d 6573 7361 6765 222c 0a20 2020 2020  ,message",.     
-00019280: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00019290: 2028 2231 2c32 222c 2022 496e 636f 7272   ("1,2", "Incorr
-000192a0: 6563 7420 2d2d 7079 696e 6b2d 6c69 6e65  ect --pyink-line
-000192b0: 7320 666f 726d 6174 2c20 6578 7065 6374  s format, expect
-000192c0: 2027 5354 4152 542d 454e 4427 2229 2c0a   'START-END'"),.
-000192d0: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000192f0: 7461 7274 2d65 6e64 222c 0a20 2020 2020  tart-end",.     
-00019300: 2020 2020 2020 2020 2020 2022 496e 636f             "Inco
-00019310: 7272 6563 7420 2d2d 7079 696e 6b2d 6c69  rrect --pyink-li
-00019320: 6e65 7320 7661 6c75 652c 2065 7870 6563  nes value, expec
-00019330: 7420 696e 7465 6765 7220 7261 6e67 6573  t integer ranges
-00019340: 2c20 666f 756e 6422 2c0a 2020 2020 2020  , found",.      
-00019350: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00019360: 205d 2c0a 2020 2020 290a 2020 2020 6465   ],.    ).    de
-00019370: 6620 7465 7374 5f70 7969 6e6b 5f6c 696e  f test_pyink_lin
-00019380: 6573 5f69 6e63 6f72 7265 6374 2873 656c  es_incorrect(sel
-00019390: 662c 2076 616c 7565 2c20 6d65 7373 6167  f, value, messag
-000193a0: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
-000193b0: 2020 2020 7061 7468 203d 2054 4849 535f      path = THIS_
-000193c0: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
-000193d0: 7079 696e 6b5f 636f 6e66 6967 7322 0a20  pyink_configs". 
-000193e0: 2020 2020 2020 2065 7861 6d70 6c65 203d         example =
-000193f0: 2073 7472 2870 6174 6820 2f20 2265 7861   str(path / "exa
-00019400: 6d70 6c65 2e70 7922 290a 2020 2020 2020  mple.py").      
-00019410: 2020 7265 7375 6c74 203d 2042 6c61 636b    result = Black
-00019420: 5275 6e6e 6572 2829 2e69 6e76 6f6b 6528  Runner().invoke(
-00019430: 7079 696e 6b2e 6d61 696e 2c20 5b66 222d  pyink.main, [f"-
-00019440: 2d70 7969 6e6b 2d6c 696e 6573 3d7b 7661  -pyink-lines={va
-00019450: 6c75 657d 222c 2065 7861 6d70 6c65 5d29  lue}", example])
-00019460: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00019470: 7265 7375 6c74 2e65 7869 745f 636f 6465  result.exit_code
-00019480: 203d 3d20 310a 2020 2020 2020 2020 6173   == 1.        as
-00019490: 7365 7274 2072 6573 756c 742e 7374 6465  sert result.stde
-000194a0: 7272 5f62 7974 6573 2069 7320 6e6f 7420  rr_bytes is not 
-000194b0: 4e6f 6e65 0a0a 2020 2020 2020 2020 6173  None..        as
-000194c0: 7365 7274 206d 6573 7361 6765 2069 6e20  sert message in 
-000194d0: 7265 7375 6c74 2e73 7464 6572 725f 6279  result.stderr_by
-000194e0: 7465 732e 6465 636f 6465 2829 0a0a 2020  tes.decode()..  
-000194f0: 2020 6465 6620 7465 7374 5f70 7969 6e6b    def test_pyink
-00019500: 5f75 7365 5f6d 616a 6f72 6974 795f 7175  _use_majority_qu
-00019510: 6f74 6573 2873 656c 6629 202d 3e20 4e6f  otes(self) -> No
-00019520: 6e65 3a0a 2020 2020 2020 2020 7061 7468  ne:.        path
-00019530: 203d 2054 4849 535f 4449 5220 2f20 2264   = THIS_DIR / "d
-00019540: 6174 6122 202f 2022 7079 696e 6b5f 636f  ata" / "pyink_co
-00019550: 6e66 6967 7322 0a20 2020 2020 2020 2065  nfigs".        e
-00019560: 7861 6d70 6c65 203d 2073 7472 2870 6174  xample = str(pat
-00019570: 6820 2f20 226d 616a 6f72 6974 795f 7175  h / "majority_qu
-00019580: 6f74 6573 2e70 7922 290a 2020 2020 2020  otes.py").      
-00019590: 2020 636f 6e66 6967 203d 2073 7472 2870    config = str(p
-000195a0: 6174 6820 2f20 226d 616a 6f72 6974 795f  ath / "majority_
-000195b0: 7175 6f74 6573 2e74 6f6d 6c22 290a 2020  quotes.toml").  
-000195c0: 2020 2020 2020 7265 7375 6c74 203d 2042        result = B
-000195d0: 6c61 636b 5275 6e6e 6572 2829 2e69 6e76  lackRunner().inv
-000195e0: 6f6b 6528 0a20 2020 2020 2020 2020 2020  oke(.           
-000195f0: 2070 7969 6e6b 2e6d 6169 6e2c 205b 222d   pyink.main, ["-
-00019600: 2d64 6966 6622 2c20 222d 2d63 6f6e 6669  -diff", "--confi
-00019610: 6722 2c20 636f 6e66 6967 2c20 6578 616d  g", config, exam
-00019620: 706c 655d 0a20 2020 2020 2020 2029 0a20  ple].        ). 
-00019630: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-00019640: 7375 6c74 2e65 7869 745f 636f 6465 203d  sult.exit_code =
-00019650: 3d20 300a 2020 2020 2020 2020 6173 7365  = 0.        asse
-00019660: 7274 2072 6573 756c 742e 7374 646f 7574  rt result.stdout
-00019670: 5f62 7974 6573 2069 7320 6e6f 7420 4e6f  _bytes is not No
-00019680: 6e65 0a0a 2020 2020 2020 2020 6469 6666  ne..        diff
-00019690: 203d 2022 2222 2d5f 646f 7562 6c65 203d   = """-_double =
-000196a0: 2022 446f 7562 6c65 225c 6e2b 5f64 6f75   "Double"\n+_dou
-000196b0: 626c 6520 3d20 2744 6f75 626c 6527 5c6e  ble = 'Double'\n
-000196c0: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
-000196d0: 7274 2064 6966 6620 696e 2072 6573 756c  rt diff in resul
-000196e0: 742e 7374 646f 7574 5f62 7974 6573 2e64  t.stdout_bytes.d
-000196f0: 6563 6f64 6528 290a 0a0a 7472 793a 0a20  ecode()...try:. 
-00019700: 2020 2077 6974 6820 6f70 656e 2870 7969     with open(pyi
-00019710: 6e6b 2e5f 5f66 696c 655f 5f2c 2022 7222  nk.__file__, "r"
-00019720: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00019730: 3822 2920 6173 205f 6266 3a0a 2020 2020  8") as _bf:.    
-00019740: 2020 2020 626c 6163 6b5f 736f 7572 6365      black_source
-00019750: 5f6c 696e 6573 203d 205f 6266 2e72 6561  _lines = _bf.rea
-00019760: 646c 696e 6573 2829 0a65 7863 6570 7420  dlines().except 
-00019770: 556e 6963 6f64 6544 6563 6f64 6545 7272  UnicodeDecodeErr
-00019780: 6f72 3a0a 2020 2020 6966 206e 6f74 2070  or:.    if not p
-00019790: 7969 6e6b 2e43 4f4d 5049 4c45 443a 0a20  yink.COMPILED:. 
-000197a0: 2020 2020 2020 2072 6169 7365 0a0a 0a64         raise...d
-000197b0: 6566 2074 7261 6365 6675 6e63 280a 2020  ef tracefunc(.  
-000197c0: 2020 6672 616d 653a 2074 7970 6573 2e46    frame: types.F
-000197d0: 7261 6d65 5479 7065 2c20 6576 656e 743a  rameType, event:
-000197e0: 2073 7472 2c20 6172 673a 2041 6e79 0a29   str, arg: Any.)
-000197f0: 202d 3e20 4361 6c6c 6162 6c65 5b5b 7479   -> Callable[[ty
-00019800: 7065 732e 4672 616d 6554 7970 652c 2073  pes.FrameType, s
-00019810: 7472 2c20 416e 795d 2c20 416e 795d 3a0a  tr, Any], Any]:.
-00019820: 2020 2020 2222 2253 686f 7720 6675 6e63      """Show func
-00019830: 7469 6f6e 2063 616c 6c73 2060 6672 6f6d  tion calls `from
-00019840: 2070 7969 6e6b 2f5f 5f69 6e69 745f 5f2e   pyink/__init__.
-00019850: 7079 6020 6173 2074 6865 7920 6861 7070  py` as they happ
-00019860: 656e 2e0a 0a20 2020 2052 6567 6973 7465  en...    Registe
-00019870: 7220 7468 6973 2077 6974 6820 6073 7973  r this with `sys
-00019880: 2e73 6574 7472 6163 6528 2960 2069 6e20  .settrace()` in 
-00019890: 6120 7465 7374 2079 6f75 2772 6520 6465  a test you're de
-000198a0: 6275 6767 696e 672e 0a20 2020 2022 2222  bugging..    """
-000198b0: 0a20 2020 2069 6620 6576 656e 7420 213d  .    if event !=
-000198c0: 2022 6361 6c6c 223a 0a20 2020 2020 2020   "call":.       
-000198d0: 2072 6574 7572 6e20 7472 6163 6566 756e   return tracefun
-000198e0: 630a 0a20 2020 2073 7461 636b 203d 206c  c..    stack = l
-000198f0: 656e 2869 6e73 7065 6374 2e73 7461 636b  en(inspect.stack
-00019900: 2829 2920 2d20 3139 0a20 2020 2073 7461  ()) - 19.    sta
-00019910: 636b 202a 3d20 320a 2020 2020 6669 6c65  ck *= 2.    file
-00019920: 6e61 6d65 203d 2066 7261 6d65 2e66 5f63  name = frame.f_c
-00019930: 6f64 652e 636f 5f66 696c 656e 616d 650a  ode.co_filename.
-00019940: 2020 2020 6c69 6e65 6e6f 203d 2066 7261      lineno = fra
-00019950: 6d65 2e66 5f6c 696e 656e 6f0a 2020 2020  me.f_lineno.    
-00019960: 6675 6e63 5f73 6967 5f6c 696e 656e 6f20  func_sig_lineno 
-00019970: 3d20 6c69 6e65 6e6f 202d 2031 0a20 2020  = lineno - 1.   
-00019980: 2066 756e 636e 616d 6520 3d20 626c 6163   funcname = blac
-00019990: 6b5f 736f 7572 6365 5f6c 696e 6573 5b66  k_source_lines[f
-000199a0: 756e 635f 7369 675f 6c69 6e65 6e6f 5d2e  unc_sig_lineno].
-000199b0: 7374 7269 7028 290a 2020 2020 7768 696c  strip().    whil
-000199c0: 6520 6675 6e63 6e61 6d65 2e73 7461 7274  e funcname.start
-000199d0: 7377 6974 6828 2240 2229 3a0a 2020 2020  swith("@"):.    
-000199e0: 2020 2020 6675 6e63 5f73 6967 5f6c 696e      func_sig_lin
-000199f0: 656e 6f20 2b3d 2031 0a20 2020 2020 2020  eno += 1.       
-00019a00: 2066 756e 636e 616d 6520 3d20 626c 6163   funcname = blac
-00019a10: 6b5f 736f 7572 6365 5f6c 696e 6573 5b66  k_source_lines[f
-00019a20: 756e 635f 7369 675f 6c69 6e65 6e6f 5d2e  unc_sig_lineno].
-00019a30: 7374 7269 7028 290a 2020 2020 6966 2022  strip().    if "
-00019a40: 7079 696e 6b2f 5f5f 696e 6974 5f5f 2e70  pyink/__init__.p
-00019a50: 7922 2069 6e20 6669 6c65 6e61 6d65 3a0a  y" in filename:.
-00019a60: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00019a70: 7b27 2027 202a 2073 7461 636b 7d7b 6c69  {' ' * stack}{li
-00019a80: 6e65 6e6f 7d3a 7b66 756e 636e 616d 657d  neno}:{funcname}
-00019a90: 2229 0a20 2020 2072 6574 7572 6e20 7472  ").    return tr
-00019aa0: 6163 6566 756e 630a                      acefunc.
+00014cb0: 2020 2020 6361 6368 6564 203d 2028 7061      cached = (pa
+00014cc0: 7468 202f 2022 6361 6368 6564 2229 2e72  th / "cached").r
+00014cd0: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
+00014ce0: 2020 2020 2063 6163 6865 645f 6275 745f       cached_but_
+00014cf0: 6368 616e 6765 6420 3d20 2870 6174 6820  changed = (path 
+00014d00: 2f20 2263 6861 6e67 6564 2229 2e72 6573  / "changed").res
+00014d10: 6f6c 7665 2829 0a20 2020 2020 2020 2020  olve().         
+00014d20: 2020 2075 6e63 6163 6865 642e 746f 7563     uncached.touc
+00014d30: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
+00014d40: 6361 6368 6564 2e74 6f75 6368 2829 0a20  cached.touch(). 
+00014d50: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00014d60: 645f 6275 745f 6368 616e 6765 642e 746f  d_but_changed.to
+00014d70: 7563 6828 290a 2020 2020 2020 2020 2020  uch().          
+00014d80: 2020 6361 6368 6520 3d20 7b0a 2020 2020    cache = {.    
+00014d90: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00014da0: 6361 6368 6564 293a 2070 7969 6e6b 2e67  cached): pyink.g
+00014db0: 6574 5f63 6163 6865 5f69 6e66 6f28 6361  et_cache_info(ca
+00014dc0: 6368 6564 292c 0a20 2020 2020 2020 2020  ched),.         
+00014dd0: 2020 2020 2020 2073 7472 2863 6163 6865         str(cache
+00014de0: 645f 6275 745f 6368 616e 6765 6429 3a20  d_but_changed): 
+00014df0: 2830 2e30 2c20 3029 2c0a 2020 2020 2020  (0.0, 0),.      
+00014e00: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00014e10: 2020 2020 746f 646f 2c20 646f 6e65 203d      todo, done =
+00014e20: 2070 7969 6e6b 2e63 6163 6865 2e66 696c   pyink.cache.fil
+00014e30: 7465 725f 6361 6368 6564 280a 2020 2020  ter_cached(.    
+00014e40: 2020 2020 2020 2020 2020 2020 6361 6368              cach
+00014e50: 652c 207b 756e 6361 6368 6564 2c20 6361  e, {uncached, ca
+00014e60: 6368 6564 2c20 6361 6368 6564 5f62 7574  ched, cached_but
+00014e70: 5f63 6861 6e67 6564 7d0a 2020 2020 2020  _changed}.      
+00014e80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00014e90: 2020 2020 6173 7365 7274 2074 6f64 6f20      assert todo 
+00014ea0: 3d3d 207b 756e 6361 6368 6564 2c20 6361  == {uncached, ca
+00014eb0: 6368 6564 5f62 7574 5f63 6861 6e67 6564  ched_but_changed
+00014ec0: 7d0a 2020 2020 2020 2020 2020 2020 6173  }.            as
+00014ed0: 7365 7274 2064 6f6e 6520 3d3d 207b 6361  sert done == {ca
+00014ee0: 6368 6564 7d0a 0a20 2020 2064 6566 2074  ched}..    def t
+00014ef0: 6573 745f 7772 6974 655f 6361 6368 655f  est_write_cache_
+00014f00: 6372 6561 7465 735f 6469 7265 6374 6f72  creates_director
+00014f10: 795f 6966 5f6e 6565 6465 6428 7365 6c66  y_if_needed(self
+00014f20: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014f30: 2020 206d 6f64 6520 3d20 4445 4641 554c     mode = DEFAUL
+00014f40: 545f 4d4f 4445 0a20 2020 2020 2020 2077  T_MODE.        w
+00014f50: 6974 6820 6361 6368 655f 6469 7228 6578  ith cache_dir(ex
+00014f60: 6973 7473 3d46 616c 7365 2920 6173 2077  ists=False) as w
+00014f70: 6f72 6b73 7061 6365 3a0a 2020 2020 2020  orkspace:.      
+00014f80: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
+00014f90: 2077 6f72 6b73 7061 6365 2e65 7869 7374   workspace.exist
+00014fa0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00014fb0: 7079 696e 6b2e 7772 6974 655f 6361 6368  pyink.write_cach
+00014fc0: 6528 7b7d 2c20 5b5d 2c20 6d6f 6465 290a  e({}, [], mode).
+00014fd0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00014fe0: 7274 2077 6f72 6b73 7061 6365 2e65 7869  rt workspace.exi
+00014ff0: 7374 7328 290a 0a20 2020 2040 6576 656e  sts()..    @even
+00015000: 745f 6c6f 6f70 2829 0a20 2020 2064 6566  t_loop().    def
+00015010: 2074 6573 745f 6661 696c 6564 5f66 6f72   test_failed_for
+00015020: 6d61 7474 696e 675f 646f 6573 5f6e 6f74  matting_does_not
+00015030: 5f67 6574 5f63 6163 6865 6428 7365 6c66  _get_cached(self
+00015040: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00015050: 2020 206d 6f64 6520 3d20 4445 4641 554c     mode = DEFAUL
+00015060: 545f 4d4f 4445 0a20 2020 2020 2020 2077  T_MODE.        w
+00015070: 6974 6820 6361 6368 655f 6469 7228 2920  ith cache_dir() 
+00015080: 6173 2077 6f72 6b73 7061 6365 2c20 7061  as workspace, pa
+00015090: 7463 6828 0a20 2020 2020 2020 2020 2020  tch(.           
+000150a0: 2022 636f 6e63 7572 7265 6e74 2e66 7574   "concurrent.fut
+000150b0: 7572 6573 2e50 726f 6365 7373 506f 6f6c  ures.ProcessPool
+000150c0: 4578 6563 7574 6f72 222c 206e 6577 3d54  Executor", new=T
+000150d0: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+000150e0: 720a 2020 2020 2020 2020 293a 0a20 2020  r.        ):.   
+000150f0: 2020 2020 2020 2020 2066 6169 6c69 6e67           failing
+00015100: 203d 2028 776f 726b 7370 6163 6520 2f20   = (workspace / 
+00015110: 2266 6169 6c69 6e67 2e70 7922 292e 7265  "failing.py").re
+00015120: 736f 6c76 6528 290a 2020 2020 2020 2020  solve().        
+00015130: 2020 2020 7769 7468 2066 6169 6c69 6e67      with failing
+00015140: 2e6f 7065 6e28 2277 2229 2061 7320 666f  .open("w") as fo
+00015150: 626a 3a0a 2020 2020 2020 2020 2020 2020  bj:.            
+00015160: 2020 2020 666f 626a 2e77 7269 7465 2822      fobj.write("
+00015170: 6e6f 7420 6163 7475 616c 6c79 2070 7974  not actually pyt
+00015180: 686f 6e22 290a 2020 2020 2020 2020 2020  hon").          
+00015190: 2020 636c 6561 6e20 3d20 2877 6f72 6b73    clean = (works
+000151a0: 7061 6365 202f 2022 636c 6561 6e2e 7079  pace / "clean.py
+000151b0: 2229 2e72 6573 6f6c 7665 2829 0a20 2020  ").resolve().   
+000151c0: 2020 2020 2020 2020 2077 6974 6820 636c           with cl
+000151d0: 6561 6e2e 6f70 656e 2822 7722 2920 6173  ean.open("w") as
+000151e0: 2066 6f62 6a3a 0a20 2020 2020 2020 2020   fobj:.         
+000151f0: 2020 2020 2020 2066 6f62 6a2e 7772 6974         fobj.writ
+00015200: 6528 2770 7269 6e74 2822 6865 6c6c 6f22  e('print("hello"
+00015210: 295c 6e27 290a 2020 2020 2020 2020 2020  )\n').          
+00015220: 2020 696e 766f 6b65 426c 6163 6b28 5b73    invokeBlack([s
+00015230: 7472 2877 6f72 6b73 7061 6365 295d 2c20  tr(workspace)], 
+00015240: 6578 6974 5f63 6f64 653d 3132 3329 0a20  exit_code=123). 
+00015250: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00015260: 203d 2070 7969 6e6b 2e72 6561 645f 6361   = pyink.read_ca
+00015270: 6368 6528 6d6f 6465 290a 2020 2020 2020  che(mode).      
+00015280: 2020 2020 2020 6173 7365 7274 2073 7472        assert str
+00015290: 2866 6169 6c69 6e67 2920 6e6f 7420 696e  (failing) not in
+000152a0: 2063 6163 6865 0a20 2020 2020 2020 2020   cache.         
+000152b0: 2020 2061 7373 6572 7420 7374 7228 636c     assert str(cl
+000152c0: 6561 6e29 2069 6e20 6361 6368 650a 0a20  ean) in cache.. 
+000152d0: 2020 2064 6566 2074 6573 745f 7772 6974     def test_writ
+000152e0: 655f 6361 6368 655f 7772 6974 655f 6661  e_cache_write_fa
+000152f0: 696c 2873 656c 6629 202d 3e20 4e6f 6e65  il(self) -> None
+00015300: 3a0a 2020 2020 2020 2020 6d6f 6465 203d  :.        mode =
+00015310: 2044 4546 4155 4c54 5f4d 4f44 450a 2020   DEFAULT_MODE.  
+00015320: 2020 2020 2020 7769 7468 2063 6163 6865        with cache
+00015330: 5f64 6972 2829 2c20 7061 7463 682e 6f62  _dir(), patch.ob
+00015340: 6a65 6374 2850 6174 682c 2022 6f70 656e  ject(Path, "open
+00015350: 2229 2061 7320 6d6f 636b 3a0a 2020 2020  ") as mock:.    
+00015360: 2020 2020 2020 2020 6d6f 636b 2e73 6964          mock.sid
+00015370: 655f 6566 6665 6374 203d 204f 5345 7272  e_effect = OSErr
+00015380: 6f72 0a20 2020 2020 2020 2020 2020 2070  or.            p
+00015390: 7969 6e6b 2e77 7269 7465 5f63 6163 6865  yink.write_cache
+000153a0: 287b 7d2c 205b 5d2c 206d 6f64 6529 0a0a  ({}, [], mode)..
+000153b0: 2020 2020 6465 6620 7465 7374 5f72 6561      def test_rea
+000153c0: 645f 6361 6368 655f 6c69 6e65 5f6c 656e  d_cache_line_len
+000153d0: 6774 6873 2873 656c 6629 202d 3e20 4e6f  gths(self) -> No
+000153e0: 6e65 3a0a 2020 2020 2020 2020 6d6f 6465  ne:.        mode
+000153f0: 203d 2044 4546 4155 4c54 5f4d 4f44 450a   = DEFAULT_MODE.
+00015400: 2020 2020 2020 2020 7368 6f72 745f 6d6f          short_mo
+00015410: 6465 203d 2072 6570 6c61 6365 2844 4546  de = replace(DEF
+00015420: 4155 4c54 5f4d 4f44 452c 206c 696e 655f  AULT_MODE, line_
+00015430: 6c65 6e67 7468 3d31 290a 2020 2020 2020  length=1).      
+00015440: 2020 7769 7468 2063 6163 6865 5f64 6972    with cache_dir
+00015450: 2829 2061 7320 776f 726b 7370 6163 653a  () as workspace:
+00015460: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00015470: 6820 3d20 2877 6f72 6b73 7061 6365 202f  h = (workspace /
+00015480: 2022 6669 6c65 2e70 7922 292e 7265 736f   "file.py").reso
+00015490: 6c76 6528 290a 2020 2020 2020 2020 2020  lve().          
+000154a0: 2020 7061 7468 2e74 6f75 6368 2829 0a20    path.touch(). 
+000154b0: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
+000154c0: 2e77 7269 7465 5f63 6163 6865 287b 7d2c  .write_cache({},
+000154d0: 205b 7061 7468 5d2c 206d 6f64 6529 0a20   [path], mode). 
+000154e0: 2020 2020 2020 2020 2020 206f 6e65 203d             one =
+000154f0: 2070 7969 6e6b 2e72 6561 645f 6361 6368   pyink.read_cach
+00015500: 6528 6d6f 6465 290a 2020 2020 2020 2020  e(mode).        
+00015510: 2020 2020 6173 7365 7274 2073 7472 2870      assert str(p
+00015520: 6174 6829 2069 6e20 6f6e 650a 2020 2020  ath) in one.    
+00015530: 2020 2020 2020 2020 7477 6f20 3d20 7079          two = py
+00015540: 696e 6b2e 7265 6164 5f63 6163 6865 2873  ink.read_cache(s
+00015550: 686f 7274 5f6d 6f64 6529 0a20 2020 2020  hort_mode).     
+00015560: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
+00015570: 7228 7061 7468 2920 6e6f 7420 696e 2074  r(path) not in t
+00015580: 776f 0a0a 0a64 6566 2061 7373 6572 745f  wo...def assert_
+00015590: 636f 6c6c 6563 7465 645f 736f 7572 6365  collected_source
+000155a0: 7328 0a20 2020 2073 7263 3a20 5365 7175  s(.    src: Sequ
+000155b0: 656e 6365 5b55 6e69 6f6e 5b73 7472 2c20  ence[Union[str, 
+000155c0: 5061 7468 5d5d 2c0a 2020 2020 6578 7065  Path]],.    expe
+000155d0: 6374 6564 3a20 5365 7175 656e 6365 5b55  cted: Sequence[U
+000155e0: 6e69 6f6e 5b73 7472 2c20 5061 7468 5d5d  nion[str, Path]]
+000155f0: 2c0a 2020 2020 2a2c 0a20 2020 2063 7478  ,.    *,.    ctx
+00015600: 3a20 4f70 7469 6f6e 616c 5b46 616b 6543  : Optional[FakeC
+00015610: 6f6e 7465 7874 5d20 3d20 4e6f 6e65 2c0a  ontext] = None,.
+00015620: 2020 2020 6578 636c 7564 653a 204f 7074      exclude: Opt
+00015630: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00015640: 652c 0a20 2020 2069 6e63 6c75 6465 3a20  e,.    include: 
+00015650: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00015660: 4e6f 6e65 2c0a 2020 2020 6578 7465 6e64  None,.    extend
+00015670: 5f65 7863 6c75 6465 3a20 4f70 7469 6f6e  _exclude: Option
+00015680: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00015690: 2020 2020 666f 7263 655f 6578 636c 7564      force_exclud
+000156a0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000156b0: 203d 204e 6f6e 652c 0a20 2020 2073 7464   = None,.    std
+000156c0: 696e 5f66 696c 656e 616d 653a 204f 7074  in_filename: Opt
+000156d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000156e0: 652c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  e,.) -> None:.  
+000156f0: 2020 6773 5f73 7263 203d 2074 7570 6c65    gs_src = tuple
+00015700: 2873 7472 2850 6174 6828 7329 2920 666f  (str(Path(s)) fo
+00015710: 7220 7320 696e 2073 7263 290a 2020 2020  r s in src).    
+00015720: 6773 5f65 7870 6563 7465 6420 3d20 5b50  gs_expected = [P
+00015730: 6174 6828 7329 2066 6f72 2073 2069 6e20  ath(s) for s in 
+00015740: 6578 7065 6374 6564 5d0a 2020 2020 6773  expected].    gs
+00015750: 5f65 7863 6c75 6465 203d 204e 6f6e 6520  _exclude = None 
+00015760: 6966 2065 7863 6c75 6465 2069 7320 4e6f  if exclude is No
+00015770: 6e65 2065 6c73 6520 636f 6d70 696c 655f  ne else compile_
+00015780: 7061 7474 6572 6e28 6578 636c 7564 6529  pattern(exclude)
+00015790: 0a20 2020 2067 735f 696e 636c 7564 6520  .    gs_include 
+000157a0: 3d20 4445 4641 554c 545f 494e 434c 5544  = DEFAULT_INCLUD
+000157b0: 4520 6966 2069 6e63 6c75 6465 2069 7320  E if include is 
+000157c0: 4e6f 6e65 2065 6c73 6520 636f 6d70 696c  None else compil
+000157d0: 655f 7061 7474 6572 6e28 696e 636c 7564  e_pattern(includ
+000157e0: 6529 0a20 2020 2067 735f 6578 7465 6e64  e).    gs_extend
+000157f0: 5f65 7863 6c75 6465 203d 2028 0a20 2020  _exclude = (.   
+00015800: 2020 2020 204e 6f6e 6520 6966 2065 7874       None if ext
+00015810: 656e 645f 6578 636c 7564 6520 6973 204e  end_exclude is N
+00015820: 6f6e 6520 656c 7365 2063 6f6d 7069 6c65  one else compile
+00015830: 5f70 6174 7465 726e 2865 7874 656e 645f  _pattern(extend_
+00015840: 6578 636c 7564 6529 0a20 2020 2029 0a20  exclude).    ). 
+00015850: 2020 2067 735f 666f 7263 655f 6578 636c     gs_force_excl
+00015860: 7564 6520 3d20 4e6f 6e65 2069 6620 666f  ude = None if fo
+00015870: 7263 655f 6578 636c 7564 6520 6973 204e  rce_exclude is N
+00015880: 6f6e 6520 656c 7365 2063 6f6d 7069 6c65  one else compile
+00015890: 5f70 6174 7465 726e 2866 6f72 6365 5f65  _pattern(force_e
+000158a0: 7863 6c75 6465 290a 2020 2020 636f 6c6c  xclude).    coll
+000158b0: 6563 7465 6420 3d20 7079 696e 6b2e 6765  ected = pyink.ge
+000158c0: 745f 736f 7572 6365 7328 0a20 2020 2020  t_sources(.     
+000158d0: 2020 2063 7478 3d63 7478 206f 7220 4661     ctx=ctx or Fa
+000158e0: 6b65 436f 6e74 6578 7428 292c 0a20 2020  keContext(),.   
+000158f0: 2020 2020 2073 7263 3d67 735f 7372 632c       src=gs_src,
+00015900: 0a20 2020 2020 2020 2071 7569 6574 3d46  .        quiet=F
+00015910: 616c 7365 2c0a 2020 2020 2020 2020 7665  alse,.        ve
+00015920: 7262 6f73 653d 4661 6c73 652c 0a20 2020  rbose=False,.   
+00015930: 2020 2020 2069 6e63 6c75 6465 3d67 735f       include=gs_
+00015940: 696e 636c 7564 652c 0a20 2020 2020 2020  include,.       
+00015950: 2065 7863 6c75 6465 3d67 735f 6578 636c   exclude=gs_excl
+00015960: 7564 652c 0a20 2020 2020 2020 2065 7874  ude,.        ext
+00015970: 656e 645f 6578 636c 7564 653d 6773 5f65  end_exclude=gs_e
+00015980: 7874 656e 645f 6578 636c 7564 652c 0a20  xtend_exclude,. 
+00015990: 2020 2020 2020 2066 6f72 6365 5f65 7863         force_exc
+000159a0: 6c75 6465 3d67 735f 666f 7263 655f 6578  lude=gs_force_ex
+000159b0: 636c 7564 652c 0a20 2020 2020 2020 2072  clude,.        r
+000159c0: 6570 6f72 743d 7079 696e 6b2e 5265 706f  eport=pyink.Repo
+000159d0: 7274 2829 2c0a 2020 2020 2020 2020 7374  rt(),.        st
+000159e0: 6469 6e5f 6669 6c65 6e61 6d65 3d73 7464  din_filename=std
+000159f0: 696e 5f66 696c 656e 616d 652c 0a20 2020  in_filename,.   
+00015a00: 2029 0a20 2020 2061 7373 6572 7420 736f   ).    assert so
+00015a10: 7274 6564 2863 6f6c 6c65 6374 6564 2920  rted(collected) 
+00015a20: 3d3d 2073 6f72 7465 6428 6773 5f65 7870  == sorted(gs_exp
+00015a30: 6563 7465 6429 0a0a 0a63 6c61 7373 2054  ected)...class T
+00015a40: 6573 7446 696c 6543 6f6c 6c65 6374 696f  estFileCollectio
+00015a50: 6e3a 0a20 2020 2064 6566 2074 6573 745f  n:.    def test_
+00015a60: 696e 636c 7564 655f 6578 636c 7564 6528  include_exclude(
+00015a70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00015a80: 2020 2020 2020 2070 6174 6820 3d20 5448         path = TH
+00015a90: 4953 5f44 4952 202f 2022 6461 7461 2220  IS_DIR / "data" 
+00015aa0: 2f20 2269 6e63 6c75 6465 5f65 7863 6c75  / "include_exclu
+00015ab0: 6465 5f74 6573 7473 220a 2020 2020 2020  de_tests".      
+00015ac0: 2020 7372 6320 3d20 5b70 6174 685d 0a20    src = [path]. 
+00015ad0: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
+00015ae0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00015af0: 5061 7468 2870 6174 6820 2f20 2262 2f64  Path(path / "b/d
+00015b00: 6f6e 745f 6578 636c 7564 652f 612e 7079  ont_exclude/a.py
+00015b10: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00015b20: 5061 7468 2870 6174 6820 2f20 2262 2f64  Path(path / "b/d
+00015b30: 6f6e 745f 6578 636c 7564 652f 612e 7079  ont_exclude/a.py
+00015b40: 6922 292c 0a20 2020 2020 2020 205d 0a20  i"),.        ]. 
+00015b50: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+00015b60: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+00015b70: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+00015b80: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00015b90: 7065 6374 6564 2c0a 2020 2020 2020 2020  pected,.        
+00015ba0: 2020 2020 696e 636c 7564 653d 7222 5c2e      include=r"\.
+00015bb0: 7079 693f 2422 2c0a 2020 2020 2020 2020  pyi?$",.        
+00015bc0: 2020 2020 6578 636c 7564 653d 7222 2f65      exclude=r"/e
+00015bd0: 7863 6c75 6465 2f7c 2f5c 2e64 6566 696e  xclude/|/\.defin
+00015be0: 6974 656c 795f 6578 636c 7564 652f 222c  itely_exclude/",
+00015bf0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00015c00: 6465 6620 7465 7374 5f67 6974 6967 6e6f  def test_gitigno
+00015c10: 7265 5f75 7365 645f 6173 5f64 6566 6175  re_used_as_defau
+00015c20: 6c74 2873 656c 6629 202d 3e20 4e6f 6e65  lt(self) -> None
+00015c30: 3a0a 2020 2020 2020 2020 6261 7365 203d  :.        base =
+00015c40: 2050 6174 6828 4441 5441 5f44 4952 202f   Path(DATA_DIR /
+00015c50: 2022 696e 636c 7564 655f 6578 636c 7564   "include_exclud
+00015c60: 655f 7465 7374 7322 290a 2020 2020 2020  e_tests").      
+00015c70: 2020 6578 7065 6374 6564 203d 205b 0a20    expected = [. 
+00015c80: 2020 2020 2020 2020 2020 2062 6173 6520             base 
+00015c90: 2f20 2262 2f2e 6465 6669 6e69 7465 6c79  / "b/.definitely
+00015ca0: 5f65 7863 6c75 6465 2f61 2e70 7922 2c0a  _exclude/a.py",.
+00015cb0: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00015cc0: 202f 2022 622f 2e64 6566 696e 6974 656c   / "b/.definitel
+00015cd0: 795f 6578 636c 7564 652f 612e 7079 6922  y_exclude/a.pyi"
+00015ce0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00015cf0: 2020 2020 7372 6320 3d20 5b62 6173 6520      src = [base 
+00015d00: 2f20 2262 2f22 5d0a 2020 2020 2020 2020  / "b/"].        
+00015d10: 6374 7820 3d20 4661 6b65 436f 6e74 6578  ctx = FakeContex
+00015d20: 7428 290a 2020 2020 2020 2020 6374 782e  t().        ctx.
+00015d30: 6f62 6a5b 2272 6f6f 7422 5d20 3d20 6261  obj["root"] = ba
+00015d40: 7365 0a20 2020 2020 2020 2061 7373 6572  se.        asser
+00015d50: 745f 636f 6c6c 6563 7465 645f 736f 7572  t_collected_sour
+00015d60: 6365 7328 7372 632c 2065 7870 6563 7465  ces(src, expecte
+00015d70: 642c 2063 7478 3d63 7478 2c20 6578 7465  d, ctx=ctx, exte
+00015d80: 6e64 5f65 7863 6c75 6465 3d72 222f 6578  nd_exclude=r"/ex
+00015d90: 636c 7564 652f 2229 0a0a 2020 2020 6465  clude/")..    de
+00015da0: 6620 7465 7374 5f67 6974 6967 6e6f 7265  f test_gitignore
+00015db0: 5f75 7365 645f 6f6e 5f6d 756c 7469 706c  _used_on_multipl
+00015dc0: 655f 736f 7572 6365 7328 7365 6c66 2920  e_sources(self) 
+00015dd0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00015de0: 2072 6f6f 7420 3d20 5061 7468 2844 4154   root = Path(DAT
+00015df0: 415f 4449 5220 2f20 2267 6974 6967 6e6f  A_DIR / "gitigno
+00015e00: 7265 5f75 7365 645f 6f6e 5f6d 756c 7469  re_used_on_multi
+00015e10: 706c 655f 736f 7572 6365 7322 290a 2020  ple_sources").  
+00015e20: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+00015e30: 205b 0a20 2020 2020 2020 2020 2020 2072   [.            r
+00015e40: 6f6f 7420 2f20 2264 6972 3122 202f 2022  oot / "dir1" / "
+00015e50: 622e 7079 222c 0a20 2020 2020 2020 2020  b.py",.         
+00015e60: 2020 2072 6f6f 7420 2f20 2264 6972 3222     root / "dir2"
+00015e70: 202f 2022 622e 7079 222c 0a20 2020 2020   / "b.py",.     
+00015e80: 2020 205d 0a20 2020 2020 2020 2063 7478     ].        ctx
+00015e90: 203d 2046 616b 6543 6f6e 7465 7874 2829   = FakeContext()
+00015ea0: 0a20 2020 2020 2020 2063 7478 2e6f 626a  .        ctx.obj
+00015eb0: 5b22 726f 6f74 225d 203d 2072 6f6f 740a  ["root"] = root.
+00015ec0: 2020 2020 2020 2020 7372 6320 3d20 5b72          src = [r
+00015ed0: 6f6f 7420 2f20 2264 6972 3122 2c20 726f  oot / "dir1", ro
+00015ee0: 6f74 202f 2022 6469 7232 225d 0a20 2020  ot / "dir2"].   
+00015ef0: 2020 2020 2061 7373 6572 745f 636f 6c6c       assert_coll
+00015f00: 6563 7465 645f 736f 7572 6365 7328 7372  ected_sources(sr
+00015f10: 632c 2065 7870 6563 7465 642c 2063 7478  c, expected, ctx
+00015f20: 3d63 7478 290a 0a20 2020 2040 7061 7463  =ctx)..    @patc
+00015f30: 6828 2270 7969 6e6b 2e66 696e 645f 7072  h("pyink.find_pr
+00015f40: 6f6a 6563 745f 726f 6f74 222c 206c 616d  oject_root", lam
+00015f50: 6264 6120 2a61 7267 733a 2028 5448 4953  bda *args: (THIS
+00015f60: 5f44 4952 2e72 6573 6f6c 7665 2829 2c20  _DIR.resolve(), 
+00015f70: 4e6f 6e65 2929 0a20 2020 2064 6566 2074  None)).    def t
+00015f80: 6573 745f 6578 636c 7564 655f 666f 725f  est_exclude_for_
+00015f90: 6973 7375 655f 3135 3732 2873 656c 6629  issue_1572(self)
+00015fa0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00015fb0: 2020 2320 4578 636c 7564 6520 7368 6f75    # Exclude shou
+00015fc0: 6c64 6e27 7420 746f 7563 6820 6669 6c65  ldn't touch file
+00015fd0: 7320 7468 6174 2077 6572 6520 6578 706c  s that were expl
+00015fe0: 6963 6974 6c79 2067 6976 656e 2074 6f20  icitly given to 
+00015ff0: 426c 6163 6b20 7468 726f 7567 6820 7468  Black through th
+00016000: 650a 2020 2020 2020 2020 2320 434c 492e  e.        # CLI.
+00016010: 2045 7863 6c75 6465 2069 7320 7375 7070   Exclude is supp
+00016020: 6f73 6564 2074 6f20 6f6e 6c79 2061 7070  osed to only app
+00016030: 6c79 2074 6f20 7468 6520 7265 6375 7273  ly to the recurs
+00016040: 6976 6520 6469 7363 6f76 6572 7920 6f66  ive discovery of
+00016050: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
+00016060: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
+00016070: 2e63 6f6d 2f70 7366 2f62 6c61 636b 2f69  .com/psf/black/i
+00016080: 7373 7565 732f 3135 3732 0a20 2020 2020  ssues/1572.     
+00016090: 2020 2070 6174 6820 3d20 4441 5441 5f44     path = DATA_D
+000160a0: 4952 202f 2022 696e 636c 7564 655f 6578  IR / "include_ex
+000160b0: 636c 7564 655f 7465 7374 7322 0a20 2020  clude_tests".   
+000160c0: 2020 2020 2073 7263 203d 205b 7061 7468       src = [path
+000160d0: 202f 2022 622f 6578 636c 7564 652f 612e   / "b/exclude/a.
+000160e0: 7079 225d 0a20 2020 2020 2020 2065 7870  py"].        exp
+000160f0: 6563 7465 6420 3d20 5b70 6174 6820 2f20  ected = [path / 
+00016100: 2262 2f65 7863 6c75 6465 2f61 2e70 7922  "b/exclude/a.py"
+00016110: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
+00016120: 5f63 6f6c 6c65 6374 6564 5f73 6f75 7263  _collected_sourc
+00016130: 6573 2873 7263 2c20 6578 7065 6374 6564  es(src, expected
+00016140: 2c20 696e 636c 7564 653d 2222 2c20 6578  , include="", ex
+00016150: 636c 7564 653d 7222 2f65 7863 6c75 6465  clude=r"/exclude
+00016160: 2f7c 615c 2e70 7922 290a 0a20 2020 2064  /|a\.py")..    d
+00016170: 6566 2074 6573 745f 6769 7469 676e 6f72  ef test_gitignor
+00016180: 655f 6578 636c 7564 6528 7365 6c66 2920  e_exclude(self) 
+00016190: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000161a0: 2070 6174 6820 3d20 5448 4953 5f44 4952   path = THIS_DIR
+000161b0: 202f 2022 6461 7461 2220 2f20 2269 6e63   / "data" / "inc
+000161c0: 6c75 6465 5f65 7863 6c75 6465 5f74 6573  lude_exclude_tes
+000161d0: 7473 220a 2020 2020 2020 2020 696e 636c  ts".        incl
+000161e0: 7564 6520 3d20 7265 2e63 6f6d 7069 6c65  ude = re.compile
+000161f0: 2872 225c 2e70 7969 3f24 2229 0a20 2020  (r"\.pyi?$").   
+00016200: 2020 2020 2065 7863 6c75 6465 203d 2072       exclude = r
+00016210: 652e 636f 6d70 696c 6528 7222 2229 0a20  e.compile(r""). 
+00016220: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
+00016230: 7079 696e 6b2e 5265 706f 7274 2829 0a20  pyink.Report(). 
+00016240: 2020 2020 2020 2067 6974 6967 6e6f 7265         gitignore
+00016250: 203d 2050 6174 6853 7065 632e 6672 6f6d   = PathSpec.from
+00016260: 5f6c 696e 6573 280a 2020 2020 2020 2020  _lines(.        
+00016270: 2020 2020 2267 6974 7769 6c64 6d61 7463      "gitwildmatc
+00016280: 6822 2c20 5b22 6578 636c 7564 652f 222c  h", ["exclude/",
+00016290: 2022 2e64 6566 696e 6974 656c 795f 6578   ".definitely_ex
+000162a0: 636c 7564 6522 5d0a 2020 2020 2020 2020  clude"].        
+000162b0: 290a 2020 2020 2020 2020 736f 7572 6365  ).        source
+000162c0: 733a 204c 6973 745b 5061 7468 5d20 3d20  s: List[Path] = 
+000162d0: 5b5d 0a20 2020 2020 2020 2065 7870 6563  [].        expec
+000162e0: 7465 6420 3d20 5b0a 2020 2020 2020 2020  ted = [.        
+000162f0: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+00016300: 2262 2f64 6f6e 745f 6578 636c 7564 652f  "b/dont_exclude/
+00016310: 612e 7079 2229 2c0a 2020 2020 2020 2020  a.py"),.        
+00016320: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+00016330: 2262 2f64 6f6e 745f 6578 636c 7564 652f  "b/dont_exclude/
+00016340: 612e 7079 6922 292c 0a20 2020 2020 2020  a.pyi"),.       
+00016350: 205d 0a20 2020 2020 2020 2074 6869 735f   ].        this_
+00016360: 6162 7320 3d20 5448 4953 5f44 4952 2e72  abs = THIS_DIR.r
+00016370: 6573 6f6c 7665 2829 0a20 2020 2020 2020  esolve().       
+00016380: 2073 6f75 7263 6573 2e65 7874 656e 6428   sources.extend(
+00016390: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
+000163a0: 6e6b 2e67 656e 5f70 7974 686f 6e5f 6669  nk.gen_python_fi
+000163b0: 6c65 7328 0a20 2020 2020 2020 2020 2020  les(.           
+000163c0: 2020 2020 2070 6174 682e 6974 6572 6469       path.iterdi
+000163d0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
+000163e0: 2020 2020 2074 6869 735f 6162 732c 0a20       this_abs,. 
+000163f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00016400: 6e63 6c75 6465 2c0a 2020 2020 2020 2020  nclude,.        
+00016410: 2020 2020 2020 2020 6578 636c 7564 652c          exclude,
+00016420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016430: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00016440: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
+00016450: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00016460: 6f72 742c 0a20 2020 2020 2020 2020 2020  ort,.           
+00016470: 2020 2020 207b 7061 7468 3a20 6769 7469       {path: giti
+00016480: 676e 6f72 657d 2c0a 2020 2020 2020 2020  gnore},.        
+00016490: 2020 2020 2020 2020 7665 7262 6f73 653d          verbose=
+000164a0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+000164b0: 2020 2020 2020 2071 7569 6574 3d46 616c         quiet=Fal
+000164c0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000164d0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+000164e0: 2020 2020 6173 7365 7274 2073 6f72 7465      assert sorte
+000164f0: 6428 6578 7065 6374 6564 2920 3d3d 2073  d(expected) == s
+00016500: 6f72 7465 6428 736f 7572 6365 7329 0a0a  orted(sources)..
+00016510: 2020 2020 6465 6620 7465 7374 5f6e 6573      def test_nes
+00016520: 7465 645f 6769 7469 676e 6f72 6528 7365  ted_gitignore(se
+00016530: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00016540: 2020 2020 2070 6174 6820 3d20 5061 7468       path = Path
+00016550: 2854 4849 535f 4449 5220 2f20 2264 6174  (THIS_DIR / "dat
+00016560: 6122 202f 2022 6e65 7374 6564 5f67 6974  a" / "nested_git
+00016570: 6967 6e6f 7265 5f74 6573 7473 2229 0a20  ignore_tests"). 
+00016580: 2020 2020 2020 2069 6e63 6c75 6465 203d         include =
+00016590: 2072 652e 636f 6d70 696c 6528 7222 5c2e   re.compile(r"\.
+000165a0: 7079 693f 2422 290a 2020 2020 2020 2020  pyi?$").        
+000165b0: 6578 636c 7564 6520 3d20 7265 2e63 6f6d  exclude = re.com
+000165c0: 7069 6c65 2872 2222 290a 2020 2020 2020  pile(r"").      
+000165d0: 2020 726f 6f74 5f67 6974 6967 6e6f 7265    root_gitignore
+000165e0: 203d 2070 7969 6e6b 2e66 696c 6573 2e67   = pyink.files.g
+000165f0: 6574 5f67 6974 6967 6e6f 7265 2870 6174  et_gitignore(pat
+00016600: 6829 0a20 2020 2020 2020 2072 6570 6f72  h).        repor
+00016610: 7420 3d20 7079 696e 6b2e 5265 706f 7274  t = pyink.Report
+00016620: 2829 0a20 2020 2020 2020 2065 7870 6563  ().        expec
+00016630: 7465 643a 204c 6973 745b 5061 7468 5d20  ted: List[Path] 
+00016640: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00016650: 5061 7468 2870 6174 6820 2f20 2278 2e70  Path(path / "x.p
+00016660: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
+00016670: 2050 6174 6828 7061 7468 202f 2022 726f   Path(path / "ro
+00016680: 6f74 2f62 2e70 7922 292c 0a20 2020 2020  ot/b.py"),.     
+00016690: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
+000166a0: 202f 2022 726f 6f74 2f63 2e70 7922 292c   / "root/c.py"),
+000166b0: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
+000166c0: 6828 7061 7468 202f 2022 726f 6f74 2f63  h(path / "root/c
+000166d0: 6869 6c64 2f63 2e70 7922 292c 0a20 2020  hild/c.py"),.   
+000166e0: 2020 2020 205d 0a20 2020 2020 2020 2074       ].        t
+000166f0: 6869 735f 6162 7320 3d20 5448 4953 5f44  his_abs = THIS_D
+00016700: 4952 2e72 6573 6f6c 7665 2829 0a20 2020  IR.resolve().   
+00016710: 2020 2020 2073 6f75 7263 6573 203d 206c       sources = l
+00016720: 6973 7428 0a20 2020 2020 2020 2020 2020  ist(.           
+00016730: 2070 7969 6e6b 2e67 656e 5f70 7974 686f   pyink.gen_pytho
+00016740: 6e5f 6669 6c65 7328 0a20 2020 2020 2020  n_files(.       
+00016750: 2020 2020 2020 2020 2070 6174 682e 6974           path.it
+00016760: 6572 6469 7228 292c 0a20 2020 2020 2020  erdir(),.       
+00016770: 2020 2020 2020 2020 2074 6869 735f 6162           this_ab
+00016780: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00016790: 2020 2069 6e63 6c75 6465 2c0a 2020 2020     include,.    
+000167a0: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+000167b0: 7564 652c 0a20 2020 2020 2020 2020 2020  ude,.           
+000167c0: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
+000167d0: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+000167e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000167f0: 2072 6570 6f72 742c 0a20 2020 2020 2020   report,.       
+00016800: 2020 2020 2020 2020 207b 7061 7468 3a20           {path: 
+00016810: 726f 6f74 5f67 6974 6967 6e6f 7265 7d2c  root_gitignore},
+00016820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016830: 2076 6572 626f 7365 3d46 616c 7365 2c0a   verbose=False,.
+00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016850: 7175 6965 743d 4661 6c73 652c 0a20 2020  quiet=False,.   
+00016860: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00016870: 2020 2029 0a20 2020 2020 2020 2061 7373     ).        ass
+00016880: 6572 7420 736f 7274 6564 2865 7870 6563  ert sorted(expec
+00016890: 7465 6429 203d 3d20 736f 7274 6564 2873  ted) == sorted(s
+000168a0: 6f75 7263 6573 290a 0a20 2020 2064 6566  ources)..    def
+000168b0: 2074 6573 745f 6e65 7374 6564 5f67 6974   test_nested_git
+000168c0: 6967 6e6f 7265 5f64 6972 6563 746c 795f  ignore_directly_
+000168d0: 696e 5f73 6f75 7263 655f 6469 7265 6374  in_source_direct
+000168e0: 6f72 7928 7365 6c66 2920 2d3e 204e 6f6e  ory(self) -> Non
+000168f0: 653a 0a20 2020 2020 2020 2023 2068 7474  e:.        # htt
+00016900: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00016910: 7073 662f 626c 6163 6b2f 6973 7375 6573  psf/black/issues
+00016920: 2f32 3539 380a 2020 2020 2020 2020 7061  /2598.        pa
+00016930: 7468 203d 2050 6174 6828 4441 5441 5f44  th = Path(DATA_D
+00016940: 4952 202f 2022 6e65 7374 6564 5f67 6974  IR / "nested_git
+00016950: 6967 6e6f 7265 5f74 6573 7473 2229 0a20  ignore_tests"). 
+00016960: 2020 2020 2020 2073 7263 203d 2050 6174         src = Pat
+00016970: 6828 7061 7468 202f 2022 726f 6f74 2220  h(path / "root" 
+00016980: 2f20 2263 6869 6c64 2229 0a20 2020 2020  / "child").     
+00016990: 2020 2065 7870 6563 7465 6420 3d20 5b73     expected = [s
+000169a0: 7263 202f 2022 612e 7079 222c 2073 7263  rc / "a.py", src
+000169b0: 202f 2022 632e 7079 225d 0a20 2020 2020   / "c.py"].     
+000169c0: 2020 2061 7373 6572 745f 636f 6c6c 6563     assert_collec
+000169d0: 7465 645f 736f 7572 6365 7328 5b73 7263  ted_sources([src
+000169e0: 5d2c 2065 7870 6563 7465 6429 0a0a 2020  ], expected)..  
+000169f0: 2020 6465 6620 7465 7374 5f69 6e76 616c    def test_inval
+00016a00: 6964 5f67 6974 6967 6e6f 7265 2873 656c  id_gitignore(sel
+00016a10: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00016a20: 2020 2020 7061 7468 203d 2054 4849 535f      path = THIS_
+00016a30: 4449 5220 2f20 2264 6174 6122 202f 2022  DIR / "data" / "
+00016a40: 696e 7661 6c69 645f 6769 7469 676e 6f72  invalid_gitignor
+00016a50: 655f 7465 7374 7322 0a20 2020 2020 2020  e_tests".       
+00016a60: 2065 6d70 7479 5f63 6f6e 6669 6720 3d20   empty_config = 
+00016a70: 7061 7468 202f 2022 7079 7072 6f6a 6563  path / "pyprojec
+00016a80: 742e 746f 6d6c 220a 2020 2020 2020 2020  t.toml".        
+00016a90: 7265 7375 6c74 203d 2042 6c61 636b 5275  result = BlackRu
+00016aa0: 6e6e 6572 2829 2e69 6e76 6f6b 6528 0a20  nner().invoke(. 
+00016ab0: 2020 2020 2020 2020 2020 2070 7969 6e6b             pyink
+00016ac0: 2e6d 6169 6e2c 205b 222d 2d76 6572 626f  .main, ["--verbo
+00016ad0: 7365 222c 2022 2d2d 636f 6e66 6967 222c  se", "--config",
+00016ae0: 2073 7472 2865 6d70 7479 5f63 6f6e 6669   str(empty_confi
+00016af0: 6729 2c20 7374 7228 7061 7468 295d 0a20  g), str(path)]. 
+00016b00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016b10: 2061 7373 6572 7420 7265 7375 6c74 2e65   assert result.e
+00016b20: 7869 745f 636f 6465 203d 3d20 310a 2020  xit_code == 1.  
+00016b30: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+00016b40: 756c 742e 7374 6465 7272 5f62 7974 6573  ult.stderr_bytes
+00016b50: 2069 7320 6e6f 7420 4e6f 6e65 0a0a 2020   is not None..  
+00016b60: 2020 2020 2020 6769 7469 676e 6f72 6520        gitignore 
+00016b70: 3d20 7061 7468 202f 2022 2e67 6974 6967  = path / ".gitig
+00016b80: 6e6f 7265 220a 2020 2020 2020 2020 6173  nore".        as
+00016b90: 7365 7274 2066 2243 6f75 6c64 206e 6f74  sert f"Could not
+00016ba0: 2070 6172 7365 207b 6769 7469 676e 6f72   parse {gitignor
+00016bb0: 657d 2220 696e 2072 6573 756c 742e 7374  e}" in result.st
+00016bc0: 6465 7272 5f62 7974 6573 2e64 6563 6f64  derr_bytes.decod
+00016bd0: 6528 290a 0a20 2020 2064 6566 2074 6573  e()..    def tes
+00016be0: 745f 696e 7661 6c69 645f 6e65 7374 6564  t_invalid_nested
+00016bf0: 5f67 6974 6967 6e6f 7265 2873 656c 6629  _gitignore(self)
+00016c00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00016c10: 2020 7061 7468 203d 2054 4849 535f 4449    path = THIS_DI
+00016c20: 5220 2f20 2264 6174 6122 202f 2022 696e  R / "data" / "in
+00016c30: 7661 6c69 645f 6e65 7374 6564 5f67 6974  valid_nested_git
+00016c40: 6967 6e6f 7265 5f74 6573 7473 220a 2020  ignore_tests".  
+00016c50: 2020 2020 2020 656d 7074 795f 636f 6e66        empty_conf
+00016c60: 6967 203d 2070 6174 6820 2f20 2270 7970  ig = path / "pyp
+00016c70: 726f 6a65 6374 2e74 6f6d 6c22 0a20 2020  roject.toml".   
+00016c80: 2020 2020 2072 6573 756c 7420 3d20 426c       result = Bl
+00016c90: 6163 6b52 756e 6e65 7228 292e 696e 766f  ackRunner().invo
+00016ca0: 6b65 280a 2020 2020 2020 2020 2020 2020  ke(.            
+00016cb0: 7079 696e 6b2e 6d61 696e 2c20 5b22 2d2d  pyink.main, ["--
+00016cc0: 7665 7262 6f73 6522 2c20 222d 2d63 6f6e  verbose", "--con
+00016cd0: 6669 6722 2c20 7374 7228 656d 7074 795f  fig", str(empty_
+00016ce0: 636f 6e66 6967 292c 2073 7472 2870 6174  config), str(pat
+00016cf0: 6829 5d0a 2020 2020 2020 2020 290a 2020  h)].        ).  
+00016d00: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+00016d10: 756c 742e 6578 6974 5f63 6f64 6520 3d3d  ult.exit_code ==
+00016d20: 2031 0a20 2020 2020 2020 2061 7373 6572   1.        asser
+00016d30: 7420 7265 7375 6c74 2e73 7464 6572 725f  t result.stderr_
+00016d40: 6279 7465 7320 6973 206e 6f74 204e 6f6e  bytes is not Non
+00016d50: 650a 0a20 2020 2020 2020 2067 6974 6967  e..        gitig
+00016d60: 6e6f 7265 203d 2070 6174 6820 2f20 2261  nore = path / "a
+00016d70: 2220 2f20 222e 6769 7469 676e 6f72 6522  " / ".gitignore"
+00016d80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00016d90: 6622 436f 756c 6420 6e6f 7420 7061 7273  f"Could not pars
+00016da0: 6520 7b67 6974 6967 6e6f 7265 7d22 2069  e {gitignore}" i
+00016db0: 6e20 7265 7375 6c74 2e73 7464 6572 725f  n result.stderr_
+00016dc0: 6279 7465 732e 6465 636f 6465 2829 0a0a  bytes.decode()..
+00016dd0: 2020 2020 6465 6620 7465 7374 5f67 6974      def test_git
+00016de0: 6967 6e6f 7265 5f74 6861 745f 6967 6e6f  ignore_that_igno
+00016df0: 7265 735f 7375 6266 6f6c 6465 7273 2873  res_subfolders(s
+00016e00: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00016e10: 2020 2020 2020 2320 4966 2067 6974 6967        # If gitig
+00016e20: 6e6f 7265 2077 6974 6820 2a2f 2a20 6973  nore with */* is
+00016e30: 2069 6e20 726f 6f74 0a20 2020 2020 2020   in root.       
+00016e40: 2072 6f6f 7420 3d20 5061 7468 2844 4154   root = Path(DAT
+00016e50: 415f 4449 5220 2f20 2269 676e 6f72 655f  A_DIR / "ignore_
+00016e60: 7375 6266 6f6c 6465 7273 5f67 6974 6967  subfolders_gitig
+00016e70: 6e6f 7265 5f74 6573 7473 2220 2f20 2273  nore_tests" / "s
+00016e80: 7562 6469 7222 290a 2020 2020 2020 2020  ubdir").        
+00016e90: 6578 7065 6374 6564 203d 205b 726f 6f74  expected = [root
+00016ea0: 202f 2022 622e 7079 225d 0a20 2020 2020   / "b.py"].     
+00016eb0: 2020 2063 7478 203d 2046 616b 6543 6f6e     ctx = FakeCon
+00016ec0: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
+00016ed0: 7478 2e6f 626a 5b22 726f 6f74 225d 203d  tx.obj["root"] =
+00016ee0: 2072 6f6f 740a 2020 2020 2020 2020 6173   root.        as
+00016ef0: 7365 7274 5f63 6f6c 6c65 6374 6564 5f73  sert_collected_s
+00016f00: 6f75 7263 6573 285b 726f 6f74 5d2c 2065  ources([root], e
+00016f10: 7870 6563 7465 642c 2063 7478 3d63 7478  xpected, ctx=ctx
+00016f20: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
+00016f30: 2e67 6974 6967 6e6f 7265 2077 6974 6820  .gitignore with 
+00016f40: 2a2f 2a20 6973 206e 6573 7465 640a 2020  */* is nested.  
+00016f50: 2020 2020 2020 726f 6f74 203d 2050 6174        root = Pat
+00016f60: 6828 4441 5441 5f44 4952 202f 2022 6967  h(DATA_DIR / "ig
+00016f70: 6e6f 7265 5f73 7562 666f 6c64 6572 735f  nore_subfolders_
+00016f80: 6769 7469 676e 6f72 655f 7465 7374 7322  gitignore_tests"
+00016f90: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
+00016fa0: 6564 203d 205b 0a20 2020 2020 2020 2020  ed = [.         
+00016fb0: 2020 2072 6f6f 7420 2f20 2261 2e70 7922     root / "a.py"
+00016fc0: 2c0a 2020 2020 2020 2020 2020 2020 726f  ,.            ro
+00016fd0: 6f74 202f 2022 7375 6264 6972 2220 2f20  ot / "subdir" / 
+00016fe0: 2262 2e70 7922 2c0a 2020 2020 2020 2020  "b.py",.        
+00016ff0: 5d0a 2020 2020 2020 2020 6374 7820 3d20  ].        ctx = 
+00017000: 4661 6b65 436f 6e74 6578 7428 290a 2020  FakeContext().  
+00017010: 2020 2020 2020 6374 782e 6f62 6a5b 2272        ctx.obj["r
+00017020: 6f6f 7422 5d20 3d20 726f 6f74 0a20 2020  oot"] = root.   
+00017030: 2020 2020 2061 7373 6572 745f 636f 6c6c       assert_coll
+00017040: 6563 7465 645f 736f 7572 6365 7328 5b72  ected_sources([r
+00017050: 6f6f 745d 2c20 6578 7065 6374 6564 2c20  oot], expected, 
+00017060: 6374 783d 6374 7829 0a0a 2020 2020 2020  ctx=ctx)..      
+00017070: 2020 2320 4966 2063 6f6d 6d61 6e64 2069    # If command i
+00017080: 7320 6578 6563 7574 6564 2066 726f 6d20  s executed from 
+00017090: 6f75 7465 7220 6469 720a 2020 2020 2020  outer dir.      
+000170a0: 2020 726f 6f74 203d 2050 6174 6828 4441    root = Path(DA
+000170b0: 5441 5f44 4952 202f 2022 6967 6e6f 7265  TA_DIR / "ignore
+000170c0: 5f73 7562 666f 6c64 6572 735f 6769 7469  _subfolders_giti
+000170d0: 676e 6f72 655f 7465 7374 7322 290a 2020  gnore_tests").  
+000170e0: 2020 2020 2020 7461 7267 6574 203d 2072        target = r
+000170f0: 6f6f 7420 2f20 2273 7562 6469 7222 0a20  oot / "subdir". 
+00017100: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
+00017110: 3d20 5b74 6172 6765 7420 2f20 2262 2e70  = [target / "b.p
+00017120: 7922 5d0a 2020 2020 2020 2020 6374 7820  y"].        ctx 
+00017130: 3d20 4661 6b65 436f 6e74 6578 7428 290a  = FakeContext().
+00017140: 2020 2020 2020 2020 6374 782e 6f62 6a5b          ctx.obj[
+00017150: 2272 6f6f 7422 5d20 3d20 726f 6f74 0a20  "root"] = root. 
+00017160: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+00017170: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+00017180: 5b74 6172 6765 745d 2c20 6578 7065 6374  [target], expect
+00017190: 6564 2c20 6374 783d 6374 7829 0a0a 2020  ed, ctx=ctx)..  
+000171a0: 2020 6465 6620 7465 7374 5f65 6d70 7479    def test_empty
+000171b0: 5f69 6e63 6c75 6465 2873 656c 6629 202d  _include(self) -
+000171c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000171d0: 7061 7468 203d 2044 4154 415f 4449 5220  path = DATA_DIR 
+000171e0: 2f20 2269 6e63 6c75 6465 5f65 7863 6c75  / "include_exclu
+000171f0: 6465 5f74 6573 7473 220a 2020 2020 2020  de_tests".      
+00017200: 2020 7372 6320 3d20 5b70 6174 685d 0a20    src = [path]. 
+00017210: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
+00017220: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00017230: 5061 7468 2870 6174 6820 2f20 2262 2f65  Path(path / "b/e
+00017240: 7863 6c75 6465 2f61 2e70 6965 2229 2c0a  xclude/a.pie"),.
+00017250: 2020 2020 2020 2020 2020 2020 5061 7468              Path
+00017260: 2870 6174 6820 2f20 2262 2f65 7863 6c75  (path / "b/exclu
+00017270: 6465 2f61 2e70 7922 292c 0a20 2020 2020  de/a.py"),.     
+00017280: 2020 2020 2020 2050 6174 6828 7061 7468         Path(path
+00017290: 202f 2022 622f 6578 636c 7564 652f 612e   / "b/exclude/a.
+000172a0: 7079 6922 292c 0a20 2020 2020 2020 2020  pyi"),.         
+000172b0: 2020 2050 6174 6828 7061 7468 202f 2022     Path(path / "
+000172c0: 622f 646f 6e74 5f65 7863 6c75 6465 2f61  b/dont_exclude/a
+000172d0: 2e70 6965 2229 2c0a 2020 2020 2020 2020  .pie"),.        
+000172e0: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+000172f0: 2262 2f64 6f6e 745f 6578 636c 7564 652f  "b/dont_exclude/
+00017300: 612e 7079 2229 2c0a 2020 2020 2020 2020  a.py"),.        
+00017310: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+00017320: 2262 2f64 6f6e 745f 6578 636c 7564 652f  "b/dont_exclude/
+00017330: 612e 7079 6922 292c 0a20 2020 2020 2020  a.pyi"),.       
+00017340: 2020 2020 2050 6174 6828 7061 7468 202f       Path(path /
+00017350: 2022 622f 2e64 6566 696e 6974 656c 795f   "b/.definitely_
+00017360: 6578 636c 7564 652f 612e 7069 6522 292c  exclude/a.pie"),
+00017370: 0a20 2020 2020 2020 2020 2020 2050 6174  .            Pat
+00017380: 6828 7061 7468 202f 2022 622f 2e64 6566  h(path / "b/.def
+00017390: 696e 6974 656c 795f 6578 636c 7564 652f  initely_exclude/
+000173a0: 612e 7079 2229 2c0a 2020 2020 2020 2020  a.py"),.        
+000173b0: 2020 2020 5061 7468 2870 6174 6820 2f20      Path(path / 
+000173c0: 2262 2f2e 6465 6669 6e69 7465 6c79 5f65  "b/.definitely_e
+000173d0: 7863 6c75 6465 2f61 2e70 7969 2229 2c0a  xclude/a.pyi"),.
+000173e0: 2020 2020 2020 2020 2020 2020 5061 7468              Path
+000173f0: 2870 6174 6820 2f20 222e 6769 7469 676e  (path / ".gitign
+00017400: 6f72 6522 292c 0a20 2020 2020 2020 2020  ore"),.         
+00017410: 2020 2050 6174 6828 7061 7468 202f 2022     Path(path / "
+00017420: 7079 7072 6f6a 6563 742e 746f 6d6c 2229  pyproject.toml")
+00017430: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00017440: 2020 2020 2320 5365 7474 696e 6720 6578      # Setting ex
+00017450: 636c 7564 6520 6578 706c 6963 6974 6c79  clude explicitly
+00017460: 2074 6f20 616e 2065 6d70 7479 2073 7472   to an empty str
+00017470: 696e 6720 746f 2062 6c6f 636b 202e 6769  ing to block .gi
+00017480: 7469 676e 6f72 6520 7573 6167 652e 0a20  tignore usage.. 
+00017490: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+000174a0: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+000174b0: 7372 632c 2065 7870 6563 7465 642c 2069  src, expected, i
+000174c0: 6e63 6c75 6465 3d22 222c 2065 7863 6c75  nclude="", exclu
+000174d0: 6465 3d22 2229 0a0a 2020 2020 6465 6620  de="")..    def 
+000174e0: 7465 7374 5f65 7874 656e 645f 6578 636c  test_extend_excl
+000174f0: 7564 6528 7365 6c66 2920 2d3e 204e 6f6e  ude(self) -> Non
+00017500: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
+00017510: 3d20 4441 5441 5f44 4952 202f 2022 696e  = DATA_DIR / "in
+00017520: 636c 7564 655f 6578 636c 7564 655f 7465  clude_exclude_te
+00017530: 7374 7322 0a20 2020 2020 2020 2073 7263  sts".        src
+00017540: 203d 205b 7061 7468 5d0a 2020 2020 2020   = [path].      
+00017550: 2020 6578 7065 6374 6564 203d 205b 0a20    expected = [. 
+00017560: 2020 2020 2020 2020 2020 2050 6174 6828             Path(
+00017570: 7061 7468 202f 2022 622f 6578 636c 7564  path / "b/exclud
+00017580: 652f 612e 7079 2229 2c0a 2020 2020 2020  e/a.py"),.      
+00017590: 2020 2020 2020 5061 7468 2870 6174 6820        Path(path 
+000175a0: 2f20 2262 2f64 6f6e 745f 6578 636c 7564  / "b/dont_exclud
+000175b0: 652f 612e 7079 2229 2c0a 2020 2020 2020  e/a.py"),.      
+000175c0: 2020 5d0a 2020 2020 2020 2020 6173 7365    ].        asse
+000175d0: 7274 5f63 6f6c 6c65 6374 6564 5f73 6f75  rt_collected_sou
+000175e0: 7263 6573 280a 2020 2020 2020 2020 2020  rces(.          
+000175f0: 2020 7372 632c 2065 7870 6563 7465 642c    src, expected,
+00017600: 2065 7863 6c75 6465 3d72 225c 2e70 7969   exclude=r"\.pyi
+00017610: 2422 2c20 6578 7465 6e64 5f65 7863 6c75  $", extend_exclu
+00017620: 6465 3d72 225c 2e64 6566 696e 6974 656c  de=r"\.definitel
+00017630: 795f 6578 636c 7564 6522 0a20 2020 2020  y_exclude".     
+00017640: 2020 2029 0a0a 2020 2020 4070 7974 6573     )..    @pytes
+00017650: 742e 6d61 726b 2e69 6e63 6f6d 7061 7469  t.mark.incompati
+00017660: 626c 655f 7769 7468 5f6d 7970 7963 0a20  ble_with_mypyc. 
+00017670: 2020 2064 6566 2074 6573 745f 7379 6d6c     def test_syml
+00017680: 696e 6b5f 6f75 745f 6f66 5f72 6f6f 745f  ink_out_of_root_
+00017690: 6469 7265 6374 6f72 7928 7365 6c66 2920  directory(self) 
+000176a0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000176b0: 2070 6174 6820 3d20 4d61 6769 634d 6f63   path = MagicMoc
+000176c0: 6b28 290a 2020 2020 2020 2020 726f 6f74  k().        root
+000176d0: 203d 2054 4849 535f 4449 522e 7265 736f   = THIS_DIR.reso
+000176e0: 6c76 6528 290a 2020 2020 2020 2020 6368  lve().        ch
+000176f0: 696c 6420 3d20 4d61 6769 634d 6f63 6b28  ild = MagicMock(
+00017700: 290a 2020 2020 2020 2020 696e 636c 7564  ).        includ
+00017710: 6520 3d20 7265 2e63 6f6d 7069 6c65 2870  e = re.compile(p
+00017720: 7969 6e6b 2e44 4546 4155 4c54 5f49 4e43  yink.DEFAULT_INC
+00017730: 4c55 4445 5329 0a20 2020 2020 2020 2065  LUDES).        e
+00017740: 7863 6c75 6465 203d 2072 652e 636f 6d70  xclude = re.comp
+00017750: 696c 6528 7079 696e 6b2e 4445 4641 554c  ile(pyink.DEFAUL
+00017760: 545f 4558 434c 5544 4553 290a 2020 2020  T_EXCLUDES).    
+00017770: 2020 2020 7265 706f 7274 203d 2070 7969      report = pyi
+00017780: 6e6b 2e52 6570 6f72 7428 290a 2020 2020  nk.Report().    
+00017790: 2020 2020 6769 7469 676e 6f72 6520 3d20      gitignore = 
+000177a0: 5061 7468 5370 6563 2e66 726f 6d5f 6c69  PathSpec.from_li
+000177b0: 6e65 7328 2267 6974 7769 6c64 6d61 7463  nes("gitwildmatc
+000177c0: 6822 2c20 5b5d 290a 2020 2020 2020 2020  h", []).        
+000177d0: 2320 6063 6869 6c64 6020 7368 6f75 6c64  # `child` should
+000177e0: 2062 6568 6176 6520 6c69 6b65 2061 2073   behave like a s
+000177f0: 796d 6c69 6e6b 2077 6869 6368 2072 6573  ymlink which res
+00017800: 6f6c 7665 6420 7061 7468 2069 7320 636c  olved path is cl
+00017810: 6561 726c 790a 2020 2020 2020 2020 2320  early.        # 
+00017820: 6f75 7473 6964 6520 6f66 2074 6865 2060  outside of the `
+00017830: 726f 6f74 6020 6469 7265 6374 6f72 792e  root` directory.
+00017840: 0a20 2020 2020 2020 2070 6174 682e 6974  .        path.it
+00017850: 6572 6469 722e 7265 7475 726e 5f76 616c  erdir.return_val
+00017860: 7565 203d 205b 6368 696c 645d 0a20 2020  ue = [child].   
+00017870: 2020 2020 2063 6869 6c64 2e72 6573 6f6c       child.resol
+00017880: 7665 2e72 6574 7572 6e5f 7661 6c75 6520  ve.return_value 
+00017890: 3d20 5061 7468 2822 2f61 2f62 2f63 2229  = Path("/a/b/c")
+000178a0: 0a20 2020 2020 2020 2063 6869 6c64 2e61  .        child.a
+000178b0: 735f 706f 7369 782e 7265 7475 726e 5f76  s_posix.return_v
+000178c0: 616c 7565 203d 2022 2f61 2f62 2f63 220a  alue = "/a/b/c".
+000178d0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000178e0: 2020 2020 2020 2020 206c 6973 7428 0a20           list(. 
+000178f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017900: 7969 6e6b 2e67 656e 5f70 7974 686f 6e5f  yink.gen_python_
+00017910: 6669 6c65 7328 0a20 2020 2020 2020 2020  files(.         
+00017920: 2020 2020 2020 2020 2020 2070 6174 682e             path.
+00017930: 6974 6572 6469 7228 292c 0a20 2020 2020  iterdir(),.     
+00017940: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00017950: 6f6f 742c 0a20 2020 2020 2020 2020 2020  oot,.           
+00017960: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+00017970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017980: 2020 2020 2020 6578 636c 7564 652c 0a20        exclude,. 
+00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179a0: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
+000179b0: 2020 2020 2020 2020 2020 2020 204e 6f6e               Non
+000179c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000179d0: 2020 2020 2020 2072 6570 6f72 742c 0a20         report,. 
+000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179f0: 2020 207b 7061 7468 3a20 6769 7469 676e     {path: gitign
+00017a00: 6f72 657d 2c0a 2020 2020 2020 2020 2020  ore},.          
+00017a10: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+00017a20: 653d 4661 6c73 652c 0a20 2020 2020 2020  e=False,.       
+00017a30: 2020 2020 2020 2020 2020 2020 2071 7569               qui
+00017a40: 6574 3d46 616c 7365 2c0a 2020 2020 2020  et=False,.      
+00017a50: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00017a60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00017a70: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00017a80: 726f 7220 6173 2076 653a 0a20 2020 2020  ror as ve:.     
+00017a90: 2020 2020 2020 2070 7974 6573 742e 6661         pytest.fa
+00017aa0: 696c 2866 2260 6765 745f 7079 7468 6f6e  il(f"`get_python
+00017ab0: 5f66 696c 6573 5f69 6e5f 6469 7228 2960  _files_in_dir()`
+00017ac0: 2066 6169 6c65 643a 207b 7665 7d22 290a   failed: {ve}").
+00017ad0: 2020 2020 2020 2020 7061 7468 2e69 7465          path.ite
+00017ae0: 7264 6972 2e61 7373 6572 745f 6361 6c6c  rdir.assert_call
+00017af0: 6564 5f6f 6e63 6528 290a 2020 2020 2020  ed_once().      
+00017b00: 2020 6368 696c 642e 7265 736f 6c76 652e    child.resolve.
+00017b10: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
+00017b20: 6365 2829 0a0a 2020 2020 4070 6174 6368  ce()..    @patch
+00017b30: 2822 7079 696e 6b2e 6669 6e64 5f70 726f  ("pyink.find_pro
+00017b40: 6a65 6374 5f72 6f6f 7422 2c20 6c61 6d62  ject_root", lamb
+00017b50: 6461 202a 6172 6773 3a20 2854 4849 535f  da *args: (THIS_
+00017b60: 4449 522e 7265 736f 6c76 6528 292c 204e  DIR.resolve(), N
+00017b70: 6f6e 6529 290a 2020 2020 6465 6620 7465  one)).    def te
+00017b80: 7374 5f67 6574 5f73 6f75 7263 6573 5f77  st_get_sources_w
+00017b90: 6974 685f 7374 6469 6e28 7365 6c66 2920  ith_stdin(self) 
+00017ba0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00017bb0: 2073 7263 203d 205b 222d 225d 0a20 2020   src = ["-"].   
+00017bc0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+00017bd0: 5b22 2d22 5d0a 2020 2020 2020 2020 6173  ["-"].        as
+00017be0: 7365 7274 5f63 6f6c 6c65 6374 6564 5f73  sert_collected_s
+00017bf0: 6f75 7263 6573 2873 7263 2c20 6578 7065  ources(src, expe
+00017c00: 6374 6564 2c20 696e 636c 7564 653d 2222  cted, include=""
+00017c10: 2c20 6578 636c 7564 653d 7222 2f65 7863  , exclude=r"/exc
+00017c20: 6c75 6465 2f7c 615c 2e70 7922 290a 0a20  lude/|a\.py").. 
+00017c30: 2020 2040 7061 7463 6828 2270 7969 6e6b     @patch("pyink
+00017c40: 2e66 696e 645f 7072 6f6a 6563 745f 726f  .find_project_ro
+00017c50: 6f74 222c 206c 616d 6264 6120 2a61 7267  ot", lambda *arg
+00017c60: 733a 2028 5448 4953 5f44 4952 2e72 6573  s: (THIS_DIR.res
+00017c70: 6f6c 7665 2829 2c20 4e6f 6e65 2929 0a20  olve(), None)). 
+00017c80: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
+00017c90: 736f 7572 6365 735f 7769 7468 5f73 7464  sources_with_std
+00017ca0: 696e 5f66 696c 656e 616d 6528 7365 6c66  in_filename(self
+00017cb0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00017cc0: 2020 2073 7263 203d 205b 222d 225d 0a20     src = ["-"]. 
+00017cd0: 2020 2020 2020 2073 7464 696e 5f66 696c         stdin_fil
+00017ce0: 656e 616d 6520 3d20 7374 7228 5448 4953  ename = str(THIS
+00017cf0: 5f44 4952 202f 2022 6461 7461 2f63 6f6c  _DIR / "data/col
+00017d00: 6c65 6374 696f 6e73 2e70 7922 290a 2020  lections.py").  
+00017d10: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
+00017d20: 205b 6622 5f5f 5059 494e 4b5f 5354 4449   [f"__PYINK_STDI
+00017d30: 4e5f 4649 4c45 4e41 4d45 5f5f 7b73 7464  N_FILENAME__{std
+00017d40: 696e 5f66 696c 656e 616d 657d 225d 0a20  in_filename}"]. 
+00017d50: 2020 2020 2020 2061 7373 6572 745f 636f         assert_co
+00017d60: 6c6c 6563 7465 645f 736f 7572 6365 7328  llected_sources(
+00017d70: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+00017d80: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00017d90: 7065 6374 6564 2c0a 2020 2020 2020 2020  pected,.        
+00017da0: 2020 2020 6578 636c 7564 653d 7222 2f65      exclude=r"/e
+00017db0: 7863 6c75 6465 2f61 5c2e 7079 222c 0a20  xclude/a\.py",. 
+00017dc0: 2020 2020 2020 2020 2020 2073 7464 696e             stdin
+00017dd0: 5f66 696c 656e 616d 653d 7374 6469 6e5f  _filename=stdin_
+00017de0: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+00017df0: 2020 290a 0a20 2020 2040 7061 7463 6828    )..    @patch(
+00017e00: 2270 7969 6e6b 2e66 696e 645f 7072 6f6a  "pyink.find_proj
+00017e10: 6563 745f 726f 6f74 222c 206c 616d 6264  ect_root", lambd
+00017e20: 6120 2a61 7267 733a 2028 5448 4953 5f44  a *args: (THIS_D
+00017e30: 4952 2e72 6573 6f6c 7665 2829 2c20 4e6f  IR.resolve(), No
+00017e40: 6e65 2929 0a20 2020 2064 6566 2074 6573  ne)).    def tes
+00017e50: 745f 6765 745f 736f 7572 6365 735f 7769  t_get_sources_wi
+00017e60: 7468 5f73 7464 696e 5f66 696c 656e 616d  th_stdin_filenam
+00017e70: 655f 616e 645f 6578 636c 7564 6528 7365  e_and_exclude(se
+00017e80: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00017e90: 2020 2020 2023 2045 7863 6c75 6465 2073       # Exclude s
+00017ea0: 686f 756c 646e 2774 2065 7863 6c75 6465  houldn't exclude
+00017eb0: 2073 7464 696e 5f66 696c 656e 616d 6520   stdin_filename 
+00017ec0: 7369 6e63 6520 6974 2069 7320 6d69 6d69  since it is mimi
+00017ed0: 636b 696e 6720 7468 650a 2020 2020 2020  cking the.      
+00017ee0: 2020 2320 6669 6c65 2062 6569 6e67 2070    # file being p
+00017ef0: 6173 7365 6420 6469 7265 6374 6c79 2e20  assed directly. 
+00017f00: 5468 6973 2069 7320 7468 6520 7361 6d65  This is the same
+00017f10: 2061 730a 2020 2020 2020 2020 2320 7465   as.        # te
+00017f20: 7374 5f65 7863 6c75 6465 5f66 6f72 5f69  st_exclude_for_i
+00017f30: 7373 7565 5f31 3537 320a 2020 2020 2020  ssue_1572.      
+00017f40: 2020 7061 7468 203d 2044 4154 415f 4449    path = DATA_DI
+00017f50: 5220 2f20 2269 6e63 6c75 6465 5f65 7863  R / "include_exc
+00017f60: 6c75 6465 5f74 6573 7473 220a 2020 2020  lude_tests".    
+00017f70: 2020 2020 7372 6320 3d20 5b22 2d22 5d0a      src = ["-"].
+00017f80: 2020 2020 2020 2020 7374 6469 6e5f 6669          stdin_fi
+00017f90: 6c65 6e61 6d65 203d 2073 7472 2870 6174  lename = str(pat
+00017fa0: 6820 2f20 2262 2f65 7863 6c75 6465 2f61  h / "b/exclude/a
+00017fb0: 2e70 7922 290a 2020 2020 2020 2020 6578  .py").        ex
+00017fc0: 7065 6374 6564 203d 205b 6622 5f5f 5059  pected = [f"__PY
+00017fd0: 494e 4b5f 5354 4449 4e5f 4649 4c45 4e41  INK_STDIN_FILENA
+00017fe0: 4d45 5f5f 7b73 7464 696e 5f66 696c 656e  ME__{stdin_filen
+00017ff0: 616d 657d 225d 0a20 2020 2020 2020 2061  ame}"].        a
+00018000: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
+00018010: 736f 7572 6365 7328 0a20 2020 2020 2020  sources(.       
+00018020: 2020 2020 2073 7263 2c0a 2020 2020 2020       src,.      
+00018030: 2020 2020 2020 6578 7065 6374 6564 2c0a        expected,.
+00018040: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+00018050: 7564 653d 7222 2f65 7863 6c75 6465 2f7c  ude=r"/exclude/|
+00018060: 615c 2e70 7922 2c0a 2020 2020 2020 2020  a\.py",.        
+00018070: 2020 2020 7374 6469 6e5f 6669 6c65 6e61      stdin_filena
+00018080: 6d65 3d73 7464 696e 5f66 696c 656e 616d  me=stdin_filenam
+00018090: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+000180a0: 2020 4070 6174 6368 2822 7079 696e 6b2e    @patch("pyink.
+000180b0: 6669 6e64 5f70 726f 6a65 6374 5f72 6f6f  find_project_roo
+000180c0: 7422 2c20 6c61 6d62 6461 202a 6172 6773  t", lambda *args
+000180d0: 3a20 2854 4849 535f 4449 522e 7265 736f  : (THIS_DIR.reso
+000180e0: 6c76 6528 292c 204e 6f6e 6529 290a 2020  lve(), None)).  
+000180f0: 2020 6465 6620 7465 7374 5f67 6574 5f73    def test_get_s
+00018100: 6f75 7263 6573 5f77 6974 685f 7374 6469  ources_with_stdi
+00018110: 6e5f 6669 6c65 6e61 6d65 5f61 6e64 5f65  n_filename_and_e
+00018120: 7874 656e 645f 6578 636c 7564 6528 7365  xtend_exclude(se
+00018130: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00018140: 2020 2020 2023 2045 7874 656e 6420 6578       # Extend ex
+00018150: 636c 7564 6520 7368 6f75 6c64 6e27 7420  clude shouldn't 
+00018160: 6578 636c 7564 6520 7374 6469 6e5f 6669  exclude stdin_fi
+00018170: 6c65 6e61 6d65 2073 696e 6365 2069 7420  lename since it 
+00018180: 6973 206d 696d 6963 6b69 6e67 2074 6865  is mimicking the
+00018190: 0a20 2020 2020 2020 2023 2066 696c 6520  .        # file 
+000181a0: 6265 696e 6720 7061 7373 6564 2064 6972  being passed dir
+000181b0: 6563 746c 792e 2054 6869 7320 6973 2074  ectly. This is t
+000181c0: 6865 2073 616d 6520 6173 0a20 2020 2020  he same as.     
+000181d0: 2020 2023 2074 6573 745f 6578 636c 7564     # test_exclud
+000181e0: 655f 666f 725f 6973 7375 655f 3135 3732  e_for_issue_1572
+000181f0: 0a20 2020 2020 2020 2073 7263 203d 205b  .        src = [
+00018200: 222d 225d 0a20 2020 2020 2020 2070 6174  "-"].        pat
+00018210: 6820 3d20 5448 4953 5f44 4952 202f 2022  h = THIS_DIR / "
+00018220: 6461 7461 2220 2f20 2269 6e63 6c75 6465  data" / "include
+00018230: 5f65 7863 6c75 6465 5f74 6573 7473 220a  _exclude_tests".
+00018240: 2020 2020 2020 2020 7374 6469 6e5f 6669          stdin_fi
+00018250: 6c65 6e61 6d65 203d 2073 7472 2870 6174  lename = str(pat
+00018260: 6820 2f20 2262 2f65 7863 6c75 6465 2f61  h / "b/exclude/a
+00018270: 2e70 7922 290a 2020 2020 2020 2020 6578  .py").        ex
+00018280: 7065 6374 6564 203d 205b 6622 5f5f 5059  pected = [f"__PY
+00018290: 494e 4b5f 5354 4449 4e5f 4649 4c45 4e41  INK_STDIN_FILENA
+000182a0: 4d45 5f5f 7b73 7464 696e 5f66 696c 656e  ME__{stdin_filen
+000182b0: 616d 657d 225d 0a20 2020 2020 2020 2061  ame}"].        a
+000182c0: 7373 6572 745f 636f 6c6c 6563 7465 645f  ssert_collected_
+000182d0: 736f 7572 6365 7328 0a20 2020 2020 2020  sources(.       
+000182e0: 2020 2020 2073 7263 2c0a 2020 2020 2020       src,.      
+000182f0: 2020 2020 2020 6578 7065 6374 6564 2c0a        expected,.
+00018300: 2020 2020 2020 2020 2020 2020 6578 7465              exte
+00018310: 6e64 5f65 7863 6c75 6465 3d72 222f 6578  nd_exclude=r"/ex
+00018320: 636c 7564 652f 7c61 5c2e 7079 222c 0a20  clude/|a\.py",. 
+00018330: 2020 2020 2020 2020 2020 2073 7464 696e             stdin
+00018340: 5f66 696c 656e 616d 653d 7374 6469 6e5f  _filename=stdin_
+00018350: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+00018360: 2020 290a 0a20 2020 2040 7061 7463 6828    )..    @patch(
+00018370: 2270 7969 6e6b 2e66 696e 645f 7072 6f6a  "pyink.find_proj
+00018380: 6563 745f 726f 6f74 222c 206c 616d 6264  ect_root", lambd
+00018390: 6120 2a61 7267 733a 2028 5448 4953 5f44  a *args: (THIS_D
+000183a0: 4952 2e72 6573 6f6c 7665 2829 2c20 4e6f  IR.resolve(), No
+000183b0: 6e65 2929 0a20 2020 2064 6566 2074 6573  ne)).    def tes
+000183c0: 745f 6765 745f 736f 7572 6365 735f 7769  t_get_sources_wi
+000183d0: 7468 5f73 7464 696e 5f66 696c 656e 616d  th_stdin_filenam
+000183e0: 655f 616e 645f 666f 7263 655f 6578 636c  e_and_force_excl
+000183f0: 7564 6528 7365 6c66 2920 2d3e 204e 6f6e  ude(self) -> Non
+00018400: 653a 0a20 2020 2020 2020 2023 2046 6f72  e:.        # For
+00018410: 6365 2065 7863 6c75 6465 2073 686f 756c  ce exclude shoul
+00018420: 6420 6578 636c 7564 6520 7468 6520 6669  d exclude the fi
+00018430: 6c65 2077 6865 6e20 7061 7373 696e 6720  le when passing 
+00018440: 6974 2074 6872 6f75 6768 0a20 2020 2020  it through.     
+00018450: 2020 2023 2073 7464 696e 5f66 696c 656e     # stdin_filen
+00018460: 616d 650a 2020 2020 2020 2020 7061 7468  ame.        path
+00018470: 203d 2054 4849 535f 4449 5220 2f20 2264   = THIS_DIR / "d
+00018480: 6174 6122 202f 2022 696e 636c 7564 655f  ata" / "include_
+00018490: 6578 636c 7564 655f 7465 7374 7322 0a20  exclude_tests". 
+000184a0: 2020 2020 2020 2073 7464 696e 5f66 696c         stdin_fil
+000184b0: 656e 616d 6520 3d20 7374 7228 7061 7468  ename = str(path
+000184c0: 202f 2022 622f 6578 636c 7564 652f 612e   / "b/exclude/a.
+000184d0: 7079 2229 0a20 2020 2020 2020 2061 7373  py").        ass
+000184e0: 6572 745f 636f 6c6c 6563 7465 645f 736f  ert_collected_so
+000184f0: 7572 6365 7328 0a20 2020 2020 2020 2020  urces(.         
+00018500: 2020 2073 7263 3d5b 222d 225d 2c0a 2020     src=["-"],.  
+00018510: 2020 2020 2020 2020 2020 6578 7065 6374            expect
+00018520: 6564 3d5b 5d2c 0a20 2020 2020 2020 2020  ed=[],.         
+00018530: 2020 2066 6f72 6365 5f65 7863 6c75 6465     force_exclude
+00018540: 3d72 222f 6578 636c 7564 652f 7c61 5c2e  =r"/exclude/|a\.
+00018550: 7079 222c 0a20 2020 2020 2020 2020 2020  py",.           
+00018560: 2073 7464 696e 5f66 696c 656e 616d 653d   stdin_filename=
+00018570: 7374 6469 6e5f 6669 6c65 6e61 6d65 2c0a  stdin_filename,.
+00018580: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00018590: 6566 2064 6563 6f64 655f 616e 645f 6e6f  ef decode_and_no
+000185a0: 726d 616c 697a 6564 2873 656c 662c 2073  rmalized(self, s
+000185b0: 7464 6f75 743a 2062 7974 6573 2920 2d3e  tdout: bytes) ->
+000185c0: 2073 7472 3a0a 2020 2020 2020 2020 2320   str:.        # 
+000185d0: 4d61 6b65 2069 7420 6561 7369 6572 2074  Make it easier t
+000185e0: 6f20 7465 7374 206f 6e20 5769 6e64 6f77  o test on Window
+000185f0: 732e 2054 6865 2074 6573 7420 646f 6573  s. The test does
+00018600: 6e27 7420 6361 7265 2061 626f 7574 0a20  n't care about. 
+00018610: 2020 2020 2020 2023 206e 6577 6c69 6e65         # newline
+00018620: 732e 0a20 2020 2020 2020 2072 6574 7572  s..        retur
+00018630: 6e20 7374 646f 7574 2e64 6563 6f64 6528  n stdout.decode(
+00018640: 292e 7265 706c 6163 6528 225c 725c 6e22  ).replace("\r\n"
+00018650: 2c20 225c 6e22 290a 0a20 2020 2064 6566  , "\n")..    def
+00018660: 2074 6573 745f 7079 696e 6b5f 6465 6661   test_pyink_defa
+00018670: 756c 7428 7365 6c66 2920 2d3e 204e 6f6e  ult(self) -> Non
+00018680: 653a 0a20 2020 2020 2020 2070 6174 6820  e:.        path 
+00018690: 3d20 5448 4953 5f44 4952 202f 2022 6461  = THIS_DIR / "da
+000186a0: 7461 2220 2f20 2270 7969 6e6b 5f63 6f6e  ta" / "pyink_con
+000186b0: 6669 6773 220a 2020 2020 2020 2020 6578  figs".        ex
+000186c0: 616d 706c 6520 3d20 7374 7228 7061 7468  ample = str(path
+000186d0: 202f 2022 6578 616d 706c 652e 7079 2229   / "example.py")
+000186e0: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
+000186f0: 3d20 7374 7228 5448 4953 5f44 4952 202f  = str(THIS_DIR /
+00018700: 2022 656d 7074 792e 746f 6d6c 2229 0a20   "empty.toml"). 
+00018710: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00018720: 426c 6163 6b52 756e 6e65 7228 292e 696e  BlackRunner().in
+00018730: 766f 6b65 280a 2020 2020 2020 2020 2020  voke(.          
+00018740: 2020 7079 696e 6b2e 6d61 696e 2c20 5b22    pyink.main, ["
+00018750: 2d2d 6469 6666 222c 2022 2d2d 636f 6e66  --diff", "--conf
+00018760: 6967 222c 2063 6f6e 6669 672c 2065 7861  ig", config, exa
+00018770: 6d70 6c65 5d0a 2020 2020 2020 2020 290a  mple].        ).
+00018780: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
+00018790: 6573 756c 742e 6578 6974 5f63 6f64 6520  esult.exit_code 
+000187a0: 3d3d 2030 0a20 2020 2020 2020 2061 7373  == 0.        ass
+000187b0: 6572 7420 7265 7375 6c74 2e73 7464 6f75  ert result.stdou
+000187c0: 745f 6279 7465 7320 6973 206e 6f74 204e  t_bytes is not N
+000187d0: 6f6e 650a 0a20 2020 2020 2020 2061 7373  one..        ass
+000187e0: 6572 7420 222d 2070 6173 735c 6e2b 2020  ert "- pass\n+  
+000187f0: 2020 7061 7373 5c6e 2220 696e 2073 656c    pass\n" in sel
+00018800: 662e 6465 636f 6465 5f61 6e64 5f6e 6f72  f.decode_and_nor
+00018810: 6d61 6c69 7a65 6428 7265 7375 6c74 2e73  malized(result.s
+00018820: 7464 6f75 745f 6279 7465 7329 0a0a 2020  tdout_bytes)..  
+00018830: 2020 6465 6620 7465 7374 5f70 7969 6e6b    def test_pyink
+00018840: 5f6f 7665 7272 6964 6573 2873 656c 6629  _overrides(self)
+00018850: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00018860: 2020 7061 7468 203d 2054 4849 535f 4449    path = THIS_DI
+00018870: 5220 2f20 2264 6174 6122 202f 2022 7079  R / "data" / "py
+00018880: 696e 6b5f 636f 6e66 6967 7322 0a20 2020  ink_configs".   
+00018890: 2020 2020 2065 7861 6d70 6c65 203d 2073       example = s
+000188a0: 7472 2870 6174 6820 2f20 2265 7861 6d70  tr(path / "examp
+000188b0: 6c65 2e70 7922 290a 2020 2020 2020 2020  le.py").        
+000188c0: 636f 6e66 6967 203d 2073 7472 2870 6174  config = str(pat
+000188d0: 6820 2f20 226f 7665 7272 6964 6573 2e74  h / "overrides.t
+000188e0: 6f6d 6c22 290a 2020 2020 2020 2020 7265  oml").        re
+000188f0: 7375 6c74 203d 2042 6c61 636b 5275 6e6e  sult = BlackRunn
+00018900: 6572 2829 2e69 6e76 6f6b 6528 0a20 2020  er().invoke(.   
+00018910: 2020 2020 2020 2020 2070 7969 6e6b 2e6d           pyink.m
+00018920: 6169 6e2c 205b 222d 2d64 6966 6622 2c20  ain, ["--diff", 
+00018930: 222d 2d63 6f6e 6669 6722 2c20 636f 6e66  "--config", conf
+00018940: 6967 2c20 6578 616d 706c 655d 0a20 2020  ig, example].   
+00018950: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+00018960: 7373 6572 7420 7265 7375 6c74 2e65 7869  ssert result.exi
+00018970: 745f 636f 6465 203d 3d20 300a 2020 2020  t_code == 0.    
+00018980: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
+00018990: 742e 7374 646f 7574 5f62 7974 6573 2069  t.stdout_bytes i
+000189a0: 7320 6e6f 7420 4e6f 6e65 0a0a 2020 2020  s not None..    
+000189b0: 2020 2020 6173 7365 7274 2022 2d20 7061      assert "- pa
+000189c0: 7373 5c6e 2b20 2070 6173 735c 6e22 2069  ss\n+  pass\n" i
+000189d0: 6e20 7365 6c66 2e64 6563 6f64 655f 616e  n self.decode_an
+000189e0: 645f 6e6f 726d 616c 697a 6564 2872 6573  d_normalized(res
+000189f0: 756c 742e 7374 646f 7574 5f62 7974 6573  ult.stdout_bytes
+00018a00: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00018a10: 7079 696e 6b5f 6469 7361 626c 6528 7365  pyink_disable(se
+00018a20: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00018a30: 2020 2020 2070 6174 6820 3d20 5448 4953       path = THIS
+00018a40: 5f44 4952 202f 2022 6461 7461 2220 2f20  _DIR / "data" / 
+00018a50: 2270 7969 6e6b 5f63 6f6e 6669 6773 220a  "pyink_configs".
+00018a60: 2020 2020 2020 2020 6578 616d 706c 6520          example 
+00018a70: 3d20 7374 7228 7061 7468 202f 2022 6578  = str(path / "ex
+00018a80: 616d 706c 652e 7079 2229 0a20 2020 2020  ample.py").     
+00018a90: 2020 2063 6f6e 6669 6720 3d20 7374 7228     config = str(
+00018aa0: 7061 7468 202f 2022 6469 7361 626c 652e  path / "disable.
+00018ab0: 746f 6d6c 2229 0a20 2020 2020 2020 2072  toml").        r
+00018ac0: 6573 756c 7420 3d20 426c 6163 6b52 756e  esult = BlackRun
+00018ad0: 6e65 7228 292e 696e 766f 6b65 280a 2020  ner().invoke(.  
+00018ae0: 2020 2020 2020 2020 2020 7079 696e 6b2e            pyink.
+00018af0: 6d61 696e 2c20 5b22 2d2d 6469 6666 222c  main, ["--diff",
+00018b00: 2022 2d2d 636f 6e66 6967 222c 2063 6f6e   "--config", con
+00018b10: 6669 672c 2065 7861 6d70 6c65 5d0a 2020  fig, example].  
+00018b20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00018b30: 6173 7365 7274 2072 6573 756c 742e 6578  assert result.ex
+00018b40: 6974 5f63 6f64 6520 3d3d 2030 0a20 2020  it_code == 0.   
+00018b50: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+00018b60: 6c74 2e73 7464 6f75 745f 6279 7465 7320  lt.stdout_bytes 
+00018b70: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
+00018b80: 2020 2020 2073 7464 6f75 7420 3d20 7365       stdout = se
+00018b90: 6c66 2e64 6563 6f64 655f 616e 645f 6e6f  lf.decode_and_no
+00018ba0: 726d 616c 697a 6564 2872 6573 756c 742e  rmalized(result.
+00018bb0: 7374 646f 7574 5f62 7974 6573 290a 2020  stdout_bytes).  
+00018bc0: 2020 2020 2020 6173 7365 7274 2028 0a20        assert (. 
+00018bd0: 2020 2020 2020 2020 2020 2022 2222 5c0a             """\.
+00018be0: 2d66 726f 6d20 7665 7279 2e6c 6f6e 672e  -from very.long.
+00018bf0: 7061 636b 6167 652e 7061 7468 2e6d 795f  package.path.my_
+00018c00: 6f72 672e 6d79 5f76 6572 795f 6c6f 6e67  org.my_very_long
+00018c10: 5f70 726f 6a65 6374 5f6e 616d 652e 6177  _project_name.aw
+00018c20: 6573 6f6d 655f 6261 636b 656e 642e 636f  esome_backend.co
+00018c30: 7265 5f66 7261 6d65 776f 726b 2e75 7469  re_framework.uti
+00018c40: 6c20 696d 706f 7274 206d 795f 6c6f 6e67  l import my_long
+00018c50: 5f6d 6f64 756c 655f 6e61 6d65 0a2b 6672  _module_name.+fr
+00018c60: 6f6d 2076 6572 792e 6c6f 6e67 2e70 6163  om very.long.pac
+00018c70: 6b61 6765 2e70 6174 682e 6d79 5f6f 7267  kage.path.my_org
+00018c80: 2e6d 795f 7665 7279 5f6c 6f6e 675f 7072  .my_very_long_pr
+00018c90: 6f6a 6563 745f 6e61 6d65 2e61 7765 736f  oject_name.aweso
+00018ca0: 6d65 5f62 6163 6b65 6e64 2e63 6f72 655f  me_backend.core_
+00018cb0: 6672 616d 6577 6f72 6b2e 7574 696c 2069  framework.util i
+00018cc0: 6d70 6f72 7420 280a 2b20 2020 206d 795f  mport (.+    my_
+00018cd0: 6c6f 6e67 5f6d 6f64 756c 655f 6e61 6d65  long_module_name
+00018ce0: 2c0a 2b29 0a22 2222 0a20 2020 2020 2020  ,.+).""".       
+00018cf0: 2020 2020 2069 6e20 7374 646f 7574 0a20       in stdout. 
+00018d00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018d10: 2061 7373 6572 7420 222d 2070 6173 735c   assert "- pass\
+00018d20: 6e2b 2020 2020 7061 7373 5c6e 2220 696e  n+    pass\n" in
+00018d30: 2073 7464 6f75 740a 0a20 2020 2064 6566   stdout..    def
+00018d40: 2074 6573 745f 7079 696e 6b5f 696e 5f74   test_pyink_in_t
+00018d50: 6f6f 6c5f 626c 6163 6b28 7365 6c66 2920  ool_black(self) 
+00018d60: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00018d70: 2070 6174 6820 3d20 5448 4953 5f44 4952   path = THIS_DIR
+00018d80: 202f 2022 6461 7461 2220 2f20 2270 7969   / "data" / "pyi
+00018d90: 6e6b 5f63 6f6e 6669 6773 220a 2020 2020  nk_configs".    
+00018da0: 2020 2020 6578 616d 706c 6520 3d20 7374      example = st
+00018db0: 7228 7061 7468 202f 2022 6578 616d 706c  r(path / "exampl
+00018dc0: 652e 7079 2229 0a20 2020 2020 2020 2063  e.py").        c
+00018dd0: 6f6e 6669 6720 3d20 7374 7228 7061 7468  onfig = str(path
+00018de0: 202f 2022 746f 6f6c 5f62 6c61 636b 2e74   / "tool_black.t
+00018df0: 6f6d 6c22 290a 2020 2020 2020 2020 7265  oml").        re
+00018e00: 7375 6c74 203d 2042 6c61 636b 5275 6e6e  sult = BlackRunn
+00018e10: 6572 2829 2e69 6e76 6f6b 6528 0a20 2020  er().invoke(.   
+00018e20: 2020 2020 2020 2020 2070 7969 6e6b 2e6d           pyink.m
+00018e30: 6169 6e2c 205b 222d 2d64 6966 6622 2c20  ain, ["--diff", 
+00018e40: 222d 2d63 6f6e 6669 6722 2c20 636f 6e66  "--config", conf
+00018e50: 6967 2c20 6578 616d 706c 655d 0a20 2020  ig, example].   
+00018e60: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+00018e70: 7373 6572 7420 7265 7375 6c74 2e65 7869  ssert result.exi
+00018e80: 745f 636f 6465 203d 3d20 300a 2020 2020  t_code == 0.    
+00018e90: 2020 2020 6173 7365 7274 2072 6573 756c      assert resul
+00018ea0: 742e 7374 646f 7574 5f62 7974 6573 2069  t.stdout_bytes i
+00018eb0: 7320 6e6f 7420 4e6f 6e65 0a0a 2020 2020  s not None..    
+00018ec0: 2020 2020 6173 7365 7274 2022 2d20 7061      assert "- pa
+00018ed0: 7373 5c6e 2b20 2020 2070 6173 735c 6e22  ss\n+    pass\n"
+00018ee0: 2069 6e20 7365 6c66 2e64 6563 6f64 655f   in self.decode_
+00018ef0: 616e 645f 6e6f 726d 616c 697a 6564 2872  and_normalized(r
+00018f00: 6573 756c 742e 7374 646f 7574 5f62 7974  esult.stdout_byt
+00018f10: 6573 290a 0a20 2020 2040 7079 7465 7374  es)..    @pytest
+00018f20: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00018f30: 6528 2276 616c 7565 7322 2c20 5b28 2237  e("values", [("7
+00018f40: 2d37 222c 292c 2028 2231 2d31 222c 2022  -7",), ("1-1", "
+00018f50: 372d 3722 295d 290a 2020 2020 6465 6620  7-7")]).    def 
+00018f60: 7465 7374 5f70 7969 6e6b 5f6c 696e 6573  test_pyink_lines
+00018f70: 2873 656c 662c 2076 616c 7565 7329 202d  (self, values) -
+00018f80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00018f90: 7061 7468 203d 2054 4849 535f 4449 5220  path = THIS_DIR 
+00018fa0: 2f20 2264 6174 6122 202f 2022 7079 696e  / "data" / "pyin
+00018fb0: 6b5f 636f 6e66 6967 7322 0a20 2020 2020  k_configs".     
+00018fc0: 2020 2065 7861 6d70 6c65 203d 2073 7472     example = str
+00018fd0: 2870 6174 6820 2f20 2265 7861 6d70 6c65  (path / "example
+00018fe0: 2e70 7922 290a 2020 2020 2020 2020 7079  .py").        py
+00018ff0: 696e 6b5f 6c69 6e65 735f 6172 6773 203d  ink_lines_args =
+00019000: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+00019010: 7661 6c75 6520 696e 2076 616c 7565 733a  value in values:
+00019020: 0a20 2020 2020 2020 2020 2020 2070 7969  .            pyi
+00019030: 6e6b 5f6c 696e 6573 5f61 7267 732e 6170  nk_lines_args.ap
+00019040: 7065 6e64 2866 222d 2d70 7969 6e6b 2d6c  pend(f"--pyink-l
+00019050: 696e 6573 3d7b 7661 6c75 657d 2229 0a20  ines={value}"). 
+00019060: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00019070: 426c 6163 6b52 756e 6e65 7228 292e 696e  BlackRunner().in
+00019080: 766f 6b65 280a 2020 2020 2020 2020 2020  voke(.          
+00019090: 2020 7079 696e 6b2e 6d61 696e 2c20 7079    pyink.main, py
+000190a0: 696e 6b5f 6c69 6e65 735f 6172 6773 202b  ink_lines_args +
+000190b0: 205b 222d 2d64 6966 6622 2c20 6578 616d   ["--diff", exam
+000190c0: 706c 655d 0a20 2020 2020 2020 2029 0a20  ple].        ). 
+000190d0: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+000190e0: 7375 6c74 2e73 7464 6f75 745f 6279 7465  sult.stdout_byte
+000190f0: 7320 6973 206e 6f74 204e 6f6e 650a 2020  s is not None.  
+00019100: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+00019110: 756c 742e 6578 6974 5f63 6f64 6520 3d3d  ult.exit_code ==
+00019120: 2030 0a20 2020 2020 2020 2061 7373 6572   0.        asser
+00019130: 7420 7265 7375 6c74 2e73 7464 6f75 745f  t result.stdout_
+00019140: 6279 7465 7320 6973 206e 6f74 204e 6f6e  bytes is not Non
+00019150: 650a 0a20 2020 2020 2020 2073 7464 6f75  e..        stdou
+00019160: 7420 3d20 7365 6c66 2e64 6563 6f64 655f  t = self.decode_
+00019170: 616e 645f 6e6f 726d 616c 697a 6564 2872  and_normalized(r
+00019180: 6573 756c 742e 7374 646f 7574 5f62 7974  esult.stdout_byt
+00019190: 6573 290a 2020 2020 2020 2020 6173 7365  es).        asse
+000191a0: 7274 2022 2d66 726f 6d22 206e 6f74 2069  rt "-from" not i
+000191b0: 6e20 7374 646f 7574 0a20 2020 2020 2020  n stdout.       
+000191c0: 2061 7373 6572 7420 222d 2070 6173 735c   assert "- pass\
+000191d0: 6e2b 2020 2020 7061 7373 5c6e 2220 696e  n+    pass\n" in
+000191e0: 2073 7464 6f75 740a 0a20 2020 2040 7079   stdout..    @py
+000191f0: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+00019200: 7472 697a 6528 0a20 2020 2020 2020 2022  trize(.        "
+00019210: 7661 6c75 652c 6d65 7373 6167 6522 2c0a  value,message",.
+00019220: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00019230: 2020 2020 2020 2822 312c 3222 2c20 2249        ("1,2", "I
+00019240: 6e63 6f72 7265 6374 202d 2d70 7969 6e6b  ncorrect --pyink
+00019250: 2d6c 696e 6573 2066 6f72 6d61 742c 2065  -lines format, e
+00019260: 7870 6563 7420 2753 5441 5254 2d45 4e44  xpect 'START-END
+00019270: 2722 292c 0a20 2020 2020 2020 2020 2020  '"),.           
+00019280: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00019290: 2020 2022 7374 6172 742d 656e 6422 2c0a     "start-end",.
+000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192b0: 2249 6e63 6f72 7265 6374 202d 2d70 7969  "Incorrect --pyi
+000192c0: 6e6b 2d6c 696e 6573 2076 616c 7565 2c20  nk-lines value, 
+000192d0: 6578 7065 6374 2069 6e74 6567 6572 2072  expect integer r
+000192e0: 616e 6765 732c 2066 6f75 6e64 222c 0a20  anges, found",. 
+000192f0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00019300: 2020 2020 2020 5d2c 0a20 2020 2029 0a20        ],.    ). 
+00019310: 2020 2064 6566 2074 6573 745f 7079 696e     def test_pyin
+00019320: 6b5f 6c69 6e65 735f 696e 636f 7272 6563  k_lines_incorrec
+00019330: 7428 7365 6c66 2c20 7661 6c75 652c 206d  t(self, value, m
+00019340: 6573 7361 6765 2920 2d3e 204e 6f6e 653a  essage) -> None:
+00019350: 0a20 2020 2020 2020 2070 6174 6820 3d20  .        path = 
+00019360: 5448 4953 5f44 4952 202f 2022 6461 7461  THIS_DIR / "data
+00019370: 2220 2f20 2270 7969 6e6b 5f63 6f6e 6669  " / "pyink_confi
+00019380: 6773 220a 2020 2020 2020 2020 6578 616d  gs".        exam
+00019390: 706c 6520 3d20 7374 7228 7061 7468 202f  ple = str(path /
+000193a0: 2022 6578 616d 706c 652e 7079 2229 0a20   "example.py"). 
+000193b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000193c0: 426c 6163 6b52 756e 6e65 7228 292e 696e  BlackRunner().in
+000193d0: 766f 6b65 2870 7969 6e6b 2e6d 6169 6e2c  voke(pyink.main,
+000193e0: 205b 6622 2d2d 7079 696e 6b2d 6c69 6e65   [f"--pyink-line
+000193f0: 733d 7b76 616c 7565 7d22 2c20 6578 616d  s={value}", exam
+00019400: 706c 655d 290a 2020 2020 2020 2020 6173  ple]).        as
+00019410: 7365 7274 2072 6573 756c 742e 6578 6974  sert result.exit
+00019420: 5f63 6f64 6520 3d3d 2031 0a20 2020 2020  _code == 1.     
+00019430: 2020 2061 7373 6572 7420 7265 7375 6c74     assert result
+00019440: 2e73 7464 6572 725f 6279 7465 7320 6973  .stderr_bytes is
+00019450: 206e 6f74 204e 6f6e 650a 0a20 2020 2020   not None..     
+00019460: 2020 2061 7373 6572 7420 6d65 7373 6167     assert messag
+00019470: 6520 696e 2072 6573 756c 742e 7374 6465  e in result.stde
+00019480: 7272 5f62 7974 6573 2e64 6563 6f64 6528  rr_bytes.decode(
+00019490: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000194a0: 7079 696e 6b5f 7573 655f 6d61 6a6f 7269  pyink_use_majori
+000194b0: 7479 5f71 756f 7465 7328 7365 6c66 2920  ty_quotes(self) 
+000194c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000194d0: 2070 6174 6820 3d20 5448 4953 5f44 4952   path = THIS_DIR
+000194e0: 202f 2022 6461 7461 2220 2f20 2270 7969   / "data" / "pyi
+000194f0: 6e6b 5f63 6f6e 6669 6773 220a 2020 2020  nk_configs".    
+00019500: 2020 2020 6578 616d 706c 6520 3d20 7374      example = st
+00019510: 7228 7061 7468 202f 2022 6d61 6a6f 7269  r(path / "majori
+00019520: 7479 5f71 756f 7465 732e 7079 2229 0a20  ty_quotes.py"). 
+00019530: 2020 2020 2020 2063 6f6e 6669 6720 3d20         config = 
+00019540: 7374 7228 7061 7468 202f 2022 6d61 6a6f  str(path / "majo
+00019550: 7269 7479 5f71 756f 7465 732e 746f 6d6c  rity_quotes.toml
+00019560: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
+00019570: 7420 3d20 426c 6163 6b52 756e 6e65 7228  t = BlackRunner(
+00019580: 292e 696e 766f 6b65 280a 2020 2020 2020  ).invoke(.      
+00019590: 2020 2020 2020 7079 696e 6b2e 6d61 696e        pyink.main
+000195a0: 2c20 5b22 2d2d 6469 6666 222c 2022 2d2d  , ["--diff", "--
+000195b0: 636f 6e66 6967 222c 2063 6f6e 6669 672c  config", config,
+000195c0: 2065 7861 6d70 6c65 5d0a 2020 2020 2020   example].      
+000195d0: 2020 290a 2020 2020 2020 2020 6173 7365    ).        asse
+000195e0: 7274 2072 6573 756c 742e 6578 6974 5f63  rt result.exit_c
+000195f0: 6f64 6520 3d3d 2030 0a20 2020 2020 2020  ode == 0.       
+00019600: 2061 7373 6572 7420 7265 7375 6c74 2e73   assert result.s
+00019610: 7464 6f75 745f 6279 7465 7320 6973 206e  tdout_bytes is n
+00019620: 6f74 204e 6f6e 650a 0a20 2020 2020 2020  ot None..       
+00019630: 2064 6966 6620 3d20 2222 222d 5f64 6f75   diff = """-_dou
+00019640: 626c 6520 3d20 2244 6f75 626c 6522 5c6e  ble = "Double"\n
+00019650: 2b5f 646f 7562 6c65 203d 2027 446f 7562  +_double = 'Doub
+00019660: 6c65 275c 6e22 2222 0a20 2020 2020 2020  le'\n""".       
+00019670: 2061 7373 6572 7420 6469 6666 2069 6e20   assert diff in 
+00019680: 7365 6c66 2e64 6563 6f64 655f 616e 645f  self.decode_and_
+00019690: 6e6f 726d 616c 697a 6564 2872 6573 756c  normalized(resul
+000196a0: 742e 7374 646f 7574 5f62 7974 6573 290a  t.stdout_bytes).
+000196b0: 0a0a 7472 793a 0a20 2020 2077 6974 6820  ..try:.    with 
+000196c0: 6f70 656e 2870 7969 6e6b 2e5f 5f66 696c  open(pyink.__fil
+000196d0: 655f 5f2c 2022 7222 2c20 656e 636f 6469  e__, "r", encodi
+000196e0: 6e67 3d22 7574 662d 3822 2920 6173 205f  ng="utf-8") as _
+000196f0: 6266 3a0a 2020 2020 2020 2020 626c 6163  bf:.        blac
+00019700: 6b5f 736f 7572 6365 5f6c 696e 6573 203d  k_source_lines =
+00019710: 205f 6266 2e72 6561 646c 696e 6573 2829   _bf.readlines()
+00019720: 0a65 7863 6570 7420 556e 6963 6f64 6544  .except UnicodeD
+00019730: 6563 6f64 6545 7272 6f72 3a0a 2020 2020  ecodeError:.    
+00019740: 6966 206e 6f74 2070 7969 6e6b 2e43 4f4d  if not pyink.COM
+00019750: 5049 4c45 443a 0a20 2020 2020 2020 2072  PILED:.        r
+00019760: 6169 7365 0a0a 0a64 6566 2074 7261 6365  aise...def trace
+00019770: 6675 6e63 280a 2020 2020 6672 616d 653a  func(.    frame:
+00019780: 2074 7970 6573 2e46 7261 6d65 5479 7065   types.FrameType
+00019790: 2c20 6576 656e 743a 2073 7472 2c20 6172  , event: str, ar
+000197a0: 673a 2041 6e79 0a29 202d 3e20 4361 6c6c  g: Any.) -> Call
+000197b0: 6162 6c65 5b5b 7479 7065 732e 4672 616d  able[[types.Fram
+000197c0: 6554 7970 652c 2073 7472 2c20 416e 795d  eType, str, Any]
+000197d0: 2c20 416e 795d 3a0a 2020 2020 2222 2253  , Any]:.    """S
+000197e0: 686f 7720 6675 6e63 7469 6f6e 2063 616c  how function cal
+000197f0: 6c73 2060 6672 6f6d 2070 7969 6e6b 2f5f  ls `from pyink/_
+00019800: 5f69 6e69 745f 5f2e 7079 6020 6173 2074  _init__.py` as t
+00019810: 6865 7920 6861 7070 656e 2e0a 0a20 2020  hey happen...   
+00019820: 2052 6567 6973 7465 7220 7468 6973 2077   Register this w
+00019830: 6974 6820 6073 7973 2e73 6574 7472 6163  ith `sys.settrac
+00019840: 6528 2960 2069 6e20 6120 7465 7374 2079  e()` in a test y
+00019850: 6f75 2772 6520 6465 6275 6767 696e 672e  ou're debugging.
+00019860: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
+00019870: 6576 656e 7420 213d 2022 6361 6c6c 223a  event != "call":
+00019880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019890: 7472 6163 6566 756e 630a 0a20 2020 2073  tracefunc..    s
+000198a0: 7461 636b 203d 206c 656e 2869 6e73 7065  tack = len(inspe
+000198b0: 6374 2e73 7461 636b 2829 2920 2d20 3139  ct.stack()) - 19
+000198c0: 0a20 2020 2073 7461 636b 202a 3d20 320a  .    stack *= 2.
+000198d0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
+000198e0: 7261 6d65 2e66 5f63 6f64 652e 636f 5f66  rame.f_code.co_f
+000198f0: 696c 656e 616d 650a 2020 2020 6c69 6e65  ilename.    line
+00019900: 6e6f 203d 2066 7261 6d65 2e66 5f6c 696e  no = frame.f_lin
+00019910: 656e 6f0a 2020 2020 6675 6e63 5f73 6967  eno.    func_sig
+00019920: 5f6c 696e 656e 6f20 3d20 6c69 6e65 6e6f  _lineno = lineno
+00019930: 202d 2031 0a20 2020 2066 756e 636e 616d   - 1.    funcnam
+00019940: 6520 3d20 626c 6163 6b5f 736f 7572 6365  e = black_source
+00019950: 5f6c 696e 6573 5b66 756e 635f 7369 675f  _lines[func_sig_
+00019960: 6c69 6e65 6e6f 5d2e 7374 7269 7028 290a  lineno].strip().
+00019970: 2020 2020 7768 696c 6520 6675 6e63 6e61      while funcna
+00019980: 6d65 2e73 7461 7274 7377 6974 6828 2240  me.startswith("@
+00019990: 2229 3a0a 2020 2020 2020 2020 6675 6e63  "):.        func
+000199a0: 5f73 6967 5f6c 696e 656e 6f20 2b3d 2031  _sig_lineno += 1
+000199b0: 0a20 2020 2020 2020 2066 756e 636e 616d  .        funcnam
+000199c0: 6520 3d20 626c 6163 6b5f 736f 7572 6365  e = black_source
+000199d0: 5f6c 696e 6573 5b66 756e 635f 7369 675f  _lines[func_sig_
+000199e0: 6c69 6e65 6e6f 5d2e 7374 7269 7028 290a  lineno].strip().
+000199f0: 2020 2020 6966 2022 7079 696e 6b2f 5f5f      if "pyink/__
+00019a00: 696e 6974 5f5f 2e70 7922 2069 6e20 6669  init__.py" in fi
+00019a10: 6c65 6e61 6d65 3a0a 2020 2020 2020 2020  lename:.        
+00019a20: 7072 696e 7428 6622 7b27 2027 202a 2073  print(f"{' ' * s
+00019a30: 7461 636b 7d7b 6c69 6e65 6e6f 7d3a 7b66  tack}{lineno}:{f
+00019a40: 756e 636e 616d 657d 2229 0a20 2020 2072  uncname}").    r
+00019a50: 6574 7572 6e20 7472 6163 6566 756e 630a  eturn tracefunc.
```

### Comparing `pyink-23.3.1/tests/test_format.py` & `pyink-23.5.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/test_ink_adjusted_lines.py` & `pyink-23.5.0/tests/test_ink_adjusted_lines.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/test_ipynb.py` & `pyink-23.5.0/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/test_no_ipynb.py` & `pyink-23.5.0/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/test_trans.py` & `pyink-23.5.0/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/util.py` & `pyink-23.5.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/conditional_expression.py` & `pyink-23.5.0/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `pyink-23.5.0/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/jupyter/notebook_trailing_newline.ipynb` & `pyink-23.5.0/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/jupyter/notebook_without_changes.ipynb` & `pyink-23.5.0/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/debug_visitor.out` & `pyink-23.5.0/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/debug_visitor.py` & `pyink-23.5.0/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/decorators.py` & `pyink-23.5.0/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/docstring_no_string_normalization.py` & `pyink-23.5.0/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `pyink-23.5.0/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/force_py36.py` & `pyink-23.5.0/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/force_pyi.py` & `pyink-23.5.0/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/long_strings_flag_disabled.py` & `pyink-23.5.0/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/python2_detection.py` & `pyink-23.5.0/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/string_quotes.py` & `pyink-23.5.0/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/miscellaneous/stub.pyi` & `pyink-23.5.0/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/cantfit.py` & `pyink-23.5.0/tests/data/preview/cantfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,18 @@
 normal_name = (
     but_the_function_name_is_now_ridiculously_long_and_it_is_still_super_annoying(
         [1, 2, 3], arg1, [1, 2, 3], arg2, [1, 2, 3], arg3
     )
 )
 # long arguments
 normal_name = normal_function_name(
-    (
-        "but with super long string arguments that on their own exceed the line limit"
-        " so there's no way it can ever fit"
-    ),
-    (
-        "eggs with spam and eggs and spam with eggs with spam and eggs and spam with"
-        " eggs with spam and eggs and spam with eggs"
-    ),
+    "but with super long string arguments that on their own exceed the line limit so"
+    " there's no way it can ever fit",
+    "eggs with spam and eggs and spam with eggs with spam and eggs and spam with eggs"
+    " with spam and eggs and spam with eggs",
     this_is_a_ridiculously_long_name_and_nobody_in_their_right_mind_would_use_one_like_it=0,
 )
 string_variable_name = "a string that is waaaaaaaayyyyyyyy too long, even in parens, there's nothing you can do"  # noqa
 for key in """
     hostname
     port
     username
```

### Comparing `pyink-23.3.1/tests/data/preview/comments7.py` & `pyink-23.5.0/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/format_unicode_escape_seq.py` & `pyink-23.5.0/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/long_dict_values.py` & `pyink-23.5.0/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/long_strings.py` & `pyink-23.5.0/tests/data/preview/long_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,18 +319,16 @@
     " on one line. In fact it may even take up three or more lines... like four or"
     " five... but probably just three."
 )
 
 y = "Short string"
 
 print(
-    (
-        "This is a really long string inside of a print statement with extra arguments"
-        " attached at the end of it."
-    ),
+    "This is a really long string inside of a print statement with extra arguments"
+    " attached at the end of it.",
     x,
     y,
     z,
 )
 
 print(
     "This is a really long string inside of a print statement with no extra arguments"
@@ -497,23 +495,21 @@
 bad_split3 = (
     "What if we have inline comments on "  # First Comment
     "each line of a bad split? In that "  # Second Comment
     "case, we should just leave it alone."  # Third Comment
 )
 
 bad_split_func1(
-    (
-        "But what should happen when code has already "
-        "been formatted but in the wrong way? Like "
-        "with a space at the end instead of the "
-        "beginning. Or what about when it is split too "
-        "soon? In the case of a split that is too "
-        "short, black will try to honer the custom "
-        "split."
-    ),
+    "But what should happen when code has already "
+    "been formatted but in the wrong way? Like "
+    "with a space at the end instead of the "
+    "beginning. Or what about when it is split too "
+    "soon? In the case of a split that is too "
+    "short, black will try to honer the custom "
+    "split.",
     xxx,
     yyy,
     zzz,
 )
 
 bad_split_func2(
     xxx,
@@ -608,19 +604,17 @@
 
 comment_string = (  # This comment gets thrown to the top.
     "Long lines with inline comments should have their comments appended to the"
     " reformatted string's enclosing right parentheses."
 )
 
 arg_comment_string = print(
-    (  # This comment gets thrown to the top.
-        "Long lines with inline comments which are apart of (and not the only member"
-        " of) an argument list should have their comments appended to the reformatted"
-        " string's enclosing left parentheses."
-    ),
+    "Long lines with inline comments which are apart of (and not the only member of) an"
+    " argument list should have their comments appended to the reformatted string's"
+    " enclosing left parentheses.",  # This comment gets thrown to the top.
     "Arg #2",
     "Arg #3",
     "Arg #4",
     "Arg #5",
 )
 
 pragma_comment_string1 = "Lines which end with an inline pragma comment of the form `# <pragma>: <...>` should be left alone."  # noqa: E501
@@ -672,39 +666,31 @@
 
 return (
     "A really really really really really really really really really really really"
     " really really long {} {}".format("return", "value")
 )
 
 func_with_bad_comma(
-    (
-        "This is a really long string argument to a function that has a trailing comma"
-        " which should NOT be there."
-    ),
+    "This is a really long string argument to a function that has a trailing comma"
+    " which should NOT be there.",
 )
 
 func_with_bad_comma(
-    (  # comment after comma
-        "This is a really long string argument to a function that has a trailing comma"
-        " which should NOT be there."
-    ),
+    "This is a really long string argument to a function that has a trailing comma"
+    " which should NOT be there.",  # comment after comma
 )
 
 func_with_bad_comma(
-    (
-        "This is a really long string argument to a function that has a trailing comma"
-        " which should NOT be there."
-    ),
+    "This is a really long string argument to a function that has a trailing comma"
+    " which should NOT be there.",
 )
 
 func_with_bad_comma(
-    (  # comment after comma
-        "This is a really long string argument to a function that has a trailing comma"
-        " which should NOT be there."
-    ),
+    "This is a really long string argument to a function that has a trailing comma"
+    " which should NOT be there.",  # comment after comma
 )
 
 func_with_bad_parens_that_wont_fit_in_one_line(
     "short string that should have parens stripped", x, y, z
 )
 
 func_with_bad_parens_that_wont_fit_in_one_line(
```

### Comparing `pyink-23.3.1/tests/data/preview/long_strings__east_asian_width.py` & `pyink-23.5.0/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/long_strings__edge_case.py` & `pyink-23.5.0/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/long_strings__regression.py` & `pyink-23.5.0/tests/data/preview/long_strings__regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,32 +711,28 @@
             )
 
 
 class A:
     def foo():
         some_func_call(
             "xxxxxxxxxx",
-            (
-                "xx {xxxxxxxxxxx}/xxxxxxxxxxx.xxx xxxx.xxx && xxxxxx -x "
-                '"xxxx xxxxxxx xxxxxx xxxx; xxxx xxxxxx_xxxxx xxxxxx xxxx; '
-                "xxxx.xxxx_xxxxxx(['xxxx.xxx'], xxxx.xxxxxxx().xxxxxxxxxx)\" "
-            ),
+            "xx {xxxxxxxxxxx}/xxxxxxxxxxx.xxx xxxx.xxx && xxxxxx -x "
+            '"xxxx xxxxxxx xxxxxx xxxx; xxxx xxxxxx_xxxxx xxxxxx xxxx; '
+            "xxxx.xxxx_xxxxxx(['xxxx.xxx'], xxxx.xxxxxxx().xxxxxxxxxx)\" ",
             None,
             ("xxxxxxxxxxx",),
         ),
 
 
 class A:
     def foo():
         some_func_call(
-            (
-                "xx {xxxxxxxxxxx}/xxxxxxxxxxx.xxx xxxx.xxx && xxxxxx -x "
-                "xxxx, ('xxxxxxx xxxxxx xxxx, xxxx') xxxxxx_xxxxx xxxxxx xxxx; "
-                "xxxx.xxxx_xxxxxx(['xxxx.xxx'], xxxx.xxxxxxx().xxxxxxxxxx)\" "
-            ),
+            "xx {xxxxxxxxxxx}/xxxxxxxxxxx.xxx xxxx.xxx && xxxxxx -x "
+            "xxxx, ('xxxxxxx xxxxxx xxxx, xxxx') xxxxxx_xxxxx xxxxxx xxxx; "
+            "xxxx.xxxx_xxxxxx(['xxxx.xxx'], xxxx.xxxxxxx().xxxxxxxxxx)\" ",
             None,
             ("xxxxxxxxxxx",),
         ),
 
 
 xxxxxxx = {
     "xx": (
@@ -846,18 +842,16 @@
 some_commented_string = (
     "This string is long but not so long that it needs hahahah toooooo be so greatttt"  # But these
     " {} that I just can't think of any more good words to say about it at"  # comments will stay
     " allllllllllll".format("ha")  # comments here are fine
 )
 
 lpar_and_rpar_have_comments = func_call(  # LPAR Comment
-    (  # Comma Comment
-        "Long really ridiculous type of string that shouldn't really even exist at all."
-        " I mean commmme onnn!!!"
-    ),
+    "Long really ridiculous type of string that shouldn't really even exist at all. I"
+    " mean commmme onnn!!!",  # Comma Comment
 )  # RPAR Comment
 
 cmd_fstring = (
     "sudo -E deluge-console info --detailed --sort-reverse=time_added "
     f"{'' if ID is None else ID} | perl -nE 'print if /^{field}:/'"
 )
```

### Comparing `pyink-23.3.1/tests/data/preview/long_strings__type_annotations.py` & `pyink-23.5.0/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/multiline_strings.py` & `pyink-23.5.0/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/prefer_rhs_split.py` & `pyink-23.5.0/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview/trailing_comma.py` & `pyink-23.5.0/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/targeting_py38.py` & `pyink-23.5.0/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/targeting_py39.py` & `pyink-23.5.0/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `pyink-23.5.0/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/parenthesized_context_managers.py` & `pyink-23.5.0/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/pattern_matching_complex.py` & `pyink-23.5.0/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/pattern_matching_extras.py` & `pyink-23.5.0/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/pattern_matching_generic.py` & `pyink-23.5.0/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/pattern_matching_simple.py` & `pyink-23.5.0/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_310/pattern_matching_style.py` & `pyink-23.5.0/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_311/pep_646.py` & `pyink-23.5.0/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_311/pep_654.py` & `pyink-23.5.0/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_311/pep_654_style.py` & `pyink-23.5.0/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_36/numeric_literals.py` & `pyink-23.5.0/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_37/python37.py` & `pyink-23.5.0/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_38/pep_570.py` & `pyink-23.5.0/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_38/pep_572.py` & `pyink-23.5.0/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_38/pep_572_remove_parens.py` & `pyink-23.5.0/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_38/python38.py` & `pyink-23.5.0/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_39/python39.py` & `pyink-23.5.0/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/py_39/remove_with_brackets.py` & `pyink-23.5.0/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/pyink/indent.py` & `pyink-23.5.0/tests/data/pyink/indent.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/pyink/nested_brackets.py` & `pyink-23.5.0/tests/data/pyink/nested_brackets.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/pyink/nested_brackets_explodes.py` & `pyink-23.5.0/tests/data/pyink/nested_brackets_explodes.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/pyink/pragma_comments.py` & `pyink-23.5.0/tests/data/pyink/pragma_comments.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/pyink/str_concat_in_func_args.py` & `pyink-23.5.0/tests/data/pyink/str_concat_in_func_args.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,52 +12,74 @@
     y,
     z,
 )
 
 arg_comment_string = print(
     "Long lines with inline comments which are apart of (and not the only member of) an"
     " argument list should have their comments appended to the reformatted string's"
-    " enclosing left parentheses.",  # This comment gets thrown to the top.
+    " enclosing left parentheses.",  # This is a comment
     "Arg #2",
     "Arg #3",
     "Arg #4",
     "Arg #5",
 )
 
+already_wrapped_in_parens(
+    (
+        " lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod"
+        " tempor incididunt ut labore et dolore magna aliqua Ut enim ad minim"
+    ),
+    " lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod tempor",
+)
+
+already_wrapped_in_parens_but_short(
+    (
+        "short"
+        " string"
+    ),
+    another_arg,
+)
+
 
 # output
 
 
 # long arguments
 normal_name = normal_function_name(
-    (
-        "but with super long string arguments that on their own exceed the line"
-        " limit so there's no way it can ever fit"
-    ),
-    (
-        "eggs with spam and eggs and spam with eggs with spam and eggs and spam"
-        " with eggs with spam and eggs and spam with eggs"
-    ),
+    "but with super long string arguments that on their own exceed the line"
+    " limit so there's no way it can ever fit",
+    "eggs with spam and eggs and spam with eggs with spam and eggs and spam"
+    " with eggs with spam and eggs and spam with eggs",
     this_is_a_ridiculously_long_name_and_nobody_in_their_right_mind_would_use_one_like_it=0,
 )
 
 print(
-    (
-        "This is a really long string inside of a print statement with extra"
-        " arguments attached at the end of it."
-    ),
+    "This is a really long string inside of a print statement with extra"
+    " arguments attached at the end of it.",
     x,
     y,
     z,
 )
 
 arg_comment_string = print(
-    (  # This comment gets thrown to the top.
-        "Long lines with inline comments which are apart of (and not the only"
-        " member of) an argument list should have their comments appended to"
-        " the reformatted string's enclosing left parentheses."
-    ),
+    "Long lines with inline comments which are apart of (and not the only"
+    " member of) an argument list should have their comments appended to the"
+    " reformatted string's enclosing left parentheses.",  # This is a comment
     "Arg #2",
     "Arg #3",
     "Arg #4",
     "Arg #5",
 )
+
+already_wrapped_in_parens(
+    (
+        " lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod"
+        " tempor incididunt ut labore et dolore magna aliqua Ut enim ad minim"
+    ),
+    " lorem ipsum dolor sit amet consectetur adipiscing elit sed do eiusmod"
+    " tempor",
+)
+
+already_wrapped_in_parens_but_short(
+    "short string",
+    another_arg,
+)
```

### Comparing `pyink-23.3.1/tests/data/simple_cases/attribute_access_on_number_literals.py` & `pyink-23.5.0/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/class_blank_parentheses.py` & `pyink-23.5.0/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/class_methods_new_line.py` & `pyink-23.5.0/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/collections.py` & `pyink-23.5.0/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments.py` & `pyink-23.5.0/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments2.py` & `pyink-23.5.0/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments3.py` & `pyink-23.5.0/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments4.py` & `pyink-23.5.0/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments5.py` & `pyink-23.5.0/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments6.py` & `pyink-23.5.0/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments9.py` & `pyink-23.5.0/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/comments_non_breaking_space.py` & `pyink-23.5.0/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/composition.py` & `pyink-23.5.0/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/composition_no_trailing_comma.py` & `pyink-23.5.0/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/docstring.py` & `pyink-23.5.0/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/docstring_preview.py` & `pyink-23.5.0/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/empty_lines.py` & `pyink-23.5.0/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/expression.diff` & `pyink-23.5.0/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/expression.py` & `pyink-23.5.0/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fmtonoff.py` & `pyink-23.5.0/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fmtonoff2.py` & `pyink-23.5.0/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fmtonoff5.py` & `pyink-23.5.0/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fmtskip2.py` & `pyink-23.5.0/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fmtskip8.py` & `pyink-23.5.0/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/fstring.py` & `pyink-23.5.0/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/function.py` & `pyink-23.5.0/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/function2.py` & `pyink-23.5.0/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/function_trailing_comma.py` & `pyink-23.5.0/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/import_spacing.py` & `pyink-23.5.0/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/one_element_subscript.py` & `pyink-23.5.0/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/power_op_spacing.py` & `pyink-23.5.0/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `pyink-23.5.0/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/remove_await_parens.py` & `pyink-23.5.0/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/remove_except_parens.py` & `pyink-23.5.0/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/remove_for_brackets.py` & `pyink-23.5.0/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `pyink-23.5.0/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/remove_parens.py` & `pyink-23.5.0/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/return_annotation_brackets.py` & `pyink-23.5.0/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/skip_magic_trailing_comma.py` & `pyink-23.5.0/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/slices.py` & `pyink-23.5.0/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/string_prefixes.py` & `pyink-23.5.0/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/torture.py` & `pyink-23.5.0/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `pyink-23.5.0/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `pyink-23.5.0/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `pyink-23.5.0/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/LICENSE` & `pyink-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyink-23.3.1/pyproject.toml` & `pyink-23.5.0/pyproject.toml`

 * *Files identical despite different names*

