# Comparing `tmp/ga4_data_import-0.1.2-py3-none-any.whl.zip` & `tmp/ga4_data_import-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 30826 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-23 23:00 ga4_data_import/__init__.py
--rw-r--r--  2.0 unx     1122 b- defN 23-May-24 20:59 ga4_data_import/common.py
--rw-r--r--  2.0 unx     8468 b- defN 23-May-31 13:49 ga4_data_import/compute.py
--rw-r--r--  2.0 unx      891 b- defN 23-May-24 18:36 ga4_data_import/storage.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    42764 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-May-31 14:53 ga4_data_import-0.1.2.dist-info/RECORD
-9 files, 89258 bytes uncompressed, 29514 bytes compressed:  66.9%
+Zip file size: 32030 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 12:03 ga4_data_import/__init__.py
+-rw-r--r--  2.0 unx      774 b- defN 23-Jun-05 15:56 ga4_data_import/common.py
+-rw-r--r--  2.0 unx     8377 b- defN 23-Jun-05 16:13 ga4_data_import/compute.py
+-rw-r--r--  2.0 unx     1322 b- defN 23-Jun-05 16:49 ga4_data_import/storage.py
+-rw-r--r--  2.0 unx     3959 b- defN 23-Jun-06 09:37 ga4_data_import/workflow.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42764 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      840 b- defN 23-Jun-06 09:41 ga4_data_import-0.1.3.dist-info/RECORD
+10 files, 93293 bytes uncompressed, 30588 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: ga4_data_import/compute.py
 Comment: 
 
 Filename: ga4_data_import/storage.py
 Comment: 
 
-Filename: ga4_data_import-0.1.2.dist-info/LICENSE
+Filename: ga4_data_import/workflow.py
 Comment: 
 
-Filename: ga4_data_import-0.1.2.dist-info/METADATA
+Filename: ga4_data_import-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: ga4_data_import-0.1.2.dist-info/WHEEL
+Filename: ga4_data_import-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: ga4_data_import-0.1.2.dist-info/top_level.txt
+Filename: ga4_data_import-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ga4_data_import-0.1.2.dist-info/RECORD
+Filename: ga4_data_import-0.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: ga4_data_import-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ga4_data_import/common.py

```diff
@@ -1,9 +1,12 @@
 # Common functions for the GA4 Data Import API code samples.
 
+import os
+import subprocess
+
 from google.cloud.resourcemanager_v3 import (
     ProjectsClient,
     SearchProjectsRequest,
 )
 
 
 def get_project_number(project_id):
@@ -18,25 +21,7 @@
     request = SearchProjectsRequest(query=f"id:{project_id}")
     response = ProjectsClient().search_projects(request=request)
     page_result = ProjectsClient().search_projects(request=request)
     for response in page_result:
         if response.project_id == project_id:
             project = response.name
             return project.replace("projects/", "")
-
-
-def get_region_from_zone(zone):
-    """
-    Get the region from the zone.
-
-    Args:
-        zone: The zone to get the region from.
-    Returns:
-        str, The region.
-    """
-    parts = zone.split("-")
-    return "-".join(parts[:-1])
-
-
-def read_pub_key(pub_key_path):
-    with open(pub_key_path, "r") as file:
-        return " ".join(file.read().strip().split(" ")[0:2])
```

## ga4_data_import/compute.py

```diff
@@ -18,30 +18,28 @@
     ServiceAccount,
     ShieldedInstanceConfig,
     ShieldedInstanceIntegrityPolicy,
     SetMetadataInstanceRequest,
     Tags,
 )
 from ga4_data_import.common import (
-    get_region_from_zone,
     get_project_number,
 )
 
 
-def create_static_address(project_id, zone, instance_name):
+def create_static_address(project_id, region, instance_name):
     """
     Create a static address with the provided name, project id, and region.
     Args:
         project_id: The project id.
-        zone: The zone to create the static address in.
+        region: The region to create the address in.
         instance_name: The name of the instance.
     Returns:
         str, The static address.
     """
-    region = get_region_from_zone(zone)
     address_name = f"{instance_name}-static"
     address_request = GetAddressRequest(
         project=project_id, region=region, address=address_name
     )
     address_client = AddressesClient()
 
     try:
@@ -57,15 +55,21 @@
         )
         address_client.insert(insert_address_request).result()
         new_address_response = address_client.get(address_request)
         return new_address_response.address
 
 
 def create_instance(
-    instance_name, project_id, zone, static_address, sftp_username, bucket_name
+    instance_name,
+    project_id,
+    zone,
+    static_address,
+    bucket_name,
+    sftp_username,
+    service_account_email = None,
 ):
     """
     Create a Compute Engine instance with the provided name, project id, zone, and bucket name.
     Args:
         instance_name: The name of the instance.
         project_id: The project id.
         zone: The zone to create the instance in.
@@ -80,83 +84,77 @@
         boot=True,
         initialize_params=AttachedDiskInitializeParams(
             disk_size_gb=10,
             source_image="projects/debian-cloud/global/images/debian-11-bullseye-v20230509",
             disk_type=f"projects/{project_id}/zones/{zone}/diskTypes/pd-balanced",
         ),
     )
-    project_number = get_project_number(project_id)
+
     metadata = [
         Items(
             key="startup-script",
             value=f"""#!/bin/bash
-
-sftp_username={sftp_username}
-bucket_name={bucket_name}
-
-# Install SFTP server
-apt-get update -y
-apt-get install -y openssh-server
-
-# Install gcloud
-# https://cloud.google.com/sdk/docs/install#installation_instructions
-echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] http://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
-curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | tee /usr/share/keyrings/cloud.google.gpg
-apt-get update -y
-apt-get install google-cloud-sdk -y
-
 # Install gcsfuse
 # https://cloud.google.com/storage/docs/gcsfuse-quickstart-mount-bucket#install
 export GCSFUSE_REPO=gcsfuse-$(lsb_release -c -s)
 echo "deb https://packages.cloud.google.com/apt $GCSFUSE_REPO main" | sudo tee /etc/apt/sources.list.d/gcsfuse.list
 curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
-sudo apt-get update -y
-sudo apt-get install -y fuse gcsfuse
+apt-get update -y
+apt-get install -y fuse gcsfuse
 rm -rf /var/lib/apt/lists/*
 
-# Create user
-adduser $sftp_username
-mkdir /home/$sftp_username
-chown root:root /home/sftp_user
+# Create SFTP user
+adduser {sftp_username}
+
+# Mount bucket
+sudo -u {sftp_username} mkdir /home/{sftp_username}/{bucket_name}_mounted
+sudo -u {sftp_username} gcsfuse -o ro --implicit-dirs --enable-storage-client-library {bucket_name} /home/{sftp_username}/{bucket_name}_mounted
+chown root:root /home/{sftp_username}
+
+# Configure SFTP server
 sed -i "s/^Subsystem\tsftp.*/Subsystem\tsftp internal-sftp/" /etc/ssh/sshd_config
 tee -a /etc/ssh/sshd_config << EOM
-Match User $sftp_username
-\tForceCommand internal-sftp -d /sftp
+Match User {sftp_username}
+\tForceCommand internal-sftp -d /{bucket_name}_mounted
 \tChrootDirectory /home/%u
 \tAllowTcpForwarding no
 \tX11Forwarding no
 \tPasswordAuthentication no
-\tAuthenticationMethods publickeyEOM
-systemctl restart ssh
-
-# Mount bucket
-sudo -u $sftp_username mkdir /home/$sftp_username/sftp
-sudo -u $sftp_username gcsfuse $bucket_name /home/$sftp_username/sftp""",
+\tAuthenticationMethods publickey
+EOM
+systemctl restart ssh""",
         )
     ]
+
     network_interface = NetworkInterface(
         name=f"{instance_name}-nic0",
         access_configs=[
             AccessConfig(
                 nat_i_p=static_address,
                 network_tier="STANDARD",
             )
         ],
     )
+
+
+    if not service_account_email:
+        project_number = get_project_number(project_id)
+        service_account_email = f"{project_number}-compute@developer.gserviceaccount.com"
     service_account = ServiceAccount(
-        email=f"{project_number}-compute@developer.gserviceaccount.com",
+        email=service_account_email,
         scopes=[
             "https://www.googleapis.com/auth/devstorage.read_only",
             "https://www.googleapis.com/auth/logging.write",
             "https://www.googleapis.com/auth/monitoring.write",
             "https://www.googleapis.com/auth/servicecontrol",
             "https://www.googleapis.com/auth/service.management.readonly",
             "https://www.googleapis.com/auth/trace.append",
         ],
     )
+
     insert_instance_request = InsertInstanceRequest(
         project=project_id,
         zone=zone,
         instance_resource=Instance(
             disks=[disk],
             machine_type=f"projects/{project_id}/zones/{zone}/machineTypes/f1-micro",
             name=instance_name,
@@ -181,65 +179,74 @@
             ignore_unknown_fields=True,
         ),
         ignore_unknown_fields=True,
     )
 
     # Create the instance
     InstancesClient().insert(request=insert_instance_request).result()
+    instance_response = InstancesClient().get(project=project_id, zone=zone, instance=instance_name)
 
+    return instance_response
 
-def add_shh_pub_key(project_id, zone, instance_name, sftp_username, key):
+
+def add_server_pub_key(
+    project_id,
+    zone,
+    instance_name,
+    key,
+    sftp_username,
+):
     """
     Add the provided SSH public key to the instance metadata.
 
     Args:
         project_id: The project id.
         zone: The zone to create the instance in.
         instance_name: The name of the instance.
         sftp_username: The username to create on the instance.
         key: SSH public key value
     Returns:
         None
     """
-    instance_client = InstancesClient()
-    instance_response = instance_client.get(
+
+    instance_response = InstancesClient().get(
         project=project_id, zone=zone, instance=instance_name
     )
 
+    metadata_items = instance_response.metadata.items
     existing_ssh_keys = ""
-    for item in instance_response.metadata.items:
-        if item.key == "ssh-keys":
-            existing_ssh_keys = item.value
+    new_key = sftp_username.strip() + ":" + key.strip()
+    for item_index in range(len(metadata_items)):
+        if metadata_items[item_index].key == "ssh-keys":
+            existing_ssh_keys = metadata_items[item_index].value.split("\n")
+
+            # Check if the key already exists
+            need_append = True
+            for key_index in range(len(existing_ssh_keys)):
+                existing_ssh_keys[key_index] = existing_ssh_keys[key_index].strip()
+                if existing_ssh_keys[key_index] == new_key:
+                    need_append = False
+                    break
+
+            existing_ssh_keys = "\n".join(existing_ssh_keys)
+
+            # Update the instance metadata with the new SSH key
+            if need_append:
+                metadata_items[item_index].value = (
+                    existing_ssh_keys + "\n" + new_key
+                )
             break
 
-    new_key = sftp_username.strip() + ":" + key.strip()
-    need_append = True
-    if existing_ssh_keys:
-        existing_ssh_keys = existing_ssh_keys.split("\n")
-        keys = []
-        for key in existing_ssh_keys:
-            keys.append(key.strip())
-            if new_key == key.strip():
-                need_append = False
-                break
-        existing_ssh_keys = "\n".join(keys)
-
-    # Update the instance metadata with the new SSH key
-    if need_append:
-        request = SetMetadataInstanceRequest(
-            project=project_id,
-            zone=zone,
-            instance=instance_name,
-            metadata_resource=Metadata(
-                fingerprint=instance_response.metadata.fingerprint,
-                items=[
-                    Items(
-                        key="ssh-keys",
-                        value=(existing_ssh_keys + "\n" + new_key)
-                        if existing_ssh_keys
-                        else new_key,
-                    )
-                ],
-            ),
-        )
+    if not existing_ssh_keys:
+        metadata_items.append(Items(key="ssh-keys", value=new_key))
+
+    request = SetMetadataInstanceRequest(
+        project=project_id,
+        zone=zone,
+        instance=instance_name,
+        metadata_resource=Metadata(
+            fingerprint=instance_response.metadata.fingerprint,
+            items=metadata_items,
+        ),
+    )
 
-        InstancesClient().set_metadata(request).result()
+    InstancesClient().set_metadata(request).result()
```

## ga4_data_import/storage.py

```diff
@@ -1,30 +1,46 @@
 # This file contains functions for interacting with Google Cloud Storage.
-from google.cloud import storage
-from ga4_data_import.common import get_project_number
+from google.cloud.storage import Client as StorageClient
+
+
+def create_bucket(bucket_name: str, region: str, ):
+    """
+    Create a new bucket with the provided name in the provided project.
+
+    Args:
+        project_id: The project id.
+        bucket_name: The name of the bucket to create.
+        region: The region to create the bucket in.
+    """
+    client = StorageClient()
+
+    try:
+        bucket = client.get_bucket(bucket_name)
+    except:
+        bucket = client.bucket(bucket_name)
+        bucket.storage_class = "STANDARD"
+        client.create_bucket(bucket, location=region)
 
 
 def add_bucket_read_access(
-    project_id: str,
     bucket_name: str,
+    service_account_email: str,
 ):
     """
     Add read access to the bucket for the compute service account.
 
     Args:
         project_id: The project id.
         bucket_name: The name of the bucket to add read access to.
     """
-    client = storage.Client()
+    client = StorageClient()
     bucket = client.get_bucket(bucket_name)
     policy = bucket.get_iam_policy(requested_policy_version=3)
-
-    project_number = get_project_number(project_id)
     policy.bindings.append(
         {
             "role": "roles/storage.objectViewer",
             "members": [
-                f"serviceAccount:{project_number}-compute@developer.gserviceaccount.com"
+                f"serviceAccount:{service_account_email}"
             ],
         }
     )
     bucket.set_iam_policy(policy)
```

## Comparing `ga4_data_import-0.1.2.dist-info/LICENSE` & `ga4_data_import-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ga4_data_import-0.1.2.dist-info/METADATA` & `ga4_data_import-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.2
+Version: 0.1.3
 Summary: Google Analytics 4 Data Import pipeline
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

## Comparing `ga4_data_import-0.1.2.dist-info/RECORD` & `ga4_data_import-0.1.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ga4_data_import/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ga4_data_import/common.py,sha256=DtqSbNbjRUmVmQ3xW7ANTzhNYX-6QobqxLRo1smm3TI,1122
-ga4_data_import/compute.py,sha256=q6SISC-JsimTzksG6WE0yMu8K39XEhleP7TRMAFaH-A,8468
-ga4_data_import/storage.py,sha256=Szmc8XlW24gllWjBheopv5Ehvwy8cTnGzaUKsCp3JEg,891
-ga4_data_import-0.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-ga4_data_import-0.1.2.dist-info/METADATA,sha256=FnVOTbI8MxLCSecl0VUi2eioHhjjx-RIQF0FskBThGo,42764
-ga4_data_import-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ga4_data_import-0.1.2.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
-ga4_data_import-0.1.2.dist-info/RECORD,,
+ga4_data_import/common.py,sha256=N4dGyc967hi91hNr2QkxZtGR1TWrWBz8jNt2ySF81cE,774
+ga4_data_import/compute.py,sha256=bk4DgpvD45SN_52rA49r16UX31z9K76z58t8eXnizw4,8377
+ga4_data_import/storage.py,sha256=ibUrR__vJTvTPX7jdMadWhfvybPA_qNNW1iuODWD8FM,1322
+ga4_data_import/workflow.py,sha256=DKGy-OvAjrpvPWvZxgXZWzV6NsgtgGxG7401jMwG574,3959
+ga4_data_import-0.1.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+ga4_data_import-0.1.3.dist-info/METADATA,sha256=7vIjbTmSbMB-hU_rvqHwyj978fji4lE9rVJ-8n_PLbM,42764
+ga4_data_import-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ga4_data_import-0.1.3.dist-info/top_level.txt,sha256=A9SJwTCHiZRjGyj-H3NS5sBdXQlEKKbEcxwZwfHqm4s,16
+ga4_data_import-0.1.3.dist-info/RECORD,,
```

