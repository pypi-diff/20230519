# Comparing `tmp/sentry_cli-2.17.5.tar.gz` & `tmp/sentry_cli-2.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.17.5.tar", last modified: Fri Apr 28 07:57:03 2023, max compression
+gzip compressed data, was "sentry_cli-2.18.0.tar", last modified: Fri May 19 17:06:17 2023, max compression
```

## Comparing `sentry_cli-2.17.5.tar` & `sentry_cli-2.18.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.841531 sentry_cli-2.17.5/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.703009 sentry_cli-2.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-19 17:06:17.707009 sentry_cli-2.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.687009 sentry_cli-2.18.0/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-19 17:06:17.000000 sentry_cli-2.18.0/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-19 17:06:17.000000 sentry_cli-2.18.0/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:06:17.000000 sentry_cli-2.18.0/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:06:17.000000 sentry_cli-2.18.0/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-19 17:06:17.707009 sentry_cli-2.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.687009 sentry_cli-2.18.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87498 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.687009 sentry_cli-2.18.0/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.691009 sentry_cli-2.18.0/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.695009 sentry_cli-2.18.0/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.695009 sentry_cli-2.18.0/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.695009 sentry_cli-2.18.0/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.695009 sentry_cli-2.18.0/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.695009 sentry_cli-2.18.0/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.699009 sentry_cli-2.18.0/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.703009 sentry_cli-2.18.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.703009 sentry_cli-2.18.0/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:06:17.703009 sentry_cli-2.18.0/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36411 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-05-19 17:05:52.000000 sentry_cli-2.18.0/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.17.5/Cargo.lock` & `sentry_cli-2.18.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2155,51 +2155,51 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "sentry"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c3d7f8bf7373e75222452fcdd9347d857452a92d0eec738f941bc4656c5b5df"
+checksum = "37dd6c0cdca6b1d1ca44cde7fff289f2592a97965afec870faa7b81b9fc87745"
 dependencies = [
  "curl",
  "httpdate",
  "sentry-anyhow",
  "sentry-contexts",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-anyhow"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ef7f47c57a1146d553b4976f20e8bba370195a88858bdf6945a63c529549236"
+checksum = "d9c3d7032fff178c77c107c32c6d3337b12847adf67165ccc876c898e7154b00"
 dependencies = [
  "anyhow",
  "sentry-backtrace",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-backtrace"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03b7cdefbdca51f1146f0f24a3cb4ecb6428951f030ff5c720cfb5c60bd174c0"
+checksum = "c029fe8317cdd75cb2b52c600bab4e2ef64c552198e669ba874340447f330962"
 dependencies = [
  "backtrace",
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.17.5"
+version = "2.18.0"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2261,44 +2261,44 @@
  "which",
  "winapi 0.3.9",
  "zip",
 ]
 
 [[package]]
 name = "sentry-contexts"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6af4cb29066e0e8df0cc3111211eb93543ccb09e1ccbe71de6d88b4bb459a2b1"
+checksum = "bc575098d73c8b942b589ab453b06e4c43527556dd8f95532220d1b54d7c6b4b"
 dependencies = [
  "hostname",
  "libc",
  "os_info",
  "rustc_version 0.4.0",
  "sentry-core",
  "uname",
 ]
 
 [[package]]
 name = "sentry-core"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e781b55761e47a60d1ff326ae8059de22b0e6b0cee68eab1c5912e4fb199a76"
+checksum = "20216140001bbf05895f013abd0dae4df58faee24e016d54cbf107f070bac56b"
 dependencies = [
  "once_cell",
  "rand",
  "sentry-types",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "sentry-types"
-version = "0.31.0"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d642a04657cc77d8de52ae7c6d93a15cb02284eb219344a89c1e2b26bbaf578c"
+checksum = "d7f6959d8cb3a77be27e588eef6ce9a2a469651a556d9de662e4d07e5ace4232"
 dependencies = [
  "debugid",
  "getrandom",
  "hex",
  "serde",
  "serde_json",
  "thiserror",
```

### Comparing `sentry_cli-2.17.5/Cargo.toml` & `sentry_cli-2.18.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.17.5"
+version = "2.18.0"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -53,15 +53,15 @@
 proguard = { version = "5.0.0", features = ["uuid"] }
 r2d2 = "0.8.10"
 rayon = "1.6.1"
 regex = "1.7.1"
 runas = "1.0.0"
 rust-ini = "0.18.0"
 semver = "1.0.16"
-sentry = { version = "0.31.0", default-features = false, features = [
+sentry = { version = "0.31.1", default-features = false, features = [
   "anyhow",
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
```

### Comparing `sentry_cli-2.17.5/LICENSE` & `sentry_cli-2.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/PKG-INFO` & `sentry_cli-2.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.17.5
+Version: 2.18.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.5 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.18.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.5/README.md` & `sentry_cli-2.18.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/build.rs` & `sentry_cli-2.18.0/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.18.0/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.17.5
+Version: 2.18.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.5 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.18.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.5/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.18.0/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/setup.cfg` & `sentry_cli-2.18.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/setup.py` & `sentry_cli-2.18.0/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/api.rs` & `sentry_cli-2.18.0/src/api.rs`

 * *Files 0% similar despite different names*

```diff
@@ -2486,27 +2486,31 @@
 }
 
 #[derive(Debug, Deserialize)]
 pub struct MonitorCheckIn {
     pub id: Uuid,
     pub status: Option<MonitorCheckinStatus>,
     pub duration: Option<u64>,
+    pub environment: Option<String>,
 }
 
 #[derive(Debug, Serialize)]
 pub struct CreateMonitorCheckIn {
     pub status: MonitorCheckinStatus,
+    pub environment: String,
 }
 
 #[derive(Debug, Serialize, Default)]
 pub struct UpdateMonitorCheckIn {
     #[serde(skip_serializing_if = "Option::is_none")]
     pub status: Option<MonitorCheckinStatus>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub duration: Option<u64>,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub environment: Option<String>,
 }
 
 #[derive(Deserialize, Debug)]
 pub struct RepoProvider {
     pub id: String,
     pub name: String,
 }
```

### Comparing `sentry_cli-2.17.5/src/bashsupport.sh` & `sentry_cli-2.18.0/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/bash_hook.rs` & `sentry_cli-2.18.0/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.18.0/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.18.0/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/check.rs` & `sentry_cli-2.18.0/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/find.rs` & `sentry_cli-2.18.0/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/mod.rs` & `sentry_cli-2.18.0/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.18.0/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/debug_files/upload.rs` & `sentry_cli-2.18.0/src/commands/debug_files/upload.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::collections::BTreeSet;
 use std::str::{self, FromStr};
 
 use anyhow::{bail, format_err, Result};
 use clap::{builder::PossibleValuesParser, Arg, ArgAction, ArgMatches, Command};
 use console::style;
+use itertools::Itertools;
 use log::info;
 use symbolic::common::DebugId;
 use symbolic::debuginfo::FileFormat;
 
 use crate::api::Api;
 use crate::config::Config;
 use crate::utils::args::ArgExt;
@@ -16,16 +17,20 @@
 use crate::utils::progress::{ProgressBar, ProgressStyle};
 use crate::utils::system::QuietExit;
 use crate::utils::xcode::{InfoPlist, MayDetach};
 
 static DERIVED_DATA_FOLDER: &str = "Library/Developer/Xcode/DerivedData";
 
 pub fn make_command(command: Command) -> Command {
-    let mut types = vec!["bcsymbolmap"];
-    types.extend(DifType::all_names());
+    let types = DifType::all_names()
+        .iter()
+        .filter(|&name| name != &"proguard")
+        .chain(&["bcsymbolmap"])
+        .sorted_by(|a, b| Ord::cmp(&a, &b))
+        .collect::<Vec<_>>();
 
     command
         .about("Upload debugging information files.")
         .org_arg()
         .project_arg(false)
         .arg(
             Arg::new("paths")
```

### Comparing `sentry_cli-2.17.5/src/commands/deploys/list.rs` & `sentry_cli-2.18.0/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/deploys/mod.rs` & `sentry_cli-2.18.0/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/deploys/new.rs` & `sentry_cli-2.18.0/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/events/list.rs` & `sentry_cli-2.18.0/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/events/mod.rs` & `sentry_cli-2.18.0/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/files/delete.rs` & `sentry_cli-2.18.0/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/files/list.rs` & `sentry_cli-2.18.0/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/files/mod.rs` & `sentry_cli-2.18.0/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/files/upload.rs` & `sentry_cli-2.18.0/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/info.rs` & `sentry_cli-2.18.0/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/issues/mod.rs` & `sentry_cli-2.18.0/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/issues/mute.rs` & `sentry_cli-2.18.0/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/issues/resolve.rs` & `sentry_cli-2.18.0/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/issues/unresolve.rs` & `sentry_cli-2.18.0/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/login.rs` & `sentry_cli-2.18.0/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/mod.rs` & `sentry_cli-2.18.0/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/monitors/list.rs` & `sentry_cli-2.18.0/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/monitors/mod.rs` & `sentry_cli-2.18.0/src/commands/repos/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 use anyhow::Result;
 use clap::{ArgMatches, Command};
 
+use crate::utils::args::ArgExt;
+
 pub mod list;
-pub mod run;
 
 macro_rules! each_subcommand {
     ($mac:ident) => {
         $mac!(list);
-        $mac!(run);
     };
 }
 
 pub fn make_command(mut command: Command) -> Command {
     macro_rules! add_subcommand {
         ($name:ident) => {{
-            command = command.subcommand(crate::commands::monitors::$name::make_command(
+            command = command.subcommand(crate::commands::repos::$name::make_command(
                 Command::new(stringify!($name).replace('_', "-")),
             ));
         }};
     }
 
     command = command
-        .about("Manage monitors on Sentry.")
+        .about("Manage repositories on Sentry.")
         .subcommand_required(true)
         .arg_required_else_help(true)
-        // Beta feature Left hidden while we iterate on this product
-        .hide(true);
-
+        .org_arg();
     each_subcommand!(add_subcommand);
     command
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     macro_rules! execute_subcommand {
         ($name:ident) => {{
             if let Some(sub_matches) =
                 matches.subcommand_matches(&stringify!($name).replace('_', "-"))
             {
-                return crate::commands::monitors::$name::execute(&sub_matches);
+                return crate::commands::repos::$name::execute(&sub_matches);
             }
         }};
     }
     each_subcommand!(execute_subcommand);
     unreachable!();
 }
```

### Comparing `sentry_cli-2.17.5/src/commands/monitors/run.rs` & `sentry_cli-2.18.0/src/commands/monitors/run.rs`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,20 @@
         .arg(
             Arg::new("monitor_slug")
                 .value_name("monitor-slug")
                 .help("The monitor slug.")
                 .required(true),
         )
         .arg(
+            Arg::new("environment")
+                .short('e')
+                .default_value("production")
+                .help("Specify the environment of the monitor."),
+        )
+        .arg(
             Arg::new("allow_failure")
                 .short('f')
                 .long("allow-failure")
                 .action(ArgAction::SetTrue)
                 .help("Run provided command even when Sentry reports an error."),
         )
         .arg(
@@ -43,23 +49,25 @@
     // Token based auth is deprecated, prefer DSN style auth for monitor checkins.
     // Using token based auth *DOES NOT WORK* when using slugs.
     if dsn.is_none() {
         warn!("Token auth is deprecated for cron monitor checkins. Please use DSN auth.");
     }
 
     let monitor_slug = matches.get_one::<String>("monitor_slug").unwrap();
+    let environment = matches.get_one::<String>("environment").unwrap();
 
     let allow_failure = matches.get_flag("allow_failure");
     let args: Vec<_> = matches.get_many::<String>("args").unwrap().collect();
 
     let monitor_checkin = api.create_monitor_checkin(
         dsn.clone(),
         monitor_slug,
         &CreateMonitorCheckIn {
             status: MonitorCheckinStatus::InProgress,
+            environment: environment.to_string(),
         },
     );
 
     let started = Instant::now();
     let mut p = process::Command::new(args[0]);
     p.args(&args[1..]);
     p.env("SENTRY_MONITOR_SLUG", monitor_slug);
@@ -89,14 +97,15 @@
                     } else {
                         MonitorCheckinStatus::Error
                     }),
                     duration: Some({
                         let elapsed = started.elapsed();
                         elapsed.as_secs() * 1000 + u64::from(elapsed.subsec_millis())
                     }),
+                    environment: Some(environment.to_string()),
                 },
             )
             .ok();
         }
         Err(e) => {
             if allow_failure {
                 print_error(&anyhow::Error::from(e));
```

### Comparing `sentry_cli-2.17.5/src/commands/organizations/list.rs` & `sentry_cli-2.18.0/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/organizations/mod.rs` & `sentry_cli-2.18.0/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/projects/list.rs` & `sentry_cli-2.18.0/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/projects/mod.rs` & `sentry_cli-2.18.0/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/react_native/appcenter.rs` & `sentry_cli-2.18.0/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/react_native/gradle.rs` & `sentry_cli-2.18.0/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/react_native/mod.rs` & `sentry_cli-2.18.0/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/react_native/xcode.rs` & `sentry_cli-2.18.0/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/archive.rs` & `sentry_cli-2.18.0/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/delete.rs` & `sentry_cli-2.18.0/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/finalize.rs` & `sentry_cli-2.18.0/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/info.rs` & `sentry_cli-2.18.0/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/list.rs` & `sentry_cli-2.18.0/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/mod.rs` & `sentry_cli-2.18.0/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/new.rs` & `sentry_cli-2.18.0/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/restore.rs` & `sentry_cli-2.18.0/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/releases/set_commits.rs` & `sentry_cli-2.18.0/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/repos/list.rs` & `sentry_cli-2.18.0/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/repos/mod.rs` & `sentry_cli-2.18.0/src/commands/monitors/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 use anyhow::Result;
 use clap::{ArgMatches, Command};
 
-use crate::utils::args::ArgExt;
-
 pub mod list;
+pub mod run;
 
 macro_rules! each_subcommand {
     ($mac:ident) => {
         $mac!(list);
+        $mac!(run);
     };
 }
 
 pub fn make_command(mut command: Command) -> Command {
     macro_rules! add_subcommand {
         ($name:ident) => {{
-            command = command.subcommand(crate::commands::repos::$name::make_command(
+            command = command.subcommand(crate::commands::monitors::$name::make_command(
                 Command::new(stringify!($name).replace('_', "-")),
             ));
         }};
     }
 
     command = command
-        .about("Manage repositories on Sentry.")
+        .about("Manage monitors on Sentry [beta].")
         .subcommand_required(true)
-        .arg_required_else_help(true)
-        .org_arg();
+        .arg_required_else_help(true);
+
     each_subcommand!(add_subcommand);
     command
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     macro_rules! execute_subcommand {
         ($name:ident) => {{
             if let Some(sub_matches) =
                 matches.subcommand_matches(&stringify!($name).replace('_', "-"))
             {
-                return crate::commands::repos::$name::execute(&sub_matches);
+                return crate::commands::monitors::$name::execute(&sub_matches);
             }
         }};
     }
     each_subcommand!(execute_subcommand);
     unreachable!();
 }
```

### Comparing `sentry_cli-2.17.5/src/commands/send_envelope.rs` & `sentry_cli-2.18.0/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/send_event.rs` & `sentry_cli-2.18.0/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.18.0/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.18.0/src/commands/sourcemaps/inject.rs`

 * *Files 10% similar despite different names*

```diff
@@ -85,26 +85,25 @@
         .get_many::<String>("ignore")
         .map(|ignores| ignores.map(|i| format!("!{i}")).collect())
         .unwrap_or_else(Vec::new);
 
     let mut extensions = matches
         .get_many::<String>("extensions")
         .map(|extensions| extensions.map(|ext| ext.trim_start_matches('.')).collect())
-        .unwrap_or_else(Vec::new);
-    if extensions.is_empty() {
-        extensions.push("js");
-        extensions.push("cjs");
-        extensions.push("mjs");
-    }
+        .unwrap_or_else(|| vec!["js", "cjs", "mjs"]);
+
+    // Sourcemaps should be discovered regardless of which JavaScript extensions have been selected.
+    extensions.push("map");
 
     for path in paths {
         println!("> Searching {}", path.display());
         let sources = ReleaseFileSearch::new(path)
             .ignore_file(ignore_file)
             .ignores(&ignores)
+            .extensions(extensions.clone())
             .collect_files()?;
         for source in sources {
             let url = path_as_url(&source.path);
             processor.add(&url, source)?;
         }
     }
```

### Comparing `sentry_cli-2.17.5/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.18.0/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.18.0/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.18.0/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/uninstall.rs` & `sentry_cli-2.18.0/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/update.rs` & `sentry_cli-2.18.0/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/commands/upload_proguard.rs` & `sentry_cli-2.18.0/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/config.rs` & `sentry_cli-2.18.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/constants.rs` & `sentry_cli-2.18.0/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/android.rs` & `sentry_cli-2.18.0/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/appcenter.rs` & `sentry_cli-2.18.0/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/args.rs` & `sentry_cli-2.18.0/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/chunks.rs` & `sentry_cli-2.18.0/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/codepush.rs` & `sentry_cli-2.18.0/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/cordova.rs` & `sentry_cli-2.18.0/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/dif.rs` & `sentry_cli-2.18.0/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/dif_upload.rs` & `sentry_cli-2.18.0/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/enc.rs` & `sentry_cli-2.18.0/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/event.rs` & `sentry_cli-2.18.0/src/utils/event.rs`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 pub fn with_sentry_client<F, R>(dsn: Dsn, callback: F) -> R
 where
     F: FnOnce(&Client) -> R,
 {
     let client = Client::from_config((
         dsn,
         apply_defaults(ClientOptions {
+            // TODO: do we want to eventually set `debug` based on the CLI log-level?
+            // debug: true,
             user_agent: USER_AGENT.into(),
             ..Default::default()
         }),
     ));
 
     let rv = callback(&client);
     client.close(Some(Duration::from_secs(2)));
```

### Comparing `sentry_cli-2.17.5/src/utils/file_search.rs` & `sentry_cli-2.18.0/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/file_upload.rs` & `sentry_cli-2.18.0/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/formatting.rs` & `sentry_cli-2.18.0/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/fs.rs` & `sentry_cli-2.18.0/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/http.rs` & `sentry_cli-2.18.0/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/logging.rs` & `sentry_cli-2.18.0/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/progress.rs` & `sentry_cli-2.18.0/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/releases.rs` & `sentry_cli-2.18.0/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/retry.rs` & `sentry_cli-2.18.0/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.18.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.18.0/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/sourcemaps.rs` & `sentry_cli-2.18.0/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/system.rs` & `sentry_cli-2.18.0/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/ui.rs` & `sentry_cli-2.18.0/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/update.rs` & `sentry_cli-2.18.0/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/vcs.rs` & `sentry_cli-2.18.0/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.5/src/utils/xcode.rs` & `sentry_cli-2.18.0/src/utils/xcode.rs`

 * *Files identical despite different names*

