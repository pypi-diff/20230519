# Comparing `tmp/phiterm-1.6.5.tar.gz` & `tmp/phiterm-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.5.tar", last modified: Fri May 19 09:06:06 2023, max compression
+gzip compressed data, was "phiterm-1.6.6.tar", last modified: Fri May 19 11:12:40 2023, max compression
```

## Comparing `phiterm-1.6.5.tar` & `phiterm-1.6.6.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-19 09:05:46.000000 phiterm-1.6.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 09:06:06.966987 phiterm-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 09:05:46.000000 phiterm-1.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.950986 phiterm-1.6.5/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.958986 phiterm-1.6.5/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.950986 phiterm-1.6.5/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.962986 phiterm-1.6.5/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45239 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 09:05:46.000000 phiterm-1.6.5/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.954986 phiterm-1.6.5/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 09:06:06.000000 phiterm-1.6.5/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-19 09:05:46.000000 phiterm-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:06:06.966987 phiterm-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 09:05:46.000000 phiterm-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:06:06.966987 phiterm-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 09:05:46.000000 phiterm-1.6.5/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.250003 phiterm-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-19 11:12:14.000000 phiterm-1.6.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 11:12:40.250003 phiterm-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 11:12:14.000000 phiterm-1.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.230002 phiterm-1.6.6/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.230002 phiterm-1.6.6/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.230002 phiterm-1.6.6/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.234003 phiterm-1.6.6/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.238003 phiterm-1.6.6/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.242003 phiterm-1.6.6/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.226003 phiterm-1.6.6/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.242003 phiterm-1.6.6/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.242003 phiterm-1.6.6/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.246003 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.246003 phiterm-1.6.6/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.246003 phiterm-1.6.6/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.246003 phiterm-1.6.6/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.250003 phiterm-1.6.6/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.250003 phiterm-1.6.6/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 11:12:14.000000 phiterm-1.6.6/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.230002 phiterm-1.6.6/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 11:12:40.000000 phiterm-1.6.6/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-19 11:12:14.000000 phiterm-1.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:12:40.250003 phiterm-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 11:12:14.000000 phiterm-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:12:40.250003 phiterm-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 11:12:14.000000 phiterm-1.6.6/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.5/LICENSE.md` & `phiterm-1.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/api/client.py` & `phiterm-1.6.6/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/api/routes.py` & `phiterm-1.6.6/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/api/user.py` & `phiterm-1.6.6/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/api/workspace.py` & `phiterm-1.6.6/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/aws/aws_operator.py` & `phiterm-1.6.6/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/cli_app.py` & `phiterm-1.6.6/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/cli_operator.py` & `phiterm-1.6.6/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.6/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.6/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.6/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.6/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.6/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.6/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/conf/auth.py` & `phiterm-1.6.6/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/conf/constants.py` & `phiterm-1.6.6/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/conf/phi_conf.py` & `phiterm-1.6.6/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/databox/databox_operator.py` & `phiterm-1.6.6/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/docker/docker_operator.py` & `phiterm-1.6.6/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/enums/user.py` & `phiterm-1.6.6/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.6/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.6/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.6/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.6/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.6/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/local/local_operator.py` & `phiterm-1.6.6/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/release/release_schemas.py` & `phiterm-1.6.6/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/release/ws_releases.py` & `phiterm-1.6.6/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/schemas/user.py` & `phiterm-1.6.6/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/schemas/user_schemas.py` & `phiterm-1.6.6/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/schemas/workspace.py` & `phiterm-1.6.6/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.6/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.6/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.6/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.6/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.6/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.6/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.6/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.6/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.6/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/cli_console.py` & `phiterm-1.6.6/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/common.py` & `phiterm-1.6.6/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/dttm.py` & `phiterm-1.6.6/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/enums.py` & `phiterm-1.6.6/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/filesystem.py` & `phiterm-1.6.6/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/git.py` & `phiterm-1.6.6/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/load_env.py` & `phiterm-1.6.6/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/log.py` & `phiterm-1.6.6/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/pyproject.py` & `phiterm-1.6.6/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/utils/ws_filter.py` & `phiterm-1.6.6/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workflow/wf_operator.py` & `phiterm-1.6.6/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workflow/wf_utils.py` & `phiterm-1.6.6/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.6/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workspace/ws_enums.py` & `phiterm-1.6.6/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workspace/ws_loader.py` & `phiterm-1.6.6/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workspace/ws_operator.py` & `phiterm-1.6.6/phiterm/workspace/ws_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         cwd/ws_name
     cwd: current working dir - where the command was run from.
     """
     from shutil import copytree
     from rich.prompt import Prompt
 
     from phiterm.cli.cli_operator import initialize_phidata
-    from phiterm.utils.common import is_empty, str_to_int
+    from phiterm.utils.common import str_to_int
     from phiterm.utils.filesystem import rmdir_recursive
     from phiterm.workspace.ws_utils import get_ws_config_dir_path
     from phiterm.utils.git import GitCloneProgress
 
     current_dir: Path = Path(".").resolve()
 
     # Phidata should be initialized before creating a workspace
@@ -216,14 +216,15 @@
     2.1 Create WorkspaceSchema for a NEWLY CREATED WORKSPACE
     2.2 Update WorkspaceSchema for EXISTING WORKSPACE
 
     3. Refresh PhiWsData and Complete Workspace setup
     `phi ws setup` is a generic catch-all function. It should handle errors graciously
     and provide "how to fix" messages and "next steps" to get the user running.
     """
+    from phiterm.cli.cli_operator import initialize_phidata
     from phiterm.utils.git import get_remote_origin_for_dir
     from phiterm.workspace.ws_utils import print_howtofix_pending_actions
 
     print_heading("Running workspace setup\n")
 
     ######################################################
     ## 1. Validate Pre-requisites
@@ -239,16 +240,20 @@
         return False
 
     ######################################################
     # 1.2 Check PhiConf is valid
     ######################################################
     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
     if not phi_conf:
-        print_conf_not_available_msg()
-        return False
+        # Phidata should be initialized before workspace setup
+        initialize_phidata()
+        phi_conf = PhiConf.get_saved_conf()
+        # If phi_conf is still None, throw an error
+        if not phi_conf:
+            raise Exception("Failed to initialize phidata")
 
     ######################################################
     # 1.3 Validate PhiWsData is available
     ######################################################
     logger.debug(f"Checking for a workspace at {ws_root_path}")
     ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_path(ws_root_path)
     if ws_data is None:
```

### Comparing `phiterm-1.6.5/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.6/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm/workspace/ws_utils.py` & `phiterm-1.6.6/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.6/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.5/pyproject.toml` & `phiterm-1.6.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.5"
+version = "1.6.6"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

