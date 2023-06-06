# Comparing `tmp/pulumi_digitalocean-4.9.0.tar.gz` & `tmp/pulumi_digitalocean-4.9.0a1637244514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_digitalocean-4.9.0.tar", last modified: Thu Nov 18 15:07:57 2021, max compression
+gzip compressed data, was "dist/pulumi_digitalocean-4.9.0a1637244514.tar", last modified: Thu Nov 18 14:14:32 2021, max compression
```

## Comparing `pulumi_digitalocean-4.9.0.tar` & `pulumi_digitalocean-4.9.0a1637244514.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (121)     8787 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)   251716 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    18293 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    21319 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/cdn.py
--rw-r--r--   0 runner    (1001) docker     (121)    27633 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    14801 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/container_registry_docker_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    23888 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/custom_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    43129 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    24336 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     9279 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_db.py
--rw-r--r--   0 runner    (1001) docker     (121)    12980 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)    26482 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_replica.py
--rw-r--r--   0 runner    (1001) docker     (121)    14894 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    26213 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (121)    10637 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)    62475 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/droplet.py
--rw-r--r--   0 runner    (1001) docker     (121)    13578 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/droplet_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)    26701 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)    12628 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     9586 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/floating_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5860 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    11291 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_database_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     9365 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_database_replica.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     6037 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_domains.py
--rw-r--r--   0 runner    (1001) docker     (121)    15855 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8700 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplet_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8851 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)     5218 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    11535 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_images.py
--rw-r--r--   0 runner    (1001) docker     (121)    12670 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     6856 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_kubernetes_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10498 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7915 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     7066 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     6245 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_records.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_sizes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)    15001 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     6655 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_buckets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     7091 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     9883 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_volume_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    42206 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    36625 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    46578 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    29726 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/monitor_alert.py
--rw-r--r--   0 runner    (1001) docker     (121)   358121 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22567 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    10082 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/project_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     9832 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    27151 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/spaces_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)    49769 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/spaces_bucket_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    10482 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    14327 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    32766 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     9622 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)    15815 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)    18673 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3155 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-11-18 15:07:57.000000 pulumi_digitalocean-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/
+-rw-r--r--   0 runner    (1001) docker     (121)     4229 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (121)     8787 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)   251716 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18293 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21319 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/cdn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27633 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14801 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/container_registry_docker_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23888 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43129 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24336 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9279 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12980 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26482 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_replica.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14894 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26213 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10637 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62475 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/droplet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13578 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/droplet_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26701 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12628 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9586 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/floating_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4714 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6072 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5860 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11291 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_database_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9365 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_database_replica.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4319 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6037 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_domains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15855 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8700 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplet_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8851 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5218 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11535 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7328 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12670 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6856 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_kubernetes_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10498 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7915 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7066 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6245 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_records.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5040 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6832 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5258 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15001 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6655 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7091 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8770 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9883 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7586 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42206 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36625 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46578 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29726 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/monitor_alert.py
+-rw-r--r--   0 runner    (1001) docker     (121)   358121 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22567 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10082 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/project_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9832 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    27151 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/spaces_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49769 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/spaces_bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10482 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14327 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32766 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9622 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15815 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18673 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4229 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3155 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 14:14:32.000000 pulumi_digitalocean-4.9.0a1637244514/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2143 2021-11-18 14:14:31.000000 pulumi_digitalocean-4.9.0a1637244514/setup.py
```

### Comparing `pulumi_digitalocean-4.9.0/PKG-INFO` & `pulumi_digitalocean-4.9.0a1637244514/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_digitalocean
-Version: 4.9.0
+Version: 4.9.0a1637244514
 Summary: A Pulumi package for creating and managing Digital Ocean cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-digitalocean
 Description: [![Actions Status](https://github.com/pulumi/pulumi-digitalocean/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-digitalocean/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdigitalocean.svg)](https://www.npmjs.com/package/@pulumi/digitalocean)
```

### Comparing `pulumi_digitalocean-4.9.0/README.md` & `pulumi_digitalocean-4.9.0a1637244514/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/__init__.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/_enums.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/_inputs.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/_utilities.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/app.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/cdn.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/cdn.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/certificate.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/config/vars.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/container_registry.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/container_registry_docker_credentials.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/container_registry_docker_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/custom_image.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/custom_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_cluster.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_connection_pool.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_db.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_firewall.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_replica.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_replica.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/database_user.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/database_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/dns_record.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/dns_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/domain.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/droplet.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/droplet.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/droplet_snapshot.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/droplet_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/firewall.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/floating_ip.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/floating_ip_assignment.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/floating_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_account.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_app.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_certificate.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_container_registry.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_database_cluster.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_database_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_database_replica.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_database_replica.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_domain.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_domains.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_domains.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplet.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplet.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplet_snapshot.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplet_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_droplets.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_droplets.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_firewall.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_floating_ip.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_image.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_images.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_images.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_kubernetes_cluster.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_kubernetes_versions.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_kubernetes_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_load_balancer.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_project.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_projects.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_record.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_records.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_records.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_region.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_regions.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_sizes.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_sizes.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket_object.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_bucket_objects.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_bucket_objects.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_spaces_buckets.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_spaces_buckets.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_ssh_key.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_ssh_keys.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_tag.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_tags.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_volume.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_volume_snapshot.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/get_vpc.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/get_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/kubernetes_cluster.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/kubernetes_node_pool.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/load_balancer.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/monitor_alert.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/monitor_alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/outputs.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/project.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/project_resources.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/project_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/provider.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/spaces_bucket.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/spaces_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/spaces_bucket_object.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/spaces_bucket_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/ssh_key.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/tag.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume_attachment.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/volume_snapshot.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean/vpc.py` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/PKG-INFO` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-digitalocean
-Version: 4.9.0
+Version: 4.9.0a1637244514
 Summary: A Pulumi package for creating and managing Digital Ocean cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-digitalocean
 Description: [![Actions Status](https://github.com/pulumi/pulumi-digitalocean/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-digitalocean/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdigitalocean.svg)](https://www.npmjs.com/package/@pulumi/digitalocean)
```

### Comparing `pulumi_digitalocean-4.9.0/pulumi_digitalocean.egg-info/SOURCES.txt` & `pulumi_digitalocean-4.9.0a1637244514/pulumi_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_digitalocean-4.9.0/setup.py` & `pulumi_digitalocean-4.9.0a1637244514/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.9.0"
-PLUGIN_VERSION = "4.9.0"
+VERSION = "4.9.0a1637244514"
+PLUGIN_VERSION = "4.9.0-alpha.1637244514+fdf90a86"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'digitalocean', PLUGIN_VERSION])
         except OSError as error:
```

