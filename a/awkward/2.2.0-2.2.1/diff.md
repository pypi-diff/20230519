# Comparing `tmp/awkward-2.2.0.tar.gz` & `tmp/awkward-2.2.1.tar.gz`

## Comparing `awkward-2.2.0.tar` & `awkward-2.2.1.tar`

### file list

```diff
@@ -1,850 +1,853 @@
--rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.0/CITATION.cff
--rw-r--r--   0        0        0    13578 2023-04-24 16:57:22.000000 awkward-2.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-04-24 16:57:22.000000 awkward-2.2.0/README.md
--rw-r--r--   0        0        0      241 2023-04-24 16:57:22.000000 awkward-2.2.0/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/conf.py
--rw-r--r--   0        0        0      346 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/index.md
--rw-r--r--   0        0        0    11642 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/redirects.json
--rw-r--r--   0        0        0      463 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/requirements.txt
--rw-r--r--   0        0        0      369 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    25309 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/reference/ak.behavior.rst
--rw-r--r--   0        0        0     1426 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/reference/index.md
--rw-r--r--   0        0        0     7349 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-04-24 16:57:22.000000 awkward-2.2.0/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1325 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/__init__.py
--rw-r--r--   0        0        0     5418 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_behavior.py
--rw-r--r--   0        0        0    39388 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    13424 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_do.py
--rw-r--r--   0        0        0    12279 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_errors.py
--rw-r--r--   0        0        0     5672 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5860 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_lookup.py
--rw-r--r--   0        0        0     5454 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    24569 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_reducers.py
--rw-r--r--   0        0        0     2041 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_typing.py
--rw-r--r--   0        0        0     2439 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forth.py
--rw-r--r--   0        0        0   103299 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8005 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/jax.py
--rw-r--r--   0        0        0     6017 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/numba.py
--rw-r--r--   0        0        0     8272 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/record.py
--rw-r--r--   0        0        0      165 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3763 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1781 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1902 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53533 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4485 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    11488 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    37988 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      755 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
--rw-r--r--   0        0        0      806 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0     1123 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0      623 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
--rw-r--r--   0        0        0      789 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0     6627 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35824 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31514 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49132 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1111 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    13294 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     4939 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2010 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2922 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    14150 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     2288 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    43770 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     8509 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    27803 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    40958 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    45020 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13347 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    40382 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    63462 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    59821 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    84844 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    49439 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    40526 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    54541 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    57744 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    18878 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6081 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5368 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3369 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    15415 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5638 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5133 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5621 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4715 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6004 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8208 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5084 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     7760 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4229 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4828 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3500 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     7381 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     3503 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5109 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3819 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5924 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5881 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3158 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      952 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9855 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6595 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12213 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5319 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4730 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3537 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     4672 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4581 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50451 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5323 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3467 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2727 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14486 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     4109 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30065 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11931 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3324 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     3000 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2513 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8934 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4757 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     6466 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     8103 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3603 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12413 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     6418 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4410 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3909 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5396 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4216 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9604 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3063 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     2839 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2670 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     7160 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10754 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2370 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6378 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1107 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13370 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11652 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4507 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2123 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    16968 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2785 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3382 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23979 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4304 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9461 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2484 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1138 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     8388 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5862 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6130 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3756 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8819 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     1914 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     2855 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6065 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4586 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8629 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3688 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1140 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0     9786 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/type.py
--rw-r--r--   0        0        0     4154 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     2261 2023-04-24 16:57:22.000000 awkward-2.2.0/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6361 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2338 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115760 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28376 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26467 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33145 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     3636 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4607 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2854 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     2765 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     5548 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4104 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0     2262 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      648 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2929 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0    37200 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2921 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5259 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5857 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      212 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0     1070 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      800 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      704 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      351 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1563 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1211 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      495 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.0/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9911 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1782 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-04-24 16:57:22.000000 awkward-2.2.0/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-04-24 16:57:22.000000 awkward-2.2.0/.gitignore
--rw-r--r--   0        0        0     1520 2023-04-24 16:57:22.000000 awkward-2.2.0/LICENSE
--rw-r--r--   0        0        0     8479 2023-04-24 16:57:22.000000 awkward-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-24 16:57:22.000000 awkward-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.1/CITATION.cff
+-rw-r--r--   0        0        0    13855 2023-04-24 16:57:22.000000 awkward-2.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-04-24 16:57:22.000000 awkward-2.2.1/README.md
+-rw-r--r--   0        0        0      241 2023-04-24 16:57:22.000000 awkward-2.2.1/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/redirects.json
+-rw-r--r--   0        0        0      463 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0      460 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    25534 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/index.md
+-rw-r--r--   0        0        0     7349 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1325 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/__init__.py
+-rw-r--r--   0        0        0     5026 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    39029 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0    13617 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_do.py
+-rw-r--r--   0        0        0    12279 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5672 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     5454 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    24569 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     2041 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2498 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forth.py
+-rw-r--r--   0        0        0   103232 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8005 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/jax.py
+-rw-r--r--   0        0        0     6017 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/numba.py
+-rw-r--r--   0        0        0     8272 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/record.py
+-rw-r--r--   0        0        0     1002 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1781 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1902 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53533 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4485 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    11395 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    37988 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      755 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
+-rw-r--r--   0        0        0      806 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0     1123 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
+-rw-r--r--   0        0        0      623 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
+-rw-r--r--   0        0        0      789 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0     6627 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35824 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31510 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49124 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1111 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    13294 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     4939 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2010 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     2922 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14150 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     2288 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    43889 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     8509 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    27803 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    40958 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13347 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    40382 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    63462 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    60161 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    85023 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    49439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    45029 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    54872 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    57740 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    18878 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     5955 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5242 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3244 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    15639 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5630 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5508 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4602 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     5902 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8095 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     4971 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     7647 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4116 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4828 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3500 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8181 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     3503 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5109 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3819 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5924 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5881 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3158 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      952 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9855 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6595 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1420 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8118 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12213 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5319 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4730 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3537 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     4672 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4581 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50451 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5323 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3467 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7802 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3154 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      813 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2727 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14486 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1839 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1651 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     4109 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1716 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    30065 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2282 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11931 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3324 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     3000 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8859 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      873 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2513 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      705 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2568 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8934 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3258 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4753 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     6466 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     8103 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3603 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12413 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3217 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     6418 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4410 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2081 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5103 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3909 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1951 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4362 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1786 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5396 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4216 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2275 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9604 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3063 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     2839 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2670 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     7160 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3058 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10754 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4931 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6725 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2370 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6378 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6050 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1107 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13370 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11648 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4507 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2612 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2123 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3354 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    16968 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2785 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3382 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23979 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4422 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9461 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2484 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1138 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2659 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     8388 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5862 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6130 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2600 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1848 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3756 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1509 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2134 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8819 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2168 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     2972 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6174 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4866 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     9079 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3874 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1341 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10063 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4602 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     2492 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6321 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2338 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   113054 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28376 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26467 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33145 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18809 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4372 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      727 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4607 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2845 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1018 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2765 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     6059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4104 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      877 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      720 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2262 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37200 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5250 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5848 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      956 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0     1070 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1211 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      495 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9911 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1782 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-04-24 16:57:22.000000 awkward-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1520 2023-04-24 16:57:22.000000 awkward-2.2.1/LICENSE
+-rw-r--r--   0        0        0     8479 2023-04-24 16:57:22.000000 awkward-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-24 16:57:22.000000 awkward-2.2.1/PKG-INFO
```

### Comparing `awkward-2.2.0/CITATION.cff` & `awkward-2.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/CONTRIBUTING.md` & `awkward-2.2.1/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,20 @@
 
   * Jim Pivarski ([jpivarski](https://github.com/jpivarski))
 
 There are two kinds of releases: (1) `awkward-cpp` updates, which only occur when the C++ is updated (rare) and involves compilation on many platforms (takes hours), and (2) `awkward` updates, which can happen with any bug-fix. The [releases listed in GitHub](https://github.com/scikit-hep/awkward/releases) are `awkward` releases, not `awkward-cpp`.
 
 If you need your merged pull request to be deployed in a release, just ask!
 
-#### Awkward-cpp releases
-When making an `awkward-cpp` release (1), the following manual steps must also be taken:
-- Creating a `git` tag `awkward-cpp-{version}` for the new version epoch.
-
-#### Awkward releases
-When making an `awkward` release (2), the following manual steps must also be taken:
-- Attaching the `headers.zip` from the `deploy.yml` workflow to the release artefacts.
-- Adding a `doc/switcher.json` entry for new minor/major versions.
+#### `awkward-cpp` releases
+To make an `awkward-cpp` release:
+1. A commit to `main` should increase the version number in `awkward-cpp/pyproject.toml`
+2. The [Deploy C++](https://github.com/scikit-hep/awkward/actions/workflows/deploy-cpp.yml) GitHub Actions workflow should be manually triggered.
+3. A `git` tag `awkward-cpp-{version}` should be created for the new version epoch.
+
+#### `awkward` releases
+To make an `awkward` release:
+1. A commit to `main` should increase the version number in `pyproject.toml`
+2. A new GitHub release must be published.
+3. A `docs/switcher.json` entry must be added for new minor/major versions.
+
+Pushes that modify `docs/switcher.json` on `main` will automatically be synchronised with AWS.
```

### Comparing `awkward-2.2.0/README.md` & `awkward-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/_toc.yml` & `awkward-2.2.1/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/conf.py` & `awkward-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/index.md` & `awkward-2.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/prepare_docstrings.py` & `awkward-2.2.1/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/redirects-user-guide.json` & `awkward-2.2.1/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/redirects.json` & `awkward-2.2.1/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/_static/css/awkward.css` & `awkward-2.2.1/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/getting-started/community-tutorials.md` & `awkward-2.2.1/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/getting-started/index.md` & `awkward-2.2.1/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/getting-started/papers-and-talks.md` & `awkward-2.2.1/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.2.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/image/example-hierarchy.svg` & `awkward-2.2.1/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/reference/ak.behavior.rst` & `awkward-2.2.1/docs/reference/ak.behavior.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-ak.behavior
------------
+# ak.behavior
 
-.. py:data:: ak.behavior
+```{py:data} ak.behavior
+```
 
-* `Motivation <#motivation>`__
-* `Parameters and behaviors <#parameters-and-behaviors>`__
-* `Adding behavior to records <#adding-behavior-to-records>`__
-* `Overriding NumPy ufuncs and binary operators <#overriding-numpy-ufuncs-and-binary-operators>`__
-* `Mixin decorators <#mixin-decorators>`__
-* `Adding behavior to arrays <#adding-behavior-to-arrays>`__
-* `Custom type names <#custom-type-names>`__
-* `Custom broadcasting <#custom-broadcasting>`__
-* `Overriding behavior in Numba <#overriding-behavior-in-numba>`__
-* `Complete example <#complete-example>`__
-
-Motivation
-==========
+## Motivation
 
 A data structure is defined both in terms of the information it encodes and
 in how it can be used. For example, a hash-table is not just a buffer, it's
 also the "get" and "set" operations that make the buffer usable as a key-value
 store. Awkward Arrays have a suite of operations for transforming tree
 structures into new tree structures, but an application of these structures to
 a data analysis problem should be able to interpret them as objects in the
@@ -38,641 +26,707 @@
 methods would have to be converted, or the analysis would have to be broken
 into different cases for each data generation. This problem is known as
 schema evolution, and there are many solutions to it.
 
 The approach taken by the Awkward Array library is to encode very little
 interpretation into the data themselves and apply an interpretation as
 late as possible. Thus, a latitude-longitude record might be stamped with
-the name ``"latlon"``, but the operations on it are added immediately before
+the name `"latlon"`, but the operations on it are added immediately before
 the user wants them. These operations can be written in such a way that
-they only require the ``"latlon"`` to have ``lat`` and ``lon`` fields, so
+they only require the `"latlon"` to have `lat` and `lon` fields, so
 different versions of the data can have additional fields or even be
 embedded in different structures.
 
-Parameters and behaviors
-========================
+## Parameters and behaviors
 
 In Awkward Array, metadata are embedded in data using an array node's
 **parameters**, and parameter-dependent operations can be defined using
 **behavior**. A global mapping from parameters to behavior is in a dict called
-:data:`.behavior`:
-
-.. code-block:: python
+{data}`.behavior`:
 
-    >>> import awkward as ak
-    >>> ak.behavior
+```python
+>>> import awkward as ak
+>>> ak.behavior
+```
 
-but behavior dicts can also be loaded into :class:`ak.Array`,
-:class:`ak.Record`, and :class:`ak.ArrayBuilder` objects as a
+but behavior dicts can also be loaded into {class}`ak.Array`,
+{class}`ak.Record`, and {class}`ak.ArrayBuilder` objects as a
 constructor argument. See
-:attr:`ak.Array.behavior`.
+{attr}`ak.Array.behavior`.
 
 The general flow is
 
-* **parameters** link data objects to names;
-* **behavior** links names to code.
+- **parameters** link data objects to names;
+- **behavior** links names to code.
 
 In large datasets, parameters may be hard to change (permanently, at least:
 on-the-fly parameter changes are easier), but behavior is easy to change
 (it is always assigned on-the-fly).
 
 In the following example, we create two nested arrays of records with fields
-``"x"`` and ``"y"`` and the records are named ``"point"``.
-
-.. code-block:: python
+`"x"` and `"y"` and the records are named `"point"`.
 
-    one = ak.Array([[{"x": 1, "y": 1.1}, {"x": 2, "y": 2.2}, {"x": 3, "y": 3.3}],
-                    [],
-                    [{"x": 4, "y": 4.4}, {"x": 5, "y": 5.5}],
-                    [{"x": 6, "y": 6.6}],
-                    [{"x": 7, "y": 7.7}, {"x": 8, "y": 8.8}, {"x": 9, "y": 9.9}]],
-                   with_name="point")
-    two = ak.Array([[{"x": 0.9, "y": 1}, {"x": 2, "y": 2.2}, {"x": 2.9, "y": 3}],
-                    [],
-                    [{"x": 3.9, "y": 4}, {"x": 5, "y": 5.5}],
-                    [{"x": 5.9, "y": 6}],
-                    [{"x": 6.9, "y": 7}, {"x": 8, "y": 8.8}, {"x": 8.9, "y": 9}]],
-                   with_name="point")
+```python
+one = ak.Array([[{"x": 1, "y": 1.1}, {"x": 2, "y": 2.2}, {"x": 3, "y": 3.3}],
+                [],
+                [{"x": 4, "y": 4.4}, {"x": 5, "y": 5.5}],
+                [{"x": 6, "y": 6.6}],
+                [{"x": 7, "y": 7.7}, {"x": 8, "y": 8.8}, {"x": 9, "y": 9.9}]],
+               with_name="point")
+two = ak.Array([[{"x": 0.9, "y": 1}, {"x": 2, "y": 2.2}, {"x": 2.9, "y": 3}],
+                [],
+                [{"x": 3.9, "y": 4}, {"x": 5, "y": 5.5}],
+                [{"x": 5.9, "y": 6}],
+                [{"x": 6.9, "y": 7}, {"x": 8, "y": 8.8}, {"x": 8.9, "y": 9}]],
+               with_name="point")
+```
 
 The name appears in the way the type is presented as a string (a departure from
-`Datashape notation <https://datashape.readthedocs.io/>`__):
+[Datashape notation](https://datashape.readthedocs.io/)):
 
-.. code-block:: python
-
-    >>> ak.type(one)
-    5 * var * point["x": int64, "y": float64]
-
-and it may be accessed as the ``"__record__"`` property, through the
-:attr:`ak.Array.layout`:
-
-.. code-block:: python
-
-    >>> one.layout
-    <ListOffsetArray64>
-        <offsets><Index64 i="[0 3 3 5 6 9]" offset="0" length="6"/></offsets>
-        <content><RecordArray>
-            <parameters>
-                <param key="__record__">"point"</param>
-            </parameters>
-            <field index="0" key="x">
-                <NumpyArray format="l" shape="9" data="1 2 3 4 5 6 7 8 9"/>
-            </field>
-            <field index="1" key="y">
-                <NumpyArray format="d" shape="9" data="1.1 2.2 3.3 4.4 5.5 6.6 7.7 8.8 9.9"/>
-            </field>
-        </RecordArray></content>
-    </ListOffsetArray64>
-    >>> one.layout.content.parameters
-    {'__record__': 'point'}
-
-We have to dig into the layout's content because the ``"__record__"`` parameter
-is set on the :class:`ak.contents.RecordArray`, which is buried inside of a
-:class:`ak.contents.ListOffsetArray`.
-
-Alternatively, we can navigate to a single :class:`ak.Record` first:
-
-.. code-block:: python
-
-    >>> one[0, 0]
-    <Record {x: 1, y: 1.1} type='point["x": int64, "y": float64]'>
-    >>> one[0, 0].layout.parameters
-    {'__record__': 'point'}
+```python
+>>> ak.type(one)
+5 * var * point["x": int64, "y": float64]
+```
+
+and it may be accessed as the `"__record__"` property, through the
+{attr}`ak.Array.layout`:
+
+```python
+>>> one.layout
+<ListOffsetArray64>
+    <offsets><Index64 i="[0 3 3 5 6 9]" offset="0" length="6"/></offsets>
+    <content><RecordArray>
+        <parameters>
+            <param key="__record__">"point"</param>
+        </parameters>
+        <field index="0" key="x">
+            <NumpyArray format="l" shape="9" data="1 2 3 4 5 6 7 8 9"/>
+        </field>
+        <field index="1" key="y">
+            <NumpyArray format="d" shape="9" data="1.1 2.2 3.3 4.4 5.5 6.6 7.7 8.8 9.9"/>
+        </field>
+    </RecordArray></content>
+</ListOffsetArray64>
+>>> one.layout.content.parameters
+{'__record__': 'point'}
+```
+
+We have to dig into the layout's content because the `"__record__"` parameter
+is set on the {class}`ak.contents.RecordArray`, which is buried inside of a
+{class}`ak.contents.ListOffsetArray`.
+
+Alternatively, we can navigate to a single {class}`ak.Record` first:
+
+```python
+>>> one[0, 0]
+<Record {x: 1, y: 1.1} type='point["x": int64, "y": float64]'>
+>>> one[0, 0].layout.parameters
+{'__record__': 'point'}
+```
 
-Adding behavior to records
-==========================
+## Adding behavior to records
 
 Suppose we want the points in the above example to be able to calculate
 distances to other points. We can do this by creating a subclass of
-:class:`ak.Record` that has the new methods and associating it with
-the ``"__record__"`` name.
-
-.. code-block:: python
-
-    class Point(ak.Record):
-        def distance(self, other):
-            return np.sqrt((self.x - other.x)**2 + (self.y - other.y)**2)
-
-    ak.behavior["point"] = Point
-
-Now ``one[0, 0]`` is instantiated as a ``Point``, rather than a :class:`ak.Record`,
+{class}`ak.Record` that has the new methods and associating it with
+the `"__record__"` name.
 
-.. code-block:: python
-
-    >>> one[0, 0]
-    <Point {x: 1, y: 1.1} type='point["x": int64, "y": float64]'>
-
-and it has the ``distance`` method.
-
-.. code-block:: python
-
-    >>> for xs, ys in zip(one, two):
-    ...     for x, y in zip(xs, ys):
-    ...         print(x.distance(y))
-    0.14142135623730953
-    0.0
-    0.31622776601683783
-    0.4123105625617664
-    0.0
-    0.6082762530298216
-    0.7071067811865477
-    0.0
-    0.905538513813742
+```python
+class Point(ak.Record):
+    def distance(self, other):
+        return np.sqrt((self.x - other.x)**2 + (self.y - other.y)**2)
+
+ak.behavior["point"] = Point
+```
+
+Now `one[0, 0]` is instantiated as a `Point`, rather than a {class}`ak.Record`,
+
+```python
+>>> one[0, 0]
+<Point {x: 1, y: 1.1} type='point["x": int64, "y": float64]'>
+```
+
+and it has the `distance` method.
+
+```python
+>>> for xs, ys in zip(one, two):
+...     for x, y in zip(xs, ys):
+...         print(x.distance(y))
+0.14142135623730953
+0.0
+0.31622776601683783
+0.4123105625617664
+0.0
+0.6082762530298216
+0.7071067811865477
+0.0
+0.905538513813742
+```
 
 Looping over data in Python is inconvenient and slow; we want to compute
-quantities like this with array-at-a-time methods, but ``distance`` is
-bound to a :class:`ak.Record`, not an :class:`ak.Array` of records.
-
-.. code-block:: python
+quantities like this with array-at-a-time methods, but `distance` is
+bound to a {class}`ak.Record`, not an {class}`ak.Array` of records.
 
-    >>> one.distance(two)
-    AttributeError: no field named 'distance'
+```python
+>>> one.distance(two)
+AttributeError: no field named 'distance'
+```
 
-To add ``distance`` as a method on arrays of points, create a subclass of
-:class:`ak.Array` and attach that as ``ak.behavior[".", "point"]`` for
+To add `distance` as a method on arrays of points, create a subclass of
+{class}`ak.Array` and attach that as `ak.behavior[".", "point"]` for
 "array of points."
 
-.. code-block:: python
+```python
+class PointArray(ak.Array):
+    def distance(self, other):
+        return np.sqrt((self.x - other.x)**2 + (self.y - other.y)**2)
 
-    class PointArray(ak.Array):
-        def distance(self, other):
-            return np.sqrt((self.x - other.x)**2 + (self.y - other.y)**2)
+ak.behavior[".", "point"] = PointArray
+```
 
-    ak.behavior[".", "point"] = PointArray
-
-Now ``one[0]`` is a ``PointArray`` and can compute ``distance`` on arrays at a
+Now `one[0]` is a `PointArray` and can compute `distance` on arrays at a
 time. Thanks to NumPy's
-`universal function <https://docs.scipy.org/doc/numpy/reference/ufuncs.html>`__
+[universal function](https://docs.scipy.org/doc/numpy/reference/ufuncs.html)
 (ufunc) syntax, the expression is the same (and could perhaps be implemented
-once and used by both ``Point`` and ``PointArray``).
-
-.. code-block:: python
-
-    >>> one[0]
-    <PointArray [{x: 1, y: 1.1}, ... {x: 3, y: 3.3}] type='3 * point["x": int64, "y"...'>
-    >>> one[0].distance(two[0])
-    <Array [0.141, 0, 0.316] type='3 * float64'>
-
-But ``one`` itself is an ``Array`` of ``PointArrays``, and does not apply.
-
-.. code-block:: python
+once and used by both `Point` and `PointArray`).
 
-    >>> one
-    <Array [[{x: 1, y: 1.1}, ... x: 9, y: 9.9}]] type='5 * var * point["x": int64, "...'>
-    >>> one.distance(two)
-    AttributeError: no field named 'distance'
+```python
+>>> one[0]
+<PointArray [{x: 1, y: 1.1}, ... {x: 3, y: 3.3}] type='3 * point["x": int64, "y"...'>
+>>> one[0].distance(two[0])
+<Array [0.141, 0, 0.316] type='3 * float64'>
+```
+
+But `one` itself is an `Array` of `PointArrays`, and does not apply.
+
+```python
+>>> one
+<Array [[{x: 1, y: 1.1}, ... x: 9, y: 9.9}]] type='5 * var * point["x": int64, "...'>
+>>> one.distance(two)
+AttributeError: no field named 'distance'
+```
+
+We can make the assignment work at all levels of list-depth by using a `"*"`
+instead of a `"."`.
+
+```python
+ak.behavior["*", "point"] = PointArray
+```
 
-We can make the assignment work at all levels of list-depth by using a ``"*"``
-instead of a ``"."``.
-
-.. code-block:: python
-
-    ak.behavior["*", "point"] = PointArray
-
-One last caveat: our ``one`` array was created *before* this behavior was
+One last caveat: our `one` array was created *before* this behavior was
 assigned, so it needs to be recreated to be a member of the new class. The
-normal :class:`ak.Array` constructor is sufficient for this. This is only
+normal {class}`ak.Array` constructor is sufficient for this. This is only
 an issue if you're working interactively (but something to think about when
 debugging!).
 
-.. code-block:: python
-
-    >>> one = ak.Array(one)
-    >>> two = ak.Array(two)
+```python
+>>> one = ak.Array(one)
+>>> two = ak.Array(two)
+```
 
 Now it works, and again we're taking advantage of the fact that the expression
-for ``distance`` based on ufuncs works equally well on Awkward Arrays.
-
-.. code-block:: python
+for `distance` based on ufuncs works equally well on Awkward Arrays.
 
-    >>> one
-    <PointArray [[{x: 1, y: 1.1}, ... x: 9, y: 9.9}]] type='5 * var * point["x": int...'>
-    >>> one.distance(two)
-    <Array [[0.141, 0, 0.316, ... 0.707, 0, 0.906]] type='5 * var * float64'>
-
-**In most cases, you want to apply array-of-records for all levels of list-depth:** use ``ak.behavior["*", record_name]``.
-
-Overriding NumPy ufuncs and binary operators
-============================================
-
-The :class:`ak.Array` class overrides Python's binary operators with the
-equivalent ufuncs, so ``__eq__`` actually calls :data:`numpy.equal`, for instance.
-This is also true of other basic functions, like ``__abs__`` for overriding
-:func:`abs` with :data:`numpy.absolute`. Each ufunc is then passed down to the leaves
+```python
+>>> one
+<PointArray [[{x: 1, y: 1.1}, ... x: 9, y: 9.9}]] type='5 * var * point["x": int...'>
+>>> one.distance(two)
+<Array [[0.141, 0, 0.316, ... 0.707, 0, 0.906]] type='5 * var * float64'>
+```
+
+**In most cases, you want to apply array-of-records for all levels of list-depth:** use `ak.behavior["*", record_name]`.
+
+## Overriding NumPy ufuncs and binary operators
+
+The {class}`ak.Array` class overrides Python's binary operators with the
+equivalent ufuncs, so `__eq__` actually calls {data}`numpy.equal`, for instance.
+This is also true of other basic functions, like `__abs__` for overriding
+{func}`abs` with {data}`numpy.absolute`. Each ufunc is then passed down to the leaves
 (deepest sub-elements) of an Awkward data structure.
 
 For example,
 
-.. code-block:: python
-
-    >>> ak.Array([[1, 2, 3], [], [4]]) == ak.Array([[3, 2, 1], [], [4]])
-    <Array [[False, True, False], [], [True]] type='3 * var * bool'>
-
+```python
+>>> ak.Array([[1, 2, 3], [], [4]]) == ak.Array([[3, 2, 1], [], [4]])
+<Array [[False, True, False], [], [True]] type='3 * var * bool'>
+```
 
 However, this does not apply to records or named types until they are explicitly
 overridden:
 
-.. code-block:: python
+```python
+>>> one == two
+Traceback (most recent call last):
+  File "<stdin>", line 1, in <module>
+...
+ValueError: no overloads for custom types: equal(point, point)
+```
 
-    >>> one == two
-    Traceback (most recent call last):
-      File "<stdin>", line 1, in <module>
-    ...
-    ValueError: no overloads for custom types: equal(point, point)
-
-We might want to take an object-oriented view in which the ``==`` operation
+We might want to take an object-oriented view in which the `==` operation
 applies to points, regardless of how deeply they are nested. If we try to do
-it by adding ``__eq__`` as a method on ``PointArray``, it would work if the
-``PointArray`` is the top of the data structure, but not if it's nested within
+it by adding `__eq__` as a method on `PointArray`, it would work if the
+`PointArray` is the top of the data structure, but not if it's nested within
 another structure.
 
-Instead, we should override :data:`numpy.equal` itself. Custom ufunc overrides are
+Instead, we should override {data}`numpy.equal` itself. Custom ufunc overrides are
 checked at every step in broadcasting, so the override would be applied if
 point objects are discovered at any level.
 
-.. code-block:: python
-
-    def point_equal(left, right):
-        return np.logical_and(left.x == right.x, left.y == right.y)
-
-    ak.behavior[np.equal, "point", "point"] = point_equal
-
-The above should be read as "override :data`np.equal` for cases in which both
-arguments are ``"point"``."
-
-.. code-block:: python
-
-    >>> ak.to_list(one == two)
-    [[False, True, False], [], [False, True], [False], [False, True, False]]
-
-Similarly for overriding :func:`abs`
-
-.. code-block:: python
-
-    >>> def point_abs(point):
-    ...     return np.sqrt(point.x**2 + point.y**2)
-    ... 
-    >>> ak.behavior[np.absolute, "point"] = point_abs
-    >>> ak.to_list(abs(one))
-    [[1.4866068747318506, 2.973213749463701, 4.459820624195552],
-     [],
-     [5.946427498927402, 7.433034373659253],
-     [8.919641248391104],
-     [10.406248123122953, 11.892854997854805, 13.379461872586655]]
+```python
+def point_equal(left, right):
+    return np.logical_and(left.x == right.x, left.y == right.y)
+
+ak.behavior[np.equal, "point", "point"] = point_equal
+```
+
+The above should be read as "override :data\`np.equal\` for cases in which both
+arguments are `"point"`."
+
+```python
+>>> ak.to_list(one == two)
+[[False, True, False], [], [False, True], [False], [False, True, False]]
+```
+
+Similarly for overriding {func}`abs`
+
+```python
+>>> def point_abs(point):
+...     return np.sqrt(point.x**2 + point.y**2)
+...
+>>> ak.behavior[np.absolute, "point"] = point_abs
+>>> ak.to_list(abs(one))
+[[1.4866068747318506, 2.973213749463701, 4.459820624195552],
+ [],
+ [5.946427498927402, 7.433034373659253],
+ [8.919641248391104],
+ [10.406248123122953, 11.892854997854805, 13.379461872586655]]
+```
 
 and all other ufuncs.
 
-If you need a placeholder for "any number," use :class:`numbers.Real`,
-:class:`numbers.Integral`, etc. Non-arrays are resolved by type; builtin Python
+If you need a placeholder for "any number," use {class}`numbers.Real`,
+{class}`numbers.Integral`, etc. Non-arrays are resolved by type; builtin Python
 numbers and NumPy numbers are subclasses of the generic number types in the
-:mod:`numbers` library.
+{mod}`numbers` library.
 
 Also, for commutative operations, be sure to override both operator orders.
-(Function signatures are matched to :data:`ak.behavior` using multiple dispatch.)
+(Function signatures are matched to {data}`ak.behavior` using multiple dispatch.)
 
-.. code-block:: python
-
-    >>> import numbers
-    >>> def point_lmult(point, scalar):
-    ...     return ak.Array({"x": point.x * scalar, "y": point.y * scalar})
-    ... 
-    >>> def point_rmult(scalar, point):
-    ...     return point_lmult(point, scalar)
-    ... 
-    >>> ak.behavior[np.multiply, "point", numbers.Real] = point_lmult
-    >>> ak.behavior[np.multiply, numbers.Real, "point"] = point_rmult
-    >>> ak.to_list(one * 10)
-    [[{'x': 10, 'y': 11.0}, {'x': 20, 'y': 22.0}, {'x': 30, 'y': 33.0}],
-     [],
-     [{'x': 40, 'y': 44.0}, {'x': 50, 'y': 55.0}],
-     [{'x': 60, 'y': 66.0}],
-     [{'x': 70, 'y': 77.0}, {'x': 80, 'y': 88.0}, {'x': 90, 'y': 99.0}]]
+```python
+>>> import numbers
+>>> def point_lmult(point, scalar):
+...     return ak.Array({"x": point.x * scalar, "y": point.y * scalar})
+...
+>>> def point_rmult(scalar, point):
+...     return point_lmult(point, scalar)
+...
+>>> ak.behavior[np.multiply, "point", numbers.Real] = point_lmult
+>>> ak.behavior[np.multiply, numbers.Real, "point"] = point_rmult
+>>> ak.to_list(one * 10)
+[[{'x': 10, 'y': 11.0}, {'x': 20, 'y': 22.0}, {'x': 30, 'y': 33.0}],
+ [],
+ [{'x': 40, 'y': 44.0}, {'x': 50, 'y': 55.0}],
+ [{'x': 60, 'y': 66.0}],
+ [{'x': 70, 'y': 77.0}, {'x': 80, 'y': 88.0}, {'x': 90, 'y': 99.0}]]
+```
 
 If you need to override ufuncs in more generality, you can use the
-:class:`numpy.ufunc` interface:
-
-.. code-block:: python
+{class}`numpy.ufunc` interface:
 
-    >>> def apply_ufunc(ufunc, method, args, kwargs):
-    ...     if ufunc in (np.sin, np.cos, np.tan):
-    ...         x = ufunc(args[0].x)
-    ...         y = ufunc(args[0].y)
-    ...         return ak.Array({"x": x, "y": y})
-    ...     else:
-    ...         return NotImplemented
-    ... 
-    >>> ak.behavior[np.ufunc, "point"] = apply_ufunc
-    >>> ak.to_list(np.sin(one))
-    [[{'x': 0.8414709848078965, 'y': 0.8912073600614354},
-      {'x': 0.9092974268256817, 'y': 0.8084964038195901},
-      {'x': 0.1411200080598672, 'y': -0.1577456941432482}],
-     [],
-     [{'x': -0.7568024953079282, 'y': -0.951602073889516},
-      {'x': -0.9589242746631385, 'y': -0.7055403255703919}],
-     [{'x': -0.27941549819892586, 'y': 0.31154136351337786}],
-     [{'x': 0.6569865987187891, 'y': 0.9881682338770004},
-      {'x': 0.9893582466233818, 'y': 0.5849171928917617},
-      {'x': 0.4121184852417566, 'y': -0.45753589377532133}]]
-    >>> np.sqrt(one)
-    Traceback (most recent call last):
-      File "<stdin>", line 1, in <module>
-    ...
-    ValueError: no overloads for custom types: sqrt(point)
+```python
+>>> def apply_ufunc(ufunc, method, args, kwargs):
+...     if ufunc in (np.sin, np.cos, np.tan):
+...         x = ufunc(args[0].x)
+...         y = ufunc(args[0].y)
+...         return ak.Array({"x": x, "y": y})
+...     else:
+...         return NotImplemented
+...
+>>> ak.behavior[np.ufunc, "point"] = apply_ufunc
+>>> ak.to_list(np.sin(one))
+[[{'x': 0.8414709848078965, 'y': 0.8912073600614354},
+  {'x': 0.9092974268256817, 'y': 0.8084964038195901},
+  {'x': 0.1411200080598672, 'y': -0.1577456941432482}],
+ [],
+ [{'x': -0.7568024953079282, 'y': -0.951602073889516},
+  {'x': -0.9589242746631385, 'y': -0.7055403255703919}],
+ [{'x': -0.27941549819892586, 'y': 0.31154136351337786}],
+ [{'x': 0.6569865987187891, 'y': 0.9881682338770004},
+  {'x': 0.9893582466233818, 'y': 0.5849171928917617},
+  {'x': 0.4121184852417566, 'y': -0.45753589377532133}]]
+>>> np.sqrt(one)
+Traceback (most recent call last):
+  File "<stdin>", line 1, in <module>
+...
+ValueError: no overloads for custom types: sqrt(point)
+```
 
-But be forewarned: the ``ak.behavior[np.ufunc, name]`` syntax will match
-*any* ufunc that has an array containing an array with type ``name``
+But be forewarned: the `ak.behavior[np.ufunc, name]` syntax will match
+*any* ufunc that has an array containing an array with type `name`
 *anywhere* in the argument list. The first array in the argument list
-with type ``name`` will be matched instead of more detailed argument lists
-with type ``name`` at a later spot in the list. The "apply_ufunc" interface
+with type `name` will be matched instead of more detailed argument lists
+with type `name` at a later spot in the list. The "apply_ufunc" interface
 is *greedy*.
 
-Mixin decorators
-================
+## Overriding NumPy reducers
+
+In addition to ufuncs, it is also possible to override _reducers_ on records. Consider a 2D vector that implements binary addition:
+
+```python
+def vector_add(left, right):
+    return ak.contents.RecordArray(
+        [
+            ak.to_layout(left["rho"] + right["rho"]),
+            ak.to_layout(left["phi"] + right["phi"]),
+        ],
+        ["rho", "phi"],
+        parameters={"__record__": "Vector2D"},
+    )
+
+
+ak.behavior[np.add, "Vector2D", "Vector2D"] = vector_add
+```
+
+Whilst the `np.add` overload permits binary addition of `Vector2D` objects,
+
+```pycon 
+>>> vector = ak.Array(
+...     [[{"rho": -1.1, "phi": -0.1}, {"rho": 1.1, "phi": 0.1}], [{"rho": -2.2, "phi": 0.0}, {"rho": 3.1, "phi": 0.9}]],
+...     with_name="Vector2D",
+... )
+>>> (vector + vector).show()
+[[{rho: -2.2, phi: -0.2}, {rho: 2.2, phi: 0.2}],
+ [{rho: -4.4, phi: 0}, {rho: 6.2, phi: 1.8}]]
+```
+
+it does not permit the use of the `ak.sum` reducer:
+
+```pycon
+>>> ak.sum(vector, axis=-1)
+TypeError: no ak.sum overloads for custom types: rho, phi
+
+This error occurred while calling
+
+    ak.sum(
+        array = <Array [[{rho: -1.1, ...}, ...], ...] type='2 * var * Vecto...'>
+        axis = -1
+        keepdims = False
+        mask_identity = False
+        highlevel = True
+        behavior = None
+    )
+```
+
+To implement support for reducers like `ak.sum`, we should override them with a behavior:
+
+```pycon 
+>>> def vector_sum(vector, mask_identity):
+...     return ak.contents.RecordArray(
+...         [
+...             ak.sum(vector["rho"], highlevel=False, axis=-1),
+...             ak.sum(vector["phi"], highlevel=False, axis=-1),
+...         ],
+...         ["rho", "phi"],
+...         parameters={"__record__": "Vector2D"},
+...     )
+>>> ak.behavior[ak.sum, "Vector2D"] = vector_sum
+>>> ak.sum(vector, axis=-1).show()
+[{rho: 0, phi: 0},
+{rho: 0.9, phi: 0.9}]
+```
+
+Custom reducers are invoked with two arguments: a 2D array containing lists of records, and a boolean `mask_identity` indicating whether the reducer should introduce an option type (for reductions along empty sublists). If the reducer does not introduce an option type, and `mask=True`, Awkward will mask the result at the appropriate positions. The reducer should return an {class}`ak.Array` or {class}`ak.contents.Content` with the same number of elements as the input array. The reduction itself should be performed along `axis=1`, dropping the reduced dimension (i.e. `keepdims=False`). 
+
+
+## Mixin decorators
+
 The pattern of adding additional properties and function overrides to records
 and arrays of records is quite common, and can be nicely described by the "mixin"
-idiom: a class with no constructor that is mixed with both the :class:`ak.Array` and :class:`ak.Record`
-class as to create new derived classes. The :func:`ak.mixin_class` and :func:`ak.mixin_class_method`
-python decorators assist with some of this boilerplate. Consider the ``Point`` class
+idiom: a class with no constructor that is mixed with both the {class}`ak.Array` and {class}`ak.Record`
+class as to create new derived classes. The {func}`ak.mixin_class` and {func}`ak.mixin_class_method`
+python decorators assist with some of this boilerplate. Consider the `Point` class
 from above; we can implement all the functionality so far described as follows:
 
-.. code-block:: python
-
-    @ak.mixin_class(ak.behavior)
-    class Point:
-        def distance(self, other):
-            return np.sqrt((self.x - other.x) ** 2 + (self.y - other.y) ** 2)
-
-        @ak.mixin_class_method(np.equal, {"Point"})
-        def point_equal(self, other):
-            return np.logical_and(self.x == other.x, self.y == other.y)
-
-        @ak.mixin_class_method(np.abs)
-        def point_abs(self):
-            return np.sqrt(self.x ** 2 + self.y ** 2)
-
-The behavior name is taken as the mixin class name, e.g. here it is ``Point`` (as opposed
-to lowercase ``point`` previously). We can extend our implementation to allow ``Point`` types
-to be added by overriding the ``np.add`` ufunc (appending to our class definition):
-
-.. code-block:: python
-
-    class Point:
-        # ...
-
-        @ak.mixin_class_method(np.add, {"Point"})
-        def point_add(self, other):
-            return ak.zip(
-                {"x": self.x + other.x, "y": self.y + other.y}, with_name="Point",
-            )
+```python
+@ak.mixin_class(ak.behavior)
+class Point:
+    def distance(self, other):
+        return np.sqrt((self.x - other.x) ** 2 + (self.y - other.y) ** 2)
+
+    @ak.mixin_class_method(np.equal, {"Point"})
+    def point_equal(self, other):
+        return np.logical_and(self.x == other.x, self.y == other.y)
+
+    @ak.mixin_class_method(np.abs)
+    def point_abs(self):
+        return np.sqrt(self.x ** 2 + self.y ** 2)
+```
+
+The behavior name is taken as the mixin class name, e.g. here it is `Point` (as opposed
+to lowercase `point` previously). We can extend our implementation to allow `Point` types
+to be added by overriding the `np.add` ufunc (appending to our class definition):
+
+```python
+class Point:
+    # ...
+
+    @ak.mixin_class_method(np.add, {"Point"})
+    def point_add(self, other):
+        return ak.zip(
+            {"x": self.x + other.x, "y": self.y + other.y}, with_name="Point",
+        )
+```
 
 The real power of using mixin classes comes from the ability to inherit behaviors.
-Consider a ``Point``-like record that also has a ``weight`` field. Suppose that we want
-these ``WeightedPoint`` types to have the same distance and magnitude functionality, but
+Consider a `Point`-like record that also has a `weight` field. Suppose that we want
+these `WeightedPoint` types to have the same distance and magnitude functionality, but
 only be considered equal when they have the same weight. Also, suppose we want the addition
 of two weighted points to give their weighted mean rather than a sum. We could implement
 such a class as follows:
 
-.. code-block:: python
-
-    @ak.mixin_class(ak.behavior)
-    class WeightedPoint(Point):
-        @ak.mixin_class_method(np.equal, {"WeightedPoint"})
-        def weighted_equal(self, other):
-            return np.logical_and(self.point_equal(other), self.weight == other.weight)
-
-        @ak.mixin_class_method(np.add, {"WeightedPoint"})
-        def weighted_add(self, other):
-            sumw = self.weight + other.weight
-            return ak.zip(
-                {
-                    "x": (self.x * self.weight + other.x * other.weight) / sumw,
-                    "y": (self.y * self.weight + other.y * other.weight) / sumw,
-                    "weight": sumw,
-                },
-                with_name="WeightedPoint",
-            )
+```python
+@ak.mixin_class(ak.behavior)
+class WeightedPoint(Point):
+    @ak.mixin_class_method(np.equal, {"WeightedPoint"})
+    def weighted_equal(self, other):
+        return np.logical_and(self.point_equal(other), self.weight == other.weight)
+
+    @ak.mixin_class_method(np.add, {"WeightedPoint"})
+    def weighted_add(self, other):
+        sumw = self.weight + other.weight
+        return ak.zip(
+            {
+                "x": (self.x * self.weight + other.x * other.weight) / sumw,
+                "y": (self.y * self.weight + other.y * other.weight) / sumw,
+                "weight": sumw,
+            },
+            with_name="WeightedPoint",
+        )
+```
 
 A footnote: in this implementation, adding a WeightedPoint and a Point returns a Point.
 One may wish to disable this by type-checking, since the functionalities are rather different.
 
-Adding behavior to arrays
-=========================
+## Adding behavior to arrays
 
 Occasionally, you may want to add behavior to an array that does not contain
 records. A good example of this is to implement strings: strings are not a
 special data type in Awkward Array as they are in many other libraries, they
 are a behavior overlaid on arrays.
 
 There are four predefined string behaviors:
 
-* :class:`ak.CharBehavior`: an array of UTF-8 encoded characters;
-* :class:`ak.ByteBehavior`: an array of unencoded characters;
-* :class:`ak.StringBehavior`: an array of variable-length UTF-8 encoded strings;
-* :class:`ak.ByteStringBehavior`: an array of variable-length unencoded bytestrings.
+- {class}`ak.CharBehavior`: an array of UTF-8 encoded characters;
+- {class}`ak.ByteBehavior`: an array of unencoded characters;
+- {class}`ak.StringBehavior`: an array of variable-length UTF-8 encoded strings;
+- {class}`ak.ByteStringBehavior`: an array of variable-length unencoded bytestrings.
 
-All four override the string representations (``__str__`` and ``__repr__``),
+All four override the string representations (`__str__` and `__repr__`),
 but the string behaviors additionally override equality:
 
-.. code-block:: python
-
-    >>> ak.Array(["one", "two", "three"]) == ak.Array(["1", "TWO", "three"])
-    <Array [False, False, True] type='3 * bool'>
-
-The only difference here is the parameter: instead of setting ``"__record__"``,
-we set ``"__array__"``.
-
-.. code-block:: python
-
-    >>> ak.Array(["one", "two", "three"]).layout
-    <ListOffsetArray64>
+```python
+>>> ak.Array(["one", "two", "three"]) == ak.Array(["1", "TWO", "three"])
+<Array [False, False, True] type='3 * bool'>
+```
+
+The only difference here is the parameter: instead of setting `"__record__"`,
+we set `"__array__"`.
+
+```python
+>>> ak.Array(["one", "two", "three"]).layout
+<ListOffsetArray64>
+    <parameters>
+        <param key="__array__">"string"</param>
+    </parameters>
+    <offsets><Index64 i="[0 3 6 11]" offset="0" length="4""/></offsets>
+    <content><NumpyArray format="B" shape="11" data="0x 6f6e6574 776f7468 726565">
         <parameters>
-            <param key="__array__">"string"</param>
+            <param key="__array__">"char"</param>
         </parameters>
-        <offsets><Index64 i="[0 3 6 11]" offset="0" length="4""/></offsets>
-        <content><NumpyArray format="B" shape="11" data="0x 6f6e6574 776f7468 726565">
-            <parameters>
-                <param key="__array__">"char"</param>
-            </parameters>
-        </NumpyArray></content>
-    </ListOffsetArray64>
+    </NumpyArray></content>
+</ListOffsetArray64>
+```
 
-In ``ak.behaviors.string``, string behaviors are assigned with lines like
+In `ak.behaviors.string`, string behaviors are assigned with lines like
 
-.. code-block:: python
+```python
+ak.behavior["string"] = StringBehavior
+ak.behavior[np.equal, "string", "string"] = _string_equal
+```
 
-    ak.behavior["string"] = StringBehavior
-    ak.behavior[np.equal, "string", "string"] = _string_equal
+## Custom type names
 
-Custom type names
-=================
+To make the string type appear as `string` in type representations, a
+`"__typestr__"` behavior is overriden (in `ak.behaviors.string`):
 
-To make the string type appear as ``string`` in type representations, a
-``"__typestr__"`` behavior is overriden (in ``ak.behaviors.string``):
-
-.. code-block:: python
-
-    ak.behavior["__typestr__", "string"] = "string"
+```python
+ak.behavior["__typestr__", "string"] = "string"
+```
 
 so that
 
-.. code-block:: python
-
-    >>> ak.type(ak.Array(["one", "two", "three"]))
-    3 * string
+```python
+>>> ak.type(ak.Array(["one", "two", "three"]))
+3 * string
+```
 
-Custom broadcasting
-===================
+## Custom broadcasting
 
 In situations where we want to think about lists as objects, such as strings,
 we may even need to override the broadcasting rules. For instance, given
 
-.. code-block:: python
-
-    ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]])
-
-we might expect ``"HAL"`` to broadcast to each ``1``, like
-
-.. code-block:: python
-
-    [[[73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77]]]
+```python
+ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]])
+```
+
+we might expect `"HAL"` to broadcast to each `1`, like
+
+```python
+[[[73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77]]]
+```
 
 but (without custom broadcasting) instead it raises a broadcasting for any
-length of ``1`` list other than 3:
-
-.. code-block:: python
+length of `1` list other than 3:
 
-    >>> # without custom broadcasting
-    >>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]]))
-    ValueError: in ListOffsetArray64, cannot broadcast nested list
-    >>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1]]))
-    [[73, 66, 77]]
+```python
+>>> # without custom broadcasting
+>>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]]))
+ValueError: in ListOffsetArray64, cannot broadcast nested list
+>>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1]]))
+[[73, 66, 77]]
+```
 
-It's matching each character of ``"HAL"`` with a number from the list, but we
+It's matching each character of `"HAL"` with a number from the list, but we
 want the string to be taken as an object. That is fixed (in
-``ak.behaviors.string``) with a custom broadcasting rule:
+`ak.behaviors.string`) with a custom broadcasting rule:
 
-.. code-block:: python
-
-    def _string_broadcast(layout, offsets):
-        # layout:  an ak.layout.Content object
-        # offsets: an ak.layout.Index of offsets to match
-        # 
-        # should return: an ak.layout.Content object of the broadcasted result
-        ...
+```python
+def _string_broadcast(layout, offsets):
+    # layout:  an ak.layout.Content object
+    # offsets: an ak.layout.Index of offsets to match
+    #
+    # should return: an ak.layout.Content object of the broadcasted result
+    ...
 
-    awkward.behavior["__broadcast__", "string"] = _string_broadcast
+awkward.behavior["__broadcast__", "string"] = _string_broadcast
+```
 
-Very few applications would need to do this, but the :data:`ak.behavior` object
+Very few applications would need to do this, but the {data}`ak.behavior` object
 provides a lot of room for customization hooks like this.
 
-Overriding behavior in Numba
-============================
+## Overriding behavior in Numba
 
 Awkward Arrays can be arguments and return values of functions compiled with
-`Numba <http://numba.pydata.org>`__. Since these functions run on low-level
+[Numba](http://numba.pydata.org). Since these functions run on low-level
 objects, most functionality must be reimplemented, including behavioral
 overrides.
 
 The documentation on
-`Extending Numba <https://numba.pydata.org/numba-doc/dev/extending/index.html>`__
+[Extending Numba](https://numba.pydata.org/numba-doc/dev/extending/index.html)
 introduces **typing**, **lowering**, and **models**, which are necessary for
 reimplementing the behavior of a Python object in the compiled environment.
 To apply the same to records and arrays from an Awkward data structure, we
-use :data:`ak.behavior` hooks that start with ``"__numba_typer__"`` and
-``"__numba_lower__"``.
+use {data}`ak.behavior` hooks that start with `"__numba_typer__"` and
+`"__numba_lower__"`.
 
-**Case 1:** Adding a property, such as ``rec.property_name``.
+**Case 1:** Adding a property, such as `rec.property_name`.
 
-.. code-block:: python
+```python
+ak.behavior["__numba_typer__", record_name, property_name] = typer
+ak.behavior["__numba_lower__", record_name, property_name] = lower
+```
 
-    ak.behavior["__numba_typer__", record_name, property_name] = typer
-    ak.behavior["__numba_lower__", record_name, property_name] = lower
-
-The ``typer`` function takes an
-:func:`ak._connect._numba.arrayview.ArrayViewType` as its only argument
+The `typer` function takes an
+{func}`ak._connect._numba.arrayview.ArrayViewType` as its only argument
 and returns the property's type.
 
-The ``lower`` function takes the standard ``context, builder, sig, args``
-arguments and returns the lowered value. Given a Python ``function`` that
-takes one record and returns the property, the ``lower`` can be
-
-.. code-block:: python
-
-    def lower(context, builder, sig, args):
-        return context.compile_internal(builder, function, sig, args)
-
-**Case 2:** Adding a method, such as ``rec.method_name(arg0, arg1)``.
-
-.. code-block:: python
+The `lower` function takes the standard `context, builder, sig, args`
+arguments and returns the lowered value. Given a Python `function` that
+takes one record and returns the property, the `lower` can be
+
+```python
+def lower(context, builder, sig, args):
+    return context.compile_internal(builder, function, sig, args)
+```
+
+**Case 2:** Adding a method, such as `rec.method_name(arg0, arg1)`.
+
+```python
+ak.behavior["__numba_typer__", record_name, method_name, ()] = typer
+ak.behavior["__numba_lower__", record_name, method_name, ()] = lower
+```
 
-    ak.behavior["__numba_typer__", record_name, method_name, ()] = typer
-    ak.behavior["__numba_lower__", record_name, method_name, ()] = lower
-
-The last item is an *empty* tuple, ``()`` (regardless of whether the method
+The last item is an *empty* tuple, `()` (regardless of whether the method
 takes any arguments).
 
-In this case, the ``typer`` takes an
-:func:`ak._connect._numba.arrayview.ArrayViewType` as well as any arguments
-and returns the property's type, and the ``sig`` and ``args`` in ``lower``
+In this case, the `typer` takes an
+{func}`ak._connect._numba.arrayview.ArrayViewType` as well as any arguments
+and returns the property's type, and the `sig` and `args` in `lower`
 include these arguments.
 
-**Case 3:** Unary and binary operations, like ``-rec1`` and ``rec1 + rec2``.
-
-.. code-block:: python
-
-    ak.behavior["__numba_typer__", operator.neg, "rec1"] = typer
-    ak.behavior["__numba_lower__", operator.neg, "rec1"] = lower
+**Case 3:** Unary and binary operations, like `-rec1` and `rec1 + rec2`.
 
-    ak.behavior["__numba_typer__", "rec1", operator.add, "rec2"] = typer
-    ak.behavior["__numba_lower__", "rec1", operator.add, "rec2"] = lower
+```python
+ak.behavior["__numba_typer__", operator.neg, "rec1"] = typer
+ak.behavior["__numba_lower__", operator.neg, "rec1"] = lower
+
+ak.behavior["__numba_typer__", "rec1", operator.add, "rec2"] = typer
+ak.behavior["__numba_lower__", "rec1", operator.add, "rec2"] = lower
+```
 
 **Case 4:** Completely replacing the Awkward record with an object in Numba.
 
 If a fully defined model for the object already exists and Numba, we can
 have references to Awkward records or arrays simply *become* these objects,
 which implies some overhead from copying data and a loss of the functionality
 that Awkward would bring.
 
 Strings, for instance, are replaced by Numba's built-in string model so that
 all string operations will work, but Awkward operations like broadcasting
 characters will not.
 
 For this case, the signatures are
 
-.. code-block:: python
-
-    # parameters["__record__"] = record_name
-    ak.behavior["__numba_typer__", record_name] = typer
-    ak.behavior["__numba_lower__", record_name] = lower
-
-    # for an array one-level deep
-    ak.behavior["__numba_typer__", ".", record_name] = typer
-    ak.behavior["__numba_lower__", ".", record_name] = lower
-
-    # for an array any number of levels deep
-    ak.behavior["__numba_typer__", "*", record_name] = typer
-    ak.behavior["__numba_lower__", "*", record_name] = lower
-
-    # parameters["__array__"] = array_name
-    ak.behavior["__numba_typer__", array_name] = typer
-    ak.behavior["__numba_lower__", array_name] = lower
-
-The ``typer`` function takes an
-:func:`ak._connect._numba.arrayview.ArrayViewType` as its only argument
-and returns the Numba type of its replacement, while the ``lower``
+```python
+# parameters["__record__"] = record_name
+ak.behavior["__numba_typer__", record_name] = typer
+ak.behavior["__numba_lower__", record_name] = lower
+
+# for an array one-level deep
+ak.behavior["__numba_typer__", ".", record_name] = typer
+ak.behavior["__numba_lower__", ".", record_name] = lower
+
+# for an array any number of levels deep
+ak.behavior["__numba_typer__", "*", record_name] = typer
+ak.behavior["__numba_lower__", "*", record_name] = lower
+
+# parameters["__array__"] = array_name
+ak.behavior["__numba_typer__", array_name] = typer
+ak.behavior["__numba_lower__", array_name] = lower
+```
+
+The `typer` function takes an
+{func}`ak._connect._numba.arrayview.ArrayViewType` as its only argument
+and returns the Numba type of its replacement, while the `lower`
 function takes
 
-* ``context``: Numba context
-* ``builder``: Numba builder
-* ``rettype``: the Numba type of its replacement
-* ``viewtype``: an :func:`ak._connect._numba.arrayview.ArrayViewType`
-* ``viewval``: a Numba value of the view
-* ``viewproxy``: a Numba proxy (``context.make_helper``) of the view
-* ``attype``: the Numba integer type of the index position
-* ``atval``: the Numba value of the index position
-
-.. Add back once https://github.com/scikit-hep/vector/issues/273 is completed
-.. Complete example
-.. ================
-
-.. The
-.. `Vector design prototype <https://vector.readthedocs.io/en/latest/usage/vector_design_prototype.html>`__
-.. has a complete example, including Numba.
+- `context`: Numba context
+- `builder`: Numba builder
+- `rettype`: the Numba type of its replacement
+- `viewtype`: an {func}`ak._connect._numba.arrayview.ArrayViewType`
+- `viewval`: a Numba value of the view
+- `viewproxy`: a Numba proxy (`context.make_helper`) of the view
+- `attype`: the Numba integer type of the index position
+- `atval`: the Numba value of the index position
+
+% Add back once https://github.com/scikit-hep/vector/issues/273 is completed
+
+% Complete example
+
+% ================
+
+% The
+
+% `Vector design prototype <https://vector.readthedocs.io/en/latest/usage/vector_design_prototype.html>`__
+
+% has a complete example, including Numba.
```

### Comparing `awkward-2.2.0/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.2.1/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/reference/awkwardforth.rst` & `awkward-2.2.1/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/reference/toctree.txt` & `awkward-2.2.1/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.2.1/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.2.1/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.2.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-json.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-python.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.2.1/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.2.1/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-constructors.md` & `awkward-2.2.1/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-lists.md` & `awkward-2.2.1/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-missing.md` & `awkward-2.2.1/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-records.md` & `awkward-2.2.1/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-strings.md` & `awkward-2.2.1/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.2.1/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.2.1/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.2.1/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.2.1/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.2.1/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-examine-type.md` & `awkward-2.2.1/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.2.1/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-filter-masked.md` & `awkward-2.2.1/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-filter-num.md` & `awkward-2.2.1/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.2.1/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.2.1/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.2.1/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-gpu.md` & `awkward-2.2.1/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-numpy.md` & `awkward-2.2.1/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-reducing.md` & `awkward-2.2.1/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-math-statistics.md` & `awkward-2.2.1/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.2.1/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.2.1/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.2.1/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.2.1/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.2.1/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.2.1/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.2.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-data-analysts.png` & `awkward-2.2.1/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-data-analysts.svg` & `awkward-2.2.1/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-developers.png` & `awkward-2.2.1/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-developers.svg` & `awkward-2.2.1/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-doxygen.png` & `awkward-2.2.1/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-sphinx.png` & `awkward-2.2.1/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-tutorials-alternate.png` & `awkward-2.2.1/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/panel-tutorials.png` & `awkward-2.2.1/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.2.1/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-timeline.png` & `awkward-2.2.1/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.2.1/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.2.1/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.2.1/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.2.1/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.2.1/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-array.svg` & `awkward-2.2.1/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-hierarchy.png` & `awkward-2.2.1/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.2.1/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.2.1/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.2.1/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-reduction.png` & `awkward-2.2.1/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/example-reduction.svg` & `awkward-2.2.1/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/git-strategy.pdf` & `awkward-2.2.1/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/git-strategy.png` & `awkward-2.2.1/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/git-strategy.svg` & `awkward-2.2.1/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.2.1/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.2.1/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/how-it-works.svg` & `awkward-2.2.1/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/sorting-axis.svg` & `awkward-2.2.1/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/all.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/any.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/count.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/max.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/min.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/product.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/diagrams/reducers/sum.svg` & `awkward-2.2.1/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/logo/favicon.ico` & `awkward-2.2.1/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/logo/logo-300px-white.png` & `awkward-2.2.1/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/logo/logo-300px.png` & `awkward-2.2.1/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/logo/logo-600px.png` & `awkward-2.2.1/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/logo/logo.svg` & `awkward-2.2.1/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/photos/desire-path.jpg` & `awkward-2.2.1/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.2.1/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/plots/awkward-0-popularity.png` & `awkward-2.2.1/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.2.1/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.2.1/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.2.1/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/__init__.py` & `awkward-2.2.1/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_behavior.py` & `awkward-2.2.1/src/awkward/_behavior.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from collections import ChainMap
 from collections.abc import Mapping
 
 import awkward as ak
 from awkward._nplikes import ufuncs
+from awkward._typing import Any
 
 
 def overlay_behavior(behavior: dict | None) -> Mapping:
     """
     Args:
         behavior: behavior dictionary, or None
 
@@ -55,108 +56,90 @@
     rec = layout.parameter("__record__")
     if isinstance(rec, str):
         return behavior.get((reducer.highlevel_function(), rec))
 
 
 def find_custom_cast(obj, behavior):
     behavior = overlay_behavior(behavior)
-    for key, fcn in behavior.items():
-        if (
-            isinstance(key, tuple)
-            and len(key) == 2
-            and key[0] == "__cast__"
-            and isinstance(obj, key[1])
-        ):
+    for cls in type(obj).__mro__:
+        fcn = behavior.get(("__cast__", cls))
+        if fcn is not None:
             return fcn
     return None
 
 
 def find_custom_broadcast(layout, behavior):
     behavior = overlay_behavior(behavior)
     custom = layout.parameter("__array__")
-    if not isinstance(custom, str):
+    if custom is None:
         custom = layout.parameter("__record__")
-    if not isinstance(custom, str):
+    if custom is None:
         custom = layout.purelist_parameter("__record__")
     if isinstance(custom, str):
-        for key, fcn in behavior.items():
-            if (
-                isinstance(key, tuple)
-                and len(key) == 2
-                and key[0] == "__broadcast__"
-                and key[1] == custom
-            ):
-                return fcn
-    return None
+        return behavior.get(("__broadcast__", custom))
+    else:
+        return None
 
 
 def find_ufunc_generic(ufunc, layout, behavior):
     behavior = overlay_behavior(behavior)
     custom = layout.parameter("__array__")
-    if not isinstance(custom, str):
+    if custom is None:
         custom = layout.parameter("__record__")
     if isinstance(custom, str):
-        for key, fcn in behavior.items():
-            if (
-                isinstance(key, tuple)
-                and len(key) == 2
-                and (key[0] is ufunc or key[0] is ufuncs.ufunc)
-                and key[1] == custom
-            ):
-                return fcn
-    return None
+        fcn = behavior.get((ufunc, custom))
+        if fcn is None:
+            fcn = behavior.get((ufuncs.ufunc, custom))
+        return fcn
+    else:
+        return None
 
 
-def find_ufunc(behavior, signature):
+def find_ufunc(behavior, signature: tuple):
     if not any(s is None for s in signature):
         behavior = overlay_behavior(behavior)
-        for key, custom in behavior.items():
-            if (
-                isinstance(key, tuple)
-                and len(key) == len(signature)
-                and key[0] == signature[0]
-                and all(
-                    k == s
-                    or (
-                        isinstance(k, type) and isinstance(s, type) and issubclass(s, k)
+
+        # Special case all strings or hashable types.
+        if all(isinstance(x, str) for x in signature):
+            return behavior.get(signature)
+        else:
+            for key, custom in behavior.items():
+                if (
+                    isinstance(key, tuple)
+                    and len(key) == len(signature)
+                    and key[0] == signature[0]
+                    and all(
+                        k == s
+                        or (
+                            isinstance(k, type)
+                            and isinstance(s, type)
+                            and issubclass(s, k)
+                        )
+                        for k, s in zip(key[1:], signature[1:])
                     )
-                    for k, s in zip(key[1:], signature[1:])
-                )
-            ):
-                return custom
-
-
-def find_typestrs(behavior):
-    behavior = overlay_behavior(behavior)
-    out = {}
-    for key, typestr in behavior.items():
-        if (
-            isinstance(key, tuple)
-            and len(key) == 2
-            and key[0] == "__typestr__"
-            and isinstance(key[1], str)
-            and isinstance(typestr, str)
-        ):
-            out[key[1]] = typestr
-    return out
-
-
-def find_typestr(parameters, typestrs):
-    if parameters is not None:
-        record = parameters.get("__record__")
-        if record is not None:
-            typestr = typestrs.get(record)
-            if typestr is not None:
-                return typestr
-        array = parameters.get("__array__")
-        if array is not None:
-            typestr = typestrs.get(array)
-            if typestr is not None:
-                return typestr
-    return None
+                ):
+                    return custom
+
+
+def find_record_typestr(
+    behavior: None | Mapping, parameters: None | Mapping[str, Any], default: str = None
+):
+    if parameters is None:
+        return default
+    behavior = overlay_behavior(behavior)
+    return behavior.get(("__typestr__", parameters.get("__record__")), default)
+
+
+def find_array_typestr(
+    behavior: None | Mapping, parameters: None | Mapping[str, Any], default: str = None
+):
+    if parameters is None:
+        return default
+    behavior = overlay_behavior(behavior)
+    return behavior.get(("__typestr__", parameters.get("__array__")), default)
 
 
 def behavior_of(*arrays, **kwargs):
     from awkward.highlevel import Array, ArrayBuilder, Record
 
     behavior = kwargs.get("behavior")
     if behavior is not None:
```

### Comparing `awkward-2.2.0/src/awkward/_broadcasting.py` & `awkward-2.2.1/src/awkward/_broadcasting.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_are_empty,
     parameters_are_equal,
     parameters_intersect,
 )
 from awkward._typing import Any, Callable, Dict, List, TypeAlias, Union
-from awkward._util import unset
+from awkward._util import UNSET, Sentinel
 from awkward.contents.bitmaskedarray import BitMaskedArray
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.contents.emptyarray import EmptyArray
 from awkward.contents.indexedarray import IndexedArray
 from awkward.contents.indexedoptionarray import IndexedOptionArray
 from awkward.contents.listarray import ListArray
@@ -171,29 +171,14 @@
 
         elif isinstance(x, Content):
             return False
 
     return True
 
 
-# TODO: move to _util or another module
-class Sentinel:
-    """A class for implementing sentinel types"""
-
-    def __init__(self, name, module=None):
-        self._name = name
-        self._module = module
-
-    def __repr__(self):
-        if self._module is not None:
-            return f"{self._module}.{self._name}"
-        else:
-            return f"{self._name}"
-
-
 NO_PARAMETERS = Sentinel("NO_PARAMETERS", __name__)
 
 
 class BroadcastParameterRule(str, enum.Enum):
     """Behaviour for parameter coalescence during broadcasting."""
 
     INTERSECT = "intersect"
@@ -437,39 +422,39 @@
     parameters_factory = parameters_factory_impl(inputs)
 
     # This whole function is one big switch statement.
     def broadcast_any_record():
         if not options["allow_records"]:
             raise ValueError(f"cannot broadcast records {in_function(options)}")
 
-        fields, length, istuple = unset, unset, unset
+        fields, length, istuple = UNSET, UNSET, UNSET
         for x in contents:
             if x.is_record:
-                if fields is unset:
+                if fields is UNSET:
                     fields = x.fields
                 elif set(fields) != set(x.fields):
                     raise ValueError(
                         "cannot broadcast records because fields don't "
                         "match{}:\n    {}\n    {}".format(
                             in_function(options),
                             ", ".join(sorted(fields)),
                             ", ".join(sorted(x.fields)),
                         )
                     )
-                if length is unset:
+                if length is UNSET:
                     length = x.length
                 elif length != x.length:
                     raise ValueError(
                         "cannot broadcast RecordArray of length {} "
                         "with RecordArray of length {}{}".format(
                             length, x.length, in_function(options)
                         )
                     )
                 # Records win over tuples
-                if istuple is unset or not x.is_tuple:
+                if istuple is UNSET or not x.is_tuple:
                     istuple = False
 
         outcontents, numoutputs = [], None
         for field in fields:
             outcontents.append(
                 apply_step(
                     backend,
```

### Comparing `awkward-2.2.0/src/awkward/_do.py` & `awkward-2.2.1/src/awkward/_do.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,35 +200,38 @@
 def remove_structure(
     layout: Content | Record,
     backend: Backend | None = None,
     flatten_records: bool = True,
     function_name: str | None = None,
     drop_nones: bool = True,
     keepdims: bool = False,
+    allow_records: bool = False,
 ):
     if isinstance(layout, Record):
         return remove_structure(
             layout._array[layout._at : layout._at + 1],
             backend,
             flatten_records,
             function_name,
             drop_nones,
             keepdims,
+            allow_records,
         )
 
     else:
         if backend is None:
             backend = layout._backend
         arrays = layout._remove_structure(
             backend,
             {
                 "flatten_records": flatten_records,
                 "function_name": function_name,
                 "drop_nones": drop_nones,
                 "keepdims": keepdims,
+                "allow_records": allow_records,
             },
         )
         return tuple(arrays)
 
 
 def flatten(layout: Content, axis: int = 1) -> Content:
     offsets, flattened = layout._offsets_and_flattened(axis, 1)
@@ -262,27 +265,31 @@
     axis: AxisMaybeNone = -1,
     mask: bool = True,
     keepdims: bool = False,
     behavior: dict | None = None,
 ):
     if axis is None:
         parts = remove_structure(
-            layout, flatten_records=False, drop_nones=False, keepdims=keepdims
+            layout,
+            flatten_records=False,
+            drop_nones=False,
+            keepdims=keepdims,
+            allow_records=True,
         )
 
         if len(parts) > 1:
             # We know that `flatten_records` must fail, so the only other type
             # that can return multiple parts here is the union array
             raise ValueError(
                 "cannot use axis=None on an array containing irreducible unions"
             )
         elif len(parts) == 0:
-            parts = [ak.contents.EmptyArray()]
-
-        (layout,) = parts
+            layout = ak.contents.EmptyArray()
+        else:
+            (layout,) = parts
 
         starts = ak.index.Index64.zeros(1, layout.backend.index_nplike)
         parents = ak.index.Index64.zeros(layout.length, layout.backend.index_nplike)
         shifts = None
         next = layout._reduce_next(
             reducer,
             1,
```

### Comparing `awkward-2.2.0/src/awkward/_errors.py` & `awkward-2.2.1/src/awkward/_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_kernels.py` & `awkward-2.2.1/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_layout.py` & `awkward-2.2.1/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_lookup.py` & `awkward-2.2.1/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_parameters.py` & `awkward-2.2.1/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_prettyprint.py` & `awkward-2.2.1/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_reducers.py` & `awkward-2.2.1/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_regularize.py` & `awkward-2.2.1/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_slicing.py` & `awkward-2.2.1/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_typetracer.py` & `awkward-2.2.1/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_typing.py` & `awkward-2.2.1/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_util.py` & `awkward-2.2.1/src/awkward/_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
+import base64
 import os
+import struct
 import sys
 from collections.abc import Collection
 
 import packaging.version
 
-from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import TypeVar
 
-np = NumpyMetadata.instance()
-
 win = os.name == "nt"
-bits32 = np.iinfo(np.intp).bits == 32
+bits32 = struct.calcsize("P") * 8 == 32
 
 # matches include/awkward/common.h
 kMaxInt8 = 127  # 2**7  - 1
 kMaxUInt8 = 255  # 2**8  - 1
 kMaxInt32 = 2147483647  # 2**31 - 1
 kMaxUInt32 = 4294967295  # 2**32 - 1
 kMaxInt64 = 9223372036854775806  # 2**63 - 2: see below
@@ -64,38 +63,38 @@
     if byteorder != native_byteorder:
         return array.byteswap(inplace=False)
     else:
         return array
 
 
 def identifier_hash(str):
-    import base64
-    import struct
-
     return (
         base64.encodebytes(struct.pack("q", hash(str)))
         .rstrip(b"=\n")
         .replace(b"+", b"")
         .replace(b"/", b"")
         .decode("ascii")
     )
 
 
-# FIXME: introduce sentinel type for this
-class _Unset:
-    def __repr__(self):
-        return f"{__name__}.unset"
+class Sentinel:
+    """A class for implementing sentinel types"""
 
+    def __init__(self, name, module=None):
+        self._name = name
+        self._module = module
 
-unset = _Unset()
+    def __repr__(self):
+        if self._module is not None:
+            return f"{self._module}.{self._name}"
+        else:
+            return f"{self._name}"
 
 
-# Sentinel object for catching pass-through values
-class Unspecified:
-    pass
+UNSET = Sentinel("UNSET", __name__)
 
 
 T = TypeVar("T")
 
 
 def unique_list(items: Collection[T]) -> list[T]:
     seen = set()
```

### Comparing `awkward-2.2.0/src/awkward/_v2.py` & `awkward-2.2.1/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/cppyy.py` & `awkward-2.2.1/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/highlevel.py` & `awkward-2.2.1/src/awkward/highlevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,17 @@
         Note that the outermost element of an Array's type is always an
         #ak.types.ArrayType, which specifies the number of elements in the array.
 
         The type of a #ak.contents.Content (from #ak.Array.layout) is not
         wrapped by an #ak.types.ArrayType.
         """
         return ak.types.ArrayType(
-            self._layout.form.type_from_behavior(self._behavior), self._layout.length
+            self._layout.form.type,
+            self._layout.length,
+            self._behavior,
         )
 
     @property
     def typestr(self):
         """
         The high-level type of this Array, presented as a string.
         """
@@ -1347,15 +1349,15 @@
             >>> sqr(array).show()
             [[1.21, 4.84, 10.9],
              [],
              [19.4, 30.2]]
 
         See also #__array_function__.
         """
-        name = f"{type(ufunc).__module__}.{ufunc.__name__}.{str(method)}"
+        name = f"{type(ufunc).__module__}.{ufunc.__name__}.{method!s}"
         arguments = {}
         for i, arg in enumerate(inputs):
             arguments[i] = arg
         arguments.update(kwargs)
         with ak._errors.OperationErrorContext(name, arguments):
             return ak._connect.numpy.array_ufunc(ufunc, method, inputs, kwargs)
 
@@ -1709,17 +1711,15 @@
 
         Note that the outermost element of a Record's type is always an
         #ak.types.ScalarType, which .
 
         The type of a #ak.record.Record (from #ak.Array.layout) is not
         wrapped by an #ak.types.ScalarType.
         """
-        return ak.types.ScalarType(
-            self._layout.array.form.type_from_behavior(self._behavior)
-        )
+        return ak.types.ScalarType(self._layout.array.form.type, self._behavior)
 
     @property
     def typestr(self):
         """
         The high-level type of this Record, presented as a string.
         """
         return str(self.type)
@@ -2025,15 +2025,15 @@
         [NEP 13](https://numpy.org/neps/nep-0013-ufunc-overrides.html)
         for overriding ufuncs, which has been
         [available since NumPy 1.13](https://numpy.org/devdocs/release/1.13.0-notes.html#array-ufunc-added)
         (and thus NumPy 1.13 is the minimum allowed version).
 
         See #ak.Array.__array_ufunc__ for a more complete description.
         """
-        name = f"{type(ufunc).__module__}.{ufunc.__name__}.{str(method)}"
+        name = f"{type(ufunc).__module__}.{ufunc.__name__}.{method!s}"
         arguments = {}
         for i, arg in enumerate(inputs):
             arguments[i] = arg
         arguments.update(kwargs)
         with ak._errors.OperationErrorContext(name, arguments):
             return ak._connect.numpy.array_ufunc(ufunc, method, inputs, kwargs)
 
@@ -2314,17 +2314,15 @@
         Note that the outermost element of an Array's type is always an
         #ak.types.ArrayType, which specifies the number of elements in the array.
 
         The type of a #ak.contents.Content (from #ak.Array.layout) is not
         wrapped by an #ak.types.ArrayType.
         """
         form = ak.forms.from_json(self._layout.form())
-        return ak.types.ArrayType(
-            form.type_from_behavior(self._behavior), len(self._layout)
-        )
+        return ak.types.ArrayType(form.type, len(self._layout), self._behavior)
 
     @property
     def typestr(self):
         """
         The high-level type of this accumulated array, presented as a string.
         """
         return str(self.type)
```

### Comparing `awkward-2.2.0/src/awkward/index.py` & `awkward-2.2.1/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/jax.py` & `awkward-2.2.1/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/numba.py` & `awkward-2.2.1/src/awkward/numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/record.py` & `awkward-2.2.1/src/awkward/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 from awkward._behavior import get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
 from awkward._typing import Self
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 
 np = NumpyMetadata.instance()
 
 
 class Record:
     """
@@ -240,17 +240,17 @@
 
     def __copy__(self) -> Self:
         return self.copy()
 
     def __deepcopy__(self, memo):
         return Record(copy.deepcopy(self._array, memo), self._at)
 
-    def copy(self, array=unset, at=unset) -> Self:
+    def copy(self, array=UNSET, at=UNSET) -> Self:
         return Record(
-            self._array if array is unset else array, self._at if at is unset else at
+            self._array if array is UNSET else array, self._at if at is UNSET else at
         )
 
 
 @register_backend_lookup_factory
 def find_record_backend(obj: type):
     if issubclass(obj, Record):
```

### Comparing `awkward-2.2.0/src/awkward/_backends/backend.py` & `awkward-2.2.1/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_backends/cupy.py` & `awkward-2.2.1/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_backends/dispatch.py` & `awkward-2.2.1/src/awkward/_backends/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from collections.abc import Iterable
 
 from awkward._backends.backend import Backend
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._typing import Callable, TypeAlias, TypeVar
-from awkward._util import unset
+from awkward._util import UNSET
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 D = TypeVar("D")
 T = TypeVar("T")
 
@@ -65,34 +65,34 @@
 
         else:
             raise ValueError(
                 "no backends were given in order to determine a common backend."
             )
 
 
-def _backend_of(obj, default: D = unset) -> Backend | D:
+def _backend_of(obj, default: D = UNSET) -> Backend | D:
     cls = type(obj)
     try:
         lookup = _type_to_backend_lookup[cls]
         return lookup(obj)
     except KeyError:
         for factory in _backend_lookup_factories:
             maybe_lookup = factory(cls)
             if maybe_lookup is not None:
                 break
         else:
-            if default is unset:
+            if default is UNSET:
                 raise TypeError(f"cannot find nplike for {cls.__name__}")
             else:
                 return default
         _type_to_backend_lookup[cls] = maybe_lookup
         return maybe_lookup(obj)
 
 
-def backend_of(*objects, default: D = unset) -> Backend | D:
+def backend_of(*objects, default: D = UNSET) -> Backend | D:
     """
     Args:
         objects: objects for which to find a suitable backend
         default: value to return if no backend is found.
 
     Return the most suitable backend for the given objects (e.g. arrays, layouts). If no
     suitable backend is found, return the `default` value, or raise a `ValueError` if
@@ -100,15 +100,15 @@
     """
     backends = [
         b for b in (_backend_of(o, default=None) for o in objects) if b is not None
     ]
 
     if backends:
         return common_backend(backends)
-    elif default is unset:
+    elif default is UNSET:
         raise ValueError("could not find backend for", objects)
     else:
         return default
 
 
 def regularize_backend(backend: str | Backend) -> Backend:
     if isinstance(backend, Backend):
```

### Comparing `awkward-2.2.0/src/awkward/_backends/jax.py` & `awkward-2.2.1/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_backends/numpy.py` & `awkward-2.2.1/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_backends/typetracer.py` & `awkward-2.2.1/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/avro.py` & `awkward-2.2.1/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cling.py` & `awkward-2.2.1/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/hist.py` & `awkward-2.2.1/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numexpr.py` & `awkward-2.2.1/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numpy.py` & `awkward-2.2.1/src/awkward/_connect/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,31 +16,25 @@
     find_ufunc,
     find_ufunc_generic,
 )
 from awkward._layout import wrap_layout
 from awkward._nplikes import to_nplike
 from awkward._regularize import is_non_string_like_iterable
 from awkward._typing import Iterator
-from awkward._util import numpy_at_least
+from awkward._util import Sentinel, numpy_at_least
 from awkward.contents.numpyarray import NumpyArray
 
 # NumPy 1.13.1 introduced NEP13, without which Awkward ufuncs won't work, which
 # would be worse than lacking a feature: it would cause unexpected output.
 # NumPy 1.17.0 introduced NEP18, which is optional (use ak.* instead of np.*).
 if not numpy_at_least("1.13.1"):
     raise ImportError("NumPy 1.13.1 or later required")
 
 
-# FIXME: introduce sentinel type for this
-class _Unsupported:
-    def __repr__(self):
-        return f"{__name__}.unsupported"
-
-
-unsupported = _Unsupported()
+UNSUPPORTED = Sentinel("UNSUPPORTED", __name__)
 
 
 def convert_to_array(layout, args, kwargs):
     out = ak.operations.to_numpy(layout, allow_missing=False)
     if args == () and kwargs == {}:
         return out
     else:
@@ -120,15 +114,15 @@
         return function(*args, **kwargs)
 
 
 def implements(numpy_function):
     def decorator(function):
         signature = inspect.signature(function)
         unsupported_names = {
-            p.name for p in signature.parameters.values() if p.default is unsupported
+            p.name for p in signature.parameters.values() if p.default is UNSUPPORTED
         }
 
         @functools.wraps(function)
         def ensure_valid_args(*args, **kwargs):
             parameters = signature.bind(*args, **kwargs)
             provided_invalid_names = parameters.arguments.keys() & unsupported_names
             if provided_invalid_names:
@@ -209,15 +203,15 @@
             elif isinstance(x, NumpyArray):
                 signature.append(x.dtype.type)
             else:
                 signature.append(None)
         else:
             signature.append(type(x))
 
-    return signature
+    return tuple(signature)
 
 
 def array_ufunc(ufunc, method, inputs, kwargs):
     if method != "__call__" or len(inputs) == 0 or "out" in kwargs:
         return NotImplemented
 
     behavior = behavior_of(*inputs)
```

### Comparing `awkward-2.2.0/src/awkward/_connect/pyarrow.py` & `awkward-2.2.1/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/__init__.py` & `awkward-2.2.1/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.2.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.2.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.2.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.2.1/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/jax/reducers.py` & `awkward-2.2.1/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/jax/trees.py` & `awkward-2.2.1/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numba/arrayview.py` & `awkward-2.2.1/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.2.1/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numba/builder.py` & `awkward-2.2.1/src/awkward/_connect/numba/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def globalstring(context, builder, pyvalue):
     import llvmlite.ir.types
 
     if pyvalue not in dynamic_addrs:
         buf = dynamic_addrs[pyvalue] = numpy.array(pyvalue.encode("utf-8") + b"\x00")
-        context.add_dynamic_addr(builder, buf.ctypes.data, info=f"str({repr(pyvalue)})")
+        context.add_dynamic_addr(builder, buf.ctypes.data, info=f"str({pyvalue!r})")
     ptr = context.get_constant(numba.types.uintp, dynamic_addrs[pyvalue].ctypes.data)
     return builder.inttoptr(ptr, llvmlite.ir.PointerType(llvmlite.ir.IntType(8)))
 
 
 class ArrayBuilderType(numba.types.Type):
     def __init__(self, behavior):
         super().__init__(
```

### Comparing `awkward-2.2.0/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.2.1/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/numba/layout.py` & `awkward-2.2.1/src/awkward/_connect/numba/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     def getitem_field(self, viewtype, key):
         if self.has_field(key):
             return ak._connect.numba.arrayview.wrap(
                 self, viewtype, (*viewtype.fields, key)
             )
         else:
-            raise TypeError(f"array does not have a field with key {repr(key)}")
+            raise TypeError(f"array does not have a field with key {key!r}")
 
     def lower_getitem_at_check(
         self,
         context,
         builder,
         rettype,
         viewtype,
@@ -223,15 +223,15 @@
         elif fromtype.width == 16:
             fromtype = numba.int16
         elif fromtype.width == 32:
             fromtype = numba.int32
         elif fromtype.width == 64:
             fromtype = numba.int64
     if not isinstance(fromtype, numba.types.Integer):
-        raise AssertionError(f"unrecognized integer type: {repr(fromtype)}")
+        raise AssertionError(f"unrecognized integer type: {fromtype!r}")
 
     if fromtype.bitwidth < totype.bitwidth:
         if fromtype.signed:
             return builder.sext(val, context.get_value_type(totype))
         else:
             return builder.zext(val, context.get_value_type(totype))
     elif fromtype.bitwidth > totype.bitwidth:
```

### Comparing `awkward-2.2.0/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.2.1/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.2.1/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.2.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/__init__.py` & `awkward-2.2.1/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/array_module.py` & `awkward-2.2.1/src/awkward/_nplikes/array_module.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/cupy.py` & `awkward-2.2.1/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/jax.py` & `awkward-2.2.1/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/numpy.py` & `awkward-2.2.1/src/awkward/_nplikes/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/numpylike.py` & `awkward-2.2.1/src/awkward/_nplikes/numpylike.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/shape.py` & `awkward-2.2.1/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/_nplikes/typetracer.py` & `awkward-2.2.1/src/awkward/_nplikes/typetracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,80 +138,14 @@
             # with calls to both methods everywhere
             self._shape_touched_set.add(label)
             self._shape_touched.append(label)
             self._data_touched_set.add(label)
             self._data_touched.append(label)
 
 
-def _attach_report(layout, form, report: TypeTracerReport):
-    if isinstance(layout, (ak.contents.BitMaskedArray, ak.contents.ByteMaskedArray)):
-        assert isinstance(form, (ak.forms.BitMaskedForm, ak.forms.ByteMaskedForm))
-        layout.mask.data.form_key = form.form_key
-        layout.mask.data.report = report
-        _attach_report(layout.content, form.content, report)
-
-    elif isinstance(layout, ak.contents.EmptyArray):
-        assert isinstance(form, ak.forms.EmptyForm)
-
-    elif isinstance(layout, (ak.contents.IndexedArray, ak.contents.IndexedOptionArray)):
-        assert isinstance(form, (ak.forms.IndexedForm, ak.forms.IndexedOptionForm))
-        layout.index.data.form_key = form.form_key
-        layout.index.data.report = report
-        _attach_report(layout.content, form.content, report)
-
-    elif isinstance(layout, ak.contents.ListArray):
-        assert isinstance(form, ak.forms.ListForm)
-        layout.starts.data.form_key = form.form_key
-        layout.starts.data.report = report
-        layout.stops.data.form_key = form.form_key
-        layout.stops.data.report = report
-        _attach_report(layout.content, form.content, report)
-
-    elif isinstance(layout, ak.contents.ListOffsetArray):
-        assert isinstance(form, ak.forms.ListOffsetForm)
-        layout.offsets.data.form_key = form.form_key
-        layout.offsets.data.report = report
-        _attach_report(layout.content, form.content, report)
-
-    elif isinstance(layout, ak.contents.NumpyArray):
-        assert isinstance(form, ak.forms.NumpyForm)
-        layout.data.form_key = form.form_key
-        layout.data.report = report
-
-    elif isinstance(layout, ak.contents.RecordArray):
-        assert isinstance(form, ak.forms.RecordForm)
-        for x, y in zip(layout.contents, form.contents):
-            _attach_report(x, y, report)
-
-    elif isinstance(layout, (ak.contents.RegularArray, ak.contents.UnmaskedArray)):
-        assert isinstance(form, (ak.forms.RegularForm, ak.forms.UnmaskedForm))
-        _attach_report(layout.content, form.content, report)
-
-    elif isinstance(layout, ak.contents.UnionArray):
-        assert isinstance(form, ak.forms.UnionForm)
-        layout.tags.data.form_key = form.form_key
-        layout.tags.data.report = report
-        layout.index.data.form_key = form.form_key
-        layout.index.data.report = report
-        for x, y in zip(layout.contents, form.contents):
-            _attach_report(x, y, report)
-
-    else:
-        raise AssertionError(f"unrecognized layout type {type(layout)}")
-
-
-def typetracer_with_report(form, forget_length=True):
-    layout = form.length_zero_array(highlevel=False).to_typetracer(
-        forget_length=forget_length
-    )
-    report = TypeTracerReport()
-    _attach_report(layout, form, report)
-    return layout, report
-
-
 class TypeTracerArray(NDArrayOperatorsMixin, ArrayLike):
     _dtype: numpy.dtype
     _shape: tuple[ShapeItem, ...]
 
     def __new__(cls, *args, **kwargs):
         raise TypeError(
             "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
@@ -1356,7 +1290,77 @@
 
     @classmethod
     def is_own_array(cls, obj) -> bool:
         return cls.is_own_array_type(type(obj))
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
         return True
+
+
+def _attach_report(
+    layout: ak.contents.Content, form: ak.forms.Form, report: TypeTracerReport
+):
+    if isinstance(layout, (ak.contents.BitMaskedArray, ak.contents.ByteMaskedArray)):
+        assert isinstance(form, (ak.forms.BitMaskedForm, ak.forms.ByteMaskedForm))
+        layout.mask.data.form_key = form.form_key
+        layout.mask.data.report = report
+        _attach_report(layout.content, form.content, report)
+
+    elif isinstance(layout, ak.contents.EmptyArray):
+        assert isinstance(form, ak.forms.EmptyForm)
+
+    elif isinstance(layout, (ak.contents.IndexedArray, ak.contents.IndexedOptionArray)):
+        assert isinstance(form, (ak.forms.IndexedForm, ak.forms.IndexedOptionForm))
+        layout.index.data.form_key = form.form_key
+        layout.index.data.report = report
+        _attach_report(layout.content, form.content, report)
+
+    elif isinstance(layout, ak.contents.ListArray):
+        assert isinstance(form, ak.forms.ListForm)
+        layout.starts.data.form_key = form.form_key
+        layout.starts.data.report = report
+        layout.stops.data.form_key = form.form_key
+        layout.stops.data.report = report
+        _attach_report(layout.content, form.content, report)
+
+    elif isinstance(layout, ak.contents.ListOffsetArray):
+        assert isinstance(form, ak.forms.ListOffsetForm)
+        layout.offsets.data.form_key = form.form_key
+        layout.offsets.data.report = report
+        _attach_report(layout.content, form.content, report)
+
+    elif isinstance(layout, ak.contents.NumpyArray):
+        assert isinstance(form, ak.forms.NumpyForm)
+        layout.data.form_key = form.form_key
+        layout.data.report = report
+
+    elif isinstance(layout, ak.contents.RecordArray):
+        assert isinstance(form, ak.forms.RecordForm)
+        for x, y in zip(layout.contents, form.contents):
+            _attach_report(x, y, report)
+
+    elif isinstance(layout, (ak.contents.RegularArray, ak.contents.UnmaskedArray)):
+        assert isinstance(form, (ak.forms.RegularForm, ak.forms.UnmaskedForm))
+        _attach_report(layout.content, form.content, report)
+
+    elif isinstance(layout, ak.contents.UnionArray):
+        assert isinstance(form, ak.forms.UnionForm)
+        layout.tags.data.form_key = form.form_key
+        layout.tags.data.report = report
+        layout.index.data.form_key = form.form_key
+        layout.index.data.report = report
+        for x, y in zip(layout.contents, form.contents):
+            _attach_report(x, y, report)
+
+    else:
+        raise AssertionError(f"unrecognized layout type {type(layout)}")
+
+
+def typetracer_with_report(
+    form: ak.forms.Form, forget_length: bool = True
+) -> tuple[ak.contents.Content, TypeTracerReport]:
+    layout = form.length_zero_array(highlevel=False).to_typetracer(
+        forget_length=forget_length
+    )
+    report = TypeTracerReport()
+    _attach_report(layout, form, report)
+    return layout, report
```

### Comparing `awkward-2.2.0/src/awkward/_nplikes/ufuncs.py` & `awkward-2.2.1/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/behaviors/categorical.py` & `awkward-2.2.1/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/behaviors/mixins.py` & `awkward-2.2.1/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/behaviors/string.py` & `awkward-2.2.1/src/awkward/behaviors/string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/contents/__init__.py` & `awkward-2.2.1/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/contents/bitmaskedarray.py` & `awkward-2.2.1/src/awkward/contents/bitmaskedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     type_parameters_equal,
 )
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.forms.bitmaskedform import BitMaskedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
@@ -201,29 +201,29 @@
     def lsb_order(self):
         return self._lsb_order
 
     form_cls: Final = BitMaskedForm
 
     def copy(
         self,
-        mask=unset,
-        content=unset,
-        valid_when=unset,
-        length=unset,
-        lsb_order=unset,
+        mask=UNSET,
+        content=UNSET,
+        valid_when=UNSET,
+        length=UNSET,
+        lsb_order=UNSET,
         *,
-        parameters=unset,
+        parameters=UNSET,
     ):
         return BitMaskedArray(
-            self._mask if mask is unset else mask,
-            self._content if content is unset else content,
-            self._valid_when if valid_when is unset else valid_when,
-            self._length if length is unset else length,
-            self._lsb_order if lsb_order is unset else lsb_order,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._mask if mask is UNSET else mask,
+            self._content if content is UNSET else content,
+            self._valid_when if valid_when is UNSET else valid_when,
+            self._length if length is UNSET else length,
+            self._lsb_order if lsb_order is UNSET else lsb_order,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/contents/bytemaskedarray.py` & `awkward-2.2.1/src/awkward/contents/bytemaskedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.bytemaskedform import ByteMaskedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 np = NumpyMetadata.instance()
@@ -143,20 +143,20 @@
 
     @property
     def valid_when(self):
         return self._valid_when
 
     form_cls: Final = ByteMaskedForm
 
-    def copy(self, mask=unset, content=unset, valid_when=unset, *, parameters=unset):
+    def copy(self, mask=UNSET, content=UNSET, valid_when=UNSET, *, parameters=UNSET):
         return ByteMaskedArray(
-            self._mask if mask is unset else mask,
-            self._content if content is unset else content,
-            self._valid_when if valid_when is unset else valid_when,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._mask if mask is UNSET else mask,
+            self._content if content is UNSET else content,
+            self._valid_when if valid_when is UNSET else valid_when,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/contents/content.py` & `awkward-2.2.1/src/awkward/contents/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     JSONMapping,
     Literal,
     Self,
     SupportsIndex,
     TypeAlias,
     TypedDict,
 )
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 from awkward.index import Index, Index64
 
 if TYPE_CHECKING:
     from awkward._nplikes.numpy import NumpyLike
     from awkward._slicing import SliceItem
 
@@ -898,21 +898,21 @@
                 n,
                 replacement,
                 self.length,
                 1,
             )
         )
         contents = []
-        length = ak._util.unset
+        length = ak._util.UNSET
         for ptr in tocarry:
             contents.append(
                 ak.contents.IndexedArray.simplified(ptr, self, parameters=None)
             )
             length = contents[-1].length
-        assert not (length is ak._util.unset and self._backend.nplike.known_data)
+        assert not (length is ak._util.UNSET and self._backend.nplike.known_data)
         return ak.contents.RecordArray(
             contents, recordlookup, length, parameters=parameters, backend=self._backend
         )
 
     def _combinations(
         self,
         n: int,
@@ -1308,15 +1308,15 @@
 
     def _numbers_to_type(self, name: str, including_unknown: bool) -> Content:
         raise NotImplementedError
 
     def _fill_none(self, value: Content) -> Content:
         raise NotImplementedError
 
-    def copy(self, *, parameters: JSONMapping | None = unset) -> Self:
+    def copy(self, *, parameters: JSONMapping | None = UNSET) -> Self:
         raise NotImplementedError
 
 
 @register_backend_lookup_factory
 def find_content_backend(obj: type):
     if issubclass(obj, Content):
```

### Comparing `awkward-2.2.0/src/awkward/contents/emptyarray.py` & `awkward-2.2.1/src/awkward/contents/emptyarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from awkward._errors import AxisError, deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.emptyform import EmptyForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -75,24 +75,24 @@
         self._init(parameters, backend)
 
     form_cls: Final = EmptyForm
 
     def copy(
         self,
         *,
-        parameters=unset,
-        backend=unset,
+        parameters=UNSET,
+        backend=UNSET,
     ):
-        if not (parameters is unset or parameters is None or len(parameters) == 0):
+        if not (parameters is UNSET or parameters is None or len(parameters) == 0):
             deprecate(
                 f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         return EmptyArray(
-            parameters=self._parameters if parameters is unset else parameters,
-            backend=self._backend if backend is unset else backend,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            backend=self._backend if backend is UNSET else backend,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(parameters=copy.deepcopy(self._parameters, memo))
```

### Comparing `awkward-2.2.0/src/awkward/contents/indexedarray.py` & `awkward-2.2.1/src/awkward/contents/indexedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.indexedform import IndexedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -124,19 +124,19 @@
 
     @property
     def content(self):
         return self._content
 
     form_cls: Final = IndexedForm
 
-    def copy(self, index=unset, content=unset, *, parameters=unset):
+    def copy(self, index=UNSET, content=UNSET, *, parameters=UNSET):
         return IndexedArray(
-            self._index if index is unset else index,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._index if index is UNSET else index,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/contents/indexedoptionarray.py` & `awkward-2.2.1/src/awkward/contents/indexedoptionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.indexedoptionform import IndexedOptionForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -122,19 +122,19 @@
 
     @property
     def content(self):
         return self._content
 
     form_cls: Final = IndexedOptionForm
 
-    def copy(self, index=unset, content=unset, *, parameters=unset):
+    def copy(self, index=UNSET, content=UNSET, *, parameters=UNSET):
         return IndexedOptionArray(
-            self._index if index is unset else index,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._index if index is UNSET else index,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/contents/listarray.py` & `awkward-2.2.1/src/awkward/contents/listarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.contents.listoffsetarray import ListOffsetArray
 from awkward.forms.listform import ListForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
@@ -168,20 +168,20 @@
 
     @property
     def content(self):
         return self._content
 
     form_cls: Final = ListForm
 
-    def copy(self, starts=unset, stops=unset, content=unset, *, parameters=unset):
+    def copy(self, starts=UNSET, stops=UNSET, content=UNSET, *, parameters=UNSET):
         return ListArray(
-            self._starts if starts is unset else starts,
-            self._stops if stops is unset else stops,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._starts if starts is UNSET else starts,
+            self._stops if stops is UNSET else stops,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
@@ -1424,15 +1424,21 @@
 
     def _to_arrow(self, pyarrow, mask_node, validbytes, length, options):
         return self.to_ListOffsetArray64(False)._to_arrow(
             pyarrow, mask_node, validbytes, length, options
         )
 
     def _to_backend_array(self, allow_missing, backend):
-        return self.to_RegularArray()._to_backend_array(allow_missing, backend)
+        array_param = self.parameter("__array__")
+        if array_param in {"bytestring", "string"}:
+            # As our array-of-strings _may_ be empty, we should pass the dtype
+            dtype = np.str_ if array_param == "string" else np.bytes_
+            return backend.nplike.asarray(self.to_list(), dtype=dtype)
+        else:
+            return self.to_RegularArray()._to_backend_array(allow_missing, backend)
 
     def _remove_structure(self, backend, options):
         return self.to_ListOffsetArray64(False)._remove_structure(backend, options)
 
     def _drop_none(self):
         return self.to_ListOffsetArray64()._drop_none()
```

### Comparing `awkward-2.2.0/src/awkward/contents/listoffsetarray.py` & `awkward-2.2.1/src/awkward/contents/listoffsetarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from awkward._nplikes.typetracer import TypeTracer, is_unknown_scalar
 from awkward._parameters import (
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.listoffsetform import ListOffsetForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -146,19 +146,19 @@
 
     @property
     def content(self):
         return self._content
 
     form_cls: Final = ListOffsetForm
 
-    def copy(self, offsets=unset, content=unset, *, parameters=unset):
+    def copy(self, offsets=UNSET, content=UNSET, *, parameters=UNSET):
         return ListOffsetArray(
-            self._offsets if offsets is unset else offsets,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._offsets if offsets is UNSET else offsets,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
@@ -2000,17 +2000,19 @@
                     validbytes, options["count_nulls"]
                 ),
             )
 
     def _to_backend_array(self, allow_missing, backend):
         array_param = self.parameter("__array__")
         if array_param in {"bytestring", "string"}:
-            return backend.nplike.asarray(self.to_list())
-
-        return self.to_RegularArray()._to_backend_array(allow_missing, backend)
+            # As our array-of-strings _may_ be empty, we should pass the dtype
+            dtype = np.str_ if array_param == "string" else np.bytes_
+            return backend.nplike.asarray(self.to_list(), dtype=dtype)
+        else:
+            return self.to_RegularArray()._to_backend_array(allow_missing, backend)
 
     def _remove_structure(self, backend, options):
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             return [self]
```

### Comparing `awkward-2.2.0/src/awkward/contents/numpyarray.py` & `awkward-2.2.1/src/awkward/contents/numpyarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.numpyform import NumpyForm
 from awkward.index import Index
 from awkward.types.numpytype import primitive_to_dtype
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
@@ -124,23 +124,23 @@
     def data(self) -> ArrayLike:
         return self._data
 
     form_cls: Final = NumpyForm
 
     def copy(
         self,
-        data=unset,
+        data=UNSET,
         *,
-        parameters=unset,
-        backend=unset,
+        parameters=UNSET,
+        backend=UNSET,
     ):
         return NumpyArray(
-            self._data if data is unset else data,
-            parameters=self._parameters if parameters is unset else parameters,
-            backend=self._backend if backend is unset else backend,
+            self._data if data is UNSET else data,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            backend=self._backend if backend is UNSET else backend,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/contents/recordarray.py` & `awkward-2.2.1/src/awkward/contents/recordarray.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,47 @@
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._behavior import find_record_reducer
 from awkward._errors import AxisError
-from awkward._layout import maybe_posaxis
+from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.recordform import RecordForm
 from awkward.index import Index
 from awkward.record import Record
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
+def _apply_record_reducer(
+    reducer, layout: RecordArray, mask: bool, offsets: ak.index.Index, behavior
+) -> Content:
+    # Build a 1D list over these contents
+    array = wrap_layout(ak.contents.ListOffsetArray(offsets, layout), behavior=behavior)
+    # Perform the reduction
+    return ak.to_layout(reducer(array, mask))
+
+
 @final
 class RecordArray(Content):
     """
     RecordArray represents an array of tuples or records, all with the
     same type. Its `contents` is an ordered list of arrays.
 
     * If `fields` is None, the data are tuples, indexed only by their order.
@@ -256,27 +265,27 @@
         else:
             return self._fields
 
     form_cls: Final = RecordForm
 
     def copy(
         self,
-        contents=unset,
-        fields=unset,
-        length=unset,
+        contents=UNSET,
+        fields=UNSET,
+        length=UNSET,
         *,
-        parameters=unset,
-        backend=unset,
+        parameters=UNSET,
+        backend=UNSET,
     ):
         return RecordArray(
-            self._contents if contents is unset else contents,
-            self._fields if fields is unset else fields,
-            self._length if length is unset else length,
-            parameters=self._parameters if parameters is unset else parameters,
-            backend=self._backend if backend is unset else backend,
+            self._contents if contents is UNSET else contents,
+            self._fields if fields is UNSET else fields,
+            self._length if length is UNSET else length,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            backend=self._backend if backend is UNSET else backend,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
@@ -363,15 +372,15 @@
         out.append(repr(str(self.length)))
         out.append(">")
         out.extend(self._repr_extra(indent + "    "))
         out.append("\n")
 
         if self._fields is None:
             for i, x in enumerate(self._contents):
-                out.append(f"{indent}    <content index={repr(str(i))}>\n")
+                out.append(f"{indent}    <content index={str(i)!r}>\n")
                 out.append(x._repr(indent + "        ", "", "\n"))
                 out.append(indent + "    </content>\n")
         else:
             for i, x in enumerate(self._contents):
                 out.append(
                     "{}    <content index={} field={}>\n".format(
                         indent, repr(str(i)), repr(self._fields[i])
@@ -738,21 +747,21 @@
                         "cannot merge "
                         + type(self).__name__
                         + " with "
                         + type(array).__name__
                     )
 
         nextcontents = []
-        minlength = ak._util.unset
+        minlength = ak._util.UNSET
         for forfield in for_each_field:
             merged = forfield[0]._mergemany(forfield[1:])
 
             nextcontents.append(merged)
 
-            if minlength is ak._util.unset or (
+            if minlength is ak._util.UNSET or (
                 not (merged.length is unknown_length or minlength is unknown_length)
                 and merged.length < minlength
             ):
                 minlength = merged.length
 
         if minlength is unknown_length:
             minlength = self.length
@@ -885,30 +894,136 @@
         keepdims,
         behavior,
     ):
         reducer_recordclass = find_record_reducer(reducer, self, behavior)
         if reducer_recordclass is None:
             raise TypeError(
                 "no ak.{} overloads for custom types: {}".format(
-                    reducer.name, ", ".join(self._fields)
+                    reducer.name, ", ".join(self.fields)
                 )
             )
         else:
-            raise NotImplementedError(
-                "overloading reducers for RecordArrays has not been implemented yet"
+            # Convert parents into offsets
+            outoffsets = ak.index.Index64.empty(
+                outlength + 1, self._backend.index_nplike
+            )
+            assert (
+                outoffsets.nplike is self._backend.index_nplike
+                and parents.nplike is self._backend.index_nplike
+            )
+            self._handle_error(
+                self._backend[
+                    "awkward_ListOffsetArray_reduce_local_outoffsets_64",
+                    outoffsets.dtype.type,
+                    parents.dtype.type,
+                ](
+                    outoffsets.data,
+                    parents.data,
+                    parents.length,
+                    outlength,
+                )
+            )
+
+            out = _apply_record_reducer(
+                reducer_recordclass, self, mask, outoffsets, behavior
             )
 
+            if reducer.needs_position:
+                assert isinstance(out, ak.contents.NumpyArray)
+
+                if shifts is None:
+                    assert (
+                        out.backend is self._backend
+                        and parents.nplike is self._backend.index_nplike
+                        and starts.nplike is self._backend.index_nplike
+                    )
+                    self._handle_error(
+                        self._backend[
+                            "awkward_NumpyArray_reduce_adjust_starts_64",
+                            out.data.dtype.type,
+                            parents.dtype.type,
+                            starts.dtype.type,
+                        ](
+                            out.data,
+                            outlength,
+                            parents.data,
+                            starts.data,
+                        )
+                    )
+                else:
+                    assert (
+                        out.backend is self._backend
+                        and parents.nplike is self._backend.index_nplike
+                        and starts.nplike is self._backend.index_nplike
+                        and shifts.nplike is self._backend.index_nplike
+                    )
+                    self._handle_error(
+                        self._backend[
+                            "awkward_NumpyArray_reduce_adjust_starts_shifts_64",
+                            out.data.dtype.type,
+                            parents.dtype.type,
+                            starts.dtype.type,
+                            shifts.dtype.type,
+                        ](
+                            out.data,
+                            outlength,
+                            parents.data,
+                            starts.data,
+                            shifts.data,
+                        )
+                    )
+
+            if mask:
+                outmask = ak.index.Index8.empty(outlength, self._backend.index_nplike)
+                assert (
+                    outmask.nplike is self._backend.index_nplike
+                    and parents.nplike is self._backend.index_nplike
+                )
+                self._handle_error(
+                    self._backend[
+                        "awkward_NumpyArray_reduce_mask_ByteMaskedArray_64",
+                        outmask.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        outmask.data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                    )
+                )
+
+                out = ak.contents.ByteMaskedArray.simplified(
+                    outmask, out, False, parameters=None
+                )
+            elif out.is_option:
+                raise TypeError(
+                    "a custom reducer function returned an option when it was not expected"
+                )
+
+            if keepdims:
+                out = ak.contents.RegularArray(out, 1, self.length, parameters=None)
+
+            return out
+
     def _validity_error(self, path):
         for i, cont in enumerate(self.contents):
             if cont.length < self.length:
                 return f"at {path} ({type(self)!r}): len(field({i})) < len(recordarray)"
         for i, cont in enumerate(self.contents):
             sub = cont._validity_error(f"{path}.field({i})")
             if sub != "":
                 return sub
+
+        # Check for duplicate fields
+        if not self.is_tuple:
+            seen_fields = set()
+            for field in self._fields:
+                if field in seen_fields:
+                    return f"at {path} ({type(self)!r}): duplicate field {field!r}"
+                seen_fields.add(field)
         return ""
 
     def _nbytes_part(self):
         result = 0
         for content in self.contents:
             result = result + content._nbytes_part()
         return result
@@ -996,14 +1111,16 @@
 
     def _remove_structure(self, backend, options):
         if options["flatten_records"]:
             out = []
             for content in self._contents:
                 out.extend(content[: self._length]._remove_structure(backend, options))
             return out
+        elif options["allow_records"]:
+            return [self]
         else:
             in_function = ""
             if options["function_name"] is not None:
                 in_function = " in " + options["function_name"]
             raise TypeError(
                 (
                     "encountered a record whilst removing array structure{}, "
```

### Comparing `awkward-2.2.0/src/awkward/contents/regulararray.py` & `awkward-2.2.1/src/awkward/contents/regulararray.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.regularform import RegularForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -171,20 +171,20 @@
 
     @property
     def size(self):
         return self._size
 
     form_cls: Final = RegularForm
 
-    def copy(self, content=unset, size=unset, zeros_length=unset, *, parameters=unset):
+    def copy(self, content=UNSET, size=UNSET, zeros_length=UNSET, *, parameters=UNSET):
         return RegularArray(
-            self._content if content is unset else content,
-            self._size if size is unset else size,
-            self._length if zeros_length is unset else zeros_length,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._content if content is UNSET else content,
+            self._size if size is UNSET else size,
+            self._length if zeros_length is UNSET else zeros_length,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
@@ -936,19 +936,19 @@
                         replacement,
                         self._size,
                         self._length,
                     )
                 )
 
             contents = []
-            length = unset
+            length = UNSET
             for ptr in tocarry:
                 contents.append(self._content._carry(ptr, True))
                 length = contents[-1].length
-            assert length is not unset
+            assert length is not UNSET
             recordarray = ak.contents.RecordArray(
                 contents,
                 recordlookup,
                 length,
                 parameters=parameters,
                 backend=self._backend,
             )
@@ -1202,27 +1202,35 @@
                 self._length,
                 parameters=self._parameters,
             )
 
     def _to_backend_array(self, allow_missing, backend):
         array_param = self.parameter("__array__")
         if array_param in {"bytestring", "string"}:
-            return backend.nplike.asarray(self.to_list())
-
-        out = self._content._to_backend_array(allow_missing, backend)
-        shape = (self._length, self._size) + out.shape[1:]
+            # As our array-of-strings _may_ be empty, we should pass the dtype
+            dtype = np.str_ if array_param == "string" else np.bytes_
+            return backend.nplike.asarray(self.to_list(), dtype=dtype)
+        else:
+            out = self._content._to_backend_array(allow_missing, backend)
+            shape = (self._length, self._size) + out.shape[1:]
 
-        # ShapeItem is a defined type, but some nplikes don't map onto the entire space; e.g.
-        # NumPy never has `None` shape items. We require that if a shape-item is used between nplikes
-        # they both be the same "known-shape-ness".
-        assert self._backend.index_nplike.known_data == self._backend.nplike.known_data
-        return self._backend.nplike.reshape(
-            out[: self._backend.nplike.shape_item_as_index(self._length * self._size)],
-            shape,
-        )
+            # ShapeItem is a defined type, but some nplikes don't map onto the entire space; e.g.
+            # NumPy never has `None` shape items. We require that if a shape-item is used between nplikes
+            # they both be the same "known-shape-ness".
+            assert (
+                self._backend.index_nplike.known_data == self._backend.nplike.known_data
+            )
+            return self._backend.nplike.reshape(
+                out[
+                    : self._backend.nplike.shape_item_as_index(
+                        self._length * self._size
+                    )
+                ],
+                shape,
+            )
 
     def _to_arrow(self, pyarrow, mask_node, validbytes, length, options):
         assert self._backend.nplike.known_data
 
         if self.parameter("__array__") == "string":
             return self.to_ListOffsetArray64(False)._to_arrow(
                 pyarrow, mask_node, validbytes, length, options
```

### Comparing `awkward-2.2.0/src/awkward/contents/unionarray.py` & `awkward-2.2.1/src/awkward/contents/unionarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.unionform import UnionForm
 from awkward.index import Index, Index8, Index64
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -184,25 +184,25 @@
     def contents(self):
         return self._contents
 
     form_cls: Final = UnionForm
 
     def copy(
         self,
-        tags=unset,
-        index=unset,
-        contents=unset,
+        tags=UNSET,
+        index=UNSET,
+        contents=UNSET,
         *,
-        parameters=unset,
+        parameters=UNSET,
     ):
         return UnionArray(
-            self._tags if tags is unset else tags,
-            self._index if index is unset else index,
-            self._contents if contents is unset else contents,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._tags if tags is UNSET else tags,
+            self._index if index is UNSET else index,
+            self._contents if contents is UNSET else contents,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
@@ -483,15 +483,15 @@
         out.append(">")
         out.extend(self._repr_extra(indent + "    "))
         out.append("\n")
         out.append(self._tags._repr(indent + "    ", "<tags>", "</tags>\n"))
         out.append(self._index._repr(indent + "    ", "<index>", "</index>\n"))
 
         for i, x in enumerate(self._contents):
-            out.append(f"{indent}    <content index={repr(str(i))}>\n")
+            out.append(f"{indent}    <content index={str(i)!r}>\n")
             out.append(x._repr(indent + "        ", "", "\n"))
             out.append(f"{indent}    </content>\n")
 
         out.append(indent + "</UnionArray>")
         out.append(post)
         return "".join(out)
```

### Comparing `awkward-2.2.0/src/awkward/contents/unmaskedarray.py` & `awkward-2.2.1/src/awkward/contents/unmaskedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.unmaskedform import UnmaskedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -85,18 +85,18 @@
 
     @property
     def content(self):
         return self._content
 
     form_cls: Final = UnmaskedForm
 
-    def copy(self, content=unset, *, parameters=unset):
+    def copy(self, content=UNSET, *, parameters=UNSET):
         return UnmaskedArray(
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
         )
 
     def __copy__(self):
         return self.copy()
 
     def __deepcopy__(self, memo):
         return self.copy(
```

### Comparing `awkward-2.2.0/src/awkward/forms/__init__.py` & `awkward-2.2.1/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/forms/bitmaskedform.py` & `awkward-2.2.1/src/awkward/forms/bitmaskedform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class BitMaskedForm(Form):
     is_option = True
 
@@ -66,29 +65,29 @@
 
     @property
     def lsb_order(self):
         return self._lsb_order
 
     def copy(
         self,
-        mask=unset,
-        content=unset,
-        valid_when=unset,
-        lsb_order=unset,
+        mask=UNSET,
+        content=UNSET,
+        valid_when=UNSET,
+        lsb_order=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return BitMaskedForm(
-            self._mask if mask is unset else mask,
-            self._content if content is unset else content,
-            self._valid_when if valid_when is unset else valid_when,
-            self._lsb_order if lsb_order is unset else lsb_order,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._mask if mask is UNSET else mask,
+            self._content if content is UNSET else content,
+            self._valid_when if valid_when is UNSET else valid_when,
+            self._lsb_order if lsb_order is UNSET else lsb_order,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         mask,
         content,
@@ -138,19 +137,18 @@
                 "valid_when": self._valid_when,
                 "lsb_order": self._lsb_order,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.OptionType(
-            self._content._type(typestrs),
-            parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
+            self._content.type, parameters=self._parameters
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, BitMaskedForm):
             return (
                 self._form_key == other._form_key
                 and self._mask == other._mask
```

### Comparing `awkward-2.2.0/src/awkward/forms/bytemaskedform.py` & `awkward-2.2.1/src/awkward/forms/bytemaskedform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ByteMaskedForm(Form):
     is_option = True
 
@@ -54,27 +53,27 @@
 
     @property
     def valid_when(self):
         return self._valid_when
 
     def copy(
         self,
-        mask=unset,
-        content=unset,
-        valid_when=unset,
+        mask=UNSET,
+        content=UNSET,
+        valid_when=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return ByteMaskedForm(
-            self._mask if mask is unset else mask,
-            self._content if content is unset else content,
-            self._valid_when if valid_when is unset else valid_when,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._mask if mask is UNSET else mask,
+            self._content if content is UNSET else content,
+            self._valid_when if valid_when is UNSET else valid_when,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         mask,
         content,
@@ -116,19 +115,18 @@
                 "mask": self._mask,
                 "valid_when": self._valid_when,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.OptionType(
-            self._content._type(typestrs),
-            parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
+            self._content.type, parameters=self._parameters
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, ByteMaskedForm):
             return (
                 self._form_key == other._form_key
                 and self._mask == other._mask
```

### Comparing `awkward-2.2.0/src/awkward/forms/emptyform.py` & `awkward-2.2.1/src/awkward/forms/emptyform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._errors import deprecate
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form, JSONMapping
 
 
 @final
 class EmptyForm(Form):
     is_numpy = True
     is_unknown = True
@@ -18,23 +17,23 @@
         if not (parameters is None or len(parameters) == 0):
             deprecate(
                 f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         self._init(parameters=parameters, form_key=form_key)
 
     def copy(
-        self, *, parameters: JSONMapping | None = unset, form_key=unset
+        self, *, parameters: JSONMapping | None = UNSET, form_key=UNSET
     ) -> EmptyForm:
-        if not (parameters is unset or parameters is None or len(parameters) == 0):
+        if not (parameters is UNSET or parameters is None or len(parameters) == 0):
             deprecate(
                 f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         return EmptyForm(
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(cls, *, parameters=None, form_key=None) -> Form:
         if not (parameters is None or len(parameters) == 0):
             deprecate(f"{cls.__name__} cannot contain parameters", version="2.2.0")
         return cls(parameters=parameters, form_key=form_key)
@@ -42,19 +41,17 @@
     def __repr__(self):
         args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _to_dict_part(self, verbose, toplevel):
         return self._to_dict_extra({"class": "EmptyArray"}, verbose)
 
-    def _type(self, typestrs):
-        return ak.types.UnknownType(
-            parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
-        )
+    @property
+    def type(self):
+        return ak.types.UnknownType(parameters=self._parameters)
 
     def __eq__(self, other) -> bool:
         return isinstance(other, EmptyForm) and self._form_key == other._form_key
 
     def to_NumpyForm(self, dtype):
         return ak.forms.numpyform.from_dtype(dtype, parameters=self._parameters)
```

### Comparing `awkward-2.2.0/src/awkward/forms/form.py` & `awkward-2.2.1/src/awkward/forms/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import itertools
 import json
 import re
 from collections.abc import Mapping
 
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
-from awkward._behavior import find_typestrs
 from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import parameters_union
 from awkward._typing import Final, JSONMapping, JSONSerializable
 
 np = NumpyMetadata.instance()
@@ -373,18 +372,25 @@
             out.append("parameters=" + repr(self._parameters))
         if self._form_key is not None:
             out.append("form_key=" + repr(self._form_key))
         return out
 
     @property
     def type(self):
-        return self._type({})
+        raise NotImplementedError
 
     def type_from_behavior(self, behavior):
-        return self._type(find_typestrs(behavior))
+        deprecate(
+            "low level types produced by forms do not hold references to behaviors. "
+            "Use a high-level type (e.g. ak.types.ArrayType or ak.types.ScalarType) to"
+            "associate a type with behavior information, or simply access the low-level"
+            "type from Form.type",
+            version="2.4.0",
+        )
+        return self.type
 
     def columns(self, list_indicator=None, column_prefix=()):
         output = []
         self._columns(column_prefix, output, list_indicator)
         return output
 
     def select_columns(self, specifier, expand_braces=True):
@@ -421,17 +427,14 @@
 
     def _column_types(self):
         raise NotImplementedError
 
     def _to_dict_part(self, verbose, toplevel):
         raise NotImplementedError
 
-    def _type(self, typestrs):
-        raise NotImplementedError
-
     def length_zero_array(
         self, *, backend=numpy_backend, highlevel=True, behavior=None
     ):
         if highlevel:
             deprecate(
                 "The `highlevel=True` variant of `Form.length_zero_array` is now deprecated. "
                 "Please use `ak.Array(form.length_zero_array(...), behavior=...)` if an `ak.Array` is required.",
```

### Comparing `awkward-2.2.0/src/awkward/forms/indexedform.py` & `awkward-2.2.1/src/awkward/forms/indexedform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import awkward as ak
 from awkward._parameters import parameters_union, type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class IndexedForm(Form):
     is_indexed = True
 
@@ -42,25 +42,25 @@
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        index=unset,
-        content=unset,
+        index=UNSET,
+        content=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return IndexedForm(
-            self._index if index is unset else index,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._index if index is UNSET else index,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         index,
         content,
@@ -102,16 +102,17 @@
                 "class": "IndexedArray",
                 "index": self._index,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
-        out = self._content._type(typestrs)
+    @property
+    def type(self):
+        out = self._content.type
 
         if self._parameters is not None:
             if out._parameters is None:
                 out._parameters = self._parameters
             else:
                 out._parameters = parameters_union(out._parameters, self._parameters)
```

### Comparing `awkward-2.2.0/src/awkward/forms/indexedoptionform.py` & `awkward-2.2.1/src/awkward/forms/indexedoptionform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import parameters_union, type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class IndexedOptionForm(Form):
     is_option = True
     is_indexed = True
@@ -43,25 +42,25 @@
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        index=unset,
-        content=unset,
+        index=UNSET,
+        content=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return IndexedOptionForm(
-            self._index if index is unset else index,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._index if index is UNSET else index,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         index,
         content,
@@ -94,26 +93,26 @@
                 "class": "IndexedOptionArray",
                 "index": self._index,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         if self.parameter("__array__") == "categorical":
             parameters = dict(self._parameters)
             del parameters["__array__"]
             parameters["__categorical__"] = True
         else:
             parameters = self._parameters
 
         return ak.types.OptionType(
-            self._content._type(typestrs),
+            self._content.type,
             parameters=parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, IndexedOptionForm):
             return (
                 self._form_key == other._form_key
                 and self._index == other._index
```

### Comparing `awkward-2.2.0/src/awkward/forms/listform.py` & `awkward-2.2.1/src/awkward/forms/listform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ListForm(Form):
     is_list = True
 
@@ -54,27 +53,27 @@
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        starts=unset,
-        stops=unset,
-        content=unset,
+        starts=UNSET,
+        stops=UNSET,
+        content=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return ListForm(
-            self._starts if starts is unset else starts,
-            self._stops if stops is unset else stops,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._starts if starts is UNSET else starts,
+            self._stops if stops is UNSET else stops,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         starts,
         stops,
@@ -101,19 +100,19 @@
                 "starts": self._starts,
                 "stops": self._stops,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.ListType(
-            self._content._type(typestrs),
+            self._content.type,
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         )
 
     def __eq__(self, other):
         if isinstance(other, ListForm):
             return (
                 self._form_key == other._form_key
                 and self._starts == other._starts
```

### Comparing `awkward-2.2.0/src/awkward/forms/listoffsetform.py` & `awkward-2.2.1/src/awkward/forms/listoffsetform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ListOffsetForm(Form):
     is_list = True
 
@@ -29,25 +28,25 @@
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        offsets=unset,
-        content=unset,
+        offsets=UNSET,
+        content=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return ListOffsetForm(
-            self._offsets if offsets is unset else offsets,
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._offsets if offsets is UNSET else offsets,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(cls, offsets, content, *, parameters=None, form_key=None):
         return cls(offsets, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
@@ -60,19 +59,19 @@
                 "class": "ListOffsetArray",
                 "offsets": self._offsets,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.ListType(
-            self._content._type(typestrs),
+            self._content.type,
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         )
 
     def __eq__(self, other):
         if isinstance(other, ListOffsetForm):
             return (
                 self._form_key == other._form_key
                 and self._offsets == other._offsets
```

### Comparing `awkward-2.2.0/src/awkward/forms/numpyform.py` & `awkward-2.2.1/src/awkward/forms/numpyform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections.abc import Iterable
 
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 np = NumpyMetadata.instance()
 
 
 def from_dtype(dtype, parameters=None):
     if dtype.subdtype is None:
@@ -69,25 +68,25 @@
 
     @property
     def inner_shape(self):
         return self._inner_shape
 
     def copy(
         self,
-        primitive=unset,
-        inner_shape=unset,
+        primitive=UNSET,
+        inner_shape=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return NumpyForm(
-            self._primitive if primitive is unset else primitive,
-            self._inner_shape if inner_shape is unset else inner_shape,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._primitive if primitive is UNSET else primitive,
+            self._inner_shape if inner_shape is UNSET else inner_shape,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         primitive,
         inner_shape=(),
@@ -123,19 +122,19 @@
                 "class": "NumpyArray",
                 "primitive": self._primitive,
             }
             if verbose or len(self._inner_shape) > 0:
                 out["inner_shape"] = list(self._inner_shape)
             return self._to_dict_extra(out, verbose)
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         out = ak.types.NumpyType(
             self._primitive,
             parameters=None,
-            typestr=find_typestr(self._parameters, typestrs),
         )
         for x in self._inner_shape[::-1]:
             out = ak.types.RegularType(out, x)
 
         out._parameters = self._parameters
 
         return out
```

### Comparing `awkward-2.2.0/src/awkward/forms/recordform.py` & `awkward-2.2.1/src/awkward/forms/recordform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import glob
 from collections.abc import Iterable
 
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class RecordForm(Form):
     is_record = True
 
@@ -56,25 +55,25 @@
         if self._fields is None:
             return [str(i) for i in range(len(self._contents))]
         else:
             return self._fields
 
     def copy(
         self,
-        contents=unset,
-        fields=unset,
+        contents=UNSET,
+        fields=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return RecordForm(
-            self._contents if contents is unset else contents,
-            self._fields if fields is unset else fields,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._contents if contents is UNSET else contents,
+            self._fields if fields is UNSET else fields,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         contents,
         fields,
@@ -161,20 +160,20 @@
             out["fields"] = list(self._fields)
         else:
             out["fields"] = None
 
         out["contents"] = contents_tolist
         return self._to_dict_extra(out, verbose)
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.RecordType(
-            [x._type(typestrs) for x in self._contents],
+            [x.type for x in self._contents],
             self._fields,
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         )
 
     def __eq__(self, other):
         if isinstance(other, RecordForm):
             if (
                 self._form_key == other._form_key
                 and self.is_tuple == other.is_tuple
```

### Comparing `awkward-2.2.0/src/awkward/forms/regularform.py` & `awkward-2.2.1/src/awkward/forms/regularform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class RegularForm(Form):
     is_list = True
     is_regular = True
@@ -36,20 +35,20 @@
     def content(self):
         return self._content
 
     @property
     def size(self):
         return self._size
 
-    def copy(self, content=unset, size=unset, *, parameters=unset, form_key=unset):
+    def copy(self, content=UNSET, size=UNSET, *, parameters=UNSET, form_key=UNSET):
         return RegularForm(
-            self._content if content is unset else content,
-            self._size if size is unset else size,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._content if content is UNSET else content,
+            self._size if size is UNSET else size,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(cls, content, size, *, parameters=None, form_key=None):
         return cls(content, size, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
@@ -62,20 +61,20 @@
                 "class": "RegularArray",
                 "size": None if self._size is unknown_length else self._size,
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.RegularType(
-            self._content._type(typestrs),
+            self._content.type,
             self._size,
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         )
 
     def __eq__(self, other):
         if isinstance(other, RegularForm):
             return (
                 self._form_key == other._form_key
                 and self._size == other._size
```

### Comparing `awkward-2.2.0/src/awkward/forms/unionform.py` & `awkward-2.2.1/src/awkward/forms/unionform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections import Counter
 from collections.abc import Iterable
 
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class UnionForm(Form):
     is_union = True
 
@@ -64,27 +63,27 @@
 
     @property
     def contents(self):
         return self._contents
 
     def copy(
         self,
-        tags=unset,
-        index=unset,
-        contents=unset,
+        tags=UNSET,
+        index=UNSET,
+        contents=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return UnionForm(
-            self._tags if tags is unset else tags,
-            self._index if index is unset else index,
-            self._contents if contents is unset else contents,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._tags if tags is UNSET else tags,
+            self._index if index is UNSET else index,
+            self._contents if contents is UNSET else contents,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         tags,
         index,
@@ -129,19 +128,19 @@
                     content._to_dict_part(verbose, toplevel=False)
                     for content in self._contents
                 ],
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.UnionType(
-            [x._type(typestrs) for x in self._contents],
+            [x.type for x in self._contents],
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         )
 
     def __eq__(self, other):
         if (
             isinstance(other, UnionForm)
             and self._form_key == other._form_key
             and self._tags == other._tags
```

### Comparing `awkward-2.2.0/src/awkward/forms/unmaskedform.py` & `awkward-2.2.1/src/awkward/forms/unmaskedform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
-from awkward._behavior import find_typestr
 from awkward._parameters import parameters_union, type_parameters_equal
 from awkward._typing import final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class UnmaskedForm(Form):
     is_option = True
 
@@ -30,23 +29,23 @@
 
     @property
     def content(self):
         return self._content
 
     def copy(
         self,
-        content=unset,
+        content=UNSET,
         *,
-        parameters=unset,
-        form_key=unset,
+        parameters=UNSET,
+        form_key=UNSET,
     ):
         return UnmaskedForm(
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            form_key=self._form_key if form_key is unset else form_key,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            form_key=self._form_key if form_key is UNSET else form_key,
         )
 
     @classmethod
     def simplified(
         cls,
         content,
         *,
@@ -74,19 +73,19 @@
             {
                 "class": "UnmaskedArray",
                 "content": self._content._to_dict_part(verbose, toplevel=False),
             },
             verbose,
         )
 
-    def _type(self, typestrs):
+    @property
+    def type(self):
         return ak.types.OptionType(
-            self._content._type(typestrs),
+            self._content.type,
             parameters=self._parameters,
-            typestr=find_typestr(self._parameters, typestrs),
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, UnmaskedForm):
             return (
                 self._form_key == other._form_key
                 and type_parameters_equal(self._parameters, other._parameters)
```

### Comparing `awkward-2.2.0/src/awkward/operations/__init__.py` & `awkward-2.2.1/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_all.py` & `awkward-2.2.1/src/awkward/operations/ak_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("all",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -82,9 +82,9 @@
     if isinstance(out, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
 @ak._connect.numpy.implements("all")
-def _nep_18_impl(a, axis=None, out=unsupported, keepdims=False, *, where=unsupported):
+def _nep_18_impl(a, axis=None, out=UNSUPPORTED, keepdims=False, *, where=UNSUPPORTED):
     return all(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_almost_equal.py` & `awkward-2.2.1/src/awkward/operations/ak_almost_equal.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,30 +60,38 @@
     def is_approx_dtype(left, right) -> bool:
         if not dtype_exact:
             for family in np.integer, np.floating:
                 if np.issubdtype(left, family):
                     return np.issubdtype(right, family)
         return left == right
 
+    def packed_list_content(layout):
+        layout = layout.to_ListOffsetArray64(False)
+        return layout.content[layout.offsets[0] : layout.offsets[-1]]
+
     def visitor(left, right) -> bool:
-        # Enforce super-canonicalisation rules
+        # First, erase indexed types!
+        if left.is_indexed and not left.is_option:
+            left = left.project()
+        if right.is_indexed and not right.is_option:
+            right = right.project()
+
+        # Simplify option types
         if left.is_option:
             left = left.to_IndexedOptionArray64()
         if right.is_option:
             right = right.to_IndexedOptionArray64()
 
-        if type(left) is not type(right):
-            if not check_regular and (
-                left.is_list and right.is_regular or left.is_regular and right.is_list
-            ):
-                left = left.to_ListOffsetArray64()
-                right = right.to_ListOffsetArray64()
-            else:
-                return False
+        # Simplify regular NumPy types
+        if left.is_numpy and left.purelist_depth > 1:
+            left = left.to_RegularArray()
+        if right.is_numpy and right.purelist_depth > 1:
+            right = right.to_RegularArray()
 
+        # Different lengths aren't equal!
         if left.length != right.length:
             return False
 
         if check_parameters and not parameters_are_equal(
             left.parameters, right.parameters
         ):
             return False
@@ -92,23 +100,37 @@
         if not (
             get_array_class(left, left_behavior)
             is get_array_class(right, right_behavior)
             or not check_parameters
         ):
             return False
 
-        if left.is_list:
-            return backend.index_nplike.array_equal(
-                left.offsets, right.offsets
-            ) and visitor(
-                left.content[: left.offsets[-1]], right.content[: right.offsets[-1]]
-            )
-        elif left.is_regular:
+        # Regular-regular
+        if left.is_regular and right.is_regular:
             return (left.size == right.size) and visitor(left.content, right.content)
-        elif left.is_numpy:
+        # List-list
+        elif left.is_list and right.is_list:
+            # Mixed regular-var
+            if left.is_regular and not right.is_regular:
+                return (not check_regular) and visitor(
+                    left.content,
+                    packed_list_content(right),
+                )
+            elif right.is_regular and not left.is_regular:
+                return (not check_regular) and visitor(
+                    packed_list_content(left),
+                    right.content,
+                )
+            else:
+                return visitor(
+                    packed_list_content(left),
+                    packed_list_content(right),
+                )
+
+        elif left.is_numpy and right.is_numpy:
             # Timelike types must be exactly compared, including their units
             if (
                 np.issubdtype(left.dtype, np.datetime64)
                 or np.issubdtype(right.dtype, np.datetime64)
                 or np.issubdtype(left.dtype, np.timedelta64)
                 or np.issubdtype(right.dtype, np.timedelta64)
             ):
@@ -123,19 +145,19 @@
                     and backend.nplike.all(
                         backend.nplike.isclose(
                             left.data, right.data, rtol=rtol, atol=atol, equal_nan=False
                         )
                     )
                     and left.shape == right.shape
                 )
-        elif left.is_option:
+        elif left.is_option and right.is_option:
             return backend.index_nplike.array_equal(
-                left.index.data < 0, right.index.data < 0
-            ) and visitor(left.project().to_packed(), right.project().to_packed())
-        elif left.is_union:
+                left.mask_as_bool(True), right.mask_as_bool(True)
+            ) and visitor(left.project(), right.project())
+        elif left.is_union and right.is_union:
             # For two unions with different content orderings to match, the tags should be equal at each index
             # Therefore, we can order the contents by index appearance
             def ordered_unique_values(values):
                 # First, find unique values and their appearance (from smallest to largest)
                 # unique_index is in ascending order of `unique` value
                 (
                     unique,
@@ -159,31 +181,29 @@
             # if the two tag arrays are equivalent
             new_left_tag = left_tag_to_right_tag[left.tags.data]
             if not backend.index_nplike.all(new_left_tag == right.tags.data):
                 return False
 
             # Now project out the contents, and check for equality
             for i, j in zip(left_tag_order, right_tag_order):
-                if not visitor(
-                    left.project(i).to_packed(), right.project(j).to_packed()
-                ):
+                if not visitor(left.project(i), right.project(j)):
                     return False
             return True
 
-        elif left.is_record:
+        elif left.is_record and right.is_record:
             return (
                 (
                     get_record_class(left, left_behavior)
                     is get_record_class(right, right_behavior)
                     or not check_parameters
                 )
                 and left.is_tuple == right.is_tuple
                 and (left.is_tuple or (len(left.fields) == len(right.fields)))
                 and all(visitor(left.content(f), right.content(f)) for f in left.fields)
             )
-        elif left.is_unknown:
+        elif left.is_unknown and right.is_unknown:
             return True
 
         else:
-            raise AssertionError
+            return False
 
     return visitor(left, right)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_any.py` & `awkward-2.2.1/src/awkward/operations/ak_count_nonzero.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("any",)
+__all__ = ("count_nonzero",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def any(
+def count_nonzero(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
     behavior=None,
@@ -35,28 +34,30 @@
             None (an option type); otherwise, reducing over empty lists
             results in the operation's identity.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
-    Returns True in each group of elements from `array` (many types supported,
-    including all Awkward Arrays and Records) if any values are True; False
-    otherwise. Thus, it represents reduction over the "logical or" operation,
-    whose identity is False (i.e. asking if there are any True values in an
-    empty list results in False). This operation is the same as NumPy's
-    [any](https://docs.scipy.org/doc/numpy/reference/generated/numpy.any.html)
+    Counts nonzero elements of `array` (many types supported, including all
+    Awkward Arrays and Records). The identity of counting is `0` and it is
+    usually not masked. This operation is the same as NumPy's
+    [count_nonzero](https://docs.scipy.org/doc/numpy/reference/generated/numpy.count_nonzero.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
+
+    Following the same rules as other reducers, #ak.count_nonzero does not
+    count None values. If it is desirable to count them, use #ak.fill_none
+    to turn them into something that would be counted.
     """
     with ak._errors.OperationErrorContext(
-        "ak.any",
+        "ak.count_nonzero",
         {
             "array": array,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
             "highlevel": highlevel,
             "behavior": behavior,
@@ -65,15 +66,15 @@
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
-    reducer = ak._reducers.Any()
+    reducer = ak._reducers.CountNonzero()
 
     out = ak._do.reduce(
         layout,
         reducer,
         axis=axis,
         mask=mask_identity,
         keepdims=keepdims,
@@ -81,10 +82,10 @@
     )
     if isinstance(out, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
-@ak._connect.numpy.implements("any")
-def _nep_18_impl(a, axis=None, out=unsupported, keepdims=False, *, where=unsupported):
-    return any(a, axis=axis, keepdims=keepdims)
+@ak._connect.numpy.implements("count_nonzero")
+def _nep_18_impl(a, axis=None, *, keepdims=False):
+    return count_nonzero(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_argcartesian.py` & `awkward-2.2.1/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_argcombinations.py` & `awkward-2.2.1/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_argmax.py` & `awkward-2.2.1/src/awkward/operations/ak_argmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argmax",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -144,14 +144,14 @@
     if isinstance(out, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
 @ak._connect.numpy.implements("argmax")
-def _nep_18_impl_argmax(a, axis=None, out=unsupported, *, keepdims=False):
+def _nep_18_impl_argmax(a, axis=None, out=UNSUPPORTED, *, keepdims=False):
     return argmax(a, axis=axis, keepdims=keepdims)
 
 
 @ak._connect.numpy.implements("nanargmax")
-def _nep_18_impl_nanargmax(a, axis=None, out=unsupported, *, keepdims=False):
+def _nep_18_impl_nanargmax(a, axis=None, out=UNSUPPORTED, *, keepdims=False):
     return nanargmax(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_argmin.py` & `awkward-2.2.1/src/awkward/operations/ak_argmin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argmin",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -143,14 +143,14 @@
     if isinstance(out, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
 @ak._connect.numpy.implements("argmin")
-def _nep_18_impl_argmin(a, axis=None, out=unsupported, *, keepdims=False):
+def _nep_18_impl_argmin(a, axis=None, out=UNSUPPORTED, *, keepdims=False):
     return argmin(a, axis=axis, keepdims=keepdims)
 
 
 @ak._connect.numpy.implements("nanargmin")
-def _nep_18_impl_nanargmin(a, axis=None, out=unsupported, *, keepdims=False):
+def _nep_18_impl_nanargmin(a, axis=None, out=UNSUPPORTED, *, keepdims=False):
     return nanargmin(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_argsort.py` & `awkward-2.2.1/src/awkward/operations/ak_argsort.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argsort",)
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -65,15 +65,15 @@
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.argsort(layout, axis, ascending, stable)
     return wrap_layout(out, behavior, highlevel, like=array)
 
 
 @ak._connect.numpy.implements("argsort")
-def _nep_18_impl(a, axis=-1, kind=None, order=unsupported):
+def _nep_18_impl(a, axis=-1, kind=None, order=UNSUPPORTED):
     if kind is None:
         stable = False
     elif kind in ("stable", "mergesort"):
         stable = True
     elif kind in ("heapsort", "quicksort"):
         stable = False
     else:
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_backend.py` & `awkward-2.2.1/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.2.1/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("broadcast_arrays",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
@@ -245,9 +245,9 @@
         numpy_to_regular=True,
     )
     assert isinstance(out, tuple)
     return [wrap_layout(x, behavior, highlevel) for x in out]
 
 
 @ak._connect.numpy.implements("broadcast_arrays")
-def _nep_18_impl(*args, subok=unsupported):
+def _nep_18_impl(*args, subok=UNSUPPORTED):
     return broadcast_arrays(*args)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.2.1/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_cartesian.py` & `awkward-2.2.1/src/awkward/operations/ak_cartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_categories.py` & `awkward-2.2.1/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_combinations.py` & `awkward-2.2.1/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_concatenate.py` & `awkward-2.2.1/src/awkward/operations/ak_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_copy.py` & `awkward-2.2.1/src/awkward/operations/ak_copy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("copy",)
 
 import copy as _copy
 
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 def copy(array):
     """
@@ -66,9 +66,9 @@
 
 
 def _impl(array):
     return _copy.deepcopy(array)
 
 
 @ak._connect.numpy.implements("copy")
-def _nep_18_impl(a, order=unsupported, subok=unsupported):
+def _nep_18_impl(a, order=UNSUPPORTED, subok=UNSUPPORTED):
     return copy(a)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_corr.py` & `awkward-2.2.1/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_count.py` & `awkward-2.2.1/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.2.1/src/awkward/operations/ak_any.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("count_nonzero",)
+__all__ = ("any",)
 import awkward as ak
 from awkward._behavior import behavior_of
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
-def count_nonzero(
+def any(
     array,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     highlevel=True,
     behavior=None,
@@ -34,30 +35,28 @@
             None (an option type); otherwise, reducing over empty lists
             results in the operation's identity.
         highlevel (bool): If True, return an #ak.Array; otherwise, return
             a low-level #ak.contents.Content subclass.
         behavior (None or dict): Custom #ak.behavior for the output array, if
             high-level.
 
-    Counts nonzero elements of `array` (many types supported, including all
-    Awkward Arrays and Records). The identity of counting is `0` and it is
-    usually not masked. This operation is the same as NumPy's
-    [count_nonzero](https://docs.scipy.org/doc/numpy/reference/generated/numpy.count_nonzero.html)
+    Returns True in each group of elements from `array` (many types supported,
+    including all Awkward Arrays and Records) if any values are True; False
+    otherwise. Thus, it represents reduction over the "logical or" operation,
+    whose identity is False (i.e. asking if there are any True values in an
+    empty list results in False). This operation is the same as NumPy's
+    [any](https://docs.scipy.org/doc/numpy/reference/generated/numpy.any.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
     See #ak.sum for a more complete description of nested list and missing
     value (None) handling in reducers.
-
-    Following the same rules as other reducers, #ak.count_nonzero does not
-    count None values. If it is desirable to count them, use #ak.fill_none
-    to turn them into something that would be counted.
     """
     with ak._errors.OperationErrorContext(
-        "ak.count_nonzero",
+        "ak.any",
         {
             "array": array,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
             "highlevel": highlevel,
             "behavior": behavior,
@@ -66,15 +65,15 @@
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     behavior = behavior_of(array, behavior=behavior)
-    reducer = ak._reducers.CountNonzero()
+    reducer = ak._reducers.Any()
 
     out = ak._do.reduce(
         layout,
         reducer,
         axis=axis,
         mask=mask_identity,
         keepdims=keepdims,
@@ -82,10 +81,10 @@
     )
     if isinstance(out, (ak.contents.Content, ak.record.Record)):
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
-@ak._connect.numpy.implements("count_nonzero")
-def _nep_18_impl(a, axis=None, *, keepdims=False):
-    return count_nonzero(a, axis=axis, keepdims=keepdims)
+@ak._connect.numpy.implements("any")
+def _nep_18_impl(a, axis=None, out=UNSUPPORTED, keepdims=False, *, where=UNSUPPORTED):
+    return any(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_covar.py` & `awkward-2.2.1/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_drop_none.py` & `awkward-2.2.1/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_enforce_type.py` & `awkward-2.2.1/src/awkward/operations/ak_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_fields.py` & `awkward-2.2.1/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_fill_none.py` & `awkward-2.2.1/src/awkward/operations/ak_fill_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_firsts.py` & `awkward-2.2.1/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_flatten.py` & `awkward-2.2.1/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_arrow.py` & `awkward-2.2.1/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.2.1/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.2.1/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_buffers.py` & `awkward-2.2.1/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_categorical.py` & `awkward-2.2.1/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_cupy.py` & `awkward-2.2.1/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_iter.py` & `awkward-2.2.1/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_jax.py` & `awkward-2.2.1/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_json.py` & `awkward-2.2.1/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_numpy.py` & `awkward-2.2.1/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_parquet.py` & `awkward-2.2.1/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.2.1/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_from_regular.py` & `awkward-2.2.1/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_full_like.py` & `awkward-2.2.1/src/awkward/operations/ak_full_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("full_like",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.typetracer import ensure_known_scalar
 from awkward.operations.ak_zeros_like import _ZEROS
 
 np = NumpyMetadata.instance()
 
@@ -209,10 +209,10 @@
 
     out = ak._do.recursively_apply(layout, action, behavior)
     return wrap_layout(out, behavior, highlevel)
 
 
 @ak._connect.numpy.implements("full_like")
 def _nep_18_impl(
-    a, fill_value, dtype=None, order=unsupported, subok=unsupported, shape=unsupported
+    a, fill_value, dtype=None, order=UNSUPPORTED, subok=UNSUPPORTED, shape=UNSUPPORTED
 ):
     return full_like(a, fill_value=fill_value, dtype=dtype)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_is_categorical.py` & `awkward-2.2.1/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_is_none.py` & `awkward-2.2.1/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_is_tuple.py` & `awkward-2.2.1/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_is_valid.py` & `awkward-2.2.1/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_isclose.py` & `awkward-2.2.1/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_linear_fit.py` & `awkward-2.2.1/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_local_index.py` & `awkward-2.2.1/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_mask.py` & `awkward-2.2.1/src/awkward/operations/ak_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 def _impl(array, mask, valid_when, highlevel, behavior):
     def action(inputs, backend, **kwargs):
         layoutarray, layoutmask = inputs
         if isinstance(layoutmask, ak.contents.NumpyArray):
             m = backend.nplike.asarray(layoutmask)
             if not issubclass(m.dtype.type, (bool, np.bool_)):
-                raise ValueError(f"mask must have boolean type, not {repr(m.dtype)}")
+                raise ValueError(f"mask must have boolean type, not {m.dtype!r}")
             bytemask = ak.index.Index8(m.view(np.int8))
             return (
                 ak.contents.ByteMaskedArray.simplified(
                     bytemask, layoutarray, valid_when=valid_when
                 ),
             )
         else:
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_max.py` & `awkward-2.2.1/src/awkward/operations/ak_max.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("max",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -165,17 +165,17 @@
         return wrap_layout(out, behavior, highlevel)
     else:
         return out
 
 
 @ak._connect.numpy.implements("amax")
 def _nep_18_impl_amax(
-    a, axis=None, out=unsupported, keepdims=False, initial=None, where=unsupported
+    a, axis=None, out=UNSUPPORTED, keepdims=False, initial=None, where=UNSUPPORTED
 ):
     return max(a, axis=axis, keepdims=keepdims, initial=initial)
 
 
 @ak._connect.numpy.implements("nanmax")
 def _nep_18_impl_nanmax(
-    a, axis=None, out=unsupported, keepdims=False, initial=None, where=unsupported
+    a, axis=None, out=UNSUPPORTED, keepdims=False, initial=None, where=UNSUPPORTED
 ):
     return nanmax(a, axis=axis, keepdims=keepdims, initial=initial)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_mean.py` & `awkward-2.2.1/src/awkward/operations/ak_mean.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("mean",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -214,27 +214,27 @@
         return out
 
 
 @ak._connect.numpy.implements("mean")
 def _nep_18_impl_mean(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return mean(a, axis=axis, keepdims=keepdims)
 
 
 @ak._connect.numpy.implements("nanmean")
 def _nep_18_impl_nanmean(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return nanmean(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.2.1/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.2.1/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.2.1/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_min.py` & `awkward-2.2.1/src/awkward/operations/ak_min.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("min",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -165,25 +165,25 @@
         return out
 
 
 @ak._connect.numpy.implements("amin")
 def _nep_18_impl_amin(
     a,
     axis=None,
-    out=unsupported,
+    out=UNSUPPORTED,
     keepdims=False,
     initial=None,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return min(a, axis=axis, keepdims=keepdims, initial=initial)
 
 
 @ak._connect.numpy.implements("nanmin")
 def _nep_18_impl_nanmin(
     a,
     axis=None,
-    out=unsupported,
+    out=UNSUPPORTED,
     keepdims=False,
     initial=None,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return nanmin(a, axis=axis, keepdims=keepdims, initial=initial)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_moment.py` & `awkward-2.2.1/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.2.1/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.2.1/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_num.py` & `awkward-2.2.1/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_ones_like.py` & `awkward-2.2.1/src/awkward/operations/ak_ones_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ones_like",)
 
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 def ones_like(
     array, *, dtype=None, including_unknown=False, highlevel=True, behavior=None
@@ -47,10 +47,10 @@
     return ak.operations.ak_full_like._impl(
         array, 1, highlevel, behavior, dtype, including_unknown
     )
 
 
 @ak._connect.numpy.implements("ones_like")
 def _nep_18_impl(
-    a, dtype=None, order=unsupported, subok=unsupported, shape=unsupported
+    a, dtype=None, order=UNSUPPORTED, subok=UNSUPPORTED, shape=UNSUPPORTED
 ):
     return ones_like(a, dtype=dtype)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_pad_none.py` & `awkward-2.2.1/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_parameters.py` & `awkward-2.2.1/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_prod.py` & `awkward-2.2.1/src/awkward/operations/ak_prod.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("prod",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -136,27 +136,27 @@
         return out
 
 
 @ak._connect.numpy.implements("prod")
 def _nep_18_impl_prod(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
-    initial=unsupported,
-    where=unsupported,
+    initial=UNSUPPORTED,
+    where=UNSUPPORTED,
 ):
     return prod(a, axis=axis, keepdims=keepdims)
 
 
 @ak._connect.numpy.implements("nanprod")
 def _nep_18_impl_nanprod(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
-    initial=unsupported,
-    where=unsupported,
+    initial=UNSUPPORTED,
+    where=UNSUPPORTED,
 ):
     return nanprod(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_ptp.py` & `awkward-2.2.1/src/awkward/operations/ak_ptp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ptp",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -109,9 +109,9 @@
                 posaxis = maybe_posaxis(out.layout, axis, 1)
                 out = out[(slice(None, None),) * posaxis + (0,)]
 
         return out
 
 
 @ak._connect.numpy.implements("ptp")
-def _nep_18_impl(a, axis=None, out=unsupported, keepdims=False):
+def _nep_18_impl(a, axis=None, out=UNSUPPORTED, keepdims=False):
     return ptp(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_ravel.py` & `awkward-2.2.1/src/awkward/operations/ak_ravel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("ravel",)
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 def ravel(array, *, highlevel=True, behavior=None):
@@ -66,9 +66,9 @@
 
     result = ak._do.mergemany(out)
 
     return wrap_layout(result, behavior, highlevel, like=array)
 
 
 @ak._connect.numpy.implements("ravel")
-def _nep_18_impl(a, order=unsupported):
+def _nep_18_impl(a, order=UNSUPPORTED):
     return ravel(a)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_run_lengths.py` & `awkward-2.2.1/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_singletons.py` & `awkward-2.2.1/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_softmax.py` & `awkward-2.2.1/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_sort.py` & `awkward-2.2.1/src/awkward/operations/ak_sort.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("sort",)
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -52,15 +52,15 @@
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.sort(layout, axis, ascending, stable)
     return wrap_layout(out, behavior, highlevel, like=array)
 
 
 @ak._connect.numpy.implements("sort")
-def _nep_18_impl(a, axis=-1, kind=None, order=unsupported):
+def _nep_18_impl(a, axis=-1, kind=None, order=UNSUPPORTED):
     if kind is None:
         stable = False
     elif kind in ("stable", "mergesort"):
         stable = True
     elif kind in ("heapsort", "quicksort"):
         stable = False
     else:
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_std.py` & `awkward-2.2.1/src/awkward/operations/ak_std.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("std",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
@@ -177,29 +177,29 @@
         return out
 
 
 @ak._connect.numpy.implements("std")
 def _nep_18_impl_std(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     ddof=0,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return std(a, axis=axis, keepdims=keepdims, ddof=ddof)
 
 
 @ak._connect.numpy.implements("nanstd")
 def _nep_18_impl_nanstd(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     ddof=0,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return nanstd(a, axis=axis, keepdims=keepdims, ddof=ddof)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_strings_astype.py` & `awkward-2.2.1/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_sum.py` & `awkward-2.2.1/src/awkward/operations/ak_sum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("sum",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -284,27 +284,27 @@
         return out
 
 
 @ak._connect.numpy.implements("sum")
 def _nep_18_impl_sum(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
-    initial=unsupported,
-    where=unsupported,
+    initial=UNSUPPORTED,
+    where=UNSUPPORTED,
 ):
     return sum(a, axis=axis, keepdims=keepdims)
 
 
 @ak._connect.numpy.implements("nansum")
 def _nep_18_impl_nansum(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     keepdims=False,
-    initial=unsupported,
-    where=unsupported,
+    initial=UNSUPPORTED,
+    where=UNSUPPORTED,
 ):
     return nansum(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_arrow.py` & `awkward-2.2.1/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.2.1/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_backend.py` & `awkward-2.2.1/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_buffers.py` & `awkward-2.2.1/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_categorical.py` & `awkward-2.2.1/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_cupy.py` & `awkward-2.2.1/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.2.1/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_jax.py` & `awkward-2.2.1/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_json.py` & `awkward-2.2.1/src/awkward/operations/ak_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     elif isinstance(array, ak.contents.Content):
         out = array
 
     elif hasattr(array, "shape") and hasattr(array, "dtype"):
         out = ak.contents.NumpyArray(array)
 
     else:
-        raise TypeError(f"unrecognized array type: {repr(array)}")
+        raise TypeError(f"unrecognized array type: {array!r}")
 
     jsondata = out.to_json(
         nan_string=nan_string,
         posinf_string=posinf_string,
         neginf_string=neginf_string,
         complex_record_fields=complex_record_fields,
         convert_bytes=convert_bytes,
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_layout.py` & `awkward-2.2.1/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_list.py` & `awkward-2.2.1/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_numpy.py` & `awkward-2.2.1/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_packed.py` & `awkward-2.2.1/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_parquet.py` & `awkward-2.2.1/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.2.1/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_to_regular.py` & `awkward-2.2.1/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_transform.py` & `awkward-2.2.1/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_type.py` & `awkward-2.2.1/src/awkward/operations/ak_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -81,52 +81,52 @@
 
 
 def _impl(array, behavior):
     behavior = behavior_of(array, behavior=behavior)
 
     if isinstance(array, _ext.ArrayBuilder):
         form = ak.forms.from_json(array.form())
-        return ak.types.ArrayType(form.type_from_behavior(behavior), len(array))
+        return ak.types.ArrayType(form.type, len(array), behavior=behavior)
 
     elif isinstance(array, ak.record.Record):
-        return ak.types.ScalarType(array.array.form.type_from_behavior(behavior))
+        return ak.types.ScalarType(array.array.form.type, behavior=behavior)
 
     elif isinstance(array, ak.contents.Content):
-        return ak.types.ArrayType(array.form.type_from_behavior(behavior), array.length)
+        return ak.types.ArrayType(array.form.type, array.length, behavior=behavior)
 
     elif isinstance(array, (np.dtype, np.generic)):
         return ak.types.ScalarType(
             ak.types.NumpyType(ak.types.numpytype.dtype_to_primitive(np.dtype(array)))
         )
 
     elif isinstance(array, bool):  # np.bool_ in np.generic (above)
-        return ak.types.ScalarType(ak.types.NumpyType("bool"))
+        return ak.types.ScalarType(ak.types.NumpyType("bool"), behavior=behavior)
 
     elif isinstance(array, numbers.Integral):
-        return ak.types.ScalarType(ak.types.NumpyType("int64"))
+        return ak.types.ScalarType(ak.types.NumpyType("int64"), behavior=behavior)
 
     elif isinstance(array, numbers.Real):
-        return ak.types.ScalarType(ak.types.NumpyType("float64"))
+        return ak.types.ScalarType(ak.types.NumpyType("float64"), behavior=behavior)
 
     elif isinstance(array, numbers.Complex):
-        return ak.types.ScalarType(ak.types.NumpyType("complex128"))
+        return ak.types.ScalarType(ak.types.NumpyType("complex128"), behavior=behavior)
 
     elif isinstance(array, datetime):  # np.datetime64 in np.generic (above)
-        return ak.types.ScalarType(ak.types.NumpyType("datetime64"))
+        return ak.types.ScalarType(ak.types.NumpyType("datetime64"), behavior=behavior)
 
     elif isinstance(array, timedelta):  # np.timedelta64 in np.generic (above)
-        return ak.types.ScalarType(ak.types.NumpyType("timedelta"))
+        return ak.types.ScalarType(ak.types.NumpyType("timedelta"), behavior=behavior)
 
     elif isinstance(array, ak.highlevel.ArrayBuilder):
         # Don't go through `to_layout`: we want to avoid snapshotting this array
         return _impl(array._layout, behavior)
 
     else:
         layout = ak.to_layout(array, allow_other=True, allow_record=True)
         if layout is None:
-            return ak.types.ScalarType(ak.types.UnknownType())
+            return ak.types.ScalarType(ak.types.UnknownType(), behavior=behavior)
 
         elif isinstance(layout, (ak.contents.Content, ak.record.Record)):
             return _impl(layout, behavior)
 
         else:
             raise TypeError(f"unrecognized array type: {array!r}")
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_unflatten.py` & `awkward-2.2.1/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_unzip.py` & `awkward-2.2.1/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_validity_error.py` & `awkward-2.2.1/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_values_astype.py` & `awkward-2.2.1/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_var.py` & `awkward-2.2.1/src/awkward/operations/ak_var.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("var",)
 import awkward as ak
 from awkward._behavior import behavior_of
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
 
 
@@ -213,29 +213,29 @@
         return out
 
 
 @ak._connect.numpy.implements("var")
 def _nep_18_impl_var(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     ddof=0,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return var(a, axis=axis, keepdims=keepdims, ddof=ddof)
 
 
 @ak._connect.numpy.implements("nanvar")
 def _nep_18_impl_nanvar(
     a,
     axis=None,
-    dtype=unsupported,
-    out=unsupported,
+    dtype=UNSUPPORTED,
+    out=UNSUPPORTED,
     ddof=0,
     keepdims=False,
     *,
-    where=unsupported,
+    where=UNSUPPORTED,
 ):
     return nanvar(a, axis=axis, keepdims=keepdims, ddof=ddof)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_where.py` & `awkward-2.2.1/src/awkward/operations/ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_with_field.py` & `awkward-2.2.1/src/awkward/operations/ak_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_with_name.py` & `awkward-2.2.1/src/awkward/operations/ak_with_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,19 @@
 
 def _impl(array, name, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array)
 
     def action(layout, **ignore):
         if isinstance(layout, ak.contents.RecordArray):
-            parameters = dict(layout.parameters)
-            parameters["__record__"] = name
             return ak.contents.RecordArray(
-                layout.contents, layout.fields, layout.length, parameters=parameters
+                layout._contents,
+                layout._fields,
+                layout._length,
+                parameters={**layout.parameters, "__record__": name},
             )
         else:
             return None
 
     out = ak._do.recursively_apply(layout, action, behavior)
 
     def action2(layout, **ignore):
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_with_parameter.py` & `awkward-2.2.1/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_without_field.py` & `awkward-2.2.1/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_without_parameters.py` & `awkward-2.2.1/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/operations/ak_zeros_like.py` & `awkward-2.2.1/src/awkward/operations/ak_zeros_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("zeros_like",)
 
 import awkward as ak
-from awkward._connect.numpy import unsupported
+from awkward._connect.numpy import UNSUPPORTED
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 _ZEROS = object()
 
@@ -54,10 +54,10 @@
     return ak.operations.ak_full_like._impl(
         array, _ZEROS, highlevel, behavior, dtype, including_unknown
     )
 
 
 @ak._connect.numpy.implements("zeros_like")
 def _nep_18_impl(
-    a, dtype=None, order=unsupported, subok=unsupported, shape=unsupported
+    a, dtype=None, order=UNSUPPORTED, subok=UNSUPPORTED, shape=UNSUPPORTED
 ):
     return zeros_like(a, dtype=dtype)
```

### Comparing `awkward-2.2.0/src/awkward/operations/ak_zip.py` & `awkward-2.2.1/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/types/__init__.py` & `awkward-2.2.1/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.2.1/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/src/awkward/types/arraytype.py` & `awkward-2.2.1/src/awkward/types/arraytype.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,61 @@
 
 import awkward as ak
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
 
 
 class ArrayType:
-    def __init__(self, content, length):
+    def __init__(self, content, length, behavior=None):
         if not isinstance(content, ak.types.Type):
             raise TypeError(
                 "{} all 'contents' must be Type subclasses, not {}".format(
                     type(self).__name__, repr(content)
                 )
             )
         if not ((is_integer(length) and length >= 0) or length is unknown_length):
             raise ValueError(
                 "{} 'length' must be a non-negative integer or unknown length, not {}".format(
                     type(self).__name__, repr(length)
                 )
             )
         self._content = content
         self._length = length
+        self._behavior = behavior
 
     @property
     def content(self):
         return self._content
 
     @property
     def length(self):
         return self._length
 
+    @property
+    def behavior(self):
+        return self._behavior
+
     def __str__(self):
         return "".join(self._str("", True))
 
     def show(self, stream=sys.stdout):
         stream.write("".join([*self._str("", False), "\n"]))
 
     def _str(self, indent, compact):
-        return [f"{self._length} * ", *self._content._str(indent, compact)]
+        return [
+            f"{self._length} * ",
+            *self._content._str(
+                indent,
+                compact,
+                self._behavior,
+            ),
+        ]
 
     def __repr__(self):
-        args = [repr(self._content), repr(self._length)]
+        args = [repr(self._content), repr(self._length), repr(self._behavior)]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def is_equal_to(self, other, *, all_parameters: bool = False) -> bool:
         return (
             isinstance(other, type(self))
             and (
                 other._length is unknown_length
```

### Comparing `awkward-2.2.0/src/awkward/types/listtype.py` & `awkward-2.2.1/src/awkward/types/unknowntype.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,67 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
+from awkward._behavior import find_array_typestr
+from awkward._errors import deprecate
 from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.type import Type
 
 
 @final
-class ListType(Type):
-    def copy(self, *, content: Type = unset, parameters=unset, typestr=unset) -> Self:
-        return ListType(
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+class UnknownType(Type):
+    def copy(self, *, parameters=UNSET, typestr=UNSET) -> Self:
+        return UnknownType(
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
-    def __init__(self, content, *, parameters=None, typestr=None):
-        if not isinstance(content, Type):
-            raise TypeError(
-                "{} 'content' must be a Type subtype, not {}".format(
-                    type(self).__name__, repr(content)
-                )
+    def __init__(self, *, parameters=None, typestr=None):
+        if parameters is not None:
+            deprecate(
+                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         if parameters is not None and not isinstance(parameters, dict):
             raise TypeError(
                 "{} 'parameters' must be of type dict or None, not {}".format(
                     type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
             raise TypeError(
                 "{} 'typestr' must be of type string or None, not {}".format(
                     type(self).__name__, repr(typestr)
                 )
             )
-        self._content = content
         self._parameters = parameters
         self._typestr = typestr
 
-    @property
-    def content(self):
-        return self._content
-
-    def _str(self, indent, compact):
+    def _str(self, indent, compact, behavior):
         if self._typestr is not None:
-            out = [self._typestr]
-
-        elif self.parameter("__array__") == "string":
-            out = ["string"]
+            deprecate("typestr argument is deprecated", "2.4.0")
 
-        elif self.parameter("__array__") == "bytestring":
-            out = ["bytes"]
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            out = [typestr]
 
         else:
             params = self._str_parameters()
             if params is None:
-                out = ["var * ", *self._content._str(indent, compact)]
+                out = ["unknown"]
             else:
-                out = ["[var * ", *self._content._str(indent, compact)] + [
-                    f", {params}]"
-                ]
+                out = ["unknown[", params, "]"]
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
-        args = [repr(self._content), *self._repr_args()]
+        args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
         compare_parameters = (
             parameters_are_equal if all_parameters else type_parameters_equal
         )
-        return (
-            isinstance(other, type(self))
-            and compare_parameters(self._parameters, other._parameters)
-            and self._content == other._content
+        return isinstance(other, type(self)) and compare_parameters(
+            self._parameters, other._parameters
         )
```

### Comparing `awkward-2.2.0/src/awkward/types/numpytype.py` & `awkward-2.2.1/src/awkward/types/numpytype.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import json
 import re
 
+from awkward._behavior import find_array_typestr
+from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.type import Type
 
 np = NumpyMetadata.instance()
 
 
 def is_primitive(primitive):
     if _primitive_to_dtype_datetime.match(primitive) is not None:
@@ -89,19 +91,19 @@
 _dtype_to_primitive_dict = {}
 for primitive, dtype in _primitive_to_dtype_dict.items():
     _dtype_to_primitive_dict[dtype] = primitive
 
 
 @final
 class NumpyType(Type):
-    def copy(self, *, primitive: Type = unset, parameters=unset, typestr=unset) -> Self:
+    def copy(self, *, primitive: Type = UNSET, parameters=UNSET, typestr=UNSET) -> Self:
         return NumpyType(
-            self._primitive if primitive is unset else primitive,
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+            self._primitive if primitive is UNSET else primitive,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
     def __init__(self, primitive, *, parameters=None, typestr=None):
         primitive = dtype_to_primitive(primitive_to_dtype(primitive))
         if parameters is not None and not isinstance(parameters, dict):
             raise TypeError(
                 "{} 'parameters' must be of type dict or None, not {}".format(
@@ -120,23 +122,21 @@
 
     @property
     def primitive(self):
         return self._primitive
 
     _str_parameters_exclude = ("__categorical__", "__unit__")
 
-    def _str(self, indent, compact):
+    def _str(self, indent, compact, behavior):
         if self._typestr is not None:
-            out = [self._typestr]
+            deprecate("typestr argument is deprecated", "2.4.0")
 
-        elif self.parameter("__array__") == "char":
-            out = ["char"]
-
-        elif self.parameter("__array__") == "byte":
-            out = ["byte"]
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            out = [typestr]
 
         else:
             if self.parameter("__unit__") is not None:
                 numpy_unit = str(np.dtype("M8[" + self._parameters["__unit__"] + "]"))
                 bracket_index = numpy_unit.index("[")
                 units = "unit=" + json.dumps(numpy_unit[bracket_index + 1 : -1])
             else:
```

### Comparing `awkward-2.2.0/src/awkward/types/optiontype.py` & `awkward-2.2.1/src/awkward/types/optiontype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
+from awkward._behavior import find_array_typestr
+from awkward._errors import deprecate
 from awkward._parameters import (
     parameters_are_equal,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.listtype import ListType
 from awkward.types.regulartype import RegularType
 from awkward.types.type import Type
 from awkward.types.uniontype import UnionType
 
 
 @final
 class OptionType(Type):
-    def copy(self, *, content: Type = unset, parameters=unset, typestr=unset) -> Self:
+    def copy(self, *, content: Type = UNSET, parameters=UNSET, typestr=UNSET) -> Self:
         return OptionType(
-            self._content if content is unset else content,
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
     def __init__(self, content, *, parameters=None, typestr=None):
         if not isinstance(content, Type):
             raise TypeError(
                 "{} 'content' must be a Type subclass, not {}".format(
                     type(self).__name__, repr(content)
@@ -46,22 +48,27 @@
         self._parameters = parameters
         self._typestr = typestr
 
     @property
     def content(self):
         return self._content
 
-    def _str(self, indent, compact):
+    def _str(self, indent, compact, behavior):
+        if self._typestr is not None:
+            deprecate("typestr argument is deprecated", "2.4.0")
+
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+
         head = []
         tail = []
-        if self._typestr is not None:
-            content_out = [self._typestr]
+        if typestr is not None:
+            content_out = [typestr]
 
         else:
-            content_out = self._content._str(indent, compact)
+            content_out = self._content._str(indent, compact, behavior)
             params = self._str_parameters()
             if params is None:
                 if isinstance(
                     self._content, (RegularType, ListType)
                 ) and self._content.parameter("__array__") not in (
                     "string",
                     "bytestring",
```

### Comparing `awkward-2.2.0/src/awkward/types/recordtype.py` & `awkward-2.2.1/src/awkward/types/recordtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 
 import json
 from collections.abc import Iterable
 from itertools import permutations
 
 import awkward as ak
 import awkward._prettyprint
+from awkward._behavior import find_record_typestr
+from awkward._errors import deprecate
 from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.type import Type
 
 
 @final
 class RecordType(Type):
     def copy(
         self,
         *,
-        contents: list[Type] = unset,
-        fields: list[str] | None = unset,
-        parameters=unset,
-        typestr=unset,
+        contents: list[Type] = UNSET,
+        fields: list[str] | None = UNSET,
+        parameters=UNSET,
+        typestr=UNSET,
     ) -> Self:
         return RecordType(
-            self._contents if contents is unset else contents,
-            self._fields if fields is unset else fields,
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+            self._contents if contents is UNSET else contents,
+            self._fields if fields is UNSET else fields,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
     def __init__(self, contents, fields, *, parameters=None, typestr=None):
         if not isinstance(contents, Iterable):
             raise TypeError(
                 "{} 'contents' must be iterable, not {}".format(
                     type(self).__name__, repr(contents)
@@ -79,36 +81,45 @@
 
     @property
     def is_tuple(self):
         return self._fields is None
 
     _str_parameters_exclude = ("__categorical__", "__record__")
 
-    def _str(self, indent, compact):
+    def _str(self, indent, compact, behavior):
         if self._typestr is not None:
-            out = [self._typestr]
+            deprecate("typestr argument is deprecated", "2.4.0")
+
+        typestr = find_record_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            out = [typestr]
 
         else:
             if compact:
                 pre, post = "", ""
             else:
                 pre, post = "\n" + indent + "    ", "\n" + indent
 
             children = []
             for i, x in enumerate(self._contents):
                 if i + 1 < len(self._contents):
                     if compact:
-                        y = [*x._str(indent, compact), ", "]
+                        y = [*x._str(indent, compact, behavior), ", "]
                     else:
-                        y = [*x._str(indent + "    ", compact), ",\n", indent, "    "]
+                        y = [
+                            *x._str(indent + "    ", compact, behavior),
+                            ",\n",
+                            indent,
+                            "    ",
+                        ]
                 else:
                     if compact:
-                        y = x._str(indent, compact)
+                        y = x._str(indent, compact, behavior)
                     else:
-                        y = x._str(indent + "    ", compact)
+                        y = x._str(indent + "    ", compact, behavior)
                 children.append(y)
 
             params = self._str_parameters()
             name = self.parameter("__record__")
 
             if name is not None:
                 if (
```

### Comparing `awkward-2.2.0/src/awkward/types/scalartype.py` & `awkward-2.2.1/src/awkward/types/scalartype.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,38 +3,47 @@
 
 import sys
 
 import awkward as ak
 
 
 class ScalarType:
-    def __init__(self, content):
+    def __init__(self, content, behavior=None):
         if not isinstance(content, ak.types.Type):
             raise TypeError(
                 "{} all 'contents' must be Type subclasses, not {}".format(
                     type(self).__name__, repr(content)
                 )
             )
         self._content = content
+        self._behavior = behavior
 
     @property
     def content(self):
         return self._content
 
+    @property
+    def behavior(self):
+        return self._behavior
+
     def __str__(self):
         return "".join(self._str("", True))
 
     def show(self, stream=sys.stdout):
         stream.write("".join([*self._str("", False), "\n"]))
 
     def _str(self, indent, compact):
-        return self._content._str(indent, compact)
+        return self._content._str(
+            indent,
+            compact,
+            self._behavior,
+        )
 
     def __repr__(self):
-        return f"{type(self).__name__}({self._content!r})"
+        return f"{type(self).__name__}({self._content!r}, {self._behavior!r})"
 
     def is_equal_to(self, other, *, all_parameters: bool = False) -> bool:
         return isinstance(other, type(self)) and self._content.is_equal_to(
             other._content, all_parameters=all_parameters
         )
 
     __eq__ = is_equal_to
```

### Comparing `awkward-2.2.0/src/awkward/types/type.py` & `awkward-2.2.1/src/awkward/types/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import json
 import sys
 
 import awkward as ak
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Self
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types._awkward_datashape_parser import Lark_StandAlone, Transformer
 
 np = NumpyMetadata.instance()
 
 
 class Type:
-    def copy(self, *, parameters=unset, typestr=unset) -> Self:
+    def copy(self, *, parameters=UNSET, typestr=UNSET) -> Self:
         raise NotImplementedError
 
     @property
     def parameters(self):
         if self._parameters is None:  # pylint: disable=E0203
             self._parameters = {}
         return self._parameters
@@ -30,18 +30,22 @@
             return self._parameters.get(key)
 
     @property
     def typestr(self):
         return self._typestr
 
     def __str__(self):
-        return "".join(self._str("", True))
+        return "".join(self._str("", True, None))
+
+    def _str(self, indent: str, compact: bool, behavior: dict | None) -> list[str]:
+        raise NotImplementedError
 
     def show(self, stream=sys.stdout):
-        stream.write("".join([*self._str("", False), "\n"]))
+        # TODO: deprecate lowlevel show
+        stream.write("".join([*self._str("", False, None), "\n"]))
 
     _str_parameters_exclude = ("__categorical__",)
 
     def _str_categorical_begin(self):
         if self.parameter("__categorical__") is not None:
             return "categorical[type="
         else:
@@ -306,35 +310,36 @@
     Parses `datashape` (str) and returns a #ak.types.Type object, the inverse of
     calling `str` on a #ak.types.Type.
 
     If `highlevel=True`, and the type string starts with a number (e.g. '1000 * ...'),
     the return type is #ak.types.ArrayType, representing an #ak.highlevel.Array.
 
     If `highlevel=True` and the type string starts with a record indicator (e.g. `{`),
-    the return type is #ak.types.RecordType, representing an #ak.highlevel.Record,
-    rather than an array of them.
+    the return type is #ak.types.ScalarType with an #ak.types.RecordType content,
+    representing a scalar #ak.highlevel.Record rather than an array of them.
 
     Other strings (e.g. starting with `var *`, `?`, `option`, etc.) are not compatible
     with `highlevel=True`; an exception would be raised.
 
     If `highlevel=False`, the type is assumed to represent a layout (e.g. a number
     indicates a #ak.types.RegularType, rather than a #ak.types.ArrayType).
     """
     from awkward.types.arraytype import ArrayType
     from awkward.types.recordtype import RecordType
     from awkward.types.regulartype import RegularType
+    from awkward.types.scalartype import ScalarType
 
     parser = Lark_StandAlone(transformer=_DataShapeTransformer())
     out = parser.parse(datashape)
 
     if highlevel:
         if isinstance(out, RegularType):
             return ArrayType(out.content, out.size)
         elif isinstance(out, RecordType):
-            return out
+            return ScalarType(out)
         else:
             raise ValueError(
                 f"type {type(out).__name__!r} is not compatible with highlevel=True"
             )
 
     else:
         return out
```

### Comparing `awkward-2.2.0/src/awkward/types/uniontype.py` & `awkward-2.2.1/src/awkward/types/uniontype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from collections.abc import Iterable
 from itertools import permutations
 
+from awkward._behavior import find_array_typestr
+from awkward._errors import deprecate
 from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.type import Type
 
 
 @final
 class UnionType(Type):
     def copy(
-        self, *, contents: list[Type] = unset, parameters=unset, typestr=unset
+        self, *, contents: list[Type] = UNSET, parameters=UNSET, typestr=UNSET
     ) -> Self:
         return UnionType(
-            self._contents if contents is unset else contents,
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+            self._contents if contents is UNSET else contents,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
     def __init__(self, contents, *, parameters=None, typestr=None):
         if not isinstance(contents, Iterable):
             raise TypeError(
                 "{} 'contents' must be iterable, not {}".format(
                     type(self).__name__, repr(contents)
@@ -53,36 +55,45 @@
         self._parameters = parameters
         self._typestr = typestr
 
     @property
     def contents(self):
         return self._contents
 
-    def _str(self, indent, compact):
+    def _str(self, indent, compact, behavior):
         if self._typestr is not None:
-            out = [self._typestr]
+            deprecate("typestr argument is deprecated", "2.4.0")
+
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            out = [typestr]
 
         else:
             if compact:
                 pre, post = "", ""
             else:
                 pre, post = "\n" + indent + "    ", "\n" + indent
 
             children = []
             for i, x in enumerate(self._contents):
                 if i + 1 < len(self._contents):
                     if compact:
-                        y = [*x._str(indent, compact), ", "]
+                        y = [*x._str(indent, compact, behavior), ", "]
                     else:
-                        y = [*x._str(indent + "    ", compact), ",\n", indent, "    "]
+                        y = [
+                            *x._str(indent + "    ", compact, behavior),
+                            ",\n",
+                            indent,
+                            "    ",
+                        ]
                 else:
                     if compact:
-                        y = x._str(indent, compact)
+                        y = x._str(indent, compact, behavior)
                     else:
-                        y = x._str(indent + "    ", compact)
+                        y = x._str(indent + "    ", compact, behavior)
                 children.append(y)
 
             flat_children = [y for x in children for y in x]
             params = self._str_parameters()
 
             if params is None:
                 out = ["union[", pre, *flat_children] + [post, "]"]
```

### Comparing `awkward-2.2.0/src/awkward/types/unknowntype.py` & `awkward-2.2.1/src/awkward/types/listtype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
+from awkward._behavior import find_array_typestr
 from awkward._errors import deprecate
 from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._typing import Self, final
-from awkward._util import unset
+from awkward._util import UNSET
 from awkward.types.type import Type
 
 
 @final
-class UnknownType(Type):
-    def copy(self, *, parameters=unset, typestr=unset) -> Self:
-        return UnknownType(
-            parameters=self._parameters if parameters is unset else parameters,
-            typestr=self._typestr if typestr is unset else typestr,
+class ListType(Type):
+    def copy(self, *, content: Type = UNSET, parameters=UNSET, typestr=UNSET) -> Self:
+        return ListType(
+            self._content if content is UNSET else content,
+            parameters=self._parameters if parameters is UNSET else parameters,
+            typestr=self._typestr if typestr is UNSET else typestr,
         )
 
-    def __init__(self, *, parameters=None, typestr=None):
-        if parameters is not None:
-            deprecate(
-                f"{type(self).__name__} cannot contain parameters", version="2.2.0"
+    def __init__(self, content, *, parameters=None, typestr=None):
+        if not isinstance(content, Type):
+            raise TypeError(
+                "{} 'content' must be a Type subtype, not {}".format(
+                    type(self).__name__, repr(content)
+                )
             )
         if parameters is not None and not isinstance(parameters, dict):
             raise TypeError(
                 "{} 'parameters' must be of type dict or None, not {}".format(
                     type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
             raise TypeError(
                 "{} 'typestr' must be of type string or None, not {}".format(
                     type(self).__name__, repr(typestr)
                 )
             )
+        self._content = content
         self._parameters = parameters
         self._typestr = typestr
 
-    def _str(self, indent, compact):
+    @property
+    def content(self):
+        return self._content
+
+    def _str(self, indent, compact, behavior):
         if self._typestr is not None:
-            out = [self._typestr]
+            deprecate("typestr argument is deprecated", "2.4.0")
 
+        typestr = find_array_typestr(behavior, self._parameters, self._typestr)
+        if typestr is not None:
+            out = [typestr]
         else:
             params = self._str_parameters()
             if params is None:
-                out = ["unknown"]
+                out = ["var * ", *self._content._str(indent, compact, behavior)]
             else:
-                out = ["unknown[", params, "]"]
+                out = ["[var * ", *self._content._str(indent, compact, behavior)] + [
+                    f", {params}]"
+                ]
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
-        args = self._repr_args()
+        args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
         compare_parameters = (
             parameters_are_equal if all_parameters else type_parameters_equal
         )
-        return isinstance(other, type(self)) and compare_parameters(
-            self._parameters, other._parameters
+        return (
+            isinstance(other, type(self))
+            and compare_parameters(self._parameters, other._parameters)
+            and self._content == other._content
         )
```

### Comparing `awkward-2.2.0/tests/test_0002_minimal_listarray.py` & `awkward-2.2.1/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0008_slices_and_getitem.py` & `awkward-2.2.1/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0011_listarray.py` & `awkward-2.2.1/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0013_error_handling_struct.py` & `awkward-2.2.1/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0014_finish_up_getitem.py` & `awkward-2.2.1/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0018_fromiter_fillable.py` & `awkward-2.2.1/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0019_use_json_library.py` & `awkward-2.2.1/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.2.1/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0021_emptyarray.py` & `awkward-2.2.1/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0023_regular_array.py` & `awkward-2.2.1/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0024_use_regular_array.py` & `awkward-2.2.1/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0025_record_array.py` & `awkward-2.2.1/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0028_add_dressed_types.py` & `awkward-2.2.1/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0032_replace_dressedtype.py` & `awkward-2.2.1/tests/test_0032_replace_dressedtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     )
     assert str(a2[0]) == "<Dummy [1.1, 2.2, 3.3]>"
     assert str(a2[1]) == "<Dummy []>"
     assert str(a2[2]) == "<Dummy [4.4, 5.5]>"
 
 
 def test_record_name():
-    typestrs = {}
     builder = ak.highlevel.ArrayBuilder()
 
     builder.begin_record("Dummy")
     builder.field("one")
     builder.integer(1)
     builder.field("two")
     builder.real(1.1)
@@ -108,16 +107,16 @@
     builder.real(2.2)
     builder.field("one")
     builder.integer(2)
     builder.end_record()
 
     a = builder.snapshot()
 
-    assert str(a.layout.form._type(typestrs)) == "Dummy[one: int64, two: float64]"
-    assert a.layout.form._type(typestrs).parameters == {"__record__": "Dummy"}
+    assert str(a.layout.form.type) == "Dummy[one: int64, two: float64]"
+    assert a.layout.form.type.parameters == {"__record__": "Dummy"}
 
 
 def test_builder_string():
     builder = ak.ArrayBuilder()
     builder.bytestring(b"one")
     builder.bytestring(b"two")
     builder.bytestring(b"three")
```

### Comparing `awkward-2.2.0/tests/test_0046_start_indexedarray.py` & `awkward-2.2.1/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.2.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0057_introducing_forms.py` & `awkward-2.2.1/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0070_argmin_and_argmax.py` & `awkward-2.2.1/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0072_fillna_operation.py` & `awkward-2.2.1/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0074_argsort_and_sort.py` & `awkward-2.2.1/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0077_zip_operation.py` & `awkward-2.2.1/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0078_argcross_and_cross.py` & `awkward-2.2.1/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0079_argchoose_and_choose.py` & `awkward-2.2.1/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.2.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0084_start_unionarray.py` & `awkward-2.2.1/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0086_nep13_ufunc.py` & `awkward-2.2.1/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0089_numpy_functions.py` & `awkward-2.2.1/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.2.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0107_assign_fields_to_records.py` & `awkward-2.2.1/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.2.1/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0115_generic_reducer_operation.py` & `awkward-2.2.1/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0118_numba_cpointers.py` & `awkward-2.2.1/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.2.1/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0124_strings_in_numba.py` & `awkward-2.2.1/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0127_tomask_operation.py` & `awkward-2.2.1/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.2.1/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0138_emptyarray_type.py` & `awkward-2.2.1/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0150_flatten.py` & `awkward-2.2.1/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0163_negative_axis_wrap.py` & `awkward-2.2.1/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.2.1/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0173_astype_operation.py` & `awkward-2.2.1/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0184_concatenate_operation.py` & `awkward-2.2.1/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.2.1/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.2.1/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0222_count_with_axis0.py` & `awkward-2.2.1/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0224_arrow_to_awkward.py` & `awkward-2.2.1/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0264_reduce_last_empty.py` & `awkward-2.2.1/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0273_path_for_with_field.py` & `awkward-2.2.1/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.2.1/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.2.1/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0315_integerindex.py` & `awkward-2.2.1/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0331_pandas_indexedarray.py` & `awkward-2.2.1/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.2.1/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.2.1/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0348_form_keys.py` & `awkward-2.2.1/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0355_mixins.py` & `awkward-2.2.1/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0395_complex_type_arrays.py` & `awkward-2.2.1/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.2.1/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.2.1/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.2.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0404_array_validity_check.py` & `awkward-2.2.1/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.2.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.2.1/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.2.1/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.2.1/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.2.1/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0496_provide_local_index.py` & `awkward-2.2.1/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.2.1/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.2.1/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.2.1/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.2.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0549_numba_array_asarray.py` & `awkward-2.2.1/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0557_min_max_initial_argument.py` & `awkward-2.2.1/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.2.1/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0572_numba_array_ndim.py` & `awkward-2.2.1/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.2.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0583_implement_unflatten_function.py` & `awkward-2.2.1/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.2.1/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.2.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.2.1/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0674_categorical_validation.py` & `awkward-2.2.1/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.2.1/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.2.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.2.1/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0733_run_lengths.py` & `awkward-2.2.1/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.2.1/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.2.1/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0773_typeparser.py` & `awkward-2.2.1/tests/test_0773_typeparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
     assert isinstance(parsedtype, ak.types.ListType)
     assert str(parsedtype) == text
 
 
 def test_record_highlevel():
     text = "Thingy[x: int64, y: float64]"
     parsedtype = ak.types.from_datashape(text, highlevel=True)
-    assert isinstance(parsedtype, ak.types.RecordType)
+    assert isinstance(parsedtype, ak.types.ScalarType)
     assert str(parsedtype) == text
 
 
 def test_numpytype_int32():
     t = NumpyType("int32")
     assert str(ak.types.from_datashape(str(t), highlevel=False)) == str(t)
```

### Comparing `awkward-2.2.0/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.2.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.2.1/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0803_argsort_fix_type.py` & `awkward-2.2.1/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.2.1/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.2.1/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.2.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0828_arrow_datatype_null.py` & `awkward-2.2.1/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0835_datetime_type.py` & `awkward-2.2.1/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0835_datetime_type_pandas.py` & `awkward-2.2.1/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.2.1/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0850_argsort_mask_array.py` & `awkward-2.2.1/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.2.1/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0875_arrow_null_type.py` & `awkward-2.2.1/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0879_non_primitive_with_field.py` & `awkward-2.2.1/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.2.1/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0889_ptp.py` & `awkward-2.2.1/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0896_content_classes_refactoring.py` & `awkward-2.2.1/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.2.1/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.2.1/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.2.1/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.2.1/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0912_packed.py` & `awkward-2.2.1/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0914_types_and_forms.py` & `awkward-2.2.1/tests/test_0914_types_and_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,64 +2,67 @@
 
 import numpy as np
 import pytest
 
 import awkward as ak
 
 
+def assert_overrides_typestr(type_, typestr: str = "override", expected: str = None):
+    # Assume typestr is expected result
+    if expected is None:
+        expected = typestr
+    # Set appropriate array or record parameter
+    if isinstance(type_, ak.types.RecordType):
+        parameters = {**type_.parameters, "__record__": "custom"}
+    else:
+        parameters = {**type_.parameters, "__array__": "custom"}
+    behavior = {("__typestr__", "custom"): typestr}
+    # Build highlevel type with custom behavior
+    with_parameter = type_.copy(parameters=parameters)
+    as_str = "".join(with_parameter._str("", False, behavior))
+    assert as_str == expected
+
+
 def test_UnknownType():
     assert str(ak.types.unknowntype.UnknownType()) == "unknown"
     with pytest.warns(DeprecationWarning):
         assert (
             str(ak.types.unknowntype.UnknownType(parameters={"x": 123}))
             == 'unknown[parameters={"x": 123}]'
         )
-    assert (
-        str(ak.types.unknowntype.UnknownType(parameters=None, typestr="override"))
-        == "override"
-    )
     with pytest.warns(DeprecationWarning):
-        assert (
-            str(
-                ak.types.unknowntype.UnknownType(
-                    parameters={"x": 123}, typestr="override"
-                )
-            )
-            == "override"
+        assert_overrides_typestr(ak.types.unknowntype.UnknownType())
+
+        assert_overrides_typestr(
+            ak.types.unknowntype.UnknownType(parameters={"x": 123})
         )
         assert (
             str(ak.types.unknowntype.UnknownType(parameters={"__categorical__": True}))
             == "categorical[type=unknown]"
         )
         assert (
             str(
                 ak.types.unknowntype.UnknownType(
                     parameters={"__categorical__": True, "x": 123}
                 )
             )
             == 'categorical[type=unknown[parameters={"x": 123}]]'
         )
-        assert (
-            str(
-                ak.types.unknowntype.UnknownType(
-                    parameters={"__categorical__": True}, typestr="override"
-                )
-            )
-            == "categorical[type=override]"
+        assert_overrides_typestr(
+            ak.types.unknowntype.UnknownType(
+                parameters={"__categorical__": True, "x": 123}
+            ),
+            expected="categorical[type=override]",
         )
 
     assert repr(ak.types.unknowntype.UnknownType()) == "UnknownType()"
     with pytest.warns(DeprecationWarning):
         assert (
-            repr(
-                ak.types.unknowntype.UnknownType(
-                    parameters={"__categorical__": True}, typestr="override"
-                )
-            )
-            == "UnknownType(parameters={'__categorical__': True}, typestr='override')"
+            repr(ak.types.unknowntype.UnknownType(parameters={"__categorical__": True}))
+            == "UnknownType(parameters={'__categorical__': True})"
         )
 
 
 @pytest.mark.skipif(
     ak._util.win,
     reason="NumPy does not have float16, float128, and complex256 -- on Windows",
 )
@@ -83,45 +86,35 @@
     assert str(ak.types.numpytype.NumpyType("complex128")) == "complex128"
     if hasattr(np, "complex256"):
         assert str(ak.types.numpytype.NumpyType("complex256")) == "complex256"
     assert (
         str(ak.types.numpytype.NumpyType("bool", parameters={"x": 123}))
         == 'bool[parameters={"x": 123}]'
     )
-    assert (
-        str(ak.types.numpytype.NumpyType("bool", parameters=None, typestr="override"))
-        == "override"
-    )
-    assert (
-        str(
-            ak.types.numpytype.NumpyType(
-                "bool", parameters={"x": 123}, typestr="override"
-            )
-        )
-        == "override"
+    assert_overrides_typestr(ak.types.numpytype.NumpyType("bool"))
+
+    assert_overrides_typestr(
+        ak.types.numpytype.NumpyType("bool", parameters={"x": 123})
     )
     assert (
         str(ak.types.numpytype.NumpyType("bool", parameters={"__categorical__": True}))
         == "categorical[type=bool]"
     )
     assert (
         str(
             ak.types.numpytype.NumpyType(
                 "bool", parameters={"__categorical__": True, "x": 123}
             )
         )
         == 'categorical[type=bool[parameters={"x": 123}]]'
     )
-    assert (
-        str(
-            ak.types.numpytype.NumpyType(
-                "bool", parameters={"__categorical__": True}, typestr="override"
-            )
-        )
-        == "categorical[type=override]"
+
+    assert_overrides_typestr(
+        ak.types.numpytype.NumpyType("bool", parameters={"__categorical__": True}),
+        expected="categorical[type=override]",
     )
     assert str(ak.types.numpytype.NumpyType("datetime64")) == "datetime64"
     assert (
         str(ak.types.numpytype.NumpyType("datetime64", parameters={"__unit__": "Y"}))
         == 'datetime64[unit="Y"]'
     )
     assert (
@@ -273,20 +266,18 @@
         str(ak.types.numpytype.NumpyType("uint8", parameters={"__array__": "byte"}))
         == "byte"
     )
     assert repr(ak.types.numpytype.NumpyType(primitive="bool")) == "NumpyType('bool')"
     assert (
         repr(
             ak.types.numpytype.NumpyType(
-                primitive="bool",
-                parameters={"__categorical__": True},
-                typestr="override",
+                primitive="bool", parameters={"__categorical__": True}
             )
         )
-        == "NumpyType('bool', parameters={'__categorical__': True}, typestr='override')"
+        == "NumpyType('bool', parameters={'__categorical__': True})"
     )
     assert (
         repr(
             ak.types.numpytype.NumpyType(
                 primitive="datetime64", parameters={"__unit__": "s"}
             )
         )
@@ -325,35 +316,27 @@
         str(
             ak.types.regulartype.RegularType(
                 ak.types.unknowntype.UnknownType(), 10, parameters={"x": 123}
             )
         )
         == '[10 * unknown, parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.regulartype.RegularType(
-                ak.types.unknowntype.UnknownType(),
-                10,
-                parameters=None,
-                typestr="override",
-            )
-        )
-        == "override"
+
+    assert_overrides_typestr(
+        ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
+        expected="override[10]",
     )
-    assert (
-        str(
-            ak.types.regulartype.RegularType(
-                ak.types.unknowntype.UnknownType(),
-                10,
-                parameters={"x": 123},
-                typestr="override",
-            )
-        )
-        == "override"
+
+    assert_overrides_typestr(
+        ak.types.regulartype.RegularType(
+            ak.types.unknowntype.UnknownType(),
+            10,
+            parameters={"x": 123},
+        ),
+        expected="override[10]",
     )
     assert (
         str(
             ak.types.regulartype.RegularType(
                 ak.types.unknowntype.UnknownType(),
                 10,
                 parameters={"__categorical__": True},
@@ -367,24 +350,21 @@
                 ak.types.unknowntype.UnknownType(),
                 10,
                 parameters={"__categorical__": True, "x": 123},
             )
         )
         == 'categorical[type=[10 * unknown, parameters={"x": 123}]]'
     )
-    assert (
-        str(
-            ak.types.regulartype.RegularType(
-                ak.types.unknowntype.UnknownType(),
-                10,
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.regulartype.RegularType(
+            ak.types.unknowntype.UnknownType(),
+            10,
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override[10]]",
     )
     assert (
         str(
             ak.types.regulartype.RegularType(
                 ak.types.numpytype.NumpyType("uint8", parameters={"__array__": "char"}),
                 10,
                 parameters={"__array__": "string"},
@@ -413,18 +393,17 @@
     )
     assert (
         repr(
             ak.types.regulartype.RegularType(
                 content=ak.types.unknowntype.UnknownType(),
                 size=10,
                 parameters={"__categorical__": True},
-                typestr="override",
             )
         )
-        == "RegularType(UnknownType(), 10, parameters={'__categorical__': True}, typestr='override')"
+        == "RegularType(UnknownType(), 10, parameters={'__categorical__': True})"
     )
     assert (
         repr(
             ak.types.regulartype.RegularType(
                 content=ak.types.numpytype.NumpyType(
                     primitive="uint8", parameters={"__array__": "char"}
                 ),
@@ -457,31 +436,22 @@
         str(
             ak.types.listtype.ListType(
                 ak.types.unknowntype.UnknownType(), parameters={"x": 123}
             )
         )
         == '[var * unknown, parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.listtype.ListType(
-                ak.types.unknowntype.UnknownType(), parameters=None, typestr="override"
-            )
-        )
-        == "override"
+    assert_overrides_typestr(
+        ak.types.listtype.ListType(ak.types.unknowntype.UnknownType())
     )
-    assert (
-        str(
-            ak.types.listtype.ListType(
-                ak.types.unknowntype.UnknownType(),
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.listtype.ListType(
+            ak.types.unknowntype.UnknownType(),
+            parameters={"x": 123},
         )
-        == "override"
     )
     assert (
         str(
             ak.types.listtype.ListType(
                 ak.types.unknowntype.UnknownType(), parameters={"__categorical__": True}
             )
         )
@@ -492,23 +462,20 @@
             ak.types.listtype.ListType(
                 ak.types.unknowntype.UnknownType(),
                 parameters={"__categorical__": True, "x": 123},
             )
         )
         == 'categorical[type=[var * unknown, parameters={"x": 123}]]'
     )
-    assert (
-        str(
-            ak.types.listtype.ListType(
-                ak.types.unknowntype.UnknownType(),
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.listtype.ListType(
+            ak.types.unknowntype.UnknownType(),
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
     )
     assert (
         str(
             ak.types.listtype.ListType(
                 ak.types.numpytype.NumpyType("uint8", parameters={"__array__": "char"}),
                 parameters={"__array__": "string"},
             )
@@ -530,18 +497,17 @@
         == "ListType(UnknownType())"
     )
     assert (
         repr(
             ak.types.listtype.ListType(
                 content=ak.types.unknowntype.UnknownType(),
                 parameters={"__categorical__": True},
-                typestr="override",
             )
         )
-        == "ListType(UnknownType(), parameters={'__categorical__': True}, typestr='override')"
+        == "ListType(UnknownType(), parameters={'__categorical__': True})"
     )
     assert (
         repr(
             ak.types.listtype.ListType(
                 content=ak.types.numpytype.NumpyType(
                     primitive="uint8", parameters={"__array__": "char"}
                 ),
@@ -610,69 +576,51 @@
                 ],
                 ["x", "y"],
                 parameters={"__record__": "Name"},
             )
         )
         == "Name[x: unknown, y: bool]"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters=None,
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters=None,
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"__record__": "Name"},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"__record__": "Name"},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"__record__": "Name"},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"__record__": "Name"},
         )
-        == "override"
     )
     assert (
         str(
             ak.types.recordtype.RecordType(
                 [
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -718,69 +666,53 @@
                 ],
                 ["x", "y"],
                 parameters={"__record__": "Name", "x": 123},
             )
         )
         == 'Name[x: unknown, y: bool, parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"x": 123},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"x": 123},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"__record__": "Name", "x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"__record__": "Name", "x": 123},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"__record__": "Name", "x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"__record__": "Name", "x": 123},
         )
-        == "override"
     )
     assert (
         str(
             ak.types.recordtype.RecordType(
                 [
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -826,69 +758,57 @@
                 ],
                 ["x", "y"],
                 parameters={"__record__": "Name", "__categorical__": True},
             )
         )
         == "categorical[type=Name[x: unknown, y: bool]]"
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"__record__": "Name", "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"__record__": "Name", "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"__record__": "Name", "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"__record__": "Name", "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
     )
     assert (
         str(
             ak.types.recordtype.RecordType(
                 [
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -934,69 +854,57 @@
                 ],
                 ["x", "y"],
                 parameters={"__record__": "Name", "x": 123, "__categorical__": True},
             )
         )
         == 'categorical[type=Name[x: unknown, y: bool, parameters={"x": 123}]]'
     )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                None,
-                parameters={"__record__": "Name", "x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.recordtype.RecordType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                ["x", "y"],
-                parameters={"__record__": "Name", "x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            None,
+            parameters={"__record__": "Name", "x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.recordtype.RecordType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            ["x", "y"],
+            parameters={"__record__": "Name", "x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
     )
 
     assert (
         repr(
             ak.types.recordtype.RecordType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
@@ -1024,18 +932,17 @@
             ak.types.recordtype.RecordType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 fields=None,
                 parameters={"__record__": "Name", "x": 123, "__categorical__": True},
-                typestr="override",
             )
         )
-        == "RecordType([UnknownType(), NumpyType('bool')], None, parameters={'__record__': 'Name', 'x': 123, '__categorical__': True}, typestr='override')"
+        == "RecordType([UnknownType(), NumpyType('bool')], None, parameters={'__record__': 'Name', 'x': 123, '__categorical__': True})"
     )
     assert (
         repr(
             ak.types.recordtype.RecordType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -1051,18 +958,17 @@
             ak.types.recordtype.RecordType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 fields=["x", "y"],
                 parameters={"__record__": "Name", "x": 123, "__categorical__": True},
-                typestr="override",
             )
         )
-        == "RecordType([UnknownType(), NumpyType('bool')], ['x', 'y'], parameters={'__record__': 'Name', 'x': 123, '__categorical__': True}, typestr='override')"
+        == "RecordType([UnknownType(), NumpyType('bool')], ['x', 'y'], parameters={'__record__': 'Name', 'x': 123, '__categorical__': True})"
     )
 
 
 def test_OptionType():
     assert (
         str(ak.types.optiontype.OptionType(ak.types.unknowntype.UnknownType()))
         == "?unknown"
@@ -1107,75 +1013,47 @@
                     ak.types.unknowntype.UnknownType(), 10
                 ),
                 parameters={"x": 123},
             )
         )
         == 'option[10 * unknown, parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.unknowntype.UnknownType(), parameters=None, typestr="override"
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.unknowntype.UnknownType(), parameters=None
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-                parameters=None,
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
+            parameters=None,
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.regulartype.RegularType(
-                    ak.types.unknowntype.UnknownType(), 10
-                ),
-                parameters=None,
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10)
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.unknowntype.UnknownType(),
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.unknowntype.UnknownType(),
+            parameters={"x": 123},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
+            parameters={"x": 123},
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.regulartype.RegularType(
-                    ak.types.unknowntype.UnknownType(), 10
-                ),
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
+            parameters={"x": 123},
         )
-        == "override"
     )
     assert (
         str(
             ak.types.optiontype.OptionType(
                 ak.types.unknowntype.UnknownType(), parameters={"__categorical__": True}
             )
         )
@@ -1226,77 +1104,55 @@
                     ak.types.unknowntype.UnknownType(), 10
                 ),
                 parameters={"x": 123, "__categorical__": True},
             )
         )
         == 'option[categorical[type=10 * unknown], parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.unknowntype.UnknownType(),
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.regulartype.RegularType(
-                    ak.types.unknowntype.UnknownType(), 10
-                ),
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.unknowntype.UnknownType(),
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.optiontype.OptionType(
-                ak.types.regulartype.RegularType(
-                    ak.types.unknowntype.UnknownType(), 10
-                ),
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.unknowntype.UnknownType(),
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.unknowntype.UnknownType(),
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.listtype.ListType(ak.types.unknowntype.UnknownType()),
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.optiontype.OptionType(
+            ak.types.regulartype.RegularType(ak.types.unknowntype.UnknownType(), 10),
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
     )
 
     assert (
         repr(ak.types.optiontype.OptionType(content=ak.types.unknowntype.UnknownType()))
         == "OptionType(UnknownType())"
     )
     assert (
@@ -1310,18 +1166,17 @@
     assert (
         repr(
             ak.types.optiontype.OptionType(
                 content=ak.types.regulartype.RegularType(
                     ak.types.unknowntype.UnknownType(), 10
                 ),
                 parameters={"x": 123, "__categorical__": True},
-                typestr="override",
             )
         )
-        == "OptionType(RegularType(UnknownType(), 10), parameters={'x': 123, '__categorical__': True}, typestr='override')"
+        == "OptionType(RegularType(UnknownType(), 10), parameters={'x': 123, '__categorical__': True})"
     )
 
 
 def test_UnionType():
     assert (
         str(
             ak.types.uniontype.UnionType(
@@ -1341,39 +1196,31 @@
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 parameters={"x": 123},
             )
         )
         == 'union[unknown, bool, parameters={"x": 123}]'
     )
-    assert (
-        str(
-            ak.types.uniontype.UnionType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                parameters=None,
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.uniontype.UnionType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            parameters=None,
         )
-        == "override"
     )
-    assert (
-        str(
-            ak.types.uniontype.UnionType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                parameters={"x": 123},
-                typestr="override",
-            )
+    assert_overrides_typestr(
+        ak.types.uniontype.UnionType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            parameters={"x": 123},
         )
-        == "override"
     )
     assert (
         str(
             ak.types.uniontype.UnionType(
                 [
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
@@ -1391,39 +1238,33 @@
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 parameters={"x": 123, "__categorical__": True},
             )
         )
         == 'categorical[type=union[unknown, bool, parameters={"x": 123}]]'
     )
-    assert (
-        str(
-            ak.types.uniontype.UnionType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                parameters={"__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
-    )
-    assert (
-        str(
-            ak.types.uniontype.UnionType(
-                [
-                    ak.types.unknowntype.UnknownType(),
-                    ak.types.numpytype.NumpyType("bool"),
-                ],
-                parameters={"x": 123, "__categorical__": True},
-                typestr="override",
-            )
-        )
-        == "categorical[type=override]"
+    assert_overrides_typestr(
+        ak.types.uniontype.UnionType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            parameters={"__categorical__": True},
+        ),
+        expected="categorical[type=override]",
+    )
+    assert_overrides_typestr(
+        ak.types.uniontype.UnionType(
+            [
+                ak.types.unknowntype.UnknownType(),
+                ak.types.numpytype.NumpyType("bool"),
+            ],
+            parameters={"x": 123, "__categorical__": True},
+        ),
+        expected="categorical[type=override]",
     )
 
     assert (
         repr(
             ak.types.uniontype.UnionType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
@@ -1437,18 +1278,17 @@
         repr(
             ak.types.uniontype.UnionType(
                 contents=[
                     ak.types.unknowntype.UnknownType(),
                     ak.types.numpytype.NumpyType("bool"),
                 ],
                 parameters={"x": 123, "__categorical__": True},
-                typestr="override",
             )
         )
-        == "UnionType([UnknownType(), NumpyType('bool')], parameters={'x': 123, '__categorical__': True}, typestr='override')"
+        == "UnionType([UnknownType(), NumpyType('bool')], parameters={'x': 123, '__categorical__': True})"
     )
 
 
 def test_ArrayType():
     assert (
         str(ak.types.arraytype.ArrayType(ak.types.unknowntype.UnknownType(), 10))
         == "10 * unknown"
@@ -1458,27 +1298,50 @@
         == "0 * unknown"
     )
     with pytest.raises(ValueError):
         ak.types.arraytype.ArrayType(ak.types.unknowntype.UnknownType(), -1)
 
     # ArrayType should not have these arguments (should not be a Type subclass)
     with pytest.raises(TypeError):
-        ak.types.arraytype.ArrayType(ak.types.unknowntype.UnknownType(), 10, {"x": 123})
-    with pytest.raises(TypeError):
         ak.types.arraytype.ArrayType(
-            ak.types.unknowntype.UnknownType(), 10, None, typestr="override"
+            ak.types.arraytype.ArrayType(ak.types.unknowntype.UnknownType(), 10), 10
         )
 
     assert (
         repr(
             ak.types.arraytype.ArrayType(
                 content=ak.types.unknowntype.UnknownType(), length=10
             )
         )
-        == "ArrayType(UnknownType(), 10)"
+        == "ArrayType(UnknownType(), 10, None)"
+    )
+
+    assert (
+        str(
+            ak.types.arraytype.ArrayType(
+                content=ak.types.numpytype.NumpyType(
+                    "int64", parameters={"__array__": "custom"}
+                ),
+                length=10,
+                behavior={("__typestr__", "custom"): "override"},
+            )
+        )
+        == "10 * override"
+    )
+
+    assert (
+        str(
+            ak.types.arraytype.ArrayType(
+                content=ak.types.numpytype.NumpyType(
+                    "int64", parameters={"__array__": "custom"}
+                ),
+                length=10,
+            )
+        )
+        == '10 * int64[parameters={"__array__": "custom"}]'
     )
 
 
 def test_EmptyForm():
     assert (
         str(ak.forms.emptyform.EmptyForm())
         == """{
```

### Comparing `awkward-2.2.0/tests/test_0916_datetime_values_astype.py` & `awkward-2.2.1/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.2.1/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.2.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.2.1/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.2.1/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0959__getitem_array_implementation.py` & `awkward-2.2.1/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.2.1/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.2.1/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.2.1/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0984_ravel.py` & `awkward-2.2.1/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.2.1/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.2.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.2.1/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1030_mixin_class_name.py` & `awkward-2.2.1/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1031_start_getitem_next.py` & `awkward-2.2.1/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.2.1/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1049_concatenate_single_array.py` & `awkward-2.2.1/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.2.1/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1059_localindex.py` & `awkward-2.2.1/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.2.1/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.2.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1072_sort.py` & `awkward-2.2.1/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1074_combinations.py` & `awkward-2.2.1/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1075_validityerror.py` & `awkward-2.2.1/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1110_type_tracer_1.py` & `awkward-2.2.1/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1116_project_maskedarrays.py` & `awkward-2.2.1/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.2.1/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.2.1/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.2.1/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1135_rpad_operation.py` & `awkward-2.2.1/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.2.1/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1137_num.py` & `awkward-2.2.1/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1142_numbers_to_type.py` & `awkward-2.2.1/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1149_datetime_sort.py` & `awkward-2.2.1/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.2.1/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1162_ak_from_json_schema.py` & `awkward-2.2.1/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.2.1/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.2.1/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.2.1/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1193_is_none_nested_option.py` & `awkward-2.2.1/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1233_ak_with_name.py` & `awkward-2.2.1/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.2.1/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1259_simplify_optiontype.py` & `awkward-2.2.1/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.2.1/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1271_fix_4D_reducers.py` & `awkward-2.2.1/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1294_to_and_from_parquet.py` & `awkward-2.2.1/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.2.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.2.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1300b_same_for_numba.py` & `awkward-2.2.1/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1308_zip_after_option.py` & `awkward-2.2.1/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1318_array_function_types.py` & `awkward-2.2.1/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1320_mask_identity_defaults.py` & `awkward-2.2.1/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.2.1/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1345_avro_reader.py` & `awkward-2.2.1/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1351_is_tuple.py` & `awkward-2.2.1/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1374_to_rdataframe.py` & `awkward-2.2.1/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1377_ravel_string.py` & `awkward-2.2.1/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.2.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1399_from_jax.py` & `awkward-2.2.1/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1399_to_jax.py` & `awkward-2.2.1/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1405_slicing_untested_cases.py` & `awkward-2.2.1/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1415_behaviour_forwarding.py` & `awkward-2.2.1/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.2.1/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.2.1/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.2.1/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.2.1/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1473_from_rdataframe.py` & `awkward-2.2.1/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.2.1/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.2.1/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.2.1/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1504_typetracer_like.py` & `awkward-2.2.1/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.2.1/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1511_set_attribute.py` & `awkward-2.2.1/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.2.1/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.2.1/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.2.1/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.2.1/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.2.1/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.2.1/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.2.1/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1607_no_reducers_on_records.py` & `awkward-2.2.1/tests/test_1607_no_reducers_on_records.py`

 * *Files 27% similar despite different names*

```diff
@@ -53,54 +53,55 @@
     with pytest.raises(TypeError):
         assert ak.to_list(ak.operations.sum(array, axis=1)) == [
             {"phi": 0.0, "rho": 0.0}
         ]
 
 
 def test_overloaded_reducers():
-    def overload_add(array, axis=-1):
+    def overload_add(array, mask):
         return ak.contents.RecordArray(
             [
-                ak.contents.NumpyArray(np.asarray([ak.sum(array["rho"], axis=axis)])),
-                ak.contents.NumpyArray(np.asarray([ak.sum(array["phi"], axis=axis)])),
+                ak.sum(array["rho"], axis=-1, mask_identity=False, highlevel=False),
+                ak.sum(array["phi"], axis=-1, mask_identity=False, highlevel=False),
             ],
             ["rho", "phi"],
         )
 
     behavior = {}
     behavior[ak.sum, "VectorArray2D"] = overload_add
 
     array = ak.Array(
         [[{"rho": -1.1, "phi": -0.1}, {"rho": 1.1, "phi": 0.1}]],
         with_name="VectorArray2D",
         behavior=behavior,
     )
 
-    with pytest.raises(NotImplementedError):
-        assert ak.to_list(ak.sum(array, axis=1)) == [{"rho": 0, "phi": 0}]
+    assert ak.to_list(ak.sum(array, axis=1)) == [{"rho": 0, "phi": 0}]
 
-    with pytest.raises(TypeError):
+    with pytest.raises(
+        TypeError, match=r"overloads for custom types: VectorArray2D, int"
+    ):
         ak.to_list(array + 1)
 
-    def overload_add2(array):
+    def overload_add2(array, mask):
         return ak.contents.RecordArray(
-            [ak.contents.NumpyArray(np.asarray([2.4, 3, 4.5, 6]))], ["rho"]
+            [ak.contents.NumpyArray(np.asarray([2.4, 3, 4.5, 6], dtype=np.float64))],
+            ["rho"],
         )
 
     behavior = {}
     behavior[ak.sum, "VectorArray2D"] = overload_add2
 
     array = ak.Array(
         [[{"rho": -1.1, "phi": -0.1}, {"rho": 1.1, "phi": 0.1}]],
         with_name="VectorArray2D",
         behavior=behavior,
     )
 
-    with pytest.raises(NotImplementedError):
-        assert ak.to_list(ak.sum(array, axis=1)) == [{"rho": 2.4}]
+    assert ak.to_list(ak.sum(array, axis=1)) == [{"rho": 2.4}]
 
     array = ak.highlevel.Array(
         ak.contents.ByteMaskedArray(
             ak.index.Index8(np.array([True, True])),
             ak.contents.RecordArray(
                 [
                     ak.contents.NumpyArray(np.arange(2)),
@@ -111,9 +112,34 @@
                 ],
                 ["a", "b"],
             ),
             valid_when=True,
         )
     )
 
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match=r"overloads for custom types: a, b"):
         ak.to_list(ak.sum(array, axis=0))
+
+    def overload_argmax(array, mask):
+        return ak.argmax(array["rho"], axis=-1, mask_identity=False, highlevel=False)
+
+    behavior = {}
+    behavior[ak.argmax, "VectorArray2D"] = overload_argmax
+
+    array = ak.Array(
+        [
+            [
+                {"rho": -1.1, "phi": -0.1},
+                {"rho": 1.1, "phi": 0.1},
+                {"rho": -1.1, "phi": 0.3},
+            ],
+            [
+                {"rho": 1.1, "phi": 0.1},
+                {"rho": -1.1, "phi": 0.3},
+                {"rho": -1.1, "phi": -0.1},
+            ],
+        ],
+        with_name="VectorArray2D",
+        behavior=behavior,
+    )
+
+    assert ak.to_list(ak.argmax(array, axis=1)) == [1, 0]
```

### Comparing `awkward-2.2.0/tests/test_1613_generator_tolayout_records.py` & `awkward-2.2.1/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.2.1/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1620_layout_builders.py` & `awkward-2.2.1/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.2.1/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.2.1/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.2.1/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1671_categorical_type.py` & `awkward-2.2.1/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1672_broadcast_parameters.py` & `awkward-2.2.1/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1677_array_builder_in_numba.py` & `awkward-2.2.1/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.2.1/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.2.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1688_pack_categorical.py` & `awkward-2.2.1/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1703_fill_none_typetracer.py` & `awkward-2.2.1/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.2.1/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.2.1/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.2.1/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.2.1/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1762_jax_behavior_support.py` & `awkward-2.2.1/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1764_jax_jacobian.py` & `awkward-2.2.1/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.2.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1766_record_form_fields.py` & `awkward-2.2.1/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.2.1/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.2.1/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1790_reduce_regulararray.py` & `awkward-2.2.1/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.2.1/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.2.1/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.2.1/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.2.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.2.1/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.2.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.2.1/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1904_drop_none.py` & `awkward-2.2.1/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.2.1/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.2.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.2.1/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1936_with_field_broadcasting.py` & `awkward-2.2.1/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1940_ak_backend.py` & `awkward-2.2.1/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1943_regular_indexing.py` & `awkward-2.2.1/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.2.1/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_1961_ak_without_field.py` & `awkward-2.2.1/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2020_reduce_axis_none.py` & `awkward-2.2.1/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.2.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2023_from_rdataframe.py` & `awkward-2.2.1/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.2.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import copy
 
 import numpy as np
 
 import awkward as ak
-from awkward._nplikes.typetracer import typetracer_with_report
+from awkward.typetracer import typetracer_with_report
 
 
 def test_prototypical_example():
     array = ak.Array(
         {
             "Muon_pt": [[1.1, 2.2, 3.3], [], [4.4, 5.5]],
             "Muon_phi": [[1.1, 2.2, 3.3], [], [4.4, 5.5]],
```

### Comparing `awkward-2.2.0/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.2.1/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2055_array_builder_check.py` & `awkward-2.2.1/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2058_merge_numpy_array.py` & `awkward-2.2.1/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2064_fill_none_record.py` & `awkward-2.2.1/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.2.1/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2070_to_layout_string.py` & `awkward-2.2.1/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.2.1/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2078_array_function_wrap.py` & `awkward-2.2.1/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2082_broadcast_zero_size.py` & `awkward-2.2.1/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2096_ak_scalar_type.py` & `awkward-2.2.1/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2101_pickle_behavior_class.py` & `awkward-2.2.1/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2104_numpy_merge_option.py` & `awkward-2.2.1/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2106_pickle_class.py` & `awkward-2.2.1/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2108_fill_none_indexed.py` & `awkward-2.2.1/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2115_fix_up_typetracers.py` & `awkward-2.2.1/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2125_type_of_scalar.py` & `awkward-2.2.1/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.2.1/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2179_parameter_merging_rules.py` & `awkward-2.2.1/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2185_merge_union_of_records.py` & `awkward-2.2.1/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.2.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2198_almost_equal.py` & `awkward-2.2.1/tests/test_2198_almost_equal.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,7 +145,23 @@
     assert ak.almost_equal(left, left)
 
 
 def test_typetracer():
     array = ak.Array([[[1, 2, 3]], [[5, 4]]], backend="typetracer")
     with pytest.raises(NotImplementedError):
         ak.almost_equal(array, 2 * array)
+
+
+def test_indexed():
+    assert ak.almost_equal(
+        ak.contents.ListOffsetArray(
+            ak.index.Index64([0, 2, 4, 8]),
+            ak.contents.IndexedArray(
+                ak.index.Index64([0, 1, 2, 3, 2, 1, 0, 5]),
+                ak.contents.NumpyArray(np.arange(6, dtype=np.int64)),
+            ),
+        ),
+        ak.contents.ListOffsetArray(
+            ak.index.Index64([0, 2, 4, 8]),
+            ak.contents.NumpyArray(np.array([0, 1, 2, 3, 2, 1, 0, 5], dtype=np.int64)),
+        ),
+    )
```

### Comparing `awkward-2.2.0/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.2.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2214_offset_bool_index.py` & `awkward-2.2.1/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.2.1/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2229_getitem_range_slice.py` & `awkward-2.2.1/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.2.1/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.2.1/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.2.1/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2246_slice_not_packed.py` & `awkward-2.2.1/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2250_full_like_bool.py` & `awkward-2.2.1/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.2.1/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2263_to_packed_list.py` & `awkward-2.2.1/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2266_fix_nan_to_num.py` & `awkward-2.2.1/tests/test_2266_fix_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2267_broadcast_fields.py` & `awkward-2.2.1/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2293_unflatten_typetracer.py` & `awkward-2.2.1/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2297_common_backend.py` & `awkward-2.2.1/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.2.1/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2306_cppyy_git.py` & `awkward-2.2.1/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2319_from_buffers_array.py` & `awkward-2.2.1/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2327_array_interface.py` & `awkward-2.2.1/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.2.1/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.2.1/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2354_ufunc_same_backend.py` & `awkward-2.2.1/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2355_to_backend_record.py` & `awkward-2.2.1/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.2.1/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2365_enforce_type.py` & `awkward-2.2.1/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2368_type_is_equal.py` & `awkward-2.2.1/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2373_unzip_touching.py` & `awkward-2.2.1/tests/test_2373_unzip_touching.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,13 +112,13 @@
                 },
             ],
             "parameters": {},
             "form_key": "outer!",
         }
     )
 
-    ttlayout, report = ak._nplikes.typetracer.typetracer_with_report(form)
+    ttlayout, report = ak.typetracer.typetracer_with_report(form)
 
     ttarray = ak.Array(ttlayout)
     pairs = ak.cartesian([ttarray.muon, ttarray.jet], axis=1, nested=True)
     a, b = ak.unzip(pairs)
     assert report.data_touched == ["muon_list!", "jet_list!"]
```

### Comparing `awkward-2.2.0/tests/test_2374_cartesian_touching.py` & `awkward-2.2.1/tests/test_2374_cartesian_touching.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 },
             ],
             "parameters": {},
             "form_key": "outer!",
         }
     )
 
-    ttlayout, report = ak._nplikes.typetracer.typetracer_with_report(form)
+    ttlayout, report = ak.typetracer.typetracer_with_report(form)
 
     ttarray = ak.Array(ttlayout)
 
     a = ak.cartesian([ttarray.muon, ttarray.jet], axis=1, nested=True)
 
     mval = delta_r2(a["0"], a["1"])
```

### Comparing `awkward-2.2.0/tests/test_2385_with_field_empty_record.py` & `awkward-2.2.1/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2395_copy_asarray_touch.py` & `awkward-2.2.1/tests/test_2395_copy_asarray_touch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import numpy as np
 import pytest  # noqa: F401
 
 import awkward as ak
-from awkward._nplikes.typetracer import TypeTracer, typetracer_with_report
+from awkward._nplikes.typetracer import TypeTracer
+from awkward.typetracer import typetracer_with_report
 
 typetracer = TypeTracer.instance()
 
 
 def test_no_copy():
     form = ak.forms.NumpyForm("int64", form_key="buffer")
     layout, report = typetracer_with_report(form)
```

### Comparing `awkward-2.2.0/tests/test_2410_string_broadcast.py` & `awkward-2.2.1/tests/test_2410_string_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.2.1/tests/test_2411_cartesian_axis_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2417_bytemasked_singletons.py` & `awkward-2.2.1/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2424_almost_equal_union_record.py` & `awkward-2.2.1/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2425_forms_from_type.py` & `awkward-2.2.1/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/test_2426_is_equal_to.py` & `awkward-2.2.1/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/list-depths-records-list.parquet` & `awkward-2.2.1/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/list-depths-records.parquet` & `awkward-2.2.1/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/list-depths-strings.parquet` & `awkward-2.2.1/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/list-depths.parquet` & `awkward-2.2.1/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nonnullable-depths.parquet` & `awkward-2.2.1/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-depths.parquet` & `awkward-2.2.1/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-levels.parquet` & `awkward-2.2.1/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.2.1/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.2.1/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.2.1/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-list-depths.parquet` & `awkward-2.2.1/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/nullable-record-primitives.parquet` & `awkward-2.2.1/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/record-primitives.parquet` & `awkward-2.2.1/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/test-nan-inf.json` & `awkward-2.2.1/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/test-two-arrays.json` & `awkward-2.2.1/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests/samples/test.json` & `awkward-2.2.1/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1276_cuda_num.py` & `awkward-2.2.1/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.2.1/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.2.1/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1276_from_cupy.py` & `awkward-2.2.1/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.2.1/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1381_check_errors.py` & `awkward-2.2.1/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.2.1/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/.gitignore` & `awkward-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/LICENSE` & `awkward-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.2.0/pyproject.toml` & `awkward-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.2.0"
+version = "2.2.1"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.0"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.1"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
```

### Comparing `awkward-2.2.0/PKG-INFO` & `awkward-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.2.0
+Version: 2.2.1
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.2.0 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.2.1 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
```

