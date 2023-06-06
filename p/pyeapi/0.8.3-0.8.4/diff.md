# Comparing `tmp/pyeapi-0.8.3.tar.gz` & `tmp/pyeapi-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyeapi-0.8.3.tar", last modified: Mon Jan 27 18:41:49 2020, max compression
+gzip compressed data, was "dist/pyeapi-0.8.4.tar", last modified: Fri Nov 13 13:45:15 2020, max compression
```

## Comparing `pyeapi-0.8.3.tar` & `pyeapi-0.8.4.tar`

### file list

```diff
@@ -1,155 +1,183 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      479 2020-01-26 11:50:00.000000 pyeapi-0.8.3/examples/get_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2020-01-26 11:50:00.000000 pyeapi-0.8.3/examples/simple.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      778 2020-01-26 11:50:00.000000 pyeapi-0.8.3/examples/vlans_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2020-01-26 11:50:00.000000 pyeapi-0.8.3/examples/nodes.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2020-01-26 11:50:00.000000 pyeapi-0.8.3/examples/sysmac.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1488 2020-01-26 11:50:00.000000 pyeapi-0.8.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2020-01-26 11:50:00.000000 pyeapi-0.8.3/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2020-01-26 11:50:00.000000 pyeapi-0.8.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2020-01-26 11:50:00.000000 pyeapi-0.8.3/.coveragerc
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2020-01-26 11:50:00.000000 pyeapi-0.8.3/CHANGELOG.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2020-01-26 12:01:24.000000 pyeapi-0.8.3/VERSION
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3596 2020-01-26 11:50:00.000000 pyeapi-0.8.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2020-01-26 11:50:00.000000 pyeapi-0.8.3/dev-requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1766 2020-01-26 11:50:00.000000 pyeapi-0.8.3/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1687 2020-01-27 18:41:49.000000 pyeapi-0.8.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2020-01-27 18:41:49.000000 pyeapi-0.8.3/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1275 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.8.2.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.2.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4060 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.4.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.1.0.rst
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     2841 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/generate_modules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      392 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.6.1.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.2.2.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/license.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.2.1.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7111 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/configfile.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.7.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1867 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.6.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1245 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.8.1.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3996 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/install.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3964 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/quickstart.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.1.1.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      360 2020-01-26 12:00:44.000000 pyeapi-0.8.3/docs/release-notes-0.8.3.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      361 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/requirements.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      623 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7012 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1120 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.3.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      870 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/description.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/modules.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.2.4.rst
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10775 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1305 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/subinterfaces.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2704 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.5.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.3.3.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/support.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/contribute.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3700 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.8.0.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.3.1.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.3.2.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      121 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/examples.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2020-01-26 11:50:00.000000 pyeapi-0.8.3/docs/release-notes-0.2.3.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40044 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/interfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9666 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/ipinterfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/vlans.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8273 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/varp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6781 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11123 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/acl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12370 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/vrfs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11793 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/users.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8043 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/abstract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7261 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/ntp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    61008 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/vrrp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13376 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/ospf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13395 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/bgp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14591 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/routemaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1619 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1712 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/spanningtree.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14275 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/staticroute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10972 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/mlag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16675 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/switchports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13541 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/api/stp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33172 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1712 2020-01-26 12:01:45.000000 pyeapi-0.8.3/pyeapi/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7560 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23686 2020-01-26 11:50:00.000000 pyeapi-0.8.3/pyeapi/eapilib.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/test/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/test/system/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7936 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_ntp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9596 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11542 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_mlag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12500 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_varp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9101 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_ospf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14937 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14942 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_vrfs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10326 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_acl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8594 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_vlans.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6103 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_ipinterfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10836 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_staticroute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6199 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_switchports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9678 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_users.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29074 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_interfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6185 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_stp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12357 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_routemaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22511 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/system/test_api_vrrp.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/test/unit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3039 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4425 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_ntp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4292 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6632 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_mlag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6111 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_varp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18863 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_bgp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_ospf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18882 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7339 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_vrfs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11353 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_acl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9951 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_eapilib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6169 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_vlans.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5868 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_ipinterfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11572 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_staticroute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8565 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_switchports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5741 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_users.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23391 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_interfaces.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7678 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_stp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7017 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_routemaps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31011 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/unit/test_api_vrrp.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/test/fixtures/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/empty.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.bgp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      685 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/vxlan.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      233 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/eapi.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2475 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/ipinterfaces.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43923 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.text
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      402 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/show_version.text
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8955 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.portchannel
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.vxlan
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/eapi.conf.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/show_portchannel.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      409 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.varp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/env_path.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      894 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.ospf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.routemaps
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7185 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/show_interfaces.text
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.varp_null
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/dut.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/nohost.conf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19736 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/show_interfaces.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/show_version.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13343 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.vrrp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5542 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/fixtures/running_config.vrf
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/test/lib/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2896 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/lib/systestlib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4253 2020-01-26 11:50:00.000000 pyeapi-0.8.3/test/lib/testlib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2020-01-26 12:32:42.000000 pyeapi-0.8.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3624 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1687 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2020-01-27 18:41:49.000000 pyeapi-0.8.3/pyeapi.egg-info/requires.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/docs/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/docs/api_modules/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      297 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/_list_of_modules.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      200 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/abstract.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      185 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/acl.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      185 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/bgp.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      206 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/interfaces.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      212 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/ipinterfaces.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      188 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/mlag.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      185 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/ntp.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      188 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/ospf.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      203 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/routemaps.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      212 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/spanningtree.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      209 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/staticroute.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      185 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/stp.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      209 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/switchports.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      194 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/system.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      191 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/users.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      188 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/varp.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      191 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/vlans.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      188 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/vrfs.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      188 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/api_modules/vrrp.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/docs/client_modules/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/client_modules/_list_of_modules.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      190 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/client_modules/client.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      193 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/client_modules/eapilib.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      187 2020-11-13 13:04:55.000000 pyeapi-0.8.4/docs/client_modules/utils.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7012 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/Makefile
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)    10775 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/conf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7111 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/configfile.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1680 2020-11-13 13:36:09.000000 pyeapi-0.8.4/docs/configsessions.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1058 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/contribute.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      870 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/description.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      121 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/examples.rst
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2841 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/generate_modules.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1120 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/index.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3996 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/install.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1504 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/license.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      114 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/modules.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3964 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/quickstart.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      234 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.1.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      459 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.1.1.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      474 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.2.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       97 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.2.1.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      106 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.2.2.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       88 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.2.3.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       84 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.2.4.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      304 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.3.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      228 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.3.1.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      105 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.3.2.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      155 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.3.3.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4060 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.4.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2704 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.5.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1867 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.6.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      392 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.6.1.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.7.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3700 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.8.0.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1245 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.8.1.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1275 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.8.2.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      360 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes-0.8.3.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      221 2020-11-13 13:36:09.000000 pyeapi-0.8.4/docs/release-notes-0.8.4.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      623 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/release-notes.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      361 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/requirements.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1305 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/subinterfaces.rst
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1176 2020-11-13 12:18:57.000000 pyeapi-0.8.4/docs/support.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/examples/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      479 2020-11-13 12:18:57.000000 pyeapi-0.8.4/examples/get_config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      149 2020-11-13 12:18:57.000000 pyeapi-0.8.4/examples/nodes.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      260 2020-11-13 12:18:57.000000 pyeapi-0.8.4/examples/simple.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      259 2020-11-13 12:18:57.000000 pyeapi-0.8.4/examples/sysmac.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      778 2020-11-13 12:18:57.000000 pyeapi-0.8.4/examples/vlans_api.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi/api/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1619 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8043 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/abstract.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11123 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/acl.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13395 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/bgp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    40052 2020-11-13 13:36:09.000000 pyeapi-0.8.4/pyeapi/api/interfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9666 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/ipinterfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    10972 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/mlag.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7261 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/ntp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13376 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/ospf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14591 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/routemaps.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1712 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/spanningtree.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14275 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/staticroute.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13541 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/stp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16675 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/switchports.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6781 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/system.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11793 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/users.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8273 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/varp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11773 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/vlans.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12370 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/vrfs.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    61008 2020-11-13 12:18:57.000000 pyeapi-0.8.4/pyeapi/api/vrrp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1712 2020-11-13 13:36:09.000000 pyeapi-0.8.4/pyeapi/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    35204 2020-11-13 13:36:09.000000 pyeapi-0.8.4/pyeapi/client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    23841 2020-11-13 13:36:09.000000 pyeapi-0.8.4/pyeapi/eapilib.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7737 2020-11-13 13:36:09.000000 pyeapi-0.8.4/pyeapi/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1721 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4388 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       72 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        7 2020-11-13 13:45:15.000000 pyeapi-0.8.4/pyeapi.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/test/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/test/fixtures/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       89 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/dut.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      233 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/eapi.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       82 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/eapi.conf.yaml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/empty.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       91 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/env_path.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2475 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/ipinterfaces.json
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       19 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/nohost.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      476 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.bgp
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      894 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.ospf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8955 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.portchannel
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      922 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.routemaps
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    43923 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.text
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      409 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.varp
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      508 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.varp_null
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5542 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.vrf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13343 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.vrrp
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1544 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/running_config.vxlan
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19736 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/show_interfaces.json
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7185 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/show_interfaces.text
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      191 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/show_portchannel.json
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      458 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/show_version.json
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      402 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/show_version.text
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      685 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/fixtures/vxlan.json
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/test/lib/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2896 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/lib/systestlib.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4253 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/lib/testlib.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/test/system/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    10326 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_acl.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    29085 2020-11-13 13:36:09.000000 pyeapi-0.8.4/test/system/test_api_interfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6103 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_ipinterfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11542 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_mlag.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7936 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_ntp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9101 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_ospf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12357 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_routemaps.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    10836 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_staticroute.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6185 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_stp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6199 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_switchports.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9596 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_system.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9678 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_users.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12500 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_varp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8594 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_vlans.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14942 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_vrfs.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22511 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_api_vrrp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14937 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/system/test_client.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2020-11-13 13:45:15.000000 pyeapi-0.8.4/test/unit/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11353 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_acl.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18863 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_bgp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    23399 2020-11-13 13:36:09.000000 pyeapi-0.8.4/test/unit/test_api_interfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5868 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_ipinterfaces.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6632 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_mlag.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4425 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_ntp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5941 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_ospf.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7017 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_routemaps.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11572 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_staticroute.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7678 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_stp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8565 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_switchports.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4292 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_system.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5741 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_users.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6111 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_varp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6169 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_vlans.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7339 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_vrfs.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    31011 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_api_vrrp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18882 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9951 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_eapilib.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3039 2020-11-13 12:18:57.000000 pyeapi-0.8.4/test/unit/test_utils.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      656 2020-11-13 12:18:57.000000 pyeapi-0.8.4/.coveragerc
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      164 2020-11-13 12:18:57.000000 pyeapi-0.8.4/CHANGELOG.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1488 2020-11-13 12:18:57.000000 pyeapi-0.8.4/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      724 2020-11-13 12:18:57.000000 pyeapi-0.8.4/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1766 2020-11-13 12:18:57.000000 pyeapi-0.8.4/Makefile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3596 2020-11-13 12:18:57.000000 pyeapi-0.8.4/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2020-11-13 13:36:09.000000 pyeapi-0.8.4/VERSION
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      152 2020-11-13 12:18:57.000000 pyeapi-0.8.4/dev-requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2020-11-13 12:18:57.000000 pyeapi-0.8.4/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2963 2020-11-13 13:36:09.000000 pyeapi-0.8.4/setup.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1721 2020-11-13 13:45:15.000000 pyeapi-0.8.4/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2020-11-13 13:45:15.000000 pyeapi-0.8.4/setup.cfg
```

### Comparing `pyeapi-0.8.3/examples/vlans_api.py` & `pyeapi-0.8.4/examples/vlans_api.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/LICENSE` & `pyeapi-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/MANIFEST.in` & `pyeapi-0.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/.coveragerc` & `pyeapi-0.8.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/README.md` & `pyeapi-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/Makefile` & `pyeapi-0.8.4/Makefile`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/PKG-INFO` & `pyeapi-0.8.4/pyeapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: pyeapi
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Client for eAPI
 Home-page: https://github.com/arista-eosplus/pyeapi
 Author: Arista EOS+ CS
 Author-email: eosplus-dev@arista.com
 License: BSD-3
+Description-Content-Type: UNKNOWN
 Description: The Python Client for eAPI
         ==========================
         
         The Python Client for eAPI (pyeapi) is a native Python library wrapper around
         Arista EOS eAPI.  It provides a set of Python language bindings for configuring
         Arista EOS nodes.
```

### Comparing `pyeapi-0.8.3/docs/release-notes-0.8.2.rst` & `pyeapi-0.8.4/docs/release-notes-0.8.2.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.4.0.rst` & `pyeapi-0.8.4/docs/release-notes-0.4.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/generate_modules.py` & `pyeapi-0.8.4/docs/generate_modules.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/license.rst` & `pyeapi-0.8.4/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/configfile.rst` & `pyeapi-0.8.4/docs/configfile.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.7.0.rst` & `pyeapi-0.8.4/docs/release-notes-0.7.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.6.0.rst` & `pyeapi-0.8.4/docs/release-notes-0.6.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.8.1.rst` & `pyeapi-0.8.4/docs/release-notes-0.8.1.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/install.rst` & `pyeapi-0.8.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/quickstart.rst` & `pyeapi-0.8.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes.rst` & `pyeapi-0.8.4/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/Makefile` & `pyeapi-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/index.rst` & `pyeapi-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/description.rst` & `pyeapi-0.8.4/docs/description.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/conf.py` & `pyeapi-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/subinterfaces.rst` & `pyeapi-0.8.4/docs/subinterfaces.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.5.0.rst` & `pyeapi-0.8.4/docs/release-notes-0.5.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/support.rst` & `pyeapi-0.8.4/docs/support.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/contribute.rst` & `pyeapi-0.8.4/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/docs/release-notes-0.8.0.rst` & `pyeapi-0.8.4/docs/release-notes-0.8.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/interfaces.py` & `pyeapi-0.8.4/pyeapi/api/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
             * name (str): The name of the interface
             * type (str): Always returns 'vxlan'
             * source_interface (str): The vxlan source-interface value
             * multicast_group (str): The vxlan multicast-group value
             * udp_port (int): The vxlan udp-port value
             * vlans (dict): The vlan to vni mappings
             * flood_list (list): The list of global VTEP flood list
-            * multicast_decap (bool): If the mutlicast decap
+            * multicast_decap (bool): If the multicast decap
                                       feature is configured
 
         Args:
             name (str): The interface identifier to retrieve from the
                 running-configuration
 
         Returns:
@@ -880,15 +880,15 @@
         match = re.search(r'vxlan multicast-group '
                           r'([\d]{3}\.[\d]+\.[\d]+\.[\d]+)',
                           config)
         value = match.group(1) if match else self.DEFAULT_MCAST_GRP
         return dict(multicast_group=value)
 
     def _parse_multicast_decap(self, config):
-        value = 'vxlan mutlicast-group decap' in config
+        value = 'vxlan multicast-group decap' in config
         return dict(multicast_decap=bool(value))
 
     def _parse_udp_port(self, config):
         match = re.search(r'vxlan udp-port (\d+)', config)
         value = int(match.group(1))
         return dict(udp_port=value)
 
@@ -1060,15 +1060,15 @@
             vlan (str, int): The vlan id to map to the vni
             vni (str, int): The vni value to use
 
         Returns:
             True if the command completes successfully
 
         """
-        cmd = 'vxlan vlan %s vni %s' % (vid, vni)
+        cmd = 'vxlan vlan add %s vni %s' % (vid, vni)
         return self.configure_interface(name, cmd)
 
     def remove_vlan(self, name, vid):
         """Removes a vlan to vni mapping for the interface
 
         EosVersion:
             4.13.7M
@@ -1076,15 +1076,15 @@
         Args:
             vlan (str, int): The vlan id to map to the vni
 
         Returns:
             True if the command completes successfully
 
         """
-        return self.configure_interface(name, 'no vxlan vlan %s vni' % vid)
+        return self.configure_interface(name, 'vxlan vlan remove %s vni' % vid)
 
 
 INTERFACE_CLASS_MAP = {
     'Et': EthernetInterface,
     'Po': PortchannelInterface,
     'Vx': VxlanInterface
 }
```

### Comparing `pyeapi-0.8.3/pyeapi/api/ipinterfaces.py` & `pyeapi-0.8.4/pyeapi/api/ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/vlans.py` & `pyeapi-0.8.4/pyeapi/api/vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/varp.py` & `pyeapi-0.8.4/pyeapi/api/varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/system.py` & `pyeapi-0.8.4/pyeapi/api/system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/acl.py` & `pyeapi-0.8.4/pyeapi/api/acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/vrfs.py` & `pyeapi-0.8.4/pyeapi/api/vrfs.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/users.py` & `pyeapi-0.8.4/pyeapi/api/users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/abstract.py` & `pyeapi-0.8.4/pyeapi/api/abstract.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/ntp.py` & `pyeapi-0.8.4/pyeapi/api/ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/vrrp.py` & `pyeapi-0.8.4/pyeapi/api/vrrp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/ospf.py` & `pyeapi-0.8.4/pyeapi/api/ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/bgp.py` & `pyeapi-0.8.4/pyeapi/api/bgp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/routemaps.py` & `pyeapi-0.8.4/pyeapi/api/routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/__init__.py` & `pyeapi-0.8.4/pyeapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/spanningtree.py` & `pyeapi-0.8.4/pyeapi/api/spanningtree.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/staticroute.py` & `pyeapi-0.8.4/pyeapi/api/staticroute.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/mlag.py` & `pyeapi-0.8.4/pyeapi/api/mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/switchports.py` & `pyeapi-0.8.4/pyeapi/api/switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/api/stp.py` & `pyeapi-0.8.4/pyeapi/api/stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi/client.py` & `pyeapi-0.8.4/pyeapi/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Node object can autoload API modules for a structured object oriented
 approach to configuring the EOS node with native Python objects.
 
 Example:
 
     >>> import pyeapi
     >>> conn = pyeapi.connect(host='10.1.1.1', transport='http')
-    >>> conn.execute(['show verson'])
+    >>> conn.execute(['show version'])
     {u'jsonrpc': u'2.0', u'result': [{u'memTotal': 2028008, u'version':
     u'4.14.5F', u'internalVersion': u'4.14.5F-2209869.4145F', u'serialNumber':
     u'', u'systemMacAddress': u'00:0c:29:f5:d2:7d', u'bootupTimestamp':
     1421765066.11, u'memFree': 213212, u'modelName': u'vEOS', u'architecture':
     u'i386', u'internalBuildId': u'f590eed4-1e66-43c6-8943-cee0390fbafe',
     u'hardwareRevision': u''}], u'id': u'4312565648'}
 
@@ -86,14 +86,15 @@
 device.  Each EOS device to be managed should have a Node instance
 
 Config -- A subclass of ConfigParser.SafeConfigParser that handles the
 configuration file.  The configuration file is an INI style file that
 contains the settings for nodes used by the connect_to function.
 
 """
+from uuid import uuid4
 import os
 import re
 
 try:
     # Try Python 3.x import first
     # Note: SafeConfigParser is deprecated and replaced by ConfigParser
     from configparser import ConfigParser as SafeConfigParser
@@ -467,14 +468,15 @@
     def __init__(self, connection, **kwargs):
         self._connection = connection
         self._running_config = None
         self._startup_config = None
         self._version = None
         self._version_number = None
         self._model = None
+        self._session_name = None
 
         self._enablepwd = kwargs.get('enablepwd')
         self.autorefresh = kwargs.get('autorefresh', True)
         self.settings = kwargs
 
     def __str__(self):
         return 'Node(connection=%s)' % str(self._connection)
@@ -574,14 +576,22 @@
                 the request
 
         Returns:
             The config method will return a list of dictionaries with the
                 output from each command.  The function will strip the
                 response from any commands it prepends.
         """
+        if self._session_name:  # If in a config session
+            return self._configure_session(commands, **kwargs)
+
+        return self._configure_terminal(commands, **kwargs)
+
+    def _configure_terminal(self, commands, **kwargs):
+        """Configures the node with the specified commands with leading "configure terminal"
+        """
         commands = make_iterable(commands)
         commands = list(commands)
 
         # push the configure command onto the command stack
         commands.insert(0, 'configure terminal')
         response = self.run_commands(commands, **kwargs)
 
@@ -589,14 +599,32 @@
             self.refresh()
 
         # pop the configure command output off the stack
         response.pop(0)
 
         return response
 
+    def _configure_session(self, commands, **kwargs):
+        """Configures the node with the specified commands with leading "configure session <session name>"
+        """
+        if not self._session_name:
+            raise CommandError('Not currently in a session')
+
+        commands = make_iterable(commands)
+        commands = list(commands)
+
+        # push the configure command onto the command stack
+        commands.insert(0, 'configure session %s' % self._session_name)
+        response = self.run_commands(commands, **kwargs)
+
+        # pop the configure command output off the stack
+        response.pop(0)
+
+        return response
+
     def section(self, regex, config='running_config'):
         """Returns a section of the config
 
         Args:
             regex (str): A valid regular expression used to select sections
                 of configuration to return
             config (str): The configuration to return.  Valid values for config
@@ -820,14 +848,49 @@
         clear the current internal instance variables.  One the next call the
         instance variables will be repopulated with the current config
 
         """
         self._running_config = None
         self._startup_config = None
 
+    def configure_session(self):
+        """Enter a config session
+        """
+        self._session_name = self._session_name or uuid4()
+
+    def diff(self):
+        """Returns session-config diffs in text encoding
+
+        Note: "show session-config diffs" doesn't support json encoding
+        """
+        response = self._configure_session(['show session-config diffs'], encoding='text')
+
+        return response[0]['output']
+
+    def commit(self):
+        """Commits the current config session
+        """
+        return self._configure_and_exit_session(['commit'])
+
+    def abort(self):
+        """Aborts the current config session
+        """
+        return self._configure_session(['abort'])
+
+    def _configure_and_exit_session(self, commands, **kwargs):
+        response = self._configure_session(commands, **kwargs)
+
+        if self.autorefresh:
+            self.refresh()
+
+        # Exit the current config session
+        self._session_name = None
+
+        return response
+
 
 def connect_to(name):
     """Creates a node instance based on an entry from the config
 
     This function will retrieve the settings for the specified connection
     from the config and return a Node instance.  The configuration must
     be loaded prior to calling this function.
```

### Comparing `pyeapi-0.8.3/pyeapi/__init__.py` & `pyeapi-0.8.4/pyeapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 __author__ = 'Arista EOS+'
 
 
 from .client import load_config, connect, connect_to, config_for
 
 __all__ = ['load_config', 'connect', 'connect_to', 'config_for']
```

### Comparing `pyeapi-0.8.3/pyeapi/utils.py` & `pyeapi-0.8.4/pyeapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,20 @@
     if sys.version_info <= (3, 0):
         # Convert unicode values to strings for Python 2
         if isinstance(value, unicode):
             value = str(value)
     if isinstance(value, str) or isinstance(value, dict):
         value = [value]
 
-    if not isinstance(value, collections.Iterable):
-        raise TypeError('value must be an iterable object')
+    if sys.version_info <= (3, 3):
+        if not isinstance(value, collections.Iterable):
+            raise TypeError('value must be an iterable object')
+    else:
+        if not isinstance(value, collections.abc.Iterable):
+            raise TypeError('value must be an iterable object')
 
     return value
 
 
 def lookahead(it):
     it1, it2 = tee(iter(it))
     next(it2)
```

### Comparing `pyeapi-0.8.3/pyeapi/eapilib.py` & `pyeapi-0.8.4/pyeapi/eapilib.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,20 +344,24 @@
         Returns:
             A JSON encoding request structure that can be send over eAPI
 
         """
         commands = make_iterable(commands)
         reqid = id(self) if reqid is None else reqid
         params = {'version': 1, 'cmds': commands, 'format': encoding}
+        streaming = False
         if 'autoComplete' in kwargs:
             params['autoComplete'] = kwargs['autoComplete']
         if 'expandAliases' in kwargs:
             params['expandAliases'] = kwargs['expandAliases']
+        if 'streaming' in kwargs:
+            streaming = kwargs['streaming']
         return json.dumps({'jsonrpc': '2.0', 'method': 'runCmds',
-                           'params': params, 'id': str(reqid)})
+                           'params': params, 'id': str(reqid),
+                           'streaming': streaming})
 
     def send(self, data):
         """Sends the eAPI request to the destination node
 
         This method is responsible for sending an eAPI request to the
         destination node and returning a response based on the eAPI response
         object.  eAPI responds to request messages with either a success
```

### Comparing `pyeapi-0.8.3/test/system/test_api_ntp.py` & `pyeapi-0.8.4/test/system/test_api_ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_system.py` & `pyeapi-0.8.4/test/system/test_api_system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_mlag.py` & `pyeapi-0.8.4/test/system/test_api_mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_varp.py` & `pyeapi-0.8.4/test/system/test_api_varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_ospf.py` & `pyeapi-0.8.4/test/system/test_api_ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_client.py` & `pyeapi-0.8.4/test/system/test_client.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_vrfs.py` & `pyeapi-0.8.4/test/system/test_api_vrfs.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_acl.py` & `pyeapi-0.8.4/test/system/test_api_acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_vlans.py` & `pyeapi-0.8.4/test/system/test_api_vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_ipinterfaces.py` & `pyeapi-0.8.4/test/system/test_api_ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_staticroute.py` & `pyeapi-0.8.4/test/system/test_api_staticroute.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_switchports.py` & `pyeapi-0.8.4/test/system/test_api_switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_users.py` & `pyeapi-0.8.4/test/system/test_api_users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_interfaces.py` & `pyeapi-0.8.4/test/system/test_api_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,20 +631,20 @@
 
     def test_update_vlan(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.update_vlan('Vxlan1', '10', '10')
             self.assertTrue(instance)
-            self.contains('vxlan vlan 10 vni 10', dut)
+            self.contains('vxlan vlan add 10 vni 10', dut)
 
     def test_remove_vlan(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.remove_vlan('Vxlan1', '10')
             self.assertTrue(instance)
-            self.notcontains('vxlan vlan 10 vni 10', dut)
+            self.notcontains('vxlan vlan remove 10 vni 10', dut)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyeapi-0.8.3/test/system/test_api_stp.py` & `pyeapi-0.8.4/test/system/test_api_stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_routemaps.py` & `pyeapi-0.8.4/test/system/test_api_routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/system/test_api_vrrp.py` & `pyeapi-0.8.4/test/system/test_api_vrrp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_utils.py` & `pyeapi-0.8.4/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_ntp.py` & `pyeapi-0.8.4/test/unit/test_api_ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_system.py` & `pyeapi-0.8.4/test/unit/test_api_system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_mlag.py` & `pyeapi-0.8.4/test/unit/test_api_mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_varp.py` & `pyeapi-0.8.4/test/unit/test_api_varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_bgp.py` & `pyeapi-0.8.4/test/unit/test_api_bgp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_ospf.py` & `pyeapi-0.8.4/test/unit/test_api_ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_client.py` & `pyeapi-0.8.4/test/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_vrfs.py` & `pyeapi-0.8.4/test/unit/test_api_vrfs.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_acl.py` & `pyeapi-0.8.4/test/unit/test_api_acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_eapilib.py` & `pyeapi-0.8.4/test/unit/test_eapilib.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_vlans.py` & `pyeapi-0.8.4/test/unit/test_api_vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_ipinterfaces.py` & `pyeapi-0.8.4/test/unit/test_api_ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_staticroute.py` & `pyeapi-0.8.4/test/unit/test_api_staticroute.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_switchports.py` & `pyeapi-0.8.4/test/unit/test_api_switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_users.py` & `pyeapi-0.8.4/test/unit/test_api_users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_interfaces.py` & `pyeapi-0.8.4/test/unit/test_api_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,20 +497,20 @@
 
     def test_set_udp_port_with_default(self):
         cmds = ['interface Vxlan1', 'default vxlan udp-port']
         func = function('set_udp_port', 'Vxlan1', default=True)
         self.eapi_positive_config_test(func, cmds)
 
     def test_update_vlan(self):
-        cmds = ['interface Vxlan1', 'vxlan vlan 10 vni 10']
+        cmds = ['interface Vxlan1', 'vxlan vlan add 10 vni 10']
         func = function('update_vlan', 'Vxlan1', 10, 10)
         self.eapi_positive_config_test(func, cmds)
 
     def test_remove_vlan(self):
-        cmds = ['interface Vxlan1', 'no vxlan vlan 10 vni']
+        cmds = ['interface Vxlan1', 'vxlan vlan remove 10 vni']
         func = function('remove_vlan', 'Vxlan1', 10)
         self.eapi_positive_config_test(func, cmds)
 
     def test_add_vtep(self):
         cmds = ['interface Vxlan1', 'vxlan flood vtep add 1.1.1.1']
         func = function('add_vtep', 'Vxlan1', '1.1.1.1')
         self.eapi_positive_config_test(func, cmds)
```

### Comparing `pyeapi-0.8.3/test/unit/test_api_stp.py` & `pyeapi-0.8.4/test/unit/test_api_stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_routemaps.py` & `pyeapi-0.8.4/test/unit/test_api_routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/unit/test_api_vrrp.py` & `pyeapi-0.8.4/test/unit/test_api_vrrp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/vxlan.json` & `pyeapi-0.8.4/test/fixtures/vxlan.json`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/ipinterfaces.json` & `pyeapi-0.8.4/test/fixtures/ipinterfaces.json`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.text` & `pyeapi-0.8.4/test/fixtures/running_config.text`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.portchannel` & `pyeapi-0.8.4/test/fixtures/running_config.portchannel`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.vxlan` & `pyeapi-0.8.4/test/fixtures/running_config.vxlan`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.ospf` & `pyeapi-0.8.4/test/fixtures/running_config.ospf`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.routemaps` & `pyeapi-0.8.4/test/fixtures/running_config.routemaps`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/show_interfaces.text` & `pyeapi-0.8.4/test/fixtures/show_interfaces.text`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/show_interfaces.json` & `pyeapi-0.8.4/test/fixtures/show_interfaces.json`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.vrrp` & `pyeapi-0.8.4/test/fixtures/running_config.vrrp`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/fixtures/running_config.vrf` & `pyeapi-0.8.4/test/fixtures/running_config.vrf`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/lib/systestlib.py` & `pyeapi-0.8.4/test/lib/systestlib.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/test/lib/testlib.py` & `pyeapi-0.8.4/test/lib/testlib.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/setup.py` & `pyeapi-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyeapi-0.8.3/pyeapi.egg-info/SOURCES.txt` & `pyeapi-0.8.4/pyeapi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 VERSION
 dev-requirements.txt
 requirements.txt
 setup.py
 docs/Makefile
 docs/conf.py
 docs/configfile.rst
+docs/configsessions.rst
 docs/contribute.rst
 docs/description.rst
 docs/examples.rst
 docs/generate_modules.py
 docs/index.rst
 docs/install.rst
 docs/license.rst
@@ -36,18 +37,43 @@
 docs/release-notes-0.6.0.rst
 docs/release-notes-0.6.1.rst
 docs/release-notes-0.7.0.rst
 docs/release-notes-0.8.0.rst
 docs/release-notes-0.8.1.rst
 docs/release-notes-0.8.2.rst
 docs/release-notes-0.8.3.rst
+docs/release-notes-0.8.4.rst
 docs/release-notes.rst
 docs/requirements.rst
 docs/subinterfaces.rst
 docs/support.rst
+docs/api_modules/_list_of_modules.rst
+docs/api_modules/abstract.rst
+docs/api_modules/acl.rst
+docs/api_modules/bgp.rst
+docs/api_modules/interfaces.rst
+docs/api_modules/ipinterfaces.rst
+docs/api_modules/mlag.rst
+docs/api_modules/ntp.rst
+docs/api_modules/ospf.rst
+docs/api_modules/routemaps.rst
+docs/api_modules/spanningtree.rst
+docs/api_modules/staticroute.rst
+docs/api_modules/stp.rst
+docs/api_modules/switchports.rst
+docs/api_modules/system.rst
+docs/api_modules/users.rst
+docs/api_modules/varp.rst
+docs/api_modules/vlans.rst
+docs/api_modules/vrfs.rst
+docs/api_modules/vrrp.rst
+docs/client_modules/_list_of_modules.rst
+docs/client_modules/client.rst
+docs/client_modules/eapilib.rst
+docs/client_modules/utils.rst
 examples/get_config.py
 examples/nodes.conf
 examples/simple.py
 examples/sysmac.py
 examples/vlans_api.py
 pyeapi/__init__.py
 pyeapi/client.py
```

### Comparing `pyeapi-0.8.3/pyeapi.egg-info/PKG-INFO` & `pyeapi-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: pyeapi
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Client for eAPI
 Home-page: https://github.com/arista-eosplus/pyeapi
 Author: Arista EOS+ CS
 Author-email: eosplus-dev@arista.com
 License: BSD-3
+Description-Content-Type: UNKNOWN
 Description: The Python Client for eAPI
         ==========================
         
         The Python Client for eAPI (pyeapi) is a native Python library wrapper around
         Arista EOS eAPI.  It provides a set of Python language bindings for configuring
         Arista EOS nodes.
```

