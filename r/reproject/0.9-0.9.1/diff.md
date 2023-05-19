# Comparing `tmp/reproject-0.9.tar.gz` & `tmp/reproject-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reproject-0.9.tar", last modified: Fri Sep  2 15:14:59 2022, max compression
+gzip compressed data, was "reproject-0.9.1.tar", last modified: Wed Nov  2 11:15:01 2022, max compression
```

## Comparing `reproject-0.9.tar` & `reproject-0.9.1.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.135244 reproject-0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.119244 reproject-0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.119244 reproject-0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-09-02 15:14:34.000000 reproject-0.9/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-02 15:14:34.000000 reproject-0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-02 15:14:34.000000 reproject-0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-09-02 15:14:34.000000 reproject-0.9/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-02 15:14:34.000000 reproject-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-02 15:14:34.000000 reproject-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-09-02 15:14:59.135244 reproject-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-09-02 15:14:34.000000 reproject-0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-09-02 15:14:34.000000 reproject-0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.119244 reproject-0.9/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-02 15:14:34.000000 reproject-0.9/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-02 15:14:34.000000 reproject-0.9/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-02 15:14:34.000000 reproject-0.9/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21469 2022-09-02 15:14:34.000000 reproject-0.9/docs/celestial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6423 2022-09-02 15:14:34.000000 reproject-0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-09-02 15:14:34.000000 reproject-0.9/docs/footprints.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-09-02 15:14:34.000000 reproject-0.9/docs/healpix.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-09-02 15:14:34.000000 reproject-0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-02 15:14:34.000000 reproject-0.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-09-02 15:14:34.000000 reproject-0.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)    15846 2022-09-02 15:14:34.000000 reproject-0.9/docs/mosaicking.rst
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-02 15:14:34.000000 reproject-0.9/docs/noncelestial.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-09-02 15:14:34.000000 reproject-0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/reproject/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-02 15:14:34.000000 reproject-0.9/reproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-02 15:14:34.000000 reproject-0.9/reproject/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-09-02 15:14:58.000000 reproject-0.9/reproject/_compiler.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/reproject/adaptive/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    25468 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/deforest.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     9572 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/high_level.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/reproject/adaptive/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/adaptive/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (121)    63360 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_2d.fits
--rw-r--r--   0 runner    (1001) docker     (121)    63360 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_2d_rotated.fits
--rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_roundtrip.fits
--rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_uncentered_jacobian.fits
--rw-r--r--   0 runner    (1001) docker     (121)    28990 2022-09-02 15:14:34.000000 reproject-0.9/reproject/adaptive/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-02 15:14:34.000000 reproject-0.9/reproject/array_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-09-02 15:14:34.000000 reproject-0.9/reproject/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/healpix/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4957 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/high_level.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/healpix/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/healpix/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   102936 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/tests/data/bayestar.fits.gz
--rw-r--r--   0 runner    (1001) docker     (121)    69120 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/tests/data/reference_result.fits
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/tests/test_healpix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-09-02 15:14:34.000000 reproject-0.9/reproject/healpix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/interpolation/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/high_level.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/interpolation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.127245 reproject-0.9/reproject/interpolation/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (121)    40320 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/reference/test_reproject_celestial_2d_gal2equ.fits
--rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/reference/test_reproject_celestial_3d_equ2gal.fits
--rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/reference/test_reproject_roundtrip.fits
--rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/reference/test_small_cutout.fits
--rw-r--r--   0 runner    (1001) docker     (121)    22952 2022-09-02 15:14:34.000000 reproject-0.9/reproject/interpolation/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.131245 reproject-0.9/reproject/mosaicking/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/background.py
--rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/coadd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/subset_array.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.131245 reproject-0.9/reproject/mosaicking/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.131245 reproject-0.9/reproject/mosaicking/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (121)   264960 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/reference/test_coadd_solar_map.fits
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/test_coadd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/test_subset_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/tests/test_wcs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8855 2022-09-02 15:14:34.000000 reproject-0.9/reproject/mosaicking/wcs_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.131245 reproject-0.9/reproject/spherical_intersect/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/high_level.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/mNaN.h
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/overlap.py
--rw-r--r--   0 runner    (1001) docker     (121)    25630 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/overlapArea.c
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/overlapArea.h
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/overlapAreaPP.c
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/reproject_slice_c.c
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/reproject_slice_c.h
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.131245 reproject-0.9/reproject/spherical_intersect/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/tests/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/tests/test_overlap.py
--rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-09-02 15:14:34.000000 reproject-0.9/reproject/spherical_intersect/tests/test_reproject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.135244 reproject-0.9/reproject/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.135244 reproject-0.9/reproject/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   139654 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/aia_171_level1.asdf
--rw-r--r--   0 runner    (1001) docker     (121)   149760 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/aia_171_level1.fits
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/cube.hdr
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/equatorial_3d.fits
--rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/galactic_2d.fits
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/gc_eq.hdr
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/gc_ga.hdr
--rw-r--r--   0 runner    (1001) docker     (121)    58239 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/mwpan2_RGB_3600.hdr
--rw-r--r--   0 runner    (1001) docker     (121)   152640 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/secchi_l0_a.fits
--rw-r--r--   0 runner    (1001) docker     (121)   152640 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/data/secchi_l0_b.fits
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-09-02 15:14:34.000000 reproject-0.9/reproject/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-09-02 15:14:34.000000 reproject-0.9/reproject/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-09-02 15:14:58.000000 reproject-0.9/reproject/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-09-02 15:14:34.000000 reproject-0.9/reproject/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 15:14:59.123244 reproject-0.9/reproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-02 15:14:59.000000 reproject-0.9/reproject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-09-02 15:14:59.139244 reproject-0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2040 2022-09-02 15:14:34.000000 reproject-0.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-09-02 15:14:34.000000 reproject-0.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.706740 reproject-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.678740 reproject-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.686740 reproject-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-11-02 11:14:34.000000 reproject-0.9.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-11-02 11:14:34.000000 reproject-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-11-02 11:14:34.000000 reproject-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-11-02 11:14:34.000000 reproject-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-11-02 11:14:34.000000 reproject-0.9.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-11-02 11:14:34.000000 reproject-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-11-02 11:14:34.000000 reproject-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-11-02 11:15:01.706740 reproject-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-11-02 11:14:34.000000 reproject-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.690740 reproject-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.678740 reproject-0.9.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.690740 reproject-0.9.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21469 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/celestial.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6423 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/footprints.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/healpix.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)    15846 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/mosaicking.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-11-02 11:14:34.000000 reproject-0.9.1/docs/noncelestial.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-02 11:14:34.000000 reproject-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.690740 reproject-0.9.1/reproject/
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject/_compiler.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.694740 reproject-0.9.1/reproject/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5143 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25468 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/deforest.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     9572 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/high_level.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.694740 reproject-0.9.1/reproject/adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.698740 reproject-0.9.1/reproject/adaptive/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)    63360 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_2d.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    63360 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_2d_rotated.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_roundtrip.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_uncentered_jacobian.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    28990 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/adaptive/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.698740 reproject-0.9.1/reproject/healpix/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4957 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/high_level.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.698740 reproject-0.9.1/reproject/healpix/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.698740 reproject-0.9.1/reproject/healpix/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   102936 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/tests/data/bayestar.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    69120 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/tests/data/reference_result.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/tests/test_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/healpix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.698740 reproject-0.9.1/reproject/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/high_level.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.702740 reproject-0.9.1/reproject/interpolation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.702740 reproject-0.9.1/reproject/interpolation/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)    40320 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_celestial_2d_gal2equ.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_celestial_3d_equ2gal.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   270720 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_roundtrip.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/reference/test_small_cutout.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    22952 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/interpolation/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.702740 reproject-0.9.1/reproject/mosaicking/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/background.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/coadd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/subset_array.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.702740 reproject-0.9.1/reproject/mosaicking/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.702740 reproject-0.9.1/reproject/mosaicking/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)   264960 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/reference/test_coadd_solar_map.fits
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10347 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/test_coadd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/test_subset_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/tests/test_wcs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8855 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/mosaicking/wcs_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.706740 reproject-0.9.1/reproject/spherical_intersect/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/mNaN.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25630 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/overlapArea.c
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/overlapArea.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/overlapAreaPP.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/reproject_slice_c.c
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/reproject_slice_c.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.706740 reproject-0.9.1/reproject/spherical_intersect/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/tests/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/tests/test_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/spherical_intersect/tests/test_reproject.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.706740 reproject-0.9.1/reproject/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.706740 reproject-0.9.1/reproject/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   139654 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/aia_171_level1.asdf
+-rw-r--r--   0 runner    (1001) docker     (121)   149760 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/aia_171_level1.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/cube.hdr
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/equatorial_3d.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/galactic_2d.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/gc_eq.hdr
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/gc_ga.hdr
+-rw-r--r--   0 runner    (1001) docker     (121)    58239 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/mwpan2_RGB_3600.hdr
+-rw-r--r--   0 runner    (1001) docker     (121)   152640 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/secchi_l0_a.fits
+-rw-r--r--   0 runner    (1001) docker     (121)   152640 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/data/secchi_l0_b.fits
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-11-02 11:14:34.000000 reproject-0.9.1/reproject/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 11:15:01.694740 reproject-0.9.1/reproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3861 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-02 11:15:01.000000 reproject-0.9.1/reproject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-11-02 11:15:01.706740 reproject-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2040 2022-11-02 11:14:34.000000 reproject-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-11-02 11:14:34.000000 reproject-0.9.1/tox.ini
```

### Comparing `reproject-0.9/.github/workflows/ci_workflows.yml` & `reproject-0.9.1/.github/workflows/ci_workflows.yml`

 * *Files 25% similar despite different names*

```diff
@@ -18,26 +18,30 @@
         - macos: py38-test-oldestdeps
         - macos: py39-test
         - macos: py310-test
         - linux: py38-test-oldestdeps
         - linux: py38-test
         - linux: py39-test
         - linux: py310-test
+        - linux: py311-test-devdeps
         - windows: py38-test-oldestdeps
         - windows: py39-test
         - windows: py310-test
+      libraries: |
+        apt:
+          - libopenblas-dev
       coverage: 'codecov'
 
   publish:
     needs: tests
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish.yml@v1
     with:
       test_extras: test
       test_command: pytest -p no:warnings --pyargs reproject
       targets: |
         - cp*-manylinux_x86_64
         - cp*-manylinux_aarch64
         - cp*-macosx_x86_64
         - cp*-macosx_arm64
-        - cp*-win*
+        - cp*-win_amd64
     secrets:
       pypi_token: ${{ secrets.pypi_token }}
```

### Comparing `reproject-0.9/.gitignore` & `reproject-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `reproject-0.9/CHANGES.md` & `reproject-0.9.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `reproject-0.9/LICENSE` & `reproject-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reproject-0.9/PKG-INFO` & `reproject-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reproject
-Version: 0.9
+Version: 0.9.1
 Summary: Reproject astronomical images
 Home-page: https://reproject.readthedocs.io
 Author: Thomas Robitaille, Christoph Deil, Adam Ginsburg
 Author-email: thomas.robitaille@gmail.com
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `reproject-0.9/README.rst` & `reproject-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/Makefile` & `reproject-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/celestial.rst` & `reproject-0.9.1/docs/celestial.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/conf.py` & `reproject-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/footprints.rst` & `reproject-0.9.1/docs/footprints.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/healpix.rst` & `reproject-0.9.1/docs/healpix.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/index.rst` & `reproject-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/installation.rst` & `reproject-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/make.bat` & `reproject-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reproject-0.9/docs/mosaicking.rst` & `reproject-0.9.1/docs/mosaicking.rst`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/__init__.py` & `reproject-0.9.1/reproject/__init__.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/_astropy_init.py` & `reproject-0.9.1/reproject/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/_compiler.c` & `reproject-0.9.1/reproject/_compiler.c`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/core.py` & `reproject-0.9.1/reproject/adaptive/core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/deforest.pyx` & `reproject-0.9.1/reproject/adaptive/deforest.pyx`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/high_level.py` & `reproject-0.9.1/reproject/adaptive/high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_2d.fits` & `reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_2d.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_2d_rotated.fits` & `reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_2d_rotated.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_roundtrip.fits` & `reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_roundtrip.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/tests/reference/test_reproject_adaptive_uncentered_jacobian.fits` & `reproject-0.9.1/reproject/adaptive/tests/reference/test_reproject_adaptive_uncentered_jacobian.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/adaptive/tests/test_core.py` & `reproject-0.9.1/reproject/adaptive/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/array_utils.py` & `reproject-0.9.1/reproject/array_utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/conftest.py` & `reproject-0.9.1/reproject/conftest.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/core.py` & `reproject-0.9.1/reproject/healpix/core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/high_level.py` & `reproject-0.9.1/reproject/healpix/high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/tests/data/bayestar.fits.gz` & `reproject-0.9.1/reproject/healpix/tests/data/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/tests/data/reference_result.fits` & `reproject-0.9.1/reproject/healpix/tests/data/reference_result.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/tests/test_healpix.py` & `reproject-0.9.1/reproject/healpix/tests/test_healpix.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/tests/test_utils.py` & `reproject-0.9.1/reproject/healpix/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/healpix/utils.py` & `reproject-0.9.1/reproject/healpix/utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/core.py` & `reproject-0.9.1/reproject/interpolation/core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/high_level.py` & `reproject-0.9.1/reproject/interpolation/high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/tests/reference/test_reproject_celestial_2d_gal2equ.fits` & `reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_celestial_2d_gal2equ.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/tests/reference/test_reproject_celestial_3d_equ2gal.fits` & `reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_celestial_3d_equ2gal.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/tests/reference/test_reproject_roundtrip.fits` & `reproject-0.9.1/reproject/interpolation/tests/reference/test_reproject_roundtrip.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/tests/reference/test_small_cutout.fits` & `reproject-0.9.1/reproject/interpolation/tests/reference/test_small_cutout.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/interpolation/tests/test_core.py` & `reproject-0.9.1/reproject/interpolation/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/background.py` & `reproject-0.9.1/reproject/mosaicking/background.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/coadd.py` & `reproject-0.9.1/reproject/mosaicking/coadd.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/subset_array.py` & `reproject-0.9.1/reproject/mosaicking/subset_array.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/tests/reference/test_coadd_solar_map.fits` & `reproject-0.9.1/reproject/mosaicking/tests/reference/test_coadd_solar_map.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/tests/test_background.py` & `reproject-0.9.1/reproject/mosaicking/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/tests/test_coadd.py` & `reproject-0.9.1/reproject/mosaicking/tests/test_coadd.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/tests/test_subset_array.py` & `reproject-0.9.1/reproject/mosaicking/tests/test_subset_array.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/tests/test_wcs_helpers.py` & `reproject-0.9.1/reproject/mosaicking/tests/test_wcs_helpers.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/mosaicking/wcs_helpers.py` & `reproject-0.9.1/reproject/mosaicking/wcs_helpers.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/_overlap.pyx` & `reproject-0.9.1/reproject/spherical_intersect/_overlap.pyx`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/core.py` & `reproject-0.9.1/reproject/spherical_intersect/core.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/high_level.py` & `reproject-0.9.1/reproject/spherical_intersect/high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/overlap.py` & `reproject-0.9.1/reproject/spherical_intersect/overlap.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/overlapArea.c` & `reproject-0.9.1/reproject/spherical_intersect/overlapArea.c`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/overlapAreaPP.c` & `reproject-0.9.1/reproject/spherical_intersect/overlapAreaPP.c`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/reproject_slice_c.c` & `reproject-0.9.1/reproject/spherical_intersect/reproject_slice_c.c`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/setup_package.py` & `reproject-0.9.1/reproject/spherical_intersect/setup_package.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/tests/test_high_level.py` & `reproject-0.9.1/reproject/spherical_intersect/tests/test_high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/tests/test_overlap.py` & `reproject-0.9.1/reproject/spherical_intersect/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/spherical_intersect/tests/test_reproject.py` & `reproject-0.9.1/reproject/spherical_intersect/tests/test_reproject.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/aia_171_level1.asdf` & `reproject-0.9.1/reproject/tests/data/aia_171_level1.asdf`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/aia_171_level1.fits` & `reproject-0.9.1/reproject/tests/data/aia_171_level1.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/cube.hdr` & `reproject-0.9.1/reproject/tests/data/cube.hdr`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/equatorial_3d.fits` & `reproject-0.9.1/reproject/tests/data/equatorial_3d.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/galactic_2d.fits` & `reproject-0.9.1/reproject/tests/data/galactic_2d.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/gc_eq.hdr` & `reproject-0.9.1/reproject/tests/data/gc_eq.hdr`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/gc_ga.hdr` & `reproject-0.9.1/reproject/tests/data/gc_ga.hdr`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/mwpan2_RGB_3600.hdr` & `reproject-0.9.1/reproject/tests/data/mwpan2_RGB_3600.hdr`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/secchi_l0_a.fits` & `reproject-0.9.1/reproject/tests/data/secchi_l0_a.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/data/secchi_l0_b.fits` & `reproject-0.9.1/reproject/tests/data/secchi_l0_b.fits`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/test_high_level.py` & `reproject-0.9.1/reproject/tests/test_high_level.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/tests/test_utils.py` & `reproject-0.9.1/reproject/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/utils.py` & `reproject-0.9.1/reproject/utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject/wcs_utils.py` & `reproject-0.9.1/reproject/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/reproject.egg-info/PKG-INFO` & `reproject-0.9.1/reproject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reproject
-Version: 0.9
+Version: 0.9.1
 Summary: Reproject astronomical images
 Home-page: https://reproject.readthedocs.io
 Author: Thomas Robitaille, Christoph Deil, Adam Ginsburg
 Author-email: thomas.robitaille@gmail.com
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `reproject-0.9/reproject.egg-info/SOURCES.txt` & `reproject-0.9.1/reproject.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
```

### Comparing `reproject-0.9/setup.cfg` & `reproject-0.9.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = reproject
 author = Thomas Robitaille, Christoph Deil, Adam Ginsburg
 author_email = thomas.robitaille@gmail.com
 license = BSD 3-Clause
-license_file = LICENSE
+license_files = LICENSE
 url = https://reproject.readthedocs.io
 description = Reproject astronomical images
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = False
 github_project = astropy/reproject
 
@@ -56,14 +56,16 @@
 	error
 	ignore:numpy\.ufunc size changed:RuntimeWarning
 	ignore:numpy\.ndarray size changed:RuntimeWarning
 	ignore:distutils Version classes are deprecated:DeprecationWarning
 	ignore:No observer defined on WCS:astropy.utils.exceptions.AstropyUserWarning
 	ignore:unclosed file:ResourceWarning
 	ignore:The conversion of these 2D helioprojective coordinates to 3D is all NaNs
+	ignore:'xdrlib' is deprecated and slated for removal in Python 3.13
+	ignore:'cgi' is deprecated and slated for removal in Python 3.13
 
 [coverage:run]
 omit = 
 	reproject/_astropy_init*
 	reproject/conftest.py
 	reproject/*setup_package*
 	reproject/tests/*
```

### Comparing `reproject-0.9/setup.py` & `reproject-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `reproject-0.9/tox.ini` & `reproject-0.9.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 [tox]
 envlist =
-    py{37,38,39,310}-{test}{-oldestdeps,-numpy121}
+    py{37,38,39,310,311}-{test}{-oldestdeps,-numpy121}
     build_docs
     codestyle
 isolated_build = True
-indexserver =
-    NIGHTLY = https://pypi.anaconda.org/scipy-wheels-nightly/simple
-    ASTROPY = https://pkgs.dev.azure.com/astropy-project/astropy/_packaging/nightly/pypi/simple/
 
 [testenv]
 whitelist_externals =
     geos-config
 passenv =
     SSL_CERT_FILE
 setenv =
     HOME = {envtmpdir}
     MPLBACKEND = Agg
-    PYTEST_COMMAND = pytest --arraydiff --arraydiff-default-format=fits --pyargs reproject --cov reproject --cov-config={toxinidir}/setup.cfg {toxinidir}/docs 
+    PYTEST_COMMAND = pytest --arraydiff --arraydiff-default-format=fits --pyargs reproject --cov reproject --cov-config={toxinidir}/setup.cfg {toxinidir}/docs
 changedir =
     .tmp/{envname}
 deps =
     numpy121: numpy==1.21.*
 
     oldestdeps: numpy==1.17.3
     oldestdeps: astropy==4.0.*
     oldestdeps: astropy-healpix==0.6
     oldestdeps: scipy==1.3.2
 
-    devdeps: :NIGHTLY:numpy
-    devdeps: :NIGHTLY:scipy
-    devdeps: :ASTROPY:astropy
+    devdeps: numpy>=0.0.dev0
+    devdeps: scipy>=0.0.dev0
+    devdeps: astropy>=0.0.dev0
     devdeps: git+https://github.com/asdf-format/asdf.git#egg=asdf
     devdeps: git+https://github.com/astropy/asdf-astropy.git
     devdeps: git+https://github.com/spacetelescope/gwcs.git#egg=gwcs
     devdeps: git+https://github.com/sunpy/sunpy.git#egg=sunpy
 extras =
     test
     # Don't run the more complex tests on oldestdeps because it pulls in a nest
```

