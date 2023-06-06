# Comparing `tmp/idem_gcp-0.8.0.tar.gz` & `tmp/idem_gcp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_gcp-0.8.0.tar", last modified: Wed Jan 25 14:07:15 2023, max compression
+gzip compressed data, was "idem_gcp-0.9.0.tar", last modified: Mon Jan 30 20:38:26 2023, max compression
```

## Comparing `idem_gcp-0.8.0.tar` & `idem_gcp-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,160 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5598 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4481 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/acct/gcp/
--rw-r--r--   0 root         (0) root         (0)      701 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/acct/gcp/basic_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/acct/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      603 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/acct/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      230 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/acct/gcp/default_auth.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/acct/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     2723 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/acct/gcp/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/autogen/gcp/
--rw-r--r--   0 root         (0) root         (0)     9965 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/autogen/gcp/schema_parser.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/autogen/init.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/None/
--rw-r--r--   0 root         (0) root         (0)       35 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/None/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/None/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      905 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/None/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     4317 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     6938 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)     6909 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)     5919 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    49348 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)     4937 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)     6812 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)    15643 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     6731 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     5997 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)     6268 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     5612 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      501 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     2644 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp/storage/buckets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/exec/gcp_api/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/exec/gcp_api/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/helpers/
--rw-r--r--   0 root         (0) root         (0)      834 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/helpers/exc.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/helpers/log.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/helpers/returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
--rw-r--r--   0 root         (0) root         (0)      187 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
--rw-r--r--   0 root         (0) root         (0)      204 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)      183 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/global_operation.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/region_operation.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/zone.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/compute/zone_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/metadata/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)      177 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/storage/buckets.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/resources/
--rw-r--r--   0 root         (0) root         (0)    12422 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/resources/properties.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/states/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)    21701 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    30426 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)    15172 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     6842 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)    36948 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    22536 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    96330 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    16603 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)    22157 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     9220 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     9244 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)    17918 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)    26219 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.293117 idem_gcp-0.8.0/idem_gcp/states/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)    11025 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/states/gcp/storage/buckets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.285117 idem_gcp-0.8.0/idem_gcp/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/
--rw-r--r--   0 root         (0) root         (0)     1132 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     5296 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/cloudkms/patch.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     5720 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/
--rw-r--r--   0 root         (0) root         (0)     1116 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/exec_context.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/exec_param.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/generic_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/post_exec/
--rw-r--r--   0 root         (0) root         (0)      677 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/scope.py
--rw-r--r--   0 root         (0) root         (0)    21705 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/operation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/policy.py
--rw-r--r--   0 root         (0) root         (0)    11807 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/resolver.py
--rw-r--r--   0 root         (0) root         (0)    12626 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/resource_prop_utils.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/session.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)     8398 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/idem_gcp/tool/gcp/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-01-25 14:07:14.000000 idem_gcp-0.8.0/idem_gcp/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 14:07:15.289117 idem_gcp-0.8.0/idem_gcp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5598 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4514 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-25 14:07:15.000000 idem_gcp-0.8.0/idem_gcp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-25 14:07:15.297117 idem_gcp-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3300 2023-01-25 14:07:01.000000 idem_gcp-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.506585 idem_gcp-0.9.0/idem_gcp/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/acct/gcp/
+-rw-r--r--   0 root         (0) root         (0)      701 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/basic_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/default_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/init.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/acct/gcp/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/autogen/gcp/
+-rw-r--r--   0 root         (0) root         (0)     9965 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/autogen/gcp/schema_parser.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/autogen/init.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/None/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     6938 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)    10875 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)     6909 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    49348 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)     4937 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)     6812 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    15643 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)     6268 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)     5130 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     5612 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp/storage/buckets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/exec/gcp_api/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/exec/gcp_api/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/helpers/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/exc.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/log.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/helpers/returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/global_operation.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/region_operation.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/zone.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/compute/zone_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/buckets.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/resources/
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/resources/properties.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/states/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.514586 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)    21701 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    30426 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)    15172 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)    36625 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    22499 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    97834 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    16492 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)    22046 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     9207 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)    17881 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)    23692 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    26026 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/states/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/states/gcp/storage/buckets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/patch.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     7282 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_context.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_param.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/generic_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      309 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/scope.py
+-rw-r--r--   0 root         (0) root         (0)    21705 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/init.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/operation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/policy.py
+-rw-r--r--   0 root         (0) root         (0)    11807 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    12626 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/resource_prop_utils.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/session.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8390 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/idem_gcp/tool/gcp/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 20:38:26.510586 idem_gcp-0.9.0/idem_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-01-30 20:38:26.000000 idem_gcp-0.9.0/idem_gcp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-01-30 20:38:26.518586 idem_gcp-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-01-30 20:38:12.000000 idem_gcp-0.9.0/setup.py
```

### Comparing `idem_gcp-0.8.0/LICENSE` & `idem_gcp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/PKG-INFO` & `idem_gcp-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem_gcp
-Version: 0.8.0
+Version: 0.9.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/issues
```

### Comparing `idem_gcp-0.8.0/README.rst` & `idem_gcp-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/acct/gcp/basic_auth.py` & `idem_gcp-0.9.0/idem_gcp/acct/gcp/basic_auth.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/acct/gcp/contracts/init.py` & `idem_gcp-0.9.0/idem_gcp/acct/gcp/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/acct/gcp/init.py` & `idem_gcp-0.9.0/idem_gcp/acct/gcp/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/acct/gcp/service_account.py` & `idem_gcp-0.9.0/idem_gcp/acct/gcp/service_account.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/autogen/gcp/schema_parser.py` & `idem_gcp-0.9.0/idem_gcp/autogen/gcp/schema_parser.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/conf.py` & `idem_gcp-0.9.0/idem_gcp/conf.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/None/recursive_contracts/init.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/None/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/import_job.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/import_job.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/key_ring.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/key_ring.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/cloudkms/location.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/cloudkms/location.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/accelerator_type.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/disk.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/disk_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,140 +1,143 @@
-"""Exec module for managing Disks."""
-__func_alias__ = {"list_": "list"}
-
+"""Exec module for managing Disk Types."""
+from typing import Any
+from typing import Dict
 
 from idem_gcp.tool.gcp.utils import get_project_from_account
 
+__func_alias__ = {"list_": "list"}
+
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
     filter: str = None,
     order_by: str = None,
-):
-    r"""Retrieves a list of persistent disks contained within the specified zone.
+    include_all_scopes: bool = False,
+) -> Dict[str, Any]:
+    r"""Retrieves a list of disk types available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
         filter(str, Optional):
-            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
+            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name \"instance\", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
+        include_all_scopes(bool, Optional):
+            Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
+
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk.list
+              - path: gcp.compute.disk_type.list
               - kwargs:
                   project: project-name
-                  zone: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
     project = get_project_from_account(ctx, project)
 
-    if zone:
-        ret = await hub.exec.gcp_api.client.compute.disk.list(
+    result = dict(comment=[], ret=[], result=True)
+
+    if zone and not include_all_scopes:
+        ret = await hub.exec.gcp_api.client.compute.disk_type.list(
             ctx,
             project=project,
             zone=zone,
             filter=filter,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.disk.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.disk_type.aggregatedList(
             ctx,
             project=project,
             filter=filter,
             orderBy=order_by,
+            includeAllScopes=include_all_scopes,
         )
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]["items"]
+    result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
+    name: str = None,
     project: str = None,
     zone: str = None,
-    name: str = None,
     resource_id: str = None,
 ):
-    r"""Returns a specified persistent disk.
-
-    Use an un-managed disk as a data-source. Supply one of the inputs as the filter.
-    Gets a list of available persistent disks by making a list() request.
+    r"""Returns the specified disk type.
 
     Args:
-        project(str, Optional):
-            Project ID for this request. Defaults to None.
-
-        zone(str, Optional):
-            The name of the zone for this request. Defaults to None.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
+            Defaults to None.
 
         name(str, Optional):
-            Name of the persistent disk to return. Defaults to None.
+            Name of the machine type to return.
 
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
+        project(str, Optional):
+            Project ID for this request.
+
+        zone(str, Optional):
+            The name of the zone for this request.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk.get
+              - path: gcp.compute.disk_type.get
               - kwargs:
-                  disk: disk-name
+                  name: disk-type-name
                   project: project-name
                   zone: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
     project = get_project_from_account(ctx, project)
 
+    result = dict(comment=[], ret=[], result=True)
+
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.disk.get(
+        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
             ctx,
             resource_id=resource_id,
         )
     elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.disk.get(
-            ctx, project=project, zone=zone, disk=name
+        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+            ctx,
+            project=project,
+            zone=zone,
+            diskType=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.disk#get(): {name} either resource_id or project, zone and name"
+            f"gcp.compute.disk_type {name} either resource_id or project, zone and name"
             f" should be specified."
         ]
         return result
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
+    result["comment"] += ret["comment"]
     return result
```

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/disk_type.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Exec module for managing Disk Types."""
+"""Exec module for managing Machine Types."""
 from typing import Any
 from typing import Dict
 
 from idem_gcp.tool.gcp.utils import get_project_from_account
 
 __func_alias__ = {"list_": "list"}
 
@@ -10,57 +10,57 @@
 async def list_(
     hub,
     ctx,
     project: str = None,
     zone: str = None,
     filter: str = None,
     order_by: str = None,
-    include_all_scopes: bool = False,
+    include_all_scopes: bool = None,
 ) -> Dict[str, Any]:
-    r"""Retrieves a list of disk types available to the specified project.
+    r"""Retrieves a list of machine types available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         zone(str, Optional):
             The name of the zone for this request.
 
         filter(str, Optional):
-            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name \"instance\", you would use `name ne .*instance`.
+            A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
         include_all_scopes(bool, Optional):
             Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk_type.list
+              - path: gcp.compute.machine_type.list
               - kwargs:
                   project: project-name
     """
-    project = get_project_from_account(ctx, project)
-
     result = dict(comment=[], ret=[], result=True)
 
+    project = get_project_from_account(ctx, project)
+
     if zone and not include_all_scopes:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.list(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.list(
             ctx,
             project=project,
             zone=zone,
             filter=filter,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.aggregatedList(
             ctx,
             project=project,
             filter=filter,
             orderBy=order_by,
             includeAllScopes=include_all_scopes,
         )
 
@@ -78,15 +78,15 @@
     hub,
     ctx,
     name: str = None,
     project: str = None,
     zone: str = None,
     resource_id: str = None,
 ):
-    r"""Returns the specified disk type.
+    r"""Returns the specified machine type.
 
     Args:
         resource_id(str, Optional):
             An identifier of the resource in the provider.
             Defaults to None.
 
         name(str, Optional):
@@ -99,40 +99,40 @@
             The name of the zone for this request.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.disk_type.get
+              - path: gcp.compute.machine_type.get
               - kwargs:
-                  name: disk-type-name
+                  name: machine-type-name
                   project: project-name
                   zone: zone-name
     """
-    project = get_project_from_account(ctx, project)
-
     result = dict(comment=[], ret=[], result=True)
 
+    project = get_project_from_account(ctx, project)
+
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
             ctx,
             resource_id=resource_id,
         )
     elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.disk_type.get(
+        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
             ctx,
             project=project,
             zone=zone,
-            diskType=name,
+            machineType=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.disk_type {name} either resource_id or project, zone and name"
+            f"gcp.compute.machine_type {name} either resource_id or project, zone and name"
             f" should be specified."
         ]
         return result
 
     if not ret["result"]:
         result["comment"] += ret["comment"]
         result["result"] = False
```

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/firewall.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/firewall.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/image.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/instance.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/machine_image.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/machine_image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/machine_type.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/resource_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,138 @@
-"""Exec module for managing Machine Types."""
-from typing import Any
-from typing import Dict
+"""Exec module for managing Resource Policies."""
+__func_alias__ = {"list_": "list"}
 
 from idem_gcp.tool.gcp.utils import get_project_from_account
 
-__func_alias__ = {"list_": "list"}
-
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    zone: str = None,
+    region: str = None,
     filter: str = None,
     order_by: str = None,
-    include_all_scopes: bool = None,
-) -> Dict[str, Any]:
-    r"""Retrieves a list of machine types available to the specified project.
+):
+    r"""A list all the resource policies that have been configured for the specified project in specified region.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
-        zone(str, Optional):
-            The name of the zone for this request.
+        region(str, Optional):
+            Name of the region for this request.
 
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
-        include_all_scopes(bool, Optional):
-            Indicates whether every visible scope for each scope type (zone, region, global) should be included in the response. For new resource types added after this field, the flag has no effect as new resource types will always include every visible scope for each scope type in response. For resource types which predate this field, if this flag is omitted or false, only scopes of the scope types where the resource type is expected to be found will be included.
-
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.machine_type.list
+              - path: gcp.compute.resource_policy.list
               - kwargs:
                   project: project-name
+                  region: region-name
     """
-    result = dict(comment=[], ret=[], result=True)
+    result = {
+        "comment": [],
+        "ret": None,
+        "result": True,
+    }
 
     project = get_project_from_account(ctx, project)
 
-    if zone and not include_all_scopes:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.list(
+    if region:
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.list(
             ctx,
             project=project,
-            zone=zone,
+            region=region,
             filter=filter,
             orderBy=order_by,
         )
     else:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.aggregatedList(
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.aggregatedList(
             ctx,
             project=project,
             filter=filter,
             orderBy=order_by,
-            includeAllScopes=include_all_scopes,
         )
 
+    result["comment"] += ret["comment"]
     if not ret["result"]:
-        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]["items"]
-    result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
-    name: str = None,
     project: str = None,
-    zone: str = None,
+    region: str = None,
+    name: str = None,
     resource_id: str = None,
 ):
-    r"""Returns the specified machine type.
+    r"""Retrieves all information of the specified resource policy.
 
     Args:
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
-            Defaults to None.
+        project(str, Optional):
+            Project ID for this request. Defaults to None.
 
-        name(str, Optional):
-            Name of the machine type to return.
+        region(str, Optional):
+            Name of the region for this request. Defaults to None.
 
-        project(str, Optional):
-            Project ID for this request.
+        name(str, Optional):
+            Name of the resource policy to retrieve. Defaults to None.
 
-        zone(str, Optional):
-            The name of the zone for this request.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.machine_type.get
+              - path: gcp.compute.resource_policy.get
               - kwargs:
-                  name: machine-type-name
                   project: project-name
-                  zone: zone-name
+                  region: region-name
+                  name: resource-policy-name
     """
-    result = dict(comment=[], ret=[], result=True)
+    result = {
+        "comment": [],
+        "ret": None,
+        "result": True,
+    }
 
     project = get_project_from_account(ctx, project)
 
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
             ctx,
             resource_id=resource_id,
         )
-    elif project and zone and name:
-        ret = await hub.exec.gcp_api.client.compute.machine_type.get(
-            ctx,
-            project=project,
-            zone=zone,
-            machineType=name,
+    elif project and region and name:
+        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
+            ctx, project=project, region=region, resource_policy=name
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.machine_type {name} either resource_id or project, zone and name"
+            f"gcp.compute.resource_policy {name} either resource_id or project, region and name"
             f" should be specified."
         ]
         return result
 
+    result["comment"] += ret["comment"]
     if not ret["result"]:
-        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
-    result["comment"] += ret["comment"]
     return result
```

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/network.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/node_template.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/node_template.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/reservation.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/reservation.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/resource_policy.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/zone.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,120 @@
-"""Exec module for managing Resource Policies."""
-__func_alias__ = {"list_": "list"}
+"""Exec module for managing Zones."""
+from typing import Any
+from typing import Dict
 
 from idem_gcp.tool.gcp.utils import get_project_from_account
 
+__func_alias__ = {"list_": "list"}
+
 
 async def list_(
     hub,
     ctx,
     project: str = None,
-    region: str = None,
     filter: str = None,
     order_by: str = None,
-):
-    r"""A list all the resource policies that have been configured for the specified project in specified region.
+) -> Dict[str, Any]:
+    r"""Retrieves the list of Zone resources available to the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
-        region(str, Optional):
-            Name of the region for this request.
-
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
 
         order_by(str, Optional):
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.resource_policy.list
+              - path: gcp.compute.zone.list
               - kwargs:
                   project: project-name
-                  region: region-name
+                  filter: status=UP
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
+    result = dict(comment=[], ret=[], result=True)
 
     project = get_project_from_account(ctx, project)
 
-    if region:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.list(
-            ctx,
-            project=project,
-            region=region,
-            filter=filter,
-            orderBy=order_by,
-        )
-    else:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.aggregatedList(
-            ctx,
-            project=project,
-            filter=filter,
-            orderBy=order_by,
-        )
+    ret = await hub.exec.gcp_api.client.compute.zone.list(
+        ctx,
+        project=project,
+        filter=filter,
+        orderBy=order_by,
+    )
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]["items"]
+    result["comment"] += ret["comment"]
     return result
 
 
 async def get(
     hub,
     ctx,
-    project: str = None,
-    region: str = None,
     name: str = None,
+    project: str = None,
     resource_id: str = None,
 ):
-    r"""Retrieves all information of the specified resource policy.
+    r"""Returns the specified Zone resource.
 
     Args:
-        project(str, Optional):
-            Project ID for this request. Defaults to None.
-
-        region(str, Optional):
-            Name of the region for this request. Defaults to None.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
+            Defaults to None.
 
         name(str, Optional):
-            Name of the resource policy to retrieve. Defaults to None.
+            Name of the zone resource to return.
 
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
+        project(str, Optional):
+            Project ID for this request.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.resource_policy.get
+              - path: gcp.compute.zone.get
               - kwargs:
                   project: project-name
-                  region: region-name
-                  name: resource-policy-name
+                  name: zone-name
     """
-    result = {
-        "comment": [],
-        "ret": None,
-        "result": True,
-    }
+    result = dict(comment=[], ret=[], result=True)
 
     project = get_project_from_account(ctx, project)
 
     if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
+        ret = await hub.exec.gcp_api.client.compute.zone.get(
             ctx,
             resource_id=resource_id,
         )
-    elif project and region and name:
-        ret = await hub.exec.gcp_api.client.compute.resource_policy.get(
-            ctx, project=project, region=region, resource_policy=name
+    elif project and name:
+        ret = await hub.exec.gcp_api.client.compute.zone.get(
+            ctx,
+            project=project,
+            zone=name,
         )
     else:
         result["result"] = False
         result["comment"] = [
-            f"gcp.compute.resource_policy {name} either resource_id or project, region and name"
+            f"gcp.compute.zone {name} either resource_id or project and name"
             f" should be specified."
         ]
         return result
 
-    result["comment"] += ret["comment"]
     if not ret["result"]:
+        result["comment"] += ret["comment"]
         result["result"] = False
         return result
 
     result["ret"] = ret["ret"]
+    result["comment"] += ret["comment"]
     return result
```

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/subnetwork.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/compute/zone.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/compute/snapshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""Exec module for managing Zones."""
-from typing import Any
-from typing import Dict
+__func_alias__ = {"list_": "list"}
 
+from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 from idem_gcp.tool.gcp.utils import get_project_from_account
 
-__func_alias__ = {"list_": "list"}
-
 
 async def list_(
     hub,
     ctx,
     project: str = None,
     filter: str = None,
     order_by: str = None,
-) -> Dict[str, Any]:
-    r"""Retrieves the list of Zone resources available to the specified project.
+):
+    r"""Retrieves the list of Snapshot resources contained within the specified project.
 
     Args:
         project(str, Optional):
             Project ID for this request.
 
         filter(str, Optional):
             A filter expression that filters resources listed in the response. Most Compute resources support two types of filter expressions: expressions that support regular expressions and expressions that follow API improvement proposal AIP-160. If you want to use AIP-160, your expression must specify the field name, an operator, and the value that you want to use for filtering. The value must be a string, a number, or a boolean. The operator must be either `=`, `!=`, `>`, `<`, `<=`, `>=` or `:`. For example, if you are filtering Compute Engine instances, you can exclude instances named `example-instance` by specifying `name != example-instance`. The `:` operator can be used with string fields to match substrings. For non-string fields it is equivalent to the `=` operator. The `:*` comparison can be used to test whether a key has been defined. For example, to find all objects with `owner` label use: ``` labels.owner:* ``` You can also filter nested fields. For example, you could specify `scheduling.automaticRestart = false` to include instances only if they are not scheduled for automatic restarts. You can use filtering on nested fields to filter based on resource labels. To filter on multiple expressions, provide each separate expression within parentheses. For example: ``` (scheduling.automaticRestart = true) (cpuPlatform = \"Intel Skylake\") ``` By default, each expression is an `AND` expression. However, you can include `AND` and `OR` expressions explicitly. For example: ``` (cpuPlatform = \"Intel Skylake\") OR (cpuPlatform = \"Intel Broadwell\") AND (scheduling.automaticRestart = true) ``` If you want to use a regular expression, use the `eq` (equal) or `ne` (not equal) operator against a single un-parenthesized expression with or without quotes or against multiple parenthesized expressions. Examples: `fieldname eq unquoted literal` `fieldname eq 'single quoted literal'` `fieldname eq \"double quoted literal\"` `(fieldname1 eq literal) (fieldname2 ne \"literal\")` The literal value is interpreted as a regular expression using Google RE2 library syntax. The literal value must match the entire field. For example, to filter for instances that do not end with name "instance", you would use `name ne .*instance`.
@@ -27,94 +24,69 @@
             Sorts list results by a certain order. By default, results are returned in alphanumerical order based on the resource name. You can also sort results in descending order based on the creation timestamp using `orderBy=\"creationTimestamp desc\"`. This sorts results based on the `creationTimestamp` field in reverse chronological order (newest result first). Use this to sort resources like operations so that the newest operation is returned first. Currently, only sorting by `name` or `creationTimestamp desc` is supported.
 
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.zone.list
+              - path: gcp.compute.snapshot.list
               - kwargs:
                   project: project-name
-                  filter: status=UP
     """
-    result = dict(comment=[], ret=[], result=True)
-
     project = get_project_from_account(ctx, project)
 
-    ret = await hub.exec.gcp_api.client.compute.zone.list(
-        ctx,
-        project=project,
-        filter=filter,
-        orderBy=order_by,
+    execution_context = ExecutionContext(
+        resource_type="compute.snapshot",
+        method_name="list",
+        method_params={
+            "ctx": ctx,
+            "project": project,
+            "filter": filter,
+            "order_by": order_by,
+        },
     )
-
-    if not ret["result"]:
-        result["comment"] += ret["comment"]
-        result["result"] = False
-        return result
-
-    result["ret"] = ret["ret"]["items"]
-    result["comment"] += ret["comment"]
-    return result
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def get(
     hub,
     ctx,
-    name: str = None,
-    project: str = None,
     resource_id: str = None,
+    project: str = None,
+    snapshot: str = None,
 ):
-    r"""Returns the specified Zone resource.
+    r"""Returns the specified Snapshot resource. Gets a list of available snapshots by making a list() request.
 
     Args:
         resource_id(str, Optional):
             An identifier of the resource in the provider.
-            Defaults to None.
-
-        name(str, Optional):
-            Name of the zone resource to return.
 
         project(str, Optional):
             Project ID for this request.
 
+        snapshot(str, Optional):
+            Name of the snapshot resource to return.
+
     Examples:
         .. code-block: sls
 
             random-name:
               exec.run:
-              - path: gcp.compute.zone.get
+              - path: gcp.compute.instance.get
               - kwargs:
                   project: project-name
-                  name: zone-name
+                  zone: zone-name
+                  instance: instance-name
     """
-    result = dict(comment=[], ret=[], result=True)
-
     project = get_project_from_account(ctx, project)
 
-    if resource_id:
-        ret = await hub.exec.gcp_api.client.compute.zone.get(
-            ctx,
-            resource_id=resource_id,
-        )
-    elif project and name:
-        ret = await hub.exec.gcp_api.client.compute.zone.get(
-            ctx,
-            project=project,
-            zone=name,
-        )
-    else:
-        result["result"] = False
-        result["comment"] = [
-            f"gcp.compute.zone {name} either resource_id or project and name"
-            f" should be specified."
-        ]
-        return result
-
-    if not ret["result"]:
-        result["comment"] += ret["comment"]
-        result["result"] = False
-        return result
-
-    result["ret"] = ret["ret"]
-    result["comment"] += ret["comment"]
-    return result
+    execution_context = ExecutionContext(
+        resource_type="compute.snapshot",
+        method_name="get",
+        method_params={
+            "ctx": ctx,
+            "resource_id": resource_id,
+            "project": project,
+            "snapshot": snapshot,
+        },
+    )
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
```

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/sample.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/sample.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp/storage/buckets.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp/storage/buckets.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/exec/gcp_api/init.py` & `idem_gcp-0.9.0/idem_gcp/exec/gcp_api/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/helpers/exc.py` & `idem_gcp-0.9.0/idem_gcp/helpers/exc.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/helpers/log.py` & `idem_gcp-0.9.0/idem_gcp/helpers/log.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/helpers/returns.py` & `idem_gcp-0.9.0/idem_gcp/helpers/returns.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/resources/properties.yaml` & `idem_gcp-0.9.0/idem_gcp/resources/properties.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -668,7 +668,40 @@
     - targetServiceAccounts
     - allowed
     - denied
     - direction
     - logConfig
     - disabled
     - selfLink
+
+compute.snapshot:
+  get:
+    - project
+    - snapshot
+  insert:
+#    path parameters
+    - project
+    - snapshot
+#    query parameters
+    - requestId
+#    body
+    - labels
+    - labelFingerprint
+    - snapshotEncryptionKey
+    - snapshotType
+    - locationHint
+    - description
+    - sourceDisk
+    - chainName
+    - storageLocations
+    - sourceDiskEncryptionKey
+    - name
+  delete:
+#   path parameters
+    - project
+    - snapshot
+#   query parameters
+    - requestId
+  exclude_paths:
+    - labelFingerprint
+  exclude_properties_from_transformation:
+    - labels
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/crypto_key.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/import_job.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/import_job.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/key_ring.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/key_ring.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/cloudkms/location.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/cloudkms/location.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/disk.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,14 @@
 
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.disk"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if resource_id:
@@ -445,15 +444,14 @@
                             operation.get("selfLink"), "compute.zone_operation"
                         )
                     )
                     op_ret = await hub.tool.gcp.operation_utils.handle_operation(
                         ctx, operation_id, "compute.disk", True
                     )
                     if not op_ret["result"]:
-                        result["result"] = False
                         result["comment"] += op_ret["comment"]
                         result["rerun_data"] = op_ret["rerun_data"]
                         return result
 
             size_gb_updated = True
 
         # Update labels
@@ -489,15 +487,14 @@
                             operation.get("selfLink"), "compute.zone_operation"
                         )
                     )
                     op_ret = await hub.tool.gcp.operation_utils.handle_operation(
                         ctx, operation_id, "compute.disk", True
                     )
                     if not op_ret["result"]:
-                        result["result"] = False
                         result["comment"] += op_ret["comment"]
                         result["rerun_data"] = op_ret["rerun_data"]
                         return result
 
             labels_updated = True
 
         # Update resource policies
@@ -569,15 +566,14 @@
                             )
                             op_ret = (
                                 await hub.tool.gcp.operation_utils.handle_operation(
                                     ctx, operation_id, "compute.disk", True
                                 )
                             )
                             if not op_ret["result"]:
-                                result["result"] = False
                                 result["comment"] += op_ret["comment"]
                                 result["rerun_data"] = op_ret["rerun_data"]
                                 return result
 
                     if (
                         remove_ret is None or remove_ret["result"]
                     ) and add_request_body is not None:
@@ -600,15 +596,14 @@
                             )
                             op_ret = (
                                 await hub.tool.gcp.operation_utils.handle_operation(
                                     ctx, operation_id, "compute.disk", True
                                 )
                             )
                             if not op_ret["result"]:
-                                result["result"] = False
                                 result["comment"] += op_ret["comment"]
                                 result["rerun_data"] = op_ret["rerun_data"]
                                 return result
 
                 resource_policies_updated = True
 
         # Reset the operation because we don't need it
@@ -666,15 +661,14 @@
             operation.get("selfLink"), "compute.zone_operation"
         )
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, operation_id, "compute.disk"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     # Try getting the resource again
@@ -792,15 +786,14 @@
                 return result
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.disk"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
     result["comment"].append(
         hub.tool.gcp.comment_utils.delete_comment("gcp.compute.disk", name)
     )
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/image.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,14 @@
                 return result
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.image"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/instance.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     ] = None,
     labels: Dict[str, Any] = None,
     display_device: make_dataclass(
         "DisplayDevice", [("enable_display", bool, field(default=None))]
     ) = None,
     source_machine_image: str = None,
     resource_policies: List[str] = None,
+    status: str = None,
     tags: make_dataclass(
         "Tags",
         [
             ("fingerprint", str, field(default=None)),
             ("items", List[str], field(default=None)),
         ],
     ) = None,
@@ -595,14 +596,28 @@
 
         source_machine_image(str, optional):
             Source machine image. Defaults to None.
 
         resource_policies(List[str], optional):
             Resource policies applied to this instance. Defaults to None.
 
+        status(str, Optional):
+            The status of the instance. One of the following values: PROVISIONING, STAGING, RUNNING, STOPPING, SUSPENDING, SUSPENDED, REPAIRING, and TERMINATED. For more information about the status of the instance, see Instance life cycle.
+                Enum type. Allowed values:
+                "DEPROVISIONING" - The Nanny is halted and we are performing tear down tasks like network deprogramming, releasing quota, IP, tearing down disks etc.
+                "PROVISIONING" - Resources are being allocated for the instance.
+                "REPAIRING" - The instance is in repair.
+                "RUNNING" - The instance is running.
+                "STAGING" - All required resources have been allocated and the instance is being started.
+                "STOPPED" - The instance has stopped successfully.
+                "STOPPING" - The instance is currently stopping (either being deleted or killed).
+                "SUSPENDED" - The instance has suspended.
+                "SUSPENDING" - The instance is suspending.
+                "TERMINATED" - The instance has stopped (either by explicit action or underlying failure). Defaults to None.
+
         tags(Dict[str, Any], optional):
             Tags to apply to this instance. Tags are used to identify valid sources or targets for network firewalls and are specified by the client during instance creation. The tags can be later modified by the setTags method. Each tag within the list must comply with RFC1035. Multiple tags can be specified via the 'tags.items' field.
                 Tags: A set of instance tags. Defaults to None.
 
                 * fingerprint (str, optional):
                     Specifies a fingerprint for this request, which is essentially a hash of the tags' contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update tags. You must always provide an up-to-date fingerprint hash in order to update or change tags. To see the latest fingerprint, make get() request to the instance.
 
@@ -1109,40 +1124,60 @@
         "name": name,
         "comment": [],
     }
     project = get_project_from_account(ctx, project)
 
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, ctx.get("rerun_data"), "compute.instance"
+            ctx, ctx.get("rerun_data").get("operation_id"), "compute.instance"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
+            result["rerun_data"] = ctx.get("rerun_data")
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
     if resource_id:
         old_get_ret = await hub.exec.gcp.compute.instance.get(
             ctx, resource_id=resource_id
         )
 
-        if not old_get_ret["result"] or not old_get_ret["ret"]:
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
 
+        # long running operation has succeeded - both update and create
+        if ctx.get("rerun_data"):
+            result["new_state"] = old_get_ret["ret"]
+            result["old_state"] = ctx["rerun_data"]["old_state"]
+            if ctx["rerun_data"]["old_state"]:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.update_comment(
+                        "gcp.compute.instance", name
+                    )
+                )
+            else:
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.create_comment(
+                        "gcp.compute.instance", name
+                    )
+                )
+            return result
+
         result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
-    elif not hub.OPT.idem.get("get_resource_only_with_resource_id", False):
-        resource_id = (ctx.get("old_state") or {}).get(
-            "resource_id"
-        ) or hub.tool.gcp.resource_prop_utils.construct_resource_id(
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
             "compute.instance", {**locals(), "instance": name}
         )
         old_get_ret = await hub.exec.gcp.compute.instance.get(
             ctx, resource_id=resource_id
         )
 
         if not old_get_ret["result"]:
@@ -1180,43 +1215,40 @@
         "shielded_instance_config": shielded_instance_config,
         "labels": labels,
         "deletion_protection": deletion_protection,
         "network_interfaces": network_interfaces,
         "can_ip_forward": can_ip_forward,
         "display_device": display_device,
         "zone": zone,
+        "status": status,
     }
 
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
     if result["old_state"]:
         # copy.copy(old_get_ret['ret']) is needed to convert any objects of type NamespaceDict to dict
         # in old_get_ret['ret']. This is done so that comparisons with the resource_body which has
         # objects of type dict works properly
         zone = hub.tool.gcp.resource_prop_utils.parse_link_to_zone(
             result["old_state"]["zone"]
         )
         result["old_state"]["zone"] = zone
 
-        # If rerun_data is set at this point this means that there has been a completed create or update operation
-        # so there is no need to run the code for create or update below again and we stop here
-        if ctx.get("rerun_data"):
-            result["new_state"] = result["old_state"]
-            return result
-
-        # TODO: if we fix isPending() to not update after creation we can make the fingerprint required upon update
+        # The fingerprint is required upon an update operation but in the time of creation the
+        # resource still do not have fingerprint so, we cannot make it a required param for present method.
         resource_body["fingerprint"] = fingerprint or result["old_state"].get(
             "fingerprint"
         )
         resource_body["label_fingerprint"] = label_fingerprint or result[
             "old_state"
         ].get("label_fingerprint")
 
         # A dictionary of additional operations to perform on the object identified by the key
-        # the values are tuples with the first element - the method to call, the second element - arguments, third - the property is required in the end result
+        # the values are tuples with the first element - the method to call, the second element - arguments,
+        # third - the property is required in the end result
         patch_operations_dict = {
             "network_interfaces": (
                 hub.tool.gcp.compute.instance.update_network_interfaces,
                 (ctx, result["old_state"], network_interfaces),
                 True,
             ),
             "shielded_instance_config": (
@@ -1232,14 +1264,19 @@
                     None,
                     None,
                     None,
                     resource_id,
                 ),
                 False,
             ),
+            "status": (
+                hub.tool.gcp.compute.instance.update_status,
+                (ctx, resource_id, result["old_state"].get("status"), status),
+                True,
+            ),
         }
 
         old_properties_dict = {
             k: result["old_state"].get(k) for k in patch_operations_dict.keys()
         }
         changed_properties_dict = {
             k: hub.tool.gcp.utils.compare_states(
@@ -1273,15 +1310,15 @@
                 )
                 result["new_state"] = copy.deepcopy(result["old_state"])
                 return result
 
         if not changes and not any(changed_properties_dict.values()):
             result["result"] = True
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
                     "gcp.compute.instance", name
                 )
             )
             result["new_state"] = copy.deepcopy(result["old_state"])
             return result
 
         if ctx["test"]:
@@ -1332,25 +1369,37 @@
                 name=name,
                 resource_id=resource_id,
                 minimal_action=minimal_action,
                 most_disruptive_allowed_action=most_disruptive_allowed_action,
                 body=resource_body,
             )
 
-            if not update_ret["result"]:
+            if not update_ret["result"] or not update_ret["ret"]:
                 result["result"] = False
                 result["comment"] += update_ret["comment"]
                 return result
-            if update_ret["ret"] is not None:
-                if "compute#operation" in update_ret["ret"].get("kind", ""):
-                    operation = update_ret["ret"]
 
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.update_comment("gcp.compute.instance", name)
-        )
+            if "compute#operation" in update_ret["ret"].get("kind", ""):
+                operation = update_ret["ret"]
+
+        if not changes and any(changed_properties_dict.values()):
+            get_ret = await hub.exec.gcp.compute.instance.get(
+                ctx, resource_id=resource_id
+            )
+            if not get_ret["result"] and not get_ret["ret"]:
+                result["result"] = False
+                result["comment"] += get_ret["comment"]
+                return result
+
+            result["new_state"] = get_ret["ret"]
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.update_comment("gcp.compute.instance", name)
+            )
+            return result
+
     else:
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
                     "gcp.compute.instance", name
                 )
             )
@@ -1364,67 +1413,46 @@
             name=name,
             project=project,
             zone=zone,
             source_instance_template=source_instance_template,
             request_id=request_id,
             body=resource_body,
         )
-        if not create_ret["result"]:
+        if not create_ret["result"] or not create_ret["ret"]:
             result["result"] = False
             if create_ret["comment"] and next(
                 (
                     comment
                     for comment in create_ret["comment"]
                     if "alreadyExists" in comment
                 ),
                 None,
             ):
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.already_exists_comment(
                         "gcp.compute.instance", name
                     )
                 )
-                return result
             else:
                 result["comment"] += create_ret["comment"]
-        else:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.create_comment("gcp.compute.instance", name)
-            )
-            resource_id = create_ret["ret"].get("resource_id")
-        if create_ret["ret"] is not None:
-            if "compute#operation" in create_ret["ret"].get("kind", ""):
-                operation = create_ret["ret"]
+            return result
+
+        if "compute#operation" in create_ret["ret"].get("kind", ""):
+            operation = create_ret["ret"]
 
     if operation:
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
             operation.get("selfLink"), "compute.zone_operation"
         )
-        handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
-            ctx, operation_id, "compute.instance"
-        )
-
-        if not handle_operation_ret["result"]:
-            result["result"] = False
-            result["comment"] += handle_operation_ret["comment"]
-            result["rerun_data"] = handle_operation_ret["rerun_data"]
-            return result
-
-        resource_id = handle_operation_ret["resource_id"]
-
-    # Try getting the resource again
-    get_ret = await hub.exec.gcp.compute.instance.get(ctx, resource_id=resource_id)
-
-    if not get_ret["result"] and not get_ret["ret"]:
-        result["result"] = False
-        result["comment"] += get_ret["comment"]
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
         return result
 
-    result["new_state"] = get_ret["ret"]
-
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str = None,
@@ -1529,15 +1557,14 @@
             return result
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.instance"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
     result["comment"].append(
         hub.tool.gcp.comment_utils.delete_comment("gcp.compute.instance", name)
     )
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/machine_image.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/machine_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,14 @@
     # TODO: Handle operation result state
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.machine_image"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if resource_id:
@@ -238,15 +237,14 @@
             operation.get("selfLink"), "compute.global_operation"
         )
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, operation_id, "compute.machine_image"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     # Try getting the resource again
@@ -334,15 +332,14 @@
 
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.machine_image"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/network.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
 
     if ctx.get("rerun_data"):
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.network"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if resource_id:
@@ -310,15 +309,14 @@
             operation.get("selfLink"), "compute.global_operation"
         )
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, operation_id, "compute.network"
         )
 
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     # Try getting the resource again
@@ -420,15 +418,14 @@
 
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.network"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/node_template.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/node_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,14 @@
 
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.node_template"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/reservation.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/reservation.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,14 @@
 
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.reservation"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/resource_policy.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/resource_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,14 @@
                 return result
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.resource_policy"
         )
         if not handle_operation_ret["result"]:
-            result["result"] = False
             result["comment"] += handle_operation_ret["comment"]
             result["rerun_data"] = handle_operation_ret["rerun_data"]
             return result
 
         resource_id = handle_operation_ret["resource_id"]
 
     if not resource_id:
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/compute/subnetwork.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/compute/subnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,14 @@
     # Handle operation(s) in progress, if any
     if ctx.get("rerun_data"):
         op_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.subnetwork"
         )
 
         if not op_ret["result"]:
-            result["result"] = False
             result["comment"] += op_ret["comment"]
             result["rerun_data"] = op_ret["rerun_data"]
             return result
 
         resource_id = op_ret["resource_id"]
 
     if resource_id:
@@ -298,15 +297,14 @@
             operation.get("selfLink"), "compute.region_operation"
         )
         op_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, op_id, "compute.subnetwork"
         )
 
         if not op_ret["result"]:
-            result["result"] = False
             result["comment"] += op_ret["comment"]
             result["rerun_data"] = op_ret["rerun_data"]
             return result
 
         resource_id = op_ret["resource_id"]
 
     new = await hub.exec.gcp.compute.subnetwork.get(
@@ -347,15 +345,14 @@
                 operation.get("selfLink"), "compute.region_operation"
             )
             handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
                 ctx, operation_id, "compute.subnetwork", True
             )
 
             if not handle_operation_ret["result"]:
-                result["result"] = False
                 result["comment"] += handle_operation_ret["comment"]
                 result["rerun_data"] = handle_operation_ret["rerun_data"]
                 return result
 
             resource_id = handle_operation_ret["resource_id"]
             prop_updated = True
 
@@ -383,15 +380,14 @@
                 operation.get("selfLink"), "compute.region_operation"
             )
             handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
                 ctx, operation_id, "compute.subnetwork", True
             )
 
             if not handle_operation_ret["result"]:
-                result["result"] = False
                 result["comment"] += handle_operation_ret["comment"]
                 result["rerun_data"] = handle_operation_ret["rerun_data"]
                 return result
 
             resource_id = handle_operation_ret["resource_id"]
             prop_updated = True
 
@@ -516,15 +512,14 @@
                     return result
     else:
         # delete() has been called on some previous iteration
         op_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.subnetwork"
         )
         if not op_ret["result"]:
-            result["result"] = False
             result["comment"] += op_ret["comment"]
             result["rerun_data"] = op_ret["rerun_data"]
             return result
 
         resource_id = op_ret["resource_id"]
 
     result["comment"].append(
```

### Comparing `idem_gcp-0.8.0/idem_gcp/states/gcp/storage/buckets.py` & `idem_gcp-0.9.0/idem_gcp/states/gcp/storage/buckets.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/case.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/case.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/cloudkms/patch.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/cloudkms/patch.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/comment_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/comment_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     return f"{resource_type} '{name}' already absent"
 
 
 def already_exists_comment(hub, resource_type: str, name: str) -> str:
     return f"{resource_type} '{name}' already exists."
 
 
+def up_to_date_comment(hub, resource_type: str, name: str) -> str:
+    return f"{resource_type} '{name}' is up to date."
+
+
 def update_tags_comment(hub, tags_to_remove, tags_to_add) -> str:
     return f"Update tags: Add keys {tags_to_add.keys()} Remove keys {tags_to_remove.keys()}"
 
 
 def would_update_tags_comment(hub, tags_to_remove, tags_to_add) -> str:
     return f"Would update tags: Add keys {tags_to_add.keys()} Remove keys {tags_to_remove.keys()}"
```

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/compute/network.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/conversion_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/exec_context.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/exec_context.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/generic_exec.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/generic_exec.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,51 +13,47 @@
     operation = execution_context.response["ret"]
     operation_type = hub.tool.gcp.generate.operators.post_exec.operation_processor.get_operation_type(
         operation
     )
     if operation_type is None:
         execution_context.response["result"] = False
         execution_context.response["comment"] += "Unexpected operation type returned"
-        execution_context.response["rerun_data"] = None
         return
     operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
         operation.get("selfLink"), operation_type
     )
     op_ret = await hub.tool.gcp.operation_utils.handle_operation(
         execution_context.method_params.get("ctx"),
         operation_id,
         execution_context.resource_type,
-        True,
+        wait_until_done=True,
     )
 
     if not op_ret["result"]:
         execution_context.response["result"] = False
         execution_context.response["comment"] += op_ret["comment"]
-        execution_context.response["rerun_data"] = op_ret["rerun_data"]
         return
 
     # if op_ret["result"] is True, then the operation is finished and resource_id is returned
     resource_id = op_ret.get("resource_id")
     resource_get_result = await hub.tool.gcp.generate.operators.post_exec.operation_processor.invoke_get_operation_for_resource(
         execution_context, resource_id
     )
 
     if resource_get_result is None:
         execution_context.response["result"] = False
         execution_context.response["comment"] += "Could not find resource"
-        execution_context.response["rerun_data"] = None
         return
     if not resource_get_result["result"]:
         execution_context.response["result"] = False
         execution_context.response["comment"] += resource_get_result["comment"]
-        execution_context.response["rerun_data"] = None
         return
+
     execution_context.response["result"] = True
     execution_context.response["ret"] = resource_get_result["ret"]
-    execution_context.response["rerun_data"] = None
 
 
 def get_operation_type(hub, operation) -> str:
     return hub.tool.gcp.operation_utils.get_operation_type(operation.get("selfLink"))
 
 
 async def invoke_get_operation_for_resource(hub, execution_context, resource_id):
```

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/init.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/operation_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/operation_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import time
 from typing import Any
 from typing import Dict
 
 
 async def handle_operation(
-    hub, ctx, operation_id: str, resource_type: str, wait_until_done: bool = False
+    hub, ctx, rerun_data, resource_type: str, wait_until_done: bool = False
 ) -> Dict[str, Any]:
     result = {
         "comment": [],
         "result": True,
         "rerun_data": None,
         "resource_id": None,
     }
 
+    rerun_dict = isinstance(rerun_data, dict)
+    operation_id = rerun_data["operation_id"] if rerun_dict else rerun_data
+
     operation_type = hub.tool.gcp.operation_utils.get_operation_type(operation_id)
 
     if operation_type is None:
         result["result"] = False
         result["comment"].append(
             f"Cannot determine operation scope (zonal/regional/global) {operation_id}"
         )
@@ -44,19 +47,25 @@
     if operation["status"] != "DONE":
         if wait_until_done:
             operation = await hub.tool.gcp.operation_utils.wait_for_operation(
                 ctx, operation, operation_type
             )
         else:
             result["result"] = False
-            result[
-                "rerun_data"
-            ] = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                operation.get("selfLink"), operation_type
+            new_operation_id = (
+                hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+                    operation.get("selfLink"), operation_type
+                )
             )
+            if rerun_dict:
+                rerun_data["operation_id"] = new_operation_id
+            else:
+                rerun_data = new_operation_id
+            result["rerun_data"] = rerun_data
+
             result["comment"] += get_ret["comment"]
             return result
 
     if operation.get("error"):
         result["result"] = False
         result["comment"] += str(operation.get("error", {}))
         return result
```

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/policy.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/resolver.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/resolver.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/resource_prop_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/resource_prop_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/session.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/session.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/state_comparison_utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-0.8.0/idem_gcp/tool/gcp/utils.py` & `idem_gcp-0.9.0/idem_gcp/tool/gcp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,20 +179,24 @@
     :param hub: The Hub into which the resolved callable will get placed.
     :param ret: The returned dictionary of the last run.
     :param state: The name of the state.
     :param pending_kwargs: (dict, Optional) May include 'ctx' and 'reruns_wo_change_count'.
 
     :return: True | False
     """
-    if ret and ret.get("rerun_data"):
+    if not ret:
+        return False
+
+    if ret.get("rerun_data"):
         return True
-    elif pending_kwargs and pending_kwargs.get("reruns_wo_change_count", 0) >= 3:
+
+    if ret["result"]:
         return False
 
-    return not ret["result"] is True or bool(ret["changes"])
+    return pending_kwargs and pending_kwargs.get("reruns_wo_change_count", 0) < 4
 
 
 def compare_states(
     hub, old_state: Dict, plan_state: Dict, resource_type: str = None
 ) -> Dict:
     exclude_paths = []
```

### Comparing `idem_gcp-0.8.0/idem_gcp.egg-info/PKG-INFO` & `idem_gcp-0.9.0/idem_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-gcp
-Version: 0.8.0
+Version: 0.9.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/issues
```

### Comparing `idem_gcp-0.8.0/idem_gcp.egg-info/SOURCES.txt` & `idem_gcp-0.9.0/idem_gcp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 idem_gcp/exec/gcp/compute/instance.py
 idem_gcp/exec/gcp/compute/machine_image.py
 idem_gcp/exec/gcp/compute/machine_type.py
 idem_gcp/exec/gcp/compute/network.py
 idem_gcp/exec/gcp/compute/node_template.py
 idem_gcp/exec/gcp/compute/reservation.py
 idem_gcp/exec/gcp/compute/resource_policy.py
+idem_gcp/exec/gcp/compute/snapshot.py
 idem_gcp/exec/gcp/compute/subnetwork.py
 idem_gcp/exec/gcp/compute/zone.py
 idem_gcp/exec/gcp/contracts/init.py
 idem_gcp/exec/gcp/storage/buckets.py
 idem_gcp/exec/gcp_api/init.py
 idem_gcp/helpers/exc.py
 idem_gcp/helpers/log.py
@@ -61,14 +62,15 @@
 idem_gcp/metadata/gcp/compute/machine_image.py
 idem_gcp/metadata/gcp/compute/machine_type.py
 idem_gcp/metadata/gcp/compute/network.py
 idem_gcp/metadata/gcp/compute/node_template.py
 idem_gcp/metadata/gcp/compute/region_operation.py
 idem_gcp/metadata/gcp/compute/reservation.py
 idem_gcp/metadata/gcp/compute/resource_policy.py
+idem_gcp/metadata/gcp/compute/snapshot.py
 idem_gcp/metadata/gcp/compute/subnetwork.py
 idem_gcp/metadata/gcp/compute/zone.py
 idem_gcp/metadata/gcp/compute/zone_operation.py
 idem_gcp/metadata/gcp/storage/buckets.py
 idem_gcp/metadata/gcp/storage/objectAccessControls.py
 idem_gcp/resources/properties.yaml
 idem_gcp/states/gcp/init.py
@@ -81,14 +83,15 @@
 idem_gcp/states/gcp/compute/image.py
 idem_gcp/states/gcp/compute/instance.py
 idem_gcp/states/gcp/compute/machine_image.py
 idem_gcp/states/gcp/compute/network.py
 idem_gcp/states/gcp/compute/node_template.py
 idem_gcp/states/gcp/compute/reservation.py
 idem_gcp/states/gcp/compute/resource_policy.py
+idem_gcp/states/gcp/compute/snapshot.py
 idem_gcp/states/gcp/compute/subnetwork.py
 idem_gcp/states/gcp/storage/buckets.py
 idem_gcp/tool/gcp/case.py
 idem_gcp/tool/gcp/comment_utils.py
 idem_gcp/tool/gcp/conversion_utils.py
 idem_gcp/tool/gcp/init.py
 idem_gcp/tool/gcp/operation_utils.py
```

### Comparing `idem_gcp-0.8.0/setup.py` & `idem_gcp-0.9.0/setup.py`

 * *Files identical despite different names*

