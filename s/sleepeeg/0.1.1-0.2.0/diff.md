# Comparing `tmp/sleepeeg-0.1.1.tar.gz` & `tmp/sleepeeg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.1.1.tar", last modified: Tue May  9 13:32:46 2023, max compression
+gzip compressed data, was "sleepeeg-0.2.0.tar", last modified: Tue Jun  6 06:18:47 2023, max compression
```

## Comparing `sleepeeg-0.1.1.tar` & `sleepeeg-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.368809 sleepeeg-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1966 2023-05-09 13:32:46.367812 sleepeeg-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1696 2023-05-09 11:39:44.000000 sleepeeg-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.339886 sleepeeg-0.1.1/docs/
--rw-rw-rw-   0        0        0     1302 2023-03-20 20:54:05.000000 sleepeeg-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0      660 2023-05-09 13:32:29.000000 sleepeeg-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 13:32:46.368809 sleepeeg-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      241 2023-03-26 21:13:28.000000 sleepeeg-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.343876 sleepeeg-0.1.1/sleepeeg/
--rw-rw-rw-   0        0        0    49799 2023-05-09 13:10:00.000000 sleepeeg-0.1.1/sleepeeg/base.py
--rw-rw-rw-   0        0        0    23551 2023-05-09 13:20:03.000000 sleepeeg-0.1.1/sleepeeg/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:46.366814 sleepeeg-0.1.1/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1966 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-09 13:32:46.000000 sleepeeg-0.1.1/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.666786 sleepeeg-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1422 2023-06-06 06:18:47.665789 sleepeeg-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-06-06 06:12:40.000000 sleepeeg-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.635870 sleepeeg-0.2.0/docs/
+-rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0      861 2023-06-06 06:07:20.000000 sleepeeg-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:18:47.666786 sleepeeg-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.645843 sleepeeg-0.2.0/sleepeeg/
+-rw-rw-rw-   0        0        0    47580 2023-06-05 11:10:20.000000 sleepeeg-0.2.0/sleepeeg/base.py
+-rw-rw-rw-   0        0        0     9796 2023-06-06 05:52:35.000000 sleepeeg-0.2.0/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    24536 2023-06-05 13:36:04.000000 sleepeeg-0.2.0/sleepeeg/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:18:47.663795 sleepeeg-0.2.0/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1422 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-06 06:18:47.000000 sleepeeg-0.2.0/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.1.1/LICENSE` & `sleepeeg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.1.1/PKG-INFO` & `sleepeeg-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.1.1
+Version: 0.2.0
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
+Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
+Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
+Keywords: sleep,eeg
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sleep-eeg-processing
-**sleepeeg** is a high-level API built on top of [mne-python](https://mne.tools/stable/index.html) for preprocessing and analysis of sleep EEG data.
+# sleepeeg
+**sleepeeg** is a high-level package built on top of [mne-python](https://mne.tools/stable/index.html), [yasa](https://raphaelvallat.com/yasa/build/html/index.html) for preprocessing and analysis of sleep EEG data.
 ## Installation
-0. Make sure you have [Python](https://www.python.org/downloads/) installed.
-    - The script was tested with the version 3.10.9
-    - Python 3.11.x currently isn't supported because of the yasa's dependency on the numba library.
+0. Make sure you have [Python](https://www.python.org/downloads/) version installed. Requires Python 3.10 or higher.
 1. Create a Python virtual environment, for more info you can refer to python [venv](https://docs.python.org/3/tutorial/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) or [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 2. Activate the environment
 3. 
     ```
     pip install sleepeeg
     ```
-4. (Optional, but recommended) [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleep-eeg-processing/tree/main/notebooks) notebooks.
-5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/). After installation, to permanently enable CUDA use, do: 
-    ```
-    mne.utils.set_config('MNE_USE_CUDA', 'true')
-    ```
-6. (Optional) For OpenGL acceleration of [MNE plot](https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.plot) install [pyopengl](https://pyopengl.sourceforge.net/documentation/installation.html) and use `plot(use_opengl=True)`.
+4. [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleepeeg/tree/main/notebooks) notebooks.
 
 ## Quickstart
 1. Open any of the downloaded notebooks using the created environment.
 2. Follow the notebook's instructions.
```

### Comparing `sleepeeg-0.1.1/README.md` & `sleepeeg-0.2.0/sleepeeg.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-# sleep-eeg-processing
-**sleepeeg** is a high-level API built on top of [mne-python](https://mne.tools/stable/index.html) for preprocessing and analysis of sleep EEG data.
+Metadata-Version: 2.1
+Name: sleepeeg
+Version: 0.2.0
+Summary: Sleep EEG preprocessing and analysis
+Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
+License: MIT
+Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
+Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
+Keywords: sleep,eeg
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sleepeeg
+**sleepeeg** is a high-level package built on top of [mne-python](https://mne.tools/stable/index.html), [yasa](https://raphaelvallat.com/yasa/build/html/index.html) for preprocessing and analysis of sleep EEG data.
 ## Installation
-0. Make sure you have [Python](https://www.python.org/downloads/) installed.
-    - The script was tested with the version 3.10.9
-    - Python 3.11.x currently isn't supported because of the yasa's dependency on the numba library.
+0. Make sure you have [Python](https://www.python.org/downloads/) version installed. Requires Python 3.10 or higher.
 1. Create a Python virtual environment, for more info you can refer to python [venv](https://docs.python.org/3/tutorial/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) or [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 2. Activate the environment
 3. 
     ```
     pip install sleepeeg
     ```
-4. (Optional, but recommended) [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleep-eeg-processing/tree/main/notebooks) notebooks.
-5. (Optional, but recommended) Prepare [GPU acceleration](https://mne.tools/stable/install/advanced.html#gpu-acceleration-with-cuda) by installing [CUDA](https://developer.nvidia.com/cuda-downloads) and [CuPy](https://cupy.dev/). After installation, to permanently enable CUDA use, do: 
-    ```
-    mne.utils.set_config('MNE_USE_CUDA', 'true')
-    ```
-6. (Optional) For OpenGL acceleration of [MNE plot](https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.plot) install [pyopengl](https://pyopengl.sourceforge.net/documentation/installation.html) and use `plot(use_opengl=True)`.
+4. [Download](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/NirLab-TAU/sleepeeg/tree/main/notebooks) notebooks.
 
 ## Quickstart
 1. Open any of the downloaded notebooks using the created environment.
-2. Follow the notebook's instructions.
+2. Follow the notebook's instructions.
```

### Comparing `sleepeeg-0.1.1/pyproject.toml` & `sleepeeg-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,30 +3,37 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
+keywords = ['sleep', 'eeg']
 dependencies = [
     "attrs",
-    "mne",
+    "mne>=1.4.1",
     "mne-qt-browser",
     "pyqt5",
     "yasa==0.6.3",
     "lspopt",
     "ipympl",
-    "numpy",
+    "numpy<=1.23.5",
     "pandas",
     "scipy",
     "fooof",
     "natsort",
-    "more-itertools"
-]
+    "more-itertools",
+    "h5io",
+    "loguru"
+]
+
+[project.urls]
+Homepage = "https://github.com/NirLab-TAU/sleepeeg"
+Documentation = "https://nirlab-tau.github.io/sleepeeg/"
```

### Comparing `sleepeeg-0.1.1/sleepeeg/base.py` & `sleepeeg-0.2.0/sleepeeg/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 import os
 import errno
+import inspect
 
+from loguru import logger
+import yaml
+import json
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from pathlib import Path
+import functools
 
 from typing import TypeVar, Type
 from attrs import define, field
 
 import matplotlib.pyplot as plt
 import numpy as np
 import mne
 from tqdm import tqdm
 
 # For type annotation of pipe elements.
 BasePipeType = TypeVar("BasePipeType", bound="BasePipe")
 
 
+def logger_wraps(*, level="DEBUG"):
+    def wrapper(func):
+        name = func.__name__
+
+        @functools.wraps(func)
+        def wrapped(self, *args, **kwargs):
+            logger_ = logger.opt(depth=1)
+            logger_.log(
+                level,
+                f"Entering '{self.__class__.__name__}.{name}' (args={args}, kwargs={kwargs})",
+            )
+            result = func(self, *args, **kwargs)
+
+            return result
+
+        return wrapped
+
+    return wrapper
+
+
 @define(kw_only=True, slots=False)
 class BasePipe(ABC):
     """A template class for the pipeline segments."""
 
-    prec_pipe: Type[BasePipeType] = field(default=None, metadata={"my_metadata": 1})
-    """Preceding pipe that hands over mne_raw attr."""
+    prec_pipe: Type[BasePipeType] = field(default=None)
+    """Preceding pipe that hands over mne_raw attribute."""
 
     path_to_eeg: Path = field(converter=Path)
-    """Can be any file type supported by 
-    `mne.io.read_raw() <https://mne.tools/stable/generated/
-    mne.io.Raw.html#mne.io.Raw.save>`_.
+    """Can be any file type supported by :py:func:`mne:mne.io.read_raw`.
     """
 
     @path_to_eeg.default
     def _set_path_to_eeg(self):
         if self.prec_pipe:
-            return "/"
+            return self.prec_pipe.path_to_eeg
         raise TypeError('Provide either "pipe" or "path_to_eeg" arguments')
 
     @path_to_eeg.validator
     def _validate_path_to_eeg(self, attr, value):
         if not value.exists():
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), value)
 
@@ -50,71 +73,57 @@
             self.prec_pipe.output_dir if self.prec_pipe else self.path_to_eeg.parents[0]
         )
 
     @output_dir.validator
     def _validate_output_dir(self, attr, value):
         self.output_dir.mkdir(exist_ok=True)
         (self.output_dir / self.__class__.__name__).mkdir(exist_ok=True)
+        logger.remove()
+        logger.add(self.output_dir / "pipeline.log")
 
     mne_raw: mne.io.Raw = field(init=False)
-    """An instanse of  
-    `mne.io.Raw <https://mne.tools/stable/generated/
-    mne.io.Raw.html#mne-io-raw>`_.
+    """An instanse of :py:class:`mne:mne.io.Raw`.
     """
 
     @mne_raw.default
     def _read_mne_raw(self):
-        from mne.io import read_raw
-
-        try:
-            return (
-                self.prec_pipe.mne_raw if self.prec_pipe else read_raw(self.path_to_eeg)
-            )
-        except Exception as err:
-            print(f"Unexpected {err=}, {type(err)=}")
-            raise
+        if self.prec_pipe:
+            return self.prec_pipe.mne_raw
+        else:
+            return mne.io.read_raw(self.path_to_eeg)
 
     @property
     def sf(self):
-        """A wrapper for
-        `mne.Info["sfreq"] <https://mne.tools/stable/generated/
-        mne.Info.html#mne-info>`_.
+        """A wrapper for :py:class:`raw.info["sfreq"] <mne:mne.Info>`.
 
         Returns:
             float: sampling frequency
         """
         return self.mne_raw.info["sfreq"]
 
     def plot(
         self,
         save_annotations: bool = False,
         save_bad_channels: bool = False,
         overwrite: bool = False,
-        mne_plot_args: dict = None,
+        **kwargs,
     ):
-        """A wrapper for `mne.io.Raw.plot() <https://mne.tools/stable/
-        generated/mne.io.Raw.html#mne.io.Raw.plot>`_.
+        """A wrapper for :py:meth:`mne:mne.io.Raw.plot`.
 
         Args:
-            butterfly: Whether to start in butterfly mode. Defaults to False.
             save_annotations: Whether to save annotations as txt. Defaults to False.
             save_bad_channels: Whether to save bad channels as txt. Defaults to False.
-            scalings: Scale for amplitude per channel type. Defaults to 'auto'.
-            use_opengl: Whether to use OpenGL acceleration. Defaults to None.
             overwrite: Whether to overwrite annotations and bad_channels files if exist.
                 Defaults to False.
-            mne_plot_args: Arguments passed to `raw.plot() <https://mne.tools/stable/
-                generated/mne.io.Raw.html#mne.io.Raw.plot>`_. Defaults to None.
+            **kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.plot`.
         """
-        mne_plot_args = mne_plot_args or dict()
-        mne_plot_args.setdefault("theme", "dark")
-        mne_plot_args.setdefault("block", True)
-        mne_plot_args.setdefault("bad_color", "r")
-        mne_plot_args.setdefault("scalings", "auto")
-        self.mne_raw.plot(**mne_plot_args)
+        kwargs.setdefault("theme", "dark")
+        kwargs.setdefault("bad_color", "r")
+        kwargs.setdefault("scalings", "auto")
+        self.mne_raw.plot(**kwargs)
 
         if save_annotations:
             self.mne_raw.annotations.save(
                 self.output_dir / self.__class__.__name__ / "annotations.txt",
                 overwrite=overwrite,
             )
         if save_bad_channels:
@@ -130,177 +139,81 @@
                 ) as f:
                     f.seek(0)
                     bads = f.read().split()
                     for bad in self.mne_raw.info["bads"]:
                         if bad not in bads:
                             f.write(f"{bad}\n")
 
-    def _plot_sensors(
-        self,
-        ch_colors=None,
-        kind="topomap",
-        ch_type=None,
-        title=None,
-        show_names=False,
-        ch_groups=None,
-        to_sphere=True,
-        axes=None,
-        block=False,
-        show=False,
-        sphere=None,
-        pointsize=7,
-        linewidth=1,
+    def plot_sensors(
+        self, legend: Iterable[str] = None, legend_args: dict = None, **kwargs
     ):
-        from mne.viz.evoked import _rgb
-        from mne.viz.utils import _plot_sensors
-        from mne.defaults import _handle_default
-        from mne.io.constants import FIFF
-        from mne.io.pick import (
-            channel_type,
-            channel_indices_by_type,
-            pick_channels,
-            _DATA_CH_TYPES_SPLIT,
-            _contains_ch_type,
-        )
-        from mne.utils import _check_ch_locs, _check_option, warn
-        from mne.transforms import apply_trans
-
-        info = self.mne_raw.info
-        _check_option("kind", kind, ["topomap", "3d", "select"])
-        if not isinstance(info, mne.io.Info):
-            raise TypeError(f"info must be an instance of Info not {type(info)}")
-        ch_indices = channel_indices_by_type(info)
-        allowed_types = _DATA_CH_TYPES_SPLIT
-        if ch_type is None:
-            for this_type in allowed_types:
-                if _contains_ch_type(info, this_type):
-                    ch_type = this_type
-                    break
-            picks = ch_indices[ch_type]
-        elif ch_type == "all":
-            picks = list()
-            for this_type in allowed_types:
-                picks += ch_indices[this_type]
-        elif ch_type in allowed_types:
-            picks = ch_indices[ch_type]
-        else:
-            raise ValueError(f"ch_type must be one of {allowed_types} not {ch_type}!")
+        """A wrapper for :py:func:`mne:mne.viz.plot_sensors` with a legend.
 
-        if len(picks) == 0:
-            raise ValueError(f"Could not find any channels of type {ch_type}.")
+        Args:
+            legend: ch_groups names to connect to colors. Defaults to None.
+            legend_args: Arguments passed to :py:meth:`mpl:matplotlib.axes.Axes.legend`.
+                Defaults to None.
+            **kwargs: Arguments passed to :py:func:`mne:mne.viz.plot_sensors`.
+        """
+        import matplotlib.patches as mpatches
 
-        if not _check_ch_locs(info=info, picks=picks):
-            raise RuntimeError("No valid channel positions found")
+        legend_args = legend_args or dict()
 
-        dev_head_t = info["dev_head_t"]
-        chs = [info["chs"][pick] for pick in picks]
-        pos = np.empty((len(chs), 3))
-        for ci, ch in enumerate(chs):
-            pos[ci] = ch["loc"][:3]
-            if ch["coord_frame"] == FIFF.FIFFV_COORD_DEVICE:
-                if dev_head_t is None:
-                    warn(
-                        "dev_head_t is None, transforming MEG sensors to head "
-                        "coordinate frame using identity transform"
-                    )
-                    dev_head_t = np.eye(4)
-                pos[ci] = apply_trans(dev_head_t, pos[ci])
-        del dev_head_t
-
-        ch_names = np.array([ch["ch_name"] for ch in chs])
-        bads = [idx for idx, name in enumerate(ch_names) if name in info["bads"]]
-        ch_colors = {} if not ch_colors else ch_colors
-        if ch_groups is None:
-            def_colors = _handle_default("color")
-            colors = [
-                ch_colors[self.mne_raw.info.ch_names[pick]]
-                if self.mne_raw.info.ch_names[pick] in ch_colors
-                else def_colors[channel_type(info, pick)]
-                for i, pick in enumerate(picks)
-            ]
-        else:
-            if ch_groups in ["position", "selection"]:
-                # Avoid circular import
-                from mne.channels import (
-                    read_vectorview_selection,
-                    _SELECTIONS,
-                    _EEG_SELECTIONS,
-                    _divide_to_regions,
-                )
-
-                if ch_groups == "position":
-                    ch_groups = _divide_to_regions(info, add_stim=False)
-                    ch_groups = list(ch_groups.values())
-                else:
-                    ch_groups, color_vals = list(), list()
-                    for selection in _SELECTIONS + _EEG_SELECTIONS:
-                        channels = pick_channels(
-                            info["ch_names"],
-                            read_vectorview_selection(selection, info=info),
-                        )
-                        ch_groups.append(channels)
-                color_vals = np.ones((len(ch_groups), 4))
-                for idx, ch_group in enumerate(ch_groups):
-                    color_picks = [
-                        np.where(picks == ch)[0][0] for ch in ch_group if ch in picks
-                    ]
-                    if len(color_picks) == 0:
-                        continue
-                    x, y, z = pos[color_picks].T
-                    color = np.mean(_rgb(x, y, z), axis=0)
-                    color_vals[idx, :3] = color  # mean of spatial color
-            else:
-                import matplotlib.pyplot as plt
+        ch_groups = kwargs.pop("ch_groups", None)
+        axes = kwargs.pop("axes", None)
+        kwargs.setdefault("show", False)
 
-                colors = np.linspace(0, 1, len(ch_groups))
-                color_vals = [plt.cm.jet(colors[i]) for i in range(len(ch_groups))]
-            if not isinstance(ch_groups, (np.ndarray, list)):
+        fig = mne.viz.plot_sensors(
+            self.mne_raw.info, ch_groups=ch_groups, axes=axes, **kwargs
+        )
+        if axes is None:
+            axes = fig.axes[0]
+        if legend:
+            if not len(legend) == len(ch_groups):
                 raise ValueError(
-                    "ch_groups must be None, 'position', "
-                    "'selection', or an array. Got %s." % ch_groups
+                    "Length of the legend and of the ch_groups should be equal"
                 )
-            colors = np.zeros((len(picks), 4))
-            for pick_idx, pick in enumerate(picks):
-                for ind, value in enumerate(ch_groups):
-                    if pick in value:
-                        colors[pick_idx] = color_vals[ind]
-                        break
-        title = "Sensor positions (%s)" % ch_type if title is None else title
-        fig = _plot_sensors(
-            pos,
-            info,
-            picks,
-            colors,
-            bads,
-            ch_names,
-            title,
-            show_names,
-            axes,
-            show,
-            kind,
-            block,
-            to_sphere,
-            sphere,
-            pointsize=pointsize,
-            linewidth=linewidth,
-        )
 
-        if kind == "select":
-            return fig, fig.lasso.selection
+            patches = []
+            # if legend:
+            colors = np.linspace(0, 1, len(ch_groups))
+            color_vals = [plt.cm.jet(colors[i]) for i in range(len(ch_groups))]
+            for i, color in enumerate(color_vals):
+                if legend[i]:
+                    patches.append(mpatches.Patch(color=color, label=legend[i]))
+            if self.mne_raw.info["bads"]:
+                patches.append(mpatches.Patch(color="red", label="Bad"))
+            axes.legend(handles=patches, **legend_args)
         return fig
 
-    def save_raw(self, fname: str):
-        """A wrapper for `mne.io.Raw.save <https://mne.tools/stable/
-        generated/mne.io.Raw.html#mne.io.Raw.save>`_.
+    @logger_wraps()
+    def save_raw(self, fname: str, **kwargs):
+        """A wrapper for :py:meth:`mne:mne.io.Raw.save`.
 
         Args:
-            fname: filename for the fif file being saved.
+            fname: Filename for the fif file being saved.
+            **kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.save`.
         """
         fif_folder = self.output_dir / self.__class__.__name__
-        self.mne_raw.save(fif_folder / fname)
+        self.mne_raw.save(fif_folder / fname, **kwargs)
+
+    @logger_wraps()
+    def set_eeg_reference(self, ref_channels="average", projection=False, **kwargs):
+        """A wrapper for :py:meth:`mne:mne.io.Raw.set_eeg_reference`.
+
+        Args:
+            ref_channels: :py:meth:`ref_channels <mne:mne.io.Raw.set_eeg_reference>`. Defaults to 'average'.
+            projection: :py:meth:`projection <mne:mne.io.Raw.set_eeg_reference>`. Defaults to False.
+            **kwargs: Additional arguments passed to :py:meth:`mne:mne.io.Raw.set_eeg_reference`.
+        """
+        if not projection:
+            logger.info(f"{ref_channels} reference has been applied")
+        self.mne_raw.load_data().set_eeg_reference(
+            ref_channels=ref_channels, projection=projection, **kwargs
+        )
 
 
 @define(kw_only=True, slots=False)
 class BaseHypnoPipe(BasePipe, ABC):
     """A template class for the sleep stage analysis pipeline segments."""
 
     path_to_hypno: Path = field(converter=Path)
@@ -362,30 +275,31 @@
     def __upsample_hypno(self):
         from yasa import hypno_upsample_to_data
 
         self.hypno_up = hypno_upsample_to_data(
             self.hypno, self.hypno_freq, self.mne_raw, verbose=False
         )
 
+    @logger_wraps()
     def predict_hypno(
         self,
         eeg_name: str = "E183",
         eog_name: str = "E252",
         emg_name: str = "E247",
         ref_name: str = "E26",
-        save=True,
+        save: bool = True,
     ):
         """Runs YASA's automatic sleep staging
 
         Args:
             eeg_name: Preferentially a central electrode. Defaults to "E183".
             eog_name: Preferentially, the left LOC channel. Defaults to "E252".
             emg_name: Preferentially a chin electrode. Defaults to "E247".
             ref_name: Reference channel, preferentially a mastoid. Defaults to "E26".
-            save: Whether to save the hypnogram. Defaults to True.
+            save: Whether to save the hypnogram to file. Defaults to True.
         """
         from yasa import SleepStaging, hypno_str_to_int
 
         sls = SleepStaging(
             self.mne_raw.copy().load_data().set_eeg_reference(ref_channels=[ref_name]),
             eeg_name=eeg_name,
             eog_name=eog_name,
@@ -405,16 +319,15 @@
             plt.savefig(
                 self.output_dir
                 / self.__class__.__name__
                 / "predicted_hypno_probabilities.png"
             )
 
     def sleep_stats(self, save: bool = False):
-        """A wrapper for
-        `yasa.sleep_statistics <https://raphaelvallat.com/yasa/build/html/generated/yasa.sleep_statistics.html#yasa-sleep-statistics>`_.
+        """A wrapper for :py:func:`yasa:yasa.sleep_statistics`.
 
         Args:
             save: Whether to save the stats to csv. Defaults to False.
         """
 
         from yasa import sleep_statistics
         from csv import DictWriter
@@ -462,23 +375,24 @@
 @define(kw_only=True, slots=False)
 class BaseEventPipe(BaseHypnoPipe, BaseTopomap, ABC):
     """A template class for event detection."""
 
     results = field(init=False)
     """Event detection results as returned by YASA's event detection methods. 
     Depending on the child class can be instance of either 
-    SpindlesResults, SWResults or REMResults classes. 
+    :py:class:`yasa:yasa.SpindlesResults`, :py:class:`yasa:yasa.SWResults` or :py:class:`yasa:yasa.REMResults` classes. 
     """
 
     tfrs: dict = field(init=False)
-    """Instances of mne.time_frequency.AverageTFR per sleep stage.
+    """Instances of :py:class:`mne:mne.time_frequency.AverageTFR` per sleep stage.
     """
 
     @abstractmethod
     def detect():
+        """Each event class should contain the detection method"""
         pass
 
     def _save_to_csv(self):
         self.results.summary().to_csv(
             self.output_dir
             / self.__class__.__name__
             / f"{self.__class__.__name__[:-4].lower()}.csv",
@@ -488,26 +402,27 @@
     def _save_avg_fig(self):
         plt.savefig(
             self.output_dir
             / self.__class__.__name__
             / f"{self.__class__.__name__[:-4].lower()}_avg.png"
         )
 
-    def plot_average(self, save: bool = False, yasa_args=None):
-        """Average of YASA's detected event.
+    @logger_wraps()
+    def plot_average(self, save: bool = False, **kwargs):
+        """Plot average of the detected event.
 
         Args:
             save: Whether to save the figure to file. Defaults to False.
-            yasa_args: Arguments passed to the YASA's plot_average(). Defaults to None.
+            **kwargs: Arguments passed to the YASA's plot_average().
         """
-        yasa_args = yasa_args or dict()
-        self.results.plot_average(**yasa_args)
+        self.results.plot_average(**kwargs)
         if save:
             self._save_avg_fig()
 
+    @logger_wraps()
     def plot_topomap(
         self,
         prop: str,
         stage: str = "N2",
         aggfunc: str = "mean",
         sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         axis: plt.axis = None,
@@ -520,20 +435,20 @@
 
         Args:
             prop: Any event property returned by self.results.summary().
             stage: One of the sleep_stages keys. Defaults to "N2".
             aggfunc: Averaging function, "mean" or "median". Defaults to "mean".
             sleep_stages: Mapping between sleep stages names and their integer representations.
                 Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
+            axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_.
-                Defaults to "plasma".
             save: Whether to save the figure. Defaults to False.
+            topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
+            cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
+            subplots_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.subplots`.Defaults to None.
         """
         from natsort import natsort_keygen
         from more_itertools import collapse
         from seaborn import color_palette
 
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
@@ -576,14 +491,15 @@
         if save and is_new_axis:
             fig.savefig(
                 self.output_dir
                 / self.__class__.__name__
                 / f"topomap_{self.__class__.__name__[:-4].lower()}_{prop.lower()}.png"
             )
 
+    @logger_wraps()
     def plot_topomap_collage(
         self,
         props: Iterable[str],
         aggfunc: str = "mean",
         stages_to_plot: tuple = "all",
         sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         low_percentile: float = 5,
@@ -604,20 +520,17 @@
             sleep_stages: Mapping between sleep stages names and their integer representations.
                 Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
             low_percentile: Set min color value by percentile of the property data.
                 Defaults to 5.
             high_percentile: Set max color value by percentile of the property data.
                 Defaults to 95.
             save: Whether to save the figure. Defaults to False.
-            topomap_args: Arguments passed to `mne.viz.plot_topomap() <https://mne.tools/
-                stable/generated/mne.viz.plot_topomap.html>`_. Defaults to None.
-            cbar_args: Arguments passed to `plt.colorbar() <https://matplotlib.org/stable
-                /api/_as_gen/matplotlib.pyplot.colorbar.html>`_. Defaults to None.
-            figure_args: Arguments passed to `plt.figure() <https://matplotlib.org/stable/
-                api/_as_gen/matplotlib.pyplot.figure.html>`_. Defaults to None.
+            topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
+            cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
+            figure_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.figure`.Defaults to None.
 
         """
         from natsort import natsort_keygen
         from more_itertools import collapse
 
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
@@ -712,37 +625,36 @@
         if save:
             fig.savefig(
                 self.output_dir
                 / self.__class__.__name__
                 / f"topomap_{self.__class__.__name__[:-4].lower()}_collage.png"
             )
 
+    @logger_wraps()
     def apply_tfr(
         self,
         freqs: Iterable[float],
         n_freqs: int,
         time_before: float,
         time_after: float,
         method: str = "morlet",
         save: bool = False,
-        tfr_method_args: dict = None,
+        **tfr_kwargs,
     ):
         """Transforms the events signal to time-frequency representation.
 
         Args:
             freqs: Lower and upper bounds of frequencies of interest in Hz, e.g., (10,20)
             n_freqs: Frequency resolution in TFR.
             time_before: Seconds before the event peak to get from the real data.
             time_after: Seconds after the event peak to get from the real data
             method: TFR transform method. Defaults to "morlet".
             save: Whether to save the TFRs to file. Defaults to False.
-            tfr_method_args: Arguments passed to `mne.time_frequency.tfr_array_morlet()
-                <https://mne.tools/stable/generated/mne.time_frequency.tfr_array_morlet.html>`_
-                or `mne.time_frequency.tfr_array_multitaper() <https://mne.tools/stable/
-                generated/mne.time_frequency.tfr_array_multitaper.html>`_. Defaults to None.
+            **tfr_kwargs: Arguments passed to :py:func:`mne:mne.time_frequency.tfr_array_morlet`
+                or :py:func:`mne:mne.time_frequency.tfr_array_multitaper`.
         """
         assert self.results, "Run detect method first"
         assert (
             method == "morlet" or method == "multitaper"
         ), "method should be 'morlet' or 'multitaper'"
         from natsort import natsorted
 
@@ -752,18 +664,17 @@
             0: "Wake",
             1: "N1",
             2: "N2",
             3: "N3",
             4: "REM",
         }
 
-        tfr_method_args = tfr_method_args or dict()
-        tfr_method_args.setdefault("n_jobs", -1)
-        tfr_method_args.setdefault("verbose", "error")
-        tfr_method_args["output"] = "avg_power"
+        tfr_kwargs.setdefault("n_jobs", -1)
+        tfr_kwargs.setdefault("verbose", "error")
+        tfr_kwargs["output"] = "avg_power"
 
         freqs = np.linspace(freqs[0], freqs[1], n_freqs)
         df_raw = self.results.get_sync_events(
             time_before=time_before, time_after=time_after
         )[["Event", "Amplitude", "Channel", "Stage"]]
 
         self.tfrs = {}
@@ -791,32 +702,34 @@
             # Calculate tfrs
             if method == "morlet":
                 tfrs = {
                     channel: mne.time_frequency.tfr_array_morlet(
                         v,
                         self.sf,
                         freqs,
-                        **tfr_method_args,
+                        **tfr_kwargs,
                     )
                     for channel, v in tqdm(for_tfrs.items())
                 }
             elif method == "multitaper":
                 tfrs = {
                     channel: mne.time_frequency.tfr_array_multitaper(
                         v,
                         self.sf,
                         freqs,
-                        **tfr_method_args,
+                        **tfr_kwargs,
                     )
                     for channel, v in tqdm(for_tfrs.items())
                 }
             # Sort and combine
             data = np.squeeze(
                 np.array([tfr for channel, tfr in natsorted(tfrs.items())])
             )
+
+            # Matrix should be 3D, so if there was only one channel need to expand.
             if data.ndim == 2:
                 data = np.expand_dims(data, axis=0)
             self.tfrs[sleep_stages[stage]] = mne.time_frequency.AverageTFR(
                 info=self.mne_raw.copy().pick(list(tfrs.keys())).info,
                 data=data,
                 times=np.linspace(
                     -time_before,
@@ -831,273 +744,256 @@
             for stage, tfr in self.tfrs.items():
                 tfr.save(
                     self.output_dir
                     / self.__class__.__name__
                     / f"{self.__class__.__name__[:-4].lower()}_{stage}-tfr.h5"
                 )
 
-    def read_tfrs(self, dirpath=None):
+    @logger_wraps()
+    def read_tfrs(self, dirpath: str | None = None):
         """Loads TFRs stored in hdf5 files.
 
         Filenames should end with {type_of_event}_{sleep_stage}-tfr.h5
 
         Args:
             dirpath: Path to the directory containing hdf5 files. Defaults to None.
         """
-        from mne.time_frequency import read_tfrs
-        from pathlib import Path
         import re
 
         r = f"{self.__class__.__name__[:-4].lower()}_(.+)(?:-tfr.h5)"
         self.tfrs = dict()
         dirpath = (
             Path(dirpath) if dirpath else self.output_dir / self.__class__.__name__
         )
         for p in dirpath.glob("*tfr.h5"):
             m = re.search(r, str(p))
             if m:
-                self.tfrs[m.groups()[0]] = read_tfrs(p)
+                self.tfrs[m.groups()[0]] = mne.time_frequency.read_tfrs(p)
 
 
 @define(kw_only=True, slots=False)
-class BaseSpectrum(BaseTopomap, ABC):
-    """A template class for the spectral analysis."""
+class SpectrumPlots(BaseTopomap, ABC):
+    """Plotting spectral data."""
 
-    psd_per_stage: dict = field(init=False)
-    """ Dictionary of the form sleep_stage:[freqs array with shape (n_freqs), 
-    psd array with shape (n_electrodes, n_freqs), 
-    sleep_stage percent from the whole unrejected data]
-    """
-
-    def plot_psd_per_stage(
+    @logger_wraps()
+    def plot_psds(
         self,
-        picks: str | Iterable[str] = ("E101",),
+        picks,
         psd_range: tuple = (-40, 60),
-        freq_range: tuple = (0, 40),
+        freq_range: tuple = (0, 60),
+        dB=True,
         xscale: str = "linear",
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         axis: plt.axis = None,
         plot_sensors: bool = False,
         save: bool = False,
-        psd_method_args: dict = None,
-        subplots_args: dict = None,
+        legend_args: dict = None,
+        **subplots_kw,
     ):
         """Plot PSD per sleep stage.
 
         Args:
-            picks: Channels to calculate PSD on, more info at
-                `mne.io.Raw.get_data <https://mne.tools/stable/generated/
-                mne.io.Raw.html#mne.io.Raw.get_data>`_.
-                Defaults to ("E101",).
             psd_range: Range of y axis on PSD plot. Defaults to (-40, 60).
             freq_range: Range of x axis on PSD plot. Defaults to (0, 40).
+            dB:
             xscale: Scale of the X axis, check available values at
-                `matplotlib.axes.Axes.set_xscale <https://mne.tools/stable/
-                generated/mne.io.Raw.html#mne.io.Raw.get_data>`_.
-                Defaults to "linear".
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
+                :py:meth:`mpl:matplotlib.axes.Axes.set_xscale`. Defaults to "linear".
+            axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
             plot_sensors: Whether to plot sensor map showing which channels were used for
                 computing PSD. Defaults to False.
             save: Whether to save the figure. Defaults to False.
-            psd_method_args: Arguments passed to the PSD method, e.g., welch. Defaults to None.
-            subplots_args: Arguments passed to the plt.subplots(). Have no effect if axis is provided.
-                Defaults to None.
+            **subplots_kw: Arguments passed to the :py:func:`mpl:matplotlib.pyplot.subplots`.
+                Have no effect if axis is provided.Defaults to None.
         """
-        subplots_args = subplots_args or dict()
+        from mne.io.pick import _picks_to_idx
+
+        legend_args = legend_args or dict()
+
         is_new_axis = False
 
         if not axis:
-            fig, axis = plt.subplots(**subplots_args)
+            fig, axis = plt.subplots(**subplots_kw)
             is_new_axis = True
 
-        psd_per_stage = self._compute_psd_per_stage(
-            picks=picks,
-            sleep_stages=sleep_stages,
-            avg_ref=False,
-            dB=True,
-            method_args=psd_method_args,
-        )
-
-        for stage in sleep_stages:
+        for stage, spectrum in self.psds.items():
+            psds = np.mean(
+                spectrum._data[_picks_to_idx(spectrum.info, picks=picks), :], axis=0
+            )
+            psds = 10 * np.log10(10**12 * psds) if dB else 10**12 * psds
             axis.plot(
-                psd_per_stage[stage][0],
-                psd_per_stage[stage][1][0],
-                label=f"{stage} ({psd_per_stage[stage][2]}%)",
+                spectrum._freqs,
+                psds,
+                label=f"{stage} ({spectrum.info.description}%)",
             )
 
         axis.set_xlim(freq_range)
         axis.set_ylim(psd_range)
         axis.set_xscale(xscale)
-        axis.set_title("Welch's PSD")
-        axis.set_ylabel("PSD [dB/Hz]")
-        axis.set_xlabel(f"{xscale} frequency [Hz]".capitalize())
-        axis.legend()
+        units = r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$"
+        axis.set_ylabel(f"Power ({units})")
+        xlabel = (
+            "Frequency (Hz)"
+            if xscale == "linear"
+            else f"{xscale} frequency [Hz]".capitalize()
+        )
+        axis.set_xlabel(xlabel)
+        axis.legend(**legend_args)
 
         if plot_sensors:
-            from mne.io.pick import _picks_to_idx
-            import matplotlib.patches as mpatches
             from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+            from more_itertools import flatten
+            from ast import literal_eval
 
-            color = "cyan"
-            # ax = fig.add_subplot(3, 3, 7)
+            # color = "cyan"
             axins = inset_axes(axis, width="30%", height="30%", loc="lower left")
-            channels = np.array(self.mne_raw.info.ch_names)[
-                _picks_to_idx(self.mne_raw.info, picks)
-            ].tolist()
-            self._plot_sensors(
-                ch_colors={ch: color for ch in channels},
-                axes=axins,
-            )
+            psd_channels = _picks_to_idx(self.mne_raw.info, picks)
 
-            patches = []
-            patches.append(mpatches.Patch(color=color, label="psd"))
-            if self.mne_raw.info["bads"]:
-                patches.append(mpatches.Patch(color="red", label="bad"))
-            axins.legend(
-                handles=patches,
-                loc="lower left",
-                bbox_to_anchor=(1, 0),
-                fontsize="x-small",
+            # Parse log to get interpolated channels
+
+            reg = r"(?:.*) \| (?:.*) \| (?:.*) Interpolated channels: (?P<channels>.*)"
+            interpolated = [
+                literal_eval(e["channels"])
+                for e in logger.parse(self.output_dir / "pipeline.log", reg)
+            ]
+            interpolated = (
+                _picks_to_idx(self.mne_raw.info, list(flatten(interpolated)))
+                if interpolated
+                else None
+            )
+            ch_groups = {
+                k: v
+                for k, v in {"PSD": psd_channels, "Interpolated": interpolated}.items()
+                if v is not None
+            }
+            self.plot_sensors(
+                legend=list(ch_groups.keys()),
+                axes=axins,
+                legend_args=dict(
+                    loc="lower left", bbox_to_anchor=(1, 0), fontsize="x-small"
+                ),
+                ch_groups=list(ch_groups.values()),
+                pointsize=7,
+                linewidth=0.7,
             )
 
         # Save the figure if 'save' set to True and no axis has been passed.
         if save and is_new_axis:
             fig.savefig(self.output_dir / self.__class__.__name__ / f"psd.png")
 
+    @logger_wraps()
     def plot_topomap(
         self,
         stage: str = "REM",
         band: dict = {"Delta": (0, 4)},
         dB: bool = False,
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         axis: plt.axis = None,
         fooof: bool = False,
         save: bool = False,
-        psd_method_args: dict = None,
         topomap_args: dict = None,
         cbar_args: dict = None,
         fooof_group_args: dict = None,
         fooof_get_band_peak_fg_args: dict = None,
         subplots_args: dict = None,
     ):
         """Plots topomap for a sleep stage and a frequency band.
 
         Args:
             stage: One of the sleep_stages keys. Defaults to "REM".
             band: Name-value pair - with name=arbitrary name
                 and value=(l_freq, h_freq).
                 Defaults to {"Delta": (0, 4)}.
             dB: Whether transform PSD to dB. Defaults to False.
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of `matplotlib.pyplot.axis <https://matplotlib.org/
-                stable/api/_as_gen/matplotlib.pyplot.axis.html#matplotlib-pyplot-axis>`_.
+            axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
             fooof: Whether to plot parametrised spectra.
-                More at `fooof <https://fooof-tools.github.io/fooof/auto_examples/analyses/
-                plot_mne_example.html#sphx-glr-auto-examples-analyses-plot-mne-example-py>`_.
+                More at :std:doc:`fooof:auto_examples/analyses/plot_mne_example`.
                 Defaults to False.
             save: Whether to save the figure. Defaults to False.
-            psd_method_args: Arguments passed to the PSD method, e.g., welch. Defaults to None.
-            topomap_args: Arguments passed to `mne.viz.plot_topomap() <https://mne.tools/
-                stable/generated/mne.viz.plot_topomap.html>`_. Defaults to None.
-            cbar_args: Arguments passed to `plt.colorbar() <https://matplotlib.org/stable
-                /api/_as_gen/matplotlib.pyplot.colorbar.html>`_. Defaults to None.
-            fooof_group_args: Arguments passed to `fooof.FOOOFGroup() <https://fooof-tools.github.io/
-                fooof/generated/fooof.FOOOFGroup.html#fooof.FOOOFGroup>`_. Defaults to None.
-            fooof_get_band_peak_fg_args: Arguments passed to the `fooof.analysis.get_band_peak_fg()
-                <https://fooof-tools.github.io/fooof/generated/fooof.analysis.get_band_peak_fg.html>`_.
-                Defaults to None.
-            subplots_args: Arguments passed to the plt.subplots(). Have no effect if axis is provided.
-                Defaults to None.
+            topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
+            cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
+            subplots_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.subplots`.Defaults to None.
+            fooof_group_args: Arguments passed to :py:class:`fooof:fooof.FOOOFGroup`. Defaults to None.
+            fooof_get_band_peak_fg_args: Arguments passed to the :py:func:`fooof:fooof.analysis.get_band_peak_fg`. Defaults to None.
         """
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         subplots_args = subplots_args or dict()
         topomap_args.setdefault("cmap", "plasma")
         cbar_args.setdefault(
-            "label", "dB/Hz" if dB else r"$\mu V^{2}/Hz$" if not fooof else None
+            "label",
+            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$" if not fooof else None,
         )
-        assert (
-            stage in sleep_stages.keys()
-        ), f"sleep_stages should contain provided stage"
+        assert stage in self.psds, f"{stage} is not in self.psds"
 
         is_new_axis = False
 
         if axis is None:
             fig, axis = plt.subplots(**subplots_args)
             is_new_axis = True
 
-        self.psd_per_stage = self._compute_psd_per_stage(
-            picks=["eeg"],
-            sleep_stages=sleep_stages,
-            avg_ref=True,
-            dB=dB,
-            method_args=psd_method_args,
-        )
-
         [(_, b)] = band.items()
 
         if fooof:
             psds = self._fooof(
                 band=band,
                 stage=stage,
                 fooof_group_args=fooof_group_args,
                 get_band_peak_fg_args=fooof_get_band_peak_fg_args,
             )
 
         else:
+            psds = (
+                10 * np.log10(10**12 * self.psds[stage]._data)
+                if dB
+                else 10**12 * self.psds[stage]._data
+            )
             psds = np.take(
-                self.psd_per_stage[stage][1],
+                psds,
                 np.where(
                     np.logical_and(
-                        self.psd_per_stage[stage][0] >= b[0],
-                        self.psd_per_stage[stage][0] <= b[1],
+                        self.psds[stage]._freqs >= b[0],
+                        self.psds[stage]._freqs <= b[1],
                     )
                 )[0],
                 axis=1,
             ).sum(axis=1)
 
         self._plot_topomap(
             data=psds,
             axis=axis,
             topomap_args=topomap_args,
             cbar_args=cbar_args,
         )
+
         if is_new_axis:
             fig.suptitle(f"{stage} ({b[0]}-{b[1]} Hz)")
         if save and is_new_axis:
             fig.savefig(
                 self.output_dir
                 / self.__class__.__name__
                 / f"topomap_psd_{list(band)[0]}.png"
             )
 
+    @logger_wraps()
     def plot_topomap_collage(
         self,
         stages_to_plot: tuple = "all",
         bands: dict = {
             "Delta": (0, 3.99),
             "Theta": (4, 7.99),
             "Alpha": (8, 12.49),
             "SMR": (12.5, 15),
             "Beta": (12.5, 29.99),
             "Gamma": (30, 60),
         },
         dB: bool = False,
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         fooof: bool = False,
         low_percentile: float = 5,
         high_percentile: float = 95,
         save: bool = False,
-        psd_method_args: dict = None,
         topomap_args: dict = None,
         cbar_args: dict = None,
         fooof_group_args: dict = None,
         fooof_get_band_peak_fg_args: dict = None,
         figure_args: dict = None,
     ):
         """Plots topomap collage for multiple sleep stages and bands.
@@ -1111,88 +1007,78 @@
                 and value=(l_freq, h_freq).
                 Defaults to { "Delta": (0, 3.99), "Theta": (4, 7.99), "Alpha": (8, 12.49),
                 "SMR": (12.5, 15), "Beta": (12.5, 29.99), "Gamma": (30, 60), }.
             dB: Whether transform PSD to dB. Defaults to False.
             sleep_stages: Mapping between sleep stages names and their integer representations.
                 Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
             fooof: Whether to plot parametrised spectra.
-                More at `fooof <https://fooof-tools.github.io/fooof/auto_examples/analyses/
-                plot_mne_example.html#sphx-glr-auto-examples-analyses-plot-mne-example-py>`_.
+                More at :std:doc:`fooof:auto_examples/analyses/plot_mne_example`.
                 Defaults to False.
             low_percentile: Set min color value by percentile of the band data.
                 Defaults to 5.
             high_percentile: Set max color value by percentile of the band data.
                 Defaults to 95.
             save: Whether to save the figure. Defaults to False.
-            psd_method_args: Arguments passed to the PSD method, e.g., welch. Defaults to None.
-            topomap_args: Arguments passed to `mne.viz.plot_topomap() <https://mne.tools/
-                stable/generated/mne.viz.plot_topomap.html>`_. Defaults to None.
-            cbar_args: Arguments passed to `plt.colorbar() <https://matplotlib.org/stable
-                /api/_as_gen/matplotlib.pyplot.colorbar.html>`_. Defaults to None.
-            fooof_group_args: Arguments passed to `fooof.FOOOFGroup() <https://fooof-tools.github.io/
-                fooof/generated/fooof.FOOOFGroup.html#fooof.FOOOFGroup>`_. Defaults to None.
-            fooof_get_band_peak_fg_args: Arguments passed to the `fooof.analysis.get_band_peak_fg()
-                <https://fooof-tools.github.io/fooof/generated/fooof.analysis.get_band_peak_fg.html>`_.
-                Defaults to None.
-            figure_args: Arguments passed to `plt.figure() <https://matplotlib.org/stable/
-                api/_as_gen/matplotlib.pyplot.figure.html>`_. Defaults to None.
+            topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
+            cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
+            figure_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.figure`.Defaults to None.
+            fooof_group_args: Arguments passed to :py:class:`fooof:fooof.FOOOFGroup`. Defaults to None.
+            fooof_get_band_peak_fg_args: Arguments passed to the :py:func:`fooof:fooof.analysis.get_band_peak_fg`. Defaults to None.
         """
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         figure_args = figure_args or dict()
         topomap_args.setdefault("cmap", "plasma")
         topomap_args.setdefault("vlim", [None, None])
         cbar_args.setdefault(
-            "label", "dB/Hz" if dB else r"$\mu V^{2}/Hz$" if not fooof else None
+            "label",
+            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$" if not fooof else None,
         )
 
         if stages_to_plot == "all":
-            stages_to_plot = sleep_stages.keys()
+            stages_to_plot = self.psds.keys()
         n_rows = len(stages_to_plot)
         n_cols = len(bands)
 
         figure_args.setdefault("figsize", (n_cols * 4, n_rows * 4))
         figure_args.setdefault("layout", "constrained")
         fig = plt.figure(**figure_args)
         subfigs = fig.subfigures(n_rows, 1)
 
-        self.psd_per_stage = self._compute_psd_per_stage(
-            picks=["eeg"],
-            sleep_stages=sleep_stages,
-            avg_ref=True,
-            dB=dB,
-            method_args=psd_method_args,
-        )
-
         if low_percentile:
             perc_low = dict()
 
         if high_percentile:
             perc_high = dict()
 
         psds_per_stage_per_band = np.empty(
             (len(stages_to_plot), len(bands)), dtype=object
         )
         for col_index, (band_key, b) in enumerate(bands.items()):
             for_perc = []
-            for row_index, stage in enumerate(self.psd_per_stage):
+            for row_index, stage in enumerate(self.psds):
                 if fooof:
                     psds = self._fooof(
                         band={band_key: b},
                         stage=stage,
                         fooof_group_args=fooof_group_args,
                         get_band_peak_fg_args=fooof_get_band_peak_fg_args,
                     )
                 else:
+                    psds = (
+                        10 * np.log10(10**12 * self.psds[stage]._data)
+                        if dB
+                        else 10**12 * self.psds[stage]._data
+                    )
                     psds = np.take(
-                        self.psd_per_stage[stage][1],
+                        psds,
                         np.where(
                             np.logical_and(
-                                self.psd_per_stage[stage][0] >= b[0],
-                                self.psd_per_stage[stage][0] <= b[1],
+                                self.psds[stage]._freqs >= b[0],
+                                self.psds[stage]._freqs <= b[1],
                             )
                         )[0],
                         axis=1,
                     ).sum(axis=1)
                 for_perc.append(psds)
                 psds_per_stage_per_band[row_index, col_index] = psds
             if low_percentile:
@@ -1216,15 +1102,15 @@
                     cbar_args=cbar_args,
                 )
                 axes[col_index].set_title(
                     f"{band_key} ({bands[band_key][0]}-{bands[band_key][1]} Hz)"
                 )
 
             subfigs[row_index].suptitle(
-                f"{stage} ({self.psd_per_stage[stage][2]}%)", fontsize="xx-large"
+                f"{stage} ({self.psds[stage].info.description}%)", fontsize="xx-large"
             )
 
         if save:
             fig.savefig(
                 self.output_dir / self.__class__.__name__ / f"topomap_psd_collage.png"
             )
 
@@ -1242,16 +1128,16 @@
         # Initialize a FOOOFGroup object, with desired settings
         fg = FOOOFGroup(**fooof_group_args)
 
         # Define the frequency range to fit
         freq_range = [1, 45]
 
         fg.fit(
-            self.psd_per_stage[stage][0],
-            self.psd_per_stage[stage][1],
+            self.psds[stage]._freqs,
+            self.psds[stage]._data,
             freq_range=freq_range,
         )
 
         # Define frequency bands of interest
         bands = Bands(band)
 
         # Extract peaks
@@ -1259,10 +1145,138 @@
 
         peaks[np.where(np.isnan(peaks))] = 0
         # Extract the power values from the detected peaks
         psds = peaks[:, 1]
 
         return psds
 
-    @abstractmethod
-    def _compute_psd_per_stage(self):
-        pass
+
+@define(kw_only=True, slots=False)
+class SleepSpectrum(mne.time_frequency.spectrum.BaseSpectrum):
+    """Spectral representation of sleep stage data.
+
+    Adapted from `MNE <https://mne.tools/stable/index.html>`_.
+    """
+
+    def __init__(
+        self,
+        inst,
+        hypno,
+        stage_idx,
+        method,
+        fmin,
+        fmax,
+        tmin,
+        tmax,
+        picks,
+        proj,
+        reject_by_annotation,
+        *,
+        n_jobs,
+        verbose=None,
+        **method_kw,
+    ):
+        # triage reading from file
+        if isinstance(inst, dict):
+            self.__setstate__(inst)
+            return
+        # do the basic setup
+        super().__init__(
+            inst,
+            method,
+            fmin,
+            fmax,
+            tmin,
+            tmax,
+            picks,
+            proj,
+            n_jobs=n_jobs,
+            verbose=verbose,
+            **method_kw,
+        )
+        data = self.inst.get_data(
+            self._picks,
+            reject_by_annotation="NaN" if reject_by_annotation else None,
+        )
+        # compute the spectra
+        self._compute_spectra(
+            method, data, hypno, stage_idx, fmin, fmax, n_jobs, verbose
+        )
+        # check for correct shape and bad values
+        self._check_values()
+        del self._shape
+        # save memory
+        del self.inst
+
+    def _compute_spectra(
+        self, method, data, hypno, stage_idx, fmin, fmax, n_jobs, verbose
+    ):
+        """
+        Weighted average for Welch's PSD.
+        Average of uniform sample regions for Multitaper's PSD.
+        """
+        from scipy import ndimage
+        from more_itertools import collapse
+
+        n_samples_total = np.count_nonzero(~np.isnan(data), axis=1)[0]
+        psds_list = []
+        weights = []
+        n_samples = 0
+        try:
+            regions = collapse(
+                ndimage.find_objects(
+                    ndimage.label(
+                        np.logical_or.reduce([hypno == i for i in stage_idx])
+                    )[0]
+                )
+            )
+        except TypeError:
+            regions = collapse(
+                ndimage.find_objects(ndimage.label(hypno == stage_idx)[0])
+            )
+
+        if method == "multitaper":
+            from more_itertools import flatten
+
+            uniform_region_samples = 2000
+            ranges = [
+                list(range(region.start, region.stop, uniform_region_samples))
+                for region in regions
+            ]
+            slice_ranges = flatten([list(zip(r[:-1], r[1:])) for r in ranges])
+            regions = [slice(z[0], z[1]) for z in slice_ranges]
+
+        for region in regions:
+            n_samples_per_region = np.count_nonzero(~np.isnan(data[:, region]), axis=1)[
+                0
+            ]
+
+            # make the spectra
+            psds, freqs = self._psd_func(
+                data[:, region],
+                self.sfreq,
+                fmin=fmin,
+                fmax=fmax,
+                n_jobs=n_jobs,
+                verbose=verbose,
+            )
+            psds_list.append(psds)
+            weights.append(n_samples_per_region)
+            n_samples += n_samples_per_region
+
+        # avg_psds = np.average(np.array(psds_list), weights=weights, axis=0)
+        masked_data = np.ma.masked_array(
+            np.array(psds_list), np.isnan(np.array(psds_list))
+        )
+        average = np.ma.average(masked_data, weights=weights, axis=0)
+        avg_psds = average.filled(np.nan)
+
+        self._data = avg_psds
+        self._freqs = freqs
+        self.info.description = str(round(n_samples / n_samples_total * 100, 2))
+        # this is *expected* shape, it gets asserted later in _check_values()
+        # (and then deleted afterwards)
+        self._shape = (len(self.ch_names), len(self.freqs))
+        # we don't need these anymore, and they make save/load harder
+        del self._picks
+        del self._psd_func
+        del self._time_mask
```

### Comparing `sleepeeg-0.1.1/sleepeeg/pipeline.py` & `sleepeeg-0.2.0/sleepeeg/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,393 +1,437 @@
 """This module contains and describes pipe elements for sleep eeg analysis.
 """
 
 from attrs import define, field
+from loguru import logger
+from typing import TypeVar
 from pathlib import Path
-import matplotlib.pyplot as plt
+from collections.abc import Iterable
+
 import numpy as np
-import mne.io
+import matplotlib.pyplot as plt
+import mne
 
 
-from collections.abc import Iterable
+from .base import (
+    BasePipe,
+    BaseHypnoPipe,
+    BaseEventPipe,
+    SpectrumPlots,
+    SleepSpectrum,
+    logger_wraps,
+)
 
-from sleepeeg.base import BasePipe, BaseHypnoPipe, BaseEventPipe, BaseSpectrum
+# For type annotation of pipe elements.
+BasePipeType = TypeVar("BasePipeType", bound="BasePipe")
 
 
 @define(kw_only=True)
 class CleaningPipe(BasePipe):
     """The cleaning pipeline element.
 
     Contains resampling function, band and notch filters,
     browser for manual selection of bad channels
     and bad data spans.
     """
 
-    def resample(
-        self,
-        save: bool = False,
-        mne_resample_args: dict = None,
-    ):
-        """A wrapper for
-        `mne.io.Raw.resample <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.resample>`_
+    @logger_wraps()
+    def resample(self, sfreq: float = 250, save: bool = False, **resample_kwargs):
+        """A wrapper for :py:meth:`mne:mne.io.Raw.resample`
         with an additional option to save the resampled data.
 
         Args:
             save: Whether to save a resampled data to a fif file. Defaults to False.
-            mne_resample_args: Arguments passed to `mne.io.Raw.resample <https://mne.tools/stable/
-                generated/mne.io.Raw.html#mne.io.Raw.resample>`_. Defaults to None.
+            **resample_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.resample`.
         """
-        mne_resample_args = mne_resample_args or dict()
-        mne_resample_args.setdefault("sfreq", 250)
-        self.mne_raw.resample(**mne_resample_args)
+        self.mne_raw.resample(sfreq=sfreq, **resample_kwargs)
         if save:
             self.save_raw(
                 "_".join(
                     filter(
                         None,
                         [
                             "resampled",
-                            str(mne_resample_args["sfreq"]) + "hz",
+                            str(sfreq) + "hz",
                             "raw.fif",
                         ],
                     )
                 )
             )
 
+    @logger_wraps()
     def filter(
-        self,
-        mne_filter_args: dict = None,
+        self, l_freq: float | None = 0.3, h_freq: float | None = None, **filter_kwargs
     ):
-        """A wrapper for
-        `mne.io.Raw.filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.filter>`_.
+        """A wrapper for :py:meth:`mne:mne.io.Raw.filter`.
 
         Args:
-            mne_filter_args: Arguments passed to `mne.io.Raw.filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.filter>`_.
+            **filter_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.filter`.
         """
-        mne_filter_args = mne_filter_args or dict()
-        mne_filter_args.setdefault("l_freq", 0.3)
-        self.mne_raw.load_data()
-        self.mne_raw.filter(**mne_filter_args)
+        self.mne_raw.load_data().filter(l_freq=l_freq, h_freq=h_freq, **filter_kwargs)
 
-    def notch(
-        self,
-        mne_notch_args: dict = None,
-    ):
-        """A wrapper for
-        `mne.io.Raw.notch_filter <https://mne.tools/stable/generated/mne.io.Raw.html#mne.io.Raw.notch_filter>`_.
+    @logger_wraps()
+    def notch(self, freqs: str | Iterable[float] = "50s", **notch_kwargs):
+        """A wrapper for :py:meth:`mne:mne.io.Raw.notch_filter`.
 
         Args:
-            freqs: Frequencies to filter out from data,
-                e.g. np.arange(50, 251, 50) for sampling freq 250 Hz.
-                Defaults to None.
-            picks: Channels to filter, if None - all channels will be filtered.
-                Defaults to "eeg".
-            n_jobs: The number of jobs to run in parallel or CUDA. Defaults to "cuda".
+            **notch_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.notch_filter`.
         """
-        mne_notch_args = mne_notch_args or dict()
-        mne_notch_args.setdefault("freqs", np.arange(50, int(self.sf / 2), 50))
-        self.mne_raw.notch_filter(**mne_notch_args)
+        if freqs == "50s":
+            freqs = np.arange(50, int(self.sf / 2), 50)
+        elif freqs == "60s":
+            freqs = np.arange(50, int(self.sf / 2), 50)
+        self.mne_raw.load_data().notch_filter(freqs=freqs, **notch_kwargs)
 
-    def read_bad_channels(self, path=None):
+    def read_bad_channels(self, path: str | None = None):
         """Imports bad channels from file to mne raw object.
 
         Args:
             path: Path to the txt file with bad channel name per row. Defaults to None.
         """
         p = (
             Path(path)
             if path
             else self.output_dir / self.__class__.__name__ / "bad_channels.txt"
         )
         with open(p, "r") as f:
             self.mne_raw.info["bads"] = list(filter(None, f.read().split("\n")))
 
-    def read_annotations(self, path=None):
+    def read_annotations(self, path: str | None = None):
         """Imports annotations from file to mne raw object
 
         Args:
             path: Path to txt file with mne-style annotations. Defaults to None.
         """
         from mne import read_annotations
 
         p = (
             Path(path)
             if path
             else self.output_dir / self.__class__.__name__ / "annotations.txt"
         )
         self.mne_raw.set_annotations(read_annotations(p))
 
+    @logger_wraps()
+    def interpolate_bads(self, **interp_kwargs):
+        """A wrapper for :py:meth:`mne:mne.io.Raw.interpolate_bads`
+
+        Args:
+            **interp_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.interpolate_bads`.
+        """
+        bads = self.mne_raw.info["bads"]
+        self.mne_raw.interpolate_bads(**interp_kwargs)
+        logger.info(f"Interpolated channels: {bads}")
+
 
 @define(kw_only=True)
 class ICAPipe(BasePipe):
     """The ICA pipeline element.
 
     Contains ica fitting, plotting multiple ica plots,
     selecting ica exclusion components and
     its application to the raw data.
-    More at `mne.preprocessing.ICA <https://mne.tools/stable/
-    generated/mne.preprocessing.ICA.html#mne-preprocessing-ica>`_.
-    """
-
-    n_components: int | float | None = field(default=30)
-    """Number of principal components (from the pre-whitening PCA step) 
-    that are passed to the ICA algorithm during fitting.
-    """
-
-    method: str = field(default="fastica")
-    """The ICA method to use in the fit method. 
-
-    Can be 'fastica', 'infomax' or 'picard'
-    Use the fit_params argument to set additional parameters.
-    """
-    fit_params: dict = field(default=None)
-    """Additional parameters passed to the ICA estimator as specified by method. 
-    Allowed entries are determined by the various algorithm implementations: 
-    see `FastICA <https://scikit-learn.org/stable/modules/generated/sklearn.
-    decomposition.FastICA.html#sklearn.decomposition.FastICA>`_, 
-    `picard <https://pierreablin.github.io/picard/generated/picard.picard.html#picard.picard>`_ and
-    `infomax <https://mne.tools/stable/generated/mne.preprocessing.infomax.html#mne.preprocessing.infomax>`_.
+    More at :py:class:`mne:mne.preprocessing.ICA`.
     """
 
-    path_to_ica: Path = field(converter=Path, default="/")
-
     mne_ica: mne.preprocessing.ICA = field()
-    """Instance of 
-    `mne.preprocessing.ICA <https://mne.tools/stable/
-    generated/mne.preprocessing.ICA.html#mne-preprocessing-ica>`_.
+    """Instance of :py:class:`mne:mne.preprocessing.ICA`.
     """
 
-    @mne_ica.default
-    def _set_mne_ica(self):
-        if self.path_to_ica == Path("/"):
-            return mne.preprocessing.ICA(
-                n_components=self.n_components,
-                method=self.method,
-                fit_params=self.fit_params,
-            )
-        return mne.preprocessing.read_ica(self.path_to_ica)
+    def __init__(
+        self,
+        prec_pipe: BasePipeType | None = None,
+        path_to_eeg: str = "",
+        output_dir: str = "",
+        method: str = "fastica",
+        n_components: int | float | None = None,
+        fit_params: dict | None = None,
+        path_to_ica: str | None = None,
+        **ica_kwargs,
+    ):
+        """
 
-    def __attrs_post_init__(self):
+        Args:
+            prec_pipe: Preceding pipe that hands over mne_raw attribute. Defaults to None.
+            path_to_eeg: Can be any file type supported by :py:func:`mne:mne.io.read_raw`. Defaults to None.
+            output_dir: Path to the directory where the output will be saved. Defaults to None.
+            method: The ICA method to use in the fit method. Defaults to 'fastica'.
+            n_components: Number of principal components (from the pre-whitening PCA step)
+                that are passed to the ICA algorithm during fitting:
+                read more at :py:class:`mne:mne.preprocessing.ICA`. Defaults to None.
+            fit_params:
+                Additional parameters passed to the ICA estimator as specified by method.
+                Allowed entries are determined by the various algorithm implementations:
+                see `FastICA <https://scikit-learn.org/stable/modules/generated/sklearn.
+                decomposition. FastICA.html#sklearn.decomposition.FastICA>`_,
+                `picard <https://pierreablin.github.io/picard/generated/picard.picard.html#picard.picard>`_ and
+                `infomax <https://mne.tools/stable/generated/mne.preprocessing.infomax.html#mne.preprocessing.infomax>`_.
+                Defaults to None.
+            path_to_ica: Path to the saved -ica.fif file you want to continue work with.
+            **ica_kwargs: Arguments passed to :py:class:`mne:mne.preprocessing.ICA`.
+        """
+        if path_to_ica is not None:
+            ica = mne.preprocessing.read_ica(path_to_ica)
+        else:
+            ica = mne.preprocessing.ICA(
+                n_components=n_components,
+                method=method,
+                fit_params=fit_params,
+                **ica_kwargs,
+            )
+        if prec_pipe is not None:
+            self.__attrs_init__(prec_pipe=prec_pipe, mne_ica=ica)
+        else:
+            self.__attrs_init__(
+                path_to_eeg=path_to_eeg,
+                output_dir=output_dir,
+                mne_ica=ica,
+            )
         self.mne_raw.load_data()
 
-    def fit(self, filter_args=None, ica_fit_args=None):
-        """Highpass-filters (1Hz) a copy of the mne_raw object
-        and then runs `mne.preprocessing.ICA.fit <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.fit>`_.
-        """
-        filter_args = filter_args or dict()
-        ica_fit_args = ica_fit_args or dict()
-        filter_args.setdefault("l_freq", 1.0)
+    @logger_wraps()
+    def fit(self, filter_kwargs: dict = None, **fit_kwargs):
+        """Highpass-filters (1 Hz) a copy of the mne_raw object
+        and then runs :py:meth:`mne:mne.preprocessing.ICA.fit`.
+
+        Args:
+            filter_args: Arguments passed to :py:meth:`mne:mne.io.Raw.filter`.
+            **fit_kwargs: Arguments passed to :py:meth:`mne:mne.preprocessing.ICA.fit`.
+        """
+        filter_kwargs = filter_kwargs or dict()
+        filter_kwargs.setdefault("l_freq", 1.0)
+        filter_kwargs.setdefault("h_freq", None)
         if self.mne_raw.info["highpass"] < 1.0:
             filtered_raw = self.mne_raw.copy()
-            filtered_raw.filter(**filter_args)
+            filtered_raw.filter(**filter_kwargs)
         else:
             filtered_raw = self.mne_raw
-        self.mne_ica.fit(filtered_raw, **ica_fit_args)
+        self.mne_ica.fit(filtered_raw, **fit_kwargs)
 
     def plot_sources(self, **kwargs):
-        """A wrapper for `mne.preprocessing.ICA.plot_sources <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_sources>`_.
-        """
-        self.mne_ica.plot_sources(self.mne_raw, block=True, **kwargs)
+        """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_sources`."""
+        self.mne_ica.plot_sources(inst=self.mne_raw, **kwargs)
 
     def plot_components(self, **kwargs):
-        """A wrapper for `mne.preprocessing.ICA.plot_components <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_components>`_.
-        """
+        """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_components`."""
         self.mne_ica.plot_components(inst=self.mne_raw, **kwargs)
 
-    def plot_overlay(self, exclude=None, picks=None, start=10, stop=20, **kwargs):
-        """A wrapper for `mne.preprocessing.ICA.plot_overlay <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_overlay>`_.
-        """
-        self.mne_ica.plot_overlay(
-            self.mne_raw, exclude=exclude, picks=picks, start=start, stop=stop, **kwargs
-        )
-
     def plot_properties(self, picks=None, **kwargs):
-        """A wrapper for `mne.preprocessing.ICA.plot_properties <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.plot_properties>`_.
-        """
+        """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_properties`."""
         self.mne_ica.plot_properties(self.mne_raw, picks=picks, **kwargs)
 
+    @logger_wraps()
     def apply(self, exclude=None, **kwargs):
-        """Remove selected components from the signal.
-
-        A wrapper for `mne.preprocessing.ICA.apply <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.apply>`_.
-        """
+        """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.apply`."""
+        logger.info(
+            f"Excluded ICA components: {list(set((exclude or [])+(self.mne_ica.exclude or [])))}"
+        )
         self.mne_ica.apply(self.mne_raw, exclude=exclude, **kwargs)
 
-    def save_ica(self, fname="data-ica.fif", overwrite=False):
-        """A wrapper for `mne.preprocessing.ICA.save <https://mne.tools/stable/
-        generated/mne.preprocessing.ICA.html#mne.preprocessing.ICA.save>`_.
+    @logger_wraps()
+    def save_ica(self, fname: str = "data-ica.fif", overwrite: bool = False):
+        """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.save`.
 
         Args:
             fname: filename for the ica file being saved. Defaults to "data-ica.fif".
             overwrite: Whether to overwrite the file. Defaults to False.
         """
-        fif_folder = self.output_dir / self.__class__.__name__ / "saved_ica"
+        fif_folder = self.output_dir / self.__class__.__name__
         fif_folder.mkdir(exist_ok=True)
         self.mne_ica.save(fif_folder / fname, overwrite=overwrite)
 
 
 @define(kw_only=True)
-class SpectralPipe(BaseHypnoPipe, BaseSpectrum):
+class SpectralPipe(BaseHypnoPipe, SpectrumPlots):
     """The spectral analyses pipeline element.
 
     Contains methods for computing and plotting PSD,
-    spectrogram and topomaps, per sleep stage.
+    spectrogram and topomaps per sleep stage.
+    """
+
+    psds: dict = field(init=False, factory=dict)
+    """Instances of :class:`.SleepSpectrum` per sleep stage.
     """
 
+    @logger_wraps()
+    def compute_psds_per_stage(
+        self,
+        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
+        reference: Iterable[str] | str | None = None,
+        method: str = "welch",
+        fmin: float = 0,
+        fmax: float = 60,
+        picks: str | Iterable[str] = "eeg",
+        reject_by_annotation: bool = True,
+        save: bool = False,
+        overwrite: bool = False,
+        n_jobs: bool = -1,
+        verbose: bool = False,
+        **psd_kwargs,
+    ):
+        """For each sleep stage creates a :class:`.SleepSpectrum` object.
+
+        Args:
+            sleep_stages: Sleep stages mapping in hypnogram.
+                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
+            reference: Which eeg reference to compute PSD with.
+                If None, the reference isn't changed. Defaults to None.
+            method: Spectral estimation method.. Defaults to "welch".
+            fmin: Lower frequency bound. Defaults to 0.
+            fmax: Upper frequency bound. Defaults to 60.
+            picks: Channels to compute spectra for. Refer to :py:meth:`mne:mne.io.Raw.pick`.
+                Defaults to "eeg".
+            reject_by_annotation: Whether to not use the annotations for the spectra computation.
+                Defaults to True.
+            save: Whether to save the spectra in .h5 files. Defaults to False.
+            overwrite: Whether to overwrite the file. Defaults to False.
+            n_jobs: _description_. Defaults to -1.
+            verbose: _description_. Defaults to False.
+            **psd_kwargs: Additional arguments passed to :py:func:`mne:mne.time_frequency.psd_array_welch`
+                or :py:func:`mne:mne.time_frequency.psd_array_multitaper`.
+        """
+        inst = self.mne_raw.copy().load_data()
+        if reference is not None:
+            inst.set_eeg_reference(ref_channels=reference)
+        for stage, stage_idx in sleep_stages.items():
+            self.psds[stage] = SleepSpectrum(
+                inst,
+                hypno=self.hypno_up,
+                stage_idx=stage_idx,
+                method=method,
+                fmin=fmin,
+                fmax=fmax,
+                tmin=None,
+                tmax=None,
+                picks=picks,
+                proj=False,
+                reject_by_annotation=reject_by_annotation,
+                n_jobs=n_jobs,
+                verbose=verbose,
+                **psd_kwargs,
+            )
+        if save:
+            import re
+
+            for stage, spectrum in self.psds.items():
+                stage = re.sub(r"[^\w\s-]", "_", stage)
+                spectrum.save(
+                    self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
+                    overwrite=overwrite,
+                )
+
+    @logger_wraps()
+    def read_spectra(self, dirpath: str | None = None):
+        """Loads spectra stored in hdf5 files.
+
+        Filenames should end with {sleep_stage}-psd.h5
+
+        Args:
+            dirpath: Path to the directory containing hdf5 files. Defaults to None.
+        """
+        from mne.time_frequency import read_spectrum
+        from pathlib import Path
+        import re
+
+        r = f"(.+)(?:-psd.h5)"
+        self.tfrs = dict()
+        dirpath = (
+            Path(dirpath) if dirpath else self.output_dir / self.__class__.__name__
+        )
+        for p in dirpath.glob("*psd.h5"):
+            m = re.search(r, str(p))
+            if m:
+                self.psds[m.groups()[0]] = read_spectrum(p)
+
+    @logger_wraps()
     def plot_hypnospectrogram(
         self,
         picks: str | Iterable[str] = ("E101",),
-        sec_per_seg: float = 4.096,
+        win_sec: float = 30,
+        trimperc: float = 2.5,
         freq_range: tuple = (0, 40),
-        cmap: str = "inferno",
+        cmap: str = "Spectral_r",
         overlap: bool = False,
         save: bool = False,
+        axis: plt.Axes = None,
     ):
         """Plots hypnogram and spectrogram.
 
+        Adapted from yasa.
+
         Args:
-            picks: Channels to calculate spectrogram on, more info at
-                `mne.io.Raw.get_data <https://mne.tools/stable/generated/
-                mne.io.Raw.html#mne.io.Raw.get_data>`_.
-                Defaults to ("E101",).
-            sec_per_seg: Segment length in seconds. Defaults to 4.096.
+            picks: Channels to compute the spectrogram on. Defaults to ("E101",).
+            win_sec: The length of the sliding window, in seconds, used for multitaper PSD calculation. Defaults to 30.
+            trimperc: The amount of data to trim on both ends of the distribution when normalizing the colormap. Defaults to 2.5.
             freq_range: Range of x axis on spectrogram plot. Defaults to (0, 40).
-            cmap: Matplotlib `colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_. Defaults to "inferno".
+            cmap: Matplotlib colormap. :std:doc:`mpl:tutorials/colors/colormaps`. Defaults to "Spectral_r".
             overlap: Whether to plot hypnogram over the spectrogram or on top of it. Defaults to False.
             save: Whether to save the figure. Defaults to False.
+            axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
+                Defaults to None.
         """
         # Import data from the raw mne file.
         data = self.mne_raw.get_data(picks, units="uV", reject_by_annotation="NaN")[0]
         # Create a plot figure
-        fig = self.__plot_hypnospectrogram(
-            data,
-            self.sf,
-            self.hypno_up,
-            win_sec=sec_per_seg,
-            fmin=freq_range[0],
-            fmax=freq_range[1],
-            trimperc=0,
-            cmap=cmap,
-            overlap=overlap,
-        )
-        # Save the figure if 'save' set to True
-        if save:
-            fig.savefig(
-                self.output_dir / self.__class__.__name__ / f"spectrogram.png",
-                bbox_inches="tight",
-            )
+        if overlap or not self.hypno_up.any():
+            if axis is None:
+                fig, axis = plt.subplots(nrows=1, figsize=(12, 4))
 
-    def _compute_psd_per_stage(
-        self, picks, sleep_stages, avg_ref, dB, method_args=None
-    ):
-        from collections import defaultdict
-        from scipy import signal, ndimage
-
-        assert (
-            self.hypno.any()
-        ), f"Hypnogram hasn't been provided, can't compute PSD per stage"
-
-        method_args = method_args or dict()
-        method_args["axis"] = 1
-        if "nperseg" not in method_args:
-            method_args["nperseg"] = self.sf * 4.096
-        # Import data from the raw mne file.
-        self.mne_raw.load_data()
-        if avg_ref:
-            data = (
-                self.mne_raw.copy()
-                .set_eeg_reference()
-                .get_data(picks=picks, units="uV", reject_by_annotation="NaN")
-            )
-        else:
-            data = self.mne_raw.get_data(
-                picks=picks, units="uV", reject_by_annotation="NaN"
-            )
-        data = np.ma.array(data, mask=np.isnan(data))
-        n_samples_total = np.ma.compress_cols(data).shape[1]
-        psds = defaultdict(list)
-        psd_per_stage = {}
-        for stage, index in sleep_stages.items():
-            weights = []
-            n_samples = 0
-            try:
-                regions = ndimage.find_objects(
-                    ndimage.label(
-                        np.logical_or.reduce([self.hypno_up == i for i in index])
-                    )[0]
-                )
-            except TypeError:
-                regions = ndimage.find_objects(ndimage.label(self.hypno_up == index)[0])
-            for region in regions:
-                compressed = np.ma.compress_cols(data[:, region[0]])
-                if compressed.size > method_args["nperseg"]:
-                    weights.append(compressed.shape[1])
-                    freqs, psd = signal.welch(
-                        compressed,
-                        fs=self.sf,
-                        **method_args,
-                    )
-                    psds[stage].append(psd)
-                    n_samples += compressed.shape[1]
-            avg = np.average(np.array(psds[stage]), weights=weights, axis=0)
-            psd_per_stage[stage] = [
-                freqs,
-                10 * np.log10(avg) if dB else avg,
-                round(n_samples / n_samples_total * 100, 2),
-            ]
-        return psd_per_stage
-
-    def __plot_hypnospectrogram(
-        self, data, sf, hypno, win_sec, fmin, fmax, trimperc, cmap, overlap
-    ):
-        """
-        ?
-        """
-        # Increase font size while preserving original
-        old_fontsize = plt.rcParams["font.size"]
-        plt.rcParams.update({"font.size": 18})
-
-        if overlap or not hypno.any():
-            fig, ax = plt.subplots(nrows=1, figsize=(12, 4))
             im = self.__plot_spectrogram(
-                data, sf, win_sec, fmin, fmax, trimperc, cmap, ax
+                data,
+                self.sf,
+                win_sec,
+                freq_range[0],
+                freq_range[1],
+                trimperc,
+                cmap,
+                axis,
             )
-            if hypno.any():
-                ax_hypno = ax.twinx()
-                self.__plot_hypnogram(sf, hypno, ax_hypno)
+            if self.hypno_up.any():
+                ax_hypno = axis.twinx()
+                self.__plot_hypnogram(self.sf, self.hypno_up, ax_hypno)
             # Add colorbar
-            cbar = fig.colorbar(
-                im, ax=ax, shrink=0.95, fraction=0.1, aspect=25, pad=0.1
+            cbar = plt.colorbar(im, ax=axis, shrink=0.95, fraction=0.1, aspect=25)
+            cbar.ax.set_ylabel(r"$\mu V^{2}/Hz$ (dB)", rotation=90)
+            return None if axis is not None else fig
+        else:
+            if axis is None:
+                fig, (ax0, ax1) = plt.subplots(
+                    nrows=2, figsize=(12, 6), gridspec_kw={"height_ratios": [1, 2]}
+                )
+                plt.subplots_adjust(hspace=0.1)
+            else:
+                ax0 = axis[0]
+                ax1 = axis[1]
+
+            if self.hypno_up.any():
+                # Hypnogram (top axis)
+                self.__plot_hypnogram(self.sf, self.hypno_up, ax0)
+            # Spectrogram (bottom axis)
+            self.__plot_spectrogram(
+                data,
+                self.sf,
+                win_sec,
+                freq_range[0],
+                freq_range[1],
+                trimperc,
+                cmap,
+                ax1,
             )
-            cbar.ax.set_ylabel("Log Power (dB / Hz)", rotation=90, labelpad=20)
-            # Revert font-size
-            plt.rcParams.update({"font.size": old_fontsize})
-            return fig
-
-        fig, (ax0, ax1) = plt.subplots(
-            nrows=2, figsize=(12, 6), gridspec_kw={"height_ratios": [1, 2]}
-        )
-        plt.subplots_adjust(hspace=0.1)
 
-        # Hypnogram (top axis)
-        self.__plot_hypnogram(sf, hypno, ax0)
-        # Spectrogram (bottom axis)
-        self.__plot_spectrogram(data, sf, win_sec, fmin, fmax, trimperc, cmap, ax1)
-        # Revert font-size
-        plt.rcParams.update({"font.size": old_fontsize})
-        return fig
+        # Save the figure if 'save' set to True
+        if save and fig:
+            fig.savefig(
+                self.output_dir / self.__class__.__name__ / f"spectrogram.png",
+                bbox_inches="tight",
+            )
 
     @staticmethod
     def __plot_hypnogram(sf, hypno, ax0):
+        """Adapted from :py:func:`yasa:yasa.plot_hypnogram`."""
         from pandas import Series
 
         hypno = np.asarray(hypno).astype(int)
         t_hyp = np.arange(hypno.size) / (sf * 3600)
         # Make sure that REM is displayed after Wake
         hypno = Series(hypno).map({-2: -2, -1: -1, 0: 0, 1: 2, 2: 3, 3: 4, 4: 1}).values
         # Hypnogram (top axis)
@@ -410,22 +454,23 @@
             ax0.set_ylim(-4.5, 1.5)
         else:
             # No artefacts or Unscored
             ax0.set_yticks([0, -1, -2, -3, -4])
             ax0.set_yticklabels(["W", "R", "N1", "N2", "N3"])
             ax0.set_ylim(-4.5, 0.5)
         ax0.set_xlim(0, t_hyp.max())
-        ax0.set_ylabel("Stage")
+        # ax0.set_ylabel("Stage")
         ax0.xaxis.set_visible(False)
         ax0.spines["right"].set_visible(False)
         ax0.spines["top"].set_visible(False)
         return ax0
 
     @staticmethod
     def __plot_spectrogram(data, sf, win_sec, fmin, fmax, trimperc, cmap, ax):
+        """Adapted from :py:func:`yasa:yasa.plot_spectrogram`."""
         from matplotlib.colors import Normalize
         from lspopt import spectrogram_lspopt
         import numpy as np
 
         # Calculate multi-taper spectrogram
         nperseg = int(win_sec * sf)
         f, t, Sxx = spectrogram_lspopt(data, sf, nperseg=nperseg, noverlap=0)
@@ -451,35 +496,38 @@
         return im
 
 
 @define(kw_only=True)
 class SpindlesPipe(BaseEventPipe):
     """Spindles detection."""
 
+    @logger_wraps()
     def detect(
         self,
         picks: str | Iterable[str] = ("eeg"),
+        reference: Iterable[str] | str = "average",
         include: Iterable[int] = (1, 2, 3),
         freq_sp: Iterable[float] = (12, 15),
         freq_broad: Iterable[float] = (1, 30),
         duration: Iterable[float] = (0.5, 2),
         min_distance: int = 500,
         thresh: dict = {"corr": 0.65, "rel_pow": 0.2, "rms": 1.5},
         multi_only: bool = False,
         remove_outliers: bool = False,
         verbose: bool = False,
         save: bool = False,
     ):
-        """Wrapper around YASA's `spindles_detect <https://raphaelvallat.com/
-        yasa/build/html/generated/yasa.spindles_detect.html>`_.
-        """
+        """A wrapper around :py:func:`yasa:yasa.spindles_detect` with option to save."""
         from yasa import spindles_detect
 
         self.results = spindles_detect(
-            data=self.mne_raw.copy().load_data().set_eeg_reference().pick(picks),
+            data=self.mne_raw.copy()
+            .load_data()
+            .set_eeg_reference(ref_channels=reference)
+            .pick(picks),
             hypno=self.hypno_up,
             verbose=verbose,
             include=include,
             freq_sp=freq_sp,
             freq_broad=freq_broad,
             duration=duration,
             min_distance=min_distance,
@@ -491,36 +539,39 @@
             self._save_to_csv()
 
 
 @define(kw_only=True)
 class SlowWavesPipe(BaseEventPipe):
     """Slow waves detection."""
 
+    @logger_wraps()
     def detect(
         self,
         picks: str | Iterable[str] = ("eeg"),
+        reference: Iterable[str] | str = "average",
         include: Iterable[int] = (1, 2, 3),
         freq_sw: Iterable[float] = (0.3, 1.5),
         dur_neg: Iterable[float] = (0.3, 1.5),
         dur_pos: Iterable[float] = (0.1, 1),
         amp_neg: Iterable[float] = (40, 200),
         amp_pos: Iterable[float] = (10, 150),
         amp_ptp: Iterable[float] = (75, 350),
         coupling: bool = False,
         coupling_params: dict = {"freq_sp": (12, 16), "p": 0.05, "time": 1},
         remove_outliers: bool = False,
         save: bool = False,
     ):
-        """Wrapper around YASA's `sw_detect <https://raphaelvallat.com/yasa/
-        build/html/generated/yasa.sw_detect.html>`_.
-        """
+        """A wrapper around :py:func:`yasa:yasa.sw_detect` with option to save."""
         from yasa import sw_detect
 
         self.results = sw_detect(
-            data=self.mne_raw.copy().load_data().set_eeg_reference().pick(picks),
+            data=self.mne_raw.copy()
+            .load_data()
+            .set_eeg_reference(ref_channels=reference)
+            .pick(picks),
             hypno=self.hypno_up,
             verbose=False,
             include=include,
             freq_sw=freq_sw,
             dur_neg=dur_neg,
             dur_pos=dur_pos,
             amp_neg=amp_neg,
@@ -531,34 +582,36 @@
             remove_outliers=remove_outliers,
         )
         if save:
             self._save_to_csv()
 
 
 @define(kw_only=True)
-class REMsPipe(BaseEventPipe):
+class RapidEyeMovementsPipe(BaseEventPipe):
     """Rapid eye movements detection."""
 
+    @logger_wraps()
     def detect(
         self,
         loc_chname: str = "E46",
         roc_chname: str = "E238",
+        reference: Iterable[str] | str = "average",
         include: int | Iterable[int] = 4,
         freq_rem: Iterable[float] = (0.5, 5),
         duration: Iterable[float] = (0.3, 1.2),
         amplitude: Iterable[float] = (50, 325),
         remove_outliers: bool = False,
         save: bool = False,
     ):
-        """Wrapper around YASA's `rem_detect <https://raphaelvallat.com/yasa/
-        build/html/generated/yasa.rem_detect.html>`_.
-        """
+        """A wrapper around :py:func:`yasa:yasa.rem_detect` with option to save."""
         from yasa import rem_detect
 
-        referenced = self.mne_raw.copy().load_data().set_eeg_reference()
+        referenced = (
+            self.mne_raw.copy().load_data().set_eeg_reference(ref_channels=reference)
+        )
         loc = referenced.get_data([loc_chname], units="uV", reject_by_annotation="NaN")
         roc = referenced.get_data([roc_chname], units="uV", reject_by_annotation="NaN")
         self.results = rem_detect(
             loc=loc,
             roc=roc,
             sf=self.sf,
             hypno=self.hypno_up,
@@ -568,59 +621,38 @@
             duration=duration,
             amplitude=amplitude,
             remove_outliers=remove_outliers,
         )
         if save:
             self._save_to_csv()
 
-    def plot_average(self, save=False, yasa_args=None):
-        yasa_args = yasa_args or dict()
-        self.results.plot_average(**yasa_args)
-        if save:
-            self._save_avg_fig()
-
     def plot_topomap(self):
         raise AttributeError("'REMsPipe' object has no attribute 'plot_topomap'")
 
     def plot_topomap_collage(self):
         raise AttributeError("'REMsPipe' object has no attribute 'plot_topomap'")
 
 
 @define(kw_only=True)
-class CombinedPipe(BaseSpectrum):
+class GrandPipe(SpectrumPlots):
     """The pipeline element combining results from multiple subjects.
 
     Contains methods for computing and plotting combined PSD,
     spectrogram and topomaps, per sleep stage.
     """
 
+    psds: dict = field(init=False, factory=dict)
+    """Instances of :class:`.SleepSpectrum` per sleep stage.
+    """
+
     pipes: Iterable[BaseHypnoPipe] = field()
     """Stores pipeline elements for multiple subjects.
     """
 
     mne_raw: mne.io.Raw = field(init=False)
 
     @mne_raw.default
     def _get_mne_raw_from_pipe(self):
         return self.pipes[0].mne_raw
 
-    def _compute_psd_per_stage(self, picks, sleep_stages, sec_per_seg, avg_ref, dB):
-        psd_per_stage = {}
-        psds = []
-        for pipe in self.pipes:
-            psds.append(
-                pipe._compute_psd_per_stage(
-                    picks=picks,
-                    sleep_stages=sleep_stages,
-                    sec_per_seg=sec_per_seg,
-                    avg_ref=avg_ref,
-                    dB=dB,
-                )
-            )
-
-        for stage in sleep_stages:
-            psd_per_stage[stage] = [
-                psds[0][stage][0],
-                np.sum([psd[stage][1] for psd in psds], axis=0) / len(self.pipes),
-                round(sum([psd[stage][2] for psd in psds]) / len(self.pipes), 2),
-            ]
-        return psd_per_stage
+    def compute_psds_per_stage(self):
+        ...
```

