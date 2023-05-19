# Comparing `tmp/specctl-0.1.2.tar.gz` & `tmp/specctl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specctl-0.1.2.tar", max compression
+gzip compressed data, was "specctl-0.1.3.tar", max compression
```

## Comparing `specctl-0.1.2.tar` & `specctl-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,20 @@
--rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.2/LICENSE
--rw-r--r--   0        0        0      306 2023-05-09 01:54:35.902307 specctl-0.1.2/README.md
--rw-r--r--   0        0        0      441 2023-05-18 19:15:10.089082 specctl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 18:38:31.015930 specctl-0.1.2/specctl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 18:38:31.023189 specctl-0.1.2/specctl/ecs2k8s/__init__.py
--rw-r--r--   0        0        0      142 2023-05-18 18:38:31.028104 specctl-0.1.2/specctl/ecs2k8s/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7436 2023-05-18 18:38:31.027441 specctl-0.1.2/specctl/ecs2k8s/__pycache__/ecs_parser.cpython-310.pyc
--rw-r--r--   0        0        0     7654 2023-05-18 18:38:31.026610 specctl-0.1.2/specctl/ecs2k8s/__pycache__/ecs_reader_writer.cpython-310.pyc
--rw-r--r--   0        0        0     1463 2023-05-18 18:38:31.025781 specctl-0.1.2/specctl/ecs2k8s/__pycache__/k8s_objects.cpython-310.pyc
--rw-r--r--   0        0        0    11015 2023-05-18 18:38:31.021743 specctl-0.1.2/specctl/ecs2k8s/ecs_parser.py
--rw-r--r--   0        0        0    11322 2023-05-18 18:38:31.028781 specctl-0.1.2/specctl/ecs2k8s/ecs_reader_writer.py
--rw-r--r--   0        0        0     2351 2023-05-18 18:38:31.022613 specctl-0.1.2/specctl/ecs2k8s/k8s_objects.py
--rw-r--r--   0        0        0     3444 2023-05-18 18:38:31.048681 specctl-0.1.2/specctl/k8s2ecs/README.md
--rw-r--r--   0        0        0        0 2023-05-18 18:38:31.038690 specctl-0.1.2/specctl/k8s2ecs/__init__.py
--rw-r--r--   0        0        0      142 2023-05-18 18:38:31.045083 specctl-0.1.2/specctl/k8s2ecs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1258 2023-05-18 18:38:31.045769 specctl-0.1.2/specctl/k8s2ecs/__pycache__/ecs_objects.cpython-310.pyc
--rw-r--r--   0        0        0     3306 2023-05-18 18:38:31.044185 specctl-0.1.2/specctl/k8s2ecs/__pycache__/ecs_output.cpython-310.pyc
--rw-r--r--   0        0        0     6773 2023-05-18 18:38:31.041063 specctl-0.1.2/specctl/k8s2ecs/__pycache__/ingress.cpython-310.pyc
--rw-r--r--   0        0        0    13857 2023-05-18 18:38:31.042714 specctl-0.1.2/specctl/k8s2ecs/__pycache__/k8s_parser.cpython-310.pyc
--rw-r--r--   0        0        0     4189 2023-05-18 18:38:31.043519 specctl-0.1.2/specctl/k8s2ecs/__pycache__/k8s_reader.cpython-310.pyc
--rw-r--r--   0        0        0     3469 2023-05-18 18:38:31.041778 specctl-0.1.2/specctl/k8s2ecs/__pycache__/tf_output.cpython-310.pyc
--rw-r--r--   0        0        0     1628 2023-05-18 18:38:31.050019 specctl-0.1.2/specctl/k8s2ecs/ecs_objects.py
--rw-r--r--   0        0        0     5175 2023-05-18 18:38:31.047023 specctl-0.1.2/specctl/k8s2ecs/ecs_output.py
--rw-r--r--   0        0        0    12173 2023-05-18 18:38:31.038266 specctl-0.1.2/specctl/k8s2ecs/ingress.py
--rw-r--r--   0        0        0    27795 2023-05-18 18:38:31.052025 specctl-0.1.2/specctl/k8s2ecs/k8s_parser.py
--rw-r--r--   0        0        0     6465 2023-05-18 18:38:31.050938 specctl-0.1.2/specctl/k8s2ecs/k8s_reader.py
--rw-r--r--   0        0        0     4753 2023-05-18 18:38:31.037049 specctl-0.1.2/specctl/k8s2ecs/tf_output.py
--rw-r--r--   0        0        0     1873 2023-05-18 18:38:31.054211 specctl-0.1.2/specctl/quantity.py
--rw-r--r--   0        0        0     4719 2023-05-18 18:38:31.053013 specctl-0.1.2/specctl/specctl.py
--rw-r--r--   0        0        0     1757 2023-05-18 18:38:31.030037 specctl-0.1.2/specctl/utils.py
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 specctl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12192 2023-05-19 00:46:47.759640 specctl-0.1.3/README.md
+-rw-r--r--   0        0        0      441 2023-05-19 00:48:17.631594 specctl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.045382 specctl-0.1.3/specctl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.064218 specctl-0.1.3/specctl/ecs2k8s/__init__.py
+-rw-r--r--   0        0        0    11015 2023-05-19 00:47:05.058566 specctl-0.1.3/specctl/ecs2k8s/ecs_parser.py
+-rw-r--r--   0        0        0    11322 2023-05-19 00:47:05.070202 specctl-0.1.3/specctl/ecs2k8s/ecs_reader_writer.py
+-rw-r--r--   0        0        0     2351 2023-05-19 00:47:05.062861 specctl-0.1.3/specctl/ecs2k8s/k8s_objects.py
+-rw-r--r--   0        0        0     3444 2023-05-19 00:47:05.082926 specctl-0.1.3/specctl/k8s2ecs/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.074140 specctl-0.1.3/specctl/k8s2ecs/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-19 00:47:05.083773 specctl-0.1.3/specctl/k8s2ecs/ecs_objects.py
+-rw-r--r--   0        0        0     5175 2023-05-19 00:47:05.081450 specctl-0.1.3/specctl/k8s2ecs/ecs_output.py
+-rw-r--r--   0        0        0    12173 2023-05-19 00:47:05.073674 specctl-0.1.3/specctl/k8s2ecs/ingress.py
+-rw-r--r--   0        0        0    27795 2023-05-19 00:47:05.090036 specctl-0.1.3/specctl/k8s2ecs/k8s_parser.py
+-rw-r--r--   0        0        0     6465 2023-05-19 00:47:05.088657 specctl-0.1.3/specctl/k8s2ecs/k8s_reader.py
+-rw-r--r--   0        0        0     5453 2023-05-19 00:47:05.072663 specctl-0.1.3/specctl/k8s2ecs/tf_output.py
+-rw-r--r--   0        0        0     1873 2023-05-19 00:47:05.092119 specctl-0.1.3/specctl/quantity.py
+-rw-r--r--   0        0        0     5377 2023-05-19 00:47:05.091443 specctl-0.1.3/specctl/specctl.py
+-rw-r--r--   0        0        0     1757 2023-05-19 00:47:05.071056 specctl-0.1.3/specctl/utils.py
+-rw-r--r--   0        0        0    12943 1970-01-01 00:00:00.000000 specctl-0.1.3/PKG-INFO
```

### Comparing `specctl-0.1.2/LICENSE` & `specctl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/ecs2k8s/ecs_parser.py` & `specctl-0.1.3/specctl/ecs2k8s/ecs_parser.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/ecs2k8s/ecs_reader_writer.py` & `specctl-0.1.3/specctl/ecs2k8s/ecs_reader_writer.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/ecs2k8s/k8s_objects.py` & `specctl-0.1.3/specctl/ecs2k8s/k8s_objects.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/README.md` & `specctl-0.1.3/specctl/k8s2ecs/README.md`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/ecs_objects.py` & `specctl-0.1.3/specctl/k8s2ecs/ecs_objects.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/ecs_output.py` & `specctl-0.1.3/specctl/k8s2ecs/ecs_output.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/ingress.py` & `specctl-0.1.3/specctl/k8s2ecs/ingress.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/k8s_parser.py` & `specctl-0.1.3/specctl/k8s2ecs/k8s_parser.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/k8s_reader.py` & `specctl-0.1.3/specctl/k8s2ecs/k8s_reader.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/k8s2ecs/tf_output.py` & `specctl-0.1.3/specctl/k8s2ecs/tf_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 import os
 import shutil
 import logging
 
 logger = logging.getLogger(__name__)
 
 # This will generate TFvars format output key = value
-TF_MODULES_DIRECTORY = {
-    "namespaces": "./terraform/namespaces",
-    "ecs-lb-service": "./terraform/ecs-lb-service",
-    "ecs-backend-service": "./terraform/ecs-backend-service"
-}
-TF_FILES = ["main.tf","variables.tf","outputs.tf", "versions.tf"]
-
 def hcl_fmt(value):
     if type(value) == int or type(value) == float:
         return str(value)
     return (json.dumps(value, indent=2, separators=[",", " = "]))
 
 def write_hcl(key, value, tf_file):
     with open(tf_file, 'a') as tf:
@@ -30,24 +23,40 @@
             continue
         write_hcl(key, value, tf_file)
 
 def write_hcl_dict_list(dict_list_obj, tf_file, ignore_keys=[]):
     for dict_obj in dict_list_obj:
         write_hcl_dict(dict_obj, tf_file, ignore_keys)
 
-def copy_tf_modules(src_dir, dest_dir):
-    for fn in TF_FILES:
+def copy_tf_modules(src_dir, dest_dir, tf_files):
+    for fn in tf_files:
         src_file = os.path.join(src_dir, fn)
         if not os.path.isfile(src_file): continue
         logger.info("Copying TF modules %s to %s"%(src_file, dest_dir))
         shutil.copy(src_file, dest_dir)
     return
+def get_tf_modules_directory_map(tf_modules_directory, tf_modules_name_map):
+    tf_modules_list = tf_modules_name_map.split(",")
+    tf_modules_directory_map = {}
+    for tf_module in tf_modules_list:
+        key = tf_module.split(":")[0].strip()
+        value = tf_module.split(":")[1].strip()
+        value_with_path =os.path.join(tf_modules_directory,value)
+        tf_modules_directory_map[key]=value_with_path
+        if not os.path.exists(value_with_path):
+            logger.error("Terraform module path %s for key %s doesn't exist"%(value_with_path,key))
+    return tf_modules_directory_map
 
 def terraform_print(output_dict, options):
     # where are the terraform modules
+    tf_modules_directory = options.get("tf_modules_directory")
+    tf_modules_name_map = options.get("tf_modules_name_map")
+    tf_files = [f.strip() for f in options.get("tf_files").split(",")]
+    tf_modules_directory_map = get_tf_modules_directory_map(tf_modules_directory, tf_modules_name_map)
+
     # ssm secrets, parameters, and namespaces are written in output/namespaces/terraform.tfvars
     output_dir = os.path.join(options.get("output_directory"),"namespaces")
     try:
         os.makedirs(output_dir)
     except FileExistsError:
         pass
     tfvars_file = os.path.join(output_dir, options.get("tfvars_file"))
@@ -60,15 +69,15 @@
     namespaces.append("default")
     namespaces = [*set(namespaces)]
     total_params = configmaps+secrets
     logger.info("Writing %d configmaps %d secrets and %d namespaces in %s"%(len(configmaps), len(secrets), len(namespaces), tfvars_file))
     write_hcl_dict_list(total_params, tfvars_file, [])
     write_hcl("namespaces", namespaces, tfvars_file)
     write_hcl_dict(ingress, tfvars_file)
-    copy_tf_modules(TF_MODULES_DIRECTORY.get("namespaces"), output_dir)
+    copy_tf_modules(tf_modules_directory_map.get("namespaces"), output_dir, tf_files)
     # rest are written in output/namespace/service/terraform.tfvars
     services = output_dict.get("services",[])
     for svc in services:
         svc_namespace = svc.get("service_namespace")
         svc_name = svc.get("service_name","")
         if svc_namespace is None or len(svc_namespace)<=0:
             svc_namespace = "default"
@@ -105,12 +114,12 @@
                 write_hcl("lb_container_name", lb_container_name, tfvars_file)
 
             write_hcl_dict(dep, tfvars_file, ["containers"])
 
         write_hcl_dict(svc, tfvars_file, ["deployment","lb_ports"])
         svc_type = svc.get("service_type","ClusterIP")
         if svc_type == "LoadBalancer":
-            copy_tf_modules(TF_MODULES_DIRECTORY["ecs-lb-service"], output_dir)
+            copy_tf_modules(tf_modules_directory_map["ecs-lb-service"], output_dir, tf_files)
         else:
-            copy_tf_modules(TF_MODULES_DIRECTORY["ecs-backend-service"], output_dir)
+            copy_tf_modules(tf_modules_directory_map["ecs-backend-service"], output_dir, tf_files)
 
     logger.log(100, "Please see %s directory for terraform tfvars" %(options.get("output_directory")))
```

### Comparing `specctl-0.1.2/specctl/quantity.py` & `specctl-0.1.3/specctl/quantity.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.2/specctl/specctl.py` & `specctl-0.1.3/specctl/specctl.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,19 +73,22 @@
 @click.option("-c", "--context", default="", type=str, help="Kubeconfig context name to load")
 @click.option("-l", "--log_level", default="WARNING", type=click.Choice(["DEBUG","INFO","WARNING","ERROR","CRITICAL"], case_sensitive=False), help="Select log level")
 @click.option("-n", "--namespaces", default="", type=str, help="Only fetch namespaces specified here as comma separated string. Applies only when converting from K8s clusters and not from spec files")
 @click.option("--td_file",default="taskdefinition.json", help="File to write ECS task definition json")
 @click.option("--sd_file",default="servicedefinition.json", help="File to write ECS service definition json")
 @click.option("--input_file", default="", help="File with additional input parameters for task, container, and/or services")
 @click.option("--tfvars_file", default="terraform.tfvars", help="File to write the Terraform tfvars")
-@click.option("--output_directory", default="./output", help="Path to output directory")
+@click.option("-d", "--tf_modules_directory", default="./terraform", help="Path to Terraform modules directory")
+@click.option("--tf_modules_name_map", default="namespaces:namespaces,ecs-lb-service:ecs-lb-service,ecs-backend-service:ecs-backend-service", help="Change the value in this map to your terraform modules directory")
+@click.option("--tf_files", default="main.tf,versions.tf,variables.tf,outputs.tf", help="List of files to use from Terraform modules")
+@click.option("-o", "--output_directory", default="./output", help="Path to output directory")
 @click.option("--ecs_cluster_name", default="", type=str, help="ECS cluster to extract services and tasks")
 @click.option("--ecs_region_name", default="", type=str, help="Region name for ECS cluster")
 @click.option("--sgp", is_flag="True", help="Create EKS Security Group Policy from task security groups")
-def transform(mode, source, context, log_level, namespaces, td_file, sd_file, input_file, tfvars_file, output_directory, ecs_cluster_name, ecs_region_name, sgp):
+def transform(mode, source, context, log_level, namespaces, td_file, sd_file, input_file, tfvars_file, tf_modules_directory, tf_modules_name_map, tf_files, output_directory, ecs_cluster_name, ecs_region_name, sgp):
     logger.setLevel(getattr(logging,log_level.upper()))
     for handler in logger.handlers:
         handler.setLevel(getattr(logging,log_level.upper()))
     try:
         makedirs(output_directory)
     except FileExistsError:
         pass
@@ -94,14 +97,17 @@
         namespace_list=namespaces.split(",")
     options = {
         "namespaces":namespace_list,
         "td_file": td_file,
         "sd_file": sd_file,
         "input_file": input_file,
         "tfvars_file": tfvars_file,
+        "tf_modules_directory": tf_modules_directory,
+        "tf_modules_name_map": tf_modules_name_map,
+        "tf_files": tf_files,
         "output_directory" : output_directory,
         "cluster_name" : ecs_cluster_name,
         "region_name" : ecs_region_name,
         "sgp": sgp
         }
     if mode == "k2e":
         k2e_cli_handler(source, context, options)
```

### Comparing `specctl-0.1.2/specctl/utils.py` & `specctl-0.1.3/specctl/utils.py`

 * *Files identical despite different names*

