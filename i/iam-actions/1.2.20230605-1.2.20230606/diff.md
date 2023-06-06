# Comparing `tmp/iam_actions-1.2.20230605.tar.gz` & `tmp/iam_actions-1.2.20230606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230605.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230606.tar", max compression
```

## Comparing `iam_actions-1.2.20230605.tar` & `iam_actions-1.2.20230606.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/README.md
--rw-r--r--   0        0        0      228 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/__init__.py
--rw-r--r--   0        0        0  4284913 2023-06-05 02:46:50.604674 iam_actions-1.2.20230605/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-05 02:45:30.746647 iam_actions-1.2.20230605/iam_actions/generate/services.py
--rw-r--r--   0        0        0   551159 2023-06-05 02:46:50.608674 iam_actions-1.2.20230605/iam_actions/policies.json
--rw-r--r--   0        0        0   195776 2023-06-05 02:46:50.608674 iam_actions-1.2.20230605/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   534622 2023-06-05 02:46:50.608674 iam_actions-1.2.20230605/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-05 02:46:51.556745 iam_actions-1.2.20230605/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230605/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230605/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/README.md
+-rw-r--r--   0        0        0      228 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4148664 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-06 02:50:17.229081 iam_actions-1.2.20230606/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   551306 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/policies.json
+-rw-r--r--   0        0        0   183844 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   534766 2023-06-06 02:51:34.434502 iam_actions-1.2.20230606/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-06 02:51:35.338519 iam_actions-1.2.20230606/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230606/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230606/PKG-INFO
```

### Comparing `iam_actions-1.2.20230605/LICENSE` & `iam_actions-1.2.20230606/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/README.md` & `iam_actions-1.2.20230606/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/actions.json` & `iam_actions-1.2.20230606/iam_actions/actions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999726504452693%*

 * *Differences: {"'athena'": "{'DeleteCapacityReservation': {'access_level': 'Write', 'description': 'Grants "*

 * *             "permission to delete a capacity reservation', 'resources': "*

 * *             "['capacity-reservation']}}",*

 * * "'cloudtrail'": "{'StopEventDataStoreIngestion': {'access_level': 'Write', 'description': 'Grants "*

 * *                 "permission to stop ingestion on an event data store', 'resources': "*

 * *                 "['eventdatastore']}, 'StartEventDataStoreIngestion': {'access_level': 'Write', "*

 * *             […]*

```diff
@@ -8190,20 +8190,22 @@
             "description": "Grants permission to create a workgroup",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
         "DeleteCapacityReservation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCapacityReservation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a capacity reservation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "capacity-reservation"
+            ]
         },
         "DeleteDataCatalog": {
             "access_level": "Write",
             "action": "DeleteDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to delete a datacatalog",
             "orphan": false,
@@ -21499,20 +21501,22 @@
             "description": "Grants permission to restore an event data store",
             "orphan": false,
             "resources": [
                 "eventdatastore"
             ]
         },
         "StartEventDataStoreIngestion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartEventDataStoreIngestion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start ingestion on an event data store",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "eventdatastore"
+            ]
         },
         "StartImport": {
             "access_level": "Write",
             "action": "StartImport",
             "condition_keys": [],
             "description": "Grants permission to start an import of logged trail events from a source S3 bucket to a destination event data store",
             "orphan": false,
@@ -21535,20 +21539,22 @@
             "description": "Grants permission to start a new query on a specified event data store",
             "orphan": false,
             "resources": [
                 "eventdatastore"
             ]
         },
         "StopEventDataStoreIngestion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopEventDataStoreIngestion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to stop ingestion on an event data store",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "eventdatastore"
+            ]
         },
         "StopImport": {
             "access_level": "Write",
             "action": "StopImport",
             "condition_keys": [],
             "description": "Grants permission to stop a specified import",
             "orphan": false,
@@ -23874,14 +23880,15 @@
                 "repository"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to disassociate resource tags from a CodeCommit resource ARN",
             "orphan": false,
             "resources": [
                 "repository"
             ]
@@ -42363,9941 +42370,4858 @@
             "resources": [
                 "snapshot"
             ]
         }
     },
     "ec2": {
         "AcceptAddressTransfer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptAddressTransfer",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to accept an Elastic IP address transfer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "AcceptReservedInstancesExchangeQuote": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptReservedInstancesExchangeQuote",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to accept a Convertible Reserved Instance exchange quote",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AcceptTransitGatewayMulticastDomainAssociations": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to accept a request to associate subnets with a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "AcceptTransitGatewayPeeringAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptTransitGatewayPeeringAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to accept a transit gateway peering attachment request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "AcceptTransitGatewayVpcAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptTransitGatewayVpcAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to accept a request to attach a VPC to a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "AcceptVpcEndpointConnections": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptVpcEndpointConnections",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to accept one or more interface VPC endpoint connections to your VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "AcceptVpcPeeringConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptVpcPeeringConnection",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AccepterVpc",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to accept a VPC peering connection request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc",
-                "vpc-peering-connection"
-            ]
+            "resources": []
         },
         "AdvertiseByoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AdvertiseByoipCidr",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to advertise an IP address range that is provisioned for use in AWS through bring your own IP addresses (BYOIP)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AllocateAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AllocateAddress",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to allocate an Elastic IP address (EIP) to your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "ipv4pool-ec2"
-            ]
+            "resources": []
         },
         "AllocateHosts": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AllocateHosts",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AutoPlacement",
-                "ec2:AvailabilityZone",
-                "ec2:HostRecovery",
-                "ec2:InstanceType",
-                "ec2:Quantity",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to allocate a Dedicated Host to your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dedicated-host"
-            ]
+            "resources": []
         },
         "AllocateIpamPoolCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AllocateIpamPoolCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to allocate a CIDR from an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "ApplySecurityGroupsToClientVpnTargetNetwork": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ApplySecurityGroupsToClientVpnTargetNetwork",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:SecurityGroupID",
-                "ec2:ServerCertificateArn",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to apply a security group to the association between a Client VPN endpoint and a target network",
-            "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "security-group",
-                "vpc"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "AssignIpv6Addresses": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssignIpv6Addresses",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to assign one or more IPv6 addresses to a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "AssignPrivateIpAddresses": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssignPrivateIpAddresses",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to assign one or more secondary private IP addresses to a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "AssignPrivateNatGatewayAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssignPrivateNatGatewayAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to assign one or more secondary private IP addresses to a private NAT gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "natgateway"
-            ]
+            "resources": []
         },
         "AssociateAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:AvailabilityZone",
-                "ec2:Domain",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkInterfaceID",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Subnet",
-                "ec2:Tenancy",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to associate an Elastic IP address (EIP) with an instance or a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "instance",
-                "network-interface"
-            ]
+            "resources": []
         },
         "AssociateClientVpnTargetNetwork": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateClientVpnTargetNetwork",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn",
-                "ec2:SubnetID"
-            ],
-            "description": "Grants permission to associate a target network with a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "subnet"
-            ]
+            "resources": []
         },
         "AssociateDhcpOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateDhcpOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:DhcpOptionsID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to associate or disassociate a set of DHCP options with a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dhcp-options",
-                "vpc"
-            ]
+            "resources": []
         },
         "AssociateEnclaveCertificateIamRole": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateEnclaveCertificateIamRole",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to associate an ACM certificate with an IAM role to be used in an EC2 Enclave",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "certificate",
-                "role"
-            ]
+            "resources": []
         },
         "AssociateIamInstanceProfile": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateIamInstanceProfile",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NewInstanceProfile",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to associate an IAM instance profile with a running or stopped instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "AssociateInstanceEventWindow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateInstanceEventWindow",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate one or more targets with an event window",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance-event-window"
-            ]
+            "resources": []
         },
         "AssociateIpamResourceDiscovery": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateIpamResourceDiscovery",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate an IPAM resource discovery with an Amazon VPC IPAM",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam",
-                "ipam-resource-discovery",
-                "ipam-resource-discovery-association"
-            ]
+            "resources": []
         },
         "AssociateNatGatewayAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateNatGatewayAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate an Elastic IP address and private IP address with a public Nat gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "natgateway"
-            ]
+            "resources": []
         },
         "AssociateRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to associate a subnet or gateway with a route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "internet-gateway",
-                "route-table",
-                "subnet",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "AssociateSubnetCidrBlock": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateSubnetCidrBlock",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to associate a CIDR block with a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet"
-            ]
+            "resources": []
         },
         "AssociateTransitGatewayMulticastDomain": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateTransitGatewayMulticastDomain",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to associate an attachment and list of subnets with a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "transit-gateway-attachment",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "AssociateTransitGatewayPolicyTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateTransitGatewayPolicyTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate a policy table with a transit gateway attachment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "AssociateTransitGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateTransitGatewayRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate an attachment with a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "AssociateTrunkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateTrunkInterface",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to associate a branch network interface with a trunk network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AssociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to associate an AWS Web Application Firewall (WAF) web access control list (ACL) with a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "AssociateVpcCidrBlock": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateVpcCidrBlock",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Ipv4IpamPoolId",
-                "ec2:Ipv6IpamPoolId",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to associate a CIDR block with a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "ipv6pool-ec2",
-                "vpc"
-            ]
+            "resources": []
         },
         "AttachClassicLinkVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachClassicLinkVpc",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:Tenancy",
-                "ec2:Vpc",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to link an EC2-Classic instance to a ClassicLink-enabled VPC through one or more of the VPC's security groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "security-group",
-                "vpc"
-            ]
+            "resources": []
         },
         "AttachInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachInternetGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to attach an internet gateway to a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "internet-gateway",
-                "vpc"
-            ]
+            "resources": []
         },
         "AttachNetworkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachNetworkInterface",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkInterfaceID",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Subnet",
-                "ec2:Tenancy",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to attach a network interface to an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "network-interface"
-            ]
+            "resources": []
         },
         "AttachVerifiedAccessTrustProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachVerifiedAccessTrustProvider",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to attach a trust provider to a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance",
-                "verified-access-trust-provider"
-            ]
+            "resources": []
         },
         "AttachVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachVolume",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ParentSnapshot",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to attach an EBS volume to a running or stopped instance and expose it to the instance with the specified device name",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "volume"
-            ]
+            "resources": []
         },
         "AttachVpnGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AttachVpnGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to attach a virtual private gateway to a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "AuthorizeClientVpnIngress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AuthorizeClientVpnIngress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to add an inbound authorization rule to a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "AuthorizeSecurityGroupEgress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AuthorizeSecurityGroupEgress",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to add one or more outbound rules to a VPC security group. Policies using the security-group-rule resource-level permission are only enforced when the API request includes TagSpecifications",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group",
-                "security-group-rule"
-            ]
+            "resources": []
         },
         "AuthorizeSecurityGroupIngress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AuthorizeSecurityGroupIngress",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to add one or more inbound rules to a VPC security group. Policies using the security-group-rule resource-level permission are only enforced when the API request includes TagSpecifications",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group",
-                "security-group-rule"
-            ]
+            "resources": []
         },
         "BundleInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "BundleInstance",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to bundle an instance store-backed Windows instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CancelBundleTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelBundleTask",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to cancel a bundling operation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CancelCapacityReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelCapacityReservation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:CapacityReservationFleet",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel a Capacity Reservation and release the reserved capacity",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation"
-            ]
+            "resources": []
         },
         "CancelCapacityReservationFleets": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelCapacityReservationFleets",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel one or more Capacity Reservation Fleets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation-fleet"
-            ]
+            "resources": []
         },
         "CancelConversionTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelConversionTask",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to cancel an active conversion task",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CancelExportTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelExportTask",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel an active export task",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "export-image-task",
-                "export-instance-task"
-            ]
+            "resources": []
         },
         "CancelImageLaunchPermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelImageLaunchPermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to remove your AWS account from the launch permissions for the specified AMI",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "CancelImportTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelImportTask",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel an in-process import virtual machine or import snapshot task",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "import-image-task",
-                "import-snapshot-task"
-            ]
+            "resources": []
         },
         "CancelReservedInstancesListing": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelReservedInstancesListing",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to cancel a Reserved Instance listing on the Reserved Instance Marketplace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CancelSpotFleetRequests": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelSpotFleetRequests",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel one or more Spot Fleet requests",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "spot-fleet-request"
-            ]
+            "resources": []
         },
         "CancelSpotInstanceRequests": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CancelSpotInstanceRequests",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to cancel one or more Spot Instance requests",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "spot-instances-request"
-            ]
+            "resources": []
         },
         "ConfirmProductInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ConfirmProductInstance",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to determine whether an owned product code is associated with an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CopyFpgaImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CopyFpgaImage",
-            "condition_keys": [
-                "ec2:Owner",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to copy a source Amazon FPGA image (AFI) to the current Region. Resource-level permissions specified for this action apply to the new AFI only. They do not apply to the source AFI",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "CopyImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CopyImage",
-            "condition_keys": [
-                "ec2:ImageID",
-                "ec2:Owner",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to copy an Amazon Machine Image (AMI) from a source Region to the current Region. Resource-level permissions specified for this action apply to the new AMI only. They do not apply to the source AMI",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "CopySnapshot": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CopySnapshot",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:OutpostArn",
-                "ec2:Region",
-                "ec2:SnapshotID"
-            ],
-            "description": "Grants permission to copy a point-in-time snapshot of an EBS volume and store it in Amazon S3. Resource-level permissions specified for this action apply to the new snapshot only. They do not apply to the source snapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "CreateCapacityReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCapacityReservation",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:CapacityReservationFleet",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a Capacity Reservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation"
-            ]
+            "resources": []
         },
         "CreateCapacityReservationFleet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCapacityReservationFleet",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a Capacity Reservation Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation-fleet"
-            ]
+            "resources": []
         },
         "CreateCarrierGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCarrierGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a carrier gateway and provides CSP connectivity to VPC customers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "carrier-gateway",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateClientVpnEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateClientVpnEndpoint",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:SecurityGroupID",
-                "ec2:ServerCertificateArn",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a Client VPN endpoint",
-            "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "security-group",
-                "vpc"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "CreateClientVpnRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateClientVpnRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn",
-                "ec2:SubnetID"
-            ],
-            "description": "Grants permission to add a network route to a Client VPN endpoint's route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "subnet"
-            ]
+            "resources": []
         },
         "CreateCoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCoipCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a range of customer-owned IP (CoIP) addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "CreateCoipPool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCoipPool",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a pool of customer-owned IP (CoIP) addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool",
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateCoipPoolPermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCoipPoolPermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to allow a service to access a customer-owned IP (CoIP) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "CreateCustomerGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateCustomerGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a customer gateway, which provides information to AWS about your customer gateway device",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "customer-gateway"
-            ]
+            "resources": []
         },
         "CreateDefaultSubnet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateDefaultSubnet",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a default subnet in a specified Availability Zone in a default VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDefaultVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateDefaultVpc",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a default VPC with a default subnet in each Availability Zone",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDhcpOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateDhcpOptions",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:DhcpOptionsID",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a set of DHCP options for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dhcp-options"
-            ]
+            "resources": []
         },
         "CreateEgressOnlyInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateEgressOnlyInternetGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create an egress-only internet gateway for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "egress-only-internet-gateway",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateFleet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateFleet",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:InstanceID",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:KmsKeyId",
-                "ec2:NetworkInterfaceID",
-                "ec2:Owner",
-                "ec2:ParentSnapshot",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroup",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to launch an EC2 Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fleet",
-                "image",
-                "instance",
-                "key-pair",
-                "launch-template",
-                "network-interface",
-                "placement-group",
-                "security-group",
-                "snapshot",
-                "subnet",
-                "volume"
-            ]
+            "resources": []
         },
         "CreateFlowLogs": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateFlowLogs",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:Vpc",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create one or more flow logs to capture IP traffic for a network interface",
-            "orphan": false,
-            "resources": [
-                "network-interface",
-                "subnet",
-                "vpc",
-                "vpc-flow-log"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "CreateFpgaImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateFpgaImage",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create an Amazon FPGA Image (AFI) from a design checkpoint (DCP)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "CreateImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateImage",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:ImageID",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
-                "ec2:Tenancy",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to create an Amazon EBS-backed AMI from a stopped or running Amazon EBS-backed instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "instance",
-                "snapshot"
-            ]
+            "resources": []
         },
         "CreateInstanceEventWindow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateInstanceEventWindow",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create an event window in which scheduled events for the associated Amazon EC2 instances can run",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance-event-window"
-            ]
+            "resources": []
         },
         "CreateInstanceExportTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateInstanceExportTask",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to export a running or stopped instance to an Amazon S3 bucket",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "export-instance-task",
-                "instance"
-            ]
+            "resources": []
         },
         "CreateInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateInternetGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:InternetGatewayID",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create an internet gateway for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "internet-gateway"
-            ]
+            "resources": []
         },
         "CreateIpam": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIpam",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create an Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam"
-            ]
+            "resources": []
         },
         "CreateIpamPool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIpamPool",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create an IP address pool for Amazon VPC IP Address Manager (IPAM), which is a collection of contiguous IP address CIDRs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "CreateIpamResourceDiscovery": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIpamResourceDiscovery",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create an IPAM resource discovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery"
-            ]
+            "resources": []
         },
         "CreateIpamScope": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateIpamScope",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create an Amazon VPC IP Address Manager (IPAM) scope, which is the highest-level container within IPAM",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam",
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "CreateKeyPair": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateKeyPair",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:KeyPairType",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a 2048-bit RSA key pair",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "key-pair"
-            ]
+            "resources": []
         },
         "CreateLaunchTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLaunchTemplate",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a launch template",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template"
-            ]
+            "resources": []
         },
         "CreateLaunchTemplateVersion": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLaunchTemplateVersion",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a new version of a launch template",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template"
-            ]
+            "resources": []
         },
         "CreateLocalGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLocalGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a static route for a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table",
-                "local-gateway-virtual-interface-group",
-                "network-interface",
-                "prefix-list"
-            ]
+            "resources": []
         },
         "CreateLocalGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLocalGatewayRouteTable",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway",
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateLocalGatewayRouteTablePermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLocalGatewayRouteTablePermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to allow a service to access a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociation",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a local gateway route table virtual interface group association",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table",
-                "local-gateway-route-table-virtual-interface-group-association",
-                "local-gateway-virtual-interface-group"
-            ]
+            "resources": []
         },
         "CreateLocalGatewayRouteTableVpcAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateLocalGatewayRouteTableVpcAssociation",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to associate a VPC with a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table",
-                "local-gateway-route-table-vpc-association",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateManagedPrefixList": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateManagedPrefixList",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a managed prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "CreateNatGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNatGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AllocationId",
-                "ec2:AvailabilityZone",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a NAT gateway in a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "natgateway",
-                "subnet"
-            ]
+            "resources": []
         },
         "CreateNetworkAcl": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkAcl",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a network ACL in a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateNetworkAclEntry": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkAclEntry",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a numbered entry (a rule) in a network ACL",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl"
-            ]
+            "resources": []
         },
         "CreateNetworkInsightsAccessScope": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkInsightsAccessScope",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a Network Access Scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-access-scope"
-            ]
+            "resources": []
         },
         "CreateNetworkInsightsPath": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkInsightsPath",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AccepterVpc",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:InternetGatewayID",
-                "ec2:NetworkInterfaceID",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Subnet",
-                "ec2:Tenancy",
-                "ec2:Vpc",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to create a path to analyze for reachability",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "internet-gateway",
-                "network-insights-path",
-                "network-interface",
-                "transit-gateway",
-                "vpc-endpoint",
-                "vpc-endpoint-service",
-                "vpc-peering-connection",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "CreateNetworkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateNetworkInterface",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a network interface in a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "security-group",
-                "subnet"
-            ]
+            "resources": []
         },
         "CreateNetworkInterfacePermission": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "CreateNetworkInterfacePermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AuthorizedService",
-                "ec2:AuthorizedUser",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Permission",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a permission for an AWS-authorized user to perform certain operations on a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "CreatePlacementGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreatePlacementGroup",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a placement group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "placement-group"
-            ]
+            "resources": []
         },
         "CreatePublicIpv4Pool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreatePublicIpv4Pool",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a public IPv4 address pool for public IPv4 CIDRs that you own and bring to Amazon to manage with Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipv4pool-ec2"
-            ]
+            "resources": []
         },
         "CreateReplaceRootVolumeTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateReplaceRootVolumeTask",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to create a root volume replacement task",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "instance",
-                "replace-root-volume-task",
-                "snapshot",
-                "volume"
-            ]
+            "resources": []
         },
         "CreateReservedInstancesListing": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateReservedInstancesListing",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a listing for Standard Reserved Instances to be sold in the Reserved Instance Marketplace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateRestoreImageTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRestoreImageTask",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:ImageID",
-                "ec2:Owner",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to start a task that restores an AMI from an S3 object previously created by using CreateStoreImageTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "CreateRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a route in a VPC route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table"
-            ]
+            "resources": []
         },
         "CreateRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRouteTable",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a route table for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateSecurityGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSecurityGroup",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateSnapshot": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSnapshot",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Encrypted",
-                "ec2:OutpostArn",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SourceOutpostArn",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to create a snapshot of an EBS volume and store it in Amazon S3",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot",
-                "volume"
-            ]
+            "resources": []
         },
         "CreateSnapshots": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSnapshots",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:InstanceID",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:OutpostArn",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SnapshotID",
-                "ec2:SourceOutpostArn",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to create crash-consistent snapshots of multiple EBS volumes and store them in Amazon S3",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "snapshot",
-                "volume"
-            ]
+            "resources": []
         },
         "CreateSpotDatafeedSubscription": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSpotDatafeedSubscription",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a data feed for Spot Instances to view Spot Instance usage logs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateStoreImageTask": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateStoreImageTask",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to store an AMI as a single object in an S3 bucket",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "CreateSubnet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSubnet",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a subnet in a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateSubnetCidrReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateSubnetCidrReservation",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a subnet CIDR reservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateTags": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "CreateTags",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AccepterVpc",
-                "ec2:AllocationId",
-                "ec2:AuthenticationType",
-                "ec2:AuthorizedUser",
-                "ec2:AutoPlacement",
-                "ec2:AvailabilityZone",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:CreateAction",
-                "ec2:DPDTimeoutSeconds",
-                "ec2:DhcpOptionsID",
-                "ec2:DirectoryArn",
-                "ec2:Domain",
-                "ec2:EbsOptimized",
-                "ec2:ElasticGpuType",
-                "ec2:Encrypted",
-                "ec2:GatewayType",
-                "ec2:HostRecovery",
-                "ec2:IKEVersions",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:InsideTunnelCidr",
-                "ec2:InsideTunnelIpv6Cidr",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:InternetGatewayID",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkAclID",
-                "ec2:NetworkInterfaceID",
-                "ec2:Owner",
-                "ec2:ParentSnapshot",
-                "ec2:ParentVolume",
-                "ec2:Permission",
-                "ec2:Phase1DHGroup",
-                "ec2:Phase1EncryptionAlgorithms",
-                "ec2:Phase1IntegrityAlgorithms",
-                "ec2:Phase1LifetimeSeconds",
-                "ec2:Phase2DHGroup",
-                "ec2:Phase2EncryptionAlgorithms",
-                "ec2:Phase2IntegrityAlgorithms",
-                "ec2:Phase2LifetimeSeconds",
-                "ec2:PlacementGroup",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:PreSharedKeys",
-                "ec2:ProductCode",
-                "ec2:Public",
-                "ec2:PublicIpAddress",
-                "ec2:Quantity",
-                "ec2:Region",
-                "ec2:RekeyFuzzPercentage",
-                "ec2:RekeyMarginTimeSeconds",
-                "ec2:ReplayWindowSizePackets",
-                "ec2:RequesterVpc",
-                "ec2:ReservedInstancesOfferingType",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:RouteTableID",
-                "ec2:RoutingType",
-                "ec2:SamlProviderArn",
-                "ec2:SecurityGroupID",
-                "ec2:ServerCertificateArn",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType",
-                "ec2:Vpc",
-                "ec2:VpcID",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to add or overwrite one or more tags for Amazon EC2 resources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation",
-                "capacity-reservation-fleet",
-                "carrier-gateway",
-                "client-vpn-endpoint",
-                "coip-pool",
-                "customer-gateway",
-                "dedicated-host",
-                "dhcp-options",
-                "egress-only-internet-gateway",
-                "elastic-gpu",
-                "elastic-ip",
-                "export-image-task",
-                "export-instance-task",
-                "fleet",
-                "fpga-image",
-                "host-reservation",
-                "image",
-                "import-image-task",
-                "import-snapshot-task",
-                "instance",
-                "instance-event-window",
-                "internet-gateway",
-                "ipam",
-                "ipam-pool",
-                "ipam-resource-discovery",
-                "ipam-resource-discovery-association",
-                "ipam-scope",
-                "ipv4pool-ec2",
-                "ipv6pool-ec2",
-                "key-pair",
-                "launch-template",
-                "local-gateway",
-                "local-gateway-route-table",
-                "local-gateway-route-table-virtual-interface-group-association",
-                "local-gateway-route-table-vpc-association",
-                "local-gateway-virtual-interface",
-                "local-gateway-virtual-interface-group",
-                "natgateway",
-                "network-acl",
-                "network-insights-access-scope",
-                "network-insights-access-scope-analysis",
-                "network-insights-analysis",
-                "network-insights-path",
-                "network-interface",
-                "placement-group",
-                "prefix-list",
-                "replace-root-volume-task",
-                "reserved-instances",
-                "route-table",
-                "security-group",
-                "security-group-rule",
-                "snapshot",
-                "spot-fleet-request",
-                "spot-instances-request",
-                "subnet",
-                "subnet-cidr-reservation",
-                "traffic-mirror-filter",
-                "traffic-mirror-session",
-                "traffic-mirror-target",
-                "transit-gateway",
-                "transit-gateway-attachment",
-                "transit-gateway-connect-peer",
-                "transit-gateway-multicast-domain",
-                "transit-gateway-policy-table",
-                "transit-gateway-route-table",
-                "transit-gateway-route-table-announcement",
-                "verified-access-endpoint",
-                "verified-access-group",
-                "verified-access-instance",
-                "verified-access-policy",
-                "verified-access-trust-provider",
-                "volume",
-                "vpc",
-                "vpc-endpoint",
-                "vpc-endpoint-connection",
-                "vpc-endpoint-service",
-                "vpc-endpoint-service-permission",
-                "vpc-flow-log",
-                "vpc-peering-connection",
-                "vpn-connection",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "CreateTrafficMirrorFilter": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTrafficMirrorFilter",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a traffic mirror filter",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter"
-            ]
+            "resources": []
         },
         "CreateTrafficMirrorFilterRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTrafficMirrorFilterRule",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a traffic mirror filter rule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter"
-            ]
+            "resources": []
         },
         "CreateTrafficMirrorSession": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTrafficMirrorSession",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a traffic mirror session",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "traffic-mirror-filter",
-                "traffic-mirror-session",
-                "traffic-mirror-target"
-            ]
+            "resources": []
         },
         "CreateTrafficMirrorTarget": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTrafficMirrorTarget",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpceServiceName",
-                "ec2:VpceServiceOwner"
-            ],
-            "description": "Grants permission to create a traffic mirror target",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "traffic-mirror-target",
-                "vpc-endpoint"
-            ]
+            "resources": []
         },
         "CreateTransitGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayConnect": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayConnect",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a Connect attachment from a specified transit gateway attachment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayConnectPeer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayConnectPeer",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a Connect peer between a transit gateway and an appliance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-connect-peer"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayMulticastDomain": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayMulticastDomain",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a multicast domain for a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayPeeringAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayPeeringAttachment",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to request a transit gateway peering attachment between a requester and accepter transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway",
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayPolicyTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayPolicyTable",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a transit gateway policy table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway",
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayPrefixListReference": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayPrefixListReference",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a transit gateway prefix list reference",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list",
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a static route for a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayRouteTable",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a route table for a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayRouteTableAnnouncement": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayRouteTableAnnouncement",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create an announcement for a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table",
-                "transit-gateway-route-table-announcement"
-            ]
+            "resources": []
         },
         "CreateTransitGatewayVpcAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTransitGatewayVpcAttachment",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:Vpc",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to attach a VPC to a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "transit-gateway",
-                "transit-gateway-attachment",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateVerifiedAccessEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVerifiedAccessEndpoint",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AuthorizedUser",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Permission",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a Verified Access endpoint",
-            "orphan": false,
-            "resources": [
-                "network-interface",
-                "security-group",
-                "subnet",
-                "verified-access-endpoint",
-                "verified-access-group"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "CreateVerifiedAccessGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVerifiedAccessGroup",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a Verified Access group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-group",
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "CreateVerifiedAccessInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVerifiedAccessInstance",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "CreateVerifiedAccessTrustProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVerifiedAccessTrustProvider",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a verified trust provider",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-trust-provider"
-            ]
+            "resources": []
         },
         "CreateVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVolume",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:KmsKeyId",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to create an EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "CreateVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpc",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Ipv4IpamPoolId",
-                "ec2:Ipv6IpamPoolId",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to create a VPC with a specified CIDR block",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "ipv6pool-ec2",
-                "vpc"
-            ]
+            "resources": []
         },
         "CreateVpcEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpcEndpoint",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:SecurityGroupID",
-                "ec2:SubnetID",
-                "ec2:VpcID",
-                "ec2:VpceServiceName",
-                "ec2:VpceServiceOwner"
-            ],
-            "description": "Grants permission to create a VPC endpoint for an AWS service",
-            "orphan": false,
-            "resources": [
-                "route-table",
-                "security-group",
-                "subnet",
-                "vpc",
-                "vpc-endpoint"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "CreateVpcEndpointConnectionNotification": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpcEndpointConnectionNotification",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a connection notification for a VPC endpoint or VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint",
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "CreateVpcEndpointServiceConfiguration": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpcEndpointServiceConfiguration",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:VpceServicePrivateDnsName"
-            ],
-            "description": "Grants permission to create a VPC endpoint service configuration to which service consumers (AWS accounts, IAM users, and IAM roles) can connect",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "CreateVpcPeeringConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpcPeeringConnection",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AccepterVpc",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to request a VPC peering connection between two VPCs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc",
-                "vpc-peering-connection"
-            ]
+            "resources": []
         },
         "CreateVpnConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpnConnection",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AuthenticationType",
-                "ec2:DPDTimeoutSeconds",
-                "ec2:GatewayType",
-                "ec2:IKEVersions",
-                "ec2:InsideTunnelCidr",
-                "ec2:InsideTunnelIpv6Cidr",
-                "ec2:Phase1DHGroup",
-                "ec2:Phase1EncryptionAlgorithms",
-                "ec2:Phase1IntegrityAlgorithms",
-                "ec2:Phase1LifetimeSeconds",
-                "ec2:Phase2DHGroup",
-                "ec2:Phase2EncryptionAlgorithms",
-                "ec2:Phase2IntegrityAlgorithms",
-                "ec2:Phase2LifetimeSeconds",
-                "ec2:PreSharedKeys",
-                "ec2:Region",
-                "ec2:RekeyFuzzPercentage",
-                "ec2:RekeyMarginTimeSeconds",
-                "ec2:ReplayWindowSizePackets",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RoutingType"
-            ],
-            "description": "Grants permission to create a VPN connection between a virtual private gateway or transit gateway and a customer gateway",
-            "orphan": false,
-            "resources": [
-                "customer-gateway",
-                "transit-gateway",
-                "transit-gateway-attachment",
-                "vpn-connection",
-                "vpn-gateway"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "CreateVpnConnectionRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpnConnectionRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to create a static route for a VPN connection between a virtual private gateway and a customer gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "CreateVpnGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateVpnGateway",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to create a virtual private gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "DeleteCarrierGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteCarrierGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a carrier gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "carrier-gateway"
-            ]
+            "resources": []
         },
         "DeleteClientVpnEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteClientVpnEndpoint",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to delete a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DeleteClientVpnRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteClientVpnRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a route from a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "subnet"
-            ]
+            "resources": []
         },
         "DeleteCoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteCoipCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a range of customer-owned IP (CoIP) addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "DeleteCoipPool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteCoipPool",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a pool of customer-owned IP (CoIP) addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "DeleteCoipPoolPermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteCoipPoolPermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to deny a service from accessing a customer-owned IP (CoIP) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "DeleteCustomerGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteCustomerGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a customer gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "customer-gateway"
-            ]
+            "resources": []
         },
         "DeleteDhcpOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteDhcpOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:DhcpOptionsID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a set of DHCP options",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dhcp-options"
-            ]
+            "resources": []
         },
         "DeleteEgressOnlyInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteEgressOnlyInternetGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an egress-only internet gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "egress-only-internet-gateway"
-            ]
+            "resources": []
         },
         "DeleteFleets": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteFleets",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more EC2 Fleets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fleet"
-            ]
+            "resources": []
         },
         "DeleteFlowLogs": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteFlowLogs",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more flow logs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-flow-log"
-            ]
+            "resources": []
         },
         "DeleteFpgaImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteFpgaImage",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an Amazon FPGA Image (AFI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "DeleteInstanceEventWindow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteInstanceEventWindow",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete the specified event window",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance-event-window"
-            ]
+            "resources": []
         },
         "DeleteInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteInternetGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an internet gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "internet-gateway"
-            ]
+            "resources": []
         },
         "DeleteIpam": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIpam",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an Amazon VPC IP Address Manager (IPAM) and remove all monitored data associated with the IPAM including the historical data for CIDRs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam"
-            ]
+            "resources": []
         },
         "DeleteIpamPool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIpamPool",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "DeleteIpamResourceDiscovery": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIpamResourceDiscovery",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an IPAM resource discovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery"
-            ]
+            "resources": []
         },
         "DeleteIpamScope": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteIpamScope",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete the scope for an Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "DeleteKeyPair": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteKeyPair",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a key pair by removing the public key from Amazon EC2",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "key-pair"
-            ]
+            "resources": []
         },
         "DeleteLaunchTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLaunchTemplate",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a launch template and its associated versions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template"
-            ]
+            "resources": []
         },
         "DeleteLaunchTemplateVersions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLaunchTemplateVersions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more versions of a launch template",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template"
-            ]
+            "resources": []
         },
         "DeleteLocalGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLocalGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a route from a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table",
-                "prefix-list"
-            ]
+            "resources": []
         },
         "DeleteLocalGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLocalGatewayRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "DeleteLocalGatewayRouteTablePermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLocalGatewayRouteTablePermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to deny a service from accessing a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "DeleteLocalGatewayRouteTableVirtualInterfaceGroupAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLocalGatewayRouteTableVirtualInterfaceGroupAssociation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a local gateway route table virtual interface group association",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table-virtual-interface-group-association"
-            ]
+            "resources": []
         },
         "DeleteLocalGatewayRouteTableVpcAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteLocalGatewayRouteTableVpcAssociation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete an association between a VPC and local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table-vpc-association"
-            ]
+            "resources": []
         },
         "DeleteManagedPrefixList": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteManagedPrefixList",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a managed prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "DeleteNatGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNatGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a NAT gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "natgateway"
-            ]
+            "resources": []
         },
         "DeleteNetworkAcl": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkAcl",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a network ACL",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl"
-            ]
+            "resources": []
         },
         "DeleteNetworkAclEntry": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkAclEntry",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete an inbound or outbound entry (rule) from a network ACL",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl"
-            ]
+            "resources": []
         },
         "DeleteNetworkInsightsAccessScope": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInsightsAccessScope",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a Network Access Scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-access-scope"
-            ]
+            "resources": []
         },
         "DeleteNetworkInsightsAccessScopeAnalysis": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInsightsAccessScopeAnalysis",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a Network Access Scope analysis",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-access-scope-analysis"
-            ]
+            "resources": []
         },
         "DeleteNetworkInsightsAnalysis": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInsightsAnalysis",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a network insights analysis",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-analysis"
-            ]
+            "resources": []
         },
         "DeleteNetworkInsightsPath": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInsightsPath",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a network insights path",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-path"
-            ]
+            "resources": []
         },
         "DeleteNetworkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInterface",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a detached network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "DeleteNetworkInterfacePermission": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "DeleteNetworkInterfacePermission",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a permission that is associated with a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "DeletePlacementGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeletePlacementGroup",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a placement group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "placement-group"
-            ]
+            "resources": []
         },
         "DeletePublicIpv4Pool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeletePublicIpv4Pool",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a public IPv4 address pool for public IPv4 CIDRs that you own and brought to Amazon to manage with Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipv4pool-ec2"
-            ]
+            "resources": []
         },
         "DeleteQueuedReservedInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteQueuedReservedInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to delete the queued purchases for the specified Reserved Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteResourcePolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteResourcePolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to remove an IAM policy that enables cross-account sharing from a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "placement-group",
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "DeleteRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a route from a route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table"
-            ]
+            "resources": []
         },
         "DeleteRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table"
-            ]
+            "resources": []
         },
         "DeleteSecurityGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSecurityGroup",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group"
-            ]
+            "resources": []
         },
         "DeleteSnapshot": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSnapshot",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to delete a snapshot of an EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "DeleteSpotDatafeedSubscription": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSpotDatafeedSubscription",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to delete a data feed for Spot Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteSubnet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSubnet",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to delete a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet"
-            ]
+            "resources": []
         },
         "DeleteSubnetCidrReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteSubnetCidrReservation",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to delete a subnet CIDR reservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteTags": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "DeleteTags",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more tags from Amazon EC2 resources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation",
-                "capacity-reservation-fleet",
-                "carrier-gateway",
-                "client-vpn-endpoint",
-                "coip-pool",
-                "customer-gateway",
-                "dedicated-host",
-                "dhcp-options",
-                "egress-only-internet-gateway",
-                "elastic-gpu",
-                "elastic-ip",
-                "export-image-task",
-                "export-instance-task",
-                "fleet",
-                "fpga-image",
-                "host-reservation",
-                "image",
-                "import-image-task",
-                "import-snapshot-task",
-                "instance",
-                "instance-event-window",
-                "internet-gateway",
-                "ipam",
-                "ipam-pool",
-                "ipam-resource-discovery",
-                "ipam-resource-discovery-association",
-                "ipam-scope",
-                "ipv4pool-ec2",
-                "ipv6pool-ec2",
-                "key-pair",
-                "launch-template",
-                "local-gateway",
-                "local-gateway-route-table",
-                "local-gateway-route-table-virtual-interface-group-association",
-                "local-gateway-route-table-vpc-association",
-                "local-gateway-virtual-interface",
-                "local-gateway-virtual-interface-group",
-                "natgateway",
-                "network-acl",
-                "network-insights-access-scope",
-                "network-insights-access-scope-analysis",
-                "network-insights-analysis",
-                "network-insights-path",
-                "network-interface",
-                "placement-group",
-                "prefix-list",
-                "replace-root-volume-task",
-                "reserved-instances",
-                "route-table",
-                "security-group",
-                "security-group-rule",
-                "snapshot",
-                "spot-fleet-request",
-                "spot-instances-request",
-                "subnet",
-                "subnet-cidr-reservation",
-                "traffic-mirror-filter",
-                "traffic-mirror-session",
-                "traffic-mirror-target",
-                "transit-gateway",
-                "transit-gateway-attachment",
-                "transit-gateway-connect-peer",
-                "transit-gateway-multicast-domain",
-                "transit-gateway-policy-table",
-                "transit-gateway-route-table",
-                "transit-gateway-route-table-announcement",
-                "verified-access-endpoint",
-                "verified-access-group",
-                "verified-access-instance",
-                "verified-access-policy",
-                "verified-access-trust-provider",
-                "volume",
-                "vpc",
-                "vpc-endpoint",
-                "vpc-endpoint-connection",
-                "vpc-endpoint-service",
-                "vpc-endpoint-service-permission",
-                "vpc-flow-log",
-                "vpc-peering-connection",
-                "vpn-connection",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "DeleteTrafficMirrorFilter": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTrafficMirrorFilter",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a traffic mirror filter",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter"
-            ]
+            "resources": []
         },
         "DeleteTrafficMirrorFilterRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTrafficMirrorFilterRule",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a traffic mirror filter rule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter",
-                "traffic-mirror-filter-rule"
-            ]
+            "resources": []
         },
         "DeleteTrafficMirrorSession": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTrafficMirrorSession",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a traffic mirror session",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-session"
-            ]
+            "resources": []
         },
         "DeleteTrafficMirrorTarget": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTrafficMirrorTarget",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a traffic mirror target",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-target"
-            ]
+            "resources": []
         },
         "DeleteTransitGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayConnect": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayConnect",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway connect attachment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayConnectPeer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayConnectPeer",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway connect peer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-connect-peer"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayMulticastDomain": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayMulticastDomain",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayPeeringAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayPeeringAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a peering attachment from a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayPolicyTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayPolicyTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway policy table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayPrefixListReference": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayPrefixListReference",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway prefix list reference",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a route from a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayRouteTableAnnouncement": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayRouteTableAnnouncement",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a transit gateway route table announcement",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-route-table-announcement"
-            ]
+            "resources": []
         },
         "DeleteTransitGatewayVpcAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTransitGatewayVpcAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a VPC attachment from a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "DeleteVerifiedAccessEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVerifiedAccessEndpoint",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a Verified Access endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-endpoint"
-            ]
+            "resources": []
         },
         "DeleteVerifiedAccessGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVerifiedAccessGroup",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a Verified Access group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "DeleteVerifiedAccessInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVerifiedAccessInstance",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "DeleteVerifiedAccessTrustProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVerifiedAccessTrustProvider",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a verified trust provider",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-trust-provider"
-            ]
+            "resources": []
         },
         "DeleteVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVolume",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to delete an EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "DeleteVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpc",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to delete a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "DeleteVpcEndpointConnectionNotifications": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpcEndpointConnectionNotifications",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more VPC endpoint connection notifications",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint",
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "DeleteVpcEndpointServiceConfigurations": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpcEndpointServiceConfigurations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete one or more VPC endpoint service configurations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "DeleteVpcEndpoints": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpcEndpoints",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpceServiceName"
-            ],
-            "description": "Grants permission to delete one or more VPC endpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint"
-            ]
+            "resources": []
         },
         "DeleteVpcPeeringConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpcPeeringConnection",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AccepterVpc",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to delete a VPC peering connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-peering-connection"
-            ]
+            "resources": []
         },
         "DeleteVpnConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpnConnection",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a VPN connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "DeleteVpnConnectionRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpnConnectionRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a static route for a VPN connection between a virtual private gateway and a customer gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "DeleteVpnGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteVpnGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to delete a virtual private gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "DeprovisionByoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeprovisionByoipCidr",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to release an IP address range that was provisioned through bring your own IP addresses (BYOIP), and to delete the corresponding address pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeprovisionIpamPoolCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeprovisionIpamPoolCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to deprovision a CIDR provisioned from an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "DeprovisionPublicIpv4PoolCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeprovisionPublicIpv4PoolCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to deprovision a CIDR from a public IPv4 pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipv4pool-ec2"
-            ]
+            "resources": []
         },
         "DeregisterImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterImage",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to deregister an Amazon Machine Image (AMI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "DeregisterInstanceEventNotificationAttributes": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterInstanceEventNotificationAttributes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to remove tags from the set of tags to include in notifications about scheduled events for your instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeregisterTransitGatewayMulticastGroupMembers": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterTransitGatewayMulticastGroupMembers",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to deregister one or more network interface members from a group IP address in a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "DeregisterTransitGatewayMulticastGroupSources": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterTransitGatewayMulticastGroupSources",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to deregister one or more network interface sources from a group IP address in a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "DescribeAccountAttributes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAccountAttributes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the attributes of the AWS account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeAddressTransfers": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAddressTransfers",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe an Elastic IP address transfer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeAddresses": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAddresses",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Elastic IP addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeAddressesAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAddressesAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the attributes of the specified Elastic IP addresses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "DescribeAggregateIdFormat": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAggregateIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the longer ID format settings for all resource types",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeAvailabilityZones": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAvailabilityZones",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more of the Availability Zones that are available to you",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeAwsNetworkPerformanceMetricSubscriptions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeAwsNetworkPerformanceMetricSubscriptions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the current infrastructure performance metric subscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeBundleTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeBundleTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more bundling tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeByoipCidrs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeByoipCidrs",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the IP address ranges that were provisioned through bring your own IP addresses (BYOIP)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeCapacityReservationFleets": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeCapacityReservationFleets",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Capacity Reservation Fleets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeCapacityReservations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeCapacityReservations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Capacity Reservations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeCarrierGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeCarrierGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Carrier Gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeClassicLinkInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClassicLinkInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more linked EC2-Classic instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeClientVpnAuthorizationRules": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClientVpnAuthorizationRules",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the authorization rules for a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DescribeClientVpnConnections": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClientVpnConnections",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to describe active client connections and connections that have been terminated within the last 60 minutes for a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DescribeClientVpnEndpoints": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClientVpnEndpoints",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to describe one or more Client VPN endpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DescribeClientVpnRoutes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClientVpnRoutes",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to describe the routes for a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DescribeClientVpnTargetNetworks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeClientVpnTargetNetworks",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to describe the target networks that are associated with a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DescribeCoipPools": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeCoipPools",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the specified customer-owned address pools or all of your customer-owned address pools",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeConversionTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeConversionTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more conversion tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeCustomerGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeCustomerGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more customer gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeDhcpOptions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeDhcpOptions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more DHCP options sets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeEgressOnlyInternetGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeEgressOnlyInternetGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more egress-only internet gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeElasticGpus": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeElasticGpus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe an Elastic Graphics accelerator that is associated with an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeExportImageTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeExportImageTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more export image tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeExportTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeExportTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more export instance tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFastLaunchImages": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFastLaunchImages",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to describe fast-launch enabled Windows AMIs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "DescribeFastSnapshotRestores": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFastSnapshotRestores",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the state of fast snapshot restores for snapshots",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFleetHistory": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFleetHistory",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the events for an EC2 Fleet during a specified time",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fleet"
-            ]
+            "resources": []
         },
         "DescribeFleetInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFleetInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the running instances for an EC2 Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fleet"
-            ]
+            "resources": []
         },
         "DescribeFleets": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFleets",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more EC2 Fleets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFlowLogs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFlowLogs",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more flow logs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFpgaImageAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFpgaImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Owner",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the attributes of an Amazon FPGA Image (AFI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "DescribeFpgaImages": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeFpgaImages",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Amazon FPGA Images (AFIs)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeHostReservationOfferings": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeHostReservationOfferings",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the Dedicated Host Reservations that are available to purchase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeHostReservations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeHostReservations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the Dedicated Host Reservations that are associated with Dedicated Hosts in the AWS account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeHosts": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeHosts",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Dedicated Hosts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIamInstanceProfileAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIamInstanceProfileAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the IAM instance profile associations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIdFormat": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the ID format settings for resources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIdentityIdFormat": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIdentityIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the ID format settings for resources for an IAM user, IAM role, or root user",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeImageAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to describe an attribute of an Amazon Machine Image (AMI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "DescribeImages": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeImages",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more images (AMIs, AKIs, and ARIs)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeImportImageTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeImportImageTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe import virtual machine or import snapshot tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeImportSnapshotTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeImportSnapshotTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe import snapshot tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to describe the attributes of an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "DescribeInstanceCreditSpecifications": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceCreditSpecifications",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the credit option for CPU usage of one or more burstable performance instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceEventNotificationAttributes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceEventNotificationAttributes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the set of tags to include in notifications about scheduled events for your instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceEventWindows": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceEventWindows",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the specified event windows or all event windows",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceStatus": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceStatus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the status of one or more instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceTypeOfferings": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceTypeOfferings",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the set of instance types that are offered in a location",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceTypes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstanceTypes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the details of instance types that are offered in a location",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInternetGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeInternetGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more internet gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamPools": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpamPools",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe Amazon VPC IP Address Manager (IPAM) pools",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamResourceDiscoveries": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpamResourceDiscoveries",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe IPAM resource discoveries",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamResourceDiscoveryAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpamResourceDiscoveryAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe resource discovery associations with an Amazon VPC IPAM",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpamScopes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpamScopes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe Amazon VPC IP Address Manager (IPAM) scopes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpams": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpams",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe an Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeIpv6Pools": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeIpv6Pools",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more IPv6 address pools",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeKeyPairs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeKeyPairs",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more key pairs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLaunchTemplateVersions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLaunchTemplateVersions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more launch template versions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLaunchTemplates": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLaunchTemplates",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more launch templates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTablePermissions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayRouteTablePermissions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to allow a service to describe local gateway route table permissions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the associations between virtual interface groups and local gateway route tables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTableVpcAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayRouteTableVpcAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe an association between VPCs and local gateway route tables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayRouteTables": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayRouteTables",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more local gateway route tables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayVirtualInterfaceGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayVirtualInterfaceGroups",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe local gateway virtual interface groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGatewayVirtualInterfaces": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGatewayVirtualInterfaces",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe local gateway virtual interfaces",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLocalGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeLocalGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more local gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeManagedPrefixLists": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeManagedPrefixLists",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe your managed prefix lists and any AWS-managed prefix lists",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeMovingAddresses": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeMovingAddresses",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe Elastic IP addresses that are being moved to the EC2-VPC platform",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNatGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNatGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more NAT gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkAcls": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkAcls",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more network ACLs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAccessScopeAnalyses": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInsightsAccessScopeAnalyses",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Network Access Scope analyses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAccessScopes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInsightsAccessScopes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the Network Access Scopes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsAnalyses": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInsightsAnalyses",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more network insights analyses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInsightsPaths": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInsightsPaths",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more network insights paths",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfaceAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInterfaceAttribute",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe a network interface attribute",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfacePermissions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInterfacePermissions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the permissions that are associated with a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeNetworkInterfaces": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeNetworkInterfaces",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more network interfaces",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribePlacementGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribePlacementGroups",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more placement groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribePrefixLists": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribePrefixLists",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe available AWS services in a prefix list format",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribePrincipalIdFormat": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribePrincipalIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the ID format settings for the root user and all IAM roles and IAM users that have explicitly specified a longer ID (17-character ID) preference",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribePublicIpv4Pools": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribePublicIpv4Pools",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more IPv4 address pools",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeRegions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeRegions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more AWS Regions that are currently available in your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeReplaceRootVolumeTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeReplaceRootVolumeTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe a root volume replacement task",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeReservedInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more purchased Reserved Instances in your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesListings": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeReservedInstancesListings",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe your account's Reserved Instance listings in the Reserved Instance Marketplace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesModifications": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeReservedInstancesModifications",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the modifications made to one or more Reserved Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeReservedInstancesOfferings": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeReservedInstancesOfferings",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the Reserved Instance offerings that are available for purchase",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeRouteTables": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeRouteTables",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more route tables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeScheduledInstanceAvailability": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeScheduledInstanceAvailability",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to find available schedules for Scheduled Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeScheduledInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeScheduledInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Scheduled Instances in your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroupReferences": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSecurityGroupReferences",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the VPCs on the other side of a VPC peering connection that are referencing specified VPC security groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroupRules": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSecurityGroupRules",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more of your security group rules",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSecurityGroups",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more security groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSnapshotAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSnapshotAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Encrypted",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to describe an attribute of a snapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "DescribeSnapshotTierStatus": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSnapshotTierStatus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the storage tier status for Amazon EBS snapshots",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSnapshots": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSnapshots",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more EBS snapshots",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotDatafeedSubscription": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotDatafeedSubscription",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the data feed for Spot Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotFleetInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotFleetInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the running instances for a Spot Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "spot-fleet-request"
-            ]
+            "resources": []
         },
         "DescribeSpotFleetRequestHistory": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotFleetRequestHistory",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the events for a Spot Fleet request during a specified time",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "spot-fleet-request"
-            ]
+            "resources": []
         },
         "DescribeSpotFleetRequests": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotFleetRequests",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Spot Fleet requests",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotInstanceRequests": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotInstanceRequests",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more Spot Instance requests",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSpotPriceHistory": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSpotPriceHistory",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the Spot Instance price history",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeStaleSecurityGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeStaleSecurityGroups",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the stale security group rules for security groups in a specified VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeStoreImageTasks": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeStoreImageTasks",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the progress of the AMI store tasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSubnets": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeSubnets",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more subnets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTags": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTags",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more tags for an Amazon EC2 resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorFilters": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTrafficMirrorFilters",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more traffic mirror filters",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorSessions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTrafficMirrorSessions",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more traffic mirror sessions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTrafficMirrorTargets": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTrafficMirrorTargets",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more traffic mirror targets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayAttachments": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayAttachments",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more attachments between resources and transit gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayConnectPeers": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayConnectPeers",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateway connect peers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayConnects": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayConnects",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateway connect attachments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayMulticastDomains": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayMulticastDomains",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateway multicast domains",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayPeeringAttachments": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayPeeringAttachments",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateway peering attachments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayPolicyTables": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayPolicyTables",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe a transit gateway policy table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayRouteTableAnnouncements": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayRouteTableAnnouncements",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe a transit gateway route table announcement",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayRouteTables": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayRouteTables",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateway route tables",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGatewayVpcAttachments": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGatewayVpcAttachments",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more VPC attachments on a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTransitGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTransitGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more transit gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTrunkInterfaceAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeTrunkInterfaceAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more network interface trunk associations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessEndpoints": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessEndpoints",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the specified Verified Access endpoints or all Verified Access endpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessGroups",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the specified Verified Access groups or all Verified Access groups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstanceLoggingConfigurations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessInstanceLoggingConfigurations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the current logging configuration for the Verified Access instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstanceWebAclAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessInstanceWebAclAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the AWS Web Application Firewall (WAF) web access control list (ACL) associations for a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessInstances": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the specified Verified Access instances or all Verified Access instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVerifiedAccessTrustProviders": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVerifiedAccessTrustProviders",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe details of existing Verified Access trust providers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumeAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVolumeAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to describe an attribute of an EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "DescribeVolumeStatus": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVolumeStatus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the status of one or more EBS volumes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVolumes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more EBS volumes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVolumesModifications": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVolumesModifications",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the current modification status of one or more EBS volumes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcAttribute": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to describe an attribute of a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "DescribeVpcClassicLink": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcClassicLink",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the ClassicLink status of one or more VPCs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcClassicLinkDnsSupport": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcClassicLinkDnsSupport",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the ClassicLink DNS support status of one or more VPCs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointConnectionNotifications": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpointConnectionNotifications",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the connection notifications for VPC endpoints and VPC endpoint services",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointConnections": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpointConnections",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe the VPC endpoint connections to your VPC endpoint services",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointServiceConfigurations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpointServiceConfigurations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe VPC endpoint service configurations (your services)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpointServicePermissions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpointServicePermissions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the principals (service consumers) that are permitted to discover your VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "DescribeVpcEndpointServices": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpointServices",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe all supported AWS services that can be specified when creating a VPC endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcEndpoints": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcEndpoints",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more VPC endpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcPeeringConnections": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcPeeringConnections",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more VPC peering connections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpcs": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpcs",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more VPCs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpnConnections": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpnConnections",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more VPN connections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeVpnGateways": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "DescribeVpnGateways",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe one or more virtual private gateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DetachClassicLinkVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachClassicLinkVpc",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to unlink (detach) a linked EC2-Classic instance from a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "vpc"
-            ]
+            "resources": []
         },
         "DetachInternetGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachInternetGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to detach an internet gateway from a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "internet-gateway",
-                "vpc"
-            ]
+            "resources": []
         },
         "DetachNetworkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachNetworkInterface",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkInterfaceID",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Subnet",
-                "ec2:Tenancy",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to detach a network interface from an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "network-interface"
-            ]
+            "resources": []
         },
         "DetachVerifiedAccessTrustProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachVerifiedAccessTrustProvider",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to detach a trust provider from a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance",
-                "verified-access-trust-provider"
-            ]
+            "resources": []
         },
         "DetachVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachVolume",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ParentSnapshot",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to detach an EBS volume from an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "volume"
-            ]
+            "resources": []
         },
         "DetachVpnGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DetachVpnGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to detach a virtual private gateway from a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "DisableAddressTransfer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableAddressTransfer",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disable Elastic IP address transfer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "DisableAwsNetworkPerformanceMetricSubscription": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableAwsNetworkPerformanceMetricSubscription",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disable infrastructure performance metric subscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisableEbsEncryptionByDefault": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableEbsEncryptionByDefault",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disable EBS encryption by default for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisableFastLaunch": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableFastLaunch",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to disable faster launching for Windows AMIs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "DisableFastSnapshotRestores": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableFastSnapshotRestores",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to disable fast snapshot restores for one or more snapshots in specified Availability Zones",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "DisableImageDeprecation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableImageDeprecation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to cancel the deprecation of the specified AMI",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "DisableIpamOrganizationAdminAccount": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableIpamOrganizationAdminAccount",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisableSerialConsoleAccess": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableSerialConsoleAccess",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disable access to the EC2 serial console of all instances for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisableTransitGatewayRouteTablePropagation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableTransitGatewayRouteTablePropagation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disable a resource attachment from propagating routes to the specified propagation route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table",
-                "transit-gateway-route-table-announcement"
-            ]
+            "resources": []
         },
         "DisableVgwRoutePropagation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableVgwRoutePropagation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disable a virtual private gateway from propagating routes to a specified route table of a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "DisableVpcClassicLink": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableVpcClassicLink",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to disable ClassicLink for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "DisableVpcClassicLinkDnsSupport": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableVpcClassicLinkDnsSupport",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to disable ClassicLink DNS support for a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "DisassociateAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:AvailabilityZone",
-                "ec2:Domain",
-                "ec2:NetworkInterfaceID",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disassociate an Elastic IP address from an instance or network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "network-interface"
-            ]
+            "resources": []
         },
         "DisassociateClientVpnTargetNetwork": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateClientVpnTargetNetwork",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to disassociate a target network from a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "DisassociateEnclaveCertificateIamRole": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateEnclaveCertificateIamRole",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disassociate an ACM certificate from a IAM role",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "certificate",
-                "role"
-            ]
+            "resources": []
         },
         "DisassociateIamInstanceProfile": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateIamInstanceProfile",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to disassociate an IAM instance profile from a running or stopped instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "DisassociateInstanceEventWindow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateInstanceEventWindow",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disassociate one or more targets from an event window",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance-event-window"
-            ]
+            "resources": []
         },
         "DisassociateIpamResourceDiscovery": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateIpamResourceDiscovery",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disassociate a resource discovery from an Amazon VPC IPAM",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery-association"
-            ]
+            "resources": []
         },
         "DisassociateNatGatewayAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateNatGatewayAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:AuthorizedUser",
-                "ec2:AvailabilityZone",
-                "ec2:Domain",
-                "ec2:NetworkInterfaceID",
-                "ec2:Permission",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disassociate a secondary Elastic IP address from a public NAT gateway",
-            "orphan": false,
-            "resources": [
-                "elastic-ip",
-                "natgateway",
-                "network-interface"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "DisassociateRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disassociate a subnet from a route table",
-            "orphan": false,
-            "resources": [
-                "internet-gateway",
-                "ipv4pool-ec2",
-                "ipv6pool-ec2",
-                "route-table",
-                "subnet",
-                "vpn-gateway"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "DisassociateSubnetCidrBlock": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateSubnetCidrBlock",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disassociate a CIDR block from a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet"
-            ]
+            "resources": []
         },
         "DisassociateTransitGatewayMulticastDomain": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateTransitGatewayMulticastDomain",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to disassociate one or more subnets from a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "transit-gateway-attachment",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "DisassociateTransitGatewayPolicyTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateTransitGatewayPolicyTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disassociate a policy table from a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "DisassociateTransitGatewayRouteTable": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateTransitGatewayRouteTable",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disassociate a resource attachment from a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "DisassociateTrunkInterface": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateTrunkInterface",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to disassociate a branch network interface to a trunk network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisassociateVerifiedAccessInstanceWebAcl": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateVerifiedAccessInstanceWebAcl",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to disassociate an AWS Web Application Firewall (WAF) web access control list (ACL) from a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "DisassociateVpcCidrBlock": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateVpcCidrBlock",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to disassociate a CIDR block from a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "EnableAddressTransfer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableAddressTransfer",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to enable Elastic IP address transfer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "EnableAwsNetworkPerformanceMetricSubscription": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableAwsNetworkPerformanceMetricSubscription",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to enable infrastructure performance subscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableEbsEncryptionByDefault": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableEbsEncryptionByDefault",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to enable EBS encryption by default for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableFastLaunch": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableFastLaunch",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to enable faster launching for Windows AMIs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "launch-template"
-            ]
+            "resources": []
         },
         "EnableFastSnapshotRestores": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableFastSnapshotRestores",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to enable fast snapshot restores for one or more snapshots in specified Availability Zones",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "EnableImageDeprecation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableImageDeprecation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to enable deprecation of the specified AMI at the specified date and time",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "EnableIpamOrganizationAdminAccount": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableIpamOrganizationAdminAccount",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to enable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableReachabilityAnalyzerOrganizationSharing": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableReachabilityAnalyzerOrganizationSharing",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to enable organization sharing of reachability analyzer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableSerialConsoleAccess": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableSerialConsoleAccess",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to enable access to the EC2 serial console of all instances for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableTransitGatewayRouteTablePropagation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableTransitGatewayRouteTablePropagation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to enable an attachment to propagate routes to a propagation route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table",
-                "transit-gateway-route-table-announcement"
-            ]
+            "resources": []
         },
         "EnableVgwRoutePropagation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableVgwRoutePropagation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to enable a virtual private gateway to propagate routes to a VPC route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table",
-                "vpn-gateway"
-            ]
+            "resources": []
         },
         "EnableVolumeIO": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableVolumeIO",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to enable I/O operations for a volume that had I/O operations disabled",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "EnableVpcClassicLink": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableVpcClassicLink",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to enable a VPC for ClassicLink",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "EnableVpcClassicLinkDnsSupport": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableVpcClassicLinkDnsSupport",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to enable a VPC to support DNS hostname resolution for ClassicLink",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "ExportClientVpnClientCertificateRevocationList": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ExportClientVpnClientCertificateRevocationList",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to download the client certificate revocation list for a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "ExportClientVpnClientConfiguration": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ExportClientVpnClientConfiguration",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to download the contents of the Client VPN endpoint configuration file for a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "ExportImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ExportImage",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to export an Amazon Machine Image (AMI) to a VM file",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "export-image-task",
-                "image"
-            ]
+            "resources": []
         },
         "ExportTransitGatewayRoutes": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ExportTransitGatewayRoutes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to export routes from a transit gateway route table to an Amazon S3 bucket",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAssociatedEnclaveCertificateIamRoles": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetAssociatedEnclaveCertificateIamRoles",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get the list of roles associated with an ACM certificate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "certificate"
-            ]
+            "resources": []
         },
         "GetAssociatedIpv6PoolCidrs": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetAssociatedIpv6PoolCidrs",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get information about the IPv6 CIDR block associations for a specified IPv6 address pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAwsNetworkPerformanceData": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetAwsNetworkPerformanceData",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get network performance data",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetCapacityReservationUsage": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetCapacityReservationUsage",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:CapacityReservationFleet",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get usage information about a Capacity Reservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation"
-            ]
+            "resources": []
         },
         "GetCoipPoolUsage": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetCoipPoolUsage",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe the allocations from the specified customer-owned address pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "coip-pool"
-            ]
+            "resources": []
         },
         "GetConsoleOutput": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetConsoleOutput",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to get the console output for an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "GetConsoleScreenshot": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetConsoleScreenshot",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NewInstanceProfile",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to retrieve a JPG-format screenshot of a running instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "GetDefaultCreditSpecification": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetDefaultCreditSpecification",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get the default credit option for CPU usage of a burstable performance instance family",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetEbsDefaultKmsKeyId": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetEbsDefaultKmsKeyId",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get the ID of the default customer master key (CMK) for EBS encryption by default",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetEbsEncryptionByDefault": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetEbsEncryptionByDefault",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to describe whether EBS encryption by default is enabled for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetFlowLogsIntegrationTemplate": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetFlowLogsIntegrationTemplate",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to generate a CloudFormation template to streamline the integration of VPC flow logs with Amazon Athena",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-flow-log"
-            ]
+            "resources": []
         },
         "GetGroupsForCapacityReservation": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetGroupsForCapacityReservation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:CapacityReservationFleet",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to list the resource groups to which a Capacity Reservation has been added",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation"
-            ]
+            "resources": []
         },
         "GetHostReservationPurchasePreview": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetHostReservationPurchasePreview",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to preview a reservation purchase with configurations that match those of a Dedicated Host",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetInstanceTypesFromInstanceRequirements": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetInstanceTypesFromInstanceRequirements",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to view a list of instance types with specified instance attributes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetInstanceUefiData": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetInstanceUefiData",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NewInstanceProfile",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to retrieve the binary representation of the UEFI variable store",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "GetIpamAddressHistory": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpamAddressHistory",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to retrieve historical information about a CIDR within an Amazon VPC IP Address Manager (IPAM) scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "GetIpamDiscoveredAccounts": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpamDiscoveredAccounts",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to retrieve IPAM discovered accounts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery"
-            ]
+            "resources": []
         },
         "GetIpamDiscoveredResourceCidrs": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpamDiscoveredResourceCidrs",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to retrieve the resource CIDRs that are monitored as part of a resource discovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery"
-            ]
+            "resources": []
         },
         "GetIpamPoolAllocations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetIpamPoolAllocations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get a list of all the CIDR allocations in an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "GetIpamPoolCidrs": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpamPoolCidrs",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get the CIDRs provisioned to an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "GetIpamResourceCidrs": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetIpamResourceCidrs",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about the resources in an Amazon VPC IP Address Manager (IPAM) scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "GetLaunchTemplateData": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetLaunchTemplateData",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to get the configuration data of the specified instance for use with a new launch template or launch template version",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "GetManagedPrefixListAssociations": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetManagedPrefixListAssociations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about the resources that are associated with the specified managed prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "GetManagedPrefixListEntries": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetManagedPrefixListEntries",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about the entries for a specified managed prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "GetNetworkInsightsAccessScopeAnalysisFindings": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetNetworkInsightsAccessScopeAnalysisFindings",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get the findings for one or more Network Access Scope analyses",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetNetworkInsightsAccessScopeContent": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetNetworkInsightsAccessScopeContent",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get the content for a specified Network Access Scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPasswordData": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetPasswordData",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to retrieve the encrypted administrator password for a running Windows instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "GetReservedInstancesExchangeQuote": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetReservedInstancesExchangeQuote",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to return a quote and exchange information for exchanging one or more Convertible Reserved Instances for a new Convertible Reserved Instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicy": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetResourcePolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to describe an IAM policy that enables cross-account sharing",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "placement-group",
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "GetSerialConsoleAccessStatus": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetSerialConsoleAccessStatus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to retrieve the access status of your account to the EC2 serial console of all instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSpotPlacementScores": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetSpotPlacementScores",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to calculate the Spot placement score for a Region or Availability Zone based on the specified target capacity and compute requirements",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSubnetCidrReservations": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetSubnetCidrReservations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to retrieve information about the subnet CIDR reservations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayAttachmentPropagations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayAttachmentPropagations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to list the route tables to which a resource attachment propagates routes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayMulticastDomainAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about the associations for a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "GetTransitGatewayPolicyTableAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayPolicyTableAssociations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about associations for a transit gateway policy table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "GetTransitGatewayPolicyTableEntries": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayPolicyTableEntries",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to get information about associations for a transit gateway policy table entry",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-policy-table"
-            ]
+            "resources": []
         },
         "GetTransitGatewayPrefixListReferences": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayPrefixListReferences",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get information about prefix list references for a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayRouteTableAssociations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayRouteTableAssociations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get information about associations for a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTransitGatewayRouteTablePropagations": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetTransitGatewayRouteTablePropagations",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to get information about the route table propagations for a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetVerifiedAccessEndpointPolicy": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVerifiedAccessEndpointPolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to show the Verified Access policy associated with the endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-endpoint"
-            ]
+            "resources": []
         },
         "GetVerifiedAccessGroupPolicy": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVerifiedAccessGroupPolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to show the contents of the Verified Access policy associated with the group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "GetVerifiedAccessInstanceWebAcl": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVerifiedAccessInstanceWebAcl",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to show the AWS Web Application Firewall (WAF) web access control list (ACL) for a Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "GetVpnConnectionDeviceSampleConfiguration": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVpnConnectionDeviceSampleConfiguration",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to download an AWS-provided sample configuration file to be used with the customer gateway device",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection",
-                "vpn-connection-device-type"
-            ]
+            "resources": []
         },
         "GetVpnConnectionDeviceTypes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVpnConnectionDeviceTypes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to obtain a list of customer gateway devices for which sample configuration files can be provided",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetVpnTunnelReplacementStatus": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "GetVpnTunnelReplacementStatus",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to view available tunnel endpoint maintenance events",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "ImportByoipCidrToIpam": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportByoipCidrToIpam",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to transfer existing BYOIP IPv4 CIDRs to IPAM",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "ImportClientVpnClientCertificateRevocationList": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportClientVpnClientCertificateRevocationList",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to upload a client certificate revocation list to a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "ImportImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportImage",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to import single or multi-volume disk images or EBS snapshots into an Amazon Machine Image (AMI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "import-image-task",
-                "snapshot"
-            ]
+            "resources": []
         },
         "ImportInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportInstance",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:InstanceID",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:SubnetID",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create an import instance task using metadata from a disk image",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "security-group",
-                "subnet",
-                "volume"
-            ]
+            "resources": []
         },
         "ImportKeyPair": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportKeyPair",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region"
-            ],
-            "description": "Grants permission to import a public key from an RSA key pair that was created with a third-party tool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "key-pair"
-            ]
+            "resources": []
         },
         "ImportSnapshot": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportSnapshot",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to import a disk into an EBS snapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "import-snapshot-task",
-                "snapshot"
-            ]
+            "resources": []
         },
         "ImportVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ImportVolume",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to create an import volume task using metadata from a disk image",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "ListImagesInRecycleBin": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListImagesInRecycleBin",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to list Amazon Machine Images (AMIs) that are currently in the Recycle Bin",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "ListSnapshotsInRecycleBin": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListSnapshotsInRecycleBin",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to list the Amazon EBS snapshots that are currently in the Recycle Bin",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "ModifyAddressAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyAddressAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify an attribute of the specified Elastic IP address",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "ModifyAvailabilityZoneGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyAvailabilityZoneGroup",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to modify the opt-in status of the Local Zone and Wavelength Zone group for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyCapacityReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyCapacityReservation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:CapacityReservationFleet",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a Capacity Reservation's capacity and the conditions under which it is to be released",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation"
-            ]
+            "resources": []
         },
         "ModifyCapacityReservationFleet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyCapacityReservationFleet",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a Capacity Reservation Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation-fleet"
-            ]
+            "resources": []
         },
         "ModifyClientVpnEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyClientVpnEndpoint",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:SecurityGroupID",
-                "ec2:ServerCertificateArn",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to modify a Client VPN endpoint",
-            "orphan": false,
-            "resources": [
-                "client-vpn-endpoint",
-                "security-group",
-                "vpc"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "ModifyDefaultCreditSpecification": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyDefaultCreditSpecification",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to change the account level default credit option for CPU usage of burstable performance instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyEbsDefaultKmsKeyId": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyEbsDefaultKmsKeyId",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to change the default customer master key (CMK) for EBS encryption by default for your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyFleet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyFleet",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:KeyPairName",
-                "ec2:NetworkInterfaceID",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:VolumeSize",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify an EC2 Fleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fleet",
-                "image",
-                "key-pair",
-                "launch-template",
-                "network-interface",
-                "security-group",
-                "snapshot",
-                "subnet"
-            ]
+            "resources": []
         },
         "ModifyFpgaImageAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyFpgaImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify an attribute of an Amazon FPGA Image (AFI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "ModifyHosts": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyHosts",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a Dedicated Host",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dedicated-host"
-            ]
+            "resources": []
         },
         "ModifyIdFormat": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to modify the ID format for a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyIdentityIdFormat": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIdentityIdFormat",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to modify the ID format of a resource for a specific principal in your account",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyImageAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to modify an attribute of an Amazon Machine Image (AMI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "ModifyInstanceAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ParentSnapshot",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify an attribute of an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "security-group",
-                "volume"
-            ]
+            "resources": []
         },
         "ModifyInstanceCapacityReservationAttributes": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceCapacityReservationAttributes",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the Capacity Reservation settings for a stopped instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation",
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyInstanceCreditSpecification": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceCreditSpecification",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the credit option for CPU usage on an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyInstanceEventStartTime": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceEventStartTime",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:InstanceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the start time for a scheduled EC2 instance event",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyInstanceEventWindow": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceEventWindow",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the specified event window",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance-event-window"
-            ]
+            "resources": []
         },
         "ModifyInstanceMaintenanceOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceMaintenanceOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the recovery behaviour for an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyInstanceMetadataOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstanceMetadataOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the metadata options for an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyInstancePlacement": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyInstancePlacement",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the placement attributes for an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dedicated-host",
-                "instance",
-                "placement-group"
-            ]
+            "resources": []
         },
         "ModifyIpam": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIpam",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam"
-            ]
+            "resources": []
         },
         "ModifyIpamPool": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIpamPool",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "ModifyIpamResourceCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIpamResourceCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) resource CIDR",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "ModifyIpamResourceDiscovery": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIpamResourceDiscovery",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a resource discovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-resource-discovery"
-            ]
+            "resources": []
         },
         "ModifyIpamScope": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyIpamScope",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configurations of an Amazon VPC IP Address Manager (IPAM) scope",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-scope"
-            ]
+            "resources": []
         },
         "ModifyLaunchTemplate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyLaunchTemplate",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a launch template",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template"
-            ]
+            "resources": []
         },
         "ModifyLocalGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyLocalGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AuthorizedUser",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Permission",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify a local gateway route",
-            "orphan": false,
-            "resources": [
-                "local-gateway-route-table",
-                "local-gateway-virtual-interface-group",
-                "network-interface",
-                "prefix-list"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "ModifyManagedPrefixList": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyManagedPrefixList",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a managed prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "ModifyNetworkInterfaceAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyNetworkInterfaceAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkInterfaceID",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:Subnet",
-                "ec2:Tenancy",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify an attribute of a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "network-interface",
-                "security-group"
-            ]
+            "resources": []
         },
         "ModifyPrivateDnsNameOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyPrivateDnsNameOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NewInstanceProfile",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify the options for instance hostnames for the specified instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ModifyReservedInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyReservedInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:InstanceType",
-                "ec2:Region",
-                "ec2:ReservedInstancesOfferingType",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to modify attributes of one or more Reserved Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "reserved-instances"
-            ]
+            "resources": []
         },
         "ModifySecurityGroupRules": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifySecurityGroupRules",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify the rules of a security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list",
-                "security-group",
-                "security-group-rule"
-            ]
+            "resources": []
         },
         "ModifySnapshotAttribute": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "ModifySnapshotAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Add/group",
-                "ec2:Add/userId",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:Remove/group",
-                "ec2:Remove/userId",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to add or remove permission settings for a snapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "ModifySnapshotTier": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifySnapshotTier",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to archive Amazon EBS snapshots",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "ModifySpotFleetRequest": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifySpotFleetRequest",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify a Spot Fleet request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "launch-template",
-                "spot-fleet-request",
-                "subnet"
-            ]
+            "resources": []
         },
         "ModifySubnetAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifySubnetAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify an attribute of a subnet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet"
-            ]
+            "resources": []
         },
         "ModifyTrafficMirrorFilterNetworkServices": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTrafficMirrorFilterNetworkServices",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to allow or restrict mirroring network services",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter"
-            ]
+            "resources": []
         },
         "ModifyTrafficMirrorFilterRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTrafficMirrorFilterRule",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a traffic mirror rule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter",
-                "traffic-mirror-filter-rule"
-            ]
+            "resources": []
         },
         "ModifyTrafficMirrorSession": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTrafficMirrorSession",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a traffic mirror session",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "traffic-mirror-filter",
-                "traffic-mirror-session",
-                "traffic-mirror-target"
-            ]
+            "resources": []
         },
         "ModifyTransitGateway": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTransitGateway",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "ModifyTransitGatewayPrefixListReference": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTransitGatewayPrefixListReference",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a transit gateway prefix list reference",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list",
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "ModifyTransitGatewayVpcAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTransitGatewayVpcAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID"
-            ],
-            "description": "Grants permission to modify a VPC attachment on a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessEndpoint",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to modify the configuration of a Verified Access endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "subnet",
-                "verified-access-endpoint",
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessEndpointPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessEndpointPolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the specified Verified Access endpoint policy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-endpoint"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessGroup",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the specified Verified Access Group configuration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-group",
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessGroupPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessGroupPolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the specified Verified Access group policy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessInstance": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessInstance",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configuration of the specified Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessInstanceLoggingConfiguration": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessInstanceLoggingConfiguration",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the logging configuration for the specified Verified Access instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-instance"
-            ]
+            "resources": []
         },
         "ModifyVerifiedAccessTrustProvider": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVerifiedAccessTrustProvider",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the configuration of the specified Verified Access trust provider",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "verified-access-trust-provider"
-            ]
+            "resources": []
         },
         "ModifyVolume": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVolume",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to modify the parameters of an EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "ModifyVolumeAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVolumeAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AvailabilityZone",
-                "ec2:Encrypted",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to modify an attribute of a volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "volume"
-            ]
+            "resources": []
         },
         "ModifyVpcAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to modify an attribute of a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "ModifyVpcEndpoint": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcEndpoint",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:SecurityGroupID",
-                "ec2:SubnetID"
-            ],
-            "description": "Grants permission to modify an attribute of a VPC endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table",
-                "security-group",
-                "subnet",
-                "vpc-endpoint"
-            ]
+            "resources": []
         },
         "ModifyVpcEndpointConnectionNotification": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcEndpointConnectionNotification",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify a connection notification for a VPC endpoint or VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint",
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "ModifyVpcEndpointServiceConfiguration": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcEndpointServiceConfiguration",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpceServicePrivateDnsName"
-            ],
-            "description": "Grants permission to modify the attributes of a VPC endpoint service configuration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "ModifyVpcEndpointServicePayerResponsibility": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcEndpointServicePayerResponsibility",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the payer responsibility for a VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "ModifyVpcEndpointServicePermissions": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "ModifyVpcEndpointServicePermissions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the permissions for a VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "ModifyVpcPeeringConnectionOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcPeeringConnectionOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AccepterVpc",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to modify the VPC peering connection options on one side of a VPC peering connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-peering-connection"
-            ]
+            "resources": []
         },
         "ModifyVpcTenancy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpcTenancy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Tenancy",
-                "ec2:VpcID"
-            ],
-            "description": "Grants permission to modify the instance tenancy attribute of a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc"
-            ]
+            "resources": []
         },
         "ModifyVpnConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpnConnection",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AuthenticationType",
-                "ec2:DPDTimeoutSeconds",
-                "ec2:GatewayType",
-                "ec2:IKEVersions",
-                "ec2:InsideTunnelCidr",
-                "ec2:InsideTunnelIpv6Cidr",
-                "ec2:Phase1DHGroup",
-                "ec2:Phase1EncryptionAlgorithms",
-                "ec2:Phase1IntegrityAlgorithms",
-                "ec2:Phase1LifetimeSeconds",
-                "ec2:Phase2DHGroup",
-                "ec2:Phase2EncryptionAlgorithms",
-                "ec2:Phase2IntegrityAlgorithms",
-                "ec2:Phase2LifetimeSeconds",
-                "ec2:PreSharedKeys",
-                "ec2:Region",
-                "ec2:RekeyFuzzPercentage",
-                "ec2:RekeyMarginTimeSeconds",
-                "ec2:ReplayWindowSizePackets",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RoutingType"
-            ],
-            "description": "Grants permission to modify the target gateway of a Site-to-Site VPN connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "ModifyVpnConnectionOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpnConnectionOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the connection options for your Site-to-Site VPN connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "ModifyVpnTunnelCertificate": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpnTunnelCertificate",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to modify the certificate for a Site-to-Site VPN connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "ModifyVpnTunnelOptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyVpnTunnelOptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:AuthenticationType",
-                "ec2:DPDTimeoutSeconds",
-                "ec2:GatewayType",
-                "ec2:IKEVersions",
-                "ec2:InsideTunnelCidr",
-                "ec2:InsideTunnelIpv6Cidr",
-                "ec2:Phase1DHGroup",
-                "ec2:Phase1EncryptionAlgorithms",
-                "ec2:Phase1IntegrityAlgorithms",
-                "ec2:Phase1LifetimeSeconds",
-                "ec2:Phase2DHGroup",
-                "ec2:Phase2EncryptionAlgorithms",
-                "ec2:Phase2IntegrityAlgorithms",
-                "ec2:Phase2LifetimeSeconds",
-                "ec2:PreSharedKeys",
-                "ec2:Region",
-                "ec2:RekeyFuzzPercentage",
-                "ec2:RekeyMarginTimeSeconds",
-                "ec2:ReplayWindowSizePackets",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RoutingType"
-            ],
-            "description": "Grants permission to modify the options for a Site-to-Site VPN connection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "MonitorInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "MonitorInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to enable detailed monitoring for a running instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "MoveAddressToVpc": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "MoveAddressToVpc",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to move an Elastic IP address from the EC2-Classic platform to the EC2-VPC platform",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "MoveByoipCidrToIpam": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "MoveByoipCidrToIpam",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to move a BYOIP IPv4 CIDR to Amazon VPC IP Address Manager (IPAM) from a public IPv4 pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "PauseVolumeIO": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PauseVolumeIO",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:Encrypted",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ParentSnapshot",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType"
-            ],
-            "description": "Grants permission to temporarily pause I/O operations for a target Amazon EBS volume",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "volume"
-            ]
+            "resources": []
         },
         "ProvisionByoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ProvisionByoipCidr",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to provision an address range for use in AWS through bring your own IP addresses (BYOIP), and to create a corresponding address pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ProvisionIpamPoolCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ProvisionIpamPoolCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to provision a CIDR to an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "ProvisionPublicIpv4PoolCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ProvisionPublicIpv4PoolCidr",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to provision a CIDR to a public IPv4 pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "ipv4pool-ec2"
-            ]
+            "resources": []
         },
         "PurchaseHostReservation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PurchaseHostReservation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to purchase a reservation with configurations that match those of a Dedicated Host",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dedicated-host"
-            ]
+            "resources": []
         },
         "PurchaseReservedInstancesOffering": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PurchaseReservedInstancesOffering",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to purchase a Reserved Instance offering",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PurchaseScheduledInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PurchaseScheduledInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to purchase one or more Scheduled Instances with a specified schedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutResourcePolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PutResourcePolicy",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to attach an IAM policy that enables cross-account sharing to a resource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool",
-                "placement-group",
-                "verified-access-group"
-            ]
+            "resources": []
         },
         "RebootInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RebootInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to request a reboot of one or more instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "RegisterImage": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterImage",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to register an Amazon Machine Image (AMI)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "snapshot"
-            ]
+            "resources": []
         },
         "RegisterInstanceEventNotificationAttributes": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterInstanceEventNotificationAttributes",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to add tags to the set of tags to include in notifications about scheduled events for your instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RegisterTransitGatewayMulticastGroupMembers": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterTransitGatewayMulticastGroupMembers",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to register one or more network interfaces as a member of a group IP address in a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "RegisterTransitGatewayMulticastGroupSources": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterTransitGatewayMulticastGroupSources",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to register one or more network interfaces as a source of a group IP address in a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "RejectTransitGatewayMulticastDomainAssociations": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectTransitGatewayMulticastDomainAssociations",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reject requests to associate cross-account subnets with a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "RejectTransitGatewayPeeringAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectTransitGatewayPeeringAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reject a transit gateway peering attachment request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "RejectTransitGatewayVpcAttachment": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectTransitGatewayVpcAttachment",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reject a request to attach a VPC to a transit gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment"
-            ]
+            "resources": []
         },
         "RejectVpcEndpointConnections": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectVpcEndpointConnections",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reject one or more VPC endpoint connection requests to a VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "RejectVpcPeeringConnection": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectVpcPeeringConnection",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AccepterVpc",
-                "ec2:Region",
-                "ec2:RequesterVpc",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:VpcPeeringConnectionID"
-            ],
-            "description": "Grants permission to reject a VPC peering connection request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-peering-connection"
-            ]
+            "resources": []
         },
         "ReleaseAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReleaseAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to release an Elastic IP address",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "ReleaseHosts": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReleaseHosts",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to release one or more On-Demand Dedicated Hosts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "dedicated-host"
-            ]
+            "resources": []
         },
         "ReleaseIpamPoolAllocation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReleaseIpamPoolAllocation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to release an allocation within an Amazon VPC IP Address Manager (IPAM) pool",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "ipam-pool"
-            ]
+            "resources": []
         },
         "ReplaceIamInstanceProfileAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceIamInstanceProfileAssociation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NewInstanceProfile",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to replace an IAM instance profile for an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ReplaceNetworkAclAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceNetworkAclAssociation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to change which network ACL a subnet is associated with",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl",
-                "subnet"
-            ]
+            "resources": []
         },
         "ReplaceNetworkAclEntry": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceNetworkAclEntry",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:NetworkAclID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to replace an entry (rule) in a network ACL",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-acl"
-            ]
+            "resources": []
         },
         "ReplaceRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to replace a route within a route table in a VPC",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "route-table"
-            ]
+            "resources": []
         },
         "ReplaceRouteTableAssociation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceRouteTableAssociation",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:InternetGatewayID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RouteTableID",
-                "ec2:SubnetID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to change the route table that is associated with a subnet",
-            "orphan": false,
-            "resources": [
-                "internet-gateway",
-                "ipv4pool-ec2",
-                "ipv6pool-ec2",
-                "route-table",
-                "subnet"
-            ]
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         },
         "ReplaceTransitGatewayRoute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceTransitGatewayRoute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to replace a route in a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-attachment",
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "ReplaceVpnTunnel": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReplaceVpnTunnel",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to replace a VPN tunnel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpn-connection"
-            ]
+            "resources": []
         },
         "ReportInstanceStatus": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ReportInstanceStatus",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to submit feedback about the status of an instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RequestSpotFleet": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RequestSpotFleet",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
-                "ec2:SubnetID",
-                "ec2:VolumeSize",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a Spot Fleet request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "key-pair",
-                "launch-template",
-                "placement-group",
-                "security-group",
-                "snapshot",
-                "spot-fleet-request",
-                "subnet"
-            ]
+            "resources": []
         },
         "RequestSpotInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RequestSpotInstances",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AuthorizedUser",
-                "ec2:AvailabilityZone",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:NetworkInterfaceID",
-                "ec2:OutpostArn",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Permission",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:SourceOutpostArn",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:VolumeSize",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to create a Spot Instance request",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image",
-                "key-pair",
-                "network-interface",
-                "placement-group",
-                "security-group",
-                "snapshot",
-                "spot-instances-request",
-                "subnet"
-            ]
+            "resources": []
         },
         "ResetAddressAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetAddressAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reset the attribute of the specified IP address",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "ResetEbsDefaultKmsKeyId": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetEbsDefaultKmsKeyId",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to reset the default customer master key (CMK) for EBS encryption for your account to use the AWS-managed CMK for EBS",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ResetFpgaImageAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetFpgaImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to reset an attribute of an Amazon FPGA Image (AFI) to its default value",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "fpga-image"
-            ]
+            "resources": []
         },
         "ResetImageAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetImageAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to reset an attribute of an Amazon Machine Image (AMI) to its default value",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "ResetInstanceAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetInstanceAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to reset an attribute of an instance to its default value",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "ResetNetworkInterfaceAttribute": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ResetNetworkInterfaceAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to reset an attribute of a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "ResetSnapshotAttribute": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "ResetSnapshotAttribute",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Attribute",
-                "ec2:Attribute/${AttributeName}",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to reset permission settings for a snapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "RestoreAddressToClassic": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RestoreAddressToClassic",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to restore an Elastic IP address that was previously moved to the EC2-VPC platform back to the EC2-Classic platform",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RestoreImageFromRecycleBin": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RestoreImageFromRecycleBin",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:Owner",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType"
-            ],
-            "description": "Grants permission to restore an Amazon Machine Image (AMI) from the Recycle Bin",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "image"
-            ]
+            "resources": []
         },
         "RestoreManagedPrefixListVersion": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RestoreManagedPrefixListVersion",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to restore the entries from a previous version of a managed prefix list to a new version of the prefix list",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "prefix-list"
-            ]
+            "resources": []
         },
         "RestoreSnapshotFromRecycleBin": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RestoreSnapshotFromRecycleBin",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to restore an Amazon EBS snapshot from the Recycle Bin",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "RestoreSnapshotTier": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RestoreSnapshotTier",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Encrypted",
-                "ec2:Owner",
-                "ec2:ParentVolume",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:VolumeSize"
-            ],
-            "description": "Grants permission to restore an archived Amazon EBS snapshot for use temporarily or permanently, or modify the restore period or restore type for a snapshot that was previously temporarily restored",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "snapshot"
-            ]
+            "resources": []
         },
         "RevokeClientVpnIngress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RevokeClientVpnIngress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to remove an inbound authorization rule from a Client VPN endpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "RevokeSecurityGroupEgress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RevokeSecurityGroupEgress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to remove one or more outbound rules from a VPC security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group"
-            ]
+            "resources": []
         },
         "RevokeSecurityGroupIngress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RevokeSecurityGroupIngress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to remove one or more inbound rules from a security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group"
-            ]
+            "resources": []
         },
         "RunInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RunInstances",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:AssociatePublicIpAddress",
-                "ec2:AuthorizedService",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:ElasticGpuType",
-                "ec2:Encrypted",
-                "ec2:ImageID",
-                "ec2:ImageType",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:IsLaunchTemplateResource",
-                "ec2:KeyPairName",
-                "ec2:KeyPairType",
-                "ec2:LaunchTemplate",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:NetworkInterfaceID",
-                "ec2:Owner",
-                "ec2:ParentSnapshot",
-                "ec2:ParentVolume",
-                "ec2:PlacementGroup",
-                "ec2:PlacementGroupName",
-                "ec2:PlacementGroupStrategy",
-                "ec2:ProductCode",
-                "ec2:Public",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:SecurityGroupID",
-                "ec2:SnapshotID",
-                "ec2:SnapshotTime",
-                "ec2:Subnet",
-                "ec2:SubnetID",
-                "ec2:Tenancy",
-                "ec2:VolumeID",
-                "ec2:VolumeIops",
-                "ec2:VolumeSize",
-                "ec2:VolumeThroughput",
-                "ec2:VolumeType",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to launch one or more instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "capacity-reservation",
-                "elastic-gpu",
-                "elastic-inference",
-                "group",
-                "image",
-                "instance",
-                "key-pair",
-                "launch-template",
-                "license-configuration",
-                "network-interface",
-                "placement-group",
-                "security-group",
-                "snapshot",
-                "subnet",
-                "volume"
-            ]
+            "resources": []
         },
         "RunScheduledInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RunScheduledInstances",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to launch one or more Scheduled Instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SearchLocalGatewayRoutes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "SearchLocalGatewayRoutes",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to search for routes in a local gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "local-gateway-route-table"
-            ]
+            "resources": []
         },
         "SearchTransitGatewayMulticastGroups": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "SearchTransitGatewayMulticastGroups",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to search for groups, sources, and members in a transit gateway multicast domain",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-multicast-domain"
-            ]
+            "resources": []
         },
         "SearchTransitGatewayRoutes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "SearchTransitGatewayRoutes",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to search for routes in a transit gateway route table",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "transit-gateway-route-table"
-            ]
+            "resources": []
         },
         "SendDiagnosticInterrupt": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SendDiagnosticInterrupt",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to send a diagnostic interrupt to an Amazon EC2 instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "SendSpotInstanceInterruptions": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SendSpotInstanceInterruptions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to interrupt a Spot Instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "StartInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to start a stopped instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance",
-                "license-configuration"
-            ]
+            "resources": []
         },
         "StartNetworkInsightsAccessScopeAnalysis": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartNetworkInsightsAccessScopeAnalysis",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to start a Network Access Scope analysis",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-access-scope",
-                "network-insights-access-scope-analysis"
-            ]
+            "resources": []
         },
         "StartNetworkInsightsAnalysis": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartNetworkInsightsAnalysis",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to start analyzing a specified path",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-insights-analysis",
-                "network-insights-path"
-            ]
+            "resources": []
         },
         "StartVpcEndpointServicePrivateDnsVerification": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartVpcEndpointServicePrivateDnsVerification",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to start the private DNS verification process for a VPC endpoint service",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "vpc-endpoint-service"
-            ]
+            "resources": []
         },
         "StopInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StopInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to stop an Amazon EBS-backed instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "TerminateClientVpnConnections": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "TerminateClientVpnConnections",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ClientRootCertificateChainArn",
-                "ec2:CloudwatchLogGroupArn",
-                "ec2:CloudwatchLogStreamArn",
-                "ec2:DirectoryArn",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SamlProviderArn",
-                "ec2:ServerCertificateArn"
-            ],
-            "description": "Grants permission to terminate active Client VPN endpoint connections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "client-vpn-endpoint"
-            ]
+            "resources": []
         },
         "TerminateInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "TerminateInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to shut down one or more instances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "UnassignIpv6Addresses": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UnassignIpv6Addresses",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to unassign one or more IPv6 addresses from a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "UnassignPrivateIpAddresses": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UnassignPrivateIpAddresses",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:NetworkInterfaceID",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:Subnet",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to unassign one or more secondary private IP addresses from a network interface",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "network-interface"
-            ]
+            "resources": []
         },
         "UnassignPrivateNatGatewayAddress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UnassignPrivateNatGatewayAddress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
-            ],
-            "description": "Grants permission to unassign secondary private IPv4 addresses from a private NAT gateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "natgateway"
-            ]
+            "resources": []
         },
         "UnmonitorInstances": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UnmonitorInstances",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AvailabilityZone",
-                "ec2:EbsOptimized",
-                "ec2:InstanceAutoRecovery",
-                "ec2:InstanceID",
-                "ec2:InstanceMarketType",
-                "ec2:InstanceMetadataTags",
-                "ec2:InstanceProfile",
-                "ec2:InstanceType",
-                "ec2:MetadataHttpEndpoint",
-                "ec2:MetadataHttpPutResponseHopLimit",
-                "ec2:MetadataHttpTokens",
-                "ec2:PlacementGroup",
-                "ec2:ProductCode",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:RootDeviceType",
-                "ec2:Tenancy"
-            ],
-            "description": "Grants permission to disable detailed monitoring for a running instance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "instance"
-            ]
+            "resources": []
         },
         "UpdateSecurityGroupRuleDescriptionsEgress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateSecurityGroupRuleDescriptionsEgress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to update descriptions for one or more outbound rules in a VPC security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group"
-            ]
+            "resources": []
         },
         "UpdateSecurityGroupRuleDescriptionsIngress": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateSecurityGroupRuleDescriptionsIngress",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:SecurityGroupID",
-                "ec2:Vpc"
-            ],
-            "description": "Grants permission to update descriptions for one or more inbound rules in a security group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "security-group"
-            ]
+            "resources": []
         },
         "WithdrawByoipCidr": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "WithdrawByoipCidr",
-            "condition_keys": [
-                "ec2:Region"
-            ],
-            "description": "Grants permission to stop advertising an address range that was provisioned for use in AWS through bring your own IP addresses (BYOIP)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "ec2-instance-connect": {
         "SendSSHPublicKey": {
             "access_level": "Write",
@@ -148578,14 +143502,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete a WebACL",
             "orphan": false,
             "resources": [
                 "webacl"
             ]
         },
+        "DescribeAllManagedProducts": {
+            "access_level": "Undocumented",
+            "action": "DescribeAllManagedProducts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeManagedProductsByVendor": {
+            "access_level": "Undocumented",
+            "action": "DescribeManagedProductsByVendor",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeManagedRuleGroup": {
             "access_level": "Read",
             "action": "DescribeManagedRuleGroup",
             "condition_keys": [],
             "description": "Grants permission to retrieve high-level information for a managed rule group",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230606/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230606/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/generate.py` & `iam_actions-1.2.20230606/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230606/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230606/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/generate/services.py` & `iam_actions-1.2.20230606/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230605/iam_actions/policies.json` & `iam_actions-1.2.20230606/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994702007202008%*

 * *Differences: {"'serviceMap'": "{'AWS WAF V2': {'Actions': {insert: [(14, 'DescribeAllManagedProducts'), (15, "*

 * *                 "'DescribeManagedProductsByVendor')]}}, 'AWS Key Management Service': "*

 * *                 "{'conditionKeys': {insert: [(31, "*

 * *                 "'kms:ScheduleKeyDeletionPendingWindowInDays')]}}, 'Amazon Elastic Compute Cloud "*

 * *                 "(EC2)': OrderedDict([('StringPrefix', 'ec2'), ('Actions', "*

 * *                 "['AcceptAddressTransfer', 'AcceptReservedInstancesExchangeQuote', "*

 * *         […]*

```diff
@@ -6022,14 +6022,15 @@
                 "kms:ReEncryptOnSameKey",
                 "kms:RecipientAttestation:ImageSha384",
                 "kms:RecipientAttestation:PCR",
                 "kms:ReplicaRegion",
                 "kms:RequestAlias",
                 "kms:ResourceAliases",
                 "kms:RetiringPrincipal",
+                "kms:ScheduleKeyDeletionPendingWindowInDays",
                 "kms:SigningAlgorithm",
                 "kms:ValidTo",
                 "kms:ViaService",
                 "kms:WrappingAlgorithm",
                 "kms:WrappingKeySpec"
             ]
         },
@@ -9329,14 +9330,16 @@
                 "DeleteFirewallManagerRuleGroups",
                 "DeleteIPSet",
                 "DeleteLoggingConfiguration",
                 "DeletePermissionPolicy",
                 "DeleteRegexPatternSet",
                 "DeleteRuleGroup",
                 "DeleteWebACL",
+                "DescribeAllManagedProducts",
+                "DescribeManagedProductsByVendor",
                 "DescribeManagedRuleGroup",
                 "DisassociateFirewallManager",
                 "DisassociateWebACL",
                 "GenerateMobileSdkReleaseUrl",
                 "GetDecryptedAPIKey",
                 "GetIPSet",
                 "GetLoggingConfiguration",
@@ -12040,15 +12043,376 @@
             ],
             "HasResource": true,
             "StringPrefix": "dax",
             "conditionKeys": [
                 "dax:EnclosingOperation"
             ]
         },
-        "Amazon EC2": {
+        "Amazon EC2 Auto Scaling": {
+            "ARNFormat": "arn:aws:autoscaling:${Region}:${Account}:${RelativeId}",
+            "ARNRegex": "^arn:aws:autoscaling:.+:.+:.+",
+            "Actions": [
+                "AttachInstances",
+                "AttachLoadBalancerTargetGroups",
+                "AttachLoadBalancers",
+                "AttachTrafficSources",
+                "BatchDeleteScheduledAction",
+                "BatchPutScheduledUpdateGroupAction",
+                "CancelInstanceRefresh",
+                "CompleteLifecycleAction",
+                "CreateAutoScalingGroup",
+                "CreateLaunchConfiguration",
+                "CreateOrUpdateTags",
+                "DeleteAutoScalingGroup",
+                "DeleteLaunchConfiguration",
+                "DeleteLifecycleHook",
+                "DeleteNotificationConfiguration",
+                "DeletePolicy",
+                "DeleteScheduledAction",
+                "DeleteTags",
+                "DeleteWarmPool",
+                "DescribeAccountLimits",
+                "DescribeAdjustmentTypes",
+                "DescribeAutoScalingGroups",
+                "DescribeAutoScalingInstances",
+                "DescribeAutoScalingNotificationTypes",
+                "DescribeInstanceRefreshes",
+                "DescribeLaunchConfigurations",
+                "DescribeLifecycleHookTypes",
+                "DescribeLifecycleHooks",
+                "DescribeLoadBalancerTargetGroups",
+                "DescribeLoadBalancers",
+                "DescribeMetricCollectionTypes",
+                "DescribeNotificationConfigurations",
+                "DescribePolicies",
+                "DescribeScalingActivities",
+                "DescribeScalingProcessTypes",
+                "DescribeScheduledActions",
+                "DescribeTags",
+                "DescribeTerminationPolicyTypes",
+                "DescribeTrafficSources",
+                "DescribeWarmPool",
+                "DetachInstances",
+                "DetachLoadBalancerTargetGroups",
+                "DetachLoadBalancers",
+                "DetachTrafficSources",
+                "DisableMetricsCollection",
+                "EnableMetricsCollection",
+                "EnterStandby",
+                "ExecutePolicy",
+                "ExitStandby",
+                "GetPredictiveScalingForecast",
+                "PutLifecycleHook",
+                "PutNotificationConfiguration",
+                "PutScalingPolicy",
+                "PutScheduledUpdateGroupAction",
+                "PutWarmPool",
+                "RecordLifecycleActionHeartbeat",
+                "ResumeProcesses",
+                "RollbackInstanceRefresh",
+                "SetDesiredCapacity",
+                "SetInstanceHealth",
+                "SetInstanceProtection",
+                "StartInstanceRefresh",
+                "SuspendProcesses",
+                "TerminateInstanceInAutoScalingGroup",
+                "UpdateAutoScalingGroup"
+            ],
+            "HasResource": true,
+            "StringPrefix": "autoscaling",
+            "conditionKeys": [
+                "autoscaling:ImageId",
+                "autoscaling:InstanceType",
+                "autoscaling:InstanceTypes",
+                "autoscaling:LaunchConfigurationName",
+                "autoscaling:LaunchTemplateVersionSpecified",
+                "autoscaling:LoadBalancerNames",
+                "autoscaling:MaxSize",
+                "autoscaling:MetadataHttpEndpoint",
+                "autoscaling:MetadataHttpPutResponseHopLimit",
+                "autoscaling:MetadataHttpTokens",
+                "autoscaling:MinSize",
+                "autoscaling:ResourceTag/${TagKey}",
+                "autoscaling:SpotPrice",
+                "autoscaling:TargetGroupARNs",
+                "autoscaling:TrafficSourceIdentifiers",
+                "autoscaling:VPCZoneIdentifiers",
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
+        "Amazon EC2 Image Builder": {
+            "ARNFormat": "arn:aws:imagebuilder:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:imagebuilder:.+:.+:.+",
+            "Actions": [
+                "CancelImageCreation",
+                "CreateComponent",
+                "CreateContainerRecipe",
+                "CreateDistributionConfiguration",
+                "CreateImage",
+                "CreateImagePipeline",
+                "CreateImageRecipe",
+                "CreateInfrastructureConfiguration",
+                "DeleteComponent",
+                "DeleteContainerRecipe",
+                "DeleteDistributionConfiguration",
+                "DeleteImage",
+                "DeleteImagePipeline",
+                "DeleteImageRecipe",
+                "DeleteInfrastructureConfiguration",
+                "GetComponent",
+                "GetComponentPolicy",
+                "GetContainerRecipe",
+                "GetContainerRecipePolicy",
+                "GetDistributionConfiguration",
+                "GetImage",
+                "GetImagePipeline",
+                "GetImagePolicy",
+                "GetImageRecipe",
+                "GetImageRecipePolicy",
+                "GetInfrastructureConfiguration",
+                "GetWorkflowExecution",
+                "GetWorkflowStepExecution",
+                "ImportComponent",
+                "ImportVmImage",
+                "ListComponentBuildVersions",
+                "ListComponents",
+                "ListContainerRecipes",
+                "ListDistributionConfigurations",
+                "ListImageBuildVersions",
+                "ListImagePackages",
+                "ListImagePipelineImages",
+                "ListImagePipelines",
+                "ListImageRecipes",
+                "ListImageScanFindingAggregations",
+                "ListImageScanFindings",
+                "ListImages",
+                "ListInfrastructureConfigurations",
+                "ListTagsForResource",
+                "ListWorkflowExecutions",
+                "ListWorkflowStepExecutions",
+                "PutComponentPolicy",
+                "PutContainerRecipePolicy",
+                "PutImagePolicy",
+                "PutImageRecipePolicy",
+                "StartImagePipelineExecution",
+                "TagResource",
+                "UntagResource",
+                "UpdateDistributionConfiguration",
+                "UpdateImagePipeline",
+                "UpdateInfrastructureConfiguration"
+            ],
+            "HasResource": true,
+            "StringPrefix": "imagebuilder",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "imagebuilder:CreatedResourceTag/<key>",
+                "imagebuilder:CreatedResourceTagKeys",
+                "imagebuilder:Ec2MetadataHttpTokens",
+                "imagebuilder:StatusTopicArn"
+            ]
+        },
+        "Amazon EC2 Instance Connect": {
+            "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:ec2:.+",
+            "Actions": [
+                "SendSSHPublicKey",
+                "SendSerialConsoleSSHPublicKey"
+            ],
+            "HasResource": true,
+            "StringPrefix": "ec2-instance-connect",
+            "conditionKeys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:osuser"
+            ]
+        },
+        "Amazon EMR Serverless": {
+            "ARNFormat": "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:emr-serverless:.+",
+            "Actions": [
+                "CancelJobRun",
+                "CreateApplication",
+                "DeleteApplication",
+                "GetApplication",
+                "GetDashboardForJobRun",
+                "GetJobRun",
+                "ListApplications",
+                "ListJobRuns",
+                "ListTagsForResource",
+                "StartApplication",
+                "StartJobRun",
+                "StopApplication",
+                "TagResource",
+                "UntagResource",
+                "UpdateApplication"
+            ],
+            "HasResource": true,
+            "StringPrefix": "emr-serverless",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
+        "Amazon EMR on EKS (EMR Containers)": {
+            "ARNFormat": "arn:aws:emr-containers:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:emr-containers:.+",
+            "Actions": [
+                "CancelJobRun",
+                "CreateJobTemplate",
+                "CreateManagedEndpoint",
+                "CreateVirtualCluster",
+                "DeleteJobTemplate",
+                "DeleteManagedEndpoint",
+                "DeleteVirtualCluster",
+                "DescribeJobRun",
+                "DescribeJobTemplate",
+                "DescribeManagedEndpoint",
+                "DescribeVirtualCluster",
+                "GetManagedEndpointSessionCredentials",
+                "ListJobRuns",
+                "ListJobTemplates",
+                "ListManagedEndpoints",
+                "ListTagsForResource",
+                "ListVirtualClusters",
+                "StartJobRun",
+                "TagResource",
+                "UntagResource"
+            ],
+            "HasResource": true,
+            "StringPrefix": "emr-containers",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "emr-containers:ExecutionRoleArn",
+                "emr-containers:JobTemplateArn"
+            ]
+        },
+        "Amazon ElastiCache": {
+            "ARNFormat": "arn:aws:elasticache:${Region}:${Account}:${ResourceType}:${ResourceName}",
+            "ARNRegex": "^arn:aws:elasticache:.+:.+:.+",
+            "Actions": [
+                "AddTagsToResource",
+                "AuthorizeCacheSecurityGroupIngress",
+                "BatchApplyUpdateAction",
+                "BatchStopUpdateAction",
+                "CompleteMigration",
+                "Connect",
+                "CopySnapshot",
+                "CreateCacheCluster",
+                "CreateCacheParameterGroup",
+                "CreateCacheSecurityGroup",
+                "CreateCacheSubnetGroup",
+                "CreateGlobalReplicationGroup",
+                "CreateReplicationGroup",
+                "CreateSnapshot",
+                "CreateUser",
+                "CreateUserGroup",
+                "DecreaseNodeGroupsInGlobalReplicationGroup",
+                "DecreaseReplicaCount",
+                "DeleteCacheCluster",
+                "DeleteCacheParameterGroup",
+                "DeleteCacheSecurityGroup",
+                "DeleteCacheSubnetGroup",
+                "DeleteGlobalReplicationGroup",
+                "DeleteReplicationGroup",
+                "DeleteSnapshot",
+                "DeleteUser",
+                "DeleteUserGroup",
+                "DescribeCacheClusters",
+                "DescribeCacheEngineVersions",
+                "DescribeCacheParameterGroups",
+                "DescribeCacheParameters",
+                "DescribeCacheSecurityGroups",
+                "DescribeCacheSubnetGroups",
+                "DescribeEngineDefaultParameters",
+                "DescribeEvents",
+                "DescribeGlobalReplicationGroups",
+                "DescribeReplicationGroups",
+                "DescribeReservedCacheNodes",
+                "DescribeReservedCacheNodesOfferings",
+                "DescribeServiceUpdates",
+                "DescribeSnapshots",
+                "DescribeUpdateActions",
+                "DescribeUserGroups",
+                "DescribeUsers",
+                "DisassociateGlobalReplicationGroup",
+                "FailoverGlobalReplicationGroup",
+                "IncreaseNodeGroupsInGlobalReplicationGroup",
+                "IncreaseReplicaCount",
+                "ListAllowedNodeTypeModifications",
+                "ListTagsForResource",
+                "ModifyCacheCluster",
+                "ModifyCacheParameterGroup",
+                "ModifyCacheSubnetGroup",
+                "ModifyGlobalReplicationGroup",
+                "ModifyReplicationGroup",
+                "ModifyReplicationGroupShardConfiguration",
+                "ModifyUser",
+                "ModifyUserGroup",
+                "PurchaseReservedCacheNodesOffering",
+                "RebalanceSlotsInGlobalReplicationGroup",
+                "RebootCacheCluster",
+                "RemoveTagsFromResource",
+                "ResetCacheParameterGroup",
+                "RevokeCacheSecurityGroupIngress",
+                "StartMigration",
+                "TestFailover"
+            ],
+            "HasResource": true,
+            "StringPrefix": "elasticache",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticache:AtRestEncryptionEnabled",
+                "elasticache:AuthTokenEnabled",
+                "elasticache:AutomaticFailoverEnabled",
+                "elasticache:CacheNodeType",
+                "elasticache:CacheParameterGroupName",
+                "elasticache:ClusterModeEnabled",
+                "elasticache:EngineType",
+                "elasticache:EngineVersion",
+                "elasticache:KmsKeyId",
+                "elasticache:MultiAZEnabled",
+                "elasticache:NumNodeGroups",
+                "elasticache:ReplicasPerNodeGroup",
+                "elasticache:SnapshotRetentionLimit",
+                "elasticache:TransitEncryptionEnabled",
+                "elasticache:UserAuthenticationMode"
+            ]
+        },
+        "Amazon Elastic Block Store": {
+            "ARNFormat": "arn:aws:ebs:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:ebs:.+",
+            "Actions": [
+                "CompleteSnapshot",
+                "GetSnapshotBlock",
+                "ListChangedBlocks",
+                "ListSnapshotBlocks",
+                "PutSnapshotBlock",
+                "StartSnapshot"
+            ],
+            "HasResource": true,
+            "StringPrefix": "ebs",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ebs:Description",
+                "ebs:ParentSnapshot",
+                "ebs:VolumeSize"
+            ]
+        },
+        "Amazon Elastic Compute Cloud (EC2)": {
             "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:ec2:.+",
             "Actions": [
                 "AcceptAddressTransfer",
                 "AcceptReservedInstancesExchangeQuote",
                 "AcceptTransitGatewayMulticastDomainAssociations",
                 "AcceptTransitGatewayPeeringAttachment",
@@ -12765,375 +13129,14 @@
                 "ec2:VpcID",
                 "ec2:VpcPeeringConnectionID",
                 "ec2:VpceServiceName",
                 "ec2:VpceServiceOwner",
                 "ec2:VpceServicePrivateDnsName"
             ]
         },
-        "Amazon EC2 Auto Scaling": {
-            "ARNFormat": "arn:aws:autoscaling:${Region}:${Account}:${RelativeId}",
-            "ARNRegex": "^arn:aws:autoscaling:.+:.+:.+",
-            "Actions": [
-                "AttachInstances",
-                "AttachLoadBalancerTargetGroups",
-                "AttachLoadBalancers",
-                "AttachTrafficSources",
-                "BatchDeleteScheduledAction",
-                "BatchPutScheduledUpdateGroupAction",
-                "CancelInstanceRefresh",
-                "CompleteLifecycleAction",
-                "CreateAutoScalingGroup",
-                "CreateLaunchConfiguration",
-                "CreateOrUpdateTags",
-                "DeleteAutoScalingGroup",
-                "DeleteLaunchConfiguration",
-                "DeleteLifecycleHook",
-                "DeleteNotificationConfiguration",
-                "DeletePolicy",
-                "DeleteScheduledAction",
-                "DeleteTags",
-                "DeleteWarmPool",
-                "DescribeAccountLimits",
-                "DescribeAdjustmentTypes",
-                "DescribeAutoScalingGroups",
-                "DescribeAutoScalingInstances",
-                "DescribeAutoScalingNotificationTypes",
-                "DescribeInstanceRefreshes",
-                "DescribeLaunchConfigurations",
-                "DescribeLifecycleHookTypes",
-                "DescribeLifecycleHooks",
-                "DescribeLoadBalancerTargetGroups",
-                "DescribeLoadBalancers",
-                "DescribeMetricCollectionTypes",
-                "DescribeNotificationConfigurations",
-                "DescribePolicies",
-                "DescribeScalingActivities",
-                "DescribeScalingProcessTypes",
-                "DescribeScheduledActions",
-                "DescribeTags",
-                "DescribeTerminationPolicyTypes",
-                "DescribeTrafficSources",
-                "DescribeWarmPool",
-                "DetachInstances",
-                "DetachLoadBalancerTargetGroups",
-                "DetachLoadBalancers",
-                "DetachTrafficSources",
-                "DisableMetricsCollection",
-                "EnableMetricsCollection",
-                "EnterStandby",
-                "ExecutePolicy",
-                "ExitStandby",
-                "GetPredictiveScalingForecast",
-                "PutLifecycleHook",
-                "PutNotificationConfiguration",
-                "PutScalingPolicy",
-                "PutScheduledUpdateGroupAction",
-                "PutWarmPool",
-                "RecordLifecycleActionHeartbeat",
-                "ResumeProcesses",
-                "RollbackInstanceRefresh",
-                "SetDesiredCapacity",
-                "SetInstanceHealth",
-                "SetInstanceProtection",
-                "StartInstanceRefresh",
-                "SuspendProcesses",
-                "TerminateInstanceInAutoScalingGroup",
-                "UpdateAutoScalingGroup"
-            ],
-            "HasResource": true,
-            "StringPrefix": "autoscaling",
-            "conditionKeys": [
-                "autoscaling:ImageId",
-                "autoscaling:InstanceType",
-                "autoscaling:InstanceTypes",
-                "autoscaling:LaunchConfigurationName",
-                "autoscaling:LaunchTemplateVersionSpecified",
-                "autoscaling:LoadBalancerNames",
-                "autoscaling:MaxSize",
-                "autoscaling:MetadataHttpEndpoint",
-                "autoscaling:MetadataHttpPutResponseHopLimit",
-                "autoscaling:MetadataHttpTokens",
-                "autoscaling:MinSize",
-                "autoscaling:ResourceTag/${TagKey}",
-                "autoscaling:SpotPrice",
-                "autoscaling:TargetGroupARNs",
-                "autoscaling:TrafficSourceIdentifiers",
-                "autoscaling:VPCZoneIdentifiers",
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
-        "Amazon EC2 Image Builder": {
-            "ARNFormat": "arn:aws:imagebuilder:${Region}:${Account}:${ResourceType}/${ResourceName}",
-            "ARNRegex": "^arn:aws:imagebuilder:.+:.+:.+",
-            "Actions": [
-                "CancelImageCreation",
-                "CreateComponent",
-                "CreateContainerRecipe",
-                "CreateDistributionConfiguration",
-                "CreateImage",
-                "CreateImagePipeline",
-                "CreateImageRecipe",
-                "CreateInfrastructureConfiguration",
-                "DeleteComponent",
-                "DeleteContainerRecipe",
-                "DeleteDistributionConfiguration",
-                "DeleteImage",
-                "DeleteImagePipeline",
-                "DeleteImageRecipe",
-                "DeleteInfrastructureConfiguration",
-                "GetComponent",
-                "GetComponentPolicy",
-                "GetContainerRecipe",
-                "GetContainerRecipePolicy",
-                "GetDistributionConfiguration",
-                "GetImage",
-                "GetImagePipeline",
-                "GetImagePolicy",
-                "GetImageRecipe",
-                "GetImageRecipePolicy",
-                "GetInfrastructureConfiguration",
-                "GetWorkflowExecution",
-                "GetWorkflowStepExecution",
-                "ImportComponent",
-                "ImportVmImage",
-                "ListComponentBuildVersions",
-                "ListComponents",
-                "ListContainerRecipes",
-                "ListDistributionConfigurations",
-                "ListImageBuildVersions",
-                "ListImagePackages",
-                "ListImagePipelineImages",
-                "ListImagePipelines",
-                "ListImageRecipes",
-                "ListImageScanFindingAggregations",
-                "ListImageScanFindings",
-                "ListImages",
-                "ListInfrastructureConfigurations",
-                "ListTagsForResource",
-                "ListWorkflowExecutions",
-                "ListWorkflowStepExecutions",
-                "PutComponentPolicy",
-                "PutContainerRecipePolicy",
-                "PutImagePolicy",
-                "PutImageRecipePolicy",
-                "StartImagePipelineExecution",
-                "TagResource",
-                "UntagResource",
-                "UpdateDistributionConfiguration",
-                "UpdateImagePipeline",
-                "UpdateInfrastructureConfiguration"
-            ],
-            "HasResource": true,
-            "StringPrefix": "imagebuilder",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "imagebuilder:CreatedResourceTag/<key>",
-                "imagebuilder:CreatedResourceTagKeys",
-                "imagebuilder:Ec2MetadataHttpTokens",
-                "imagebuilder:StatusTopicArn"
-            ]
-        },
-        "Amazon EC2 Instance Connect": {
-            "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:ec2:.+",
-            "Actions": [
-                "SendSSHPublicKey",
-                "SendSerialConsoleSSHPublicKey"
-            ],
-            "HasResource": true,
-            "StringPrefix": "ec2-instance-connect",
-            "conditionKeys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:ResourceTag/${TagKey}",
-                "ec2:osuser"
-            ]
-        },
-        "Amazon EMR Serverless": {
-            "ARNFormat": "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:emr-serverless:.+",
-            "Actions": [
-                "CancelJobRun",
-                "CreateApplication",
-                "DeleteApplication",
-                "GetApplication",
-                "GetDashboardForJobRun",
-                "GetJobRun",
-                "ListApplications",
-                "ListJobRuns",
-                "ListTagsForResource",
-                "StartApplication",
-                "StartJobRun",
-                "StopApplication",
-                "TagResource",
-                "UntagResource",
-                "UpdateApplication"
-            ],
-            "HasResource": true,
-            "StringPrefix": "emr-serverless",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
-        "Amazon EMR on EKS (EMR Containers)": {
-            "ARNFormat": "arn:aws:emr-containers:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:emr-containers:.+",
-            "Actions": [
-                "CancelJobRun",
-                "CreateJobTemplate",
-                "CreateManagedEndpoint",
-                "CreateVirtualCluster",
-                "DeleteJobTemplate",
-                "DeleteManagedEndpoint",
-                "DeleteVirtualCluster",
-                "DescribeJobRun",
-                "DescribeJobTemplate",
-                "DescribeManagedEndpoint",
-                "DescribeVirtualCluster",
-                "GetManagedEndpointSessionCredentials",
-                "ListJobRuns",
-                "ListJobTemplates",
-                "ListManagedEndpoints",
-                "ListTagsForResource",
-                "ListVirtualClusters",
-                "StartJobRun",
-                "TagResource",
-                "UntagResource"
-            ],
-            "HasResource": true,
-            "StringPrefix": "emr-containers",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "emr-containers:ExecutionRoleArn",
-                "emr-containers:JobTemplateArn"
-            ]
-        },
-        "Amazon ElastiCache": {
-            "ARNFormat": "arn:aws:elasticache:${Region}:${Account}:${ResourceType}:${ResourceName}",
-            "ARNRegex": "^arn:aws:elasticache:.+:.+:.+",
-            "Actions": [
-                "AddTagsToResource",
-                "AuthorizeCacheSecurityGroupIngress",
-                "BatchApplyUpdateAction",
-                "BatchStopUpdateAction",
-                "CompleteMigration",
-                "Connect",
-                "CopySnapshot",
-                "CreateCacheCluster",
-                "CreateCacheParameterGroup",
-                "CreateCacheSecurityGroup",
-                "CreateCacheSubnetGroup",
-                "CreateGlobalReplicationGroup",
-                "CreateReplicationGroup",
-                "CreateSnapshot",
-                "CreateUser",
-                "CreateUserGroup",
-                "DecreaseNodeGroupsInGlobalReplicationGroup",
-                "DecreaseReplicaCount",
-                "DeleteCacheCluster",
-                "DeleteCacheParameterGroup",
-                "DeleteCacheSecurityGroup",
-                "DeleteCacheSubnetGroup",
-                "DeleteGlobalReplicationGroup",
-                "DeleteReplicationGroup",
-                "DeleteSnapshot",
-                "DeleteUser",
-                "DeleteUserGroup",
-                "DescribeCacheClusters",
-                "DescribeCacheEngineVersions",
-                "DescribeCacheParameterGroups",
-                "DescribeCacheParameters",
-                "DescribeCacheSecurityGroups",
-                "DescribeCacheSubnetGroups",
-                "DescribeEngineDefaultParameters",
-                "DescribeEvents",
-                "DescribeGlobalReplicationGroups",
-                "DescribeReplicationGroups",
-                "DescribeReservedCacheNodes",
-                "DescribeReservedCacheNodesOfferings",
-                "DescribeServiceUpdates",
-                "DescribeSnapshots",
-                "DescribeUpdateActions",
-                "DescribeUserGroups",
-                "DescribeUsers",
-                "DisassociateGlobalReplicationGroup",
-                "FailoverGlobalReplicationGroup",
-                "IncreaseNodeGroupsInGlobalReplicationGroup",
-                "IncreaseReplicaCount",
-                "ListAllowedNodeTypeModifications",
-                "ListTagsForResource",
-                "ModifyCacheCluster",
-                "ModifyCacheParameterGroup",
-                "ModifyCacheSubnetGroup",
-                "ModifyGlobalReplicationGroup",
-                "ModifyReplicationGroup",
-                "ModifyReplicationGroupShardConfiguration",
-                "ModifyUser",
-                "ModifyUserGroup",
-                "PurchaseReservedCacheNodesOffering",
-                "RebalanceSlotsInGlobalReplicationGroup",
-                "RebootCacheCluster",
-                "RemoveTagsFromResource",
-                "ResetCacheParameterGroup",
-                "RevokeCacheSecurityGroupIngress",
-                "StartMigration",
-                "TestFailover"
-            ],
-            "HasResource": true,
-            "StringPrefix": "elasticache",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "elasticache:AtRestEncryptionEnabled",
-                "elasticache:AuthTokenEnabled",
-                "elasticache:AutomaticFailoverEnabled",
-                "elasticache:CacheNodeType",
-                "elasticache:CacheParameterGroupName",
-                "elasticache:ClusterModeEnabled",
-                "elasticache:EngineType",
-                "elasticache:EngineVersion",
-                "elasticache:KmsKeyId",
-                "elasticache:MultiAZEnabled",
-                "elasticache:NumNodeGroups",
-                "elasticache:ReplicasPerNodeGroup",
-                "elasticache:SnapshotRetentionLimit",
-                "elasticache:TransitEncryptionEnabled",
-                "elasticache:UserAuthenticationMode"
-            ]
-        },
-        "Amazon Elastic Block Store": {
-            "ARNFormat": "arn:aws:ebs:${Region}:${Account}:${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:ebs:.+",
-            "Actions": [
-                "CompleteSnapshot",
-                "GetSnapshotBlock",
-                "ListChangedBlocks",
-                "ListSnapshotBlocks",
-                "PutSnapshotBlock",
-                "StartSnapshot"
-            ],
-            "HasResource": true,
-            "StringPrefix": "ebs",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "ebs:Description",
-                "ebs:ParentSnapshot",
-                "ebs:VolumeSize"
-            ]
-        },
         "Amazon Elastic Container Registry": {
             "ARNFormat": "arn:aws:ecr:${Region}:${Account}:repository/${RepositoryName}",
             "ARNRegex": "^arn:aws:ecr:.+",
             "Actions": [
                 "BatchCheckLayerAvailability",
                 "BatchDeleteImage",
                 "BatchGetImage",
```

### Comparing `iam_actions-1.2.20230605/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230606/iam_actions/resourcetypes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'ec2'": '{replace: OrderedDict()}'}*

```diff
@@ -1891,368 +1891,15 @@
     },
     "ebs": {
         "snapshot": {
             "arn_pattern": "arn:*:ec2:*::snapshot/*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
-    "ec2": {
-        "capacity-reservation": {
-            "arn_pattern": "arn:*:ec2:*:*:capacity-reservation/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "capacity-reservation-fleet": {
-            "arn_pattern": "arn:*:ec2:*:*:capacity-reservation-fleet/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "carrier-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:carrier-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "certificate": {
-            "arn_pattern": "arn:*:acm:*:*:certificate/*",
-            "condition_keys": null
-        },
-        "client-vpn-endpoint": {
-            "arn_pattern": "arn:*:ec2:*:*:client-vpn-endpoint/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "coip-pool": {
-            "arn_pattern": "arn:*:ec2:*:*:coip-pool/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "customer-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:customer-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "dedicated-host": {
-            "arn_pattern": "arn:*:ec2:*:*:dedicated-host/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "dhcp-options": {
-            "arn_pattern": "arn:*:ec2:*:*:dhcp-options/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "egress-only-internet-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:egress-only-internet-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "elastic-gpu": {
-            "arn_pattern": "arn:*:ec2:*:*:elastic-gpu/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "elastic-inference": {
-            "arn_pattern": "arn:*:elastic-inference:*:*:elastic-inference-accelerator/*",
-            "condition_keys": null
-        },
-        "elastic-ip": {
-            "arn_pattern": "arn:*:ec2:*:*:elastic-ip/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "export-image-task": {
-            "arn_pattern": "arn:*:ec2:*:*:export-image-task/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "export-instance-task": {
-            "arn_pattern": "arn:*:ec2:*:*:export-instance-task/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "fleet": {
-            "arn_pattern": "arn:*:ec2:*:*:fleet/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "fpga-image": {
-            "arn_pattern": "arn:*:ec2:*:*:fpga-image/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "group": {
-            "arn_pattern": "arn:*:resource-groups:*:*:group/*",
-            "condition_keys": null
-        },
-        "host-reservation": {
-            "arn_pattern": "arn:*:ec2:*:*:host-reservation/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "image": {
-            "arn_pattern": "arn:*:ec2:*::image/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "import-image-task": {
-            "arn_pattern": "arn:*:ec2:*:*:import-image-task/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "import-snapshot-task": {
-            "arn_pattern": "arn:*:ec2:*:*:import-snapshot-task/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "instance": {
-            "arn_pattern": "arn:*:ec2:*:*:instance/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "instance-event-window": {
-            "arn_pattern": "arn:*:ec2:*:*:instance-event-window/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "internet-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:internet-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipam": {
-            "arn_pattern": "arn:*:ec2::*:ipam/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipam-pool": {
-            "arn_pattern": "arn:*:ec2::*:ipam-pool/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipam-resource-discovery": {
-            "arn_pattern": "arn:*:ec2::*:ipam-resource-discovery/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipam-resource-discovery-association": {
-            "arn_pattern": "arn:*:ec2::*:ipam-resource-discovery-association/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipam-scope": {
-            "arn_pattern": "arn:*:ec2::*:ipam-scope/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipv4pool-ec2": {
-            "arn_pattern": "arn:*:ec2:*:*:ipv4pool-ec2/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "ipv6pool-ec2": {
-            "arn_pattern": "arn:*:ec2:*:*:ipv6pool-ec2/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "key-pair": {
-            "arn_pattern": "arn:*:ec2:*:*:key-pair/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "launch-template": {
-            "arn_pattern": "arn:*:ec2:*:*:launch-template/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "license-configuration": {
-            "arn_pattern": "arn:*:license-manager:*:*:license-configuration:*",
-            "condition_keys": null
-        },
-        "local-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "local-gateway-route-table": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "local-gateway-route-table-virtual-interface-group-association": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table-virtual-interface-group-association/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "local-gateway-route-table-vpc-association": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway-route-table-vpc-association/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "local-gateway-virtual-interface": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway-virtual-interface/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "local-gateway-virtual-interface-group": {
-            "arn_pattern": "arn:*:ec2:*:*:local-gateway-virtual-interface-group/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "natgateway": {
-            "arn_pattern": "arn:*:ec2:*:*:natgateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-acl": {
-            "arn_pattern": "arn:*:ec2:*:*:network-acl/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-insights-access-scope": {
-            "arn_pattern": "arn:*:ec2:*:*:network-insights-access-scope/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-insights-access-scope-analysis": {
-            "arn_pattern": "arn:*:ec2:*:*:network-insights-access-scope-analysis/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-insights-analysis": {
-            "arn_pattern": "arn:*:ec2:*:*:network-insights-analysis/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-insights-path": {
-            "arn_pattern": "arn:*:ec2:*:*:network-insights-path/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "network-interface": {
-            "arn_pattern": "arn:*:ec2:*:*:network-interface/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "placement-group": {
-            "arn_pattern": "arn:*:ec2:*:*:placement-group/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "prefix-list": {
-            "arn_pattern": "arn:*:ec2:*:*:prefix-list/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "replace-root-volume-task": {
-            "arn_pattern": "arn:*:ec2:*:*:replace-root-volume-task/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "reserved-instances": {
-            "arn_pattern": "arn:*:ec2:*:*:reserved-instances/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "role": {
-            "arn_pattern": "arn:*:iam::*:role/*",
-            "condition_keys": null
-        },
-        "route-table": {
-            "arn_pattern": "arn:*:ec2:*:*:route-table/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "security-group": {
-            "arn_pattern": "arn:*:ec2:*:*:security-group/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "security-group-rule": {
-            "arn_pattern": "arn:*:ec2:*:*:security-group-rule/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "snapshot": {
-            "arn_pattern": "arn:*:ec2:*::snapshot/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "spot-fleet-request": {
-            "arn_pattern": "arn:*:ec2:*:*:spot-fleet-request/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "spot-instances-request": {
-            "arn_pattern": "arn:*:ec2:*:*:spot-instances-request/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "subnet": {
-            "arn_pattern": "arn:*:ec2:*:*:subnet/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "subnet-cidr-reservation": {
-            "arn_pattern": "arn:*:ec2:*:*:subnet-cidr-reservation/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "traffic-mirror-filter": {
-            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-filter/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "traffic-mirror-filter-rule": {
-            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-filter-rule/*",
-            "condition_keys": "ec2:Attribute"
-        },
-        "traffic-mirror-session": {
-            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-session/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "traffic-mirror-target": {
-            "arn_pattern": "arn:*:ec2:*:*:traffic-mirror-target/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-attachment": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-attachment/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-connect-peer": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-connect-peer/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-multicast-domain": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-multicast-domain/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-policy-table": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-policy-table/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-route-table": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-route-table/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "transit-gateway-route-table-announcement": {
-            "arn_pattern": "arn:*:ec2:*:*:transit-gateway-route-table-announcement/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "verified-access-endpoint": {
-            "arn_pattern": "arn:*:ec2:*:*:verified-access-endpoint/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "verified-access-group": {
-            "arn_pattern": "arn:*:ec2:*:*:verified-access-group/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "verified-access-instance": {
-            "arn_pattern": "arn:*:ec2:*:*:verified-access-instance/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "verified-access-policy": {
-            "arn_pattern": "arn:*:ec2:*:*:verified-access-policy/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "verified-access-trust-provider": {
-            "arn_pattern": "arn:*:ec2:*:*:verified-access-trust-provider/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "volume": {
-            "arn_pattern": "arn:*:ec2:*:*:volume/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-endpoint": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-endpoint-connection": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-connection/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-endpoint-service": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-service/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-endpoint-service-permission": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-endpoint-service-permission/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-flow-log": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-flow-log/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpc-peering-connection": {
-            "arn_pattern": "arn:*:ec2:*:*:vpc-peering-connection/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpn-connection": {
-            "arn_pattern": "arn:*:ec2:*:*:vpn-connection/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        },
-        "vpn-connection-device-type": {
-            "arn_pattern": "arn:*:ec2:*:*:vpn-connection-device-type/*",
-            "condition_keys": "ec2:Region"
-        },
-        "vpn-gateway": {
-            "arn_pattern": "arn:*:ec2:*:*:vpn-gateway/*",
-            "condition_keys": "aws:RequestTag/${TagKey}"
-        }
-    },
+    "ec2": {},
     "ec2-instance-connect": {
         "instance": {
             "arn_pattern": "arn:*:ec2:*:*:instance/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ec2messages": {},
```

### Comparing `iam_actions-1.2.20230605/iam_actions/services.json` & `iam_actions-1.2.20230606/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998769223769224%*

 * *Differences: {"'ec2'": "{'ServiceNames': ['Amazon Elastic Compute Cloud (EC2)']}",*

 * * "'kms'": "{'ConditionKeys': {insert: [(31, 'kms:ScheduleKeyDeletionPendingWindowInDays')]}}",*

 * * "'wafv2'": "{'Actions': {insert: [(14, 'DescribeAllManagedProducts'), (15, "*

 * *            "'DescribeManagedProductsByVendor')]}}"}*

```diff
@@ -7012,15 +7012,15 @@
             "ec2:VpcPeeringConnectionID",
             "ec2:VpceServiceName",
             "ec2:VpceServiceOwner",
             "ec2:VpceServicePrivateDnsName"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "Amazon EC2"
+            "Amazon Elastic Compute Cloud (EC2)"
         ]
     },
     "ec2-instance-connect": {
         "ARNFormats": [
             "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
@@ -11901,14 +11901,15 @@
             "kms:ReEncryptOnSameKey",
             "kms:RecipientAttestation:ImageSha384",
             "kms:RecipientAttestation:PCR",
             "kms:ReplicaRegion",
             "kms:RequestAlias",
             "kms:ResourceAliases",
             "kms:RetiringPrincipal",
+            "kms:ScheduleKeyDeletionPendingWindowInDays",
             "kms:SigningAlgorithm",
             "kms:ValidTo",
             "kms:ViaService",
             "kms:WrappingAlgorithm",
             "kms:WrappingKeySpec"
         ],
         "HasResource": true,
@@ -20879,14 +20880,16 @@
             "DeleteFirewallManagerRuleGroups",
             "DeleteIPSet",
             "DeleteLoggingConfiguration",
             "DeletePermissionPolicy",
             "DeleteRegexPatternSet",
             "DeleteRuleGroup",
             "DeleteWebACL",
+            "DescribeAllManagedProducts",
+            "DescribeManagedProductsByVendor",
             "DescribeManagedRuleGroup",
             "DisassociateFirewallManager",
             "DisassociateWebACL",
             "GenerateMobileSdkReleaseUrl",
             "GetDecryptedAPIKey",
             "GetIPSet",
             "GetLoggingConfiguration",
```

### Comparing `iam_actions-1.2.20230605/pyproject.toml` & `iam_actions-1.2.20230606/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230605"
+version = "1.2.20230606"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230605/setup.py` & `iam_actions-1.2.20230606/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230605',
+    'version': '1.2.20230606',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230605/PKG-INFO` & `iam_actions-1.2.20230606/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230605
+Version: 1.2.20230606
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

