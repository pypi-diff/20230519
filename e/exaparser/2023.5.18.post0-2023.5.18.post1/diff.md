# Comparing `tmp/exaparser-2023.5.18.post0.tar.gz` & `tmp/exaparser-2023.5.18.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exaparser-2023.5.18.post0.tar", last modified: Thu May 18 19:21:21 2023, max compression
+gzip compressed data, was "exaparser-2023.5.18.post1.tar", last modified: Thu May 18 23:41:09 2023, max compression
```

## Comparing `exaparser-2023.5.18.post0.tar` & `exaparser-2023.5.18.post1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/data/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/data/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/exabyte.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/job/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/job/compute/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/job/compute/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.912169 exaparser-2023.5.18.post0/exaparser/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/vasp.json
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/subworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/espresso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.912169 exaparser-2023.5.18.post0/exaparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/job.rms
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   160469 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   377892 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   160388 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pw-scf.in
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CHG
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CHGCAR
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CONTCAR
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/DOSCAR
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/EIGENVAL
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/IBZKPT
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/INCAR
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/KPOINTS
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OSZICAR
--rw-r--r--   0 runner    (1001) docker     (123)    53180 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/PCDAT
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POTCAR
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/WAVECAR
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/XDATCAR
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/job.rms
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    37663 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/integration/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.727234 exaparser-2023.5.18.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/data/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/handlers/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/handlers/exabyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/data/handlers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/job/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/compute/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/job/compute/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/compute/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/compute/managers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/job/compute/managers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/templates/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/templates/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/templates/vasp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.731233 exaparser-2023.5.18.post1/exaparser/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/subworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser/workflow/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/espresso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/shell_with_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/units/subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/exaparser/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.735234 exaparser-2023.5.18.post1/exaparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 23:41:09.000000 exaparser-2023.5.18.post1/exaparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.739234 exaparser-2023.5.18.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.727234 exaparser-2023.5.18.post1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.739234 exaparser-2023.5.18.post1/tests/fixtures/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.739234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/job.rms
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.727234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.739234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160469 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.743234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   377892 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160388 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.747234 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.747234 exaparser-2023.5.18.post1/tests/fixtures/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/CHG
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/CHGCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/CONTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/DOSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/EIGENVAL
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/IBZKPT
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/OSZICAR
+-rw-r--r--   0 runner    (1001) docker     (123)    53180 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/PCDAT
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/WAVECAR
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/XDATCAR
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/job.rms
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    37663 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/integration/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:41:09.751234 exaparser-2023.5.18.post1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:40:29.000000 exaparser-2023.5.18.post1/tests/utils.py
```

### Comparing `exaparser-2023.5.18.post0/.github/workflows/cicd.yml` & `exaparser-2023.5.18.post1/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/.gitignore` & `exaparser-2023.5.18.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/LICENSE` & `exaparser-2023.5.18.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/PKG-INFO` & `exaparser-2023.5.18.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2023.5.18.post0
+Version: 2023.5.18.post1
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
```

### Comparing `exaparser-2023.5.18.post0/README.md` & `exaparser-2023.5.18.post1/README.md`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/config` & `exaparser-2023.5.18.post1/config`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # directory to store the job if DISK data handler is enabled
 data_dir = .exabyte
 
 [exabyte_api_data_handler]
 # Exabyte RESTful API Data Handler Settings
 # See https://docs.exabyte.io/rest-api/overview for more information.
-hostname = platform.exabyte.io
+hostname = platform.mat3ra.com
 port = 443
 account_id = zX6Wf8QdQkgEpP26u
 auth_token = 8YpFg97E-zN17xP9bqngoGFJV8mBXT553zh8iE9a0nP
 secure = True
 version = 2018-10-01
 
 # Number of workers used for uploading files in parallel
```

### Comparing `exaparser-2023.5.18.post0/exaparser/cli.py` & `exaparser-2023.5.18.post1/exaparser/cli.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/config.py` & `exaparser-2023.5.18.post1/exaparser/config.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/data/factory.py` & `exaparser-2023.5.18.post1/exaparser/data/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/data/handlers/disk.py` & `exaparser-2023.5.18.post1/exaparser/data/handlers/disk.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/data/handlers/exabyte.py` & `exaparser-2023.5.18.post1/exaparser/data/handlers/exabyte.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/enums.py` & `exaparser-2023.5.18.post1/exaparser/enums.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/job/__init__.py` & `exaparser-2023.5.18.post1/exaparser/job/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/job/compute/__init__.py` & `exaparser-2023.5.18.post1/exaparser/job/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/templates/espresso.json` & `exaparser-2023.5.18.post1/exaparser/templates/espresso.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/templates/shell.json` & `exaparser-2023.5.18.post1/exaparser/templates/shell.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/templates/vasp.json` & `exaparser-2023.5.18.post1/exaparser/templates/vasp.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/utils.py` & `exaparser-2023.5.18.post1/exaparser/utils.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/subworkflow.py` & `exaparser-2023.5.18.post1/exaparser/workflow/subworkflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/__init__.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/__init__.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/__init__.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/espresso.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/espresso.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/vasp.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/modeling/vasp.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/shell.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/execution/scripting/shell_with_results.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/factory.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/units/subworkflow.py` & `exaparser-2023.5.18.post1/exaparser/workflow/units/subworkflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser/workflow/workflow.py` & `exaparser-2023.5.18.post1/exaparser/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/exaparser.egg-info/PKG-INFO` & `exaparser-2023.5.18.post1/exaparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2023.5.18.post0
+Version: 2023.5.18.post1
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
```

### Comparing `exaparser-2023.5.18.post0/exaparser.egg-info/SOURCES.txt` & `exaparser-2023.5.18.post1/exaparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/requirements-dev.txt` & `exaparser-2023.5.18.post1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/requirements.txt` & `exaparser-2023.5.18.post1/requirements.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/run-tests.sh` & `exaparser-2023.5.18.post1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/setup.cfg` & `exaparser-2023.5.18.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/__init__.py` & `exaparser-2023.5.18.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/shell-job.json` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pw-scf.in` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/pw-scf.in`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/stdout` & `exaparser-2023.5.18.post1/tests/fixtures/espresso/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/shell-job.json` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CONTCAR` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/CONTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/DOSCAR` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/DOSCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/EIGENVAL` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/EIGENVAL`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OSZICAR` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/OSZICAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OUTCAR` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/OUTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POTCAR` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/POTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/stdout` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/vasprun.xml` & `exaparser-2023.5.18.post1/tests/fixtures/vasp/test-001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2023.5.18.post0/tests/integration/test_job.py` & `exaparser-2023.5.18.post1/tests/integration/test_job.py`

 * *Files identical despite different names*

