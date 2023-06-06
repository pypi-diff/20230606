# Comparing `tmp/pyDFTutils-0.1.8.tar.gz` & `tmp/pyDFTutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDFTutils-0.1.8.tar", last modified: Thu Nov  3 16:38:55 2022, max compression
+gzip compressed data, was "pyDFTutils-0.1.9.tar", last modified: Sun Jun  4 18:47:52 2023, max compression
```

## Comparing `pyDFTutils-0.1.8.tar` & `pyDFTutils-0.1.9.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.296800 pyDFTutils-0.1.8/
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7651 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/LICENSE
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      524 2022-11-03 16:38:55.296800 pyDFTutils-0.1.8/PKG-INFO
--rw-r--r--   0 hexu      (1000) hexu      (1000)       71 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.244800 pyDFTutils-0.1.8/pyDFTutils/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/__init__.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.252800 pyDFTutils-0.1.8/pyDFTutils/abinit/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7848 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/abinit.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1173 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/abinit_io.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14424 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/abinit_reader.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2050 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/dos.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    60314 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    63035 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit_e.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)    69432 2020-04-29 08:40:17.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit_vca.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     5579 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abinit/read_2DE.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.256800 pyDFTutils-0.1.8/pyDFTutils/abipy/
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4075 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/Perovskite.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      294 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/abi_poscar.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6787 2020-04-19 08:06:07.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/flow.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6333 2022-02-07 14:02:18.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/input_utils.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3788 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/pp_finder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3195 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/abipy/test.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.260800 pyDFTutils-0.1.8/pyDFTutils/ase_utils/
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      127 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)       24 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/ase_utils.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6894 2022-11-03 15:54:29.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/frozenphonon.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7559 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/gen_pp.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    23306 2021-09-06 10:15:04.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/geometry.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      410 2021-11-03 08:19:54.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/get_wyckoff.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3705 2021-01-10 11:02:41.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/ioput.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4785 2021-05-17 18:34:37.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/kpoints.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     3431 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/spacegroup.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1165 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/ase_utils/symbol.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.264800 pyDFTutils-0.1.8/pyDFTutils/espresso/
--rw-r--r--   0 hexu      (1000) hexu      (1000)    41702 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/espresso/Pwscf.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/espresso/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5957 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/espresso/qe_pp_finder.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.264800 pyDFTutils-0.1.8/pyDFTutils/math/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/math/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    27246 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/math/peakdetect.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.268800 pyDFTutils-0.1.8/pyDFTutils/perovskite/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2875 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/calc_many.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     2732 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/cubic_perovskite.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    23834 2021-10-30 08:51:36.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/frozen_mode.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      805 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/gen_111.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8373 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/lattice_factory.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    21324 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/octahedra.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    11371 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/perovskite_mode.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14848 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/plotphon.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    13199 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/perovskite/tfactor.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.268800 pyDFTutils-0.1.8/pyDFTutils/phonon/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/phonon/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    16721 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/phonon/parser.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7142 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/phonon/plot_phon_nc.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14805 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/phonon/plotphon.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1505 2021-01-06 08:59:24.000000 pyDFTutils-0.1.8/pyDFTutils/phonon/plotphonopy.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.268800 pyDFTutils-0.1.8/pyDFTutils/plot/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/plot/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8300 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/plot/wannier_band_plot.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.272800 pyDFTutils-0.1.8/pyDFTutils/pseudopotential/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       49 2020-04-08 18:36:52.000000 pyDFTutils-0.1.8/pyDFTutils/pseudopotential/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1250 2020-04-08 19:16:07.000000 pyDFTutils-0.1.8/pyDFTutils/pseudopotential/download_dojo.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1887 2022-08-22 11:33:34.000000 pyDFTutils-0.1.8/pyDFTutils/pseudopotential/find_pp.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7507 2020-04-08 16:08:14.000000 pyDFTutils-0.1.8/pyDFTutils/pseudopotential/gen_pp.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.272800 pyDFTutils-0.1.8/pyDFTutils/queue/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/queue/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14466 2022-02-14 08:08:09.000000 pyDFTutils-0.1.8/pyDFTutils/queue/commander.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      398 2022-02-14 07:47:34.000000 pyDFTutils-0.1.8/pyDFTutils/queue/template.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.272800 pyDFTutils-0.1.8/pyDFTutils/siesta/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       48 2020-03-04 12:05:32.000000 pyDFTutils-0.1.8/pyDFTutils/siesta/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10147 2022-08-22 16:01:20.000000 pyDFTutils-0.1.8/pyDFTutils/siesta/mysiesta.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2486 2020-11-20 20:02:23.000000 pyDFTutils-0.1.8/pyDFTutils/siesta/read_MDnc.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.276800 pyDFTutils-0.1.8/pyDFTutils/tightbinding/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/tightbinding/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    18994 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/tightbinding/mypythTB.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2820 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/tightbinding/mytb.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3821 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/tightbinding/occupations.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.276800 pyDFTutils-0.1.8/pyDFTutils/unfolding/
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7680 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/unfolding/DDB_unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)       76 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/unfolding/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     6698 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/unfolding/phonon_unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4854 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/unfolding/unfolder.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.284800 pyDFTutils-0.1.8/pyDFTutils/vasp/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5834 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/bader.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)    29832 2021-04-20 20:43:16.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/myvasp.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4451 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/plot_potential.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     3569 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/procar_reader.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      364 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/sumdos.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)    35218 2022-06-19 16:26:19.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_dos.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      790 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_read.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4626 2020-04-30 07:04:33.000000 pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_utils.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.292800 pyDFTutils-0.1.8/pyDFTutils/wannier90/
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      176 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/__init__.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5996 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/band_plot.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7630 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/green.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      476 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/move_wannier.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)   153556 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/pythtb.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)   153581 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/pythtb_forj.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1669 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/read_ham.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7727 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wann_green_J.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    10371 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wann_ham.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    25277 2021-12-20 08:03:40.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     2137 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_TB.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7373 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_interface.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)    15119 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_utils.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4850 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/pyDFTutils/wannier90/xyz_read.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.244800 pyDFTutils-0.1.8/pyDFTutils.egg-info/
--rw-r--r--   0 hexu      (1000) hexu      (1000)      524 2022-11-03 16:38:55.000000 pyDFTutils-0.1.8/pyDFTutils.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3247 2022-11-03 16:38:55.000000 pyDFTutils-0.1.8/pyDFTutils.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)        1 2022-11-03 16:38:55.000000 pyDFTutils-0.1.8/pyDFTutils.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)       49 2022-11-03 16:38:55.000000 pyDFTutils-0.1.8/pyDFTutils.egg-info/requires.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)       11 2022-11-03 16:38:55.000000 pyDFTutils-0.1.8/pyDFTutils.egg-info/top_level.txt
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-11-03 16:38:55.296800 pyDFTutils-0.1.8/scripts/
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1241 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/scripts/AFM_parameter.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      910 2020-04-16 15:55:30.000000 pyDFTutils-0.1.8/scripts/plotldos.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1169 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/scripts/plotpdos.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      234 2020-03-03 13:52:28.000000 pyDFTutils-0.1.8/scripts/run_wannier.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)      928 2021-05-12 15:10:19.000000 pyDFTutils-0.1.8/scripts/view_pos_info.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2022-11-03 16:38:55.296800 pyDFTutils-0.1.8/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      832 2022-11-03 16:38:40.000000 pyDFTutils-0.1.8/setup.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.227690 pyDFTutils-0.1.9/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7651 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/LICENSE
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      477 2023-06-04 18:47:52.223690 pyDFTutils-0.1.9/PKG-INFO
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       71 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/README.md
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.211690 pyDFTutils-0.1.9/pyDFTutils/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/__init__.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.215690 pyDFTutils-0.1.9/pyDFTutils/abinit/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7848 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/abinit.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1173 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/abinit_io.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14424 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/abinit_reader.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2050 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/dos.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    60314 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    63035 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit_e.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)    69432 2020-04-29 08:40:17.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit_vca.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     5579 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abinit/read_2DE.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.215690 pyDFTutils-0.1.9/pyDFTutils/abipy/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4075 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/Perovskite.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      294 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/abi_poscar.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6787 2020-04-19 08:06:07.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/flow.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6333 2022-02-07 14:02:18.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/input_utils.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3788 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/pp_finder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3195 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/abipy/test.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.215690 pyDFTutils-0.1.9/pyDFTutils/ase_utils/
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      127 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       24 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/ase_utils.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6892 2022-11-06 10:10:23.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/frozenphonon.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7559 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/gen_pp.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    23306 2021-09-06 10:15:04.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/geometry.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      410 2021-11-03 08:19:54.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/get_wyckoff.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3705 2021-01-10 11:02:41.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/ioput.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4785 2021-05-17 18:34:37.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/kpoints.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     3431 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/spacegroup.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1165 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/ase_utils/symbol.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.215690 pyDFTutils-0.1.9/pyDFTutils/espresso/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    41702 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/espresso/Pwscf.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/espresso/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5957 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/espresso/qe_pp_finder.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.215690 pyDFTutils-0.1.9/pyDFTutils/math/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/math/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    27246 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/math/peakdetect.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/perovskite/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2875 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/calc_many.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     2732 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/cubic_perovskite.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    23834 2021-10-30 08:51:36.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/frozen_mode.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      805 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/gen_111.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8373 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/lattice_factory.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    21324 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/octahedra.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    11371 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/perovskite_mode.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14848 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/plotphon.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    13199 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/perovskite/tfactor.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/phonon/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/phonon/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    16721 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/phonon/parser.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7142 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/phonon/plot_phon_nc.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14805 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/phonon/plotphon.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1505 2021-01-06 08:59:24.000000 pyDFTutils-0.1.9/pyDFTutils/phonon/plotphonopy.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/plot/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/plot/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8300 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/plot/wannier_band_plot.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/pseudopotential/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       49 2020-04-08 18:36:52.000000 pyDFTutils-0.1.9/pyDFTutils/pseudopotential/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1250 2020-04-08 19:16:07.000000 pyDFTutils-0.1.9/pyDFTutils/pseudopotential/download_dojo.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1887 2022-08-22 11:33:34.000000 pyDFTutils-0.1.9/pyDFTutils/pseudopotential/find_pp.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7507 2020-04-08 16:08:14.000000 pyDFTutils-0.1.9/pyDFTutils/pseudopotential/gen_pp.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/queue/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/queue/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14466 2022-02-14 08:08:09.000000 pyDFTutils-0.1.9/pyDFTutils/queue/commander.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      398 2022-02-14 07:47:34.000000 pyDFTutils-0.1.9/pyDFTutils/queue/template.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/siesta/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       48 2020-03-04 12:05:32.000000 pyDFTutils-0.1.9/pyDFTutils/siesta/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10339 2023-06-04 18:45:24.000000 pyDFTutils-0.1.9/pyDFTutils/siesta/mysiesta.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2486 2020-11-20 20:02:23.000000 pyDFTutils-0.1.9/pyDFTutils/siesta/read_MDnc.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/tightbinding/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/tightbinding/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    18994 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/tightbinding/mypythTB.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2820 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/tightbinding/mytb.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3821 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/tightbinding/occupations.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.219690 pyDFTutils-0.1.9/pyDFTutils/unfolding/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7680 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/unfolding/DDB_unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       76 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/unfolding/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     6698 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/unfolding/phonon_unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4854 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/unfolding/unfolder.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.223690 pyDFTutils-0.1.9/pyDFTutils/vasp/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5834 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/bader.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)    29832 2021-04-20 20:43:16.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/myvasp.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4451 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/plot_potential.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     3569 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/procar_reader.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      364 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/sumdos.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)    35218 2022-06-19 16:26:19.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_dos.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      790 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_read.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4626 2020-04-30 07:04:33.000000 pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_utils.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.223690 pyDFTutils-0.1.9/pyDFTutils/wannier90/
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      176 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/__init__.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     5996 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/band_plot.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7630 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/green.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      476 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/move_wannier.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)   153556 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/pythtb.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)   153581 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/pythtb_forj.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1669 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/read_ham.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7727 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wann_green_J.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    10371 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wann_ham.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    25277 2021-12-20 08:03:40.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     2137 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_TB.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7373 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_interface.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)    15119 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_utils.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     4850 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/pyDFTutils/wannier90/xyz_read.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.211690 pyDFTutils-0.1.9/pyDFTutils.egg-info/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      477 2023-06-04 18:47:52.000000 pyDFTutils-0.1.9/pyDFTutils.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3247 2023-06-04 18:47:52.000000 pyDFTutils-0.1.9/pyDFTutils.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        1 2023-06-04 18:47:52.000000 pyDFTutils-0.1.9/pyDFTutils.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       49 2023-06-04 18:47:52.000000 pyDFTutils-0.1.9/pyDFTutils.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       11 2023-06-04 18:47:52.000000 pyDFTutils-0.1.9/pyDFTutils.egg-info/top_level.txt
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2023-06-04 18:47:52.223690 pyDFTutils-0.1.9/scripts/
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1241 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/scripts/AFM_parameter.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      910 2020-04-16 15:55:30.000000 pyDFTutils-0.1.9/scripts/plotldos.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1169 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/scripts/plotpdos.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      234 2020-03-03 13:52:28.000000 pyDFTutils-0.1.9/scripts/run_wannier.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)      928 2021-05-12 15:10:19.000000 pyDFTutils-0.1.9/scripts/view_pos_info.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2023-06-04 18:47:52.227690 pyDFTutils-0.1.9/setup.cfg
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      904 2023-06-04 18:46:15.000000 pyDFTutils-0.1.9/setup.py
```

### Comparing `pyDFTutils-0.1.8/LICENSE` & `pyDFTutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/abinit.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/abinit.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/abinit_io.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/abinit_io.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/abinit_reader.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/abinit_reader.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/dos.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/dos.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit_e.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit_e.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/myabinit_vca.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/myabinit_vca.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abinit/read_2DE.py` & `pyDFTutils-0.1.9/pyDFTutils/abinit/read_2DE.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abipy/Perovskite.py` & `pyDFTutils-0.1.9/pyDFTutils/abipy/Perovskite.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abipy/flow.py` & `pyDFTutils-0.1.9/pyDFTutils/abipy/flow.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abipy/input_utils.py` & `pyDFTutils-0.1.9/pyDFTutils/abipy/input_utils.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abipy/pp_finder.py` & `pyDFTutils-0.1.9/pyDFTutils/abipy/pp_finder.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/abipy/test.py` & `pyDFTutils-0.1.9/pyDFTutils/abipy/test.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/frozenphonon.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/frozenphonon.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 cell=scell.get_cell(),
                 pbc=True)
             if is_mag:
                 cell.set_initial_magnetic_moments(
                     sc_mag)
             write('Supercell.cif', cell)
             mcalc = copy.deepcopy(calc)
-            mcalc.set(lwave=True, lcharg=True)
+            #mcalc.set(lwave=True, lcharg=True)
             cell.set_calculator(mcalc)
             dir_name = "SUPERCELL0"
             cur_dir = os.getcwd()
             if not os.path.exists(dir_name):
                 os.mkdir(dir_name)
             os.chdir(dir_name)
             mcalc.scf_calculation(cell)
@@ -132,15 +132,15 @@
             cur_dir = os.getcwd()
             if not os.path.exists(dir_name):
                 os.mkdir(dir_name)
             if prepare_initial_wavecar:
                 os.system('ln -s %s %s' %
                           (os.path.abspath("SUPERCELL0/WAVECAR"),
                            os.path.join(dir_name, 'WAVECAR')))
-                os.system('ln -s %s %s' %
+                os.system('cp %s %s' %
                           (os.path.abspath("SUPERCELL0/siesta.DM"),
                            os.path.join(dir_name, 'siesta.DM')))
 
 
             os.chdir(dir_name)
             forces = cell.get_forces()
             print("[Phonopy] Forces: %s" % forces)
```

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/gen_pp.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/gen_pp.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/geometry.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/ioput.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/ioput.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/kpoints.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/kpoints.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/spacegroup.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/spacegroup.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/ase_utils/symbol.py` & `pyDFTutils-0.1.9/pyDFTutils/ase_utils/symbol.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/espresso/Pwscf.py` & `pyDFTutils-0.1.9/pyDFTutils/espresso/Pwscf.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/espresso/qe_pp_finder.py` & `pyDFTutils-0.1.9/pyDFTutils/espresso/qe_pp_finder.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/math/peakdetect.py` & `pyDFTutils-0.1.9/pyDFTutils/math/peakdetect.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/calc_many.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/calc_many.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/cubic_perovskite.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/cubic_perovskite.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/frozen_mode.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/frozen_mode.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/gen_111.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/gen_111.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/lattice_factory.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/lattice_factory.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/octahedra.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/octahedra.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/perovskite_mode.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/perovskite_mode.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/plotphon.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/plotphon.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/perovskite/tfactor.py` & `pyDFTutils-0.1.9/pyDFTutils/perovskite/tfactor.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/phonon/parser.py` & `pyDFTutils-0.1.9/pyDFTutils/phonon/parser.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/phonon/plot_phon_nc.py` & `pyDFTutils-0.1.9/pyDFTutils/phonon/plot_phon_nc.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/phonon/plotphon.py` & `pyDFTutils-0.1.9/pyDFTutils/phonon/plotphon.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/phonon/plotphonopy.py` & `pyDFTutils-0.1.9/pyDFTutils/phonon/plotphonopy.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/plot/wannier_band_plot.py` & `pyDFTutils-0.1.9/pyDFTutils/plot/wannier_band_plot.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/pseudopotential/download_dojo.py` & `pyDFTutils-0.1.9/pyDFTutils/pseudopotential/download_dojo.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/pseudopotential/find_pp.py` & `pyDFTutils-0.1.9/pyDFTutils/pseudopotential/find_pp.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/pseudopotential/gen_pp.py` & `pyDFTutils-0.1.9/pyDFTutils/pseudopotential/gen_pp.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/queue/commander.py` & `pyDFTutils-0.1.9/pyDFTutils/queue/commander.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/siesta/mysiesta.py` & `pyDFTutils-0.1.9/pyDFTutils/siesta/mysiesta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import math
 import numpy as np
 from ase.calculators.siesta import Siesta
 from ase.calculators.calculator import FileIOCalculator, ReadError
 from ase.calculators.siesta.parameters import format_fdf
 from ase.calculators.siesta.parameters import Species, PAOBasisBlock
+from ase.io import write
 from pyDFTutils.pseudopotential import DojoFinder
 import copy
 
 
 def get_species(atoms, xc, rel='sr', accuracy='standard'):
     finder = DojoFinder()
     elems = list(dict.fromkeys(atoms.get_chemical_symbols()).keys())
@@ -38,14 +39,15 @@
 class MySiesta(Siesta):
     def __init__(self,
                  atoms=None,
                  command=None,
                  xc='LDA',
                  spin='non-polarized',
                  basis_set='DZP',
+                 species=None,
                  ghosts=[],
                  input_basis_set={},
                  pseudo_path=None,
                  input_pp={},
                  pp_accuracy='standard',
                  fincore=False,
                  **kwargs):
@@ -184,14 +186,15 @@
         TypeOfRun='Broyden',
         VariableCell=True,
         ConstantVolume=False,
         RelaxCellOnly=False,
         MaxForceTol=0.001,
         MaxStressTol=1,
         NumCGSteps=40,
+        relaxed_file="relaxed.vasp"
     ):
         pbc = atoms.get_pbc()
         initial_magnetic_moments = atoms.get_initial_magnetic_moments()
         self.update_fdf_arguments({
             'MD.TypeOfRun': TypeOfRun,
             'MD.VariableCell': VariableCell,
             'MD.ConstantVolume': ConstantVolume,
@@ -204,14 +207,16 @@
         self.read(self.prefix + '.XV')
         self.atoms.set_pbc(pbc)
         self.atoms.set_initial_magnetic_moments(initial_magnetic_moments)
         atoms = self.atoms
         self.update_fdf_arguments({
             'MD.NumCGSteps': 0,
         })
+        if relaxed_file is not None:
+            write(relaxed_file, atoms, vasp5=True, sort=False)
         return self.atoms
 
     def _write_structure(self, f, atoms):
         """Translate the Atoms object to fdf-format.
 
         Parameters:
             - f:     An open file object.
```

### Comparing `pyDFTutils-0.1.8/pyDFTutils/siesta/read_MDnc.py` & `pyDFTutils-0.1.9/pyDFTutils/siesta/read_MDnc.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/tightbinding/mypythTB.py` & `pyDFTutils-0.1.9/pyDFTutils/tightbinding/mypythTB.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/tightbinding/mytb.py` & `pyDFTutils-0.1.9/pyDFTutils/tightbinding/mytb.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/tightbinding/occupations.py` & `pyDFTutils-0.1.9/pyDFTutils/tightbinding/occupations.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/unfolding/DDB_unfolder.py` & `pyDFTutils-0.1.9/pyDFTutils/unfolding/DDB_unfolder.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/unfolding/phonon_unfolder.py` & `pyDFTutils-0.1.9/pyDFTutils/unfolding/phonon_unfolder.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/unfolding/unfolder.py` & `pyDFTutils-0.1.9/pyDFTutils/unfolding/unfolder.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/bader.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/bader.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/myvasp.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/myvasp.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/plot_potential.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/plot_potential.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/procar_reader.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/procar_reader.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_dos.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_dos.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_read.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_read.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/vasp/vasp_utils.py` & `pyDFTutils-0.1.9/pyDFTutils/vasp/vasp_utils.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/band_plot.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/band_plot.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/green.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/green.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/pythtb.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/pythtb.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/pythtb_forj.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/pythtb_forj.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/read_ham.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/read_ham.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wann_green_J.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wann_green_J.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wann_ham.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wann_ham.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_TB.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_TB.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_interface.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_interface.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/wannier_utils.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/wannier_utils.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils/wannier90/xyz_read.py` & `pyDFTutils-0.1.9/pyDFTutils/wannier90/xyz_read.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/pyDFTutils.egg-info/SOURCES.txt` & `pyDFTutils-0.1.9/pyDFTutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/scripts/AFM_parameter.py` & `pyDFTutils-0.1.9/scripts/AFM_parameter.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/scripts/plotldos.py` & `pyDFTutils-0.1.9/scripts/plotldos.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/scripts/plotpdos.py` & `pyDFTutils-0.1.9/scripts/plotpdos.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/scripts/view_pos_info.py` & `pyDFTutils-0.1.9/scripts/view_pos_info.py`

 * *Files identical despite different names*

### Comparing `pyDFTutils-0.1.8/setup.py` & `pyDFTutils-0.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(
     name='pyDFTutils',
-    version='0.1.8',
+    version='0.1.9',
     description='utils for DFT/TB calculation',
     author='Xu He',
     author_email='mailhexu@gmail.com',
     license='GPLv3',
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scipy',
                       'ase', 'spglib',  'phonopy', 'pathos'],
-    scripts=[],
+    scripts=["scripts/view_pos_info.py", "scripts/plotldos.py", "scripts/plotpdos.py"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
```

