# Comparing `tmp/sts_libs-0.0.3.dev3.tar.gz` & `tmp/sts_libs-0.0.4.tar.gz`

## Comparing `sts_libs-0.0.3.dev3.tar` & `sts_libs-0.0.4.tar`

### file list

```diff
@@ -1,232 +1,50 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/requirements-stable.txt
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/__about__.data.json
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/__about__.meta.json
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/__init__.data.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/__init__.meta.json
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/noxfile.data.json
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/noxfile.meta.json
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/__init__.data.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/__init__.meta.json
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/__init__.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/__init__.meta.json
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/dm.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/dm.meta.json
--rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/dmpd.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/dmpd.meta.json
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/fc.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/fc.meta.json
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/fio.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/fio.meta.json
--rw-r--r--   0        0        0    34691 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/iscsi.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/iscsi.meta.json
--rw-r--r--   0        0        0    30934 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/linux.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/linux.meta.json
--rw-r--r--   0        0        0    32725 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lio.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lio.meta.json
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/loopdev.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/loopdev.meta.json
--rw-r--r--   0        0        0    51175 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lsm.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lsm.meta.json
--rw-r--r--   0        0        0    36542 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lvm.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/lvm.meta.json
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/md.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/md.meta.json
--rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/mp.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/mp.meta.json
--rw-r--r--   0        0        0    13318 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/net.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/net.meta.json
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/qemu_img.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/qemu_img.meta.json
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/scsi.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/scsi.meta.json
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/scsi_debug.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/scsi_debug.meta.json
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/stratis.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/stratis.meta.json
--rw-r--r--   0        0        0    19904 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/vdo.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/vdo.meta.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/__init__.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/__init__.meta.json
--rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/atomic_run.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/atomic_run.meta.json
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/beaker.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/beaker.meta.json
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/cli_tools.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/cli_tools.meta.json
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/cmdline.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/cmdline.meta.json
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/logchecker.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/logchecker.meta.json
--rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/persistent_vars.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/persistent_vars.meta.json
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/restraint.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/restraint.meta.json
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/size.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/size.meta.json
--rw-r--r--   0        0        0    11096 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/tc.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/tc.meta.json
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/tmt.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/src/sts/utils/tmt.meta.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/__init__.data.json
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/__init__.meta.json
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/cmdline_test.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/cmdline_test.meta.json
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/fio_test.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/fio_test.meta.json
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/iscsi_test.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/iscsi_test.meta.json
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/linux_test.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/linux_test.meta.json
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/logchecker_test.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/logchecker_test.meta.json
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/loopdev_test.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/loopdev_test.meta.json
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/lvm_test.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/lvm_test.meta.json
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/md_test.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/md_test.meta.json
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/net_test.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/net_test.meta.json
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/persistent_vars_test.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/persistent_vars_test.meta.json
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/scsi_test.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.7/sts_libs/tests/scsi_test.meta.json
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/__about__.meta.json
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/__init__.data.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/__init__.meta.json
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/__init__.data.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/__init__.meta.json
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/__init__.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/__init__.meta.json
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/dm.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/dm.meta.json
--rw-r--r--   0        0        0    18160 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/dmpd.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/dmpd.meta.json
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/fc.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/fc.meta.json
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/fio.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/fio.meta.json
--rw-r--r--   0        0        0    34682 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/iscsi.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/iscsi.meta.json
--rw-r--r--   0        0        0    30923 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/linux.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/linux.meta.json
--rw-r--r--   0        0        0    32727 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lio.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lio.meta.json
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/loopdev.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/loopdev.meta.json
--rw-r--r--   0        0        0    51177 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lsm.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lsm.meta.json
--rw-r--r--   0        0        0    36544 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lvm.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/lvm.meta.json
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/md.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/md.meta.json
--rw-r--r--   0        0        0    17230 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/mp.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/mp.meta.json
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/net.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/net.meta.json
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/qemu_img.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/qemu_img.meta.json
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/scsi.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/scsi.meta.json
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/scsi_debug.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/scsi_debug.meta.json
--rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/stratis.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/stratis.meta.json
--rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/vdo.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/vdo.meta.json
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/__init__.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/__init__.meta.json
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/atomic_run.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/atomic_run.meta.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/beaker.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/beaker.meta.json
--rw-r--r--   0        0        0    14260 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/cli_tools.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/cli_tools.meta.json
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/cmdline.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/cmdline.meta.json
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/logchecker.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/logchecker.meta.json
--rw-r--r--   0        0        0    19270 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/persistent_vars.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/persistent_vars.meta.json
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/restraint.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/restraint.meta.json
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/size.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/size.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/tc.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/tc.meta.json
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/tmt.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/src/sts/utils/tmt.meta.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/__init__.data.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/__init__.meta.json
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/cmdline_test.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/cmdline_test.meta.json
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/fio_test.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/fio_test.meta.json
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/iscsi_test.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/iscsi_test.meta.json
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/linux_test.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/linux_test.meta.json
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/logchecker_test.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/logchecker_test.meta.json
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/loopdev_test.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/loopdev_test.meta.json
--rw-r--r--   0        0        0     7992 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/lvm_test.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/lvm_test.meta.json
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/md_test.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/md_test.meta.json
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/net_test.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/net_test.meta.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/persistent_vars_test.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/persistent_vars_test.meta.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/scsi_test.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/.mypy_cache/3.8/sts_libs/tests/scsi_test.meta.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    40145 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    16943 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    48966 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    65812 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35343 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42046 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28673 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22247 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/atomic_run.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/tc.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/LICENSE
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/sts_libs/README.md
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 sts_libs-0.0.3.dev3/PKG-INFO
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20604 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    40316 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17015 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    49132 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    46093 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    64839 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35438 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42191 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28682 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    15159 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22311 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/atomic_run.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/tc.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 sts_libs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.4/sts_libs/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 sts_libs-0.0.4/PKG-INFO
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/dm.py` & `sts_libs-0.0.4/sts_libs/src/sts/dm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re  # regex
 
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 
 def dm_show_status(dm_device=None):
     """Show dmsetup status.
     The arguments are:
     dm_device:           Device name (optional).
 
@@ -19,31 +19,30 @@
     or
     False.
     """
     cmd = "dmsetup status"
     if dm_device:
         cmd += f" {dm_device}"
 
-    retcode, _ = run(cmd, return_output=True, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not show dmsetup status")
         return False
     return True
 
 
 def dm_query_status(dm_device=None):
     """Query dmsetup status and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with status info for each device.
     """
     cmd = "dmsetup status"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not list status")
         return None
     devices = output.split("\n")
 
     status_basic_format_regex = r"(.*):\s+(\d+)\s+(\d+)\s+(\S+)"
     # Thin formats are available on: https://www.kernel.org/doc/Documentation/device-mapper/thin-provisioning.txt
@@ -185,31 +184,30 @@
     or
     False.
     """
     cmd = "dmsetup table"
     if dm_device:
         cmd += f" {dm_device}"
 
-    retcode, _ = run(cmd, return_output=True, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not show dmsetup table")
         return False
     return True
 
 
 def dm_query_table(dm_device=None):
     """Query dmsetup table and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with table info for each device.
     """
     cmd = "dmsetup table"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not list table")
         return None
     devices = output.split("\n")
 
     # Basic format information is found on man dmsetup under "TABLE FORMAT" section
     # format of dmsetup table: logical_start_sector num_sectors target_type target_args
@@ -382,15 +380,15 @@
 def dm_get_table_device(dm_name):
     """Get table information for specific device.
     The table info is not parsed.
     """
     if not dm_name:
         return None
     cmd = f"dmsetup table {dm_name}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: Could not query table for {dm_name}")
         return None
 
     return output
 
 
@@ -418,16 +416,15 @@
     if not m:
         sts_print(f"FAIL: dm_set_target_type() - ({table_info}) does not match dmsetup table output format")
         return False
     # load the table with new target type
     new_table = f'"{m.group(1)} {m.group(2)} {target_type} {m.group(4)}"'
 
     cmd = f"dmsetup load {dm_name} --table {new_table}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: dm_set_target_type() - could not load table on {dm_name}")
         dm_resume_dev(dm_name)
         return False
 
     if not dm_resume_dev(dm_name):
         return False
 
@@ -440,16 +437,15 @@
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup suspend {dm_name}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: could not suspend {dm_name}")
         return False
 
     return True
 
 
 def dm_resume_dev(dm_name):
@@ -458,16 +454,15 @@
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup resume {dm_name}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: could not resume {dm_name}")
         return False
 
     return True
 
 
 def dm_message_dev(dm_name, message):
@@ -476,16 +471,15 @@
     Device name: e.g. mpatha
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
     cmd = f"dmsetup message {dm_name} {message}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: could not send message to {dm_name}")
         return False
 
     return True
 
 
 def dm_remove(dm_name):
@@ -499,12 +493,11 @@
     """
     devs = dm_query_table()
     if dm_name not in list(devs.keys()):
         # device name does not exist
         return True
 
     cmd = f"dmsetup remove {dm_name}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: could not remove {dm_name}")
         return False
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.4/sts_libs/src/sts/dmpd.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 import sys
 from pathlib import Path
 
 from sts import linux, lvm
 from sts.utils import sts_print
 from sts.utils.cli_tools import Wrapper
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 
 def _get_devices():
     return lvm.lv_query()
 
 
 def _get_active_devices():
     cmd = "ls /dev/mapper/"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not find active dm devices")
         return False
     return output.split()
 
 
 def _get_device_path(vg_name, lv_name):
@@ -56,15 +56,15 @@
     sts_print(f"INFO: device {lv_name} is active")
     return True
 
 
 def _fallocate(_file, size, command_message):
     cmd = f"fallocate -l {size}M {_file}"
     try:
-        retcode = run(cmd)
+        retcode = run(cmd).returncode
         if retcode != 0:
             sts_print(f"FAIL: Command failed with code {retcode}.")
             sts_print(f"FAIL: Could not create file to {command_message} metadata to.")
             return False
     except OSError as e:
         print("command failed: ", e, file=sys.stderr)
         return False
@@ -94,15 +94,15 @@
         "thin_trim",
     ]
     if cmd not in commands:
         sts_print(f"FAIL: Unknown command {cmd}")
         return False
 
     command = f"{cmd} -h"
-    retcode = run(command, verbose=True)
+    retcode = run(command, verbose=True).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not get help for {cmd}.")
         return False
 
     return True
 
 
@@ -129,15 +129,15 @@
         "thin_trim",
     ]
     if cmd not in commands:
         sts_print(f"FAIL: Unknown command {cmd}")
         return False
 
     command = f"{cmd} -V"
-    retcode = run(command, verbose=True)
+    retcode = run(command, verbose=True).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not get version of {cmd}.")
         return False
 
     return True
 
 
@@ -171,15 +171,15 @@
 
     return False
 
 
 def _metadata_size(source=None, lv_name=None, vg_name=None):
     if source is None:
         cmd = "lvs -a --units m"
-        ret, data = run(cmd, return_output=True)
+        ret, data = run_ret_out(cmd, return_output=True)
         if ret != 0:
             sts_print("FAIL: Could not list LVs")
         data_line = data.splitlines()
         for line in data_line:
             cut = line.split()
             if not cut or lv_name != cut[0] and vg_name != cut[1]:
                 continue
@@ -261,15 +261,15 @@
     if skip_hints:
         options += "--skip-hints "
 
     if skip_discards:
         options += "--skip-discards "
 
     cmd = f"cache_check {device} {options}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not check {device} metadata")
         return False
 
     return True
 
 
@@ -332,17 +332,17 @@
         options += f"-o {output} "
 
     if repair:
         options += "--repair"
 
     cmd = f"cache_dump {device} {options}"
     if return_output:
-        retcode, data = run(cmd, return_output=True, verbose=verbose)
+        retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
     else:
-        retcode = run(cmd, verbose=verbose)
+        retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not dump {device} metadata.")
         return ret_fail
 
     if return_output:
         return True, data
     return True
@@ -401,15 +401,15 @@
             size = _metadata_size(source_file, source_lv, source_vg)
             ret = _fallocate(target_file, size + 1, "repair")
             if not ret:
                 return False
         target = target_file
 
     cmd = f"cache_repair -i {source} -o {target}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not repair metadata from {source} to {target}")
         return False
 
     return True
 
 
@@ -477,15 +477,15 @@
         options += "--omit-clean-shutdown "
 
     if override_metadata_version:
         options += f"--debug-override-metadata-version {override_metadata_version}"
 
     cmd = f"cache_restore -i {source_file} -o {target} {options}"
 
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not restore metadata from {source_file} to {target}")
         return False
 
     return True
 
 
@@ -552,15 +552,15 @@
     if skip_mappings:
         options += "--skip-mappings "
 
     if ignore_non_fatal_errors:
         options += "--ignore-non-fatal-errors "
 
     cmd = f"thin_check {device} {options}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not check {device} metadata")
         return False
 
     return True
 
 
@@ -621,15 +621,15 @@
                 return False
         options += f" --format \"{','.join([str(i) for i in fields])}\" "
 
     if snapshot:
         options += "--metadata-snap"
 
     cmd = f"thin_ls {device} {options}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not list {device} metadata")
         return False
 
     return True
 
 
@@ -734,17 +734,17 @@
             return ret_fail
 
     if skip_mappings:
         options += "--skip-mappings "
 
     cmd = f"thin_dump {device} {options}"
     if return_output:
-        retcode, data = run(cmd, return_output=True, verbose=verbose)
+        retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
     else:
-        retcode = run(cmd, verbose=verbose)
+        retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not dump {device} metadata.")
         return ret_fail
 
     if return_output:
         return True, data
     return True
@@ -802,15 +802,15 @@
         target = target_file
 
     if quiet:
         options += "--quiet"
 
     cmd = f"thin_restore -i {source_file} -o {target} {options}"
 
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not restore metadata from {source_file} to {target}")
         return False
 
     return True
 
 
@@ -867,15 +867,15 @@
             size = _metadata_size(source_file, source_lv, source_vg)
             ret = _fallocate(target_file, size + 1, "repair")
             if not ret:
                 return False
         target = target_file
 
     cmd = f"thin_repair -i {source} -o {target}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not repair metadata from {source} to {target}")
         return False
 
     return True
 
 
@@ -923,15 +923,15 @@
     # region 1..-1 must be valid, using unsigned 32bit ints
     if int(regions[0]) & 0xFFFFFFFF >= int(regions[2]) & 0xFFFFFFFF:
         print("FAIL: Beginning of the region must be before its end.")
         return False
     options = f"--region {region}"
 
     cmd = f"thin_rmap {device} {options}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not output reverse map from {device} metadata device")
         return False
 
     return True
 
 
@@ -985,15 +985,15 @@
         if not Path(metadata_file).is_file():
             sts_print(f"FAIL: metadata_file {metadata_file} is not a file.")
             return False
         metadata_dev = metadata_file
 
     data_dev = _get_device_path(data_vg, data_lv)
     cmd = f"thin_trim --data-dev {data_dev} --metadata-dev {metadata_dev} {options}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not discard free pool space on device {data_dev} with metadata device {metadata_dev}.")
         return False
 
     return True
 
 
@@ -1050,15 +1050,15 @@
             return False
 
     if verbosity:
         options += "--verbose"
 
     if _get_dev_id(thin1, source_file, source_lv, source_vg) and _get_dev_id(thin2, source_file, source_lv, source_vg):
         cmd = f"thin_delta {options} --thin1 {thin1} --thin2 {thin2} {device}"
-        retcode = run(cmd, verbose=verbose)
+        retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
             sts_print("FAIL: Could not get differences in mappings between two thin LVs.")
             return False
     else:
         sts_print("FAIL: Specified id does not exist.")
         return False
     return True
@@ -1167,19 +1167,19 @@
     @staticmethod
     def _remove_nones(kwargs):
         return {k: v for k, v in kwargs.items() if v is not None}
 
     def _get_possible_arguments(self, command=None):
         return super()._get_possible_arguments(command.split()[0])
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):
+    def _run(self, cmd, verbosity=True, **kwargs):
         # Constructs the command to run and runs it
         cmd = self._add_arguments(cmd, **kwargs)
 
-        ret = run(cmd, verbose=verbosity, return_output=return_output)
+        ret = run(cmd, verbose=verbosity).returncode
         if isinstance(ret, tuple) and ret[0] != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     def cache_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/fc.py` & `sts_libs-0.0.4/sts_libs/src/sts/fc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import os.path
 import re  # regex
 from pathlib import Path
 
 from sts import linux, scsi
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run_ret_out
 
 host_path = "/sys/class/fc_host/"
 
 remote_port_path = "/sys/class/fc_remote_ports/"
 
 regex_target_id = re.compile(r"target(\d+):(\d+):(\d+)")
 regex_target = re.compile(r"(\d+):(\d+):(\d+)")
@@ -117,27 +117,27 @@
 
     return False
 
 
 # Return an array with all fc_hosts numbers
 def get_fc_hosts():
     cmd = "ls " + host_path
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     # remove 'host' prefix
     output = re.sub("host", "", output)
     return output.split()
 
 
 def get_fc_host_wwpn(host):
     """Return the WWPN of specific sts."""
     host_port_path = f"/sys/class/fc_host/host{host}/port_name"
     cmd = "cat " + host_port_path
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
 def fc_host_id_of_wwpn(wwpn):
     """Given a WWPN, return its host id."""
@@ -186,23 +186,23 @@
     if not rports:
         return None
     return rports
 
 
 def get_fc_host_remote_ports(host):
     cmd = f"ls {remote_port_path} | grep rport-{host}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output.split()
 
 
 def wwpn_of_rport(r_port):
     cmd = f"cat {remote_port_path}/{r_port}/port_name"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
 def rport_of_h_wwpn_t_wwpn(h_wwpn, t_wwpn):
     """Return the remote port of given wwpn
@@ -363,28 +363,28 @@
                 return False
             return disk_name
     return None
 
 
 def get_fc_host_rport_targets(host, r_port):
     cmd = f"ls /sys/bus/scsi/devices/host{host}/{r_port} | grep target"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     output = re.sub("target", "", output)
     return output.split()
 
 
 def get_fc_host_rport_target_devices(host, r_port, target):
     if not host or not r_port or not target:
         sts_print("FAIL: get_fc_host_rport_target_devices. Usage: host, r_port, target")
         return None
 
     cmd = f'ls /sys/bus/scsi/devices/host{host}/{r_port}/target{target} | grep "{target}"'
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     output = re.sub("target", "", output)
     return output.split()
 
 
 def rport_id_2_target_id():
@@ -520,15 +520,15 @@
         return None
 
     sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
     if not Path(sys_r_port_param).is_file():
         sts_print(f"FAIL: get_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return None
 
-    ret, value = run(f"cat {sys_r_port_param}", return_output=True, verbose=False)
+    ret, value = run_ret_out(f"cat {sys_r_port_param}", return_output=True, verbose=False)
     if ret != 0:
         sts_print(f"FAIL: get_value_rport_parameter() - Could not read {sys_r_port_param}")
         # print command output
         print(value)
         return None
 
     return value
@@ -554,14 +554,14 @@
         return False
 
     sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
     if not Path(sys_r_port_param).is_file():
         sts_print(f"FAIL: set_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return False
 
-    ret, output = run(f"echo {value} > {sys_r_port_param}", return_output=True, verbose=False)
+    ret, output = run_ret_out(f"echo {value} > {sys_r_port_param}", return_output=True, verbose=False)
     if ret != 0:
         sts_print(f"FAIL: set_value_rport_parameter() - Could not set {sys_r_port_param} to {value}")
         # print command output
         print(output)
         return False
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/fio.py` & `sts_libs-0.0.4/sts_libs/src/sts/fio.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 import subprocess
 import sys
 
 from sts import linux
 from sts.utils import sts_print
-from sts.utils.cmdline import exists, run
+from sts.utils.cmdline import exists, run, run_ret_out
 
 fio_default_options = {
     "rw": "randrw",  # Type of I/O pattern. Supported(read, write, trim, randread, randwrite, rw, randrw, trimwrite)
     "name": "fio_test",  # signalling the start of a new job.
     "filename": None,  # device or filename
     "direct": 1,  # If true, use non-buffered I/O (usually O_DIRECT)
     "iodepth": 1,  # Number  of  I/O  units  to keep in flight against the file. Note that increasing
@@ -28,22 +28,23 @@
 }  # (supports: md5 crc16 crc32 crc32c crc32c-intel crc64 crc7 sha256 sha512 sha1 xxhash)
 
 fio_default_verify_options = {
     "verify_backlog": 1024,  # fio will write only N blocks before verifying these blocks.
     # Set to None to verify after all IO is written
     "verify_fatal": 1,  # If true, exit the job on the first observed verification failure
     "do_verify": 1,
+    "verify": "crc32c",
 }
 
 
 def install_fio():
     pkg = "fio"
     if linux.install_package(pkg):
         return True
-    if run("fio >/dev/null 2>&1") == 1:
+    if run("fio >/dev/null 2>&1").returncode == 1:
         return True
     # Try to install FIO from source
     return install_fio_from_src()
 
 
 def install_fio_from_src():
     git_url = "git://git.kernel.org/pub/scm/linux/kernel/git/axboe/fio.git"
@@ -52,29 +53,30 @@
         sts_print("FAIL: Could not install libaio-devel")
         return False
 
     if not linux.install_package("zlib-devel"):
         sts_print("FAIL: Could not install zlib-devel")
         return False
 
-    if run(f"git clone {git_url}") != 0:
+    if run(f"git clone {git_url}").returncode != 0:
         sts_print("FAIL: Could not clone fio repo")
         return False
 
     sts_print("INFO: Installing FIO")
-    if run("cd fio && ./configure && make && make install") != 0:
+    if run("cd fio && ./configure && make && make install").returncode != 0:
         sts_print("FAIL: Could not build fio")
         return False
 
     if not exists("fio"):
         sts_print("FAIL: FIO did not install properly")
         return False
     return True
 
 
+# TODO: rewrite to cmdline.run()
 def fio_stress(of, verbose=False, return_output=False, **fio_opts):
     # For compatibility with tests using other named parameters
     convert_param = {
         "io_type": "rw",
         "time": "runtime",
         "thread": "numjobs",
         "log_file": "output",
@@ -115,15 +117,15 @@
     stdout, _ = p.communicate()
     stdout = stdout.decode("ascii", "ignore")
     stdout = stdout.rstrip("\n")
     if not verbose:  # If verbose option is selected, the run() will print the fio command.
         sts_print(f"INFO: [{stdout}] FIO Running: '{cmd}'...")
 
     # sts_print("INFO: Running %s" % cmd)
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print("FAIL: running FIO")
         print(output)
         if return_output:
             return False, None
         return False
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.4/sts_libs/src/sts/iscsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """iscsi.py: Module with methods for iSCSI initiator."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
+import subprocess
 from ast import literal_eval
 from os import getenv
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Tuple, Union
+from typing import Dict, List, Literal, Optional, Union
 
 from sts import linux, mp, net, scsi
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 PACKAGE_NAME = "iscsi-initiator-utils"
 CLI_NAME = "iscsiadm"
 ISCSID_SERVICE_NAME = "iscsid"
 ISCSIUIO_SERVICE_NAME = "iscsiuio"
 
 
@@ -113,38 +114,36 @@
 
     def available_options(self, mode: str) -> List[str]:
         return self.get_short_options_list(mode) + self.get_long_options_list(mode)
 
     def _run(
         self,
         mode: str = "",
-        return_output: bool = True,
+        capture_output: bool = False,
         arguments: Optional[Union[Dict[str, str], Dict[str, Optional[str]]]] = None,
         timeout: Union[int, None] = None,
-    ) -> Union[int, Tuple[int, str]]:
+    ) -> subprocess.CompletedProcess:
         if mode is not None:
             self.validate_mode(mode)
         if arguments is not None and self.disable_check is not True:
             self.validate_arguments(mode, arguments)
 
         command_list: list = [CLI_NAME, "--mode", mode]
         if arguments is not None:
             command_list = command_list + [f"{k}" if v is None else f"{k} {v}" for k, v in arguments.items()]
         if self.debug_level:
             command_list = [*command_list, "--debug", str(self.debug_level)]
         command: str = " ".join(command_list)
 
-        if self.verbose:
-            return run(command, verbose=True, return_output=return_output, timeout=timeout)
-        return run(command, verbose=False, return_output=return_output, timeout=timeout)
+        return run(command, capture_output=capture_output, timeout=timeout, verbose=self.verbose)
 
-    def iface(self, op: str, iface: str, name: Optional[str] = None, value: Optional[str] = None, return_output=True):
+    def iface(self, op: str, iface: str, name: Optional[str] = None, value: Optional[str] = None, capture_output=True):
         return self._run(
             mode="iface",
-            return_output=return_output,
+            capture_output=capture_output,
             arguments={"-o": op, "-n": name, "-v": value, "-I": iface},
         )
 
     def iface_update(self, iface: str, name: str, value: str):
         return self.iface(op="update", iface=iface, name=f"iface.{name}", value=value)
 
     def iface_update_iqn(self, iface: str, iqn: str):
@@ -154,32 +153,31 @@
         return self.iface_update(iface=iface, name="iface.ipaddress", value=ip)
 
     def discovery(
         self,
         portal: str,
         discovery_type: str = "st",
         iface: Optional[str] = None,
-        return_output=True,
         **kwargs,
     ):
         arguments = {"-t": discovery_type, "-p": portal, **kwargs}
         if iface:
             arguments.update({"-I": iface})
-        return self._run(mode="discovery", return_output=return_output, arguments=arguments)
+        return self._run(mode="discovery", arguments=arguments)
 
-    def node(self, return_output=True, **kwargs):
-        return self._run(mode="node", return_output=return_output, arguments={**kwargs})
+    def node(self, **kwargs):
+        return self._run(mode="node", arguments={**kwargs})
 
-    def node_login(self, return_output=True, **kwargs):
+    def node_login(self, **kwargs):
         arguments = {"--login": None, **kwargs}
-        return self.node(return_output=return_output, **arguments)
+        return self.node(**arguments)
 
-    def node_logout(self, return_output=True, **kwargs):
+    def node_logout(self, **kwargs):
         arguments = {"--logout": None, **kwargs}
-        return self.node(return_output=return_output, **arguments)
+        return self.node(**arguments)
 
 
 def get_env_vars() -> dict:
     """Parse general environmental variables needed for iscsi initiator
     Accepts following env vars:
     'ISCSI_INITIATORNAME': str
     'ISCSI_TARGET': str
@@ -220,37 +218,39 @@
     """Configure iSCSI initiator based on env variables."""
     iscsiadm = IscsiAdm(verbose=True)
     if not env_vars:
         env_vars = get_env_vars()
     if "initiatorname" in env_vars:
         if not set_initiatorname(env_vars["initiatorname"]):
             return False
-        linux.service_restart("iscsid", verbose=False)
+        linux.service_restart(ISCSID_SERVICE_NAME, verbose=False)
     if "ifaces" in env_vars:
         for iface in env_vars["ifaces"]:
             ifacename = iface["iscsi_ifacename"]
             if ("qedi" in ifacename or "bnx2i" in ifacename) and not linux.is_service_running(ISCSIUIO_SERVICE_NAME):
                 linux.service_enable(ISCSIUIO_SERVICE_NAME, now=True)
             values_to_set: Optional[dict] = iface["setup"]
             if not values_to_set:
                 continue
             if "hwaddress" in values_to_set:
                 create_iscsi_iface(iface_name=ifacename)
             for n, v in values_to_set.items():
-                ret, out = iscsiadm.iface_update(iface=ifacename, name=n, value=v)
+                completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=v)
+                ret = completed_process.returncode
+                out = completed_process.output
                 if ret != 0:
                     sts_print(f"FAIL: iscsi update command returned {ret}. Output: {out}")
                     return False
             if discover_targets:
                 iface_targets = iface["targets"]
                 for t in iface_targets:
                     if not t["portal"]:
                         sts_print(f"FAIL: No portal specified for iSCSI discovery: {iface}")
                         return False
-                    if iscsiadm.discovery(iface=ifacename, portal=t["portal"], return_output=False) != 0:
+                    if iscsiadm.discovery(iface=ifacename, portal=t["portal"]) != 0:
                         return False
     if not linux.is_service_enabled(ISCSID_SERVICE_NAME):
         linux.service_enable(ISCSID_SERVICE_NAME)
     return True
 
 
 def discovery_login(iface_name, portal, iqn, iface_ip=None, subnet_mask=None, gateway=None):
@@ -337,15 +337,15 @@
 
     return True
 
 
 # Return an array with all iscsi_hosts numbers
 def get_iscsi_hosts():
     cmd = "ls " + host_path
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     # remove 'host' prefix
     output = re.sub("host", "", output)
     return output.split()
 
 
@@ -355,15 +355,15 @@
     The arguments are:
     None
     Returns:
     Dict:    Dict with all discovered targets
     None:    If some problem happened.
     """
     cmd = "iscsiadm -m discovery -P1"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         # If no target is found iscsiadm returns error code
         return None
     lines = output.split("\n")
 
     supported_discovery_modes = ["SENDTARGETS", "iSNS", "STATIC", "FIRMWARE"]
     supported_mode_type = {"SENDTARGETS": "sendtargets", "iSNS": "isns"}
@@ -464,20 +464,20 @@
         if ("bnx2i" in ifaces or "qedi" in ifaces) and linux.is_service_running(ISCSIUIO_SERVICE_NAME) != 0:
             linux.service_enable(ISCSIUIO_SERVICE_NAME, now=True)
         interfaces = ifaces.split(" ")
         for interface in interfaces:
             cmd += f" -I {interface}"
     cmd += " -t st"
     retries = 0
-    retcode, data = run(cmd, return_output=True, verbose=True)
+    retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
     while retcode == 0 and "(err 29)" in data and retries < max_retries:
-        retcode, data = run(cmd, return_output=True, verbose=True)
+        retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
         retries += 1
     if retcode != 0 or retries == max_retries:
-        sts_print("FAIL: Could not discover iSCSI target")
+        sts_print(f"FAIL: Could not discover iSCSI target. Return code: {retcode}")
         return False
     return True
 
 
 def is_target_discovered(t_iqn):
     """Check if an iSCSI target is already discovered
     The arguments are:
@@ -544,16 +544,15 @@
     """
     sts_print(f"INFO: Deleting target portal: {portal}")
     if net.get_ip_version(portal) == 6:
         # IF IPv6 we need to append squared brackets to the address
         portal = "[" + portal + "]"
 
     cmd = f'iscsiadm -m discoverydb --type {tp} --portal "{portal}:{port}" -o delete'
-    retcode, _ = run(cmd, return_output=True, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not delete discover iSCSI target")
         return False
     return True
 
 
 def clean_up(portal="all"):
     """Remove iSCSI session and discover information for specific target
@@ -635,15 +634,15 @@
     return True
 
 
 # iSCSI session ###
 # def query_sessions():
 #    #cmd output: tcp: [21] 127.0.0.1:3260,1 iqn.2009-10.com.redhat:storage-1 (non-flash)
 #    cmd = "iscsiadm -m session"
-#    retcode, output = run(cmd, return_output=True, verbose=False)
+#    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
 #    if (retcode != 0):
 #        return None
 #    lines = output.split("\n")
 #    session_regex = re.compile("(\S+):\s[(\d+)]\s(\S+):(\S+),(\d+),(\S+)")
 #    sessions_dict = {}
 #    for line in lines:
 #        m = session_regex.search(line)
@@ -656,15 +655,15 @@
 #            ses_dict["target_iqn"] = m.group(6)
 #            sessions[sid] = ses_dict
 #    return sessions_dict
 
 
 def get_all_session_ids():
     cmd = "iscsiadm -m session -P1"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         # sts_print ("INFO: there is no iSCSI session")
         return None
     lines = output.split("\n")
 
     session_ids = []
 
@@ -687,15 +686,15 @@
     """
     if not sid:
         sts_print("FAIL: query_iscsi_session() - requires sid as argument")
         return None
 
     regex_session_scsi_id = "^[ \t]+scsi([0-9]+) Channel ([0-9]+) Id ([0-9])+ Lun: ([0-9]+)$"
     cmd = f"iscsiadm -m session -P3 -S -r {sid}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     lines = output.split("\n")
 
     session_info_dict = {}
     # dict with disk name and its status
     session_disks_dict = {}
@@ -748,15 +747,15 @@
                             session_info_dict[key] = net.get_mac_of_nic(nic)
     # added info for the specific session
     session_info_dict["disks"] = session_disks_dict
     session_info_dict["host"] = session_host_dict
     return session_info_dict
 
 
-def query_all_iscsi_sessions():
+def query_all_iscsi_sessions() -> Union[dict, None]:
     """First we get all iSCSI ids, later on we get the information of each session individually."""
     session_ids = get_all_session_ids()
     if not session_ids:
         return None
 
     iscsi_sessions = {}
     # Collecting info from each session
@@ -768,15 +767,15 @@
     return iscsi_sessions
 
 
 def session_logout(sid=None):
     cmd = "iscsiadm -m session -u"
     if sid:
         cmd += f" -r {sid}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(output)
         sts_print("FAIL: session_logout() - Could not logout from session")
         return None
     return True
 
 
@@ -1036,15 +1035,15 @@
     if target:
         for target_iqn in target.split():
             cmd += f" -T {target_iqn}"
 
     if portal:
         cmd += f" -p {portal}"
 
-    retcode, output = run(cmd, return_output=True, verbose=True)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
         sts_print("FAIL: Could not login to iSCSI target")
         print(output)
         return False
 
     linux.wait_udev(udev_wait_time)
     return True
@@ -1069,15 +1068,15 @@
 
     if target:
         cmd += f" -T {target}"
 
     if portal:
         cmd += f" -p {portal}"
 
-    retcode, output = run(cmd, return_output=True, verbose=True)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
         sts_print("FAIL: Could not logout from iSCSI target")
         print(output)
         return False
     return True
 
 
@@ -1087,16 +1086,15 @@
         sts_print("FAIL: node_delete() - requires portal and/or target parameters")
         return False
 
     cmd = "iscsiadm -m node -o delete"
     if options:
         cmd += f" {options}"
 
-    retcode, _ = run(cmd, return_output=True, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not delete node iSCSI target")
         return False
     return True
 
 
 # iSCSI iface ###
 def iface_query_all_info(iface_name=None):
@@ -1109,15 +1107,15 @@
         return None
 
     all_iface_dict = {}
     iface_info_regex = re.compile(r"iface\.(\S+) = (\S+)")
 
     for iface in ifaces:
         cmd = f"iscsiadm -m iface -I {iface}"
-        retcode, output = run(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print("FAIL: Could not delete node iSCSI target")
             continue
         details = output.split("\n")
         for info in details:
             m = iface_info_regex.match(info)
             if not m:
@@ -1149,32 +1147,36 @@
     False:    If some problem happened.
     """
     if not iface or not name or not value:
         sts_print("FAIL: iface_update() - required parameters: iface, name, value")
         return False
 
     cmd = f"iscsiadm -m iface -I {iface} -o update -n iface.{name} -v {value}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: Could not set {name} to {value} on iface {iface}")
         print(output)
         return False
 
     return True
 
 
 def set_initiatorname(iqn: str) -> bool:
     initiatorname_file = "/etc/iscsi/initiatorname.iscsi"
+    str_to_write = f"InitiatorName={iqn}"
     try:
-        with Path(initiatorname_file).open(mode="r+") as i:
-            existing_name = i.read()
-            if iqn != existing_name:
+        path = Path(initiatorname_file)
+        if not path.is_file():
+            linux.service_start(ISCSID_SERVICE_NAME)
+        existing_name = path.read_text()
+        if str_to_write != existing_name:
+            with path.open(mode="w") as i:
                 sts_print(f"INFO: Writing {iqn} to {initiatorname_file}")
-                i.write(f"InitiatorName={iqn}")
-                linux.service_restart("iscsid", verbose=True)
+                i.write(str_to_write)
+                linux.service_restart(ISCSID_SERVICE_NAME, verbose=True)
     except Exception as e:
         sts_print(f"FAIL: Could not set iqn in {initiatorname_file}. Exception: {e}")
         return False
     return True
 
 
 def iface_set_iqn(iqn, iface="default"):
@@ -1221,15 +1223,15 @@
 
     return True
 
 
 def get_iscsi_iface_names():
     """Return a list with the name of all iSCSI interfaces on the host."""
     cmd = 'iscsiadm -m iface | cut -d " " -f 1'
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not read iSCSI interfaces")
         print(output)
         return None
     ifaces = output.split("\n")
     ifaces[:] = (value for value in ifaces if "iSCSI ERROR" not in value)  # bz1997710
     return ifaces
@@ -1240,15 +1242,15 @@
     Use dictionary with parameter:value as argument.
     """
     filename = "/etc/iscsi/iscsid.conf"
     if not linux.edit_config(filename, parameters, list_values=False):
         sts_print(f"FAIL: Unable to set iscsi parameters: {parameters}")
         return False
 
-    if not linux.service_restart("iscsid"):
+    if not linux.service_restart(ISCSID_SERVICE_NAME):
         sts_print("FAIL: Unable to restart iscsid service")
         return False
 
     return True
 
 
 def set_chap(target_user, target_pass, initiator_user=None, initiator_pass=None):
@@ -1391,25 +1393,24 @@
 
 def remove_iscsi_iface(iface_name):
     if iface_name not in get_iscsi_iface_names():
         sts_print(f"INFO: iSCSI interface '{iface_name}' does not exist")
         return False
 
     cmd = f"iscsiadm -m iface -o delete -I {iface_name}"
-    retcode = run(cmd, verbose=False)
-    if retcode != 0:
+    if run(cmd, verbose=False).returncode != 0:
         sts_print("FAIL: Could not remove iSCSI interface")
         return False
 
     return True
 
 
 def node_iface_info(iface_name):
     cmd = f"iscsiadm -m node -I {iface_name}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not get iface info!")
         print(output)
         return False
 
     return True
 
@@ -1430,16 +1431,22 @@
         if ses["disks"]:
             # disk names are key values
             disks.extend(list(ses["disks"].keys()))
 
     return disks
 
 
-def get_session_id_from_disk(disk_name):
-    for sid in query_all_iscsi_sessions():
+def get_session_id_from_disk(disk_name: str):
+    sids = query_all_iscsi_sessions()
+    fail_msg = f"FAIL: Could not find disk '{disk_name}' in iscsi sessions."
+    if not sids:
+        sts_print(fail_msg)
+        return None
+    for sid in sids:
         session = query_iscsi_session(sid)
         if not session:
             sts_print(f"FAIL: Could not query iscsi session sid: '{sid}'.")
+            continue
         if disk_name in session["disks"]:
             return session["sid"]
-    sts_print(f"FAIL: Could not find disk '{disk_name}' in iscsi sessions.")
+    sts_print(fail_msg)
     return None
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/linux.py` & `sts_libs-0.0.4/sts_libs/src/sts/linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from typing import Any, List, Literal, Optional, Tuple, Union
 
 from configobj import ConfigObj
 from pkg_resources import parse_version
 
 from sts import mp, scsi
 from sts.utils import sts_print
-from sts.utils.cmdline import exists, run
+from sts.utils.cmdline import exists, run, run_ret_out
 
 
 def hostname():
-    ret, host = run("hostname", verbose=False, return_output=True)
+    ret, host = run_ret_out("hostname", verbose=False, return_output=True)
     if ret != 0:
         sts_print("FAIL: hostname() - could not run command")
         print(host)
         return None
     return host
 
 
@@ -46,15 +46,15 @@
             data[k] = v.strip('"')
     return [data["ID"], data["VERSION_ID"]]
 
 
 def dist_release():
     """Find out the release number of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
-    # ret, release = run("lsb_release --release --short", verbose=False, return_output=True)
+    # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
         sts_print("FAIL: Could not determine dist release!")
         return None
     return dist[1]
@@ -92,15 +92,15 @@
     sts_print(f"FAIL: dist_ver_minor() - Release does not seem to have minor version: {release}")
     return None
 
 
 def dist_name():
     """Find out the name of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
-    # ret, release = run("lsb_release --release --short", verbose=False, return_output=True)
+    # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
         sts_print("FAIL: dist_name() - Could not determine dist name")
         return None
 
@@ -122,16 +122,15 @@
     has_systemctl = True
 
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} start"
 
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: Could not start {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
@@ -148,16 +147,15 @@
     has_systemctl = True
 
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} stop"
 
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not stop {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
@@ -180,27 +178,25 @@
     service_timestamp = get_service_timestamp(service_name)
     if service_timestamp is not None:
         timestamp_struct = time.strptime(service_timestamp, "%a %Y-%m-%d %H:%M:%S %Z")
         actual_time = time.localtime()
         if time.mktime(actual_time) - time.mktime(timestamp_struct) < 5:
             print("Waiting 5 seconds before restart.")
             time.sleep(5)
-    retcode = run(cmd, return_output=False, verbose=verbose)
-    if retcode != 0:
+    if run(cmd, capture_output=False, verbose=verbose).returncode != 0:
         sts_print(f"FAIL: Could not restart {service_name}")
         if has_systemctl:
             run(f"systemctl status {service_name}")
             run("journalctl -xn")
         return False
     return True
 
 
 def systemctl_is_enabled(unit: str) -> bool:
-    retcode = run(f"systemctl is-enabled {unit}", return_output=False, verbose=False)
-    if retcode != 0:
+    if run(f"systemctl is-enabled {unit}", verbose=False).returncode != 0:
         return False
     return True
 
 
 def is_service_enabled(service_name: str) -> bool:
     return systemctl_is_enabled(f"{service_name}.service")
 
@@ -213,16 +209,15 @@
     True: Service got enabled
     False: There was some problem.
     """
     cmd = f"systemctl enable {service_name}"
     if now:
         cmd = cmd + " --now"
 
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not enable {service_name}")
         run(f"systemctl status {service_name}")
         run("journalctl -xn")
         return False
     return True
 
 
@@ -242,15 +237,15 @@
     has_systemctl = True
 
     if not exists("systemctl"):
         has_systemctl = False
     if not has_systemctl:
         cmd = f"service {service_name} status"
 
-    retcode = run(cmd, return_output=False, verbose=verbose)
+    retcode = run(cmd, capture_output=False, verbose=verbose).returncode
     if retcode == 0:
         sts_print(f"INFO: Service {service_name} is running.")
     elif retcode == 1:
         sts_print(f"INFO: Service {service_name} is dead and /run pid file exists.")
     elif retcode == 2:
         sts_print(f"INFO: Service {service_name} is dead and /lock lock file exists.")
     elif retcode == 3:
@@ -270,25 +265,25 @@
      True: service is running
      False: service is not running.
     """
     return service_status(service_name, verbose=False) == 0
 
 
 def os_arch():
-    ret, arch = run("uname -m", verbose=False, return_output=True)
+    ret, arch = run_ret_out("uname -m", verbose=False, return_output=True)
     if ret != 0:
         sts_print("FAIL: could not get OS arch")
         return None
 
     return arch
 
 
 def is_installed(pack, verbose=False):
     """Checks if package is installed."""
-    ret, ver = run(f"rpm -q {pack}", verbose=False, return_output=True)
+    ret, ver = run_ret_out(f"rpm -q {pack}", verbose=False, return_output=True)
     if ret == 0:
         if verbose:
             print(f"INFO: {pack} is installed ({ver})")
         return True
 
     if verbose:
         print(f"INFO: {pack} is not installed ")
@@ -301,15 +296,15 @@
     if check and is_installed(pack, verbose):
         return True
 
     packmngr = "yum"
     if is_installed("dnf"):
         packmngr = "dnf"
 
-    if run(f"{packmngr} install -y {pack}") != 0:
+    if run(f"{packmngr} install -y {pack}").returncode != 0:
         msg = f"FAIL: Could not install {pack}"
         sts_print(msg)
         return False
 
     if verbose:
         print(f"INFO: {pack} was successfully installed")
     return True
@@ -322,15 +317,15 @@
         return None
 
     release = dist_name().lower()
     if not release:
         sts_print("FAIL: package_version() - Couldn't get release")
         return None
     if exists("rpm"):
-        ret, output = run(
+        ret, output = run_ret_out(
             "rpm -qa --qf='%%{version}.%%{release}' %s" % pkg,
             return_output=True,
             verbose=False,
         )
         if ret != 0:
             sts_print(f"FAIL: Could not get version for package: {pkg}")
             print(output)
@@ -369,28 +364,28 @@
     return parse_version(version + "." + release) < parse_version(pkg)
 
 
 def wait_udev(sleeptime=15):
     """Wait udev to finish. Often used after scsi rescan."""
     sts_print("INFO: Waiting udev to finish storage scan")
     # For example, on RHEL 7 scsi_wait_scan module is deprecated
-    if run("modinfo scsi_wait_scan", verbose=False) == 0:
+    if run("modinfo scsi_wait_scan", verbose=False).returncode == 0:
         run("modprobe -q scsi_wait_scan")
         run("modprobe -r -q scsi_wait_scan")
 
     run("udevadm settle")
     sleep(sleeptime)
 
     return True
 
 
 def get_all_loaded_modules():
     """Check /proc/modules and return a list of all modules that are loaded."""
     cmd = 'cat /proc/modules | cut -d " " -f 1'
-    ret, output = run(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
         sts_print(f"FAIL: load_module() - Could not execute: {cmd}")
         print(output)
         return None
 
     return output.split("\n")
 
@@ -400,15 +395,15 @@
     Parameters:
     module:       module name and it's parameters.
     """
     if not module:
         sts_print("FAIL: load_module() - requires module parameter")
         return False
     cmd = f"modprobe {module}"
-    if run(cmd) != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: load_module() - Could not execute: {module}")
         return False
     return True
 
 
 def unload_module(module_name, remove_dependent=False):
     """Run rmmod to unload module
@@ -425,15 +420,15 @@
         if dep_modules:  # print info only if there are any modules to remove
             sts_print(f"INFO: Removing modules dependent on {module_name}")
             for module in dep_modules:
                 if not unload_module(module, remove_dependent=remove_dependent):
                     sts_print("FAIL: unload_module() - Could not unload dependent modules")
                     return False
 
-    if run(cmd) != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: unload_module() - Could not unload: {module_name}")
         return False
 
     return True
 
 
 def get_dependent_modules(module_name):
@@ -442,15 +437,15 @@
     Parameters:
     module_name:      module_name.
     """
     if not module_name:
         sts_print("FAIL: get_dependent_modules() - requires module_name parameter")
         return None
     cmd = f'cat /proc/modules | grep -Ew "^{module_name}" | cut -d \' \' -f 4 | tr "," " "'
-    ret, dependent_modules = run(cmd, return_output=True, verbose=False)
+    ret, dependent_modules = run_ret_out(cmd, return_output=True, verbose=False)
     if dependent_modules == "-":
         return []  # No dependent modules found
     if ret != 0:
         sts_print("FAIL: get_dependent_modules() - failed to get a list of modules")
         return None
     return dependent_modules.split()
 
@@ -489,15 +484,15 @@
         cmd += f" -t {fs}"
     if options:
         cmd += f" -o {options}"
     if device:
         cmd += f" {device}"
     if mountpoint:
         cmd += f" {mountpoint}"
-    if run(cmd) != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not mount partition")
         return False
 
     return True
 
 
 def umount(device=None, mountpoint=None):
@@ -510,15 +505,15 @@
 
     if mountpoint:
         cmd += f" {mountpoint}"
         if not is_mounted(mountpoint=mountpoint):
             # Device is not mounted
             return True
 
-    if run(cmd) != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not umount partition")
         return False
 
     return True
 
 
 def get_default_fs():
@@ -557,15 +552,15 @@
         sleep(1)
         if check_pid(pid):
             return False
     return True
 
 
 def kill_all(process_name):
-    ret = run(f"killall {process_name}", verbose=None)
+    ret = run(f"killall {process_name}", verbose=False).returncode
     # Wait few seconds for process to finish
     sleep(3)
     return ret
 
 
 def check_pid(pid):
     """Check there is a process running with this PID."""
@@ -591,15 +586,15 @@
     if in_seconds:
         ts = now.strftime("%s")
     return ts
 
 
 def kernel_command_line():
     """Return the kernel command line used to boot."""
-    retcode, output = run("cat /proc/cmdline", return_output=True, verbose=False)
+    retcode, output = run_ret_out("cat /proc/cmdline", return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: could not get kernel command line")
         print(output)
         return None
     return output
 
 
@@ -609,15 +604,15 @@
     Purpose
         Check out running kernel version. The same as output of `uname -r`
     Parameter
         N/A
     Returns
         kernel_version.
     """
-    retcode, output = run("uname -r", return_output=True, verbose=False)
+    retcode, output = run_ret_out("uname -r", return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: could not get kernel version")
         print(output)
         return None
     # remove arch detail and kernel type
     return re.sub(r"\.%s.*" % os_arch(), "", output)
 
@@ -631,15 +626,15 @@
             2. debug kernel.
             3. rt kernel.
     Parameter
         N/A
     Returns
         kernel_type        # 'debug|rt|default'.
     """
-    retcode, version = run("uname -r", return_output=True, verbose=False)
+    retcode, version = run_ret_out("uname -r", return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: kernel_type() - could not get kernel version")
         print(version)
         return None
 
     if re.match(r".*\.debug$", version):
         return "debug"
@@ -674,21 +669,21 @@
         return False
 
     k_commandline = kernel_command_line()
     if not re.search("kmemleak=on", k_commandline):
         sts_print("WARN: kmem_leak_start(): need 'kmemleak=on' kernel_option to enable kernel memory leak detection")
 
     check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
-    retcode = run(check_debugfs_mount_cmd, verbose=False)
+    retcode = run(check_debugfs_mount_cmd, verbose=False).returncode
     if retcode != 0:
         # debugfs is not mounted
         mount_debugfs_cli_cmd = "mount -t debugfs nodev /sys/kernel/debug"
         run(mount_debugfs_cli_cmd, verbose=True)
         check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
-        retcode, output = run(check_debugfs_mount_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(check_debugfs_mount_cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print("WARN: Failed to mount debugfs to /sys/kernel/debug")
             print(output)
             return False
 
     # enable kmemleak and clear
     sts_print("INFO: Begin kernel memory leak check")
@@ -748,16 +743,16 @@
         False       # failed to run 'echo' command.
     """
     sysfs_kmemleak = "/sys/kernel/debug/kmemleak"
     if not Path(sysfs_kmemleak).is_file():
         return True
 
     sts_print("INFO: kmem_leak_disable(): Disabling kernel memory leak detection")
-    ok1, ok1_output = run(f"echo scan=off > {sysfs_kmemleak}", return_output=True)
-    ok2, ok2_output = run(f"echo stack=off > {sysfs_kmemleak}", return_output=True)
+    ok1, ok1_output = run_ret_out(f"echo scan=off > {sysfs_kmemleak}", return_output=True)
+    ok2, ok2_output = run_ret_out(f"echo stack=off > {sysfs_kmemleak}", return_output=True)
     if ok1 != 0 or ok2 != 0:
         print("FAIL: kmem_leak_disable(): Failed to disable kernel memory leak detection")
         print(ok1_output)
         print(ok2_output)
         return False
 
     sts_print("INFO: kmem_leak_disable(): Kernel memory leak detection disabled")
@@ -812,49 +807,49 @@
 
     driver_info = {}
     infos = ["srcversion", "version", "taint"]
     for info in infos:
         info_path = sysfs_driver_folder / info
         if not Path(info_path).is_file():
             continue
-        _, output = run(f"cat {info_path}", return_output=True, verbose=False)
+        output = run(f"cat {info_path}", capture_output=True, verbose=False).output
         driver_info[info] = output
 
     sys_driver_parameter = sysfs_driver_folder / "parameters"
     if sys_driver_parameter.is_dir():
         # Need to add driver parameters
         param_files = list(sys_driver_parameter.iterdir())
         for param in param_files:
-            _, output = run(f"cat {sys_driver_parameter}/{param}", return_output=True, verbose=False)
+            output = run(f"cat {sys_driver_parameter}/{param}", capture_output=True, verbose=False).output
             if "parameters" not in driver_info:
                 driver_info["parameters"] = {}
             driver_info["parameters"][param] = output
     return driver_info
 
 
 def mkdir(new_dir):
     if Path(new_dir).is_dir():
         sts_print(f"INFO: {new_dir} already exist")
         return True
     cmd = f"mkdir -p {new_dir}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: could create directory {new_dir}")
         print(output)
         return False
     return True
 
 
 def rmdir(dir_name):
     """Remove directory and all content from it."""
     if not Path(dir_name).is_dir():
         sts_print(f"INFO: {dir_name} does not exist")
         return True
     cmd = f"rm -rf {dir_name}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: could remove directory {dir_name}")
         print(output)
         return False
     return True
 
 
@@ -868,27 +863,27 @@
     if fs_type == "xfs":
         force_option = "-f"
 
     cmd = f"mkfs.{fs_type} "
     if force:
         cmd += f"{force_option} "
     cmd += device_name
-    retcode, output = run(cmd, return_output=True, verbose=True)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
     if retcode != 0:
         sts_print(f"FAIL: could create filesystem {fs_type} on {device_name}")
         print(output)
         return False
     return True
 
 
 def sync(directory=None):
     cmd = "sync"
     if directory:
         cmd += f" {directory}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: could not sync")
         print(output)
         return False
     return True
 
 
@@ -899,15 +894,15 @@
     /root
     ./.
     """
     if not path:
         return None
 
     cmd = f"df -B 1 {path}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: get_free_space() - could not run {cmd}")
         print(output)
         return None
     fs_list = output.split("\n")
     # delete the header info
     del fs_list[0]
@@ -931,15 +926,15 @@
     eg. lvm1 from /dev/mapper/lvm1.
     """
     if not device.startswith("/dev/"):
         device = get_full_path(device)
     if not device:
         sts_print("FAIL: get_block_device_name - unknown device")
     cmd = f"lsblk -ndlo NAME {device}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: run {cmd}")
         print(output)
         return None
     return output
 
 
@@ -947,15 +942,15 @@
     """Returns full block device path, eg. from device: /dev/mapper/device."""
     cmds = [
         f"lsblk -pnalo NAME  | grep {device_name} -m1",  # should be more robust
         f"find /dev/ -name {device_name}",
     ]  # older OS(rhel-6), will fail with partitions
 
     for cmd in cmds:
-        retcode, output = run(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode == 0 and output != "":
             return output
 
     sts_print(f"FAIL: get_full_path() - {device_name}")
     return None
 
 
@@ -967,15 +962,15 @@
     if not child_device.startswith("/dev/"):
         child_device = get_full_path(child_device)
     if not child_device:  # get_full_path would return None if device does not exist
         sts_print(f"FAIL: get_parent_device - unknown child_device '{child_device}'")
     cmd = f"lsblk -nsl {child_device} -o KNAME | tail -n 1"
     if only_direct:
         cmd = f"lsblk -nsl {child_device} -o KNAME | sed -n 2p"  # if no parent, returns nothing
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: run {cmd}")
         print(output)
         return None
     if output == "" or output == child_device:
         sts_print("WARN: get_parent_device - device has no parent")
         return None
@@ -1000,15 +995,15 @@
         sts_print(f"FAIL: get_udev_property - unknown device_name '{device_name}'")
 
     # Trying to catch wrong key name when dm-multipath is used.
     if mp.is_mpath_device(device_name, print_fail=False):  # noqa: SIM102
         if property_key.startswith("ID_") and not property_key.startswith("ID_FS_"):
             property_key = property_key.replace("ID_", "DM_")
 
-    ret, property_value = run(
+    ret, property_value = run_ret_out(
         f"udevadm info -q property --name={device} | grep {property_key}= | cut -d = -f 2",
         return_output=True,
         verbose=False,
     )
     if ret:
         sts_print(f"WARN: Could not get udevadm info of device '{device}'")
         return None
@@ -1024,23 +1019,23 @@
     parent_device, eg. 'sda'
     full_path, eg. '/dev/sda1'.
     """
     boot_mount = "/boot"
     root_mount = "/"
     # get boot device
     cmd = f"mount | grep ' {boot_mount} ' | cut -d ' ' -f 1"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: run {cmd}")
         print(output)
         return None
     boot_device = output
     # get root device
     cmd = f"mount | grep ' {root_mount} ' | cut -d ' ' -f 1"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: run {cmd}")
         print(output)
         return None
     root_device = output
 
     if not boot_device and not root_device:
@@ -1068,15 +1063,15 @@
       device_name: e.g. 'sda', 'mpatha', ...
     """
     # Converts for example mpatha to /dev/mapper/mpatha or sda to /dev/sda
     device = get_full_path(device_name)
     if not device:
         sts_print(f"FAIL: is_dm_device - unknown device_name '{device_name}'")
         return False
-    ret, name = run(f"udevadm info -q name --name={device}", return_output=True)
+    ret, name = run_ret_out(f"udevadm info -q name --name={device}", return_output=True, verbose=False)
     if ret:
         sts_print(f"FAIL: Could not get udevadm info for device '{device}'")
         return False
     if not name:
         sts_print(f"FAIL: Could not find udev name for '{device}'")
         return False
 
@@ -1154,15 +1149,15 @@
 def get_partitions(device):
     """Return a list of all parition numbers from the device."""
     if not device:
         sts_print("WARN: get_partitions() - requires device as parameter")
         return None
 
     cmd = f"parted -s {device} print"
-    ret, output = run(cmd, verbose=False, return_output=True)
+    ret, output = run_ret_out(cmd, verbose=False, return_output=True)
     if ret != 0:
         # sts_print("FAIL: get_partitions() - Could not read partition information from %s" % device)
         # print output
         return None
 
     lines = output.split("\n")
     if not lines:
@@ -1187,15 +1182,15 @@
 def delete_partition(device, partition):
     """Delete specific partition from the device."""
     if not device or not partition:
         sts_print("FAIL: delete_partition() - requires device and partition as argument")
         return False
 
     cmd = f"parted -s {device} rm {partition}"
-    ret, output = run(cmd, verbose=False, return_output=True)
+    ret, output = run_ret_out(cmd, verbose=False, return_output=True)
     if ret != 0:
         sts_print("FAIL: delete_partition() - Could not delete partition %d from %s" % (partition, device))
         print(output)
         return False
 
     return True
 
@@ -1263,30 +1258,29 @@
 def check_repo(name, check_if_enabled=True):
     """Checks if repository works and is enabled."""
     if not name:
         print("FAIL: repo name argument required")
         return False
 
     cmd = f"yum repoinfo {name} | grep Repo-status"  # yum=dnf alias works here
-    ret, out = run(cmd, return_output=True)
+    ret, out = run_ret_out(cmd, return_output=True)
     if ret != 0:
         print(f"{name} repo is not present")
         return False
     if check_if_enabled and "enabled" not in out:
         print(f"{name} repo is not enabled")
         return False
 
     return True
 
 
 def is_docker():
     """Check if we are running inside docker container."""
     cmd = "cat /proc/self/cgroup | grep docker"
-    ret = run(cmd, verbose=False, return_output=False)
-    if ret == 0:
+    if run(cmd, verbose=False).returncode == 0:
         # It is docker
         return True
     return False
 
 
 def get_memory(units="m", total=False):
     """Returns data from 'free' as a dict."""
@@ -1299,15 +1293,15 @@
     columns = []
 
     if len(units) > 1:
         units = "-" + units
     cmd = f"free -{units}"
     if total:
         cmd += " -t"
-    ret, mem = run(cmd=cmd, return_output=True)
+    ret, mem = run_ret_out(cmd=cmd, return_output=True)
     if ret != 0:
         sts_print(f"FAIL: Running '{cmd}' failed.")
         return None
 
     for row, m in enumerate(mem.splitlines()):
         if row == 0:
             columns = [c.strip() for c in m.split()]
@@ -1329,15 +1323,15 @@
 
     Returns:
     Time in format: a YYYY-MM-DD hh:mm:ss Z
     None: systemctl is not installed or timestamp does not exist
     """
     if not exists("systemctl"):
         cmd = f"systemctl show {service_name} --property=ActiveEnterTimestamp"
-        ret, data = run(cmd, return_output=True)
+        ret, data = run_ret_out(cmd, return_output=True)
         if ret == 0:
             timestamp = data.split("=")
             if timestamp[1] != "":
                 return timestamp[1]
             return None
         sts_print(f"WARN: Could not get active enter timestamp of service: {service_name}")
     return None
@@ -1380,15 +1374,15 @@
         cmd += f" -S {since}"
     if options:
         cmd += " " + " ".join(options)
 
     if grep:
         cmd += f" | grep '{grep}'"
 
-    ret, journal = run(cmd, return_output=return_output, verbose=verbose)
+    ret, journal = run_ret_out(cmd, return_output=return_output, verbose=verbose)
     if ret:
         sts_print(f"FAIL: cmd '{cmd}' failed with retcode {ret}.")
         return None
     if not return_output:
         return ret
 
     # shorten the hostname to match /var/log/messages format
@@ -1495,15 +1489,15 @@
         print("INFO: Unmounting /var/crash to avoid sosreport being hang there")
         umount("/var/crash")
         mount_flag = True
 
     if skip_plugins:
         cmd = cmd + f" --skip-plugins {skip_plugins}"
 
-    ret_code, sosreport_ret = run(cmd, return_output=True, timeout=timeout)
+    ret_code, sosreport_ret = run_ret_out(cmd, return_output=True, timeout=timeout)
     if ret_code != 0:
         print("FAIL: sosreport command failed")
         if mount_flag:
             mount("/var/crash")
         return False
 
     sos_report = None
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/lio.py` & `sts_libs-0.0.4/sts_libs/src/sts/lio.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re  # regex
 
 from sts import fc, linux
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 regex_tgtcli_wwpn = "naa.\\S+"
 
 
 def _tgt_wwn_2_wwn(wwn):
     """On RHEL-6 targetcli stores WWN on WWN format,
     but on RHEL-7 it is something like: naa.200090e2baa397ca
@@ -56,15 +56,15 @@
     """Query all information from targetcli using targetcli ls
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with targetcli information.
     """
     cmd = "targetcli ls"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not run targetcli")
         return None
     lio_data = output.split("\n")
 
     lio_field_regex = re.compile(r"o-\s(.*?)\s.*\[(.*)\]")
     # supported types for LIO
@@ -395,15 +395,15 @@
 def lio_get_backstore_lun_details(bs_type, lun_name):
     """Get the detailed information about the lun."""
     if not bs_type or not lun_name:
         sts_print("FAIL: lio_get_backstore_lun_details() - requires bs_type and lun_name")
         return None
 
     cmd = f"targetcli /backstores/{bs_type}/{lun_name} info"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: Could not get {bs_type} details for {lun_name}")
         return None
 
     details = output.split("\n")
     supported_details = {
         "dev": r"^dev: (\S+)",
@@ -469,25 +469,23 @@
         print("FAIL: _lio_create_backstore_block needs lun_name parameter")
         return False
     if not device:
         print("FAIL: _lio_create_backstore_block needs device parameter")
         return False
 
     cmd = f"targetcli /backstores/block create {lun_name} {device}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: Could not create block {lun_name}")
         return False
     return True
 
 
 def _lio_delete_backstore_block(lun_name):
     cmd = f"targetcli /backstores/block delete {lun_name}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: Could not delete block {lun_name}")
         return False
 
     return True
 
 
 # ## FILEIO ###
@@ -502,71 +500,64 @@
 
     # disable spare, to force targetcli to allocate the whole file to avoid problem
     # of running out of disk space and not have enough space to store data
     cmd = f"targetcli /backstores/fileio create {lun_name} {file_name} sparse=false"
     if lun_size:
         cmd = cmd + f" {lun_size}"
 
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: Could not create fileio {lun_name}")
         return False
     return True
 
 
 def _lio_delete_backstore_fileio(lun_name):
     file_name = _lio_get_backstore_fileio_file(lun_name)
 
-    cmd = f"targetcli /backstores/fileio delete {lun_name}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(f"targetcli /backstores/fileio delete {lun_name}").returncode != 0:
         sts_print(f"FAIL: Could not delete fileio {lun_name}")
         return False
 
-    if file_name:
-        cmd = f"rm -f {file_name}"
-        retcode = run(cmd, return_output=False, verbose=True)
-        if retcode != 0:
-            sts_print(f"WARN: could not delete file {file_name}")
+    if file_name and run(f"rm -f {file_name}").returncode != 0:
+        sts_print(f"WARN: could not delete file {file_name}")
 
     return True
 
 
 def _lio_get_backstore_fileio_file(lun_name):
     """Get the file used by a specific LUN."""
     cmd = f"targetcli /backstores/fileio/{lun_name} ls"
-    retcode, output = run(cmd, return_output=True, verbose=False)
-    if retcode != 0:
+    completed_process = run(cmd, capture_output=True, verbose=False)
+    if completed_process.returncode != 0:
         sts_print(f"FAIL: Could not get fileio file {lun_name}")
         return None
 
     path_regex = re.compile(r"\[(.*)\s\(")
-    m = path_regex.search(output)
+    m = path_regex.search(completed_process.output)
     if m:
         return m.group(1)
     return None
 
 
 # ## PSCSI ###
 def _lio_create_backstore_pscsi(lun_name, device, lun_size=None):
     cmd = f"targetcli /backstores/pscsi create {lun_name} {device}"
     if lun_size:
         cmd = cmd + f" {lun_size}M"
 
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not create pscsi {lun_name}")
         return False
     return True
 
 
 def _lio_delete_backstore_pscsi(lun_name):
     cmd = f"targetcli /backstores/pscsi delete {lun_name}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete pscsi {lun_name}")
         return False
 
     return True
 
 
 ##################################################
@@ -598,16 +589,16 @@
     False: If some problem happened.
     """
     if not lio_support_iscsi_target():
         sts_print("FAIL: server does not support iSCSI target")
         return False
 
     cmd = f"targetcli /iscsi/ create {iqn}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not create iSCSI target {iqn}")
         return False
 
     if iqn not in lio_iscsi_get_target():
         sts_print("FAIL: It seems to have added iSCSI target, but it did not")
         lio_dict = lio_query()
         print(lio_dict["iscsi"])
@@ -655,16 +646,15 @@
     True: If target is attribute is set
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi set {group} {attr_name}={attr_value}"
     if tgt_iqn:
         cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/ set {group} {attr_name}={attr_value}"
 
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print(f"FAIL: Could not set iSCSI target attribute {attr_name}")
         return False
     return True
 
 
 # ## iSCSI ACLS ###
 def lio_iscsi_create_acl(tgt_iqn, tpg, init_iqn):
@@ -674,16 +664,16 @@
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init IQN is created
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls create {init_iqn} add_mapped_luns=false"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not add iSCSI initiator {init_iqn}")
         return False
     return True
 
 
 def lio_iscsi_delete_acl(tgt_iqn, tpg, init_iqn):
     """Remove an initiator IQN from target IQN
@@ -692,16 +682,16 @@
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init iqn is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls delete {init_iqn}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete iSCSI initiator {init_iqn}")
         return False
 
     return True
 
 
 # ## iSCSI LUNs ###
@@ -718,16 +708,16 @@
     """
     cmd = "targetcli /iscsi/{}/{}/luns create /backstores/{}/{} add_mapped_luns=false".format(
         tgt_iqn,
         tpg,
         bs_type,
         lun_name,
     )
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not add lun to iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
 def lio_iscsi_remove_lun(tgt_iqn, tpg, lun_id):
@@ -737,16 +727,16 @@
     tpg:         Target Portal Group
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/luns delete {lun_id}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete LUN from iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
 def lio_iscsi_get_luns(tgt_iqn, tpg):
@@ -788,16 +778,16 @@
 
     portal = portal_ip + ":" + portal_port
     if portal in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
         print(f"INFO: portal {portal} does already exist on target {tgt_iqn}")
         return True
 
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals create {portal_ip} {portal_port}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
         return False
 
     return True
 
 
 def lio_iscsi_delete_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):
@@ -818,16 +808,16 @@
 
     portal = portal_ip + ":" + portal_port
     if portal not in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
         print(f"INFO: portal {portal} does not exist on target {tgt_iqn}")
         return True
 
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals delete {portal_ip} {portal_port}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
         return False
     return True
 
 
 # ## iSCSI LUNs mapping ###
 def lio_iscsi_map_lun(tgt_iqn, tpg, init_iqn, init_lun_id, bs_type, lun_name):
@@ -838,16 +828,16 @@
     init_iqn:     Host IQN
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
     lun_path = f"/backstores/{bs_type}/{lun_name}"
     cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls/{init_iqn} create {init_lun_id} {lun_path}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not map lun to iSCSI target {tgt_iqn}/{init_iqn}")
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
         sts_print(f"FAIL: It seems to have mapped lun {init_lun_id}, but it did not")
         return False
 
@@ -862,16 +852,16 @@
     tpg:          Target Portal group
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/{init_iqn}/acls/{tpg} delete {init_lun_id}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not unmap LUN from target {tgt_iqn}/{init_iqn}")
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
         sts_print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
         return False
     return True
@@ -885,15 +875,15 @@
     tpg:          Target Portal group no.
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/tpg{tpg}/acls/{init_iqn} ls | grep {tgt_lun_id}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}")
         return False
 
     if output == "":
         return False
     return True
@@ -1067,22 +1057,22 @@
     False: If some problem happened.
     """
     if not wwn:
         sts_print("FAIL: lio_create_fc_target() - requires wwn parameter")
         return False
 
     cmd = f"targetcli /tcm_fc/ create {wwn}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: lio_create_fc_target() - Could not create FC target {wwn}")
         return False
 
     if wwn not in lio_get_fc_target():
         lio_dict = lio_query()
-        run("targetcli ls", return_output=False, verbose=True)
+        run("targetcli ls", verbose=True)
         sts_print("FAIL: lio_create_fc_target() - It seems to have added FC target, but it did not")
         print(lio_dict["tcm_fc"])
         print(lio_dict)
 
         return False
 
     return True
@@ -1097,16 +1087,16 @@
     False: If some problem happened.
     """
     if not wwn:
         sts_print("FAIL: lio_delete_fc_target() - requires wwn parameter")
         return False
 
     cmd = f"targetcli /tcm_fc/ delete {wwn}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: lio_delete_fc_target() - Could not delete FC target {wwn}")
         return False
 
     if wwn in lio_get_fc_target():
         lio_dict = lio_query()
         run("targetcli ls", return_output=False, verbose=True)
         sts_print("FAIL: lio_delete_fc_target() - It seems to have deleted FC target, but it did not")
@@ -1147,16 +1137,16 @@
     """
     tgt_acls = lio_get_fc_target_acl(tgt_wwn, lio_dict=lio_dict)
     if tgt_acls and (init_wwn in tgt_acls):
         print(f"INFO: {init_wwn} is already added to target {tgt_wwn}")
         return True
 
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls create {init_wwn} add_mapped_luns=false"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not add FC initiator {init_wwn}")
         return False
 
     return True
 
 
 def lio_delete_fc_target_acl(tgt_wwn, init_wwn):
@@ -1165,16 +1155,16 @@
     tgt_wwn:     Host WWN
     init_wwn:    Initiator WWN
     Returns:
     True: If init wwn is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls delete {init_wwn}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete FC initiator {init_wwn}")
         return False
 
     return True
 
 
 def lio_get_fc_target_acl(tgt_wwn, lio_dict=None):
@@ -1215,16 +1205,16 @@
     False: If some problem happened.
     """
     cmd = "targetcli /tcm_fc/{}/luns create /backstores/{}/{} add_mapped_luns=false".format(
         _wwn_2_tgt_wwn(tgt_wwn),
         bs_type,
         lun_name,
     )
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not add lun to FC target {tgt_wwn}")
         return False
 
     return True
 
 
 def lio_delete_fc_target_lun(tgt_wwn, lun_id):
@@ -1233,16 +1223,16 @@
     tgt_wwn:     Target WWN
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/luns delete {lun_id}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not delete LUN from target {tgt_wwn}")
         return False
 
     return True
 
 
 def lio_get_fc_target_luns(tgt_wwn, lio_dict=None):
@@ -1288,15 +1278,15 @@
     for lun_id in list(t_luns_dict.keys()):
         if t_luns_dict[lun_id]["bs_type"] == bs_type and t_luns_dict[lun_id]["lun_name"] == lun_name:
             return lun_id
     return None
 
 
 #    cmd = "targetcli /tcm_fc/%s/luns ls | grep %s/%s | awk '{print$2}'" % (_wwn_2_tgt_wwn(tgt_wwn), bs_type, lun_name)
-#    retcode, output = run(cmd, return_output=True, verbose=False)
+#    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
 #    if (retcode != 0):
 #        sts_print ("FAIL: Could not get lun %s for FC target %s" % (lun_name, tgt_wwn))
 #        return None
 #
 #    if output == "":
 #        return None
 #    return output
@@ -1361,16 +1351,16 @@
 
     cmd = "targetcli /tcm_fc/{}/acls/{} create {} {}".format(
         _wwn_2_tgt_wwn(tgt_wwn),
         _wwn_2_tgt_wwn(init_wwn),
         init_lun_id,
         tgt_lun_id,
     )
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not map lun to FC target {tgt_wwn}/{init_wwn}")
         return False
 
     if not lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id):
         sts_print(f"FAIL: It seems to have mapped lun {tgt_lun_id}, but it did not")
         return False
 
@@ -1405,16 +1395,16 @@
     init_wwn:     Host WWN
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls/{_wwn_2_tgt_wwn(init_wwn)} delete {init_lun_id}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not unmap LUN from target {tgt_wwn}/{init_wwn}")
         return False
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id):
         sts_print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
         return False
     return True
@@ -1479,16 +1469,16 @@
     init_wwn:    Initiator wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls tag {_wwn_2_tgt_wwn(init_wwn)} {tag}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not tag FC initiator {init_wwn}")
         return False
 
     return True
 
 
 def lio_untag_fc_initiator(tgt_wwn, tag):
@@ -1497,16 +1487,16 @@
     tgt_wwn:     Host wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls untag {tag}"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print(f"FAIL: Could not untag FC tag {tag}")
         return False
 
     return True
 
 
 def lio_is_fc_tag(tgt_wwn, tag):
@@ -1514,16 +1504,15 @@
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     cmd = f"targetcli /tcm_fc/{tgt_wwn}/acls/{tag}"
-    retcode = run(cmd, return_output=False, verbose=False)
-    if retcode != 0:
+    if run(cmd, verbose=False).returncode != 0:
         return False
     return True
 
 
 ##################################################
 # ################ LIO General ####################
 ##################################################
@@ -1596,32 +1585,32 @@
     The arguments are:
     None
     Returns:
     True: If listed config
     False: If some problem happened.
     """
     cmd = "targetcli ls"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print("FAIL: Could not show LIO config")
         return False
     return True
 
 
 def lio_saveconfig():
     """Save LIO configuration
     The arguments are:
     None
     Returns:
     True: If config is saved
     False: If some problem happened.
     """
     cmd = "targetcli saveconfig"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print("FAIL: Could not save LIO config")
         return False
     return True
 
 
 def lio_clearconfig():
     """Clear LIO configuration
@@ -1639,16 +1628,16 @@
     fileio_dict = lio_get_backstores("fileio")
     if fileio_dict:
         # Delete all files before cleaning configuration
         for lun in list(fileio_dict.keys()):
             lio_delete_backstore(bs_type="fileio", lun_name=lun)
 
     cmd = "targetcli clearconfig true"
-    retcode = run(cmd, return_output=False, verbose=True)
-    if retcode != 0:
+
+    if run(cmd, verbose=True).returncode != 0:
         sts_print("FAIL: Could not delete LIO config")
         return False
 
     return True
 
 
 def lio_version():
@@ -1656,15 +1645,15 @@
     The arguments are:
     None
     Returns:
     String: TargetCli version
     None: If some problem happened.
     """
     cmd = "targetcli version"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: Could not get targetcli version")
         return None
 
     version_regex = re.compile(".* version (.*)$")
     m = version_regex.search(output)
     if m:
@@ -1738,20 +1727,20 @@
 
         if path is not None:
             self.path = path
 
         cmd = "targetcli cd" if cmd == "cd" and self.path is None else "targetcli " + self.path + " " + cmd
 
         if return_output:
-            ret, data = run(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
                 sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
-        ret = run(cmd, verbose=verbosity)
+        ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     def ls(self, depth="", **kwargs):
         return self._run(f"ls {depth}", **kwargs)
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.4/sts_libs/src/sts/loopdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import sys
 from pathlib import Path
 
 from sts import linux
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 from sts.utils.size import size_bytes_2_size_human, size_human_2_size_bytes
 
 
 def _get_loop_path(name):
     loop_path = name
     if "/dev/" not in name:
         loop_path = "/dev/" + name
@@ -46,15 +46,15 @@
 
     #    size = args['size']
     #    if size is None:
     #        size = 1024
 
     if not name:
         cmd = "losetup -f"
-        retcode, output = run(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print("FAIL: Could not find free loop device")
             print(output)
             return None
         name = output
     name = _standardize_name(name)
 
@@ -77,31 +77,29 @@
         sts_print(f"available space: {size_bytes_2_size_human(free_space_bytes)}")
         return None
     print(f"INFO: Creating file {fname}")
     # cmd = "dd if=/dev/zero of=%s seek=%d bs=1M count=0" % (fname, size)
     cmd = f"fallocate -l {size}M {fname}"
     try:
         # We are just creating the file, not writting zeros to it
-        retcode = run(cmd)
-        if retcode != 0:
+        if run(cmd).returncode != 0:
             sts_print(f"command failed with code {retcode}")
             sts_print("FAIL: Could not create loop device image file")
             return None
     except OSError as e:
         print("command failed: ", e, file=sys.stderr)
         return None
 
     loop_path = _get_loop_path(name)
     # detach loop device if it exists
     detach_loopdev(loop_path)
 
     # Going to associate the file to the loopdevice
     cmd = f"losetup {loop_path} {fname}"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not create loop device")
         return None
 
     return loop_path
 
 
 def delete_loopdev(name):
@@ -128,39 +126,38 @@
     # detach loop device if it exists
     if not detach_loopdev(name):
         sts_print(f"FAIL: could not detach {loop_path}")
         return False
 
     if Path(fname).is_file():
         cmd = f"rm -f {fname}"
-        retcode = run(cmd)
-        if retcode != 0:
+        if run(cmd).returncode != 0:
             sts_print(f"FAIL: Could not delete loop device file {fname}")
             return False
 
     # check if loopdev file is deleted as it sometimes remains
     if Path(fname).is_file():
         sts_print(f"FAIL: Deleted loop device file {fname} but it is still there")
         return False
 
     return True
 
 
 # show loop devices
 def list_loopdev():
-    retcode, output = run("losetup -a", return_output=True)
+    retcode, output = run_ret_out("losetup -a", return_output=True)
     return retcode, output
 
 
 # Return all loop devices
 def get_loopdev():
     # example of output on rhel-6.7
     # /dev/loop0: [fd00]:396428 (/var/tmp/loop0.img)
-    retcode, output = run("losetup -a | awk '{print$1}'", return_output=True, verbose=False)
-    # retcode, output = run("losetup -l | tail -n +2", return_output=True, verbose=False)
+    retcode, output = run_ret_out("losetup -a | awk '{print$1}'", return_output=True, verbose=False)
+    # retcode, output = run_ret_out("losetup -l | tail -n +2", return_output=True, verbose=False)
     if retcode != 0:
         sts_print("FAIL: get_loopdev failed to execute")
         print(output)
         return None
 
     devs = None
     if output:
@@ -171,15 +168,15 @@
     return devs
 
 
 # Return loop device file for given path
 def get_loopdev_file(loop_path):
     # example of output on rhel-6.7
     # /dev/loop0: [fd00]:396428 (/var/tmp/loop0.img)
-    retcode, output = run(
+    retcode, output = run_ret_out(
         "losetup -a | grep '%s:' | awk '{print$3}'" % loop_path,
         return_output=True,
         verbose=False,
     )
     if retcode != 0:
         sts_print("FAIL: get_loopdev_file failed to execute")
         print(output)
@@ -211,13 +208,12 @@
         if dev_path in devs:
             cmd = f"losetup -d {dev_path}"
         else:
             # if loop device does not exist just ignore it
             return True
 
     # run losetup -D or -d <device>
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not detach loop device")
         return False
 
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.4/sts_libs/src/sts/lsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sts.utils import sts_print
 from sts.utils.cli_tools import (
     FailedCheckExceptionError,
     Wrapper,
     WrongArgumentExceptionError,
     WrongCommandExceptionError,
 )
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 from sts.utils.persistent_vars import read_env, read_var
 
 
 def check_ssl(protocol) -> bool:
     """Checks if fmf_protocol is ssl/no_ssl and limits the protocol by this."""
     try:
         ssl = read_env("fmf_protocol")
@@ -251,15 +251,15 @@
                     else:
                         requires_restart = True
                 # needs to install 3rd party tool
                 if not linux.install_package("storcli"):
                     sts_print("FATAL: Could not install storcli")
 
         if requires_restart:
-            if run("service libstoragemgmt restart", verbose=True) != 0:
+            if run("service libstoragemgmt restart", verbose=True).returncode != 0:
                 sts_print("FATAL: Could not restart libstoragemgmt service")
             else:
                 sts_print("INFO: Waiting for service to restart.")
                 sleep(5)
         elif linux.service_status("libstoragemgmt") != 0:  # noqa: SIM102
             if linux.service_start("libstoragemgmt"):
                 sts_print("INFO: Waiting for service to start.")
@@ -537,20 +537,20 @@
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
             sts_print(f"WARN: Failed checking on argument {e.argument}")
             return ret_fail
 
         if return_output:
-            ret, data = run(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
                 sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
-        ret = run(cmd, verbose=verbosity)
+        ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
     def _remove_nones(kwargs):
         return {k: v for k, v in kwargs.items() if v is not None}
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.4/sts_libs/src/sts/lvm.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 from functools import wraps
 from pathlib import Path
 
 from sts import vdo
 from sts.utils import sts_print
 from sts.utils.cli_tools import Wrapper
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 
 def check_lv_expected_value(test_obj, lv_name, vg_name, opt_val_dict):
     if not test_obj or not opt_val_dict or not lv_name or not vg_name:
         return
 
     opt_str = ",".join(opt_val_dict)
@@ -42,15 +42,15 @@
     """Query Physical Volumes and return a dictionary with PV information for each PV.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with PV info for each PV.
     """
     cmd = 'pvs --noheadings --separator ","'
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print("INFO: there is no VGs")
         return None
     pvs = output.split("\n")
 
     # format of PV info: PV,VG,Fmt,Attr,PSize,PFree
     pv_info_regex = r"\s+(\S+),(\S+)?,(\S+),(.*),(.*),(.*)$"
@@ -82,16 +82,15 @@
     True if success
     False in case of failure.
     """
     if not pv_name:
         sts_print("FAIL: pv_create requires pv_name")
         return False
     cmd = f"pvcreate {options} {pv_name}"
-    retcode = run(cmd, verbose=verbose)
-    if retcode != 0:
+    if run(cmd, verbose=verbose).returncode != 0:
         # sts_print ("FAIL: Could not create %s" % pv_name)
         return False
     return True
 
 
 def pv_remove(pv_name: str, force=None, verbose=True):
     """Delete a Volume Group.
@@ -117,15 +116,15 @@
             sts_print(f"INFO: pv_remove - {pv_name} does not exist. Skipping...")
             return True
 
         options = ""
         if force:
             options += "--force --force"
         cmd = f"pvremove {options} {pv_name}"
-        retcode = run(cmd, verbose=verbose)
+        retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
             sts_print(f"FAIL: Could not delete {pv_name}")
             return False
     return True
 
 
 ###########################################
@@ -139,30 +138,29 @@
     None
     Returns:
     True
     or
     False.
     """
     cmd = "vgs -a"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not show VGs")
         return False
     return True
 
 
 def vg_query(verbose=False):
     """Query Volume Groups and return a dictonary with VG information for each VG.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with VG info for each VG.
     """
     cmd = 'vgs --noheadings --separator ","'
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print("INFO: there is no VGs")
         return None
     vgs = output.split("\n")
 
     # format of VG info: name #PV #LV #SN Attr VSize VFree
     vg_info_regex = r"\s+(\S+),(\S+),(\S+),(.*),(.*),(.*),(.*)$"
@@ -199,15 +197,15 @@
         sts_print("FAIL: vg_create requires vg_name and pv_name")
         return False
 
     options = ""
     if force:
         options += "--force"
     cmd = f"vgcreate {options} {vg_name} {pv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         # sts_print ("FAIL: Could not create %s" % vg_name)
         return False
     return True
 
 
 def vg_remove(vg_name: str, force=False, verbose=True):
@@ -230,15 +228,15 @@
         sts_print(f"INFO: vg_remove - {vg_name} does not exist. Skipping...")
         return True
 
     options = ""
     if force:
         options += "--force"
     cmd = f"vgremove {options} {vg_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         # sts_print ("FAIL: Could not delete %s" % vg_name)
         return False
     return True
 
 
 ###########################################
@@ -252,16 +250,15 @@
     None
     Returns:
     True
     or
     False.
     """
     cmd = "lvs -a"
-    retcode = run(cmd)
-    if retcode != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not show LVs")
         return False
     return True
 
 
 def lv_query(options="", verbose=False):
     """Query Logical Volumes and return a dictonary with LV information for each LV.
@@ -303,15 +300,15 @@
         parameters = options.split(",")
         for param in parameters:
             lv_info_regex += '","(.*)'
             param_names.append(param)
         lv_info_regex += "$"
         cmd += f" -o lv_name,vg_name,{options}"
 
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print("INFO: there is no LVs")
         return None
     lvs = output.split("\n")
 
     lv_list = []
     for lv in lvs:
@@ -339,15 +336,15 @@
     False in case of failure.
     """
     if not vg_name or not lv_name:
         sts_print("FAIL: lv_create requires vg_name and lv_name")
         return False
 
     cmd = f"lvcreate {' '.join(str(i) for i in options)} {vg_name} -n {lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         # sts_print ("FAIL: Could not create %s" % lv_name)
         return False
     return True
 
 
 def lv_info(lv_name: str, vg_name: str, options="", verbose=False):
@@ -378,15 +375,15 @@
     False if something went wrong.
     """
     if not lv_name or not vg_name:
         sts_print("FAIL: lv_activate requires lv_name and vg_name")
         return False
 
     cmd = f"lvchange -ay {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not activate LV {lv_name}")
         return False
 
     # Maybe we should query the LVs and make sure it is really activated
     return True
 
@@ -402,15 +399,15 @@
     False if something went wrong.
     """
     if not lv_name or not vg_name:
         sts_print("FAIL: lv_deactivate requires lv_name and vg_name")
         return False
 
     cmd = f"lvchange -an {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not deactivate LV {lv_name}")
         return False
 
     # Maybe we should query the LVs and make sure it is really deactivated
     return True
 
@@ -433,15 +430,15 @@
 
     for lv_name in lv_names:
         if not lv_info(lv_name, vg_name):
             sts_print(f"INFO: lv_remove - LV {lv_name} does not exist. Skipping")
             continue
 
         cmd = f"lvremove --force {vg_name}/{lv_name}"
-        retcode = run(cmd, verbose=verbose)
+        retcode = run(cmd, verbose=verbose).returncode
         if retcode != 0:
             sts_print(f"FAIL: Could not remove LV {lv_name}")
             return False
 
         if lv_info(lv_name, vg_name):
             sts_print(f"INFO: lv_remove - LV {lv_name} still exists.")
             return False
@@ -465,15 +462,15 @@
         return False
 
     if not lv_name or not vg_name:
         sts_print("FAIL: lv_convert requires vg_name and lv_name")
         return False
 
     cmd = f"lvconvert {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not convert {lv_name}")
         return False
 
     return True
 
 
@@ -493,15 +490,15 @@
         return False
 
     if not lv_name or not vg_name:
         sts_print("FAIL: lv_extend requires vg_name and lv_name")
         return False
 
     cmd = f"lvextend {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not extend {lv_name}")
         return False
 
     return True
 
 
@@ -521,15 +518,15 @@
         return False
 
     if not lv_name or not vg_name:
         sts_print("FAIL: lv_reduce requires vg_name and lv_name")
         return False
 
     cmd = f"lvreduce {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose)
+    retcode = run(cmd, verbose=verbose).returncode
     if retcode != 0:
         sts_print(f"FAIL: Could not reduce {lv_name}")
         return False
 
     return True
 
 
@@ -557,15 +554,15 @@
         # need to remove new line character as print will add it
         line = line.rstrip("\n")  # noqa: PLW2901
         print(line)
 
 
 def get_lvm_config_options(all_params=False):
     """Get all the configuration types from lvm.conf file."""
-    _, out = run("lvmconfig --type full", return_output=True, verbose=False)
+    out = run("lvmconfig --type full", capture_output=True, verbose=False).output
 
     options = {}
     category = ""
     for line in out.split("\n"):
         line = line.strip()  # noqa: PLW2901
         if line == "" or "}" in line:
             # skip empty or end of list line
@@ -584,16 +581,15 @@
     options_all = []
     for value in options.values():
         options_all.extend(value)
     return options_all
 
 
 def check_lvm_config(option):
-    _, out = run(f"lvs -o {option}", return_output=True)
-    return out
+    return run(f"lvs -o {option}", capture_output=True).output
 
 
 def get_all_lvm_config_options():
     all_opts = check_lvm_config("asdf")  # needs just something that it doesn't know
     # we need to test_filter on lines that look like this
     # lvm_blahblah - explanation
     # and remove separators
@@ -606,15 +602,15 @@
     # TODO: Duplicate of run_command
     """Decorator for running commands
     kwargs need to be edited every time, so decorator is probably the best solution.
     """
 
     @wraps(func)
     def wrapped(*args, **kwargs):
-        return run(func(), *args, **kwargs, return_output=True)  # cmd == func()
+        return run_ret_out(func(), *args, **kwargs, return_output=True)  # cmd == func()
 
     return wrapped
 
 
 @run_cmd
 def get_all_lvmvdoconfig_options():
     return "lvmconfig --type list"
@@ -838,20 +834,20 @@
         if "vg_name" in kwargs:
             command += kwargs["vg_name"]
         return command
 
     def _get_possible_arguments(self, command=None):
         return super()._get_possible_arguments(command.split()[0])
 
-    def run(self, cmd, verbosity=True, return_output=False, **kwargs):
+    def run(self, cmd, verbosity=True, **kwargs):
         """Constructs the command to run and runs it."""
         cmd = self._add_arguments(cmd, **kwargs)
 
         print(cmd)
-        ret = run(cmd, verbose=verbosity, return_output=return_output)
+        ret = run(cmd, verbose=verbosity).returncode
 
         if isinstance(ret, tuple) and ret[0] != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
@@ -882,29 +878,29 @@
     def minimum_slab_size(self, device_name, default_to_2g=True):  # reused from vdo.py
         """Computing minimum slab size, used from vdo.py."""
 
         class VDODeviceNotFoundError(Exception):
             pass
 
         print(device_name)
-        ret, device_size = run(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
+        ret, device_size = run_ret_out(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
         print(device_name, ret, device_size)
         if ret != 0:
             raise VDODeviceNotFoundError
 
         # ['└─myvg-vdotest', '252:2', '0', '4G', '0', 'lvm'][3] == '4G'
         size = device_size.split()[3]
         multipliers = ["M", "G", "T", "P", "E"]
 
         device_size = (float(size[:-1]) * (1024 ** multipliers.index(size[-1:]))).__int__()
         max_number_of_slabs = 8192
         minimum_size = max(2 ** int(device_size / max_number_of_slabs).bit_length(), 128)  # reused from vdo.py
         if default_to_2g and minimum_size < 2048:
             return "2G"
-        return f"{str(minimum_size)}M"
+        return f"{minimum_size!s}M"
 
     def check_conf_value(self, val):
         """Remove units K, G, T and convert accordingly."""
         if "fail" in self.tmp_kwargs["name"]:
             return val  # don't check
 
         units = {
@@ -1036,15 +1032,15 @@
         use_conf_file = False
 
         if use_conf_file:
             profile_name = "vdo_create"
             args_to_remove = self.create_profile_file(profile_name, args_to_remove, **kwargs)
             cmd += f"--metadataprofile {profile_name} "
             print_profile_file(profile_name)
-        elif self.number_of_conf_args(**kwargs) != 0:
+        elif self.number_of_conf_args(**kwargs).returncode != 0:
             cmd += "--config"
             # --config="    for condition == 1
             # --config '   else
             cmd += '="' if self.number_of_conf_args(**kwargs) == 1 else " '"
 
             for arg, value in kwargs.items():
                 if arg in self.config_arguments:  # do just what is necessary
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/md.py` & `sts_libs-0.0.4/sts_libs/src/sts/md.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 from pathlib import Path
 
 from sts.utils import sts_print
-from sts.utils.cmdline import exists, run
+from sts.utils.cmdline import exists, run_ret_out
 
 
 def _mdadm_query(md_device, verbose=False):
     if not exists("mdadm"):
         if verbose:
             sts_print("INFO: mdadm is not installed")
         return None
 
     cmd = f"mdadm -D /dev/{md_device}"
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print(f"FAIL: couldn't query {md_device}")
         if verbose:
             print(output)
         return None
     return output
 
@@ -37,15 +37,15 @@
 
     if not Path(mdstat_file).exists():
         if verbose:
             sts_print("INFO: there is no MD device")
         return False
 
     cmd = f"cat {mdstat_file}"
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         if verbose:
             sts_print("INFO: there is no MD device")
         return None
 
     md_name_regex = r"^(md\d+) :"
     md_devices = []
@@ -140,15 +140,15 @@
     verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     cmd = f"mdadm --stop /dev/{md_device}"
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print(f"FAIL: couldn't stop {md_device}")
         if verbose:
             print(output)
         return False
     return True
 
@@ -160,15 +160,15 @@
     verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     cmd = f"mdadm --zero-superblock {device}"
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if retcode != 0:
         sts_print(f"FAIL: couldn't clean {device}")
         if verbose:
             print(output)
         return False
     return True
 
@@ -185,15 +185,15 @@
     """
     sto_devices = md_get_storage_dev(md_device)
 
     if not md_stop(md_device):
         return False
 
     cmd = f"mdadm --remove /dev/{md_device}"
-    retcode, output = run(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
     if (
         retcode != 0
         and
         # error opening the device can be ignored
         f"mdadm: error opening /dev/{md_device}: No such file or directory" not in output
     ):
         sts_print(f"FAIL: couldn't remove {md_device}")
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/mp.py` & `sts_libs-0.0.4/sts_libs/src/sts/mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """mp.py: Module to manage multipath devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 from pathlib import Path
+from typing import Literal
 
 from sts import fc, iscsi, linux, lvm, net, scsi
 from sts.utils import sts_print
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 from sts.utils.size import size_human_2_size_bytes
 
 MULTIPATH_CONF_PATH = "/etc/multipath.conf"
 aug_conf_path = "/files/etc/multipath.conf"
 package_name = "device-mapper-multipath"
 
 
@@ -34,21 +35,20 @@
 
 
 def is_multipathd_running():
     """Check if multipathd is running."""
     return linux.is_service_running(mp_service_name())
 
 
-def mpathconf_enable(find_mpaths=False) -> bool:
+def mpathconf_enable(find_mpaths: Literal["yes", "no", "strict", "greedy", "smart", None] = None) -> bool:
     """Runs 'mpathconf --enable' command."""
     cmd = "mpathconf --enable"
     if find_mpaths:
-        cmd = cmd + " --find_multipaths n"
-    retcode = run(cmd)
-    if retcode != 0:
+        cmd = cmd + f" --find_multipaths {find_mpaths}"
+    if run(cmd).returncode != 0:
         return False
 
     return True
 
 
 def mp_enable() -> bool:
     """Installs and enable multipath."""
@@ -68,15 +68,15 @@
       mpath_name: name of device to check
       print_fail: Should we print "FAIL: ..." in case of fail?
 
     Returns:
       True / False.
     """
     cmd = f"multipath -l {mpath_name}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         if print_fail:
             sts_print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     # There could be error in the output, so we need to check if we really found the mpath device.
     # 'multipath -l device_name' always should return device_name at the beginning if found
@@ -91,37 +91,37 @@
     Disk:   Disk
     Returns:
     String: Return the name of multipath device.
     """
     if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
         device = f"/dev/{disk}"
         mmnum_cmd = 'ls -l %s | awk \'{print "("$5,$6")"}\'' % device
-        retcode, output = run(mmnum_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(mmnum_cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print(f"FAIL: Could not get device information for {device}")
             print(output)
             return None
         deps_cmd = rf"dmsetup deps | grep \"{output}\" | awk -v device={device} '{{print $1}}' | tr -d \"\:\""
-        retcode, output = run(deps_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(deps_cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print(f"FAIL: Could not get dmsetup information for {device}")
             print(output)
             return None
         mpath = output
     else:
         # BZ891921 - Multipath provides the mpath device of given scsi block device
         cmd = "pidof multipathd"
-        retcode, output = run(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print("FAIL: For some reason multipathd is not running")
             print(output)
             return None
         fmt = '"%d %m"'
         cmd = f"multipathd show paths format {fmt} | egrep \"^{disk}\" | awk '{{print$2}}'"
-        retcode, output = run(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
         if retcode != 0:
             sts_print(f"FAIL: to find multipath of disk {disk}")
             print(output)
             return None
         mpath = output
 
     if not mpath:
@@ -231,15 +231,15 @@
     # device, the kernel won't return an error on the path, and so you will
     # not see any errors until the next checker is run after you bring the
     # port down.
     cmd = "multipath -ll"
     if mpath_name:
         cmd += f" {mpath_name}"
     # cmd = "multipathd -k\"show top\""
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     if not output:
         # sts_print("FAIL: Got no output from \"%s\"" % cmd)
         return None
@@ -805,38 +805,35 @@
         undef
     Exceptions
         N/A.
     """
     cmd = "multipath -r"
     if mpath_name:
         cmd += f" {mpath_name}"
-    ret = run(cmd, verbose=True)
-    if ret != 0:
+    if run(cmd).returncode != 0:
         return False
 
     return True
 
 
 def remove_mpath(mpath_name):
     """Remove specific mpath."""
     if not mpath_name:
         sts_print("FAIL: remove_mpath() - requires mpath_name parameter")
         return False
-    retcode = run(f"multipath -f {mpath_name}")
-    if retcode != 0:
+    if run(f"multipath -f {mpath_name}").returncode != 0:
         sts_print(f"FAIL: Could not remove mpath {mpath_name}")
         return False
     return True
 
 
 def flush_all():
     """Flush all unused multipath device maps."""
     cmd = "multipath -F"
-    ret = run(cmd, verbose=True)
-    if ret != 0:
+    if run(cmd).returncode != 0:
         return False
 
     return True
 
 
 def multipath_backup_conf(bak_file):
     """backup_mp_conf ()
@@ -859,15 +856,15 @@
 
     if Path(bak_file).is_file():
         sts_print(f"FAIL: mpath backup file {bak_file} already exists")
         return False
 
     sts_print(f"INFO: Backing up {MULTIPATH_CONF_PATH} to {bak_file}")
     cmd = f"cp -f {MULTIPATH_CONF_PATH} {bak_file}"
-    ret, output = run(cmd, return_output=True)
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
         sts_print(f"FAIL: Could not backup {MULTIPATH_CONF_PATH}")
         print(output)
         return False
 
     return True
 
@@ -890,15 +887,15 @@
     """
     if not Path(bak_file).is_file():
         sts_print(f"FAIL: {bak_file} does not exist")
         return False
 
     sts_print(f"INFO: Restoring multipath configuration from {bak_file}")
     cmd = f"cp -f {bak_file} {MULTIPATH_CONF_PATH}"
-    ret, output = run(cmd, return_output=True)
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
         sts_print(f"FAIL: Could not restore backup from {bak_file}")
         print(output)
         return False
 
     multipath_reload_conf()
     return True
@@ -916,15 +913,15 @@
         1
             or
         undef
     Exceptions
         N/A.
     """
     cmd = "multipathd -k'reconfig'"
-    ret = run(cmd, verbose=True)
+    ret = run(cmd, verbose=True).returncode
 
     multipath_reload()
     if ret != 0:
         return False
 
     return True
 
@@ -980,15 +977,15 @@
 
     Raises:
       IOError: Augeas save fails. Check if multipath.conf changes are valid.
     """
     matched_path = mpath_conf_match(path, value)
 
     if matched_path:
-        _, out = run(f'augtool -s rm "{matched_path}"', return_output=True, verbose=False)
+        out = run(f'augtool -s rm "{matched_path}"', capture_output=True, verbose=False).output
         if "Saved 1 file(s)" not in out:
             sts_print(f"FAIL: unable to set {path} to {value}")
             return False
 
     return True
 
 
@@ -1008,15 +1005,15 @@
     if not linux.install_package("augeas", verbose=False):
         sts_print("FAIL: Could not install augeas")
         return None
 
     full_path = path if path.startswith(aug_conf_path) else aug_conf_path + path
 
     # successfully matches also when end of path is not unique - path[*] value, but not path[*]/path value
-    _, out = run(f'augtool match "{full_path}" "{value}"', return_output=True, verbose=False)
+    out = run(f'augtool match "{full_path}" "{value}"', capture_output=True, verbose=False).output
 
     # augtool prints path when matched, return codes seems useless
     if aug_conf_path in out:
         # returning path, as it can be useful when modifying non-unique paths
         return out
     return None
 
@@ -1043,15 +1040,15 @@
     path_to_match = re.sub(r"\[[^]]*]", "[.]", path)  # in case path expressions are being used
     matched_path = mpath_conf_match(path_to_match, value)
 
     if not matched_path:
         if not linux.is_installed("augeas"):
             sts_print("FAIL: Could not install augeas")
             return False
-        _, out = run(f'augtool -s set "{full_path}" "{value}"', return_output=True, verbose=False)
+        out = run(f'augtool -s set "{full_path}" "{value}"', capture_output=True, verbose=False).output
         if "Saved 1 file(s)" not in out:
             sts_print(f"FAIL: unable to set {path} to {value}. Try")
             return False
 
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/net.py` & `sts_libs-0.0.4/sts_libs/src/sts/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from os.path import lexists
 from pathlib import Path
 
 import netifaces
 
 from sts import linux
 from sts.utils import sts_print
-from sts.utils.cmdline import exists, run
+from sts.utils.cmdline import exists, run, run_ret_out
 
 __author__ = "Bruno Goncalves"
 __copyright__ = "Copyright (c) 2016 Red Hat, Inc. All rights reserved."
 
 sysfs_class_net_path = "/sys/class/net"
 
 
@@ -73,28 +73,28 @@
 
 
 def get_ip_address_of_nic(nic):
     """Get IPv4 of specific network interface."""
     try:
         ip = netifaces.ifaddresses(nic)[netifaces.AF_INET][0]["addr"]
     except KeyError as e:
-        print(f"KeyError - Iface probably does not have a IP address - {str(e)}")
+        print(f"KeyError - Iface probably does not have a IP address - {e!s}")
     except Exception as e:
         print(repr(e))
     else:
         return ip
     return None
 
 
 def get_ipv6_address_of_nic(nic):
     """Get IPv6 of specific network interface."""
     try:
         ip = netifaces.ifaddresses(nic)[netifaces.AF_INET6][0]["addr"]
     except KeyError as e:
-        print(f"KeyError - Iface probably does not have a IPv6 address - {str(e)}")
+        print(f"KeyError - Iface probably does not have a IPv6 address - {e!s}")
     except Exception as e:
         print(repr(e))
     else:
         return ip
     return None
 
 
@@ -317,15 +317,15 @@
     """
     if not nic_or_mac:
         sts_print("FAIL: iface_up() - requires nic or mac as argument")
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
-    retcode, output = run(f"ip link set {nic} up", return_output=True)
+    retcode, output = run_ret_out(f"ip link set {nic} up", return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
 def iface_down(nic_or_mac):
@@ -335,15 +335,15 @@
     """
     if not nic_or_mac:
         sts_print("FAIL: iface_down() - requires nic or mac as argument")
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
-    retcode, output = run(f"ip link set {nic} down", return_output=True)
+    retcode, output = run_ret_out(f"ip link set {nic} down", return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
 def set_ifcfg(nic_or_mac, parameters):
@@ -404,96 +404,96 @@
 
 
 def nm_get_conn_iface(conn):
     """Returns interface name used by NM connection
     conn: connection id or uuid.
     """
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get connection.interface-name for connection " + conn)
         print(output)
         return None
     return output
 
 
 def nm_get_conn_uuid(conn):
     """Returns NetworkManager connection UUID
     conn: connection id.
     """
     cmd = f"nmcli -g connection.uuid conn show '{conn}'"
     print(cmd)
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get NM connection uuid using " + conn)
         print(output)
         return None
     return output
 
 
 def nm_get_conn_from_dev(nic):
     """Returns connection id(name) using specified device.
     nic: network interface - device.
     """
     nic = str(nic)
     cmd = "nmcli -g GENERAL.CONNECTION device show " + nic
 
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get NM connection using device " + nic)
         print(output)
         return None
     return output
 
 
 def nm_get_dev_from_conn(conn):
     """Returns a device used by specified connection
     conn: networkmanager connection id(name) or uuid.
     """
     conn = str(conn)
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
 
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Couldn't get device used by NM connection " + conn)
         print(output)
         return None
     return output
 
 
 def nm_conn_up(conn):
     """Uses nmcli to activate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn up "{conn}"'
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to activate the connection: {conn}")
         return False
     print(output)
     return True
 
 
 def nm_conn_down(conn):
     """Uses nmcli to deactivate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn down "{conn}"'
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to deactivate the connection: {conn}")
         return False
     print(output)
     return True
 
 
 def nm_conn_reload():
     """Runs `nmcli conn reload`. Does not support RHEL6."""
     cmd = "nmcli conn reload"
-    retcode = run(cmd, verbose=False)
+    retcode = run(cmd, verbose=False).returncode
     if retcode != 0:
         print("FAIL: Unable to reload NetworkManager")
         return False
     return True
 
 
 def nm_conn_show(conn):
@@ -501,28 +501,28 @@
     conn: networkmanager connection id(name) or uuid.
     """
     if not conn:
         print("FAIL: No conn specified")
         return False
 
     cmd = f'nmcli conn show "{conn}"'
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print("FAIL: Unable to show conn")
         return False
     print(output)
     return True
 
 
 def nm_conn_del(conn):
     """Deletes NetworkManager connection using nmcli
     conn: connection id(name) or uuid.
     """
     cmd = f"nmcli conn delete {conn}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to delete the conn {conn}")
         return False
     print(output)
     return True
 
 
@@ -550,15 +550,15 @@
         return True
 
     cmd = f"nmcli conn add type {nic_type} con-name {name}"
     if nic:
         cmd += f" ifname {nic}"
     if "_" in cmd:
         cmd = cmd.replace("_", "-")
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to add con with cmd {cmd} ")
         print(output)
         return False
     nm_conn_reload()
     return True
 
@@ -585,15 +585,15 @@
     conn_uuid = nm_get_conn_uuid(conn)
     if not conn_uuid:
         return False
     cmd = f"nmcli conn modify {conn_uuid}"
 
     cmd += f" {key} {value}"
 
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to modify conn {conn} with cmd {cmd} ")
         print(output)
         return False
     return True
 
 
@@ -601,15 +601,15 @@
     """Modify one or more properties that are currently active on the device without modifying
     the connection profile. The changes have immediate effect.
     nmcli dev modify em1 ipv4.method shared
     nmcli dev modify em1 ipv4.address xx.
     """
     cmd = f"nmcli device modify {dev}"
     cmd += f" {key} {value}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to modify dev {dev} with cmd {cmd} ")
         print(output)
         return False
     return True
 
 
@@ -629,15 +629,15 @@
         print("FAIL: Invalid IP format")
         return False
 
     if "." in netmask:
         netmask = convert_netmask(netmask)
 
     cmd = f"nmcli conn modify {conn} {cmd_ip}.method manual {cmd_ip}.addr {ip}/{netmask}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Unable to set IP using nmcli: {conn} {ip}")
         print(output)
         return False
 
     if activate and not nm_conn_up(conn):
         return False
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.4/sts_libs/src/sts/qemu_img.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,16 +72,15 @@
     if fmt is not None:
         cmd += f"-f {fmt}"
     if fmt == "qcow2" and options:
         cmd += " -o "
         option = [str(i) + "=" + str(options[i]) for i in options if i in _QCOW_SUPPORTED_OPTIONS]
         cmd += ",".join(option)
     cmd += f" {filename} {size}"
-    ret = run(cmd)
-    if ret != 0:
+    if run(cmd).returncode != 0:
         sts_print("FAIL: Could not create disk image.")
         return False
     return True
 
 
 def delete_image(name, image_path="/var/tmp"):
     """Delete the disk image.
@@ -98,12 +97,11 @@
         sts_print("FAIL: delete_image() - requires name parameter")
         return False
 
     print(f"INFO: Deleting image device {name}")
     fname = _get_image_file(name, image_path)
     if Path(fname).is_file():
         cmd = f"rm -f {fname}"
-        retcode = run(cmd)
-        if retcode != 0:
+        if run(cmd).returncode != 0:
             sts_print(f"FAIL: Could not delete image disk file {fname}")
             return False
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.4/sts_libs/src/sts/scsi.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os.path
 import re
 from os import readlink
 from pathlib import Path
 
 from sts import linux, lvm, md, mp, net
 from sts.utils import size, sts_print
-from sts.utils.cmdline import exists, run
+from sts.utils.cmdline import exists, run, run_ret_out
 
 # I'm still note sure whether to use /sys/class/scsi_disk or /sys/class/scsi_device
 
 sys_disk_path = "/sys/class/scsi_disk"
 host_path = "/sys/class/scsi_host"
 
 # add /lib/udev to PATH because scsi_id is located there on RHEL7
@@ -35,51 +35,51 @@
     The arguments are:
     None
     Device name: eg. sda
     Returns:
     array: Return an array of SCSI IDs.
     """
     cmd = f"ls {sys_disk_path}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output.split()
 
 
 def get_scsi_disk_name(device_id):
     if not device_id:
         sts_print("FAIL: get_scsi_disk_name() requires scsi_device_id as parameter")
         return None
 
     cmd = f"ls {sys_disk_path}/{device_id}/device/block"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
 def get_scsi_disk_vendor(device_id):
     if not device_id:
         sts_print("FAIL: get_scsi_disk_vendor() requires scsi_device_id as parameter")
         return None
 
     cmd = f"cat {sys_disk_path}/{device_id}/device/vendor"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
 def get_scsi_disk_model(device_id):
     if not device_id:
         sts_print("FAIL: get_scsi_disk_model() requires scsi_device_id as parameter")
         return None
 
     cmd = f"cat {sys_disk_path}/{device_id}/device/model"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     return output
 
 
 def query_all_scsi_disks(scsi_disk=None):
     """Query information of all SCSI disks and return them as a dict
@@ -197,16 +197,15 @@
 
     device_id = scsi_name_2_scsi_id(device_name)
     if not device_id:
         sts_print(f"FAIL: delete_disk() could not find disk {device_name}")
         return None
 
     cmd = f'echo "1" >  {sys_disk_path}/{device_id}/device/delete'
-    retcode = run(cmd, verbose=False)
-    if retcode != 0:
+    if run(cmd, verbose=False).returncode != 0:
         return None
     return True
 
 
 def get_hosts(somethings=None):
     """Return a list with all SCSI hosts.
     The arguments are:
@@ -216,15 +215,15 @@
     or
     scsi_id       e.g. 3:0:0:1
     Returns:
     Host list     if no problem executing command
     None          if something went wrong.
     """
     cmd = f"ls {host_path}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         return None
     # remove 'host' prefix
     output = re.sub("host", "", output)
     all_host_ids = output.split()
     if not somethings:
         return all_host_ids
@@ -287,15 +286,15 @@
         "scsi_host_id": host_id,
         "pci_id": pci_id_of_host_id(host_id),
         "driver": scsi_driver_of_host_id(host_id),
     }
 
     param_files = list(sysfs_folder.iterdir())
     for param in param_files:
-        ret, output = run(f"cat {sysfs_folder}/{param}", return_output=True, verbose=False)
+        ret, output = run_ret_out(f"cat {sysfs_folder}/{param}", return_output=True, verbose=False)
         if ret != 0:
             # For some reason could not read the file
             continue
         scsi_host_info[param] = ", ".join(output.split("\n"))
 
     sysfs_hosts = [
         f"/sys/class/iscsi_host/host{host_id}",
@@ -303,15 +302,15 @@
     ]
     for sysfs_host in sysfs_hosts:
         path = Path(sysfs_host)
         if not path.is_dir():
             continue
         host_files = list(path.iterdir())
         for param in host_files:
-            ret, output = run(f"cat {sysfs_host}/{param}", return_output=True, verbose=False)
+            ret, output = run_ret_out(f"cat {sysfs_host}/{param}", return_output=True, verbose=False)
             if ret != 0:
                 # For some reason could not read the file
                 continue
             scsi_host_info[param] = ", ".join(output.split("\n"))
 
     return scsi_host_info
 
@@ -321,60 +320,60 @@
         sts_print("FAIL: scsi_driver_of_host_id() - requires host_id parameter")
         return None
     scsi_drv_sysfs = f"/sys/class/scsi_host/host{host_id}/proc_name"
     if not Path(scsi_drv_sysfs).is_file():
         sts_print(f"FAIL: {scsi_drv_sysfs} is not a valid path")
         return None
 
-    _, output = run(f"cat {scsi_drv_sysfs}", return_output=True, verbose=False)
+    output = run(f"cat {scsi_drv_sysfs}", capture_output=True, verbose=False).output
     scsi_driver = output
     if scsi_driver == "(null)" or scsi_driver == "":
         # Driver information was not exported, let try to find it out some other way
         lpfc_sysfs_file = f"/sys/class/scsi_host/host{host_id}/lpfc_drvr_version"
         if Path(lpfc_sysfs_file).is_file():
             return "lpfc"
 
         driver_sysfs_file = f"/sys/class/scsi_host/host{host_id}/driver_name"
         if Path(driver_sysfs_file).is_file():
-            _, output = run(f"cat {driver_sysfs_file}", return_output=True, verbose=False)
+            output = run(f"cat {driver_sysfs_file}", capture_output=True, verbose=False).output
             return output
 
         model_sysfs_file = f"/sys/class/scsi_host/host{host_id}/model_name"
         if Path(model_sysfs_file).is_file():
-            _, output = run(f"cat {model_sysfs_file}", return_output=True, verbose=False)
+            output = run(f"cat {model_sysfs_file}", capture_output=True, verbose=False).output
             if re.match("^QLE", output):
                 return "qla2xxx"
 
         symbolic_sysfs_file = f"/sys/class/fc_host/host{host_id}/symbolic_name"
         if Path(symbolic_sysfs_file).is_file():
-            _, output = run(f"cat {symbolic_sysfs_file}", return_output=True, verbose=False)
+            output = run(f"cat {symbolic_sysfs_file}", capture_output=True, verbose=False).output
             if re.search("bnx2fc", output):
                 return "bnx2fc"
 
         pci_id = pci_id_of_host_id(host_id)
         if pci_id:
             lspci_regex = r"Kernel modules:\s+(\S+)"
             if not exists("lspci"):
                 sts_print("FAIL: pciutils is not installed. Can't query driver name using pci_id.")
                 return None
-            _, output = run(
+            output = run(
                 f'lspci -s "{pci_id}" -v | grep "Kernel modules:"',
-                return_output=True,
+                capture_output=True,
                 verbose=False,
-            )
+            ).output
             if output:
                 m = re.search(lspci_regex, output)
                 if m:
                     return m.group(1)
 
         sts_print(f"FAIL: Could not get driver name for SCSI host{host_id}")
         return None
     if scsi_driver == "fcoe":
         drv_version_path = f"/sys/class/fc_host/host{host_id}/driver_version"
-        _, output = run(f"cat {drv_version_path}", return_output=True, verbose=False)
+        output = run(f"cat {drv_version_path}", capture_output=True, verbose=False).output
         if re.search("ixgbe", output):
             return "ixgbe"
     return scsi_driver
 
 
 def pci_id_of_host_id(host_id):
     """Usage
@@ -436,16 +435,15 @@
         sts_print("WARN: No host found on server to rescan")
         return True
 
     for host in host_list:
         if verbose:
             sts_print(f"INFO: Rescanning host{host}")
         cmd = f'echo "- - -" > {host_path}/host{host}/scan'
-        retcode, _ = run(cmd, return_output=True, verbose=verbose)
-        if retcode != 0:
+        if run(cmd, verbose=verbose).returncode != 0:
             error += 1
             sts_print(f"FAIL: there was some problem scanning host{host}")
 
     if error:
         return False
 
     return True
@@ -468,16 +466,15 @@
         ids = get_scsi_disk_ids()
         for _id in ids:
             scsi_disks.append(get_scsi_disk_name(_id))
 
     error = 0
     for scsi_disk in scsi_disks:
         cmd = f"echo 1 > /sys/block/{scsi_disk}/device/rescan"
-        retcode, _ = run(cmd, return_output=True)
-        if retcode != 0:
+        if run(cmd).returncode != 0:
             sts_print(f"FAIL: Could not rescan {scsi_disk}")
             error += 1
 
     if error:
         return False
 
     return True
@@ -494,25 +491,25 @@
         size in bytes.
 
     """
     if not scsi_disk:
         return None
 
     cmd = f"cat /sys/block/{scsi_disk}/queue/logical_block_size"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: size_of_disk() - Could not get size for disk {scsi_disk}")
         print(output)
         return None
     if not output:
         return None
     logical_block_size = output
 
     cmd = f"cat /sys/block/{scsi_disk}/size"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: size_of_disk() - Could not get sectore size for disk {scsi_disk}")
         print(output)
         return None
     if not output:
         return None
 
@@ -551,24 +548,22 @@
     Returns
         scsi_ids.
     """
     if not wwid:
         sts_print("FAIL: scsi_ids_of_wwid(): Got NULL input for WWID")
         return None
 
-    scsi_ids = None
+    scsi_ids = []
     all_scsi_info = query_all_scsi_disks()
     if not all_scsi_info:
         # Could not find any SCSI device
         return None
 
     for _id in list(all_scsi_info.keys()):
         if all_scsi_info[_id]["wwid"] == wwid:
-            if not scsi_ids:
-                scsi_ids = []
             scsi_ids.append(_id)
     if scsi_ids:
         scsi_ids = list(set(scsi_ids))  # dedup
     return scsi_ids
 
 
 def wwn_of_disk(scsi_disk):
@@ -584,30 +579,30 @@
     if not scsi_disk:
         sts_print("FAIL: wwn_of_disk() - requires scsi_disk parameter")
         return None
 
     key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
 
     # cmd = "udevadm info --name=%s --query=all" % scsi_disk
-    # retcode, output = run(cmd, return_output=True, verbose=False)
+    # retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     # if (retcode != 0):
     # #sts_print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
     # #print output
 
     # return None
 
     # udev_wwn = None
     # lines = output.split("\n")
     # for line in lines:
     # m = re.search(key_regex, line)
     # if m:
     # udev_wwn = m.group(1)
 
     cmd = f"scsi_id --whitelisted --export /dev/{scsi_disk}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         # sts_print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
     lines = output.split("\n")
     for line in lines:
@@ -640,15 +635,15 @@
     if not scsi_disk:
         sts_print("FAIL: udev_wwn_of_disk() - requires scsi_disk parameter")
         return None
 
     key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
 
     cmd = f"udevadm info --name={scsi_disk} --query=all"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         # sts_print("FAIL: udev_wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
     lines = output.split("\n")
     for line in lines:
@@ -826,15 +821,15 @@
 
     if action == "UP":
         action = "running"
     if action == "DOWN":
         action = "offline"
 
     cmd = f"echo {action} > {sys_path}"
-    retcode, output = run(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         sts_print(f"FAIL: disk_sys_trigger() - Could not execute {cmd}")
         print(output)
         return None
 
     # cmd = "cat %s 2>/dev/null" % sys_path
     new_state = disk_sys_check(scsi_disk)
@@ -868,15 +863,15 @@
 
     sys_path = f"/sys/block/{scsi_disk}/device/state"
     if not Path(sys_path).is_file():
         sts_print(f"FAIL: disk_sys_check() - No such file: {sys_path}")
         return None
 
     cmd = f"cat {sys_path} 2>/dev/null"
-    _, state = run(cmd, return_output=True, verbose=False)
+    state = run(cmd, capture_output=True, verbose=False).output
     if not state:
         sts_print(f"FAIL: disk_sys_check() - Could not read from {sys_path}")
         return None
 
     return state
 
 
@@ -899,13 +894,13 @@
 
     sys_path = f"/sys/block/{scsi_disk}/device/timeout"
     if not Path(sys_path).is_file():
         sts_print(f"FAIL: timeout_of_disk() - No such file: {sys_path}")
         return None
 
     cmd = f"cat {sys_path} 2>/dev/null"
-    _, timeout = run(cmd, return_output=True, verbose=False)
+    timeout = run(cmd, capture_output=True, verbose=False).output
     if not timeout:
         sts_print(f"FAIL: timeout_of_disk() - Could not read from {sys_path}")
         return None
 
     return timeout
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.4/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.4/sts_libs/src/sts/stratis.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,26 +49,26 @@
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
     def _remove_nones(kwargs):
         return {k: v for k, v in kwargs.items() if v is not None}
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):
+    def _run(self, cmd, verbosity=True, **kwargs):
         # Constructs the command to run and runs it
 
         # add '--propagate' flag by default to show whole trace when getting errors
         # This is a suggestion from devs
         if not ("propagate" in kwargs and not kwargs["propagate"]):
             cmd = self.arguments["propagate"][1] + cmd
 
         cmd = "stratis " + cmd
         cmd = self._add_arguments(cmd, **kwargs)
 
-        ret = run(cmd, verbose=verbosity, return_output=return_output)
+        ret = run(cmd, verbose=verbosity).returncode
         if isinstance(ret, tuple) and ret[0] != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     def set_stratis_version(self, version):
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.4/sts_libs/src/sts/vdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sts.utils.atomic_run import atomic_run
 from sts.utils.cli_tools import (
     FailedCheckExceptionError,
     Wrapper,
     WrongArgumentExceptionError,
     WrongCommandExceptionError,
 )
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 
 def restart_modify(vdo_object, vdo_name, errors):
     # sometimes VDO needs to be restarted for changes to take effect
     print("Restarting VDO for changes to take effect.")
     commands = [
         {
@@ -51,22 +51,22 @@
         print(error)
         errors.append(error)
 
 
 def minimum_slab_size(device, default_to_2g=True):
     def _get_raid_device(device):
         device_name = device.split("/").pop()
-        ret, device_link = run(cmd=f"ls -al /dev/md | grep {device_name}", return_output=True)
+        ret, device_link = run_ret_out(cmd=f"ls -al /dev/md | grep {device_name}", return_output=True)
         if ret or device_link is None:
             print(f"WARN: Device {device_name} not found in /dev/md.")
             return None
         return device_link.split("../").pop()  # raid device
 
     device_name = _get_raid_device(device) if device.startswith("/dev/md") else device.split("/").pop()
-    ret, device_size = run(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
+    ret, device_size = run_ret_out(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
     if ret or device_size is None:
         print(f"WARN: Device {device_name} not found using lsblk. Using default 2G size.")
         return "2G"
     size = device_size.split()[3]
     multipliers = ["M", "G", "T", "P", "E"]
     device_size = (float(size[:-1]) * (1024 ** multipliers.index(size[-1:]))).__int__()
     max_number_of_slabs = 8192
@@ -141,15 +141,15 @@
                 correct_vdo_device = True
             if correct_vdo_device and "device:" in line:
                 # Now we have the device, just need to follow the link
                 device = line.split("device:").pop().strip()
                 break
 
     # now we might have /dev/disk/by-id/UUID, need to get something reasonable
-    _, data = run(f"ls -la {device}", return_output=True, verbose=False)
+    data = run(f"ls -la {device}", capture_output=True, verbose=False).output
     device = data.split("/").pop().strip()
 
     # format dm-X causes issues later on, where the device cannot be found using lsblk to check for size
     if device.startswith("dm-"):
         with Path(f"/sys/block/{device}/dm/name").open() as f:
             dev_name = f.readline().rstrip("\n")
         device = f"/dev/mapper/{dev_name}"
@@ -417,19 +417,19 @@
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
             sts_print(f"WARN: Failed checking on argument {e.argument}")
             return ret_fail
 
         if return_output:
-            ret, data = run(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
             if ret != 0:
                 sts_print(f"WARN: Running command: '{cmd}' failed. Return with output.")
             return ret, data
-        ret = run(cmd, verbose=verbosity)
+        ret = run(cmd, verbose=verbosity).returncode
         if ret != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
     def help():  # noqa: A003
         if run("vdo --help", verbose=True) != 0:
@@ -562,15 +562,15 @@
         if cmd is None:
             return False
 
         if not self._check(cmd):
             # Requested command did not pass checking, reason was already written by _check()
             return False
 
-        if run(cmd, verbose=True) != 0:
+        if run(cmd, verbose=True).returncode != 0:
             sts_print(f"WARN: Running command: '{cmd}' failed.")
             return False
         return True
 
     def help(self):  # noqa: A003
         if not self._run(help=True):
             return False
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/__init__.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/atomic_run.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/atomic_run.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/beaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import os
 import re  # regex
 
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 from sts.utils.restraint import is_restraint_job, log_submit
 
 
 def sts_print(string):
     module_name = __name__
     string = re.sub("DEBUG:", "DEBUG:(" + module_name + ") ", string)
     string = re.sub("FAIL:", "FAIL:(" + module_name + ") ", string)
@@ -34,15 +34,15 @@
         return None
 
     if task_id is None:
         sts_print("FAIL: beaker get_task_timeout() - requires task_id as parameter")
         return None
 
     cmd = f"bkr watchdog-show {task_id}"
-    ret, output = run(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
         sts_print("FAIL: beaker get_task_timeout() - Could not get beaker kill time")
         print(output)
         return None
 
     output_regex = re.compile(r"%s: (\d+)" % task_id)
     m = output_regex.match(output)
@@ -59,15 +59,15 @@
         return None
 
     if not task_id:
         sts_print("FAIL: get_task_status() - requires task id")
         return None
 
     cmd = f"bkr job-results --prettyxml T:{task_id}"
-    ret, output = run(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
         sts_print(f"FAIL: get_task_status() - Could not get beaker task result for T:{task_id}")
         print(output)
         return None
 
     lines = output.split("\n")
     status_regex = re.compile(r"<task.*status=\"(\S+)\"")
@@ -91,15 +91,15 @@
 
     lab_controller = os.environ["LAB_CONTROLLER"]
     recipe_id = os.environ["BEAKER_RECIPE_ID"]
 
     # get current console log
     url = f"http://{lab_controller}:8000/recipes/{recipe_id}/logs/console.log"
 
-    if run(f"wget -q {url} -O {new_console_log_file}") != 0:
+    if run(f"curl -s {url} -O {new_console_log_file}") != 0:
         print("INFO: Could not get console log")
         # return success when could not get console.log
         return True
 
     # if there was previous console log, we just check the new part
     run(
         f"diff -N -n --unidirectional-new-file {prev_console_log_file} {new_console_log_file} > {console_log_file}",
@@ -108,15 +108,15 @@
     # backup the current full console.log
     # next time we run the test we will compare just
     # what has been appended to console.log
     run(f"mv -f {new_console_log_file} {prev_console_log_file}")
 
     print(f"INFO: Checking for errors on {console_log_file}")
     for msg in error_mgs:
-        _, output = run(f"cat {console_log_file} | grep -i '{msg}'", return_output=True)
+        output = run(f"cat {console_log_file} | grep -i '{msg}'", capture_output=True).output
         if output:
             print(f"INFO found {msg} on {console_log_file}")
             log_submit(console_log_file)
             error = +1
 
     if error:
         return False
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/logchecker.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 from datetime import datetime
 from os import getenv
 from pathlib import Path
 
 import sts.linux
 from sts.utils import beaker, restraint
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 
 segfault_msg = " segfault "
 calltrace_msg = "Call Trace:"
 
 error_mgs = [segfault_msg, calltrace_msg]
 
 tmt_test_data = getenv("TMT_TEST_DATA")
@@ -22,15 +22,15 @@
 
 
 def journalctl_timestamp() -> str:
     """Returns current time in journalctl-compatible format.
 
     Usage example:
         logging_start = journalctl_timestamp()
-        _, failure_logs = run(f"journalctl -S {logging_start}, return_output=True"
+        failure_logs = run(f"journalctl -S {logging_start}, capture_output=True).output"
     """
     return datetime.now().isoformat(sep=" ", timespec="minutes")  # noqa: DTZ005 <- We want local timezone.
 
 
 def check_all():
     """Check for error on the system
     Returns:
@@ -86,15 +86,15 @@
         print("WARN: skipping abrt check")
         return True
 
     if run("pidof abrtd", verbose=False) != 0:
         print("FAIL: abrtd is not running")
         return False
 
-    ret, log = run("abrt-cli list", return_output=True)
+    ret, log = run_ret_out("abrt-cli list", return_output=True)
     if ret != 0:
         print("FAIL: abrt-cli command failed")
         return False
 
     # We try to match for "Directory" to check if
     # abrt-cli list is actually listing any issue
     error = False
@@ -135,26 +135,26 @@
     True if did not find any issue
     False if found some issue.
     """
     print("INFO: Checking for tainted kernel")
 
     previous_tainted_file = "/tmp/previous-tainted"
 
-    _, tainted = run("cat /proc/sys/kernel/tainted", return_output=True)
+    tainted = run("cat /proc/sys/kernel/tainted", capture_output=True).output
 
     tainted_val = int(tainted)
     if tainted_val == 0:
         run("echo %d > %s" % (tainted_val, previous_tainted_file), verbose=False)
         return True
 
     print("WARN: Kernel is tainted!")
 
     if not Path(previous_tainted_file).is_file():
         run(f"echo {tainted_val} > {previous_tainted_file}", verbose=False)
-    _, prev_taint = run(f"cat {previous_tainted_file}", return_output=True)
+    prev_taint = run(f"cat {previous_tainted_file}", capture_output=True).output
     prev_taint_val = int(prev_taint)
     if prev_taint_val == tainted_val:
         print("INFO: Kernel tainted has already been handled")
         return True
 
     run("echo %d > %s" % (tainted_val, previous_tainted_file), verbose=False)
 
@@ -170,15 +170,15 @@
         tainted_val /= 2
     # List all tainted bits that are defined
     print("List bit definition for tainted kernel")
     run("cat /usr/src/kernels/`uname -r`/include/linux/kernel.h | grep TAINT_")
 
     found_issue = False
     # try to find the module which tainted the kernel, tainted module have a mark between '('')'
-    _, output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1", return_output=True)
+    output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1", capture_output=True).output
     tainted_mods = output.split("\n")
     # For example during iscsi async_events scst tool loads an unsigned module
     # just ignores it, so we will ignore this tainted if there is no tainted
     # modules loaded
     if not tainted_mods:
         print("INFO: ignoring tainted as the module is not loaded anymore")
     else:
@@ -257,15 +257,15 @@
 
     if not Path(previous_time_file).is_file():
         first_time = "Jan 01 00:00:00"
         time = _date2num(first_time)
         run(f"echo {time} > {previous_time_file}")
 
     # Read the last time test ran
-    _, last_run = run(f"cat {previous_time_file}", return_output=True)
+    last_run = run(f"cat {previous_time_file}", capture_output=True).output
     print(f"INFO: Checking for stack dump messages after: {last_run}")
 
     # Going to search the file for text that matches begin_tag until end_tag
     dump_regex = begin_tag + "(.*?)" + end_tag
     m = re.findall(dump_regex, log, re.MULTILINE)
     if m:
         print(f"INFO: Checking if it is newer than: {last_run}")
@@ -277,15 +277,15 @@
 
 
 def dmesg_check():
     """Check for error messages on dmesg ("Call Trace and segfault")."""
     print("INFO: Checking for errors on dmesg.")
     error = 0
     for msg in error_mgs:
-        _, output = run(f"dmesg | grep -i '{msg}'", return_output=True)
+        output = run(f"dmesg | grep -i '{msg}'", capture_output=True).output
         if output:
             print(f"FAIL: found {msg} on dmesg")
             run(f"echo '\nINFO found {msg}  Saving it\n'>> dmesg.log")
             run(f"dmesg >> {LOG_PATH}dmesg.log")
             restraint.log_submit("dmesg.log")
             error = 1
     sts.linux.clear_dmesg()
@@ -308,21 +308,21 @@
     """Check for kdump error messages.
     It assumes kdump is configured on /var/crash.
     """
     error = 0
 
     previous_kdump_check_file = "/tmp/previous-kdump-check"
     kdump_dir = "/var/crash"
-    ret, hostname = run("hostname", verbose=False, return_output=True)
+    ret, hostname = run_ret_out("hostname", verbose=False, return_output=True)
 
     if not Path(f"{kdump_dir}/{hostname}").exists():
         print("INFO: No kdump log found for this server")
         return True
 
-    ret, output = run(f"ls -l {kdump_dir}/{hostname} |  awk '{{print$9}}'", return_output=True)
+    ret, output = run_ret_out(f"ls -l {kdump_dir}/{hostname} |  awk '{{print$9}}'", return_output=True)
     kdumps = output.split("\n")
     kdump_dates = []
     for kdump in kdumps:
         if kdump == "":
             continue
         # parse on the date, remove the ip of the uploader
         m = re.match(".*?-(.*)", kdump)
@@ -337,41 +337,41 @@
         date = date[:index] + " " + date[index + 1 :]
         print(f"INFO: Found kdump from {date}")
         kdump_dates.append(date)
 
     # checks if a file to store last run exists, if not create it
     if not Path(f"{previous_kdump_check_file}").is_file():
         # time in seconds
-        ret, time = run(r"date +\"\%s\"", verbose=False, return_output=True)
+        ret, time = run_ret_out(r"date +\"\%s\"", verbose=False, return_output=True)
         run(f"echo -n {time} > {previous_kdump_check_file}", verbose=False)
         print("INFO: kdump check is executing for the first time.")
         print("INFO: doesn't know from which date should check files.")
         print("PASS: Returning success.")
         return True
 
     # Read the last time test ran
-    ret, previous_check_time = run(f"cat {previous_kdump_check_file}", return_output=True)
+    ret, previous_check_time = run_ret_out(f"cat {previous_kdump_check_file}", return_output=True)
     # just add new line to terminal because the file should not have already new line character
     print("")
 
     for date in kdump_dates:
         # Note %% is escape form to use % in a string
-        ret, kdump_time = run('date --date="%s" +%%s' % date, return_output=True)
+        ret, kdump_time = run_ret_out('date --date="%s" +%%s' % date, return_output=True)
         if ret != 0:
             print(f"WARN: Could not convert date {date}")
             continue
 
         if not kdump_time:
             continue
         if int(kdump_time) > int(previous_check_time):
             print(f"FAIL: Found a kdump log from {date} (more recent than {previous_check_time})")
             print(f"FAIL: Check {kdump_dir}/{hostname}")
             error += 1
 
-    ret, time = run(r"date +\"\%s\"", verbose=False, return_output=True)
+    ret, time = run_ret_out(r"date +\"\%s\"", verbose=False, return_output=True)
     run(f"echo -n {time} > {previous_kdump_check_file}", verbose=False)
 
     if error:
         return False
 
     print("PASS: No errors on kdump have been found.")
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,10 +287,10 @@
 
     Returns:
       list.: List of persistent vars file names having the specified prefix
     """
     if exists_persistent_vars_file():
         variables = read_var(get_persistent_vars_file_name())
     else:
-        _, variables = run(f"ls -la {get_persistent_files_dir()}", return_output=True, verbose=False)
+        variables = run(f"ls -la {get_persistent_files_dir()}", capture_output=True, verbose=False).output
         variables = [line.split().pop() for line in variables.splitlines()[3:]]
     return [value for value in variables if value.startswith(prefix)]
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/restraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import os
 import re
 from pathlib import Path
 
 from sts import linux
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run_ret_out
 
 
 def sts_print(string):
     module_name = __name__
     string = re.sub("DEBUG:", "DEBUG:(" + module_name + ") ", string)
     string = re.sub("FAIL:", "FAIL:(" + module_name + ") ", string)
     string = re.sub("FATAL:", "FATAL:(" + module_name + ") ", string)
@@ -47,15 +47,15 @@
         result_server,
         host,
         jobid,
         test,
         kill_time,
         testid,
     )
-    ret, output = run(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
         sts_print("FAIL: Could not update beaker kill time")
         print(output)
         return False
     sts_print("INFO: beaker_update_killtime() - Watchdog timer successfully updated to %d hours" % kill_time)
     return True
 
@@ -70,15 +70,15 @@
         return False
 
     if not Path(log_file).exists():
         sts_print(f"FAIL: log_submit() - file ({log_file}) does not exist")
         return False
 
     cmd = f'rhts-submit-log -l "{log_file}"'
-    ret, output = run(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
     if ret != 0:
         sts_print(f"FAIL: Could not upload log {log_file}")
         print(output)
         return False
     sts_print(f"INFO: log_submit() - {log_file} uploaded successfully")
     return True
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/tc.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/tc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
 import sys
 from pathlib import Path
 
 from sts import linux, mp
-from sts.utils.cmdline import run
+from sts.utils.cmdline import run, run_ret_out
 from sts.utils.logchecker import check_all
 from sts.utils.restraint import is_restraint_job, log_submit
 
 
 def show_sys_info():
     print("### Kernel Info: ###")
-    _, kernel = run("uname -a", return_output=True, verbose=False)
-    _, taint_val = run("cat /proc/sys/kernel/tainted", return_output=True, verbose=False)
+    kernel = run("uname -a", capture_output=True, verbose=False).output
+    taint_val = run("cat /proc/sys/kernel/tainted", capture_output=True, verbose=False).output
     print(f"Kernel version: {kernel}")
     print(f"Kernel tainted: {taint_val}")
     print("### IP settings: ###")
     run("ip a")
     print("### File system disk space usage: ###")
     run("df -h")
 
@@ -119,17 +119,17 @@
         Boolean: return_code
         True: If command excuted successfully
         False: Something went wrong
         str: command output (optional).
         """
         output = None
         if not return_output:
-            cmd_code = run(cmd)
+            cmd_code = run(cmd).returncode
         else:
-            cmd_code, output = run(cmd, return_output)
+            cmd_code, output = run_ret_out(cmd, return_output)
 
         if cmd_code == 0:
             self.tpass(cmd)
             ret_code = True
         else:
             self.tfail(cmd)
             ret_code = False
@@ -148,17 +148,17 @@
         Boolean: return_code
         False: If command executed successfully
         True: Something went wrong
         str: command output (optional).
         """
         output = None
         if not return_output:
-            cmd_code = run(cmd)
+            cmd_code = run(cmd).returncode
         else:
-            cmd_code, output = run(cmd, return_output)
+            cmd_code, output = run_ret_out(cmd, return_output)
 
         if cmd_code != 0:
             self.tpass(cmd + " [exited with error, as expected]")
             ret_code = True
         else:
             self.tfail(cmd + " [expected to fail, but it did not]")
             ret_code = False
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.4/sts_libs/src/sts/utils/tmt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 """Test Management Tool related things."""
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import json
+import tarfile
 import time
 from os import getenv
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from typing_extensions import TypedDict
 
 test_data_path = getenv("TMT_TEST_DATA")
 if not test_data_path:
     from uuid import uuid4
 
     dir_name = str(uuid4())
     print(f"WARN: TMT_TEST_DATA env var not detected. Using '/var/tmp/{dir_name}'")
     test_data_path = dir_name
 
 TMT_TEST_DATA = Path(test_data_path)
 
 
+def gather_logs_from_dir(logs_path: str, name: Optional[str]) -> Union[Path, None]:
+    path = Path(logs_path)
+    if not path.is_dir():
+        return None
+    if not name:
+        name = str(path).replace("/", "_")
+    if ".tar" not in name:
+        name = f"{name}.tar"
+
+    tarfile_path = f"{TMT_TEST_DATA}/{name}"
+    with tarfile.open(tarfile_path, "w") as tar:
+        tar.add(path, recursive=True)
+    return Path(tarfile_path)
+
+
 def timestamp() -> float:
     return time.time()
 
 
 def calculate_duration(start: float, end: float) -> str:
     """Returns hh:mm:ss duration."""
     secs = int(end - start)
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/fio_test.py` & `sts_libs-0.0.4/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.4/sts_libs/tests/iscsi_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def test_install_initiator():
     if not iscsi.install():
         pytest.fail("FAIL: Could not install iSCSI initiator package")
     assert 1
 
 
-@patch("sts.iscsi.run")
+@patch("sts.iscsi.run_ret_out")
 def test_query_discovery(iscsi_run_func):
     discovery_output = """
 SENDTARGETS:
 DiscoveryAddress: localhost,3260
 Target: iqn.2009-10.com.redhat:storage-0
     Portal: [::1]:3260,1
         Iface Name: default
@@ -47,20 +47,18 @@
                 },
             },
         },
         "iSNS": {},
         "STATIC": {},
         "FIRMWARE": {},
     }
-    if iscsi.query_discovery() != expected_ret:
-        pytest.fail("FAIL: Could not  query discovery iSCSI target")
-    assert 1
+    assert iscsi.query_discovery() == expected_ret
 
 
-@patch("sts.iscsi.run")
+@patch("sts.iscsi.run_ret_out")
 def test_discovery(iscsi_run_func):
     discovery_output = "[::1]:3260,1 iqn.2009-10.com.redhat:storage-0"
     iscsi_run_func.return_value = (0, discovery_output)
 
     if not iscsi.discovery_st(target):
         pytest.fail("FAIL: Could not discovery iSCSI target")
     assert 1
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/linux_test.py` & `sts_libs-0.0.4/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.4/sts_libs/tests/logchecker_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,43 +29,46 @@
 
     return 0, ""
 
 
 class Testlogchecker(unittest.TestCase):
     @patch("sts.utils.logchecker.run")
     def test_kernel_check(self, run_func):
-        run_func.return_value = (0, 0)
+        run_func.return_value.returncode = 0
+        run_func.return_value.output = "0"
         assert log_checker.kernel_check() is True
         # already handled taint
-        run_func.return_value = (0, 1)
+        run_func.return_value.returncode = 0
+        run_func.return_value.output = "1"
         assert log_checker.kernel_check() is True
 
     @patch("sts.utils.logchecker.run")
     def test_dmesg_check(self, run_func):
-        run_func.return_value = (0, "")
+        run_func.return_value.returncode = 0
+        run_func.return_value.output = ""
         assert log_checker.dmesg_check() is True
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_segfault
         assert log_checker.dmesg_check() is False
         run_calls = [
-            call("dmesg | grep -i ' segfault '", return_output=True),
+            call("dmesg | grep -i ' segfault '", capture_output=True),
             call("echo '\nINFO found  segfault   Saving it\n'>> dmesg.log"),
             call("dmesg >> ./dmesg.log"),
-            call("dmesg | grep -i 'Call Trace:'", return_output=True),
+            call("dmesg | grep -i 'Call Trace:'", capture_output=True),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_calltrace
         assert log_checker.dmesg_check() is False
         run_calls = [
-            call("dmesg | grep -i ' segfault '", return_output=True),
-            call("dmesg | grep -i 'Call Trace:'", return_output=True),
+            call("dmesg | grep -i ' segfault '", capture_output=True),
+            call("dmesg | grep -i 'Call Trace:'", capture_output=True),
             call("echo '\nINFO found Call Trace:  Saving it\n'>> dmesg.log"),
             call("dmesg >> ./dmesg.log"),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.4/sts_libs/tests/lvm_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,34 +16,34 @@
             "attr": "a--",
             "psize": "98.41g",
             "pfree": "0",
         },
     }
 
     def test_pv_query(self):
-        with patch("sts.lvm.run") as run_func:
+        with patch("sts.lvm.run_ret_out") as run_func:
             run_func.return_value = [0, self.pvs_output]
             assert self.pv_query_output == lvm.pv_query()
 
     def test_pv_create(self):
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 0
+            run_func.return_value.returncode = 0
             assert lvm.pv_create("/dev/vda1")
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 1
+            run_func.return_value.returncode = 1
             assert not lvm.pv_create("/dev/vda1")
 
     @patch("sts.lvm.pv_query")
     def test_pv_remove(self, mock):
         mock.return_value = self.pv_query_output
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 0
+            run_func.return_value.returncode = 0
             assert lvm.pv_remove("/dev/vda1")
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 1
+            run_func.return_value.returncode = 1
             assert not lvm.pv_remove("/dev/vda1")
 
 
 class TestVG(unittest.TestCase):
     vgs_output = "  lvm_test,1,3,0,wz--n-,98.41g,0"
     vg_query_output = {
         "lvm_test": {
@@ -53,28 +53,28 @@
             "attr": "wz--n-",
             "vsize": "98.41g",
             "vfree": "0",
         },
     }
 
     def test_vg_query(self):
-        with patch("sts.lvm.run") as run_func:
+        with patch("sts.lvm.run_ret_out") as run_func:
             run_func.return_value = [0, self.vgs_output]
             assert self.vg_query_output == lvm.vg_query()
 
     def test_pv_create(self):
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 0
+            run_func.return_value.returncode = 0
             assert lvm.vg_create("lvm_test", "/dev/vda1")
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 1
+            run_func.return_value.returncode = 1
             assert not lvm.vg_create("lvm_test", "/dev/vda1")
 
     @patch("sts.lvm.pv_query")
     def test_pv_remove(self, mock):
         mock.return_value = self.vg_query_output
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 0
+            run_func.return_value.returncode = 0
             assert lvm.pv_remove("lvm_test")
         with patch("sts.lvm.run") as run_func:
-            run_func.return_value = 1
+            run_func.return_value.returncode = 1
             assert not lvm.pv_remove("lvm_test")
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/md_test.py` & `sts_libs-0.0.4/sts_libs/tests/md_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             "state": "inactive",
         },
     },
 }
 
 
 class TestMD(unittest.TestCase):
-    @patch("sts.md.run")
+    @patch("sts.md.run_ret_out")
     def test_md_query(self, run_func):
         run_func.return_value = (0, mdstat_output)
 
         assert md.md_query() == ["md0"]
 
         assert run_func.call_count == 1
         run_calls = [call("cat /proc/mdstat", return_output=True, verbose=False)]
@@ -105,29 +105,29 @@
     def test_md_get_storage_dev(self, md_get_info_func):
         md_get_info_func.return_value = md0_info
 
         storage_devs = md.md_get_storage_dev("md0")
         assert "/dev/sda" in storage_devs
         assert "/dev/sdb1" in storage_devs
 
-    @patch("sts.md.run")
+    @patch("sts.md.run_ret_out")
     def test_md_stop(self, run_func):
         run_func.return_value = (0, "")
         assert md.md_stop("md0")
         run_calls = [call("mdadm --stop /dev/md0", return_output=True, verbose=False)]
         run_func.assert_has_calls(run_calls)
 
-    @patch("sts.md.run")
+    @patch("sts.md.run_ret_out")
     def test_md_clean(self, run_func):
         run_func.return_value = (0, "")
         assert md.md_clean("/dev/sda")
         run_calls = [call("mdadm --zero-superblock /dev/sda", return_output=True, verbose=False)]
         run_func.assert_has_calls(run_calls)
 
-    @patch("sts.md.run")
+    @patch("sts.md.run_ret_out")
     @patch("sts.md.md_stop")
     @patch("sts.md.md_get_storage_dev")
     def test_md_remove(self, get_sto_func, md_stop_func, run_func):
         run_func.return_value = (0, "")
         md_stop_func.return_value = True
         get_sto_func.return_value = ["/dev/sda1", "/dev/sdb1"]
         assert md.md_remove("md0", clean=True)
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/net_test.py` & `sts_libs-0.0.4/sts_libs/tests/net_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,25 +85,25 @@
         assert not net.nm_conn_up(NOTVALID)
 
     def test_nm_set_ip(self):
         assert not net.nm_set_ip(NOTVALID, NOTIP)
         assert not net.nm_set_ip(NOTVALID, IPV6)
 
     def test_nm_dev_mod_success(self):
-        with patch("sts.net.run") as run_func:
+        with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [0, ""]
             assert net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
 
     def test_nm_dev_mod_failure(self):
-        with patch("sts.net.run") as run_func:
+        with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [1, "Mocked failure"]
             assert not net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
 
     def test_nm_set_ip_success(self):
-        with patch("sts.net.run") as run_func:
+        with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [0, ""]
             assert net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
 
     def test_nm_set_ip_failure(self):
-        with patch("sts.net.run") as run_func:
+        with patch("sts.net.run_ret_out") as run_func:
             run_func.return_value = [1, "Mocked failure"]
             assert not net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.4/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.4/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/LICENSE` & `sts_libs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/pyproject.toml` & `sts_libs-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["hatchling", "hatch-requirements-txt"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sts-libs"
 description = ""
 readme = "sts_libs/README.md"
 requires-python = ">=3.8"
-dynamic = ["version", "optional-dependencies"]
+dynamic = ["version"]
 authors = [
   { name = "Bruno Goncalves", email = "bgoncalv@redhat.com" },
   { name = "Filip Suba", email = "fsuba@redhat.com" },
   { name = "Jakub Krysl", email = "jkrysl@redhat.com" },
   { name = "Martin Hoyer", email = "mhoyer@redhat.com" },
 ]
 maintainers = [
@@ -24,39 +24,43 @@
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Testing",
+  "Topic :: Software Development :: Quality Assurance",
   "Intended Audience :: Developers",
   "Operating System :: POSIX :: Linux",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "Framework :: Hatch",
 ]
 
 dependencies = [
-  "configobj >=5.0.8",
-  "netifaces2 >=0.0.15",
+  "pytest",
+  "configobj==5.0.8",
+  "netifaces2==0.0.16",
+  "six==1.16.0",
+      # via configobj
+  "typing-extensions==4.5.0"
+      # via netifaces2
 ]
 
 [project.urls]
 Repository = "https://gitlab.com/rh-kernel-stqe/sts/"
 
 [tool.hatch.version]
 path = "sts_libs/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["sts_libs", "requirements-stable.txt", "LICENSE"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["sts_libs/src/sts"]
 
-[tool.hatch.metadata.hooks.requirements_txt.optional-dependencies]
-stable = ["requirements-stable.txt"]
-
 [tool.black]
 line-length = 120
 target-version = ["py311", "py39", "py38"]
 
 [tool.ruff]
 line-length = 120
 namespace-packages = ["sts_libs"]
@@ -109,14 +113,15 @@
 ignore = [
   "D10",  # Missing docstring
   "D205",  # 1 blank line required between summary line and description
   "D417",  # Missing argument descriptions -> Do not use docstring description for well type-annotated args
   "PLR09",  # pylint-refactor too-many
   "PLC1901",  # compare-to-empty-string
   "PLR2004",  # magic value
+  "TRY300",  # Consider moving this statement to an `else` block. Seems to be broken?
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["INP001"]
 
 [tool.ruff.flake8-builtins]
 builtins-ignorelist = ["id"]
```

### Comparing `sts_libs-0.0.3.dev3/sts_libs/README.md` & `sts_libs-0.0.4/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.3.dev3/PKG-INFO` & `sts_libs-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.3.dev3
+Version: 0.0.4
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
+Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
-Requires-Dist: configobj>=5.0.8
-Requires-Dist: netifaces2>=0.0.15
-Provides-Extra: stable
-Requires-Dist: configobj==5.0.8; extra == 'stable'
-Requires-Dist: netifaces2==0.0.15; extra == 'stable'
-Requires-Dist: six==1.16.0; extra == 'stable'
-Requires-Dist: typing-extensions==4.1.1; extra == 'stable'
+Requires-Dist: configobj==5.0.8
+Requires-Dist: netifaces2==0.0.16
+Requires-Dist: pytest
+Requires-Dist: six==1.16.0
+Requires-Dist: typing-extensions==4.5.0
 Description-Content-Type: text/markdown
 
 # sts-libs
 
 Libs for testing storage drivers and userspace utilities on rpm-based operating systems.
 
 ## What is this?
```

