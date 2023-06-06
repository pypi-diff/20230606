# Comparing `tmp/pyw90-1.0.6.tar.gz` & `tmp/pyw90-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyw90-1.0.6.tar", max compression
+gzip compressed data, was "pyw90-1.0.7.tar", max compression
```

## Comparing `pyw90-1.0.6.tar` & `pyw90-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35823 2022-09-15 04:43:07.000000 pyw90-1.0.6/LICENSE
--rw-r--r--   0        0        0    42298 2022-09-23 14:41:06.000000 pyw90-1.0.6/README.md
--rw-r--r--   0        0        0     1165 2022-10-14 06:19:06.000000 pyw90-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-22 07:22:09.000000 pyw90-1.0.6/pyw90/__init__.py
--rw-r--r--   0        0        0     5760 2022-10-01 16:54:38.000000 pyw90-1.0.6/pyw90/auto_w90_fit.py
--rw-r--r--   0        0        0     2098 2022-09-23 14:40:27.000000 pyw90-1.0.6/pyw90/auto_w90_input.yaml
--rw-r--r--   0        0        0        0 2022-09-22 07:22:08.000000 pyw90-1.0.6/pyw90/lib/__init__.py
--rw-r--r--   0        0        0     9133 2022-09-30 13:30:59.000000 pyw90-1.0.6/pyw90/lib/config.py
--rw-r--r--   0        0        0    20520 2022-09-29 13:47:31.000000 pyw90-1.0.6/pyw90/lib/dos.py
--rw-r--r--   0        0        0     5153 2022-09-29 14:57:35.000000 pyw90-1.0.6/pyw90/lib/job.py
--rw-r--r--   0        0        0    39549 2022-09-30 07:45:35.000000 pyw90-1.0.6/pyw90/lib/w90.py
--rw-r--r--   0        0        0    10736 2022-09-30 14:08:28.000000 pyw90-1.0.6/pyw90/pre_w90_tool.py
--rw-r--r--   0        0        0    20149 2022-09-30 14:08:27.000000 pyw90-1.0.6/pyw90/pyw90_cli.py
--rw-r--r--   0        0        0        0 2022-09-22 07:22:09.000000 pyw90-1.0.6/pyw90/utility/__init__.py
--rw-r--r--   0        0        0     6910 2022-09-23 14:40:34.000000 pyw90-1.0.6/pyw90/utility/utility.py
--rw-r--r--   0        0        0    43303 1970-01-01 00:00:00.000000 pyw90-1.0.6/setup.py
--rw-r--r--   0        0        0    42678 1970-01-01 00:00:00.000000 pyw90-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-15 04:43:07.000000 pyw90-1.0.7/LICENSE
+-rw-r--r--   0        0        0    42298 2022-09-23 14:41:06.000000 pyw90-1.0.7/README.md
+-rw-r--r--   0        0        0     1165 2023-06-06 08:38:30.000000 pyw90-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-14 07:02:13.000000 pyw90-1.0.7/pyw90/__init__.py
+-rw-r--r--   0        0        0     5796 2022-10-14 07:02:11.000000 pyw90-1.0.7/pyw90/auto_w90_fit.py
+-rw-r--r--   0        0        0     2098 2022-10-14 07:02:11.000000 pyw90-1.0.7/pyw90/auto_w90_input.yaml
+-rw-r--r--   0        0        0        0 2022-10-14 07:02:13.000000 pyw90-1.0.7/pyw90/lib/__init__.py
+-rw-r--r--   0        0        0     9133 2022-10-14 07:02:12.000000 pyw90-1.0.7/pyw90/lib/config.py
+-rw-r--r--   0        0        0    20556 2022-10-14 07:02:12.000000 pyw90-1.0.7/pyw90/lib/dos.py
+-rw-r--r--   0        0        0     5163 2022-10-14 07:02:12.000000 pyw90-1.0.7/pyw90/lib/job.py
+-rw-r--r--   0        0        0    39586 2022-10-14 13:43:17.000000 pyw90-1.0.7/pyw90/lib/w90.py
+-rw-r--r--   0        0        0    10772 2022-10-14 07:02:12.000000 pyw90-1.0.7/pyw90/pre_w90_tool.py
+-rw-r--r--   0        0        0    20185 2022-10-14 07:02:13.000000 pyw90-1.0.7/pyw90/pyw90_cli.py
+-rw-r--r--   0        0        0        0 2022-10-14 07:02:13.000000 pyw90-1.0.7/pyw90/utility/__init__.py
+-rw-r--r--   0        0        0     6946 2022-10-14 07:02:13.000000 pyw90-1.0.7/pyw90/utility/utility.py
+-rw-r--r--   0        0        0    43303 1970-01-01 00:00:00.000000 pyw90-1.0.7/setup.py
+-rw-r--r--   0        0        0    42678 1970-01-01 00:00:00.000000 pyw90-1.0.7/PKG-INFO
```

### Comparing `pyw90-1.0.6/LICENSE` & `pyw90-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyw90-1.0.6/README.md` & `pyw90-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyw90-1.0.6/pyproject.toml` & `pyw90-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyw90"
-version = "1.0.6"
+version = "1.0.7"
 description = "A VASP and Wannier90 interfaced tool for projection analysis and fully automated dis energy window optimization."
 authors = ["En Wang (Cloudiiink) <wangenzj@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Natural Language :: English",
```

### Comparing `pyw90-1.0.6/pyw90/auto_w90_fit.py` & `pyw90-1.0.7/pyw90/auto_w90_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 # Copyright (c) En Wang (Cloudiiink) <wangenzj@outlook.com>, SF10, IOP/CAS.
 # Distributed under the terms of GPLv3.Please see the LICENSE file that should have been included as part of this package.
 # For more information, please refer to https://github.com/Cloudiiink/pyw90.
 # All rights reserved.
 
+from __future__ import annotations
 import argparse
 import time, os
 from scipy.optimize import minimize
 import numpy as np
 from numpy.typing import ArrayLike
 import argparse
```

### Comparing `pyw90-1.0.6/pyw90/auto_w90_input.yaml` & `pyw90-1.0.7/pyw90/auto_w90_input.yaml`

 * *Files identical despite different names*

### Comparing `pyw90-1.0.6/pyw90/lib/config.py` & `pyw90-1.0.7/pyw90/lib/config.py`

 * *Files identical despite different names*

### Comparing `pyw90-1.0.6/pyw90/lib/dos.py` & `pyw90-1.0.7/pyw90/lib/dos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from math import sqrt
 import pandas as pd
 import numpy as np
 from numpy.typing import ArrayLike
 from typing import Tuple
 import warnings
 from collections import Counter
```

### Comparing `pyw90-1.0.6/pyw90/lib/job.py` & `pyw90-1.0.7/pyw90/lib/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
                                 capture_output=True, text=True)
         # logger.debug(jobs.stdout, jobs.stderr)
         df = pd.read_csv(io.StringIO(jobs.stdout), sep='\s+')
 
         # Not sure about job states codes is necessary or not
         # Ref:　https://slurm.schedmd.com/squeue.html
 
-        # Print jobs nice
-        logger.debug('SQUEUE RESULTS'.ljust(80, " "))
+        # Printing jobs nicely
+        logger.debug('FULL SQUEUE RESULTS'.ljust(80, " "))
         for l in str(df).split('\n'):
             logger.debug(l.ljust(80, " "))
             
         df = df[df['NAME'] == self.job_name]
         # df = df[df['USER'] == self.usr_name]
         # logger.debug(df)
         return df
```

### Comparing `pyw90-1.0.6/pyw90/lib/w90.py` & `pyw90-1.0.7/pyw90/lib/w90.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import re, os, copy
 import numpy as np
 from numpy.typing import ArrayLike
 import pandas as pd
 from typing import Dict, Tuple
 import matplotlib.pyplot as plt
 from collections import OrderedDict
@@ -406,15 +407,15 @@
         dN = N - self.nwann
         froz_min_list, froz_max_list, N = [], [], []
 
         if self.nwann <= 0:
             bc.cprint(bc.RED, f'Please input vaild number of WF, now is {self.nwann}.')
             return pd.DataFrame(columns=['dis_froz_min', 'dis_froz_max', 'N'])
 
-        elif dN > 0:
+        elif dN >= 0:
             for i in range(0, dN + 1, self.ndeg):
                 # First get froz_max for nwann = nwann_input + i, then get froz_min for nwann = nwann_input and froz_max
                 froz_max = self.suggest_froz_max(emin, nwann=self.nwann+i)
                 froz_min = self.suggest_froz_min(froz_max)
                 nstates  = self.count_states_most((froz_min, froz_max))
                 froz_max_list.append(froz_max)
                 froz_min_list.append(froz_min)
```

### Comparing `pyw90-1.0.6/pyw90/pre_w90_tool.py` & `pyw90-1.0.7/pyw90/pre_w90_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 # Copyright (c) En Wang (Cloudiiink) <wangenzj@outlook.com>, SF10, IOP/CAS.
 # Distributed under the terms of GPLv3.Please see the LICENSE file that should have been included as part of this package.
 # For more information, please refer to https://github.com/Cloudiiink/pyw90.
 # All rights reserved.
 
+from __future__ import annotations
 import argparse
 import os
 import pandas as pd
 from os.path import abspath, relpath
 
 # pymatgen
 from pymatgen.io.vasp.outputs import Vasprun
```

### Comparing `pyw90-1.0.6/pyw90/pyw90_cli.py` & `pyw90-1.0.7/pyw90/pyw90_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 # Copyright (c) En Wang (Cloudiiink) <wangenzj@outlook.com>, SF10, IOP/CAS.
 # Distributed under the terms of GPLv3.Please see the LICENSE file that should have been included as part of this package.
 # For more information, please refer to https://github.com/Cloudiiink/pyw90.
 # All rights reserved.
 
+from __future__ import annotations
 import subprocess
 import signal
 import os, sys
 import argparse
 import shutil
 import pandas as pd
```

### Comparing `pyw90-1.0.6/pyw90/utility/utility.py` & `pyw90-1.0.7/pyw90/utility/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 from numpy.typing import ArrayLike
 from typing import Callable
 import os, re, copy
 
 from pymatgen.core import structure
```

### Comparing `pyw90-1.0.6/setup.py` & `pyw90-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'scipy>=1.8']
 
 entry_points = \
 {'console_scripts': ['pyw90 = pyw90.pyw90_cli:main_cli']}
 
 setup_kwargs = {
     'name': 'pyw90',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'A VASP and Wannier90 interfaced tool for projection analysis and fully automated dis energy window optimization.',
     'long_description': "# pyw90\n\nA `VASP` and `Wannier90` interfaced tool for projection analysis and fully automated dis energy window optimization.\n\n## Key features\n\n1. Display the distribution of eigenvalues.\n2. Pre-analysis before the `Wannier90` interpolation with projection and dis energy window recommendations.\n3. Auto Wannier90 Fit. Using minimization method to choose the most appropriate dis energy windows. \n4. Comparison. Evaluate the differences between the `VASP` and `Wannier90` band structure.\n\n## Installation via `pip`\n\nInstall `pyw90` using `pip.\n\n```bash\npip install pyw90\n# update the package\npip install pyw90 --upgrade\n```\n\nThe dependencies for `pyw90` are listed below:\n\n- python (>= 3.8, < 3.12)\n- pymatgen\n- scipy (>= 1.8)\n- numpy (>= 1.20.1)\n- python-yaml (PyYAML)\n- pandas\n- matplotlib (>=3.4)\n\n## Usage\n\nAfter installing `pyw90`, you could use command line to line it. \nTo access help message, please use `pyw90 -h`. \nIn submenus, you can also use `-h` (e.g., `pyw90 auto -h`).\n\n```\nusage: pyw90 [-h] {eig,pre,auto,cmp} ...\n\nCommand-line toolbox interfaced between VASP and Wannier90. You can also use -h\nto display the submenu help message. e.g., pyw90 pre -h\n\npositional arguments:\n  {eig,pre,auto,cmp}  Menus\n    eig               Display the distribution of eigenvalues and dis energy\n                      window recommendations.\n    pre               (Pre)-analysis before `Wannier90` interpolation:\n                      generation of `Wannier90` input and improved dis energy\n                      window recommendations based on projected density of\n                      states.\n    auto              (Auto Wannier90 Fit) Using minimization method to choose\n                      the most appropriate dis energy windows.\n    cmp               (Comparison) Evaluate the differences between the `VASP`\n                      and `Wannier90` band structure.`bnd.dat` for VASP band\n                      data in `p4vasp` format and `wannier90_band.dat`,\n                      `wannier90_band.labelinfo.dat`,and `wannier90.wout` are\n                      required for plotting and analysis.\n\noptional arguments:\n  -h, --help          show this help message and exit\n```\n\n### 1. `eig` Menu\n\nThis menu provides you an overview of the entire distribution of eigenvalues. \nThese information may assisit you in determining the `exclude_bands` block in `Wannier90` and the outer window `dis_win_min` and `dis_win_max`.\n\nThe help message of `eig` menu is listed below.\n\n```\nusage: pyw90 eig [-h] [-e ERANGE ERANGE] [--config] [--path PATH] [-i EIG]\n                 [--rm-fermi] [--efermi EFERMI] [-w NWANN] [-n NBNDS_EXCL]\n                 [--deg DEG] [--plot] [--separate] [--eps EPS]\n                 mode\n\npositional arguments:\n  mode              Mode: dist, count, suggest. Only the first character is\n                    recognized.\n\noptional arguments:\n  -h, --help        show this help message and exit\n  -e ERANGE ERANGE  Energy ranges. Default: [-1e3, 1e3]\n  --config          Read input from config file `auto_w90_input.yaml` directly.\n                    Default: False\n  --path PATH       The path of working dir. Default: .\n  -i EIG            Select `wannier90.eig` file or `EIGENVAL` file. Default:\n                    EIGENVAL\n  --rm-fermi        Control whether the input energy ranges `erange` has removed\n                    the non-zero Fermi level. Default: False\n  --efermi EFERMI   Fermi level. Default value is generated from `vasprun.xml`.\n  -w NWANN          Total number of Wannier Functions. Default: 0\n  -n NBNDS_EXCL     Total number of ignored bands beginning with the lowest KS\n                    band.\n  --deg DEG         Total number of band degeneracy. Default: 1\n  --plot            Control whether the distribution is output as a figure or\n                    not\n  --separate        Control calculate bands separately\n  --eps EPS         Tolerance for dis energy window recommendations. Default:\n                    0.004\n```\n\nThe `dist` mode displays the distribution of eigenvalues \nand allows you to either generating figure named `dos_analysis.pdf` \nor print the results directly  to the terminal. Here is an example for GaAs. \nThe starting band index is indicated by the label above the bar plot and the Fermi level has been set to 0.\n\n![](image/eigenval_dis_cmp.png)\n\nIn `count` mode, the code can determine how many states exist at least and at most for each k-point within the given energy ranges `erange`. \nAnd the `suggest` mode is used to provide dis energy window recommendations. \n\nThe data is extracted from the `EIGENVAL` file or `wannier90.eig` file.\nYou could directly input the absolute or relative path to the file using the `-i` argument, \nor you could specify its location folder through the `-path` argument.\nUsing the `-e` argument, the output energy ranges can be controlled both in printing and figure.\nIt is also possible to use the `-e` argument to calculate the number of states existed within the given energe ranges and provide recommendations for the `dis_win_min` and `dis_win_max` values.\nThis requires the `-w` argument passes non-zero number of Wannier functions (#WFs) to the code. \n\nWe read the data from the `EIGENVAL` file without modification.\nTherefore, the Fermi level for most materials is typically non-zero.\nIf you add the argument `—rm-fermi`, the code will consider Fermi level to be 0.\nThis will affect the energy ranges obtained from `-e` argument.\nThe default Fermi level is read from the `vasprun.xml` file located in the `—path` directory.\nWithin the `—efermi` argument, you can also explicitly state a different number to become Fermi level. \n\nOther arguments and parameters:\n\n- `-n NBNDS_EXCL`. Total number of ignored bands beginning with the lowest KS band. These bands will be hidden in 'dist' mode.\n- `--deg DEG`. Band degeneracy. Please enter `--deg 2` to account for the degree of spin freedom when counting Wannier functions. The default value is 1.\n- `--eps EPS`. Due to the insufficient sampling in the Brilliouin zone as well as the numerical error, the number of states within the energy ranges may be underestimated. This may result in the failure of `Wannier90`. Therefore, we change the final dis energy windows by substracting or adding `eps` to the band minimum and band maximum respectively.\n\n**Among all the features, the dis energy recommendation is the key feature of the `eig` menu.**\nTo activate the outer window recommendation, please use `suggest` mode.\nWe obtain all potential `dis_win_min` values from the mid-point of the global gap below Fermi level. During this step, there is no extra\nWith the extra argument `-w` (#WFs), the code would provide the `dis_win_max` values by counting the number of states inside the energy ranges. \nBecause `Wannier90` demands there ought to be at least as many states as #WFs for each kpoints. \nDuring this step, we only present the `dis_win_min` for which the band minimum is greater than the lower limit of energy ranges and the number of states between `dis_win_min` and Fermi level is less than #WFs.\n\nWe can also use `-w` argument (without input, the default value of #WFs is 0) for inner window recommendation.\nAll recommended `dis_win_min` values $E_{\\text{wmin}}$ obtained above are also utilizied as `dis_froz_min` for generating possible `dis_froz_max`. \n\nThe first step in generating `dis_froz_max` is to count how many states there are, at a minimum, over all k-points in Brilliouin zone. \nThe energy ranges here is consisted of $E_{\\text{wmin}}$ and $E_2$, which is the upper limit of given energy ranges $(E_1, E_2)$ from arguments. \nWe assume there are $N>N_{\\text{WF}}$ states at least in this energy ranges. \n\nThen the code will generate $E_{\\text{fmax}}$, upper bound of new `dis_win_max`, with at most $N_i = N_{\\text{WF}} + i$ states inside the energy ranges $\\left(E_{\\text{wmin}}, E_{\\text{fmax}}\\right)$. \nHere $i=1,2,\\cdots, N-N_{\\text{WF}}$.\nAnd then the same method is then utilized to construct the lower bound of new `dis_froz_min` as well by searching $E_{\\text{fmin}}$ matching at most $N_{\\text{WF}}$ states in energy ranges $\\left(E_{\\text{fmin}}, E_{\\text{fmax}}\\right)$.\nThis approach guarantees the generated dis frozen energy window satisfying the requirement of `Wannier90` that there are at most $N_{\\text{WF}}$ states inside. \n\nHowever, owing to the presence of degenerate points, such a straightforward approach might omit some vital frozen energy windows.\nThis is resulted by substracting `eps` from the band maximum, which is also the degenerate points.\nWith the occurance of additional states, the iteration over all states within energy ranges become discontinous and the obtained `dis_froz_min` will skip several bands and states.\n\nTo prevent the problem described above, we include an additional check to see whether there are skipped states between the input $E_{\\text{wmin}}$ and $\\min E_{\\text{fmin}}$, the minimum of all `dis_froz_min`. \nIf there are $\\Delta N$ skipped states, we will re-examine number of Wannier functions with\n\n$$\nN'_{\\text{WF}}=N_{\\text{WF}}-1, \\cdots, N_{\\text{WF}}-\\Delta N\n$$\n\nto produce potential dis frozen energy windows.\n\n### 2. `pre` Menu\n\nThis menu offers some basic `Wannier90` input and improved dis energy\nwindow recommendations based on projected density of states. The help message of `pre` menu is provided as below.\n\n```\nusage: pyw90 pre [-h] [--path PATH] [-e ERANGE ERANGE] [--lb LB] [--rm-fermi]\n                 [--extra EXTRA] [--spin-down] [--plot] [--eps EPS] [--deg DEG]\n                 mode\n\npositional arguments:\n  mode              Mode: kpath, band, template, dos. Only the first character\n                    is recognized.\n\noptional arguments:\n  -h, --help        show this help message and exit\n  --path PATH       The path of working dir. Default: .\n  -e ERANGE ERANGE  Energy range. Default: [-1e3, 1e3]\n  --lb LB           Lower bound for selected orbital / max single orbital.\n                    default: 0.1\n  --rm-fermi        Control whether the input energy ranges `erange` has removed\n                    the non-zero Fermi level. Default: False\n  --extra EXTRA     Extra input. In `template` mode and within extra input\n                    (basic, wann, band), we can choose one of the detailed parts\n                    to print.In `dos` mode and within extra input (`species`,\n                    `structure_id`, `orbital_id` list separated by ;), we can\n                    treat input as projections for `Wannier90` input to suggest\n                    dis frozen energy. Details can be found in the document.\n  --spin-down       Specify the spin channel to `Spin.down`. Without this\n                    argument, the default spin channel is `Spin.up`.\n  --plot            plot the dos distribution\n  --eps EPS         Tolerance for dis energy window recommendations. Default:\n                    0.004\n  --deg DEG         Degeneracy of bands. Default: 1\n\n```\n\nDifferent input parts are provided by **the `kpath`, `band` and `template` modes** for `Wannier90`.\n\n- `kpath` : Converting the line-mode `KPOINTS` file from `VASP` to `Kpoint_Path` block in `Wannier90`.\n- `band` : Converting `VASP` band structure into a p4vasp-type $k-E$ `.dat` file.\nDefault file name is `bnd.dat`. If the system has two spin channels, the band data will be exported into two separate files named `bnd_up.dat` and `bnd_down.dat`.\n- `template` : Print the input template for `Wannier90`, which includes the `seedname.win` file format, the dis energy window block, and the band structure calculation block. \n\n**The `dos` mode is the most important feature of `pre` menu.** From the first-principle calculation in VASP with `LORBIT=11`, `vasprun.xml` are written with decomposed orbital projection information.\n> For further details, see [LORBIT - Vaspwiki](https://www.vasp.at/wiki/index.php/LORBIT).\n\nIn order to describe the band structure `VASP` in a way that is both precise and comprehensive (especially for topological semimetal), `Wannier90` has to select projections that is both accurate and thorough.\nHere, we compare the projected density of states (pDOS) to the total density of states (tDOS) and offer recommendations of inner energy ranges `dis_froz_min(max)` based on the pDOS / tDOS ratio. \n\nYou must specify the folder where `VASP` results are stored by using `--path` argument when using the `kpath` and `band` modes.\nThe current working directory is used as default. In `template` mode,\nAll of the `Wannier90` input templates will be printed by default. \nYou can also enter the keywords `basic`, `wann` and `band` to print\nbasic structure of `seedname.win`, dis energy window block, and the band structure calculation block correspondingly.\n\nWhile the code running in `dos` mode, you must also specify the path of the `vasprun.xml` file by using `--path` argument\nThe pDOS distribution of each orbital each atom can be determined below with energy ranges $(E_1, E_2)$ obtained from `-e` argument.\nThe `--rm-fermi` argument is used if the input energy ranges `erange` assumes the eigenvalues has already removed the non-zero Fermi level.\n\n$$\n\\text{pDOS} = \\int_{E_1}^{E_2} \\text{dos}_{\\text{atom, orb}}(E)\\,\\mathrm{d}E\n$$\n\nThe output of pDOS is presented as a table with columns containing: `species`, `structure_id`, `orb_id`, `orb_name`, `key_string` and `dos`. \nThe `structure_id` is obtained from `vasprun.xml` (also same as listed in `POSCAR`) with index beginning at $0$. The `orb_id` and `orb_name` use the notation in pymatgen (same as `VASP` in old version). \n\n> For further details, see note at the end of the section.\n\nThe `key_string` is formatted with `species`, `structure_id` and `orb_name` (e.g. `Ga_0_px`). The dos column is calculated from above formula. \nSince we are only interested in the relative comparisons of pDOS, the maximum value of `dos` column is normalized to $1$.\n\nThe lower bound specified by the `lb` argument is used to determine the most representative projections.\nThe orbitals and sites are used as the `projection` block for `Wannier90` input only when the `dos` column values is greater than `lb`. \nAs soon as the projections are picked upon, the total number of Wannier functions is also determined. \nThe results are presented in a table with `species`, `site` and `orb` columns.\nThe default value for the `site` column is the `structure_id` mentioned above.\nYou might encounter the value in `site` column becomes -1 instead of other non-negative integers.\nThis is because we further simplify the selection information by unifying the case when orbitals are located at one site and all sites of the same species have the same orbitals.\n\nThe projection Information will be transformed into Wannier90's `projection` block format. \nFor further usage, it will also be written in `key_string` format for `pyw90` input with replacing the orbital name to orbital index. By default, a comma separates keys within the same species, whereas `;` separates keys from different species. (e.g., `Ga,0,1-3;As,1,1-3` represents choosing the p orbital of Ga and As)\n\nOur pDOS-based dis frozen window recommendation will be shown if the user specifies `--extra` while running in `dos` mode and provides explicit energy ranges.\nColumns for `dis_froz_min`, `dis_froz_max`, `N`, `pdos`, `tdos` and `percent` will be presented in the output. The values of `percent` column is pDOS / tDOS ratio.\nThe entire table is sorted acordding to the value of pDOS percentage.\nWe can treat the highest percentage as the initial guess for `Wannier90`.\n\nIn addition, the code also computes the minimum value of `dis_win_max`.\n\n**Note:**\n\nThe notation of orbitals has varied a lot between different softwares and differernt versions.\nThe notation for `pyw90` and `pymatgen` (2022.8.23) is identical. Notations for all orbitals are listed below:\n\n```bash\n# pymatgen 2022.8.23\ns \npy   pz   px\ndxy  dyz  dz2  dxz  dx2\nf_3  f_2  f_1  f0   f1   f2  f3\n\n# VASP 5.4.4\ns\npy     pz    px \ndxy    dyz   dz2   dxz  x2-y2\nfy3x2  fxyz  fyz2  fz3  fxz2   fzx2  fx3\n\n# Wannier90\ns\npz   px    py\ndz2  dxz   dyz   dx2-y2     dxy\nfz3  fxz2  fyz2  fz(x2-y2)  fxyz  fx(x2-3y2)  fy(3x2-y2)\n```\n\n### 3. `auto` Menu\n\n**This menu enables you do fully automated dis energy optimization** and the `auto` menu help message is listed below.\n\n```\nusage: pyw90 auto [-h] [--path PATH] [--pid PID] mode\n\npositional arguments:\n  mode         Mode: run, term(inate), input. Only first character is\n               recognized.\n\noptional arguments:\n  -h, --help   show this help message and exit\n  --path PATH  The path of working dir. Default: .\n  --pid PID    PID to terminate.\n```\n\nIf the code is executed with the `input` mode, it will generate the configuration file `auto_w90_input.yaml` in the directory specified by the `--path` option.\nThis file contains all the necessary inputs for `Wannier90` to function properly, including the initial dis energy window in `Wannier90`, minimization parameters, running and display settings.\nSince other menus share same parameters in config file, and the `--config` option has been added to other menus so that data can be extracted directly from the file.\n\nIn `run` mode, the `Wannier90` task can be executed automatically using the SLURM job system or by running the job locally. The quality of `Wannier90` result is evaulated from\n\n$$\n\\Delta=\\frac{1}{C} \\frac{1}{N_{\\mathbf{k}}} \\sum_{i=1}^{M} \\sum_{\\mathbf{k}}\\left|\\varepsilon_{i, \\mathbf{k}}^{\\mathrm{DFT}}-\\varepsilon_{i, \\mathbf{k}}^{\\mathrm{TB}}\\right|{\\color{red} f\\left(\\varepsilon_{i, \\mathbf{k}}^{\\mathrm{DFT}}\\right)}.\n$$\n\n$f(\\cdot)$ is the kernel function (unit function or gaussian function). $i$ and $\\bf k$ represent band index and kpoint separately. $C$ is the normalization constant obtained from\n\n$$\nC= \\frac{1}{N_{\\mathbf{k}}} \\sum_{i=1}^{M} \\sum_{\\mathbf{k}}{\\color{red} f\\left(\\varepsilon_{i, \\mathbf{k}}^{\\mathrm{DFT}}\\right)}.\n$$\n\nThe structure of the optimization process is displayed in the sequence diagram.\nBy executing the command `pyw90 auto run`, the script launches a daemon process called `python auto_w90_fit.py` that manages `Wannier90` submission/running and status checks.\nThe code do the primary calculation through submitting to the SLURM system or running locally.\nThe production of new parameters within the loop and the termination condition are controlled by the minimization method.\nWe will obtain the final dis energy window after a number of iterations (the maximum number of iterations is customizable in config file).\n\n\n```mermaid\nsequenceDiagram\n    participant pyw90\n    participant auto_w90_fit\n    pyw90->>auto_w90_fit: pyw90 auto run\n    Note left of auto_w90_fit: start<br/>daemon process\n    loop Wannier90 task\n        auto_w90_fit->>SLURM / local: sbatch\n        SLURM / local->>auto_w90_fit: squeue\n    end\n    Note right of auto_w90_fit: the parameters and results<br/>will export to `log_autow90_{timestamp}.log`\n    pyw90-->>auto_w90_fit: pyw90 auto term\n    Note left of auto_w90_fit: End<br/>daemon process\n    auto_w90_fit-->>SLURM / local: scancel\n```\nIn `term` mode, you will be able to finish your optimization task.\nPlease follow the execution message to kill all processes and be careful when terminating the 'pyw90' process.\n\nTypically, the public server prohibits intensive computing tasks on the login node.\nTherefore, we provide a function that allows you to execute the `Wannier90` task on a public server using SLURM system.\nLocal `Wannier90` execution for `pyw90` is also possible. \nSince the daemon process tracks the progress of your `Wannier90` job and not ending to launch new jobs until the stop condition for minimizing, terminating the SLURM job or `wannier.x` process is not enough.\nIn pratical, the `python auto_w90_fit.py` process is very simple to identify.\nThe process name is lengthy because it must pass the entire environment. \n\n**Configuration file**\n\nThe configuration file is written in YAML format and you can use `#` to comment. The contents are case-sensitive and they use indentation to indicate hierarchical relationships. Tabs are not permitted for indentation with only spaces permitted.\n\n| key              | description  |\n|------------------|--------------|\n|`seedname`        | Seedname string. The `Wannier90` code will read its input from file `seedname.win`. The band structure will be written to `seedname_band.dat`.Default: `wannier90` | \n|`runfile`         | Job file for SLURM job system to submit the `Wannier90` task  | \n|`vasp_band_file`  | Band structure file of `VASP` in `p4vasp` format. This file can be generated using `pyw90 pre band` command. Default: `bnd.dat`  | \n|`jobname`         | Name of your task. | \n|`username`        | Your username. `jobname` and `username` aer used to determine which `squeue` result corresponds to the automated `Wannier90` job from . Default `username` is obtained from `getpass.getuser`.| \n|`local`           | Boolean. If it's `True`, the `Wannier90` task will execute based on the input from `localrun`. Default: `False`. | \n|`localrun`        | Command to execute `Wannier90`. Only is used when `local: True`  | \n|`efermi`          | Fermi level of material. | \n|`kernel`          | Kernel funtion for evaluating the quality of `Wannier90` band structure result. Formatted input: type, middle, width (e.g. unit,0,1). Kernel functions are classified into two types: `unit` and `gaussian`. **The Fermi level is not subtracted from eigenvalues when using the kernel function to evaluate difference.**  | \n|`method`          | The solving method of minimization. This parameter is treated as the input for `scipy.optimize.minimize`. **We recommend you to use solver allow no gradient information, such as Nelder-Mead, Powell and COBYLA.** (See [scipy.optimize.minimize — SciPy v1.9.1 Manual](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html)). Default: COBYLA  | \n|`tol`             | Tolerance for termination. Default: 0.02. | \n|`maxiter`         | Maximum number of iterations to perform. Both `tol` and `maxiter` are also passed to `scipy.optimize.minimize`. Default: 100.| \n|`ini_dis`         | Initial dis energy windows dictionary. Input each value with indent. If some parameters is not needed, please set to `None` or `~`. | \n|`opt_dis`         | Boolean dictionary determine which parameters to optimize. `pyw90` will only optimized the key is `True`.  | \n|`bounds`          | Boundary of energy window parameters. Please using `None` or `+/- inf` to set the boundary which is unbounded. Since there is also parameters correction during each iteration of `Wannier90`, you can set a really rough bound.| \n|`num_print_check` | Frequency of printing the check message. Default: 10 |\n|`check_time`      | Time period of checking the job status. The job status is examined via the result from `squeue` in SLURM system or `pid` when `local` is `True`. Default: 30 |\n|`display`         | Boolean dictionary control display the band difference (`diff`) and total spreading of Wannier functions (`spread`). Default: both `True`.   |\n\n\n**Before executing your task, remember to modify the value of each key to your own.**\n\n### 4. `cmp` Menu\n\nThis menu enables you compare the result from `Wannier90` and `VASP`. The help message of `cmp` menu is listed below.\n\n```\nusage: pyw90 cmp [-h] [--config] [--path PATH] [--efermi EFERMI] [--vasp VASP]\n                 [--seedname SEEDNAME] [--ylim YLIM YLIM] [--kernel KERNEL]\n                 [--show-fonts] [--fontfamily FONTFAMILY] [--fontsize FONTSIZE]\n                 [--no-spread] [--no-quality] [--quiet]\n                 name\n\npositional arguments:\n  name                  name of system\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --config              Read input from config file `auto_w90_input.yaml`\n                        directly. Default: False\n  --path PATH           The path of working dir. Default: .\n  --efermi EFERMI       Fermi level. Default value is generated from\n                        `vasprun.xml`.\n  --vasp VASP           Path of VASP band file in `p4vasp` format. Default:\n                        bnd.dat\n  --seedname SEEDNAME   Seedname of Wannier90 input. Default: wannier90\n  --ylim YLIM YLIM      Energy bound for plot. Please note that the Fermi level\n                        has been shifted to 0 during the plotting\n                        process. Default: [E_w90.min - 1, E_w90.max + 1]\n  --kernel KERNEL       Formatted input: type, middle, width (Defalut:\n                        unit,0,1). Kernel functions are classified into two\n                        types: `unit` and `gaussian`. **The Fermi level is not\n                        subtracted from eigenvalues when using the kernel\n                        function to evaluate difference**.\n  --show-fonts          Show all availabel font families can be used in\n                        `rcParams`\n  --fontfamily FONTFAMILY\n                        Set font family manually. Default: Open Sans\n  --fontsize FONTSIZE   Set font size manually. Default: 18\n  --no-spread           Don't plot spreading\n  --no-quality          Don't show quality of fitting\n  --quiet               Equal to --no-spreading --no-quality\n```\n\nFinal figure `name_VASP_W90_cmp.png` will be created in current folder for comparison with `name` argument from input.\n\n![](image/GaAs_VASP_W90_cmp.png)\n\nThe `--path` parameter specifies the directory in which to find the required file, while the `--vasp` and `--seedname` arguments locate the `VASP` and `Wannier90` band structure data, respectively.\nThe `--efermi` option lets you choose the Fermi energy level.\nTo assess the accuracy of `Wannier90` output, the `--kernel` option specifies the kernel function to evaluate quality described in the `auto` subsection.\nBy default, the wannierization of all Wannier functions and a band difference notification will display as shown below.\nYou may skip one of the messages by using the `--no-spread` or `--no-quality` options.\nTo block either of these messages, please use the `--quiet` option. \n\n```\n+-----+--------------------------------++-----+--------------------------------+\n|   i | MAX DIFF (meV)                 ||   i | AVERAGE DIFF (meV)             |\n+-----+--------------------------------++-----+--------------------------------+\n|   1 |████ 0.36                       ||   1 |██████ 0.12                     |\n|   2 |████████████ 1.10               ||   2 |█████████████████████ 0.36      |\n|   3 |██████████████████████ 1.88     ||   3 |██████████████████████ 0.38     |\n|   4 |███████████████ 1.32            ||   4 |██████████████ 0.25             |\n|   5 | 0.00                           ||   5 | 0.00                           |\n|   6 | 0.00                           ||   6 | 0.00                           |\n+-----+--------------------------------++-----+--------------------------------+\n\nSpreading for each iteration is displayed below\nSpread (Ang^2) in `./wannier90.wout`:                                           \n+-----+--------------------------------++-----+--------------------------------+\n|   i | Spread                         ||   i | Spread                         |\n+-----+--------------------------------++-----+--------------------------------+\n|   1 |████████████████████ 86.8       ||  15 |████ 21.4                       |\n|   2 |███████████████████ 86.5        ||  16 |████ 21.4                       |\n|   3 |██████████ 45.8                 ||  17 |████ 21.4                       |\n|   4 |█████ 22.1                      ||  18 |████ 21.4                       |\n|   5 |████ 21.6                       ||  19 |████ 21.4                       |\n|   6 |████ 21.5                       ||  20 |████ 21.4                       |\n|   7 |████ 21.5                       ||  21 |████ 21.4                       |\n|   8 |████ 21.4                       ||  22 |████ 21.4                       |\n|   9 |████ 21.4                       ||  23 |████ 21.4                       |\n|  10 |████ 21.4                       ||  24 |████ 21.4                       |\n|  11 |████ 21.4                       ||  25 |████ 21.4                       |\n|  12 |████ 21.4                       ||  26 |████ 21.4                       |\n|  13 |████ 21.4                       ||  27 |████ 21.4                       |\n|  14 |████ 21.4                       ||  28 |                                |\n+-----+--------------------------------++-----+--------------------------------+\n```\n\n**Arguments for plotting:**\n\n- `ylim` : the limitation of y-axis.\n- `fontfamily` : Font used in plotting. One can also print all the avaible fonts via `--show-fonts`.\n- `fontsize`: Font size used in plotting.\n\n## Example\n\nThe following is a sample folder structure.\nAssuming you are familiar with `Wannier90`, we will not go into detail and you can prepare the necessary files.\nThe working folder of following demonstration of `pyw90` is `tests/GaAs/wannier`\n\n```\ntests/GaAs\n├── bnd\n│   ├── INCAR\n│   ├── KPOINTS  \n│   └── POSCAR\n├── wannier  <-- Current working dir\n│   ├── afolder  \n│   ├── wannier90_input.win\n│   └── wannier90.win \n├── GaAs_mp-2534_primitive.cif\n├── INCAR \n├── KPOINTS\n├── POSCAR\n├── run.script\n└── vasprun.xml\n```\n\n### Show the distribution of eigenvalues via `eig` menu\n\n```bash\n$ pyw90 eig report --path ..\n\nCalculated Energy Range: -1000.0, 1000.0 with Fermi level 3.468000\nEFERMI:  3.468000\n--------------------------------\nBand No.     EMIN        EMAX\n--------------------------------\n  0~  0   -11.34770   -11.25584\n  1~  2   -11.25584   -11.21526\n  3~  4   -11.20921   -11.17821\n  5~  5    -8.90723    -6.59221\n  6~  8    -3.10923    +3.46765\n  9~ 15    +3.61014   +17.33278\n--------------------------------\n```\n\nYou can also add `--separate` argument or use `plot` mode to get the energy ranges of each band and get the figure output `eigenval_dis(_separate).pdf` at current folder.\n\n![](/image/eigenval_dis_cmp.png)\n\nGet `dis_win_min` and `dis_win_max` suggestion as following (you can also input `-w` if you make a guess).\n\n```\n$ pyw90 eig suggest --path ..\n\nCalculated Energy Range: -1000.0, 1000.0 with Fermi level 3.468000\nThere are at most 16 states and at least 16 states in [-1000.0, 1000.0].\n\n`dis_win_min` and `dis_win_max` Table:\n    Column `dis_win_max` shows the **lowest** dis_win_max for `dis_win_min`\n    Column `i+1_min` / `i_max` shows the band minimum / maximum near the gap\n    Column `Nleast`  / `Nmost` shows the least / most number of states inside `dis_win_min` and Fermi level.\n\n   dis_win_min     i+1_min      i_max  Nleast  Nmost\n2    -4.850718   -3.109228  -6.592207       3      3\n1   -10.042721   -8.907233 -11.178209       4      4\n0   -11.212233  -11.209206 -11.215260       6      6\n```\n\n### Show projection suggestion and create `Wannier90` input file\n\nHere, we evaluate the energy ranges with [-1, 1] close to the Fermi level in order to derive the most representative projection recommendation.\n\nYou can also modify the lower selection bound using the `--lb` argument to observe the outputs change. \n\n```\n$ pyw90 pre dos --path .. -e -1 1 --rm-fermi --plot\n\nReading vasprun.xml file from\n    `/path/to/vasprun.xml` \nfor DOS analysis...\n    Fermi level : 3.46800 eV\n    DOS Gap     : 0.46600 eV\n\nCalculated DOS Energy Range: 2.468, 4.468\n\n\n   species  structure_id  orb_id orb_name key_string       dos\n11      As             1       2       pz    As_1_pz  1.000000\n10      As             1       1       py    As_1_py  0.518581\n2       Ga             0       2       pz    Ga_0_pz  0.362974\n12      As             1       3       px    As_1_px  0.333035\n1       Ga             0       1       py    Ga_0_py  0.182324\n3       Ga             0       3       px    Ga_0_px  0.134955\n6       Ga             0       6      dz2   Ga_0_dz2  0.082642\n0       Ga             0       0        s     Ga_0_s  0.043391\n8       Ga             0       8      dx2   Ga_0_dx2  0.029531\n9       As             1       0        s     As_1_s  0.024745\n5       Ga             0       5      dyz   Ga_0_dyz  0.023917\n4       Ga             0       4      dxy   Ga_0_dxy  0.022256\n15      As             1       6      dz2   As_1_dz2  0.011725\n7       Ga             0       7      dxz   Ga_0_dxz  0.011414\n17      As             1       8      dx2   As_1_dx2  0.004456\n13      As             1       4      dxy   As_1_dxy  0.004176\n14      As             1       5      dyz   As_1_dyz  0.004174\n16      As             1       7      dxz   As_1_dxz  0.001948\n\nBased on your input, set the lower selection bound to 0.1 and 6 orbitals are selected.\nNumber of WFs selected: 6 (with degeneracy 1)\n\nOrbitals Selected: \n  species site  orb\n0      Ga   -1  [p]\n1      As   -1  [p]\n\nWannier90 Projection:\nGa:l=1\nAs:l=1\n\npyw90 --extra input:\nGa,0,1-3;As,1,1-3\n\nPlotted with selected orbitals in `brown` and non-selected orbitals in `orange`.\nPlotted with a total of 14 orbitals, 6 of which are selected.\nFigure should be stored at /current/working/folder/dos_analysis.pdf\n```\n\n![](image/dos_analysis.png)\n\nThen we can change the energy ranges to a very large energy ranges such as [-4.85, 20] (-4.85 is obtained from the previous result from `eig` menu).\n\n```\n$ pyw90 pre dos --path .. -e -4.85 20 --extra 'Ga,0,1-3;As,1,1-3'\n\nCalculated DOS Energy Range: -4.85, 20.0\n\n/public/home/enwang/pyw90/pyw90/lib/dos.py:294: UserWarning: CHECK YOUR INPUT! The energies in `EIGENVAL` is ranged from -15.0 to 15.0, which does not include all the energy ranged from -4.85 to 20.0 you input.\n  warnings.warn(f'CHECK YOUR INPUT! The energies in `EIGENVAL` is ranged from {ee.min()} to {ee.max()}, ' \\\n    WANRING: There are 1 states between given `emin`: -4.85 and lowest `dis_froz_min`: -11.174209000000001. \n    Please carefully consider the suggestion of dis frozen window and double-check energy ranges of each band.\n    This is a frequent occurrence in no-SOC systems with numerous denegeracy point.\n    However, we still want to provide you with some alternative energy window options.\n\nDis frozen window table\nThe table is sorted according to the percentage of pdos/tdos.\nIf you want to see `dis_win_min(max)` suggestion, please use `pyw90 eig suggest` menu.\n   dis_froz_min  dis_froz_max  N      pdos       tdos   percent\n5     -4.850000      7.174749  5  3.343966   8.991494  0.371903\n1      3.471648     10.658571  4  2.112846   6.822463  0.309690\n4      7.464314     18.000000  6  3.166871  10.782830  0.293696\n3      3.471649     12.386890  6  3.098248  10.639050  0.291215\n2      3.471649     12.060069  5  3.160086  11.136491  0.283760\n0    -11.174209      7.174749  6  2.312163  13.604458  0.169956\n\nLowest `dis_win_max` for -4.85: 13.098955\n```\nThus, an initial guess of the Wannier function was obtained.\nThen, we can seek the `wannier90.win` template for the `Wannier90` and `VASP` interface using `pyw90 pre template --extra basic`.\n\nSince `VASP` (<6.0) only supports `Wannier90` with version 1.2. You may modify and recompile `VASP` so that it can calculate non-collinear Wannier functions and support spinor projection method. For further details, please refer to [Chengcheng-Xiao/VASP2WAN90_v2_fix: An updated version of the VASP2WANNIER90v2 interface](https://github.com/Chengcheng-Xiao/VASP2WAN90_v2_fix).\n\n```\nnum_wann  = 6\n# num_bands = 15\n\nexclude_bands : 1-5\n\nbegin projections\nGa:l=1\nAs:l=1\nend projections\n\n# spinors = .true.\n```\n\nThis `wannier90.win` should be created in `GaAs/wannier` folder. You also have to set `LWANNIER90 = .TRUE.` in `VASP` to interface between `VASP` and `Wannier90`.\nThis feature is only present if VASP is compiled with `-DVASP2WANNIER90` or `-DVASP2WANNIER90v2`. \n\nOther inputs is set automatically based on the `VASP` calculation, such as `kpoints`, `atoms`, `unit_cell`, `mp_grid` etc.\n\n> With VASP (>= 6.2.0), it will support `Wannier90` >=3.0. And the `wannier90.win` input can also directly input via `INCAR` with `WANNIER90_WIN` (See [WANNIER90_WIN - Vaspwiki](https://www.vasp.at/wiki/index.php/WANNIER90_WIN)) and no more initial `wannier90.win` file needed.\n\nAfter executing the task, `VASP` will write the input files for a preceeding `WANNIER90` run: `wannier90.win`, `wannier90.mmn`, `wannier90.eig` and `wannier90.amn`.\n\nHere we write the initial guess of dis energy window and band structure calculation card into `wannier90.win` file. The `Kpoint_Path` block can be obtained from `pyw90 pre kpath --path ../bnd`.\n\n```\n# disentanglement and wannierization\ndis_win_max       = 13.098955\ndis_froz_max      =  7.174749\ndis_froz_min      = -4.86\ndis_win_min       = -4.85\n\nnum_iter          = 1000\nnum_print_cycles  =   40\ndis_num_iter      = 5000\ndis_mix_ratio     =  1.0\n\n# Band Plot  \n# restart = plot\nwrite_hr          = true\nbands_plot        = true\nbands_num_points  = 151 \nbands_plot_format = gnuplot\n\nBegin Kpoint_Path\nEnd Kpoint_Path\n```\n\nThen we can use the `pyw90 auto` menu to optimize the dis energy window automatically.\nThe configuration file `auto_w90_input.yaml` should be generated using `pyw90 auto input`.\n**Customize the configuration file before running a calculation.**\n(see the `auto` menu's documentation for the meaning of each key)\n\nAfter preparing all input, type `pyw90 auto run` to execute the procedure.\nThere are two output files.\n\n- `auto_w90_output.txt`: save the stdout output.\n- `log_autow90_{timestamp you submit}.log`: record the complete process of the 'Wannier90' input.\n\nExecute `pyw90 auto term` and follow the instructions to kill all processes to terminate the automated task. \n\n###  Show quality of Wannier functions\n\nFigure `{name}_VASP_W90_cmp.pdf` will be generated with both `VASP` and `Wannier90` band structure plotted. You can also use `--config` to read the `efermi` and `kernel` parameters from configuration file `auto_w90_input.yaml` directly.\n\n![](image/GaAs_VASP_W90_cmp.png)\n\n```\n$ pyw90 cmp GaAs --efermi 3.468 --kernel unit,3.5,1\n\nReading Data from .\nThe output figure should be stored at\n    /current/working/folder/GaAs_VASP_W90_cmp.png\nFinal Quality 0.324071 meV with dEs for each bands\n+-----+--------------------------------++-----+--------------------------------+\n|   i | MAX DIFF (meV)                 ||   i | AVERAGE DIFF (meV)             |\n+-----+--------------------------------++-----+--------------------------------+\n|   1 |████ 0.36                       ||   1 |██████ 0.12                     |\n|   2 |████████████ 1.10               ||   2 |█████████████████████ 0.36      |\n|   3 |██████████████████████ 1.88     ||   3 |██████████████████████ 0.38     |\n|   4 |███████████████ 1.32            ||   4 |██████████████ 0.25             |\n|   5 | 0.00                           ||   5 | 0.00                           |\n|   6 | 0.00                           ||   6 | 0.00                           |\n+-----+--------------------------------++-----+--------------------------------+\n\nSpreading for each iteration is displayed below\nSpread (Ang^2) in `wannier90.wout`:                                             \n+-----+--------------------------------++-----+--------------------------------+\n|   i | Spread                         ||   i | Spread                         |\n+-----+--------------------------------++-----+--------------------------------+\n|   1 |████████████████████ 86.8       ||  15 |████ 21.4                       |\n|   2 |███████████████████ 86.5        ||  16 |████ 21.4                       |\n|   3 |██████████ 45.8                 ||  17 |████ 21.4                       |\n|   4 |█████ 22.1                      ||  18 |████ 21.4                       |\n|   5 |████ 21.6                       ||  19 |████ 21.4                       |\n|   6 |████ 21.5                       ||  20 |████ 21.4                       |\n|   7 |████ 21.5                       ||  21 |████ 21.4                       |\n|   8 |████ 21.4                       ||  22 |████ 21.4                       |\n|   9 |████ 21.4                       ||  23 |████ 21.4                       |\n|  10 |████ 21.4                       ||  24 |████ 21.4                       |\n|  11 |████ 21.4                       ||  25 |████ 21.4                       |\n|  12 |████ 21.4                       ||  26 |████ 21.4                       |\n|  13 |████ 21.4                       ||  27 |████ 21.4                       |\n|  14 |████ 21.4                       ||  28 |                                |\n+-----+--------------------------------++-----+--------------------------------+\n```",
     'author': 'En Wang (Cloudiiink)',
     'author_email': 'wangenzj@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Cloudiiink/pyw90',
```

### Comparing `pyw90-1.0.6/PKG-INFO` & `pyw90-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyw90
-Version: 1.0.6
+Version: 1.0.7
 Summary: A VASP and Wannier90 interfaced tool for projection analysis and fully automated dis energy window optimization.
 Home-page: https://github.com/Cloudiiink/pyw90
 License: GPL-3.0-only
 Keywords: python,vasp,wannier90,tight-binding,solid-state-physics
 Author: En Wang (Cloudiiink)
 Author-email: wangenzj@gmail.com
 Requires-Python: >=3.8,<3.12
```

