# Comparing `tmp/inhandtest-0.0.51.tar.gz` & `tmp/inhandtest-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.51.tar", last modified: Thu Jun  1 09:31:01 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.52.tar", last modified: Tue Jun  6 05:27:38 2023, max compression
```

## Comparing `inhandtest-0.0.51.tar` & `inhandtest-0.0.52.tar`

### file list

```diff
@@ -1,83 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.51/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-01 09:31:01.000000 inhandtest-0.0.51/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.51/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.51/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.51/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.51/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.51/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39706 2023-05-31 08:51:14.000000 inhandtest-0.0.51/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.51/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.51/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    58057 2023-06-01 03:29:00.000000 inhandtest-0.0.51/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23326 2023-06-01 01:06:15.000000 inhandtest-0.0.51/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.51/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.51/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.51/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.51/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.51/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51904 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.51/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.51/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.51/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     6182 2023-06-01 03:29:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/docker_manager_locators.py
--rw-rw-rw-   0        0        0      878 2023-06-01 03:02:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/edge_computing.py
--rw-rw-rw-   0        0        0      469 2023-06-01 02:49:02.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    10706 2023-06-01 03:16:20.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     6112 2023-06-01 01:34:12.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py
--rw-rw-rw-   0        0        0     2531 2023-06-01 09:19:48.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     4165 2023-06-01 03:13:15.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      767 2023-05-25 07:59:28.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0     6939 2023-05-25 02:09:36.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/acl_locators.py
--rw-rw-rw-   0        0        0     3783 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/bridge_locators.py
--rw-rw-rw-   0        0        0    15320 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/cellular_locators.py
--rw-rw-rw-   0        0        0     3388 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/dhcp_locators.py
--rw-rw-rw-   0        0        0     2457 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/dns_locators.py
--rw-rw-rw-   0        0        0     5274 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/ethernet_locators.py
--rw-rw-rw-   0        0        0     7476 2023-05-25 08:45:27.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/firewall.py
--rw-rw-rw-   0        0        0     8415 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/gps_locators.py
--rw-rw-rw-   0        0        0      470 2023-05-23 03:37:38.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/host_list_locators.py
--rw-rw-rw-   0        0        0    11017 2023-05-25 06:05:46.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/l2tp_locators.py
--rw-rw-rw-   0        0        0     3667 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/lan_locators.py
--rw-rw-rw-   0        0        0     2341 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/loopback_locators.py
--rw-rw-rw-   0        0        0     5698 2023-05-25 02:19:26.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/nat_locators.py
--rw-rw-rw-   0        0        0     2628 2023-05-25 05:59:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    32342 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_interface.py
--rw-rw-rw-   0        0        0     1745 2023-05-25 03:11:00.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_locators.py
--rw-rw-rw-   0        0        0    13074 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/network_services.py
--rw-rw-rw-   0        0        0     4371 2023-05-25 01:08:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing.py
--rw-rw-rw-   0        0        0     1305 2023-05-23 06:46:19.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/routing_status_locators.py
--rw-rw-rw-   0        0        0     2972 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/static_routing_locators.py
--rw-rw-rw-   0        0        0     9910 2023-05-25 05:58:37.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/vpn.py
--rw-rw-rw-   0        0        0     5208 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/wan_locators.py
--rw-rw-rw-   0        0        0    10254 2023-05-24 10:28:05.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/network/wlan_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6971 2023-05-25 08:09:35.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview_locators.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.51/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.51/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33736 2023-06-01 08:56:40.000000 inhandtest-0.0.51/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25747 2023-06-01 09:03:09.000000 inhandtest-0.0.51/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2838 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 09:31:01.000000 inhandtest-0.0.51/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.51/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:31:01.000000 inhandtest-0.0.51/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-06-01 09:30:50.000000 inhandtest-0.0.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.52/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-06 05:27:38.000000 inhandtest-0.0.52/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.52/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.52/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.52/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.52/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.52/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40079 2023-06-06 03:00:03.000000 inhandtest-0.0.52/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.52/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.52/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    58788 2023-06-06 05:15:22.000000 inhandtest-0.0.52/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23364 2023-06-05 10:27:40.000000 inhandtest-0.0.52/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.52/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.52/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.52/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.52/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.52/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51904 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.52/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.52/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.52/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     2393 2023-06-06 05:25:15.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8317 2023-06-06 01:49:59.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67781 2023-06-02 09:30:51.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86145 2023-06-02 02:13:33.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0     9556 2023-06-06 05:26:06.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0     9456 2023-06-06 05:25:15.000000 inhandtest-0.0.52/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.52/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.52/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33681 2023-06-06 05:26:30.000000 inhandtest-0.0.52/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    27448 2023-06-02 06:02:42.000000 inhandtest-0.0.52/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 05:27:38.000000 inhandtest-0.0.52/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.52/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:27:38.000000 inhandtest-0.0.52/setup.cfg
+-rw-rw-rw-   0        0        0     1626 2023-06-06 05:27:26.000000 inhandtest-0.0.52/setup.py
```

### Comparing `inhandtest-0.0.51/PKG-INFO` & `inhandtest-0.0.52/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.51
+Version: 0.0.52
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.51/README.md` & `inhandtest-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/dm/mqtt.py` & `inhandtest-0.0.52/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/dm/register_v1.py` & `inhandtest-0.0.52/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.52/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                                    'alarm': 'Alarm', 'realtime_alarms': 'Realtime Alarms', 'alarm_rules': 'Alarm Rules',
                                    'history_alarms': 'History Alarms', 'alarm_label': 'Alarm Label',
                                    'cloud': 'Cloud', 'mqtt_cloud_service': 'MQTT Cloud Service',
                                    'whitehawk_energy_manager': 'Whitehawk Energy Manager', 'protocol': 'Protocol',
                                    'parameter_settings': 'Parameter Settings',
                                    'custom_quickfunctions': 'Custom QuickFunctions',
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
+                                   'clear_history_log': 'Clear History Log',
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
                                    'system_network_tools': 'Network Tools',
                                    'system_3rd_party': '3rd Party Notification',
                                    'configuration': ' Configuration', 'trigger_condition': 'Trigger Condition',
                                    'gigabitethernet': 'Gigabitethernet', 'flow_usage_day': 'Flow Usage Monitoring(Day)',
@@ -73,14 +74,15 @@
                                    'measure_monitor': '测点监控', 'monitoring_list': '监控列表', 'group': '分组',
                                    'alarm': '告警', 'realtime_alarms': '实时告警', 'alarm_rules': '告警规则',
                                    'history_alarms': '历史告警', 'alarm_label': '告警标签',
                                    'cloud': '云服务', 'mqtt_cloud_service': 'MQTT云服务',
                                    'whitehawk_energy_manager': '白鹰能源管家', 'protocol': '协议转换',
                                    'parameter_settings': '参数设置', 'custom_quickfunctions': '自定义快函数',
                                    'system': '系统管理', 'system_time': '系统时间', 'system_log': '系统日志',
+                                   'clear_history_log': '清除历史日志',
                                    'system_config': '配置管理', 'system_cloud': '设备云平台',
                                    'system_firmware': '固件升级', 'system_tools': '管理工具',
                                    'system_user_management': '用户管理', 'system_reboot': '重启',
                                    'system_network_tools': '工具', 'system_3rd_party': '第三方软件声明',
                                    'configuration': '配置',
                                    'trigger_condition': '触发条件', 'gigabitethernet': '千兆以太网口',
                                    'flow_usage_day': '流量使用监测（当天）', 'flow_usage_month': '流量使用监测（当月）'
@@ -631,20 +633,22 @@
                 'log': {
                     'default': 'log',
                     'menu': self.system_log_menu,
                     'visible_locator': [self.content_target('system_log')],
                     'wait_locator': [self.content_target('system_log')],
                     'log': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=0'),
+                        'visible_locator': [self.page.locator('//button', has_text=self.__locale.get('clear_history_log'))],
                         'attributes': {
                             self.page.locator('.ant-tabs-tab >> nth=0'): {'aria-selected': 'true'}},
                         'wait_locator': [self.page.locator('//button[@class="ant-btn"]').first],
                     },
                     'configure': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=1'),
+                        'visible_locator': [self.page.locator('#log_to_remote_enable')],
                         'attributes': {
                             self.page.locator('.ant-tabs-tab >> nth=1'): {'aria-selected': 'true'}},
                         'wait_locator': [self.page.locator('#log_to_remote_enable')],
                     }
                 },
                 'configuration_management': {
                     'menu': self.system_config_menu,
```

### Comparing `inhandtest-0.0.51/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.52/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.52/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/base_page/base_page.py` & `inhandtest-0.0.52/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     'submit': self.page.locator('.login_button'),
                     'wait_locator': self.page.locator('#logo')}
         else:
             raise Exception(f'not support this model {self.model}')
 
     def __new_page(self):
         def dialog_(dialog):
-            logging.info(f'dialog message is {dialog.message}, accepted')
+            logging.debug(f'dialog message is {dialog.message}, accepted')
             dialog.accept()
 
         self.__playwright = sync_playwright().start()
         if self.__browser_type == 'firefox':
             browser = self.__playwright.firefox
         elif self.__browser_type == 'webkit':
             browser = self.__playwright.webkit
@@ -135,39 +135,38 @@
                 logging.info(f'Open {self.host} device address {device} and login')
             else:
                 logging.info(f'Open {self.host} device address {device}')
 
         def _login():
             if self.model not in self.__http_credentials_model:
                 self.__login_locator.get('username').fill(username)
-                logging.info('Device %s fill username %s' % (self.host, username))
+                logging.debug('Device %s fill username %s' % (self.host, username))
                 self.__login_locator.get('password').fill(password)
-                logging.info('Device %s fill password %s' % (self.host, password))
+                logging.debug('Device %s fill password %s' % (self.host, password))
                 self.__login_locator.get('submit').click()
                 logging.info("Device %s  login" % self.host)
                 if status == 'success':
                     self.__login_locator.get('wait_locator').wait_for(state='visible')
                     self.page.wait_for_timeout(500)
 
         for i in range(0, 10):
             if self.__login_locator.get('username') and self.__login_locator.get(
                     'username').is_visible():
                 _login()
                 break
             elif self.__login_locator.get('wait_locator') and self.__login_locator.get(
                     'wait_locator').is_visible():
-                # logging.info("Device %s already login in" % self.host)
                 break
             elif self.page.url == 'about:blank':
                 goto_router()
                 _login()
                 break
             else:
                 try:
-                    logging.info(f"Device %s refresh page {i + 1} times" % self.host)
+                    logging.debug(f"Device %s refresh page {i + 1} times" % self.host)
                     self.page.reload()
                 except TimeoutError:
                     pass
         else:
             raise Exception(f'Device {self.host} page error')
 
     @allure.step('页面抓取接口返回结果')
@@ -176,15 +175,15 @@
 
         :param url:  pattern 匹配的正则表达式,
         :param timeout: 默认30秒
         :return: 返回结果
         """
         with self.page.expect_response(lambda response: re.search(url, response.url) and response.status == 200,
                                        timeout=timeout * 1000) as response_info:
-            logging.info("Device %s fetch url %s " % (self.host, response_info.value.url))
+            logging.debug("Device %s fetch url %s " % (self.host, response_info.value.url))
         logging.info("Device %s the api response is  %s " % (self.host, response_info.value.json()))
         return response_info.value.json()
 
     @allure.step('进入菜单')
     def access_menu(self, menu: str, wait_time=None) -> None:
         """进入菜单，多个菜单使用点号隔开，不限多少层级   menu_locator 存放在 base_locators 里面，
             定义menu = {'system': {'locator': '#menu_id', 'wait_locator': '#wait_locator_id'},
@@ -203,28 +202,29 @@
             _in_current_menu = False
             if locators.get('visible_locator'):
                 _in_current_menu = True
                 for visible_locator in locators.get('visible_locator'):
                     if not visible_locator.is_visible():
                         _in_current_menu = False
                         break
-            if locators.get('attributes'):
-                for locator, value in locators.get('attributes').items():
-                    if locator.is_visible():
-                        for attr, expect_value in value.items():
-                            if expect_value not in locator.get_attribute(attr):
-                                _in_current_menu = False
-                                break
+            if _in_current_menu:
+                if locators.get('attributes'):
+                    for locator, value in locators.get('attributes').items():
+                        if locator.is_visible():
+                            for attr, expect_value in value.items():
+                                if expect_value not in locator.get_attribute(attr):
+                                    _in_current_menu = False
+                                    break
+                            else:
+                                _in_current_menu = True
+                                continue
+                            break
                         else:
-                            _in_current_menu = True
-                            continue
-                        break
-                    else:
-                        _in_current_menu = False
-                        break
+                            _in_current_menu = False
+                            break
             return _in_current_menu
 
         def access_one_menu(menu_one: str, locators: dict, level: int):  # 进入某一个菜单
             if not in_current_menu(locators):
                 menus = locators.get('menu') if isinstance(locators.get('menu'), list) else [locators.get('menu')]
                 for menu_1 in menus:
                     self.click(menu_1)
@@ -252,15 +252,15 @@
                 else:
                     break
             if click_menus:
                 click_menus.reverse()  # 回归原来的顺序
                 for menu_one, locators, level_ in click_menus:
                     access_one_menu(menu_one, locators, level_)
             else:
-                logging.info(f'already in {".".join(menu)} menu')
+                logging.debug(f'already in {".".join(menu)} menu')
 
         def default_change(menu_old, locators: dict) -> str:
             menu_old_s = menu_old.split('.')
             for menu_old_ in menu_old_s:
                 locators = locators.get(menu_old_)
             default = locators.get('default')
             menu_new = menu_old + '.' + default if default else menu_old
@@ -364,32 +364,32 @@
                     option_.click()
                     select = True
                     break
                 elif option_.count() == 0:
                     if option_end != all_option_.last.inner_text():
                         option_end = all_option_.last.inner_text()
                         all_option_.last.scroll_into_view_if_needed()
-                        logging.info(f'scroll down the scroll bar {find_time + 1} tims')
+                        logging.debug(f'scroll down the scroll bar {find_time + 1} tims')
                     else:
-                        logging.info(f'scroll down the bottom')
+                        logging.debug(f'scroll down the bottom')
                         break
                 else:
                     raise Exception('found more option elements')
             if not select:
                 for find_time in range(0, times):
                     if option_.count() == 1:
                         option_.click()
                         break
                     elif option_.count() == 0:
                         if option_end != all_option_.first.inner_text():
                             option_end = all_option_.first.inner_text()
                             all_option_.first.scroll_into_view_if_needed()
-                            logging.info(f'scroll up the scroll bar {find_time + 1}')
+                            logging.debug(f'scroll up the scroll bar {find_time + 1}')
                         else:
-                            logging.info(f'scroll up the top')
+                            logging.debug(f'scroll up the top')
                             break
                     else:
                         raise Exception('found more option elements')
                 else:
                     raise Exception('scroll bar too lang, more 100 times')
 
         if value is not None:
@@ -463,15 +463,15 @@
             if option.count() == 1:
                 if 'ant-radio-wrapper-checked' not in option.get_attribute('class'):
                     option.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} radio select {value}")
                 else:
                     if log_desc:
-                        logging.info(f"Device {self.host} {log_desc} radio already select {value}")
+                        logging.debug(f"Device {self.host} {log_desc} radio already select {value}")
             else:
                 raise Exception(f'found {value} option {option.count()} elements')
 
     @allure.step('伸缩按钮')
     def expand(self, left_text: str, action: str = 'expand') -> None:
         """ 伸缩按钮
 
@@ -517,15 +517,15 @@
         def upload():
             if path_:
                 if os.path.isfile(path_) and os.path.exists(path_):
                     with self.page.expect_file_chooser() as fc:
                         locator.click()
                     file_chooser = fc.value
                     file_chooser.set_files(path_)
-                    logging.info(f'Device {self.host} upload {path_} Successful')
+                    logging.info(f'Device {self.host} upload {path_} success')
                 else:
                     logging.error(f'{path_} Does Not Exist.')
 
         if dialog_massage:
             self.dialog_massage(upload, dialog_massage)
         else:
             upload()
@@ -543,32 +543,48 @@
             if os.path.isdir(file_path) and os.path.exists(file_path):
                 with self.page.expect_download() as download_info:
                     locator.click()
                 download = download_info.value
                 file_name = download.suggested_filename if file_name is None else file_name
                 download.save_as(path.join(file_path, file_name))
                 logging.info(
-                    f'Device {self.host} download {download.suggested_filename} to path {file_path} successful')
+                    f'Device {self.host} download {download.suggested_filename} to path {file_path} success')
             else:
                 logging.error(f'{file_path} Does Not Exist.')
 
+    @allure.step('输入时间或日期')
+    def fill_date(self, locator: Locator, date: str) -> None:
+        """输入时间或日期
+
+        :param locator:
+        :param date: 日期，格式为 2020-01-01
+        :return:
+        """
+        self.click(locator)
+        if locator.get_attribute('class') == 'ant-calendar-picker':   # date
+            locator_ = self.page.locator('.ant-calendar-input')
+        else:
+            locator_ = self.page.locator('.ant-time-picker-panel-input')
+        locator_.fill(date)
+        locator_.press('Enter')
+
     @allure.step("校验dialog message")
     def dialog_massage(self, f, message: str = '') -> None:
         """对话框提示进行校验， 使用时需要在base_locator 里面定义dialog_massage 且返回字典数据
 
         :param f:  是一个操作函数，执行后会有dialog弹窗出现
         :param message: 校验的信息, 支持模糊匹配
         :return:
         """
         if message:
             message = self.locale.get(message) if self.locale.get(message) else message
             with self.page.expect_event('dialog') as dialog_info:
                 f()
             assert message in dialog_info.value.message, f'{self.host} assert {message} dialog error'
-            logging.info(f'Device {self.host} assert dialog {message} successful')
+            logging.info(f'Device {self.host} assert dialog {message} success')
 
     @allure.step("校验tip messages")
     def tip_messages(self, messages: str or list = None, timeout=30) -> None:
         """ 某些提交操作会出现文本的提示，提示在过几秒钟后会消失，对于该类消息的验证使用该方法，
             使用时需要在base_locator tip_messages 且返回字典数据
 
         :param messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
@@ -579,15 +595,15 @@
         """
         if messages:
             tip_messages = [messages] if isinstance(messages, str) else messages
             for message in tip_messages:
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_hidden(timeout=timeout * 1000)
-                logging.info(f'{self.host} assert tip {message} visible successful')
+                logging.info(f'{self.host} assert tip {message} visible success')
 
     @allure.step("校验text messages")
     def text_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对文本内容做验证，如在输入框输入错误内容时出现的文本，该类文本会一直存在
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
@@ -596,15 +612,15 @@
             text_messages = [messages] if isinstance(messages, str) else messages
             text_messages = Counter(text_messages)  # 处理多个相同的文本
             for message, count in text_messages.items():
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 for i_ in range(0, count):
                     expect(self.page.get_by_text(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
                         timeout=timeout * 1000)
-                    logging.info(f'{self.host} assert text the {i_}th {message}  visible successful')
+                    logging.info(f'{self.host} assert text the {i_}th {message}  visible success')
 
     @allure.step("校验元素Title")
     def title_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对元素的属性title做内容验证，
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
@@ -613,15 +629,15 @@
             text_messages = [messages] if isinstance(messages, str) else messages
             text_messages = Counter(text_messages)
             for message, count in text_messages.items():
                 message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 for i_ in range(0, count):
                     expect(self.page.get_by_title(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
                         timeout=timeout * 1000)
-                    logging.info(f'{self.host} assert title the {i_}th {message} visible successful')
+                    logging.info(f'{self.host} assert title the {i_}th {message} visible success')
 
     @allure.step('设置页面翻页')
     def page_refresh(self, refresh_time: str, select_locator: Locator) -> None:
         """
         :param refresh_time: str
                         '0'|'3'|'4'|'5'|'10'|'15'|'30'|'60'|'120'|'180'|'240'|'300'|'600'|'900'|'1200'|'1800'
         :param select_locator: 元素定位
@@ -716,15 +732,15 @@
                 :param locators:  列表 嵌套 长度为2的元组，元组的第一项为操作项名称， 第二项为对应的一个字典
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
-                    $type: 操作项的类型 text|select|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|
+                    $type: 操作项的类型 text|select|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|fill_date|
                                      multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
@@ -825,14 +841,16 @@
             elif param_locator.get('type') == 'title_messages':
                 if value:
                     messages, timeout = value, 10
                     if isinstance(value, dict):
                         timeout = value.get('timeout') if value.get('timeout') else 10
                         messages = value.get('messages')
                     self.title_messages(messages, timeout)
+            elif param_locator.get('type') == 'fill_date':
+                self.fill_date(param_locator.get('locator'), value)
             else:
                 raise Exception(f"not support this param type {param_locator.get('type')}")
             if param_locator.get('wait_for'):
                 wait_for = [param_locator.get('wait_for')] if isinstance(param_locator.get('wait_for'),
                                                                          dict) else param_locator.get('wait_for')
                 for wait_for_ in wait_for:
                     if wait_for_.get('type') == 'timeout':
@@ -895,20 +913,20 @@
                         if '${value}' in expect_.get(key):
                             expression = expect_.get(key).replace('${value}', value).replace('\n', ' ')
                         else:
                             expression = f'"{expect_.get(key)}" == "{value}"'  # 默认使用等于判断
                         if option[1].get('param'):
                             expression = replace_str(expression, option[1].get('param'))
                         if eval(expression):
-                            logging.info(f'Check {option[0]} , {expression} is true')
+                            logging.info(f'Check {option[0]} , {expression} is success')
                         else:
-                            logging.info(f'Check {option[0]} , {expression} is false')
+                            logging.info(f'Check {option[0]} , {expression} is failed')
                             return False
                     except TypeError:
-                        logging.info(f'get {key} inner_text failed')
+                        logging.error(f'get {key} inner_text failed')
                         return False
                 else:
                     raise KeyError(f'not support the key {key}')
         return True
 
     @allure.step("获取页面元素文本值")
     def get_text(self, keys: str or list or tuple, locators: list) -> str or dict or None:
@@ -976,18 +994,18 @@
         :return:
         """
         tag_result = True
         if host_or_ip:
             host_or_ip = [host_or_ip] if isinstance(host_or_ip, str) else host_or_ip
             for host in host_or_ip:
                 command = f'ping {host} -n {number}' if src is None else f'ping -S {src} {host} -n {number}'
-                logging.info(command)
+                logging.debug(command)
                 if assert_result:
                     result = os.popen(command).read()
-                    logging.info(result)
+                    logging.debug(result)
                     if lost_packets:  # 判断需要丢包
                         send = re.findall(r'已发送 = (.*?)，', result, re.S)[0]
                         accept = re.findall(r'已接收 = (.*?)，', result, re.S)[0]
                         if send == accept:
                             if '无法访问' not in result:
                                 logging.info(f'PC {src} ping {host} does not loss packet')
                                 tag_result = False
@@ -1010,15 +1028,15 @@
             self.__context.close()
             self.__browser.close()
             self.__playwright.stop()
             logging.info('close browser and playwright')
 
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
+    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.DEBUG,
                         stream=sys.stdout)
     with BasePage('10.5.24.96', 'adm', '123456', 'https', 443, model='ig902') as my_page:
         # system = (
         #     '3rd party notification', '3rd party notification', 'cloud edge computing.azure iot edge',
         #     'cloud edge computing.aws iot greengrass',
         #     'device supervisor',
         #     'device supervisor.measure monitor.group', 'device supervisor.alarm', 'device supervisor.alarm.alarm rules',
```

### Comparing `inhandtest-0.0.51/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.52/inhandtest/base_page/table_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # @File    : table_tr.py
 """
 table_tr
 
 """
 import logging
 import re
-import time
 from typing import List
 from inhandtest.tools import replace_str
 from playwright.sync_api import Locator, TimeoutError
 
 
 class Table:
 
@@ -118,15 +117,15 @@
         for i in range(0, self.tr.get_by_role('button').count()):
             action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
             if action_attribute in (
                     'TGO(this).onAdd()', 'TGO(this).footerAdd()', 'footerAdd()') and self.tr.get_by_role(
                 'button').nth(i).is_enabled():
                 self.tr.get_by_role('button').nth(i).click()
                 if self.log_desc is not None:
-                    logging.info(f'add table {self.log_desc} success')
+                    logging.debug(f'add table {self.log_desc} success')
                 break
 
     def delete(self, **kwargs) -> None:
         """
         :param kwargs str, 待删除列 及对应值
         :return:
         """
@@ -136,15 +135,15 @@
             for i in range(0, self.tr.get_by_role('button').count()):
                 action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
                 if action_attribute in (
                         "TGO(this).onDelete()", "TGO(this).footerDel()", "footerDel()", 'delete_save(this)'):
                     if not self.tr.get_by_role('button').nth(i).is_disabled():
                         self.tr.get_by_role('button').nth(i).click()
                         if self.log_desc is not None:
-                            logging.info(f'delete table {self.log_desc} success')
+                            logging.debug(f'delete table {self.log_desc} success')
                         break
                     else:
                         logging.error(f'the data in the row {find_tr} cannot be deleted')
         else:
             logging.warning(f'not found the resource {kwargs}')
 
     def delete_all(self) -> None:
@@ -249,15 +248,15 @@
                          说明列的表名以及类型， 必须定义"add"、"save" 按钮， 因为添加按钮和保存按钮的定位不能自动获取
                         eg:[("列名称变量","列字段对应类型"), ...]
                         在选择时只接收label, 不支持value选择， 因为查找时也使用的label，
                         在表格只有查找功能是时，只要列属性不定义为check 都可以
         :param table_locator: 添加按钮元素上面的div定位
         :param locale: dict, 国际化文件,
         :param log_desc: str, 日志描述
-        :param action_confirm: Locator, 是否操作有确认弹窗， 如delete，
+        :param action_confirm: Locator, 弹窗中的confirm 按钮定位 是否操作有确认弹窗， 如delete，
         :param pop_up_locator: Locator, 弹窗定位, 只有在操作表格操作时如果有弹窗需要给出该定位， 如edge import config
         """
         self.columns = columns  # 列名要与实际的列相对应，不能多也不能少
         self.table_locator = table_locator
         self.locale = locale
         self.log_desc = log_desc
         self.action_confirm = action_confirm
@@ -288,22 +287,22 @@
         if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
             kwargs['save'] = True
         if kwargs.get('is_exists'):
             is_exists = kwargs.pop('is_exists')
             if not self.exist(is_exists, self.locale):
                 self.table_locator.locator('//button').first.click()
                 agg_in(self.columns, kwargs)
-                logging.info(f'table resource {kwargs} add success')
+                logging.debug(f'table resource {kwargs} add success')
             else:
-                logging.info(f'table resource {kwargs} exist')
+                logging.debug(f'table resource {kwargs} exist')
         else:
             self.table_locator.locator('//button').first.click()
             agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
-                logging.info(f'table resource {kwargs} add success')
+                logging.debug(f'table resource {kwargs} add success')
 
     def edit(self, agg_in, old_value, **kwargs) -> None:
         """ 只能编辑匹配到的第一条记录
 
         :param agg_in: function, 导致该方法不能单独使用
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
@@ -313,17 +312,17 @@
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(old_value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
             if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
             agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
-                logging.info(f'table resource {kwargs} edit success')
+                logging.debug(f'table resource {kwargs} edit success')
         else:
-            logging.info(f'table resource {old_value} not exist')
+            logging.debug(f'table resource {old_value} not exist')
 
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
@@ -331,132 +330,132 @@
         exist_tr_number = exist_tr.count()
         for i in range(0, exist_tr_number):
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
             while exist_tr.count() + i + 1 != exist_tr_number:   # 等待删除完成,
                 self.table_locator.page.wait_for_timeout(500)
-        logging.info(f'table resource {value} all delete')
+        logging.debug(f'table resource {value} all delete')
 
     def associate_delete(self, value: str) -> None:
         """
         :param value str, 关联删除按钮，如VPN 中l2tp client表格中的删除按钮
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         while exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-close"]').click()
-        logging.info(f'table resource {value} all delete associate')
+        logging.debug(f'table resource {value} all delete associate')
 
     def download(self, action, value: str, file_path: str, file_name: str = None):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str,
         :param file_path: str, 下载文件存放路径
         :param file_name: str, 下载文件名
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             action(exist_tr.first.locator('//i[@class="anticon anticon-download"]').first, file_path,
                    file_name=file_name)
-        logging.info(f'table resource {value} download success')
+        logging.debug(f'table resource {value} download success')
 
     def upload(self, action, value, file_path):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str, 待上传列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :param file_path: str, 上传文件全路径
         :return:
         """
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-upload"]').click()
             action(self.pop_up_locator.locator('.anticon.anticon-upload').nth(0), file_path)
             self.pop_up_locator.locator('.ant-btn.ant-btn-primary').nth(0).click()
-        logging.info(f'table resource {value}  click upload')
+        logging.debug(f'table resource {value}  click upload')
 
     def check(self, action, value, check_value):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str, 待check 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :param check_value: str, 待check值
         :return:
         """
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
-        logging.info(f'table resource {value}  {check_value}')
+        logging.debug(f'table resource {value}  {check_value}')
 
     def start(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-play-circle"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
-        logging.info(f'table resource {value} all start')
+        logging.debug(f'table resource {value} all start')
 
     def stop(self, value: str) -> None:
         """
         :param value str, 待停止列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-pause-circle"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
-        logging.info(f'table resource {value} all stop')
+        logging.debug(f'table resource {value} all stop')
 
     def restart(self, value: str) -> None:
         """
         :param value str, 待重启列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-undo"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
-        logging.info(f'table resource {value} all restart')
+        logging.debug(f'table resource {value} all restart')
 
     def clear_log(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-delete"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
-        logging.info(f'table resource {value} all clear log')
+        logging.debug(f'table resource {value} all clear log')
 
     def connect(self, value: str) -> None:
         """
         :param value str, WLAN 页面connect连接，每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :return:
         """
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             if exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').is_enabled():
                 exist_tr.first.locator('//button[@class="ant-btn ant-btn-background-ghost"]').click()
                 logging.info(f'table resource {value} connect success')
             else:
-                logging.info(f'table resource {value} already connected')
+                logging.debug(f'table resource {value} already connected')
 
     def delete_all(self) -> None:
         tr_locators = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr').locator(
             '//i[@class="anticon anticon-delete"]')
         while tr_locators.count() > 0:
             tr_locators.first.click()
-        logging.info('table resource all delete')
+        logging.debug('table resource all delete')
```

### Comparing `inhandtest-0.0.51/inhandtest/exception.py` & `inhandtest-0.0.52/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/file.py` & `inhandtest-0.0.52/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inmodbus.py` & `inhandtest-0.0.52/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inmongodb.py` & `inhandtest-0.0.52/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inmqtt.py` & `inhandtest-0.0.52/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inrequest.py` & `inhandtest-0.0.52/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inserial.py` & `inhandtest-0.0.52/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/insocket.py` & `inhandtest-0.0.52/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/inssh.py` & `inhandtest-0.0.52/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/ip.py` & `inhandtest-0.0.52/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/mail.py` & `inhandtest-0.0.52/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/docker_manager_locators.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/6/1 10:28:48
+# @Time    : 2023/5/25 15:58:25
 # @Author  : Pane Li
-# @File    : docker_manager_locators.py
+# @File    : edge_computing_locators.py
 """
-docker_manager_locators
+edge_computing_locators
 
 """
 from playwright.sync_api import Page
 
 
 class DockerManagerLocators:
     def __init__(self, page: Page, locale: dict):
@@ -30,21 +30,66 @@
             ('password', {'locator': self.page.locator('#password'), 'type': 'fill'}),
             ('port', {'locator': self.page.locator('#port'), 'type': 'fill'}),
         ]
 
     @property
     def docker_manager_locator(self) -> list:
         return [
-
+            ('docker_manager', {'locator': self.page.locator('#enable').nth(0), 'type': 'switch_button'}),
             ('docker_upgrade', {'locator': self.page.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
             ('docker_upgrade_confirm',
              {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button',
-              'wait_for': [{'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000},
+              'wait_for': [{'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000},   # 文件大时间就长
                            {'type': 'timeout', 'timeout': 3 * 1000}]}),
+            ('docker_upgrade_tip', {'type': 'tip_messages'}),
+            ('submit_docker_manager', {'locator': self.page.locator('.ant-btn.ant-btn-primary').nth(1), 'type': 'button'}),
+            ('portainer_manager', {'locator': self.page.locator('#enable').nth(1), 'type': 'switch_button'}),
+            ('password', {'locator': self.page.locator('#password'), 'type': 'text', }),
+            ('port', {'locator': self.page.locator('#port'), 'type': 'text', }),
+            ('submit_portainer_manager',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit).nth(1),
+              'type': 'button'}),
+            ('errors_text', {'type': 'text_messages'}),
+            ('success_tip', {'type': 'tip_messages'}),
+            ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]').nth(1),
+                       'type': 'button'}),
+        ]
+
+
+class PythonEdgeComputingLocators:
+    def __init__(self, page: Page, locale: dict):
+        self.page = page
+        self.locale = locale
+        self.pop_up = self.page.locator('.ant-modal-content')
+
+    @property
+    def python_engine_status_locator(self) -> list:
+        return [
+            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
+            ('sdk_version',
+             {'locator': self.page.locator('//span', has_text=self.locale.sdk_version).locator('../span[2]').nth(0),
+              'type': 'text'}),
+            ('python_version',
+             {'locator': self.page.locator('//span', has_text=self.locale.python_version).locator('../span[2]').nth(0),
+              'type': 'text'}),
+            ('username',
+             {'locator': self.page.locator('//span', has_text=self.locale.username).locator('../span[2]').nth(0),
+              'type': 'text'}),
+            ('used_user_storage',
+             {'locator': self.page.locator('//span', has_text=self.locale.used_user_storage).locator('../div').nth(0),
+              'type': 'text'}),
+            ('password', {'locator': self.page.locator('.anticon.anticon-copy'), 'type': 'clipboard'}),
+        ]
+
+    @property
+    def python_edge_computing_locator(self) -> list:
+        return [
             ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
+            ('sdk_upgrade', {'locator': self.page.locator('//button').nth(1), 'type': 'upload_file',
+                             'relation': [('python_engine', 'enable')]}),
             ('sdk_upgrade_confirm',
              {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button'}),
             ('sdk_upgrade_tip', {'type': 'tip_messages'}),
             ('edit_password', {'locator': self.page.locator('.anticon.anticon-form').nth(0), 'type': 'button',
                                'relation': [('python_engine', 'enable')]}),
             ('password',
              {'locator': self.page.locator('.ant-input'), 'type': 'text', 'relation': [('python_engine', 'enable')]}),
@@ -94,7 +139,11 @@
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
+
+
+class EdgeComputingLocators(PythonEdgeComputingLocators, DockerManagerLocators):
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     @allure.step('配置Python Edge Computing')
     def config(self, **kwargs):
         """
         :param kwargs:
                python_engine: enable,disable ex: python_engine='enable'
                sdk_upgrade: file_path ex: sdk_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               sdk_upgrade_tip: dict sdk_upgrade_tip={'tip_messages': 'install_success', 'timeout': 100}
                password: 123456 ex: password='123456'
                start_all_app: True, False ex: app_all_start=True
                stop_all_app: True, False ex: app_all_stop=True
                restart_all_app: True, False ex: restart_all_app=True
                app: [($action, **kwarg)] ex:
                     [('enable', 'device_supervisor', True)],   # 启用 device_supervisor
                     [('enable', 'device_supervisor', False)]   # 禁用 device_supervisor
@@ -68,25 +69,26 @@
                     [('restart', 'device_supervisor')]   # 重启 device_supervisor
                     edit parameters:
                         log_file_size: int
                         number_of_log: int
                         start_args: str  启动参数
                         error_text: str or list
                         cancel: True, False
-               submit: True,False ex: submit=True
+               submit: True,False ex: submit=True  or submit={'tip_messages': 'APP start successful'}
                error_text: str ex: error_text='ip_address_conflict'
                success_tip: ‘APP start successful’
                reset: True, False ex: reset=True
         """
         self.access_menu('edge computing.python edge computing')
         self.page.wait_for_load_state(state='networkidle')
         self.page.wait_for_timeout(1 * 1000)
         if kwargs.get('sdk_upgrade'):
-            kwargs.update(
-                {'sdk_upgrade_confirm': True, 'sdk_upgrade_tip': {'messages': 'install_success', 'timeout': 100}})
+            kwargs.update({'sdk_upgrade_confirm': True})
+            if kwargs.get('sdk_upgrade_tip') is None:
+                kwargs.update({'sdk_upgrade_tip': {'tip_messages': 'install_success', 'timeout': 100}})
         if kwargs.get('password'):
             kwargs.update({'edit_password': True, 'submit_password': True})
         if kwargs.get('app'):
             app_list_action = []
             app_status_action = []
             for action in kwargs.pop('app'):
                 if action[0] in ('enable', 'install', 'import_config', 'export_config', 'uninstall', 'edit'):
@@ -129,55 +131,37 @@
         self.page.wait_for_timeout(1000)
         return self.get_text(keys, self.edge_locators.docker_manager_status_locator)
 
     @allure.step('配置Docker Manager')
     def config(self, **kwargs):
         """
         :param kwargs:
-               python_engine: enable,disable ex: python_engine='enable'
-               sdk_upgrade: file_path ex: sdk_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               docker_manager: enable,disable ex: docker_manager='enable'
+               docker_upgrade: file_path ex: docker_upgrade='C:\\Users\\Administrator\\Downloads\\inhand-1.4.3.tar.gz'
+               docker_upgrade_tip: 'install_failure', 'install_success', ex: docker_upgrade_tip='install_success'
+               submit_docker_manager: True, False ex: submit_docker_manager=True or submit_docker_manager={'tip_messages': 'submit_success'}
+               portainer_manager: enable,disable ex: portainer_manager='enable'
                password: 123456 ex: password='123456'
-               start_all_app: True, False ex: app_all_start=True
-               stop_all_app: True, False ex: app_all_stop=True
-               restart_all_app: True, False ex: restart_all_app=True
-               app: [($action, **kwarg)] ex:
-                    [('enable', 'device_supervisor', True)],   # 启用 device_supervisor
-                    [('enable', 'device_supervisor', False)]   # 禁用 device_supervisor
-                    [('install', {'app_package': 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.tar.gz'})] # 添加 device_supervisor
-                    [('import_config', 'device_supervisor', 'C:\\Users\\Administrator\\Downloads\\device_supervisor-1.0.0.conf')] # 导入device_supervisor配置
-                    [('export_config', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.conf"})] # 导出device_supervisor配置， 文件名可以不传
-                    [('uninstall', 'device_supervisor')]   # 卸载 device_supervisor
-                    [('edit', 'device_supervisor', {'log_file_size': 1, 'number_of_log': 2, 'start_args': ''})]   # 编辑 device_supervisor
-                    [('download_log', 'device_supervisor', {'file_path': 'C:\\Users\\Administrator\\Downloads', 'file_name': "device_supervisor-1.0.0.log"})] # 导出device_supervisor日志， 文件名可以不传
-                    [('clear_log', 'device_supervisor')]   # 清除 device_supervisor 日志
-                    [('start', 'device_supervisor')]  # 启动 device_supervisor
-                    [('stop', 'device_supervisor')]   # 停止 device_supervisor
-                    [('restart', 'device_supervisor')]   # 重启 device_supervisor
-                    edit parameters:
-                        log_file_size: int
-                        number_of_log: int
-                        start_args: str  启动参数
-                        error_text: str or list
-                        cancel: True, False
-               submit: True,False ex: submit=True
+               port: 9000 ex: port='9000'
+               submit_portainer_manager: True, False ex: submit_portainer_manager=True or submit_portainer_manager={'tip_messages': 'submit_success'}
                error_text: str ex: error_text='ip_address_conflict'
-               success_tip: ‘APP start successful’
+               success_tip: ‘submit_success’
                reset: True, False ex: reset=True
         """
-        self.access_menu('edge computing.python edge computing')
+        self.access_menu('edge computing.docker manager')
         self.page.wait_for_load_state(state='networkidle')
         self.page.wait_for_timeout(1 * 1000)
-        if kwargs.get('sdk_upgrade'):
-            kwargs.update(
-                {'sdk_upgrade_confirm': True, 'sdk_upgrade_tip': {'messages': 'install_success', 'timeout': 100}})
-        if kwargs.get('password'):
-            kwargs.update({'edit_password': True, 'submit_password': True})
-        if kwargs.get('app'):
-            app_list_action = []
-            app_status_action = []
-            for action in kwargs.pop('app'):
-                if action[0] in ('enable', 'install', 'import_config', 'export_config', 'uninstall', 'edit'):
-                    app_list_action.append(action)
-                else:
-                    app_status_action.append(action)
-            kwargs.update({'app_list': app_list_action, 'app_status': app_status_action})
-        self.agg_in(self.edge_locators.python_edge_computing_locator, kwargs)
+        if kwargs.get('docker_upgrade'):
+            kwargs.update({'docker_upgrade_confirm': True})
+            if kwargs.get('docker_upgrade_tip') is None:
+                kwargs.update({'docker_upgrade_tip': {'tip_messages': 'install_success', 'timeout': 100}})
+        self.agg_in(self.edge_locators.docker_manager_locator, kwargs)
+
+
+class EdgeComputing:
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        self.python_edge: PythonEdgeComputing = PythonEdgeComputing(host, username, password, protocol, port,
+                                                                    model, language, page, locale)
+        self.docker_manager: DockerManager = DockerManager(host, username, password, protocol, port, model, language,
+                                                           page, locale)
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/edge_computing/python_edge_computing_locators.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,158 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/5/25 15:33:14
+# @Time    : 2023/6/2 14:29:16
 # @Author  : Pane Li
-# @File    : python_edge_computing_locators.py
+# @File    : system_locators.py
 """
-python_edge_computing_locators
+system_locators
 
 """
 from playwright.sync_api import Page
 
 
-class PythonEdgeComputingLocators:
+class SystemTimeLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
         self.pop_up = self.page.locator('.ant-modal-content')
+        self.utc_key = (
+            'utc-12', 'utc-11', 'utc-10', 'utc-9', 'utc-8', 'utc-7', 'utc-6', 'utc-6_atlantic', 'utc-5',
+            'utc-5_colombia', 'utc-4', 'utc-4_atlantic', 'utc-4_brazil', 'utc-3_30', 'utc-3', 'utc-3_brazil',
+            'utc-3_guyana', 'utc-2', 'utc-1', 'utc', 'utc_england,', 'utc+1', 'utc+1_france', 'utc+2', 'utc+2_greece',
+            'utc+3', 'utc+3_finland', 'utc+4', 'utc+5', 'utc+5_30', 'utc+6', 'utc+7', 'utc+8', 'utc+9', 'utc+9_30',
+            'utc+10', 'utc+11', 'utc+12', 'utc+12_zealand')
 
     @property
-    def python_engine_status_locator(self) -> list:
+    def system_time_status_locators(self) -> list:
         return [
-            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
-            ('sdk_version',
-             {'locator': self.page.locator('//span', has_text=self.locale.sdk_version).locator('../span[2]').nth(0),
+            ('local_time',
+             {'locator': self.page.locator(f'//label[text()="{self.locale.local_time}"]').locator('../../div[2]'),
               'type': 'text'}),
-            ('python_version',
-             {'locator': self.page.locator('//span', has_text=self.locale.python_version).locator('../span[2]').nth(0),
-              'type': 'text'}),
-            ('username',
-             {'locator': self.page.locator('//span', has_text=self.locale.username).locator('../span[2]').nth(0),
-              'type': 'text'}),
-            ('used_user_storage',
-             {'locator': self.page.locator('//span', has_text=self.locale.used_user_storage).locator('../div').nth(0),
-              'type': 'text'}),
-            ('password', {'locator': self.page.locator('.anticon.anticon-copy'), 'type': 'clipboard'}),
+            ('device_time',
+             {'locator': self.page.locator(f'//label[text()="{self.locale.device_time}"]').locator(
+                 '../../div[2]/div/span/div/span'), 'type': 'text'}),
         ]
 
     @property
-    def python_edge_computing_locator(self) -> list:
+    def system_time_locators(self) -> list:
         return [
-            ('python_engine', {'locator': self.page.locator('//button').nth(0), 'type': 'switch_button'}),
-            ('sdk_upgrade', {'locator': self.page.locator('//button').nth(1), 'type': 'upload_file',
-                             'relation': [('python_engine', 'enable')]}),
-            ('sdk_upgrade_confirm',
-             {'locator': self.pop_up.locator('.ant-btn.ant-btn-primary').nth(0), 'type': 'button'}),
-            ('sdk_upgrade_tip', {'type': 'tip_messages'}),
-            ('edit_password', {'locator': self.page.locator('.anticon.anticon-form').nth(0), 'type': 'button',
-                               'relation': [('python_engine', 'enable')]}),
-            ('password',
-             {'locator': self.page.locator('.ant-input'), 'type': 'text', 'relation': [('python_engine', 'enable')]}),
-            ('submit_password', {'locator': self.page.locator('.anticon.anticon-check').nth(1), 'type': 'button'}),
-            ('start_all_app', {'locator': [self.page.locator('.anticon.anticon-play-circle').nth(0),
-                                           self.page.locator('.ant-popover-inner-content').locator(
-                                               '.ant-btn.ant-btn-primary.ant-btn-sm').first],
-                               'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('stop_all_app', {'locator': [self.page.locator('.anticon.anticon-pause-circle').nth(0),
-                                          self.page.locator('.ant-popover-inner-content').locator(
-                                              '.ant-btn.ant-btn-primary.ant-btn-sm').first],
-                              'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('restart_all_app', {'locator': [self.page.locator('.anticon.anticon-undo').nth(0),
-                                             self.page.locator('.ant-popover-inner-content').locator(
-                                                 '.ant-btn.ant-btn-primary.ant-btn-sm').first],
-                                 'type': 'button', 'relation': [('python_engine', 'enable')]}),
-            ('app_list',
-             {'locator': {
-                 'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox').nth(0),
-                 'pop_up_locator': self.pop_up,
-                 'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
-                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
-                 "columns": [
-                     ('app_package',
-                      {'locator': self.pop_up.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
-                     ('log_file_size', {'locator': self.pop_up.locator('#log_size'), 'type': 'text'}),
-                     ('number_of_log', {'locator': self.pop_up.locator('#log_file_num'), 'type': 'text'}),
-                     ('start_args', {'locator': self.pop_up.locator('#start_args'), 'type': 'text'}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                 'type': 'button'}),
-                     ('save', {'locator': self.pop_up.locator(
-                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
-                         'wait_for': {'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000}}),
-                     ('errors_text', {'type': 'text_messages'}),
-                     ('success_tip', {'type': 'tip_messages'}),
-                 ]},
-                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
-            ('app_status',
-             {'locator': {
-                 'locator': self.page.locator(
-                     '.ant-table.ant-table-default.ant-table-bordered.ant-table-scroll-position-left').nth(0),
-                 'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
-                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
-             },
-                 'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
-            ('submit',
-             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
+            ('time_zone', {'locator': self.page.locator('.ant-select.ant-select-enabled').first, 'type': 'select',
+                           'param': {utc: self.locale.get(utc) for utc in self.utc_key}}),
+            ('time_zone_apply',
+             {'locator': self.page.locator('.ant-btn.ant-btn-primary.ant-btn-round').nth(0),
+              'type': 'button'}),
+            ('auto_daylight_saving_time',
+             {'locator': self.page.locator('.ant-checkbox-input'), 'type': 'check'}),
+            ('sync_time',
+             {'locator': self.page.locator('.ant-btn.ant-btn-primary.ant-btn-round').nth(1), 'type': 'button'}),
+            ('date', {'locator': self.page.locator('#date'), 'type': 'fill_date'}),
+            ('time_', {'locator': self.page.locator('.ant-time-picker'), 'type': 'fill_date'}),
+            ('apply_time',
+             {'locator': self.page.locator('.ant-btn.ant-btn-primary.ant-btn-round').nth(2), 'type': 'button'}),
+            ('enable_sntp_clients', {'locator': self.page.locator('#enable').nth(0), 'type': 'switch_button'}),
+            ('sntp_interval', {'locator': self.page.locator('#update_interval'), 'type': 'text',
+                               'relation': [('enable_sntp_clients', True)]}),
+            ('sntp_servers', {'locator': {
+                "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
+                "columns": [
+                    ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
+                    ('port', {'locator': self.pop_up.locator('#port'), 'type': 'text'}),
+                    ('errors_text', {'type': 'text_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                ]}, 'type': 'table_tr', 'relation': [('enable_sntp_clients', True)]}),
+            ('submit_sntp',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
+                                           has_text=self.locale.submit).nth(0),
+              'type': 'button'}),
+            ('enable_ntp_server', {'locator': self.page.locator('#enable').nth(1), 'type': 'switch_button'}),
+            ('pre_ntp_server', {'locator': self.page.locator('#master'), 'type': 'text',
+                                'relation': [('enable_ntp_server', True)]}),
+            ('source_interface', {'locator': self.page.locator('#source_interface'), 'type': 'select',
+                                  'relation': [('enable_ntp_server', True)]}),
+            ('source_ip', {'locator': self.page.locator('#source_ip'), 'type': 'select',
+                           'relation': [('enable_ntp_server', True)]}),
+            ('ntp_servers', {'locator': {
+                "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox'),
+                'action_confirm': self.page.locator('.ant-popover-inner').locator(
+                    '.ant-btn.ant-btn-primary.ant-btn-sm'),
+                "columns": [
+                    ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
+                    ('errors_text', {'type': 'text_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                ]}, 'type': 'table_tr'}),
+            ('submit_ntp',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
+                                           has_text=self.locale.submit).nth(1),
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
-            ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
         ]
+
+
+class LogLocators:
+    def __init__(self, page: Page, locale: dict):
+        self.page = page
+        self.locale = locale
+        self.pop_up = self.page.locator('.ant-modal-content')
+
+    @property
+    def log_locators(self) -> list:
+        return [
+            ('recent_lines',
+             {'locator': self.page.locator('.ant-select-sm.ant-select.ant-select-enabled'), 'type': 'select',
+              'param': {'all': self.locale.all_}}),
+            ('refresh_policy', {'locator': self.page.locator('.ant-select.ant-select-enabled').nth(1), 'type': 'select',
+                                'param': {'manual_refresh': self.locale.manual_refresh, 'sec': self.locale.sec,
+                                          'min': self.locale.min}}),
+            ('refresh', {'locator': self.page.locator('.ant-btn.ant-btn-sm'), 'type': 'button'}),
+            (
+                'clear_history_log',
+                {'locator': self.page.locator('//button[@class="ant-btn"]').nth(0), 'type': 'button'}),
+            ('clear_log', {'locator': self.page.locator('//button[@class="ant-btn"]').nth(1), 'type': 'button'}),
+            ('download_log', {'locator': self.page.locator('//button[@class="ant-btn"]').nth(2), 'type': 'download_file'}),
+            ('download_history_log',
+             {'locator': self.page.locator('//button[@class="ant-btn"]').nth(3), 'type': 'download_file'}),
+            ('download_diagnostic_data',
+             {'locator': self.page.locator('//button[@class="ant-btn"]').nth(4), 'type': 'download_file'}),
+            ('confirm',
+             {'locator': self.page.locator('.ant-popover-content').locator('.ant-btn.ant-btn-primary.ant-btn-sm'),
+              'type': 'button'}),
+
+        ]
+
+    @property
+    def log_config_locators(self) -> list:
+        return [
+            ('enable_remote_server', {'locator': self.page.locator('#log_to_remote_enable'), 'type': 'check'}),
+            ('remote_server', {'locator': {
+                "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
+                "columns": [
+                    ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
+                    ('port', {'locator': self.pop_up.locator('#server_port'), 'type': 'text'}),
+                    ('errors_text', {'type': 'text_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                ]}, 'type': 'table_tr', 'relation': [('enable_remote_server', True)]}),
+            ('log_to_console', {'locator': self.page.locator('#log_to_console'), 'type': 'check'}),
+            ('history_log_file_size',
+             {'locator': self.page.locator('//input[@class="ant-input-number-input"]'), 'type': 'text'}),
+            ('history_log_level',
+             {'locator': self.page.locator('.ant-select.ant-select-enabled'), 'type': 'select',
+              'param': {'emergency': self.locale.emergency, 'alarm': self.locale.alarm,
+                        'serious': self.locale.serious, 'error': self.locale.error, 'warning': self.locale.warning,
+                        'notice': self.locale.notice, 'information': self.locale.information,
+                        'debug': self.locale.debug}}),
+            ('submit',
+             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
+                                           has_text=self.locale.submit), 'type': 'button'}),
+            ('errors_text', {'type': 'text_messages'}),
+            ('success_tip', {'type': 'tip_messages'}),
+        ]
+
+
+class SystemLocators(SystemTimeLocators, LogLocators):
+    pass
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/ingateway.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 # @Time    : 2023/5/15 16:09:27
 # @Author  : Pane Li
 # @File    : ingateway.py
 """
 ingateway
 
 """
+import logging
+
 from playwright.sync_api import Page
 from inhandtest.base_page.base_page import BasePage
-from inhandtest.pages.ingateway.edge_computing.edge_computing import EdgeComputing
+from inhandtest.pages.ingateway.edge_computing.python_edge_computing import EdgeComputing
 from inhandtest.pages.ingateway.network.network import Network
 from inhandtest.pages.ingateway.overview.overview import Overview
+from inhandtest.pages.ingateway.system.system import System
 from inhandtest.pages.locale import in_setting
 from inhandtest.telnet import Telnet
 
 
 class InGateway(BasePage):
 
     def __init__(self, host: str, super_user: str, super_password: str, page: Page = None, model='IG902',
@@ -25,30 +28,23 @@
         else:
             self.telnet = None
         if self.language == 'en':
             self.telnet.send_cli(command='language English', type_='user')
         else:
             self.telnet.send_cli(command='language Chinese', type_='user')
         self.login()
-        self.overview = Overview(host, username, password, protocol, port, model, language, self.page,
-                                 locale=self.locale)
+        self.overview = Overview(host, username, password, protocol, port, model, language, self.page, self.locale)
         self.network: Network = Network(host, username, password, protocol, port, model, language, self.page,
-                                        locale=self.locale)
-        self.edge = EdgeComputing(host, username, password, protocol, port, model, language, self.page,
-                                  locale=self.locale)
+                                        self.locale)
+        self.edge = EdgeComputing(host, username, password, protocol, port, model, language, self.page, self.locale)
+        self.system = System(host, username, password, protocol, port, model, language, self.page, self.locale)
 
 
 if __name__ == '__main__':
-    import logging
-    file_handler = logging.FileHandler('./log1.log')
-    console_handler = logging.StreamHandler()
-    formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
-    file_handler.setFormatter(formatter)
-    console_handler.setFormatter(formatter)
-    logging.basicConfig(level=logging.DEBUG, handlers=[file_handler, console_handler])
-    file_handler.setLevel(logging.DEBUG)
-    console_handler.setLevel(logging.INFO)
+    from inhandtest.tools import enable_log
+
+    enable_log(console_level=logging.DEBUG)
     with InGateway('10.5.24.96', 'inhand', '64391099@inhand') as device:
-        device.network.dhcp.config_dhcp(
-            static_ip_setting=[('add', {"ip_address": '10.5.24.97', 'mac_address': '00:00:00:00:00:01'})],
-            submit=True)
-        device.page.wait_for_timeout(5 * 1000)
+        device.system.log.config(remote_server=[('add', {'server_address': 'log.server.com', 'port': 514})],
+                                 log_to_console=True, history_log_file_size=100, history_log_level='warning',
+                                 submit={'tip_messages': 'submit_success'})
+        device.page.wait_for_timeout(10 * 1000)
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/locators.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 """
 from playwright.sync_api import Page
 
 from inhandtest.pages.ingateway.edge_computing.edge_computing_locators import EdgeComputingLocators
 from inhandtest.pages.ingateway.network.network_locators import NetworkLocators
 from inhandtest.pages.ingateway.overview.overview_locators import OverviewLocators
+from inhandtest.pages.ingateway.system.system_locators import SystemLocators
 
 
 class IgLocators:
     def __init__(self, page: Page, locale):
         self.page = page
         self.locale = locale
         self.overview_locators = OverviewLocators(page, self.locale)
         self.network_locators = NetworkLocators(page, self.locale)
         self.edge_locators = EdgeComputingLocators(page, self.locale)
+        self.system_locators = SystemLocators(page, self.locale)
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/network/vpn.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/system/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,168 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/5/25 11:05:50
+# @Time    : 2023/6/2 14:29:03
 # @Author  : Pane Li
-# @File    : vpn.py
+# @File    : system.py
 """
-vpn
+system
 
 """
 import allure
 from inhandtest.tools import loop_inspector
-
 from inhandtest.base_page.base_page import BasePage
 from inhandtest.pages.ingateway.locators import IgLocators
 
 
-class Vpn(BasePage, IgLocators):
+class SystemTime(BasePage, IgLocators):
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
         IgLocators.__init__(self, page, locale)
 
-    @allure.step('断言L2tp Status状态')
-    @loop_inspector('l2tp_status')
-    def assert_l2tp_status(self, client: dict = None, server: dict = None):
-        """
-        :param client: 字典，包含以下key
-                tunnel_name:
-                l2tp_server:
-                status: disconnect, connect, disable
-                time:
-                local_ip_address
-                remote_ip_address
-                local_session_id
-                remote_session_id
-                exist: True,False ex: exist=True # True:存在,False:不存在， 默认查询存在
-        :param server: 字典，包含以下key
-               tunnel_name:
-               status: disconnect, connect, disable
-               time:
-               local_ip_address
-               remote_ip_address
-               exist: True,False ex: exist=True # True:存在,False:不存在， 默认查询存在
-        """
-        result = True
-        if client or server:
-            self.access_menu('network.vpn.l2tp.status')
-        if client is not None:
-            exist = True if client.get('exist') is None else client.pop('exist')
-            value = ''
-            for cl_ in ('tunnel_name', 'l2tp_server', 'status', 'time', 'local_ip_address', 'remote_ip_address',
-                        'local_session_id', 'remote_session_id'):
-                if client.get(cl_):
-                    value = value + client.get(cl_)
-                else:
-                    value = value + '.*'
-            if exist:
-                result = \
-                    self.table_tr(self.network_locators.l2tp_client_status_locators, [('exist', value)],
-                                  'routing status')[0]
-            else:
-                result = not \
-                    self.table_tr(self.network_locators.l2tp_client_status_locators, [('exist', value)],
-                                  'routing status')[0]
-        if server is not None:
-            exist = True if server.get('exist') is None else server.pop('exist')
-            value = ''
-            for cl_ in ('tunnel_name', 'status', 'time', 'local_ip_address', 'remote_ip_address'):
-                if server.get(cl_):
-                    value = value + server.get(cl_)
-                else:
-                    value = value + '.*'
-            if exist:
-                result = \
-                    self.table_tr(self.network_locators.l2tp_server_status_locators, [('exist', value)],
-                                  'routing status')[0]
-            else:
-                result = not \
-                    self.table_tr(self.network_locators.l2tp_server_status_locators, [('exist', value)],
-                                  'routing status')[0]
-        return result
-
-    @allure.step('配置L2tp Client')
-    def config_l2tp_client(self, **kwargs):
-        """ 注意如果是删除，需要先删除关联项，再删除本身，否则多次删除会删除不了
+    @allure.step('断言系统时间状态')
+    @loop_inspector('system_time_status')
+    def assert_status(self, **kwargs):
+        """
+
+        :param kwargs:
+                     local_time: 00:00:00 ex: connect_time='"${value}".startswith("00:00")'
+                     device_time: 00:00:00 ex: connect_time='"${value}".startswith("00:00")'
+        :return:
+        """
+        self.access_menu('system.system_time')
+        return self.eval_locator_attribute(kwargs, self.system_locators.system_time_status_locators)
+
+    @allure.step('获取系统时间')
+    def get_status(self, keys: str or list or tuple) -> str or dict or None:
+        """
+
+        :param keys: local_time device_time
+
+        :return: 当key为列表或者元组时， 使用字典返回相关关键字的信息
+        """
+        self.access_menu('system.system_time')
+        return self.get_text(keys, self.system_locators.system_time_status_locators)
+
+    @allure.step('配置系统时间')
+    def config(self, **kwargs):
+        """ 配置系统时间, 无需配置时均不填写参数
 
         :param kwargs:
-            l2tp_class:
-               [($action, **kwarg)] ex: [('delete_all', )],
-                [('delete', 'nameyes')]
-                [('add', {'name': 'name', 'auth': 'yes', 'hostname': hostname, 'challenge_secret': challenge_secret})]
-                    add parameter:
-                        name:
-                        auth: yes, no
-                        hostname:
-                        challenge_secret:
-                        errors_text: str or list
-                        cancel: True, False
-                [('add', {'name': 'name', 'hostname': hostname, 'is_exists': 'nameyes'})] 如果存在则不添加
-                [('edit', 'nameyes', {'name': 'name1'})]
-                [('associate_delete', 'nameyes')]   # 删除关联项
-            pseudowire_class:
-               [($action, **kwarg)] ex: [('delete_all', )],
-                [('delete', 'namel2tp_class')]
-                [('add', {'name': 'name', 'l2tp_class': l2tp_class, 'source_interface': source_interface, 'data_encapsulation_method': data_encapsulation_method, 'tunnel_management_protocol': tunnel_management_protocol})]'})]
-                    add parameter:
-                        name:
-                        l2tp_class: l2tp_class
-                        source_interface: 'Cellular 1', 'Bridge 1'
-                        data_encapsulation_method: 'L2TPv2', 'L2TPv3'
-                        tunnel_management_protocol: 'L2TPv2', 'NONE', 'L2TPv3'
-                        errors_text: str or list
-                        cancel: True, False
-                [('add', {'name': 'name', 'l2tp_class': l2tp_class, 'is_exists': 'namel2tp_class'})] 如果存在则不添加
-                [('edit', 'namel2tp_class', {'name': 'name1'})]
-                [('associate_delete', 'namel2tp_class')]   # 删除关联项
-            l2tpv2_tunnel:
-               [($action, **kwarg)] ex: [('delete_all', )],
-                [('delete', 'id')]
-                [('add', {'enable': True, 'id': id, 'l2tp_server': l2tp_server, 'pseudowire_class': pseudowire_class, 'auth_type': auth_type, 'username': username, 'password': password, 'local_ip_address': local_ip_address})]
-                    add parameter:
-                        enable: True, False
-                        id: str or int
-                        l2tp_server:
-                        pseudowire_class:
-                        auth_type: 'AUTO', 'PAP', 'CHAP'
-                        username: str
-                        password: str
-                        local_ip_address: str
-                        remote_ip_address: str
-                        errors_text: str or list
-                        cancel: True, False
-                [('add', {'enable': True, 'id': id, 'is_exists': 'id'})] 如果存在则不添加
-                [('edit', 'id', {'enable': False})]
-                [('associate_delete', 'id')]   # 删除关联项
-            l2tpv3_tunnel:
-               [($action, **kwarg)] ex: [('delete_all', )],
-                [('delete', 'id')]
-                [('add', {'enable': True, 'id': id, 'peer_id': peer_id})]
-                    add parameter:
-                        enable: True, False
-                        id: str or int
-                        peer_id:
-                        pseudowire_class:
-                        protocol: 'IP', 'UDP'
-                        source_port: int
-                        destination_port: int
-                        xconnect_interface: str
-                        errors_text: str or list
-                        cancel: True, False
-                [('add', {'enable': True, 'id': id, 'is_exists': 'id'})] 如果存在则不添加
-                [('edit', 'id', {'enable': False})]
-                [('associate_delete', 'id')]   # 删除关联项
-            l2tpv3_session:
-               [($action, **kwarg)] ex: [('delete_all', )],
-                [('delete', 'local_session_id')]
-                [('add', {'local_session_id': local_session_id, 'remote_session_id': remote_session_id})]
-                    add parameter:
-                        local_session_id: str or int
-                        remote_session_id: str or int
-                        local_tunnel_id:
-                        local_session_ip_address:
-                        errors_text: str or list
-                        cancel: True, False
-                [('add', {'local_session_id': local_session_id, 'is_exists': 'local_session_id'})] 如果存在则不添加
-                [('edit', 'local_session_id', {'local_session_id': local_session_id})]
-                [('associate_delete', 'local_session_id')]   # 删除关联项
-            submit: True,False ex: submit=True
-            errors_text: str or list
-            success_tip: True,False ex: success_tip=True
-            reset: True,False ex: reset=True
+               time_zone: utc-12, utc-11, utc-10, utc-9, utc-8, utc-7, utc-6, utc-6_atlantic, utc-5, utc-5_colombia,
+                          utc-4, utc-4_atlantic, utc-4_brazil, utc-3_30, utc-3, utc-3_brazil, utc-3_guyana, utc-2, utc-1, utc, utc_england,
+                          utc+1, utc+1_france, utc+2, utc+2_greece, utc+3, utc+3_finland, utc+4, utc+5, utc+5_30, utc+6,
+                          utc+7, utc+8, utc+9, utc+9_30, utc+10, utc+11, utc+12, utc+12_zealand
+               time_zone_apply： True, False  ex time_zone_apply=True or time_zone_apply={'tip_messages': 'apply_success'}
+               auto_daylight_saving_time: enable, disable ex: auto_daylight_saving_time='enable'
+               sync_time: True, False ex: sync_time=True  or sync_time={'tip_messages': 'sync_success'}
+               date: 2021-06-02 ex: date='2021-06-02'
+               time_: 00:00:00 ex: time_='00:00:00'
+               apply_time: True, False ex: apply_time=True or apply_time={'tip_messages': 'apply_success'}
+
+               enable_sntp_clients: True, False ex: enable_sntp_clients=True
+               sntp_interval: 60 ex: sntp_interval=60
+               sntp_servers: [($action, **kwarg)]
+                  ex: [('delete_all', )],
+                 [('delete', '0.pool.ntp.org')]
+                 [('add', {'server_address': '0.pool.ntp.org', 'port': '4444'})]
+                     add parameter:
+                     server_address:  0.pool.ntp.org ex: server_address="0.pool.ntp.org"
+                     port: 4444 ex: port=4444
+                     error_text: str or list
+                     cancel: True, False
+                 [('add', {'server_address': '0.pool.ntp.org', 'port': '4444', 'is_exists': '0.pool.ntp.org'})] 如果存在0.pool.ntp.org则不添加
+                 [('edit', '0.pool.ntp.org', {'server_address': '1.pool.ntp.org'})]
+                 多个操作时使用列表 [('add',{}), ('add',{})]
+               submit_sntp: True, False ex: submit_sntp=True or submit_sntp={'tip_messages': 'submit_success'}
+
+               enable_ntp_server: True, False ex: enable_ntp_server=True
+               pre_ntp_server: server_address ex: pre_ntp_server='0.pool.ntp.org'
+               source_interface: Cellular 1、Bridge 1 ex: source_interface='Cellular 1'
+               source_ip: 192.168.2.1 ex: source_ip='192.168.2.1'
+               ntp_servers: [($action, **kwarg)]
+                 ex: [('delete_all', )],
+                 [('delete', '0.pool.ntp.org')]
+                 [('add', {'server_address': '0.pool.ntp.org'})]
+                     add parameter:
+                     server_address:  0.pool.ntp.org ex: server_address="0.pool.ntp.org"
+                     error_text: str or list
+                     cancel: True, False
+                 [('add', {'server_address': '0.pool.ntp.org',  'is_exists': '0.pool.ntp.org'})] 如果存在0.pool.ntp.org则不添加
+                 [('edit', '0.pool.ntp.org', {'server_address': '1.pool.ntp.org'})]
+                 [('enable', '0.pool.ntp.org', True)] or  [('enable', '0.pool.ntp.org', False)]
+               error_text: str or list or tuple
+               submit_ntp: True or False ex: submit_ntp=True  or  submit_ntp={'tip_messages': 'apply_success'}
+               success_tip: True or False ex: success_tip=True or success_tip={'tip_messages': 'apply_success'}
         :return:
         """
-        self.access_menu('network.vpn.l2tp.l2tp client')
-        if kwargs.get('success_tip'):
-            kwargs.update({'success_tip': 'submit_success'})
-        self.agg_in(self.network_locators.l2tp_client_locators, kwargs)
+        self.access_menu('system.system_time')
+        self.agg_in(self.system_locators.system_time_locators, kwargs)
+
+
+class Log(BasePage, IgLocators):
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
+        IgLocators.__init__(self, page, locale)
+
+    @allure.step('操作系统日志')
+    def log(self, **kwargs):
+        """
 
-    @allure.step('配置L2tp Service')
-    def config_l2tp_service(self, **kwargs):
+        :param kwargs:
+                     recent_lines: 20,50,100,200,all ex: recent_lines='all'
+                     refresh_policy: manual_refresh, 5sec, 10sec, 15sec, 30sec, 1min, 2min, 3min, 4min, 5min, 10min, 15min, 20min, 30min
+                                     ex: refresh_policy='manual_refresh'
+                     refresh: True, False ex: refresh=True or refresh={'wait_for_time': 3* 1000}
+                     clear_history_log: True, False ex: clear_history_log=True
+                     clear_log: True, False ex: clear_log=True
+                     download_log: {'file_path': $file_path, 'file_name': $file_name} ex: download_log={'file_path': './tmp', 'file_name': 'log.log'}
+                     download_history_log: {'file_path': $file_path, 'file_name': $file_name} ex: download_history_log={'file_path': './tmp', 'file_name': 'log.log'}
+                     download_diagnostic_data: {'file_path': $file_path, 'file_name': $file_name} ex: download_diagnostic_data={'file_path': './tmp', 'file_name': 'log.log'}
+        :return:
         """
+        self.access_menu('system.log.log')
+        if kwargs.get('refresh_policy') == 'manual_refresh' and kwargs.get('refresh') is None:
+            kwargs.update({'refresh': {'wait_for_time': 3 * 1000}})
+        if kwargs.get('clear_history_log') or kwargs.get('clear_log'):
+            kwargs.update({'confirm': {'tip_messages': 'log_cleared'}})
+        self.agg_in(self.system_locators.log_locators, kwargs)
+
+    @allure.step('配置系统日志')
+    def config(self, **kwargs):
+        """ 配置系统时间, 无需配置时均不填写参数
 
         :param kwargs:
-            enable： True,False ex: enable=True
-            username: str
-            password: str
-            auth_type: 'AUTO', 'PAP', 'CHAP'
-            local_ip_address: str
-            client_start_ip: str
-            client_end_ip: str
-            link_detection_interval:  int
-            max_retries_for_link: int
-            enable_mppe: True,False ex: enable_mppe=True
-            enable_tunnel_auth: True,False ex: enable_tunnel_auth=True
-            export_options: str
-            submit: True,False ex: submit=True
-            errors_text: str or list
-            success_tip: True,False ex: success_tip=True
-            reset: True,False ex: reset=True
+               enable_remote_server: True, False ex: enable_remote_server=True
+               remote_server: [($action, **kwarg)]
+                  ex: [('delete_all', )],
+                 [('delete', 'log.server.com')]
+                 [('add', {'server_address': 'log.server.com', 'port': '4444'})]
+                     add parameter:
+                     server_address:  0.pool.ntp.org ex: server_address="0.pool.ntp.org"
+                     port: 4444 ex: port=4444
+                     error_text: str or list
+                     cancel: True, False
+                 [('add', {'server_address': 'log.server.com', 'port': '4444', 'is_exists': 'log.server.com'})] 如果存在0.pool.ntp.org则不添加
+                 [('edit', 'log.server.com', {'server_address': 'log.server.com.cn'})]
+                 多个操作时使用列表 [('add',{}), ('add',{})]
+               log_to_console： check, uncheck  ex log_to_console='check'
+               history_log_file_size: str, int ex: history_log_file_size='100' or history_log_file_size=100
+               history_log_level: debug, information, notice, warning, error, serious, alarm, emergency ex: history_log_level='debug'
+               error_text: str or list or tuple
+               submit: True or False ex: submit=True  or  submit={'tip_messages': 'submit_success'}
+               success_tip: True or False ex: success_tip=True or success_tip={'tip_messages': 'submit_success'}
         :return:
         """
-        self.access_menu('network.vpn.l2tp.l2tp service')
-        if kwargs.get('success_tip'):
-            kwargs.update({'success_tip': 'submit_success'})
-        self.agg_in(self.network_locators.l2tp_service_locators, kwargs)
+        self.access_menu('system.log.configure')
+        self.agg_in(self.system_locators.log_config_locators, kwargs)
+
+
+class System:
+
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='IG902', language='en', page=None, locale: dict = None):
+        self.system_time: SystemTime = SystemTime(host, username, password, protocol, port, model, language, page,
+                                                  locale)
+        self.log: Log = Log(host, username, password, protocol, port, model, language, page, locale)
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
         IgLocators.__init__(self, page, locale)
 
     @allure.step('断言概览状态')
     @loop_inspector('overview status')
-    def assert_overview_status(self, **kwargs):
+    def assert_status(self, **kwargs):
         """
         assert overview status
         :param kwargs:  wan_image: 检查外网图标状态，ex: wan_image='"${value}" =="enable"'
                                                  or wan_status='"${value}" !="enable"'
                         wan_ip: 检查wan ip，ex: wan_ip='"${value}" =="0.0.0.0"'
                         wan_gateway: 检查wan gateway，ex: wan_gateway='"${value}" =="10.5.24.254"'
                         wan_dns: 检查wan dns，ex: wan_dns='"${value}" =="0.0.0.0"'
@@ -66,16 +66,16 @@
                         timeout: 超时时间
                         interval: 检查间隔
         :return:
         """
         self.access_menu('overview')
         return self.eval_locator_attribute(kwargs, self.overview_locators.overview_locators)
 
-    @allure.step('偶去概览信息')
-    def get_overview_status(self, keys: str or list or tuple) -> str or dict or None:
+    @allure.step('获取概览信息')
+    def get_status(self, keys: str or list or tuple) -> str or dict or None:
         """
         get overview status
         :param keys: 同assert_overview_status keys
         :return: 当key为列表或者元组时， 使用字典返回相关关键字的信息
         """
         self.access_menu('overview')
         return self.get_text(keys, self.overview_locators.overview_locators)
```

### Comparing `inhandtest-0.0.51/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.52/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/pytest_email.html` & `inhandtest-0.0.52/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.51/inhandtest/telnet.py` & `inhandtest-0.0.52/inhandtest/telnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,17 +648,17 @@
         @return:
         """
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
-    import sys
+    from inhandtest.tools import enable_log
 
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.DEBUG, stream=sys.stdout)
+    enable_log('./log.log')
     device = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
     # device.tcpdump(expect='10.5.24.224.62227', interface='eth0.4094',)
     device.send_cli('ifconfig', '/www #', 'super')
 
     # device = Telnet('IG902', '
     # device = Telnet('VG710', '10.5.24.206', 'inhand', '64391099@inhand')
     # a = device.send_cli('ping www.baidu.com -c 4', '/www #', 'super')
```

### Comparing `inhandtest-0.0.51/inhandtest/tools.py` & `inhandtest-0.0.52/inhandtest/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,30 +218,42 @@
 def kill_windows_port(ip_, port: int or list) -> None:
     """ 杀死windows 相关端口服务
 
     :param ip_: 本机IP地址
     :param port: int|list, 端口号，可以是多个
     """
     import psutil
+    import socket
 
     def kill_one_port(one_port: int):
         for proc in psutil.process_iter(['pid', 'name']):
             try:
                 conn_list = proc.connections()
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 continue
             for conn in conn_list:
                 if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
                     logging.debug(f"process {proc.pid} already use port {one_port}")
                     # 终止进程
                     proc.kill()
-                    time.sleep(3)
                     logging.info(f"kill process {proc.pid} success")
 
+    def port_is_close(one_port: int):  # 杀死后要一直等到进程完全退出才能继续执行，否则会报错
+        for i in range(0, 15):
+            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+                try:
+                    s.bind((ip_, one_port))
+                    time.sleep(1)
+                except socket.error:
+                    break
+        else:
+            raise Exception(f"kill process {one_port} failed")
+
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
+    [port_is_close(port_) for port_ in port] if isinstance(port, list) else port_is_close(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
     """输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言
 
     :param command: 输入的一条或多条命令，注意操作者的权限
     :param expect: str or list or dict, 一条或多条希望校验的存在的结果，如需要判断不存在时，可以使用字典{$expect: False}
@@ -582,14 +594,44 @@
         except:
             pass
     else:
         logging.debug(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
+def enable_log(filename: str = None, console_level=logging.INFO):
+    """
+
+    :param filename:  日志文件名称 ex: './test.log'
+    :param console_level: logging.INFO, logging.DEBUG
+    :return:
+    """
+    import colorlog
+    console_handler = logging.StreamHandler()
+    formatter = colorlog.ColoredFormatter(
+        '%(log_color)s%(asctime)s %(levelname)s [%(module)s]:%(message)s',
+        log_colors={
+            'DEBUG': 'blue',
+            'INFO': 'green',
+            'WARNING': 'yellow',
+            'ERROR': 'red',
+            'CRITICAL': 'red,bg_white',
+        }
+    )
+    console_handler.setFormatter(formatter)
+    if filename is not None:
+        file_handler = logging.FileHandler(filename)  # 日志文件及名称
+        file_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s [%(module)s]:%(message)s'))
+        logging.basicConfig(level=logging.DEBUG, handlers=[file_handler, console_handler])
+        file_handler.setLevel(logging.DEBUG)
+    else:
+        logging.basicConfig(level=logging.DEBUG, handlers=[console_handler])
+    console_handler.setLevel(console_level)
+
+
 class DotDict(dict):
     """使用点号深度获取字典key的值
 
     """
 
     def __getattr__(self, key):
         try:
```

### Comparing `inhandtest-0.0.51/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.52/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.51
+Version: 0.0.52
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.51/setup.py` & `inhandtest-0.0.52/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.51',
+    version='0.0.52',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
@@ -25,11 +25,11 @@
     package_data={'inhandtest': ['pytest_email.html'], 'inhandtest.pages.ingateway': ['*.yml']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
-                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf'
+                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf', 'colorlog'
                       # 这里是依赖列表，表示运行这个包的运行某些功能还需要你安装其他的包
                       ],
 )
```

