# Comparing `tmp/iam_actions-1.2.20230518.tar.gz` & `tmp/iam_actions-1.2.20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230518.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230519.tar", max compression
```

## Comparing `iam_actions-1.2.20230518.tar` & `iam_actions-1.2.20230519.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/README.md
--rw-r--r--   0        0        0      228 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/__init__.py
--rw-r--r--   0        0        0  4256968 2023-05-18 02:27:59.004777 iam_actions-1.2.20230518/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-18 02:26:27.872776 iam_actions-1.2.20230518/iam_actions/generate/services.py
--rw-r--r--   0        0        0   547379 2023-05-18 02:27:59.004777 iam_actions-1.2.20230518/iam_actions/policies.json
--rw-r--r--   0        0        0   193861 2023-05-18 02:27:59.004777 iam_actions-1.2.20230518/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   530973 2023-05-18 02:27:59.004777 iam_actions-1.2.20230518/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-18 02:27:59.928776 iam_actions-1.2.20230518/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230518/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230518/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 02:26:50.505310 iam_actions-1.2.20230519/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-19 02:26:50.505310 iam_actions-1.2.20230519/README.md
+-rw-r--r--   0        0        0      228 2023-05-19 02:26:50.505310 iam_actions-1.2.20230519/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4258838 2023-05-19 02:28:26.650880 iam_actions-1.2.20230519/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-19 02:26:50.509311 iam_actions-1.2.20230519/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   547482 2023-05-19 02:28:26.650880 iam_actions-1.2.20230519/iam_actions/policies.json
+-rw-r--r--   0        0        0   194119 2023-05-19 02:28:26.650880 iam_actions-1.2.20230519/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   531071 2023-05-19 02:28:26.650880 iam_actions-1.2.20230519/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-19 02:28:27.402892 iam_actions-1.2.20230519/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230519/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230519/PKG-INFO
```

### Comparing `iam_actions-1.2.20230518/LICENSE` & `iam_actions-1.2.20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/README.md` & `iam_actions-1.2.20230519/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/actions.json` & `iam_actions-1.2.20230519/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999494126804693%*

 * *Differences: {"'apigateway'": "{'PUT': {'resources': {insert: [(0, 'Api')]}}}",*

 * * "'cloud9'": "{'GetMigrationExperiences': {'access_level': 'Read', 'description': 'Grants "*

 * *             "permission to get the migration experience for a cloud9 user'}}",*

 * * "'cloudformation'": "{'DescribeStacks': {'description': 'Grants permission to return the "*

 * *                     'description for the specified stack, and to all stacks when used in '*

 * *                     "combination with the ListStacks action'}, 'ListStacks': {'descripti […]*

```diff
@@ -3336,14 +3336,15 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a particular resource",
             "orphan": false,
             "resources": [
+                "Api",
                 "Apis"
             ]
         },
         "RemoveCertificateFromDomain": {
             "access_level": "Permissions management",
             "action": "RemoveCertificateFromDomain",
             "condition_keys": [],
@@ -17532,18 +17533,18 @@
             "description": "Grants permission to get the AWS Cloud9 IDE settings for a specified environment member",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "GetMigrationExperiences": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetMigrationExperiences",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the migration experience for a cloud9 user",
             "orphan": false,
             "resources": []
         },
         "GetUserPublicKey": {
             "access_level": "Read",
             "action": "GetUserPublicKey",
             "condition_keys": [
@@ -18674,15 +18675,15 @@
                 "stackset"
             ]
         },
         "DescribeStacks": {
             "access_level": "List",
             "action": "DescribeStacks",
             "condition_keys": [],
-            "description": "Grants permission to return the description for the specified stack",
+            "description": "Grants permission to return the description for the specified stack, and to all stacks when used in combination with the ListStacks action",
             "orphan": false,
             "resources": [
                 "stack"
             ]
         },
         "DescribeType": {
             "access_level": "Read",
@@ -18899,15 +18900,15 @@
                 "stackset"
             ]
         },
         "ListStacks": {
             "access_level": "List",
             "action": "ListStacks",
             "condition_keys": [],
-            "description": "Grants permission to return the summary information for stacks whose status matches the specified StackStatusFilter",
+            "description": "Grants permission to return the summary information for stacks whose status matches the specified StackStatusFilter. In combination with the DescribeStacks action, grants permission to list descriptions for stacks",
             "orphan": false,
             "resources": []
         },
         "ListTypeRegistrations": {
             "access_level": "List",
             "action": "ListTypeRegistrations",
             "condition_keys": [],
@@ -29817,14 +29818,22 @@
             "description": "Grants permission to add a participant to an ongoing contact",
             "orphan": false,
             "resources": [
                 "contact",
                 "instance"
             ]
         },
+        "CreatePrompt": {
+            "access_level": "Undocumented",
+            "action": "CreatePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateQueue": {
             "access_level": "Write",
             "action": "CreateQueue",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "connect:InstanceId"
@@ -30082,14 +30091,22 @@
             "description": "Grants permission to delete an integration association from an Amazon Connect instance. The association must not have any use cases associated with it",
             "orphan": false,
             "resources": [
                 "instance",
                 "integration-association"
             ]
         },
+        "DeletePrompt": {
+            "access_level": "Undocumented",
+            "action": "DeletePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteQuickConnect": {
             "access_level": "Write",
             "action": "DeleteQuickConnect",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -30350,14 +30367,22 @@
             ],
             "description": "Grants permission to describe phone number resources in an Amazon Connect instance or traffic distribution group",
             "orphan": false,
             "resources": [
                 "phone-number"
             ]
         },
+        "DescribePrompt": {
+            "access_level": "Undocumented",
+            "action": "DescribePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeQueue": {
             "access_level": "Read",
             "action": "DescribeQueue",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -30700,14 +30725,22 @@
             "resources": [
                 "hierarchy-group",
                 "queue",
                 "routing-profile",
                 "user"
             ]
         },
+        "GetPromptFile": {
+            "access_level": "Undocumented",
+            "action": "GetPromptFile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetTaskTemplate": {
             "access_level": "Read",
             "action": "GetTaskTemplate",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -31723,14 +31756,22 @@
             "orphan": false,
             "resources": [
                 "instance",
                 "phone-number",
                 "traffic-distribution-group"
             ]
         },
+        "UpdatePrompt": {
+            "access_level": "Undocumented",
+            "action": "UpdatePrompt",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateQueueHoursOfOperation": {
             "access_level": "Write",
             "action": "UpdateQueueHoursOfOperation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
@@ -41577,29 +41618,25 @@
             "resources": [
                 "table"
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:TagKeys"
-            ],
+            "condition_keys": [],
             "description": "Grants permission to associate a set of tags with an Amazon DynamoDB resource",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:TagKeys"
-            ],
+            "condition_keys": [],
             "description": "Grants permission to remove the association of tags from an Amazon DynamoDB resource",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "UpdateContinuousBackups": {
@@ -42286,20 +42323,26 @@
                 "ec2:Region"
             ],
             "description": "Grants permission to associate a branch network interface with a trunk network interface",
             "orphan": false,
             "resources": []
         },
         "AssociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to associate an AWS Web Application Firewall (WAF) web access control list (ACL) with a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "AssociateVpcCidrBlock": {
             "access_level": "Write",
             "action": "AssociateVpcCidrBlock",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Ipv4IpamPoolId",
@@ -42833,21 +42876,24 @@
                 "coip-pool"
             ]
         },
         "CreateCoipPool": {
             "access_level": "Write",
             "action": "CreateCoipPool",
             "condition_keys": [
+                "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to create a pool of customer-owned IP (CoIP) addresses",
             "orphan": false,
             "resources": [
+                "coip-pool",
                 "local-gateway-route-table"
             ]
         },
         "CreateCoipPoolPermission": {
             "access_level": "Write",
             "action": "CreateCoipPoolPermission",
             "condition_keys": [
@@ -42932,16 +42978,14 @@
         "CreateFleet": {
             "access_level": "Write",
             "action": "CreateFleet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AvailabilityZone",
                 "ec2:EbsOptimized",
                 "ec2:Encrypted",
                 "ec2:ImageID",
                 "ec2:ImageType",
                 "ec2:InstanceID",
                 "ec2:InstanceProfile",
@@ -43419,16 +43463,14 @@
             "access_level": "Write",
             "action": "CreateNetworkInsightsPath",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:AccepterVpc",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AvailabilityZone",
                 "ec2:EbsOptimized",
                 "ec2:InstanceID",
                 "ec2:InstanceProfile",
                 "ec2:InstanceType",
                 "ec2:InternetGatewayID",
                 "ec2:NetworkInterfaceID",
@@ -43447,14 +43489,15 @@
             "resources": [
                 "instance",
                 "internet-gateway",
                 "network-insights-path",
                 "network-interface",
                 "transit-gateway",
                 "vpc-endpoint",
+                "vpc-endpoint-service",
                 "vpc-peering-connection",
                 "vpn-gateway"
             ]
         },
         "CreateNetworkInterface": {
             "access_level": "Write",
             "action": "CreateNetworkInterface",
@@ -43780,29 +43823,26 @@
         "CreateTags": {
             "access_level": "Tagging",
             "action": "CreateTags",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AccepterVpc",
                 "ec2:AllocationId",
-                "ec2:AssociatePublicIpAddress",
                 "ec2:AuthenticationType",
-                "ec2:AuthorizedService",
                 "ec2:AuthorizedUser",
                 "ec2:AutoPlacement",
                 "ec2:AvailabilityZone",
                 "ec2:ClientRootCertificateChainArn",
                 "ec2:CloudwatchLogGroupArn",
                 "ec2:CloudwatchLogStreamArn",
                 "ec2:CreateAction",
                 "ec2:DPDTimeoutSeconds",
                 "ec2:DhcpOptionsID",
                 "ec2:DirectoryArn",
                 "ec2:Domain",
-                "ec2:DomainCertificateArn",
                 "ec2:EbsOptimized",
                 "ec2:ElasticGpuType",
                 "ec2:Encrypted",
                 "ec2:GatewayType",
                 "ec2:HostRecovery",
                 "ec2:IKEVersions",
                 "ec2:ImageID",
@@ -43814,15 +43854,14 @@
                 "ec2:InstanceMarketType",
                 "ec2:InstanceMetadataTags",
                 "ec2:InstanceProfile",
                 "ec2:InstanceType",
                 "ec2:InternetGatewayID",
                 "ec2:KeyPairName",
                 "ec2:KeyPairType",
-                "ec2:LoadBalancerArn",
                 "ec2:MetadataHttpEndpoint",
                 "ec2:MetadataHttpPutResponseHopLimit",
                 "ec2:MetadataHttpTokens",
                 "ec2:NetworkAclID",
                 "ec2:NetworkInterfaceID",
                 "ec2:Owner",
                 "ec2:ParentSnapshot",
@@ -43865,16 +43904,15 @@
                 "ec2:VolumeID",
                 "ec2:VolumeIops",
                 "ec2:VolumeSize",
                 "ec2:VolumeThroughput",
                 "ec2:VolumeType",
                 "ec2:Vpc",
                 "ec2:VpcID",
-                "ec2:VpcPeeringConnectionID",
-                "ec2:VpceServicePrivateDnsName"
+                "ec2:VpcPeeringConnectionID"
             ],
             "description": "Grants permission to add or overwrite one or more tags for Amazon EC2 resources",
             "orphan": false,
             "resources": [
                 "capacity-reservation",
                 "capacity-reservation-fleet",
                 "carrier-gateway",
@@ -44216,20 +44254,16 @@
         "CreateVerifiedAccessEndpoint": {
             "access_level": "Write",
             "action": "CreateVerifiedAccessEndpoint",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AuthorizedUser",
                 "ec2:AvailabilityZone",
-                "ec2:DomainCertificateArn",
-                "ec2:LoadBalancerArn",
                 "ec2:NetworkInterfaceID",
                 "ec2:Permission",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SecurityGroupID",
                 "ec2:Subnet",
                 "ec2:SubnetID",
@@ -44367,15 +44401,16 @@
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to create a connection notification for a VPC endpoint or VPC endpoint service",
             "orphan": false,
             "resources": [
-                "vpc-endpoint"
+                "vpc-endpoint",
+                "vpc-endpoint-service"
             ]
         },
         "CreateVpcEndpointServiceConfiguration": {
             "access_level": "Write",
             "action": "CreateVpcEndpointServiceConfiguration",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -45000,16 +45035,14 @@
             ]
         },
         "DeleteNetworkInterfacePermission": {
             "access_level": "Permissions management",
             "action": "DeleteNetworkInterfacePermission",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
                 "ec2:Vpc"
             ],
@@ -45133,15 +45166,14 @@
                 "ec2:OutpostArn",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
                 "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
                 "ec2:VolumeSize"
             ],
             "description": "Grants permission to delete a snapshot of an EBS volume",
             "orphan": false,
             "resources": [
                 "snapshot"
             ]
@@ -45491,16 +45523,14 @@
             ]
         },
         "DeleteVerifiedAccessEndpoint": {
             "access_level": "Write",
             "action": "DeleteVerifiedAccessEndpoint",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:DomainCertificateArn",
-                "ec2:LoadBalancerArn",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to delete a Verified Access endpoint",
             "orphan": false,
             "resources": [
                 "verified-access-endpoint"
@@ -46856,15 +46886,14 @@
             "resources": []
         },
         "DescribeSnapshotAttribute": {
             "access_level": "List",
             "action": "DescribeSnapshotAttribute",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
                 "ec2:Encrypted",
                 "ec2:OutpostArn",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
@@ -47173,18 +47202,20 @@
                 "ec2:Region"
             ],
             "description": "Grants permission to describe the current logging configuration for the Verified Access instances",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstanceWebAclAssociations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "DescribeVerifiedAccessInstanceWebAclAssociations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "ec2:Region"
+            ],
+            "description": "Grants permission to describe the AWS Web Application Firewall (WAF) web access control list (ACL) associations for a Verified Access instance",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstances": {
             "access_level": "List",
             "action": "DescribeVerifiedAccessInstances",
             "condition_keys": [
@@ -47322,19 +47353,23 @@
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointServicePermissions": {
             "access_level": "List",
             "action": "DescribeVpcEndpointServicePermissions",
             "condition_keys": [
-                "ec2:Region"
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to describe the principals (service consumers) that are permitted to discover your VPC endpoint service",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-endpoint-service"
+            ]
         },
         "DescribeVpcEndpointServices": {
             "access_level": "List",
             "action": "DescribeVpcEndpointServices",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -47833,16 +47868,14 @@
         },
         "DisassociateNatGatewayAddress": {
             "access_level": "Write",
             "action": "DisassociateNatGatewayAddress",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AllocationId",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AuthorizedUser",
                 "ec2:AvailabilityZone",
                 "ec2:Domain",
                 "ec2:NetworkInterfaceID",
                 "ec2:Permission",
                 "ec2:PublicIpAddress",
                 "ec2:Region",
@@ -47955,20 +47988,26 @@
                 "ec2:Region"
             ],
             "description": "Grants permission to disassociate a branch network interface to a trunk network interface",
             "orphan": false,
             "resources": []
         },
         "DisassociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to disassociate an AWS Web Application Firewall (WAF) web access control list (ACL) from a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "DisassociateVpcCidrBlock": {
             "access_level": "Write",
             "action": "DisassociateVpcCidrBlock",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
@@ -48829,16 +48868,14 @@
             "resources": []
         },
         "GetVerifiedAccessEndpointPolicy": {
             "access_level": "List",
             "action": "GetVerifiedAccessEndpointPolicy",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:DomainCertificateArn",
-                "ec2:LoadBalancerArn",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to show the Verified Access policy associated with the endpoint",
             "orphan": false,
             "resources": [
                 "verified-access-endpoint"
@@ -48855,20 +48892,26 @@
             "description": "Grants permission to show the contents of the Verified Access policy associated with the group",
             "orphan": false,
             "resources": [
                 "verified-access-group"
             ]
         },
         "GetVerifiedAccessInstanceWebAcl": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVerifiedAccessInstanceWebAcl",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to show the AWS Web Application Firewall (WAF) web access control list (ACL) for a Verified Access instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "verified-access-instance"
+            ]
         },
         "GetVpnConnectionDeviceSampleConfiguration": {
             "access_level": "List",
             "action": "GetVpnConnectionDeviceSampleConfiguration",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
@@ -48888,28 +48931,40 @@
                 "ec2:Region"
             ],
             "description": "Grants permission to obtain a list of customer gateway devices for which sample configuration files can be provided",
             "orphan": false,
             "resources": []
         },
         "GetVpnTunnelReplacementStatus": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "GetVpnTunnelReplacementStatus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to view available tunnel endpoint maintenance events",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ImportByoipCidrToIpam": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportByoipCidrToIpam",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to transfer existing BYOIP IPv4 CIDRs to IPAM",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ipam-pool"
+            ]
         },
         "ImportClientVpnClientCertificateRevocationList": {
             "access_level": "Write",
             "action": "ImportClientVpnClientCertificateRevocationList",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:ClientRootCertificateChainArn",
@@ -49059,15 +49114,14 @@
             ]
         },
         "ListSnapshotsInRecycleBin": {
             "access_level": "List",
             "action": "ListSnapshotsInRecycleBin",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
                 "ec2:Encrypted",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
                 "ec2:SnapshotTime",
@@ -49188,18 +49242,16 @@
             "resources": []
         },
         "ModifyFleet": {
             "access_level": "Write",
             "action": "ModifyFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AssociatePublicIpAddress",
                 "ec2:Attribute",
                 "ec2:Attribute/${AttributeName}",
-                "ec2:AuthorizedService",
                 "ec2:AvailabilityZone",
                 "ec2:ImageID",
                 "ec2:ImageType",
                 "ec2:KeyPairName",
                 "ec2:NetworkInterfaceID",
                 "ec2:Owner",
                 "ec2:ParentVolume",
@@ -49630,16 +49682,14 @@
             ]
         },
         "ModifyLocalGatewayRoute": {
             "access_level": "Write",
             "action": "ModifyLocalGatewayRoute",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AuthorizedUser",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Permission",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
@@ -49807,15 +49857,14 @@
         "ModifySnapshotTier": {
             "access_level": "Write",
             "action": "ModifySnapshotTier",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Attribute",
                 "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
                 "ec2:Encrypted",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
                 "ec2:SnapshotTime",
@@ -49973,16 +50022,14 @@
         },
         "ModifyVerifiedAccessEndpoint": {
             "access_level": "Write",
             "action": "ModifyVerifiedAccessEndpoint",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
-                "ec2:DomainCertificateArn",
-                "ec2:LoadBalancerArn",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SubnetID",
                 "ec2:Vpc"
             ],
             "description": "Grants permission to modify the configuration of a Verified Access endpoint",
             "orphan": false,
@@ -49993,16 +50040,14 @@
             ]
         },
         "ModifyVerifiedAccessEndpointPolicy": {
             "access_level": "Write",
             "action": "ModifyVerifiedAccessEndpointPolicy",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:DomainCertificateArn",
-                "ec2:LoadBalancerArn",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to modify the specified Verified Access endpoint policy",
             "orphan": false,
             "resources": [
                 "verified-access-endpoint"
@@ -50851,23 +50896,25 @@
         },
         "ReplaceRouteTableAssociation": {
             "access_level": "Write",
             "action": "ReplaceRouteTableAssociation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
+                "ec2:InternetGatewayID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:RouteTableID",
                 "ec2:SubnetID",
                 "ec2:Vpc"
             ],
             "description": "Grants permission to change the route table that is associated with a subnet",
             "orphan": false,
             "resources": [
+                "internet-gateway",
                 "ipv4pool-ec2",
                 "ipv6pool-ec2",
                 "route-table",
                 "subnet"
             ]
         },
         "ReplaceTransitGatewayRoute": {
@@ -50882,20 +50929,26 @@
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
         },
         "ReplaceVpnTunnel": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReplaceVpnTunnel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}"
+            ],
+            "description": "Grants permission to replace a VPN tunnel",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpn-connection"
+            ]
         },
         "ReportInstanceStatus": {
             "access_level": "Write",
             "action": "ReportInstanceStatus",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -50946,16 +50999,14 @@
         "RequestSpotInstances": {
             "access_level": "Write",
             "action": "RequestSpotInstances",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
                 "ec2:AuthorizedUser",
                 "ec2:AvailabilityZone",
                 "ec2:ImageID",
                 "ec2:ImageType",
                 "ec2:KeyPairName",
                 "ec2:KeyPairType",
                 "ec2:NetworkInterfaceID",
@@ -51168,15 +51219,14 @@
             ]
         },
         "RestoreSnapshotFromRecycleBin": {
             "access_level": "Write",
             "action": "RestoreSnapshotFromRecycleBin",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
                 "ec2:Encrypted",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
                 "ec2:SnapshotTime",
@@ -51189,15 +51239,14 @@
             ]
         },
         "RestoreSnapshotTier": {
             "access_level": "Write",
             "action": "RestoreSnapshotTier",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
                 "ec2:Encrypted",
                 "ec2:Owner",
                 "ec2:ParentVolume",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SnapshotID",
                 "ec2:SnapshotTime",
@@ -65722,15 +65771,17 @@
         },
         "BatchGetCustomEntityTypes": {
             "access_level": "Read",
             "action": "BatchGetCustomEntityTypes",
             "condition_keys": [],
             "description": "Grants permission to retrieve one or more Custom Entity Types",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "customEntityType"
+            ]
         },
         "BatchGetDevEndpoints": {
             "access_level": "Read",
             "action": "BatchGetDevEndpoints",
             "condition_keys": [],
             "description": "Grants permission to retrieve one or more development endpoints",
             "orphan": false,
@@ -65894,15 +65945,18 @@
             "description": "Grants permission to create a crawler",
             "orphan": false,
             "resources": []
         },
         "CreateCustomEntityType": {
             "access_level": "Write",
             "action": "CreateCustomEntityType",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to create a Custom Entity Type",
             "orphan": false,
             "resources": []
         },
         "CreateDataQualityRuleset": {
             "access_level": "Write",
             "action": "CreateDataQualityRuleset",
@@ -66154,15 +66208,17 @@
         },
         "DeleteCustomEntityType": {
             "access_level": "Write",
             "action": "DeleteCustomEntityType",
             "condition_keys": [],
             "description": "Grants permission to delete a Custom Entity Type",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "customEntityType"
+            ]
         },
         "DeleteDataQualityRuleset": {
             "access_level": "Write",
             "action": "DeleteDataQualityRuleset",
             "condition_keys": [],
             "description": "Grants permission to delete a Data Quality ruleset",
             "orphan": false,
@@ -66491,15 +66547,17 @@
         },
         "GetCustomEntityType": {
             "access_level": "Read",
             "action": "GetCustomEntityType",
             "condition_keys": [],
             "description": "Grants permission to read a Custom Entity Type",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "customEntityType"
+            ]
         },
         "GetDataCatalogEncryptionSettings": {
             "access_level": "Read",
             "action": "GetDataCatalogEncryptionSettings",
             "condition_keys": [],
             "description": "Grants permission to retrieve catalog encryption settings",
             "orphan": false,
@@ -66912,14 +66970,15 @@
             "action": "GetTags",
             "condition_keys": [],
             "description": "Grants permission to retrieve all tags associated with a resource",
             "orphan": false,
             "resources": [
                 "blueprint",
                 "crawler",
+                "customEntityType",
                 "devendpoint",
                 "job",
                 "trigger",
                 "workflow"
             ]
         },
         "GetTrigger": {
@@ -67053,15 +67112,18 @@
             "description": "Grants permission to retrieve crawl run history for a crawler",
             "orphan": false,
             "resources": []
         },
         "ListCustomEntityTypes": {
             "access_level": "List",
             "action": "ListCustomEntityTypes",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to retrieve all Custom Entity Types",
             "orphan": false,
             "resources": []
         },
         "ListDataQualityResults": {
             "access_level": "List",
             "action": "ListDataQualityResults",
@@ -67522,14 +67584,15 @@
             ],
             "description": "Grants permission to add tags to a resource",
             "orphan": false,
             "resources": [
                 "blueprint",
                 "connection",
                 "crawler",
+                "customEntityType",
                 "dataQualityRuleset",
                 "devendpoint",
                 "job",
                 "mlTransform",
                 "registry",
                 "schema",
                 "session",
@@ -67554,14 +67617,15 @@
             ],
             "description": "Grants permission to remove tags associated with a resource",
             "orphan": false,
             "resources": [
                 "blueprint",
                 "connection",
                 "crawler",
+                "customEntityType",
                 "dataQualityRuleset",
                 "devendpoint",
                 "job",
                 "mlTransform",
                 "registry",
                 "schema",
                 "session",
@@ -147452,14 +147516,15 @@
             "orphan": false,
             "resources": [
                 "apigateway",
                 "apprunner",
                 "appsync",
                 "loadbalancer/app/",
                 "userpool",
+                "verified-access-instance",
                 "webacl"
             ]
         },
         "CheckCapacity": {
             "access_level": "Read",
             "action": "CheckCapacity",
             "condition_keys": [],
@@ -147628,15 +147693,16 @@
             "description": "Grants permission to disassociate a WebACL from an application resource",
             "orphan": false,
             "resources": [
                 "apigateway",
                 "apprunner",
                 "appsync",
                 "loadbalancer/app/",
-                "userpool"
+                "userpool",
+                "verified-access-instance"
             ]
         },
         "GenerateMobileSdkReleaseUrl": {
             "access_level": "Read",
             "action": "GenerateMobileSdkReleaseUrl",
             "condition_keys": [],
             "description": "Grants permission to generate a presigned download URL for the specified release of the mobile SDK",
@@ -147768,15 +147834,16 @@
             "description": "Grants permission to retrieve the WebACL that's associated with a resource",
             "orphan": false,
             "resources": [
                 "apigateway",
                 "apprunner",
                 "appsync",
                 "loadbalancer/app/",
-                "userpool"
+                "userpool",
+                "verified-access-instance"
             ]
         },
         "ListAPIKeys": {
             "access_level": "List",
             "action": "ListAPIKeys",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of the API keys that you've defined for the specified scope",
```

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230519/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230519/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/generate.py` & `iam_actions-1.2.20230519/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230519/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230519/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/generate/services.py` & `iam_actions-1.2.20230519/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230518/iam_actions/policies.json` & `iam_actions-1.2.20230519/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997215688371%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(23, 'CreatePrompt'), (43, "*

 * *                 "'DeletePrompt'), (65, 'DescribePrompt'), (94, 'GetPromptFile'), (176, "*

 * *                 "'UpdatePrompt')]}}}"}*

```diff
@@ -11254,14 +11254,15 @@
                 "CreateContactFlow",
                 "CreateContactFlowModule",
                 "CreateEvaluationForm",
                 "CreateHoursOfOperation",
                 "CreateInstance",
                 "CreateIntegrationAssociation",
                 "CreateParticipant",
+                "CreatePrompt",
                 "CreateQueue",
                 "CreateQuickConnect",
                 "CreateRoutingProfile",
                 "CreateRule",
                 "CreateSecurityProfile",
                 "CreateTaskTemplate",
                 "CreateTrafficDistributionGroup",
@@ -11273,14 +11274,15 @@
                 "DeleteContactEvaluation",
                 "DeleteContactFlow",
                 "DeleteContactFlowModule",
                 "DeleteEvaluationForm",
                 "DeleteHoursOfOperation",
                 "DeleteInstance",
                 "DeleteIntegrationAssociation",
+                "DeletePrompt",
                 "DeleteQuickConnect",
                 "DeleteRule",
                 "DeleteSecurityProfile",
                 "DeleteTaskTemplate",
                 "DeleteTrafficDistributionGroup",
                 "DeleteUseCase",
                 "DeleteUser",
@@ -11294,14 +11296,15 @@
                 "DescribeEvaluationForm",
                 "DescribeForecastingPlanningSchedulingIntegration",
                 "DescribeHoursOfOperation",
                 "DescribeInstance",
                 "DescribeInstanceAttribute",
                 "DescribeInstanceStorageConfig",
                 "DescribePhoneNumber",
+                "DescribePrompt",
                 "DescribeQueue",
                 "DescribeQuickConnect",
                 "DescribeRoutingProfile",
                 "DescribeRule",
                 "DescribeSecurityProfile",
                 "DescribeTrafficDistributionGroup",
                 "DescribeUser",
@@ -11322,14 +11325,15 @@
                 "GetContactAttributes",
                 "GetCurrentMetricData",
                 "GetCurrentUserData",
                 "GetFederationToken",
                 "GetFederationTokens",
                 "GetMetricData",
                 "GetMetricDataV2",
+                "GetPromptFile",
                 "GetTaskTemplate",
                 "GetTrafficDistribution",
                 "ListAgentStatuses",
                 "ListApprovedOrigins",
                 "ListBots",
                 "ListContactEvaluations",
                 "ListContactFlowModules",
@@ -11403,14 +11407,15 @@
                 "UpdateContactSchedule",
                 "UpdateEvaluationForm",
                 "UpdateHoursOfOperation",
                 "UpdateInstanceAttribute",
                 "UpdateInstanceStorageConfig",
                 "UpdateParticipantRoleConfig",
                 "UpdatePhoneNumber",
+                "UpdatePrompt",
                 "UpdateQueueHoursOfOperation",
                 "UpdateQueueMaxContacts",
                 "UpdateQueueName",
                 "UpdateQueueOutboundCallerConfig",
                 "UpdateQueueStatus",
                 "UpdateQuickConnectConfig",
                 "UpdateQuickConnectName",
```

### Comparing `iam_actions-1.2.20230518/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230519/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997089628879322%*

 * *Differences: {"'glue'": "{'customEntityType': OrderedDict([('arn_pattern', "*

 * *           "'arn:*:glue:*:*:customEntityType/*'), ('condition_keys', "*

 * *           "'aws:ResourceTag/${TagKey}')])}",*

 * * "'outposts'": "{'outpost': {'arn_pattern': 'arn:*:outposts:*:*:outpost/*'}}",*

 * * "'wafv2'": "{'verified-access-instance': OrderedDict([('arn_pattern', "*

 * *            "'arn:*:ec2:*:*:verified-access-instance/*'), ('condition_keys', None)])}"}*

```diff
@@ -2889,14 +2889,18 @@
             "arn_pattern": "arn:*:glue:*:*:connection/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "crawler": {
             "arn_pattern": "arn:*:glue:*:*:crawler/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "customEntityType": {
+            "arn_pattern": "arn:*:glue:*:*:customEntityType/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "dataQualityRuleset": {
             "arn_pattern": "arn:*:glue:*:*:dataQualityRuleset/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "database": {
             "arn_pattern": "arn:*:glue:*:*:database/*",
             "condition_keys": null
@@ -4638,15 +4642,15 @@
             "arn_pattern": "arn:*:organizations::*:root/o-*/r-*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "osis": {},
     "outposts": {
         "outpost": {
-            "arn_pattern": "arn:*:outposts:*:*:outpost:*",
+            "arn_pattern": "arn:*:outposts:*:*:outpost/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "site": {
             "arn_pattern": "arn:*:outposts:*:*:site/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
@@ -6467,14 +6471,18 @@
             "arn_pattern": "arn:*:wafv2:*:*:*/rulegroup/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "userpool": {
             "arn_pattern": "arn:*:cognito-idp:*:*:userpool/*",
             "condition_keys": null
         },
+        "verified-access-instance": {
+            "arn_pattern": "arn:*:ec2:*:*:verified-access-instance/*",
+            "condition_keys": null
+        },
         "webacl": {
             "arn_pattern": "arn:*:wafv2:*:*:*/webacl/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "wam": {},
     "wellarchitected": {
```

### Comparing `iam_actions-1.2.20230518/iam_actions/services.json` & `iam_actions-1.2.20230519/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999997083840745%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(23, 'CreatePrompt'), (43, 'DeletePrompt'), (65, "*

 * *              "'DescribePrompt'), (94, 'GetPromptFile'), (176, 'UpdatePrompt')]}}"}*

```diff
@@ -4540,14 +4540,15 @@
             "CreateContactFlow",
             "CreateContactFlowModule",
             "CreateEvaluationForm",
             "CreateHoursOfOperation",
             "CreateInstance",
             "CreateIntegrationAssociation",
             "CreateParticipant",
+            "CreatePrompt",
             "CreateQueue",
             "CreateQuickConnect",
             "CreateRoutingProfile",
             "CreateRule",
             "CreateSecurityProfile",
             "CreateTaskTemplate",
             "CreateTrafficDistributionGroup",
@@ -4559,14 +4560,15 @@
             "DeleteContactEvaluation",
             "DeleteContactFlow",
             "DeleteContactFlowModule",
             "DeleteEvaluationForm",
             "DeleteHoursOfOperation",
             "DeleteInstance",
             "DeleteIntegrationAssociation",
+            "DeletePrompt",
             "DeleteQuickConnect",
             "DeleteRule",
             "DeleteSecurityProfile",
             "DeleteTaskTemplate",
             "DeleteTrafficDistributionGroup",
             "DeleteUseCase",
             "DeleteUser",
@@ -4580,14 +4582,15 @@
             "DescribeEvaluationForm",
             "DescribeForecastingPlanningSchedulingIntegration",
             "DescribeHoursOfOperation",
             "DescribeInstance",
             "DescribeInstanceAttribute",
             "DescribeInstanceStorageConfig",
             "DescribePhoneNumber",
+            "DescribePrompt",
             "DescribeQueue",
             "DescribeQuickConnect",
             "DescribeRoutingProfile",
             "DescribeRule",
             "DescribeSecurityProfile",
             "DescribeTrafficDistributionGroup",
             "DescribeUser",
@@ -4608,14 +4611,15 @@
             "GetContactAttributes",
             "GetCurrentMetricData",
             "GetCurrentUserData",
             "GetFederationToken",
             "GetFederationTokens",
             "GetMetricData",
             "GetMetricDataV2",
+            "GetPromptFile",
             "GetTaskTemplate",
             "GetTrafficDistribution",
             "ListAgentStatuses",
             "ListApprovedOrigins",
             "ListBots",
             "ListContactEvaluations",
             "ListContactFlowModules",
@@ -4689,14 +4693,15 @@
             "UpdateContactSchedule",
             "UpdateEvaluationForm",
             "UpdateHoursOfOperation",
             "UpdateInstanceAttribute",
             "UpdateInstanceStorageConfig",
             "UpdateParticipantRoleConfig",
             "UpdatePhoneNumber",
+            "UpdatePrompt",
             "UpdateQueueHoursOfOperation",
             "UpdateQueueMaxContacts",
             "UpdateQueueName",
             "UpdateQueueOutboundCallerConfig",
             "UpdateQueueStatus",
             "UpdateQuickConnectConfig",
             "UpdateQuickConnectName",
```

### Comparing `iam_actions-1.2.20230518/pyproject.toml` & `iam_actions-1.2.20230519/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230518"
+version = "1.2.20230519"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230518/setup.py` & `iam_actions-1.2.20230519/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230518',
+    'version': '1.2.20230519',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230518/PKG-INFO` & `iam_actions-1.2.20230519/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230518
+Version: 1.2.20230519
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

