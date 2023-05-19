# Comparing `tmp/phiterm-1.6.4.tar.gz` & `tmp/phiterm-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.4.tar", last modified: Wed May 17 22:34:35 2023, max compression
+gzip compressed data, was "phiterm-1.6.5.tar", last modified: Fri May 19 09:06:06 2023, max compression
```

## Comparing `phiterm-1.6.4.tar` & `phiterm-1.6.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.523362 phiterm-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-17 22:34:14.000000 phiterm-1.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-17 22:34:35.523362 phiterm-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 22:34:14.000000 phiterm-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.507361 phiterm-1.6.4/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.507361 phiterm-1.6.4/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.507361 phiterm-1.6.4/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35062 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.511361 phiterm-1.6.4/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.507361 phiterm-1.6.4/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.515361 phiterm-1.6.4/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.519362 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.519362 phiterm-1.6.4/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.519362 phiterm-1.6.4/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.519362 phiterm-1.6.4/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.519362 phiterm-1.6.4/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.523362 phiterm-1.6.4/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-17 22:34:14.000000 phiterm-1.6.4/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.507361 phiterm-1.6.4/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 22:34:35.000000 phiterm-1.6.4/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 22:34:14.000000 phiterm-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:34:35.523362 phiterm-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 22:34:14.000000 phiterm-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:34:35.523362 phiterm-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 22:34:14.000000 phiterm-1.6.4/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-19 09:05:46.000000 phiterm-1.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 09:06:06.966987 phiterm-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 09:05:46.000000 phiterm-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.950986 phiterm-1.6.5/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.950986 phiterm-1.6.5/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45239 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-19 09:05:46.000000 phiterm-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:06:06.966987 phiterm-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 09:05:46.000000 phiterm-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 09:05:46.000000 phiterm-1.6.5/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.4/LICENSE.md` & `phiterm-1.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/api/client.py` & `phiterm-1.6.5/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/api/routes.py` & `phiterm-1.6.5/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/api/user.py` & `phiterm-1.6.5/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/api/workspace.py` & `phiterm-1.6.5/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/aws/aws_operator.py` & `phiterm-1.6.5/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/cli_app.py` & `phiterm-1.6.5/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/cli_operator.py` & `phiterm-1.6.5/phiterm/cli/cli_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     phi_conf.user = user
     print_info("Welcome {}, you are now logged in\n".format(user.email))
 
     return phi_conf.sync_workspaces_from_api()
 
 
 def initialize_phidata(reset: bool = False, login: bool = False) -> bool:
-    """This function is called by `phi init` and initializes phidata on the users machine.
+    """Initialize phidata on the users machine.
+
     Steps:
     1. Check if PHI_CONF_DIR exists, if not, create it. If reset == True, recreate PHI_CONF_DIR.
     2. Check if PhiConf exists, if it does, try and authenticate the user
         If the user is authenticated, phi is configured and authenticated. Return True.
     3. If PhiConf does not exist, create a new PhiConf. Return True.
     """
 
@@ -96,46 +97,44 @@
     if PHI_CONF_DIR.exists():
         logger.debug(f"{PHI_CONF_DIR} exists")
         if not PHI_CONF_DIR.is_dir():
             try:
                 delete_from_fs(PHI_CONF_DIR)
             except Exception as e:
                 logger.exception(e)
-                print_info(
-                    f"Something went wrong, please delete {PHI_CONF_DIR} and run `phi init` again"
+                raise Exception(
+                    f"Something went wrong, please delete {PHI_CONF_DIR} and run again"
                 )
-                return False
             PHI_CONF_DIR.mkdir(parents=True)
     else:
         PHI_CONF_DIR.mkdir(parents=True)
         logger.debug(f"created {PHI_CONF_DIR}")
 
     # Confirm PHI_CONF_DIR exists otherwise we should return
     if PHI_CONF_DIR.exists():
         logger.debug(f"Your phidata config is stored at: {PHI_CONF_DIR}")
     else:
-        print_info(f"Something went wrong, please run `phi init` again")
-        return False
+        raise Exception(f"Something went wrong, please run again")
 
     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
     if phi_conf is None:
         # Create a new PhiConf
         phi_conf = PhiConf()
 
     # Authenticate user
+    auth_success: bool = True
     if login:
         auth_success = authenticate_user()
 
-    if phi_conf is not None:
-        print_info("Phidata is initialized. Next steps:\n")
-        print_info(" 1. Run `phi ws create` to create a new workspace")
-        print_info(" 2. Run `phi ws setup` to setup an existing workspace")
-        print_info(" 3. Run `phi ws up -dr` to dry-run workspace deploy")
-        print_info(" 4. Run `phi ws up` to deploy the workspace")
-    return True
+    if phi_conf is not None and auth_success:
+        logger.info("Phidata initialized")
+        return True
+    else:
+        logger.error("Something went wrong, please run again")
+        return False
 
 
 def sign_in_using_cli() -> bool:
     from getpass import getpass
 
     print_heading("Log in")
     email_raw = input("email: ")
```

### Comparing `phiterm-1.6.4/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.5/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.5/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.5/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.5/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.5/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.5/phiterm/cli/ws/ws_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,157 +1,121 @@
 """Phi Workspace Cli
 
 This is the entrypoint for the `phi ws` commands
 """
+from pathlib import Path
 from typing import Optional, cast
 
 import typer
 
 from phiterm.utils.cli_console import (
     print_error,
     print_info,
     print_heading,
     print_available_workspaces,
     print_conf_not_available_msg,
     print_active_workspace_not_available,
 )
 from phiterm.utils.log import logger, set_log_level_to_debug
-from phiterm.workspace.ws_enums import (
-    WorkspaceEnv,
-    WorkspaceStarterTemplate,
-    WorkspaceConfigType,
-)
+from phiterm.workspace.ws_enums import WorkspaceConfigType
 
 ws_app = typer.Typer(
     name="ws",
     short_help="Manage workspaces",
     help="""\b
-Use `phi ws <command>` to create, setup or update your workspace.
+Use `phi ws <command>` to create, setup, start or stop your workspace.
 Run `phi ws <command> --help` for more info.
 """,
     no_args_is_help=True,
     add_completion=False,
     invoke_without_command=True,
     options_metavar="\b",
     subcommand_metavar="<command>",
 )
 
 
 @ws_app.command(short_help="Create a new workspace in the current directory.")
 def create(
-    ws_name: str = typer.Option(
-        None, "-ws", help="Name of the new workspace", show_default=False
-    ),
-    template: str = typer.Option(
-        "ml-app",
+    template: Optional[str] = typer.Option(
+        None,
         "-t",
         "--template",
-        help="Choose a starter template for the workspace",
-        show_default=True,
+        help="Starter template for the workspace.",
+        show_default=False,
+    ),
+    name: Optional[str] = typer.Option(
+        None,
+        "-n",
+        "--name",
+        help="Name of the new workspace.",
+        show_default=False,
     ),
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
 ):
     """\b
-    Creates a new workspace in the current directory using the selected starter template
-    [default: ml-app]
-
+    Create a new workspace in the current directory using a starter template
     \b
     Examples:
-    $ phi ws create            -> Create a new workspace
-    $ phi ws create -ws ml     -> Create a workspace named data using the default starter template (aws)
+    > phi ws create -t ai-app     -> Create an `ai-app` workspace in the current directory
+    > phi ws create -t ai-app -n ai  -> Create an `ai-app` workspace named `ai` in the current directory
     """
-    from phiterm.workspace.ws_operator import (
-        create_new_workspace,
-        initialize_workspace,
-    )
+    from phiterm.workspace.ws_operator import create_workspace
 
     if print_debug_log:
         set_log_level_to_debug()
 
-    if ws_name is None:
-        initialize_workspace()
-        return
-
-    if (
-        template is None
-        or template.lower() not in WorkspaceStarterTemplate.values_list()
-    ):
-        print_error(
-            f"{template} is not a supported template, please choose from: {WorkspaceStarterTemplate.values_list()}"
-        )
-        return
-    _template: WorkspaceStarterTemplate = cast(
-        WorkspaceStarterTemplate,
-        WorkspaceStarterTemplate.from_str(template),
-    )
-
-    create_new_workspace(ws_name, _template)
+    create_workspace(template=template, name=name)
 
 
 @ws_app.command(short_help="Setup phidata workspace from the current directory")
 def setup(
-    ws_name: str = typer.Option(None, "-ws", help="Name of the workspace to setup"),
+    path: Optional[str] = typer.Argument(
+        None,
+        help="Optional path to workspace.",
+        show_default=False,
+    ),
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
 ):
     """\b
-    Setup a phidata workspace from the current directory.
-    This command can be run from within the workspace directory
-        OR with a "-ws" flag to setup a workspace by name.
-
+    Setup a phidata workspace. This command can be run from the workspace directory OR using the workspace path.
     \b
     Examples:
-    $ `phi ws setup`           -> Setup the current directory as a phidata workspace
-    $ `phi ws setup -ws idata` -> Setup the workspace named idata
+    > `phi ws setup`           -> Setup the current directory as a workspace
+    > `phi ws setup ai-app`    -> Setup the `ai-app` folder as a workspace
     """
-    from pathlib import Path
     from phiterm.workspace.ws_operator import setup_workspace
 
     if print_debug_log:
         set_log_level_to_debug()
 
     # By default, we assume this command is run from the workspace directory
-    if ws_name is None:
-        # If the user does not provide a ws_name, that implies `phi ws setup` is ran from
-        # the workspace directory.
-        ws_path: Path = Path(".").resolve()
-        setup_workspace(ws_path)
-    else:
-        # If the user provides a workspace name manually, we find the dir for that ws and set it up
-        from phiterm.conf.phi_conf import PhiConf
-
-        phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
-        if not phi_conf:
-            print_conf_not_available_msg()
-            return
+    ws_root_path: Path = Path(".").resolve()
 
-        _ws_path: Optional[Path] = phi_conf.get_ws_root_path_by_name(ws_name)
-        if _ws_path is None:
-            print_error(f"Could not find workspace {ws_name}")
-            avl_ws = phi_conf.available_ws
-            if avl_ws:
-                print_available_workspaces(avl_ws)
-            return
-        setup_workspace(_ws_path)
+    # If the user provides a path, use that to setup the workspace
+    if path is not None:
+        ws_root_path = Path(".").joinpath(path).resolve()
+
+    setup_workspace(ws_root_path=ws_root_path)
 
 
 @ws_app.command(short_help="Create resources for active workspace")
 def up(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
+        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
         metavar="[FILTER]",
     ),
     env_filter: Optional[str] = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to deploy"
     ),
     config_filter: Optional[str] = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to deploy"
@@ -192,29 +156,29 @@
         "-f",
         "--force",
         help="Force",
     ),
 ):
     """\b
     Create resources for the active workspace.
-    Options can be used to limit the resources to deploy.
+    Options can be used to limit the resources to create.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
+    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
     \b
     Examples:
-    $ `phi ws up`            -> Deploy all resources
-    $ `phi ws up dev`        -> Deploy all dev resources
-    $ `phi ws up prd`        -> Deploy all prd resources
-    $ `phi ws up prd:aws`    -> Deploy all prd aws resources
-    $ `phi ws up prd:::s3`   -> Deploy prd resources matching name s3
+    > `phi ws up`            -> Deploy all resources
+    > `phi ws up dev`        -> Deploy all dev resources
+    > `phi ws up prd`        -> Deploy all prd resources
+    > `phi ws up prd:aws`    -> Deploy all prd aws resources
+    > `phi ws up prd::s3`    -> Deploy prd resources matching name s3
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import deploy_workspace
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -229,64 +193,78 @@
     if active_ws_data is None:
         print_active_workspace_not_available()
         avl_ws = phi_conf.available_ws
         if avl_ws:
             print_available_workspaces(avl_ws)
         return
 
+    current_path: Path = Path(".").resolve()
+    if active_ws_data.ws_root_path != current_path and not auto_confirm:
+        ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
+        if ws_at_current_path is not None:
+            print_info(
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+            )
+            update_active_workspace = typer.confirm(
+                f"Update active workspace to {ws_at_current_path.ws_name}", default=True
+            )
+            if update_active_workspace:
+                phi_conf.active_ws_name = ws_at_current_path.ws_name
+                active_ws_data = ws_at_current_path
+
     # Load environment from .env
     load_env(
         env={
             "PHI_WS_FORCE": str(force),
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
-    target_config: Optional[WorkspaceConfigType] = None
+    target_env: Optional[str] = None
     target_config_str: Optional[str] = None
+    target_config: Optional[WorkspaceConfigType] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_app: Optional[str] = None
-    target_env: Optional[str] = None
+    target_group: Optional[str] = None
 
-    # derive env/name/type/config from ws_filter
+    # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
-            target_app,
             target_name,
             target_type,
+            target_group,
         ) = parse_ws_filter(resource_filter)
 
-    # derive env/app/name/type/config from command options
+    # derive env:config:name:type:group from command options
+    if target_env is None and env_filter is not None and isinstance(env_filter, str):
+        target_env = env_filter
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
     if target_name is None and name_filter is not None and isinstance(name_filter, str):
         target_name = name_filter
     if target_type is None and type_filter is not None and isinstance(type_filter, str):
         target_type = type_filter
     if (
-        target_app is None
+        target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
-        target_app = group_filter
-    if target_env is None and env_filter is not None and isinstance(env_filter, str):
-        target_env = env_filter
+        target_group = group_filter
 
-    # derive env/config/name/type from defaults
+    # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
         )
     if target_config_str is None:
         target_config_str = (
             active_ws_data.ws_config.default_config
@@ -305,35 +283,35 @@
         )
 
     logger.debug("Deploying workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_app   : {target_app}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Deploying workspace: {}\n".format(active_ws_data.ws_name))
     deploy_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
         target_name=target_name,
         target_type=target_type,
-        target_app=target_app,
+        target_app=target_group,
         dry_run=dry_run,
         auto_confirm=auto_confirm,
     )
 
 
 @ws_app.command(short_help="Delete resources for active workspace")
 def down(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
+        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to shut down"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to shut down"
@@ -373,26 +351,26 @@
         False,
         "-f",
         "--force",
         help="Force",
     ),
 ):
     """\b
-    Delete resources for active workspace.
+    Delete resources for the active workspace.
     Options can be used to limit the resources to delete.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
+    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
     \b
     Examples:
-    $ `phi ws down`            -> Delete all resources
+    > `phi ws down`            -> Delete all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import shutdown_workspace
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -407,64 +385,78 @@
     if active_ws_data is None:
         print_active_workspace_not_available()
         avl_ws = phi_conf.available_ws
         if avl_ws:
             print_available_workspaces(avl_ws)
         return
 
+    current_path: Path = Path(".").resolve()
+    if active_ws_data.ws_root_path != current_path and not auto_confirm:
+        ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
+        if ws_at_current_path is not None:
+            print_info(
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+            )
+            update_active_workspace = typer.confirm(
+                f"Update active workspace to {ws_at_current_path.ws_name}", default=True
+            )
+            if update_active_workspace:
+                phi_conf.active_ws_name = ws_at_current_path.ws_name
+                active_ws_data = ws_at_current_path
+
     # Load environment from .env
     load_env(
         env={
             "PHI_WS_FORCE": str(force),
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
-    target_config: Optional[WorkspaceConfigType] = None
+    target_env: Optional[str] = None
     target_config_str: Optional[str] = None
+    target_config: Optional[WorkspaceConfigType] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_app: Optional[str] = None
-    target_env: Optional[str] = None
+    target_group: Optional[str] = None
 
-    # derive env/config/name/type from ws_filter
+    # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
-            target_app,
             target_name,
             target_type,
+            target_group,
         ) = parse_ws_filter(resource_filter)
 
-    # derive env/app/name/type/config from command options
+    # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
     if target_name is None and name_filter is not None and isinstance(name_filter, str):
         target_name = name_filter
     if target_type is None and type_filter is not None and isinstance(type_filter, str):
         target_type = type_filter
     if (
-        target_app is None
+        target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
-        target_app = group_filter
+        target_group = group_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
-    # derive env/config/name/type from defaults
+    # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
         )
     if target_config_str is None:
         target_config_str = (
             active_ws_data.ws_config.default_config
@@ -483,35 +475,35 @@
         )
 
     logger.debug("Shutting down workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_app   : {target_app}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Shutdown workspace: {}\n".format(active_ws_data.ws_name))
     shutdown_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
         target_name=target_name,
         target_type=target_type,
-        target_app=target_app,
+        target_app=target_group,
         dry_run=dry_run,
         auto_confirm=auto_confirm,
     )
 
 
 @ws_app.command(short_help="Update resources for active workspace")
 def patch(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
+        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to patch"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config to patch"
@@ -551,26 +543,26 @@
         False,
         "-f",
         "--force",
         help="Force",
     ),
 ):
     """\b
-    Update resources for active workspace.
+    Update resources for the active workspace.
     Options can be used to limit the resources to update.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
+    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
     Examples:
     \b
-    $ `phi ws patch`           -> Patch all resources
+    > `phi ws patch`           -> Patch all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import patch_workspace
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -585,64 +577,78 @@
     if active_ws_data is None:
         print_active_workspace_not_available()
         avl_ws = phi_conf.available_ws
         if avl_ws:
             print_available_workspaces(avl_ws)
         return
 
+    current_path: Path = Path(".").resolve()
+    if active_ws_data.ws_root_path != current_path and not auto_confirm:
+        ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
+        if ws_at_current_path is not None:
+            print_info(
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+            )
+            update_active_workspace = typer.confirm(
+                f"Update active workspace to {ws_at_current_path.ws_name}", default=True
+            )
+            if update_active_workspace:
+                phi_conf.active_ws_name = ws_at_current_path.ws_name
+                active_ws_data = ws_at_current_path
+
     # Load environment from .env
     load_env(
         env={
             "PHI_WS_FORCE": str(force),
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
-    target_config: Optional[WorkspaceConfigType] = None
+    target_env: Optional[str] = None
     target_config_str: Optional[str] = None
+    target_config: Optional[WorkspaceConfigType] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_app: Optional[str] = None
-    target_env: Optional[str] = None
+    target_group: Optional[str] = None
 
-    # derive env/name/type/config from ws_filter
+    # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
-            target_app,
             target_name,
             target_type,
+            target_group,
         ) = parse_ws_filter(resource_filter)
 
-    # derive env/app/name/type/config from command options
+    # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
     if target_name is None and name_filter is not None and isinstance(name_filter, str):
         target_name = name_filter
     if target_type is None and type_filter is not None and isinstance(type_filter, str):
         target_type = type_filter
     if (
-        target_app is None
+        target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
-        target_app = group_filter
+        target_group = group_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
-    # derive env/config/name/type from defaults
+    # derive env:config:name:type:group from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
         )
     if target_config_str is None:
         target_config_str = (
             active_ws_data.ws_config.default_config
@@ -661,35 +667,35 @@
         )
 
     logger.debug("Patching workspace")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_app   : {target_app}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Patching workspace: {}\n".format(active_ws_data.ws_name))
     patch_workspace(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
         target_name=target_name,
         target_type=target_type,
-        target_app=target_app,
+        target_app=target_group,
         dry_run=dry_run,
         auto_confirm=auto_confirm,
     )
 
 
 @ws_app.command(short_help="Restart resources for active workspace")
 def restart(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
+        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment to restart"
     ),
     config_filter: str = typer.Option(
         None, "-i", "--config", metavar="", help="Filter the config to restart"
@@ -733,15 +739,15 @@
     ),
 ):
     """\b
     Restarts the active workspace. i.e. runs `phi ws down` and then `phi ws up`.
 
     \b
     Examples:
-    $ `phi ws restart`
+    > `phi ws restart`
     """
     from time import sleep
 
     down(
         resource_filter=resource_filter,
         env_filter=env_filter,
         config_filter=config_filter,
@@ -765,19 +771,19 @@
         dry_run=dry_run,
         auto_confirm=auto_confirm,
         print_debug_log=print_debug_log,
         force=force,
     )
 
 
-@ws_app.command(short_help="Print workspace status")
+@ws_app.command(short_help="Show status for workspace resources")
 def status(
     resource_filter: Optional[str] = typer.Argument(
         None,
-        help="Resource filter. Format - ENV:CONFIG:GROUP:NAME:TYPE",
+        help="Resource filter. Format - ENV:CONFIG:NAME:TYPE:GROUP",
         metavar="[FILTER]",
     ),
     env_filter: str = typer.Option(
         None, "-e", "--env", metavar="", help="Filter the environment"
     ),
     config_filter: str = typer.Option(
         None, "-c", "--config", metavar="", help="Filter the config"
@@ -825,18 +831,18 @@
     Options can be used to limit the resources to update.
       --env     : Env (dev, stg, prd)
       --group   : Group name
       --name    : Resource name
       --type    : Resource type
       --config  : Config type (docker, aws, k8s)
     \b
-    Filters can also be provided as a single argument - ENV:CONFIG:GROUP:NAME:TYPE
+    Filters can also be provided as a single argument - ENV:CONFIG:NAME:TYPE:GROUP
     Examples:
     \b
-    $ `phi ws patch`           -> Patch all resources
+    > `phi ws patch`           -> Patch all resources
     """
     from phiterm.conf.phi_conf import PhiConf, PhiWsData
     from phiterm.workspace.ws_operator import print_workspace_status
     from phiterm.utils.load_env import load_env
     from phiterm.utils.ws_filter import parse_ws_filter
 
     if print_debug_log:
@@ -851,60 +857,74 @@
     if active_ws_data is None:
         print_active_workspace_not_available()
         avl_ws = phi_conf.available_ws
         if avl_ws:
             print_available_workspaces(avl_ws)
         return
 
+    current_path: Path = Path(".").resolve()
+    if active_ws_data.ws_root_path != current_path and not auto_confirm:
+        ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
+        if ws_at_current_path is not None:
+            print_info(
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+            )
+            update_active_workspace = typer.confirm(
+                f"Update active workspace to {ws_at_current_path.ws_name}", default=True
+            )
+            if update_active_workspace:
+                phi_conf.active_ws_name = ws_at_current_path.ws_name
+                active_ws_data = ws_at_current_path
+
     # Load environment from .env
     load_env(
         env={
             "PHI_WS_FORCE": str(force),
         },
         dotenv_dir=active_ws_data.ws_root_path,
     )
 
-    target_config: Optional[WorkspaceConfigType] = None
+    target_env: Optional[str] = None
     target_config_str: Optional[str] = None
+    target_config: Optional[WorkspaceConfigType] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
-    target_app: Optional[str] = None
-    target_env: Optional[str] = None
+    target_group: Optional[str] = None
 
-    # derive env/name/type/config from ws_filter
+    # derive env:config:name:type:group from ws_filter
     if resource_filter is not None:
         if not isinstance(resource_filter, str):
             raise TypeError(
                 f"Invalid resource_filter. Expected: str, Received: {type(resource_filter)}"
             )
         (
             target_env,
             target_config_str,
-            target_app,
             target_name,
             target_type,
+            target_group,
         ) = parse_ws_filter(resource_filter)
 
-    # derive env/app/name/type/config from command options
+    # derive env:config:name:type:group from command options
     if (
         target_config_str is None
         and config_filter is not None
         and isinstance(config_filter, str)
     ):
         target_config_str = config_filter
     if target_name is None and name_filter is not None and isinstance(name_filter, str):
         target_name = name_filter
     if target_type is None and type_filter is not None and isinstance(type_filter, str):
         target_type = type_filter
     if (
-        target_app is None
+        target_group is None
         and group_filter is not None
         and isinstance(group_filter, str)
     ):
-        target_app = group_filter
+        target_group = group_filter
     if target_env is None and env_filter is not None and isinstance(env_filter, str):
         target_env = env_filter
 
     # derive env/config/name/type from defaults
     if target_env is None:
         target_env = (
             active_ws_data.ws_config.default_env if active_ws_data.ws_config else None
@@ -927,25 +947,25 @@
         )
 
     logger.debug("Reading workspace status")
     logger.debug(f"\ttarget_env   : {target_env}")
     logger.debug(f"\ttarget_config: {target_config}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
-    logger.debug(f"\ttarget_app   : {target_app}")
+    logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     print_heading("Reading workspace status: {}\n".format(active_ws_data.ws_name))
     print_workspace_status(
         ws_data=active_ws_data,
         target_env=target_env,
         target_config=target_config,
         target_name=target_name,
         target_type=target_type,
-        target_app=target_app,
+        target_app=target_group,
         dry_run=dry_run,
         auto_confirm=auto_confirm,
     )
 
 
 @ws_app.command(short_help="Prints active workspace config", hidden=True)
 def config(
```

### Comparing `phiterm-1.6.4/phiterm/conf/auth.py` & `phiterm-1.6.5/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/conf/constants.py` & `phiterm-1.6.5/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/conf/phi_conf.py` & `phiterm-1.6.5/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/databox/databox_operator.py` & `phiterm-1.6.5/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/docker/docker_operator.py` & `phiterm-1.6.5/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/enums/user.py` & `phiterm-1.6.5/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.5/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.5/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.5/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.5/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.5/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/local/local_operator.py` & `phiterm-1.6.5/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/release/release_schemas.py` & `phiterm-1.6.5/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/release/ws_releases.py` & `phiterm-1.6.5/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/schemas/user.py` & `phiterm-1.6.5/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/schemas/user_schemas.py` & `phiterm-1.6.5/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/schemas/workspace.py` & `phiterm-1.6.5/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.5/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.5/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.5/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.5/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.5/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.5/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.5/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.5/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/cli_console.py` & `phiterm-1.6.5/phiterm/utils/cli_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,20 @@
 
 
 def log_auth_error_msg() -> None:
     logger.debug("AuthError: could not authenticate, please run `phi auth` again")
 
 
 def print_active_workspace_not_available() -> None:
-    print_warning("No active workspace")
-    print_warning("Run `phi ws create` to create a new workspace")
+    print_warning("No active workspace. You can:")
+    print_warning("- Run `phi ws create` to create a new workspace")
     print_warning(
-        "Run `phi ws setup` from an existing workspace directory to setup the workspace"
+        "- Run `phi ws setup` from an existing directory to setup the workspace"
     )
-    print_warning("Or set an existing workspace as active using `phi set [ws_name]`")
+    print_warning("- Set an existing workspace as active using `phi set [ws_name]`")
 
 
 def print_available_workspaces(avl_ws_list) -> None:
     avl_ws_names = [w.name for w in avl_ws_list] if avl_ws_list else []
     print_info("Available Workspaces:\n  - {}".format("\n  - ".join(avl_ws_names)))
```

### Comparing `phiterm-1.6.4/phiterm/utils/common.py` & `phiterm-1.6.5/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/dttm.py` & `phiterm-1.6.5/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/enums.py` & `phiterm-1.6.5/phiterm/utils/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 class ExtendedEnum(enum.Enum):
     @classmethod
     def values_list(cls: Any) -> List[Any]:
         return list(map(lambda c: c.value, cls))
 
     @classmethod
-    def from_str(
-        cls: Any, str_to_convert_to_enum: Optional[str]
-    ) -> Optional["ExtendedEnum"]:
+    def from_str(cls: Any, str_to_convert_to_enum: Optional[str]) -> Optional[Any]:
         """Convert a string value to an enum object. Case Sensitive"""
 
         if str_to_convert_to_enum is None:
             return None
 
         if str_to_convert_to_enum in cls._value2member_map_:
             return cls._value2member_map_.get(str_to_convert_to_enum)
```

### Comparing `phiterm-1.6.4/phiterm/utils/filesystem.py` & `phiterm-1.6.5/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/git.py` & `phiterm-1.6.5/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/load_env.py` & `phiterm-1.6.5/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/log.py` & `phiterm-1.6.5/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/pyproject.py` & `phiterm-1.6.5/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/utils/ws_filter.py` & `phiterm-1.6.5/phiterm/utils/ws_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 
 def parse_ws_filter(
     ws_filter: str,
 ) -> Tuple[Optional[str], Optional[str], Optional[str], Optional[str], Optional[str]]:
     target_env: Optional[str] = None
     target_config: Optional[str] = None
-    target_app: Optional[str] = None
     target_name: Optional[str] = None
     target_type: Optional[str] = None
+    target_group: Optional[str] = None
 
     filters = ws_filter.split(":")
     num_filters = len(filters)
     if num_filters >= 1:
         if filters[0] != "":
             target_env = filters[0]
     if num_filters >= 2:
         if filters[1] != "":
             target_config = filters[1]
     if num_filters >= 3:
         if filters[2] != "":
-            target_app = filters[2]
+            target_name = filters[2]
     if num_filters >= 4:
         if filters[3] != "":
-            target_name = filters[3]
+            target_type = filters[3]
     if num_filters >= 5:
         if filters[4] != "":
-            target_type = filters[4]
+            target_group = filters[4]
 
-    return target_env, target_config, target_app, target_name, target_type
+    return target_env, target_config, target_name, target_type, target_group
```

### Comparing `phiterm-1.6.4/phiterm/workflow/wf_operator.py` & `phiterm-1.6.5/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/workflow/wf_utils.py` & `phiterm-1.6.5/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.5/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/workspace/ws_enums.py` & `phiterm-1.6.5/phiterm/workspace/ws_enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     PUBLIC = "PUBLIC"
 
 
 class WorkspaceStarterTemplate(ExtendedEnum):
     ai_app = "ai-app"
     ml_app = "ml-app"
     api_app = "api-app"
+    django_app = "django-app"
     streamlit_app = "streamlit-app"
     aws_dp = "data-platform"
     aws_spark_dp = "spark-data-platform"
     aws_snowflake_dp = "snowflake-data-platform"
 
 
 class WorkspaceEnv(ExtendedEnum):
```

### Comparing `phiterm-1.6.4/phiterm/workspace/ws_loader.py` & `phiterm-1.6.5/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/workspace/ws_operator.py` & `phiterm-1.6.5/phiterm/workspace/ws_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,75 +19,124 @@
 from phiterm.utils.log import logger
 from phiterm.workspace.ws_enums import (
     WorkspaceConfigType,
     WorkspaceStarterTemplate,
 )
 from phiterm.workspace.exceptions import WorkspaceException
 
-# List of reserved workspace names
-RESERVED_WS_NAMES = ["root", "bedi", "ashpreet", "ashpreetbedi"]
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.ai_app: "ai-app",
     WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.api_app: "api-app",
+    WorkspaceStarterTemplate.django_app: "django-app",
     WorkspaceStarterTemplate.streamlit_app: "streamlit-app",
     WorkspaceStarterTemplate.aws_dp: "data-platform",
     WorkspaceStarterTemplate.aws_spark_dp: "spark-data-platform",
     WorkspaceStarterTemplate.aws_snowflake_dp: "snowflake-data-platform",
 }
 TEMPLATE_TO_REPO_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.ai_app: "https://github.com/phidatahq/ai-app.git",
     WorkspaceStarterTemplate.ml_app: "https://github.com/phidatahq/ml-app.git",
     WorkspaceStarterTemplate.api_app: "https://github.com/phidatahq/api-app.git",
+    WorkspaceStarterTemplate.django_app: "https://github.com/phidatahq/django-app.git",
     WorkspaceStarterTemplate.streamlit_app: "https://github.com/phidatahq/streamlit-app.git",
     WorkspaceStarterTemplate.aws_dp: "https://github.com/phidatahq/aws-dp-template.git",
     WorkspaceStarterTemplate.aws_spark_dp: "https://github.com/phidatahq/aws-spark-dp-template.git",
     WorkspaceStarterTemplate.aws_snowflake_dp: "https://github.com/phidatahq/aws-snowflake-dp-template.git",
 }
 
 
-def create_new_workspace(ws_name: str, template: WorkspaceStarterTemplate) -> bool:
+def create_workspace(
+    template: Optional[str] = None, name: Optional[str] = None
+) -> bool:
     """Creates a new workspace for the user.
     This function clones a phidata template on the users machine at the path:
         cwd/ws_name
     cwd: current working dir - where the command was run from.
-
-    Steps:
-    1. Validate ws_name and if we can create a folder with that name
-    2. Clone the starter template in cwd/ws_name
-    3. Delete the .git folder
-    4. Provide the user with steps to add a remote origin for this workspace
-
-    NOTE: till the user runs `phi ws setup` the workspace is not registered with phidata
-        and can only be used locally
     """
     from shutil import copytree
+    from rich.prompt import Prompt
+
+    from phiterm.cli.cli_operator import initialize_phidata
+    from phiterm.utils.common import is_empty, str_to_int
     from phiterm.utils.filesystem import rmdir_recursive
     from phiterm.workspace.ws_utils import get_ws_config_dir_path
     from phiterm.utils.git import GitCloneProgress
 
     current_dir: Path = Path(".").resolve()
 
     # Phidata should be initialized before creating a workspace
     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
     if not phi_conf:
-        print_conf_not_available_msg()
-        return False
+        initialize_phidata()
+        phi_conf = PhiConf.get_saved_conf()
+        # If phi_conf is still None, throw an error
+        if not phi_conf:
+            raise Exception("Failed to initialize phidata")
+
+    # Parse template and ws_name
+    ws_template: WorkspaceStarterTemplate
+    ws_name: str
+
+    # Get starter template from the user if not provided
+    if template is None:
+        # Display available starter templates and ask user to select one
+        print_info("Select workspace template or press Enter for default (ai-app)")
+        templates = WorkspaceStarterTemplate.values_list()
+        for template_id, template_name in enumerate(templates, start=1):
+            print_info("  [{}] {}".format(template_id, template_name))
+
+        # Get starter template from the user
+        template_choices = [str(idx) for idx, _ in enumerate(templates, start=1)]
+        template_inp_raw = Prompt.ask(
+            "Template Number", choices=template_choices, default="1", show_choices=False
+        )
+        # Convert input to int value.
+        template_inp = str_to_int(template_inp_raw)
 
-    # Error if the workspace name provided is a reserved name
-    if ws_name in RESERVED_WS_NAMES:
-        logger.error(f"The name `{ws_name}` is reserved")
-        return False
+        ws_template = WorkspaceStarterTemplate.ai_app
+        if template_inp is not None:
+            try:
+                ws_template = cast(
+                    WorkspaceStarterTemplate,
+                    WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
+                )
+            except Exception as e:
+                logger.exception(e)
+                logger.error("Invalid template number, please try again")
+                return False
+        logger.debug("Selected: {}".format(ws_template.value))
+    elif template.lower() in WorkspaceStarterTemplate.values_list():
+        _ws_template = WorkspaceStarterTemplate.from_str(template)
+        if _ws_template is not None and isinstance(
+            _ws_template, WorkspaceStarterTemplate
+        ):
+            ws_template = _ws_template
+        else:
+            raise Exception(f"Failed to parse template: {template}")
+    else:
+        raise Exception(
+            f"{template} is not a supported template, please choose from: {WorkspaceStarterTemplate.values_list()}"
+        )
+
+    # Get workspace name from user if not provided
+    if name is None:
+        ws_name = Prompt.ask(
+            "Workspace Name",
+            default=TEMPLATE_TO_NAME_MAP.get(ws_template, DEFAULT_WS_NAME),
+        )
+    else:
+        ws_name = name
 
     # Check if a workspace with the same name exists
     _existing_ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_name(ws_name)
     if _existing_ws_data is not None:
         logger.error(f"Found existing record for a workspace: {ws_name}")
         delete_existing_ws_data = typer.confirm(
-            "Replace the existing record?", default=True
+            "Replace existing record?", default=True
         )
         if delete_existing_ws_data:
             phi_conf.delete_ws(ws_name)
         else:
             return False
 
     # Check if we can create the workspace in the current dir
@@ -95,16 +144,16 @@
     if ws_root_path.exists():
         logger.error(
             f"Directory {ws_root_path} exists, please delete files manually or choose another name for workspace"
         )
         return False
 
     print_info(f"Creating {str(ws_root_path)}")
-    # Clone the starter repo for this cloud in the new directory
-    repo_to_clone = TEMPLATE_TO_REPO_MAP.get(template)
+    # Clone the starter repo
+    repo_to_clone = TEMPLATE_TO_REPO_MAP.get(ws_template)
     logger.debug("Cloning: {}".format(repo_to_clone))
     try:
         _cloned_git_repo: git.Repo = git.Repo.clone_from(
             repo_to_clone, str(ws_root_path), progress=GitCloneProgress()  # type: ignore
         )
     except Exception as e:
         logger.error(e)
@@ -124,14 +173,15 @@
 
     phi_conf.add_new_ws_to_config(
         ws_name=ws_name,
         ws_root_path=ws_root_path,
     )
 
     try:
+        # ws_config_dir_path is the path to the ws_root/workspace dir
         ws_config_dir_path: Path = get_ws_config_dir_path(ws_root_path)
         ws_config_secrets_dir = ws_config_dir_path.joinpath("secrets").resolve()
         ws_config_example_secrets_dir = ws_config_dir_path.joinpath(
             "example_secrets"
         ).resolve()
 
         print_info(f"Creating {str(ws_config_secrets_dir)}")
@@ -145,101 +195,32 @@
             "Please manually copy workspace/example_secrets to workspace/secrets"
         )
 
     print_info(f"Your new workspace is available at {str(ws_root_path)}\n")
     return setup_workspace(ws_root_path=ws_root_path)
 
 
-def create_workspace_using_input():
-    """Takes input from the user and calls create_new_workspace()"""
-
-    from phiterm.utils.common import is_empty, str_to_int
-
-    # Display available starter templates and ask user to select one
-    print_info("Input Template Number (default: ai-app)")
-    templates = WorkspaceStarterTemplate.values_list()
-    for idx, prvdr in enumerate(templates, start=1):
-        print_info("  [{}] {}".format(idx, prvdr))
-
-    # Get starter template from the user
-    template_inp_raw = input(": ")
-    # Convert input to int value.
-    template_inp = str_to_int(template_inp_raw)
-    template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.api_app
-
-    if template_inp is not None:
-        try:
-            template = cast(
-                WorkspaceStarterTemplate,
-                WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
-            )
-        except Exception as e:
-            logger.error(e)
-    logger.debug("Selected: {}".format(template.value))
-
-    # Get workspace name from user
-    default_ws_name = TEMPLATE_TO_NAME_MAP.get(template, DEFAULT_WS_NAME)
-    ws_name_inp_raw = input(f"Workspace name (default: {default_ws_name}): ")
-    if is_empty(ws_name_inp_raw):
-        ws_name_inp_raw = default_ws_name
-
-    print_info(
-        f"Creating workspace {ws_name_inp_raw} using the {template.value} template\n"
-    )
-    create_new_workspace(ws_name_inp_raw, template)
-
-
-def initialize_workspace() -> None:
-    """Initialize a phidata workspace.
-
-    This function is called by `phi ws create` to create a new workspace.
-    """
-    phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
-    if not phi_conf:
-        print_conf_not_available_msg()
-        return
-
-    print_heading("New phidata workspace")
-    create_workspace_using_input()
-
-
 def setup_workspace(ws_root_path: Path) -> bool:
     """Setup a phidata workspace at directory: `ws_root_path`.
     This is the catchall function for a workspace. Run it in a directory and it
     should figure everything out.
 
     1. Validate pre-requisites
     1.1 Check ws_root_path is valid
     1.2 Check PhiConf is valid
     1.3 Validate PhiWsData is available
-        Get the ws_data using the ws_root_path
-        If ws_data is None, read the ws_config_file_path to map it to an available workspace
-            This may happen if the user ran `phi init -r`
-        If the user cloned this directory directly, there will be no record of this workspace in the PhiConf
-        In that case, we manually add the ws to PhiConf and process the ws_config_file_path and setup this workspace.
-    1.4 Check if this is the active workspace or if it needs to be set as active
+    1.4 Set workspace as active
     1.5 Check if remote origin is available
 
-    2. Create or Update WorkspaceSchema
-    If a ws_schema exists for this workspace, this workspace has been setup before
+    2. Create or Update WorkspaceSchema (if user is logged in)
+    If a ws_schema exists for this workspace, this workspace has a record in the backend
     2.1 Create WorkspaceSchema for a NEWLY CREATED WORKSPACE
-        If ws_schema is None, this is a NEWLY CREATED WORKSPACE.
-        i.e. A new workspace was created using create_new_workspace() <- which is called using `phi ws create`.
-        This ws does not have a ws_schema, make an api call to create one.
-        If the api call returns None, then we could not create the workspace.
-    2.2 Update WorkspaceSchema if ws_schema exists
-    2.3 Set as active if needed
-    2.4 Refresh PhiWsData
-
-    3. Complete Workspace setup
-    3.1 Validate ws_config_file_path
-    3.2 Validate PhiWsData
-        Reaching here implies a all ws_data is available and updated.
-        Validate the ws_data and print any pending setup actions.
+    2.2 Update WorkspaceSchema for EXISTING WORKSPACE
 
+    3. Refresh PhiWsData and Complete Workspace setup
     `phi ws setup` is a generic catch-all function. It should handle errors graciously
     and provide "how to fix" messages and "next steps" to get the user running.
     """
     from phiterm.utils.git import get_remote_origin_for_dir
     from phiterm.workspace.ws_utils import print_howtofix_pending_actions
 
     print_heading("Running workspace setup\n")
@@ -268,125 +249,115 @@
     ######################################################
     # 1.3 Validate PhiWsData is available
     ######################################################
     logger.debug(f"Checking for a workspace at {ws_root_path}")
     ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_path(ws_root_path)
     if ws_data is None:
         # This happens if
-        # - The user is setting up an existing workspace
-        # - the user ran `phi init -r` which erases the self._path_to_ws_data_map
+        # - The user is setting up a workspace not previously setup on this machine
+        # - the user ran `phi init -r` which erases existing records of workspaces
         logger.debug(f"Could not find an existing workspace at path: {ws_root_path}")
 
         # In this case, the local workspace directory exists but PhiConf does not have a record
         print_info(f"Adding {ws_root_path} as a workspace")
         phi_conf.add_new_ws_to_config(
             ws_name=ws_root_path.stem,
             ws_root_path=ws_root_path,
         )
         ws_data = phi_conf.get_ws_data_by_path(ws_root_path)
-        # If the ws_data is still none it means the workspace has bad data in it
-        if ws_data is None:
-            logger.error(f"Could not add workspace from: {ws_root_path}")
-            logger.error("Please try again")
-            return False
     else:
         logger.debug(f"Found workspace {ws_data.ws_name}")
         phi_conf.refresh_ws_config(ws_data.ws_name)
 
+    # If the ws_data is still None it means the workspace is corrupt
+    if ws_data is None:
+        logger.error(f"Could not add workspace from: {ws_root_path}")
+        logger.error("Please try again")
+        return False
+
     ######################################################
     # 1.4 Set workspace as active
     ######################################################
-    is_active_ws = True
     phi_conf.active_ws_name = ws_data.ws_name
+    is_active_ws = True
 
     ######################################################
     # 1.5 Check if remote origin is available
     ######################################################
     _remote_origin_url: Optional[str] = get_remote_origin_for_dir(ws_root_path)
     logger.debug("Git origin: {}".format(_remote_origin_url))
 
     ######################################################
-    ## 2. Create or Update WorkspaceSchema
+    ## 2. Create or Update WorkspaceSchema (if user is logged in)
     ######################################################
-    # If a ws_schema exists for this workspace, this workspace has a record in the backend
-    ws_schema: Optional[WorkspaceSchema] = ws_data.ws_schema
+    if phi_conf.user is not None:
+        # If a ws_schema exists for this workspace, this workspace has a record in the backend
+        ws_schema: Optional[WorkspaceSchema] = ws_data.ws_schema
 
-    ######################################################
-    # 2.1 Create WorkspaceSchema for a NEWLY CREATED WORKSPACE
-    ######################################################
-    if ws_schema is None:
-        from phiterm.api.workspace import create_workspace
+        ######################################################
+        # 2.1 Create WorkspaceSchema for NEW WORKSPACE
+        ######################################################
+        if ws_schema is None:
+            from phiterm.api.workspace import create_workspace
 
-        # If ws_schema is None, this is a NEWLY CREATED WORKSPACE.
-        # We make a call to the backend to create a new ws_schema
-        logger.debug("ws_schema not found, trying to create one... ")
-        logger.debug("ws_name: {}".format(ws_data.ws_name))
-        logger.debug("is_active_ws: {}".format(is_active_ws))
+            # If ws_schema is None, this is a NEWLY CREATED WORKSPACE.
+            # We make a call to the backend to create a new ws_schema
+            logger.debug("Creating ws_schema for new workspace")
+            logger.debug("ws_name: {}".format(ws_data.ws_name))
+            logger.debug("is_active_ws: {}".format(is_active_ws))
 
-        if phi_conf.user is not None:
             ws_schema = create_workspace(
                 user=phi_conf.user,
                 workspace=WorkspaceSchema(
                     ws_name=ws_data.ws_name,
                     is_primary_ws_for_user=is_active_ws,
                 ),
             )
-        if ws_schema is not None:
-            phi_conf.update_ws_data(ws_name=ws_data.ws_name, ws_schema=ws_schema)
-    else:
-        from phiterm.api.workspace import update_workspace
+            if ws_schema is not None:
+                phi_conf.update_ws_data(ws_name=ws_data.ws_name, ws_schema=ws_schema)
+        ######################################################
+        # 2.2 Update WorkspaceSchema for EXISTING WORKSPACE
+        ######################################################
+        else:
+            from phiterm.api.workspace import update_workspace
 
-        # 2.2 Update WorkspaceSchema
-        logger.debug("ws_schema found, updating... ")
-        logger.debug("ws_name: {}".format(ws_data.ws_name))
-        logger.debug("is_active_ws: {}".format(is_active_ws))
+            logger.debug("Updating ws_schema for existing workspace")
+            logger.debug("ws_name: {}".format(ws_data.ws_name))
+            logger.debug("is_active_ws: {}".format(is_active_ws))
 
-        if phi_conf.user is not None:
             ws_schema.is_primary_ws_for_user = is_active_ws
             ws_schema_updated = update_workspace(
                 user=phi_conf.user,
                 workspace=ws_schema,
             )
             if ws_schema_updated is not None:
                 # Update the ws_schema for this workspace.
                 phi_conf.update_ws_data(
                     ws_name=ws_data.ws_name, ws_schema=ws_schema_updated
                 )
 
     ######################################################
-    # 2.3 Refresh PhiWsData
+    # 3. Refresh PhiWsData and Complete Workspace setup
     ######################################################
-    # Refresh ws_data because phi_conf.update_ws_data()
-    # will create a new ws_data object in PhiConf
-    # Also, cast it to PhiWsData because ws_data is no longer Optional[PhiWsData]
+    # Refresh ws_data because phi_conf.update_ws_data() will create a new ws_data object in PhiConf
     ws_data = cast(PhiWsData, phi_conf.get_ws_data_by_name(ws_data.ws_name))
 
-    ######################################################
-    ## 3. Complete Workspace setup
-    ######################################################
-
-    ######################################################
-    # 3.1 Validate PhiWsData
-    ######################################################
+    # Check if workspace is valid and complete setup
     ws_is_valid, pending_actions = phi_conf.validate_workspace(ws_name=ws_data.ws_name)
-
     if ws_is_valid and ws_data.ws_config is not None:
         scripts_dir = ws_data.ws_config.scripts_dir
         install_deps_file = f"sh {ws_root_path}/{scripts_dir}/install.sh"
-        print_subheading(f"Setup complete! Next steps:\n")
+        print_subheading(f"Setup complete! Next steps:")
         print_info("1. Deploy workspace:")
         print_info("\tphi ws up")
         print_info("2. Install workspace dependencies:")
         print_info(f"\t{install_deps_file}")
-        # if pending_actions and len(pending_actions) > 0:
-        #     print_info("3. Complete pending actions:")
-        #     print_howtofix_pending_actions(pending_actions)
         return True
     else:
-        print_info(f"Workspace setup pending.")
+        print_info(f"Workspace setup pending")
         print_howtofix_pending_actions(pending_actions)
         return False
 
     ######################################################
     ## End Workspace setup
     ######################################################
 
@@ -896,17 +867,168 @@
             # )
             num_configs_patched += 1
         # white space between runs
         print_info("")
 
 
 ######################################################
-## Deprecated functions
+## TODO: Delete deprecated functions
 ######################################################
 #
+# def create_new_workspace(ws_name: str, template: WorkspaceStarterTemplate) -> bool:
+#     """Creates a new workspace for the user.
+#     This function clones a phidata template on the users machine at the path:
+#         cwd/ws_name
+#     cwd: current working dir - where the command was run from.
+#
+#     Steps:
+#     1. Validate ws_name and if we can create a folder with that name
+#     2. Clone the starter template in cwd/ws_name
+#     3. Delete the .git folder
+#     4. Provide the user with steps to add a remote origin for this workspace
+#
+#     NOTE: till the user runs `phi ws setup` the workspace is not registered with phidata
+#         and can only be used locally
+#     """
+#     from shutil import copytree
+#     from phiterm.utils.filesystem import rmdir_recursive
+#     from phiterm.workspace.ws_utils import get_ws_config_dir_path
+#     from phiterm.utils.git import GitCloneProgress
+#
+#     current_dir: Path = Path(".").resolve()
+#
+#     # Phidata should be initialized before creating a workspace
+#     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
+#     if not phi_conf:
+#         print_conf_not_available_msg()
+#         return False
+#
+#     # Check if a workspace with the same name exists
+#     _existing_ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_name(ws_name)
+#     if _existing_ws_data is not None:
+#         logger.error(f"Found existing record for a workspace: {ws_name}")
+#         delete_existing_ws_data = typer.confirm(
+#             "Replace the existing record?", default=True
+#         )
+#         if delete_existing_ws_data:
+#             phi_conf.delete_ws(ws_name)
+#         else:
+#             return False
+#
+#     # Check if we can create the workspace in the current dir
+#     ws_root_path: Path = current_dir.joinpath(ws_name)
+#     if ws_root_path.exists():
+#         logger.error(
+#             f"Directory {ws_root_path} exists, please delete files manually or choose another name for workspace"
+#         )
+#         return False
+#
+#     print_info(f"Creating {str(ws_root_path)}")
+#     # Clone the starter repo for this cloud in the new directory
+#     repo_to_clone = TEMPLATE_TO_REPO_MAP.get(template)
+#     logger.debug("Cloning: {}".format(repo_to_clone))
+#     try:
+#         _cloned_git_repo: git.Repo = git.Repo.clone_from(
+#             repo_to_clone, str(ws_root_path), progress=GitCloneProgress()  # type: ignore
+#         )
+#     except Exception as e:
+#         logger.error(e)
+#         return False
+#
+#     # Remove existing .git folder
+#     _dot_git_folder = ws_root_path.joinpath(".git")
+#     _dot_git_exists = _dot_git_folder.exists()
+#     if _dot_git_exists:
+#         logger.debug(f"Deleting {_dot_git_folder}")
+#         try:
+#             _dot_git_exists = not rmdir_recursive(_dot_git_folder)
+#         except Exception as e:
+#             logger.warning(f"Failed to delete {_dot_git_folder}: {e}")
+#             logger.info("Please delete the .git folder manually")
+#             pass
+#
+#     phi_conf.add_new_ws_to_config(
+#         ws_name=ws_name,
+#         ws_root_path=ws_root_path,
+#     )
+#
+#     try:
+#         ws_config_dir_path: Path = get_ws_config_dir_path(ws_root_path)
+#         ws_config_secrets_dir = ws_config_dir_path.joinpath("secrets").resolve()
+#         ws_config_example_secrets_dir = ws_config_dir_path.joinpath(
+#             "example_secrets"
+#         ).resolve()
+#
+#         print_info(f"Creating {str(ws_config_secrets_dir)}")
+#         copytree(
+#             str(ws_config_example_secrets_dir),
+#             str(ws_config_secrets_dir),
+#         )
+#     except Exception as e:
+#         logger.warning(f"Could not create workspace/secrets: {e}")
+#         logger.warning(
+#             "Please manually copy workspace/example_secrets to workspace/secrets"
+#         )
+#
+#     print_info(f"Your new workspace is available at {str(ws_root_path)}\n")
+#     return setup_workspace(ws_root_path=ws_root_path)
+#
+#
+# def create_workspace_using_input():
+#     """Takes input from the user and calls create_new_workspace()"""
+#
+#     from phiterm.utils.common import is_empty, str_to_int
+#
+#     # Display available starter templates and ask user to select one
+#     print_info("Input Template Number (default: ai-app)")
+#     templates = WorkspaceStarterTemplate.values_list()
+#     for idx, prvdr in enumerate(templates, start=1):
+#         print_info("  [{}] {}".format(idx, prvdr))
+#
+#     # Get starter template from the user
+#     template_inp_raw = input(": ")
+#     # Convert input to int value.
+#     template_inp = str_to_int(template_inp_raw)
+#     template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.api_app
+#
+#     if template_inp is not None:
+#         try:
+#             template = cast(
+#                 WorkspaceStarterTemplate,
+#                 WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
+#             )
+#         except Exception as e:
+#             logger.error(e)
+#     logger.debug("Selected: {}".format(template.value))
+#
+#     # Get workspace name from user
+#     default_ws_name = TEMPLATE_TO_NAME_MAP.get(template, DEFAULT_WS_NAME)
+#     ws_name_inp_raw = input(f"Workspace name (default: {default_ws_name}): ")
+#     if is_empty(ws_name_inp_raw):
+#         ws_name_inp_raw = default_ws_name
+#
+#     print_info(
+#         f"Creating workspace {ws_name_inp_raw} using the {template.value} template\n"
+#     )
+#     create_new_workspace(ws_name_inp_raw, template)
+#
+#
+# def initialize_workspace() -> None:
+#     """Initialize a phidata workspace.
+#
+#     This function is called by `phi ws create` to create a new workspace.
+#     """
+#     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
+#     if not phi_conf:
+#         print_conf_not_available_msg()
+#         return
+#
+#     print_heading("New phidata workspace")
+#     create_workspace_using_input()
+#
 # def print_git_setup(
 #     ws_name: str,
 #     ws_root_path: Path,
 #     version_control_provider: Optional[
 #         VersionControlProviderEnum
 #     ] = VersionControlProviderEnum.GITHUB,
 # ) -> None:
```

### Comparing `phiterm-1.6.4/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.5/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm/workspace/ws_utils.py` & `phiterm-1.6.5/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.5/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.4/pyproject.toml` & `phiterm-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.4"
+version = "1.6.5"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

