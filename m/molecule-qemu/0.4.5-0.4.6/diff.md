# Comparing `tmp/molecule-qemu-0.4.5.tar.gz` & `tmp/molecule-qemu-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.5.tar", last modified: Tue Jun  6 05:26:39 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.6.tar", last modified: Tue Jun  6 07:47:44 2023, max compression
```

## Comparing `molecule-qemu-0.4.5.tar` & `molecule-qemu-0.4.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:26:39.057215 molecule-qemu-0.4.5/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 05:26:39.000000 molecule-qemu-0.4.5/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 05:26:28.000000 molecule-qemu-0.4.5/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 05:26:39.061215 molecule-qemu-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.799676 molecule-qemu-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.791676 molecule-qemu-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-06 07:47:44.799676 molecule-qemu-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.791676 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.799676 molecule-qemu-0.4.6/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/playbooks/QEMU_EFI.fd
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.799676 molecule-qemu-0.4.6/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:47:44.795676 molecule-qemu-0.4.6/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 07:47:44.000000 molecule-qemu-0.4.6/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 07:47:33.000000 molecule-qemu-0.4.6/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 07:47:44.799676 molecule-qemu-0.4.6/setup.cfg
```

### Comparing `molecule-qemu-0.4.5/.github/workflows/lint.yml` & `molecule-qemu-0.4.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/.github/workflows/publish.yml` & `molecule-qemu-0.4.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/.github/workflows/release.yml` & `molecule-qemu-0.4.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/.gitignore` & `molecule-qemu-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/.yamllint` & `molecule-qemu-0.4.6/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/LICENSE` & `molecule-qemu-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/Makefile` & `molecule-qemu-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/PKG-INFO` & `molecule-qemu-0.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.5
+Version: 0.4.6
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,15 +25,16 @@
 ```
 
 Supported platforms:
 * MacOS 13.x (aaarch64)
 
 Support guest OS:
 * Ubuntu 20.04 LTS (aarch64, x86_64)
-* Debian 11 (x86_64)
+* Ubuntu 22.04 LTS (aarch64, x86_64)
+* Debian 11 (aarch64, x86_64)
 
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 ## Network modes
 
 Network mode is selected by setting `vm_network` in `molecule.yml`. Supported modes are: `user` and `vmnet-shared`. Default mode is `user`. All modes are mutually exclusive.
 
@@ -61,26 +62,50 @@
 ```yaml
 ---
 dependency:
   name: galaxy
 driver:
   name: molecule-qemu
 platforms:
-  - name: ubuntu-1
+  - name: ubuntu-focal-arm64
     image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
     image_arch: aarch64
-    ssh_port: 10022
+    ssh_port: 10000
     ssh_user: ubuntu
-  - name: ubuntu-2
-    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
+  - name: ubuntu-focal-amd64
+    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
-    image_arch: x86_64  # default
-    ssh_port: 10023
+    image_arch: x86_64
+    ssh_port: 10001
     ssh_user: ubuntu
+  - name: ubuntu-jammy-arm64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-arm64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: aarch64
+    ssh_port: 10002
+    ssh_user: ubuntu
+  - name: ubuntu-jammy-amd64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: x86_64
+    ssh_port: 10003
+    ssh_user: ubuntu
+  - name: debian-bullseye-arm64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-arm64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: aarch64
+    ssh_port: 10004
+    ssh_user: debian
+  - name: debian-bullseye-amd64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: x86_64
+    ssh_port: 10005
+    ssh_user: debian
 provisioner:
   name: ansible
 verifier:
   name: ansible
 ```
 
 ## Example `molecule.yml` for `vmnet-shared` network mode
@@ -126,12 +151,13 @@
 * https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
 
 # Reference
 
 * [Ansible](https://www.ansible.com/)
 * [Molecule](https://molecule.readthedocs.io/en/latest/)
 * [QEMU](https://www.qemu.org/)
+* [QEMU BIOS](https://packages.debian.org/bullseye/qemu-efi-aarch64)
 
 ## QEMU vmnet-shared networking
 
 * [vmnet.framework modes](https://lore.kernel.org/all/20220315230741.21578-7-Vladislav.Yaroshchuk@jetbrains.com/T/)
```

### Comparing `molecule-qemu-0.4.5/README.md` & `molecule-qemu-0.4.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 ```
 
 Supported platforms:
 * MacOS 13.x (aaarch64)
 
 Support guest OS:
 * Ubuntu 20.04 LTS (aarch64, x86_64)
-* Debian 11 (x86_64)
+* Ubuntu 22.04 LTS (aarch64, x86_64)
+* Debian 11 (aarch64, x86_64)
 
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 ## Network modes
 
 Network mode is selected by setting `vm_network` in `molecule.yml`. Supported modes are: `user` and `vmnet-shared`. Default mode is `user`. All modes are mutually exclusive.
 
@@ -51,26 +52,50 @@
 ```yaml
 ---
 dependency:
   name: galaxy
 driver:
   name: molecule-qemu
 platforms:
-  - name: ubuntu-1
+  - name: ubuntu-focal-arm64
     image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
     image_arch: aarch64
-    ssh_port: 10022
+    ssh_port: 10000
     ssh_user: ubuntu
-  - name: ubuntu-2
-    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
+  - name: ubuntu-focal-amd64
+    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
-    image_arch: x86_64  # default
-    ssh_port: 10023
+    image_arch: x86_64
+    ssh_port: 10001
     ssh_user: ubuntu
+  - name: ubuntu-jammy-arm64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-arm64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: aarch64
+    ssh_port: 10002
+    ssh_user: ubuntu
+  - name: ubuntu-jammy-amd64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: x86_64
+    ssh_port: 10003
+    ssh_user: ubuntu
+  - name: debian-bullseye-arm64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-arm64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: aarch64
+    ssh_port: 10004
+    ssh_user: debian
+  - name: debian-bullseye-amd64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: x86_64
+    ssh_port: 10005
+    ssh_user: debian
 provisioner:
   name: ansible
 verifier:
   name: ansible
 ```
 
 ## Example `molecule.yml` for `vmnet-shared` network mode
@@ -116,12 +141,13 @@
 * https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
 
 # Reference
 
 * [Ansible](https://www.ansible.com/)
 * [Molecule](https://molecule.readthedocs.io/en/latest/)
 * [QEMU](https://www.qemu.org/)
+* [QEMU BIOS](https://packages.debian.org/bullseye/qemu-efi-aarch64)
 
 ## QEMU vmnet-shared networking
 
 * [vmnet.framework modes](https://lore.kernel.org/all/20220315230741.21578-7-Vladislav.Yaroshchuk@jetbrains.com/T/)
```

### Comparing `molecule-qemu-0.4.5/molecule_qemu/driver.py` & `molecule-qemu-0.4.6/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.6/molecule_qemu/playbooks/create.yml`

 * *Files 1% similar despite different names*

```diff
@@ -127,18 +127,18 @@
     - name: Create OpenSSH key pair
       community.crypto.openssh_keypair:
         path: "{{ molecule_ephemeral_directory }}/run/id_ed25519"
         type: ed25519
       register: ssh_keypair
 
     - name: Fetch ARM VMs bios
-      ansible.builtin.get_url:
-        url: "https://releases.linaro.org/components/kernel/uefi-linaro/latest/release/qemu64/QEMU_EFI.fd"
-        checksum: "sha256:42f915c44de6858f69ae6f1ffc9eaa3884d1b2ca97a7537d81312fb0dfd712cd"
+      ansible.builtin.copy:
+        src: "QEMU_EFI.fd"
         dest: "{{ molecule_driver_directory }}/QEMU_EFI.fd"
+        checksum: "sha256:d28d0f28b31b9982f0bed6123d9e1b9c4b9f49aa57de159808487318056ba89b"
         mode: "0644"
       when: "'aarch64' in molecule_instances | map(attribute='image_arch') | list | unique"
 
     ### images ###############################################################
 
     - name: Create images directory
       ansible.builtin.file:
@@ -241,15 +241,15 @@
         -hda {{ item.path_disk }}
         -m {{ item.vm_memory }}
         -smp {{ item.vm_cpus }}
         {% if item.vm_network == 'vmnet-shared' %}
         -nic vmnet-shared,model=virtio-net-pci,mac={{ item.vm_network_mac }}
         {% endif %}
         {% if item.vm_network == 'user' %}
-        -nic user,hostfwd=tcp::{{ item.ssh_port }}-:22
+        -nic user,model=virtio-net-pci,hostfwd=tcp::{{ item.ssh_port }}-:22
         {% endif %}
         -display none
         -daemonize
         -pidfile {{ item.path_pid }}
         {% if item.image_arch == 'aarch64' %}
         -bios {{ molecule_driver_directory }}/QEMU_EFI.fd
         -cpu cortex-a72
@@ -314,16 +314,16 @@
 
     ### ssh ###################################################################
 
     - name: Wait for SSH
       ansible.builtin.wait_for:
         host: "{{ molecule_instances_ipv4[item.name] }}"
         port: "{{ item.ssh_port }}"
-        delay: 5
-        timeout: 180
+        delay: 30
+        timeout: "{{ 60 * molecule_instances | length }}"
         search_regex: "OpenSSH"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     ### molecule ##############################################################
```

### Comparing `molecule-qemu-0.4.5/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.6/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.5/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.6/molecule_qemu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.5
+Version: 0.4.6
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,15 +25,16 @@
 ```
 
 Supported platforms:
 * MacOS 13.x (aaarch64)
 
 Support guest OS:
 * Ubuntu 20.04 LTS (aarch64, x86_64)
-* Debian 11 (x86_64)
+* Ubuntu 22.04 LTS (aarch64, x86_64)
+* Debian 11 (aarch64, x86_64)
 
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 ## Network modes
 
 Network mode is selected by setting `vm_network` in `molecule.yml`. Supported modes are: `user` and `vmnet-shared`. Default mode is `user`. All modes are mutually exclusive.
 
@@ -61,26 +62,50 @@
 ```yaml
 ---
 dependency:
   name: galaxy
 driver:
   name: molecule-qemu
 platforms:
-  - name: ubuntu-1
+  - name: ubuntu-focal-arm64
     image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
     image_arch: aarch64
-    ssh_port: 10022
+    ssh_port: 10000
     ssh_user: ubuntu
-  - name: ubuntu-2
-    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-arm64.img
+  - name: ubuntu-focal-amd64
+    image: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     image_checksum: sha256:https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
-    image_arch: x86_64  # default
-    ssh_port: 10023
+    image_arch: x86_64
+    ssh_port: 10001
     ssh_user: ubuntu
+  - name: ubuntu-jammy-arm64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-arm64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: aarch64
+    ssh_port: 10002
+    ssh_user: ubuntu
+  - name: ubuntu-jammy-amd64
+    image: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
+    image_checksum: sha256:https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
+    image_arch: x86_64
+    ssh_port: 10003
+    ssh_user: ubuntu
+  - name: debian-bullseye-arm64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-arm64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: aarch64
+    ssh_port: 10004
+    ssh_user: debian
+  - name: debian-bullseye-amd64
+    image: https://cloud.debian.org/images/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
+    image_checksum: sha512:https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
+    image_arch: x86_64
+    ssh_port: 10005
+    ssh_user: debian
 provisioner:
   name: ansible
 verifier:
   name: ansible
 ```
 
 ## Example `molecule.yml` for `vmnet-shared` network mode
@@ -126,12 +151,13 @@
 * https://cloud.debian.org/images/cloud/bullseye/latest/SHA512SUMS
 
 # Reference
 
 * [Ansible](https://www.ansible.com/)
 * [Molecule](https://molecule.readthedocs.io/en/latest/)
 * [QEMU](https://www.qemu.org/)
+* [QEMU BIOS](https://packages.debian.org/bullseye/qemu-efi-aarch64)
 
 ## QEMU vmnet-shared networking
 
 * [vmnet.framework modes](https://lore.kernel.org/all/20220315230741.21578-7-Vladislav.Yaroshchuk@jetbrains.com/T/)
```

### Comparing `molecule-qemu-0.4.5/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.6/molecule_qemu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 molecule_qemu.egg-info/dependency_links.txt
 molecule_qemu.egg-info/entry_points.txt
 molecule_qemu.egg-info/requires.txt
 molecule_qemu.egg-info/top_level.txt
 molecule_qemu/cookiecutter/cookiecutter.json
 molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
 molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+molecule_qemu/playbooks/QEMU_EFI.fd
 molecule_qemu/playbooks/create.yml
 molecule_qemu/playbooks/destroy.yml
 molecule_qemu/playbooks/templates/meta-data.j2
 molecule_qemu/playbooks/templates/user-data.j2
```

### Comparing `molecule-qemu-0.4.5/pyproject.toml` & `molecule-qemu-0.4.6/pyproject.toml`

 * *Files identical despite different names*

