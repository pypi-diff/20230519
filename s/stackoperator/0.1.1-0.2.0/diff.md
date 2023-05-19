# Comparing `tmp/stackoperator-0.1.1.tar.gz` & `tmp/stackoperator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoperator-0.1.1.tar", last modified: Thu May 18 12:41:09 2023, max compression
+gzip compressed data, was "stackoperator-0.2.0.tar", last modified: Fri May 19 13:47:28 2023, max compression
```

## Comparing `stackoperator-0.1.1.tar` & `stackoperator-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:41:09.705670 stackoperator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-18 12:41:09.705670 stackoperator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-18 12:40:59.000000 stackoperator-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 12:40:59.000000 stackoperator-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:41:09.705670 stackoperator-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:41:09.701670 stackoperator-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:41:09.701670 stackoperator-0.1.1/src/stackoperator/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-18 12:40:59.000000 stackoperator-0.1.1/src/stackoperator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5132 2023-05-18 12:40:59.000000 stackoperator-0.1.1/src/stackoperator/batchOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-18 12:40:59.000000 stackoperator-0.1.1/src/stackoperator/cfnReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 12:40:59.000000 stackoperator-0.1.1/src/stackoperator/readerFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-18 12:40:59.000000 stackoperator-0.1.1/src/stackoperator/tfReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:41:09.705670 stackoperator-0.1.1/src/stackoperator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 12:41:09.000000 stackoperator-0.1.1/src/stackoperator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:28.843603 stackoperator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-19 13:47:28.843603 stackoperator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-19 13:47:20.000000 stackoperator-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-19 13:47:20.000000 stackoperator-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:47:28.843603 stackoperator-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:28.843603 stackoperator-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:28.843603 stackoperator-0.2.0/src/stackoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5211 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/batchOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/cfnReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/readerFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/resourcegroupReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-19 13:47:20.000000 stackoperator-0.2.0/src/stackoperator/tfReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:47:28.843603 stackoperator-0.2.0/src/stackoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 13:47:28.000000 stackoperator-0.2.0/src/stackoperator.egg-info/top_level.txt
```

### Comparing `stackoperator-0.1.1/PKG-INFO` & `stackoperator-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: stackoperator
-Version: 0.1.1
+Version: 0.2.0
 Summary: A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.
 Author-email: Henry Huo <happy78@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.  
-Stackoperator now support CloudFormation and Terraform stack.  
+Stackoperator now support CloudFormation,Terraform stack,as well Resource Group.  
 It's a great idea to use stackoperator with [Instance Scheduler on AWS](https://aws.amazon.com/solutions/implementations/instance-scheduler-on-aws) solution by tagging stoppable resources created by IaC stack.  
 
 ## Use cases:
 - During the POC testing process of solutions deployed using CloudFormation or Terraform, toggle related resources with one click to save testing costs.
 - For solutions deployed using CloudFormation or Terraform, save operation costs by tagging toggleable resources and controlling their runtime using the Instance Scheduler on AWS solution.
+- Batch Start,Stop and Tag toggleable resources in a resource group.
 
 ## Prerequisites:
 Before using stackoperator script, please make sure correct AWS credential in envs, using [aws-vault](https://github.com/99designs/aws-vault) to store and switch AWS credentials is recommend.
 
 ## Install
 ```
 pip install stackoperator
@@ -51,7 +52,19 @@
 ```
 stoptfstack [--statefile <Terraform_Stack_StateFile>]  
 ```
 ### Tag stoppable running resources in Terraform Stack (at current path)
 ```
 tagtfstack --tags "Key1=Value1,Key2=Value2" [--statefile <Terraform_Stack_StateFile>]  
 ```
+### Start stopped resources in Resrouce Group
+```
+startresourcegroup --groupname <Resource_Group_Name>   
+```
+### Stop stoppable running resources in Resource Group
+```
+startresourcegroup --groupname <Resource_Group_Name>    
+```
+### Tag stoppable running resources in Resource Group
+```
+tagresourcegroup --tags "Key1=Value1,Key2=Value2" --groupname <Resource_Group_Name>
+```
```

### Comparing `stackoperator-0.1.1/README.md` & `stackoperator-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.  
-Stackoperator now support CloudFormation and Terraform stack.  
+Stackoperator now support CloudFormation,Terraform stack,as well Resource Group.  
 It's a great idea to use stackoperator with [Instance Scheduler on AWS](https://aws.amazon.com/solutions/implementations/instance-scheduler-on-aws) solution by tagging stoppable resources created by IaC stack.  
 
 ## Use cases:
 - During the POC testing process of solutions deployed using CloudFormation or Terraform, toggle related resources with one click to save testing costs.
 - For solutions deployed using CloudFormation or Terraform, save operation costs by tagging toggleable resources and controlling their runtime using the Instance Scheduler on AWS solution.
+- Batch Start,Stop and Tag toggleable resources in a resource group.
 
 ## Prerequisites:
 Before using stackoperator script, please make sure correct AWS credential in envs, using [aws-vault](https://github.com/99designs/aws-vault) to store and switch AWS credentials is recommend.
 
 ## Install
 ```
 pip install stackoperator
@@ -39,8 +40,20 @@
 ### Stop stoppable running resources in Terraform Stack (at current path)
 ```
 stoptfstack [--statefile <Terraform_Stack_StateFile>]  
 ```
 ### Tag stoppable running resources in Terraform Stack (at current path)
 ```
 tagtfstack --tags "Key1=Value1,Key2=Value2" [--statefile <Terraform_Stack_StateFile>]  
+```
+### Start stopped resources in Resrouce Group
+```
+startresourcegroup --groupname <Resource_Group_Name>   
+```
+### Stop stoppable running resources in Resource Group
+```
+startresourcegroup --groupname <Resource_Group_Name>    
+```
+### Tag stoppable running resources in Resource Group
+```
+tagresourcegroup --tags "Key1=Value1,Key2=Value2" --groupname <Resource_Group_Name>
 ```
```

### Comparing `stackoperator-0.1.1/pyproject.toml` & `stackoperator-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stackoperator"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     {name = "Henry Huo", email = "happy78@live.com"},
 ]
 description = "A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -19,11 +19,14 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent"
 ]
 
 [project.scripts]
 startcfnstack = "stackoperator:start_cfnstack"
 stopcfnstack = "stackoperator:stop_cfnstack"
+tagcfnstack = "stackoperator:tag_cfnstack"
 starttfstack = "stackoperator:start_tfstack"
 stoptfstack = "stackoperator:stop_tfstack"
-tagcfnstack = "stackoperator:tag_cfnstack"
-tagtfstack = "stackoperator:tag_tfstack"
+tagtfstack = "stackoperator:tag_tfstack"
+startresourcegroup = "stackoperator:start_resourcegroup"
+stopresourcegroup = "stackoperator:stop_resourcegroup"
+tagresourcegroup = "stackoperator:tag_resourcegroup"
```

### Comparing `stackoperator-0.1.1/src/stackoperator/__init__.py` & `stackoperator-0.2.0/src/stackoperator/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,14 +63,40 @@
     factory = readerFactory()
     reader = factory.create_reader('tf',args.StateFile)
     ec2_list,rds_list,asg_list = reader.list_stoppable_resources()
 
     operator = batchOperator()
     operator.batch_stop_resources(ec2_list,rds_list,asg_list)
 
+def start_resourcegroup():
+    # 创建 ArgumentParser 对象
+    parser = argparse.ArgumentParser(description='Start all startable resources in a Resource Group.')
+    parser.add_argument('--groupname', help='Resource Group name.', dest='GroupName')
+    args = parser.parse_args()
+
+    factory = readerFactory()
+    reader = factory.create_reader('rsg',args.GroupName)
+    ec2_list,rds_list,asg_list = reader.list_stoppable_resources(filterstatus='stopped')
+
+    operator = batchOperator()
+    operator.batch_start_resources(ec2_list,rds_list,asg_list)
+
+def stop_resourcegroup():
+    # 创建 ArgumentParser 对象
+    parser = argparse.ArgumentParser(description='Stop all startable resources in a Resource Group.')
+    parser.add_argument('--groupname', help='Resource Group name.', dest='GroupName')
+    args = parser.parse_args()
+
+    factory = readerFactory()
+    reader = factory.create_reader('rsg',args.GroupName)
+    ec2_list,rds_list,asg_list = reader.list_stoppable_resources()
+
+    operator = batchOperator()
+    operator.batch_stop_resources(ec2_list,rds_list,asg_list)
+
 def tag_cfnstack():
     # 创建 ArgumentParser 对象
     parser = argparse.ArgumentParser(description='Tag all stoppable resources in CloudFormation stack.')
     parser.add_argument('--stackname', dest='StackName', help='CloudFormation stack name.')
     parser.add_argument('--tags', dest='Tags', help='Tags to apply to resources. Format: key1=value1,key2=value2')
     args = parser.parse_args()
 
@@ -90,14 +116,28 @@
     factory = readerFactory()
     reader = factory.create_reader('tf',args.StateFile)
     ec2_list,rds_list,asg_list = reader.list_stoppable_resources(filterstatus='both')
 
     operator = batchOperator()
     operator.batch_tag_resources(ec2_list,rds_list,asg_list,parse_tags(args.Tags))
 
+def tag_resourcegroup():
+    # 创建 ArgumentParser 对象
+    parser = argparse.ArgumentParser(description='Tag all stoppable resources in Resource Group.')
+    parser.add_argument('--groupname', help='Resource Group name.', dest='GroupName')
+    parser.add_argument('--tags', dest='Tags', help='Tags to apply to resources. Format: key1=value1,key2=value2')
+    args = parser.parse_args()
+
+    factory = readerFactory()
+    reader = factory.create_reader('rsg',args.GroupName)
+    ec2_list,rds_list,asg_list = reader.list_stoppable_resources(filterstatus='both')
+
+    operator = batchOperator()
+    operator.batch_tag_resources(ec2_list,rds_list,asg_list,parse_tags(args.Tags))
+
 def parse_tags(tag_string):  
     tag_list = tag_string.split(',')  
     tags = []  
   
     for tag in tag_list:  
         key, value = tag.split('=')  
         tags.append({
```

### Comparing `stackoperator-0.1.1/src/stackoperator/batchOperator.py` & `stackoperator-0.2.0/src/stackoperator/batchOperator.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
                     AutoScalingGroupName=asg_item['AutoScalingGroupName'],
                     MinSize=int(original_min_size),
                     DesiredCapacity=int(original_desired_capacity)
                 )
 
         print("All startable resources within the CloudFormation stack have been started.")
 
-    def batch_tag_resources(self,ec2,rds,asg,tags):
+    def batch_tag_resources(self,ec2,rds,asg,tags=''):
+        if tags == '':
+            raise ValueError("Tags not specified")
         ec2_client = boto3.client('ec2')
         rds_client = boto3.client('rds')
         
         # Add tags to EC2 instances
         if ec2:
             for instance_id in ec2:
                 print(f"Adding tags to EC2 Instance: {instance_id}")
```

### Comparing `stackoperator-0.1.1/src/stackoperator/cfnReader.py` & `stackoperator-0.2.0/src/stackoperator/cfnReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import boto3
 
 class cfnReader:
-    def __init__(self, StackName):
+    def __init__(self, StackName=''):
+        if StackName == '':
+            raise ValueError("Stackname not specified")
         self.stackname = StackName
 
     def list_stoppable_resources(self,StackName="",filterstatus='running'):
         # Initialize AWS clients
         cf_client = boto3.client('cloudformation')
         ec2_client = boto3.client('ec2')
         rds_client = boto3.client("rds")
```

### Comparing `stackoperator-0.1.1/src/stackoperator/tfReader.py` & `stackoperator-0.2.0/src/stackoperator/tfReader.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.1.1/src/stackoperator.egg-info/PKG-INFO` & `stackoperator-0.2.0/src/stackoperator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: stackoperator
-Version: 0.1.1
+Version: 0.2.0
 Summary: A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.
 Author-email: Henry Huo <happy78@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.  
-Stackoperator now support CloudFormation and Terraform stack.  
+Stackoperator now support CloudFormation,Terraform stack,as well Resource Group.  
 It's a great idea to use stackoperator with [Instance Scheduler on AWS](https://aws.amazon.com/solutions/implementations/instance-scheduler-on-aws) solution by tagging stoppable resources created by IaC stack.  
 
 ## Use cases:
 - During the POC testing process of solutions deployed using CloudFormation or Terraform, toggle related resources with one click to save testing costs.
 - For solutions deployed using CloudFormation or Terraform, save operation costs by tagging toggleable resources and controlling their runtime using the Instance Scheduler on AWS solution.
+- Batch Start,Stop and Tag toggleable resources in a resource group.
 
 ## Prerequisites:
 Before using stackoperator script, please make sure correct AWS credential in envs, using [aws-vault](https://github.com/99designs/aws-vault) to store and switch AWS credentials is recommend.
 
 ## Install
 ```
 pip install stackoperator
@@ -51,7 +52,19 @@
 ```
 stoptfstack [--statefile <Terraform_Stack_StateFile>]  
 ```
 ### Tag stoppable running resources in Terraform Stack (at current path)
 ```
 tagtfstack --tags "Key1=Value1,Key2=Value2" [--statefile <Terraform_Stack_StateFile>]  
 ```
+### Start stopped resources in Resrouce Group
+```
+startresourcegroup --groupname <Resource_Group_Name>   
+```
+### Stop stoppable running resources in Resource Group
+```
+startresourcegroup --groupname <Resource_Group_Name>    
+```
+### Tag stoppable running resources in Resource Group
+```
+tagresourcegroup --tags "Key1=Value1,Key2=Value2" --groupname <Resource_Group_Name>
+```
```

