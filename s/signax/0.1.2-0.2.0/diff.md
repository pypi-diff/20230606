# Comparing `tmp/signax-0.1.2.tar.gz` & `tmp/signax-0.2.0.tar.gz`

## Comparing `signax-0.1.2.tar` & `signax-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 signax-0.1.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 signax-0.1.2/.gitattributes
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 signax-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 signax-0.1.2/.readthedocs.yml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 signax-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 signax-0.1.2/noxfile.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 signax-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 signax-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0    30518 2020-02-02 00:00:00.000000 signax-0.1.2/assets/backward_cpu.png
--rw-r--r--   0        0        0    29589 2020-02-02 00:00:00.000000 signax-0.1.2/assets/backward_gpu.png
--rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 signax-0.1.2/assets/forward_cpu.png
--rw-r--r--   0        0        0    30986 2020-02-02 00:00:00.000000 signax-0.1.2/assets/forward_gpu.png
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 signax-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 signax-0.1.2/docs/index.rst
--rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 signax-0.1.2/examples/compare.ipynb
--rw-r--r--   0        0        0    23963 2020-02-02 00:00:00.000000 signax-0.1.2/examples/estimate_hurst.ipynb
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 signax-0.1.2/examples/fbm.py
--rw-r--r--   0        0        0   525790 2020-02-02 00:00:00.000000 signax-0.1.2/examples/generative_model.ipynb
--rw-r--r--   0        0        0    43878 2020-02-02 00:00:00.000000 signax-0.1.2/examples/inversion.ipynb
--rw-r--r--   0        0        0    12578 2020-02-02 00:00:00.000000 signax-0.1.2/examples/nets.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/brownian_motion.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/dataloader.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/ornstein_uhlenbeck.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/signature_normalization.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/__init__.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/py.typed
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/signature.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/signature_flattened.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/tensor_ops.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/utils.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/_compat/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/_compat/typing.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_package.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_signature.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_tensor_ops.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 signax-0.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 signax-0.1.2/LICENSE
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 signax-0.1.2/README.md
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 signax-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 signax-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 signax-0.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 signax-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 signax-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 signax-0.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 signax-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 signax-0.2.0/noxfile.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 signax-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 signax-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    68830 2020-02-02 00:00:00.000000 signax-0.2.0/assets/backward_cpu.png
+-rw-r--r--   0        0        0    67192 2020-02-02 00:00:00.000000 signax-0.2.0/assets/backward_gpu.png
+-rw-r--r--   0        0        0    67406 2020-02-02 00:00:00.000000 signax-0.2.0/assets/forward_cpu.png
+-rw-r--r--   0        0        0    67792 2020-02-02 00:00:00.000000 signax-0.2.0/assets/forward_gpu.png
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 signax-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 signax-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0    48260 2020-02-02 00:00:00.000000 signax-0.2.0/examples/compare.ipynb
+-rw-r--r--   0        0        0    36683 2020-02-02 00:00:00.000000 signax-0.2.0/examples/estimate_hurst.ipynb
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 signax-0.2.0/examples/fbm.py
+-rw-r--r--   0        0        0   504474 2020-02-02 00:00:00.000000 signax-0.2.0/examples/generative_model.ipynb
+-rw-r--r--   0        0        0    76892 2020-02-02 00:00:00.000000 signax-0.2.0/examples/inversion.ipynb
+-rw-r--r--   0        0        0    12610 2020-02-02 00:00:00.000000 signax-0.2.0/examples/nets.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 signax-0.2.0/examples/requirements.txt
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 signax-0.2.0/examples/utils/brownian_motion.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 signax-0.2.0/examples/utils/dataloader.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 signax-0.2.0/examples/utils/ornstein_uhlenbeck.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 signax-0.2.0/examples/utils/signature_normalization.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/__init__.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/py.typed
+-rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/signatures.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/tensor_ops.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/utils.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/_compat/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 signax-0.2.0/src/signax/_compat/typing.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 signax-0.2.0/tests/test_module.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 signax-0.2.0/tests/test_package.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 signax-0.2.0/tests/test_signature.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 signax-0.2.0/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 signax-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 signax-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 signax-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 signax-0.2.0/README.md
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 signax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 signax-0.2.0/PKG-INFO
```

### Comparing `signax-0.1.2/.pre-commit-config.yaml` & `signax-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/CONTRIBUTING.md` & `signax-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/noxfile.py` & `signax-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/.github/workflows/ci.yml` & `signax-0.2.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,25 @@
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v3.1.4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+
+      - name: Run examples
+        run: |
+          cd examples
+          python -m pip install -r requirements.txt
+          python -m pip install jupyter nbclient
+          jupyter execute estimate_hurst.ipynb
+          jupyter execute generative_model.ipynb
+          jupyter execute inversion.ipynb
 
   dist:
     needs: [pre-commit]
     name: Distribution build
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `signax-0.1.2/docs/conf.py` & `signax-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/examples/compare.ipynb` & `signax-0.2.0/examples/compare.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995866935483871%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'source': {insert: [(6, 'from signax import "*

 * *            "signature')], delete: [6]}}, 3: {'attachments': OrderedDict()}, 5: {'attachments': "*

 * *            "OrderedDict()}, 18: {'attachments': OrderedDict()}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Benchmark between Signatory and Signax\n",
                 "\n",
                 "This is just a rough comparison. "
             ]
@@ -21,15 +22,15 @@
             "source": [
                 "import jax\n",
                 "import jax.numpy as jnp\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import signatory\n",
                 "import torch\n",
-                "from signax.signature import signature  # noqa: E501"
+                "from signax import signature"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
@@ -68,14 +69,15 @@
                 "        func(self.jax_path, self.depth)\n",
                 "\n",
                 "    def run_torch(self, func):\n",
                 "        func(self.torch_path, self.depth)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Function we want to test"
             ]
         },
         {
@@ -109,14 +111,15 @@
                 "def torch_signature_backward(X, depth):\n",
                 "    sig = signatory.signature(X.requires_grad_(True), depth)\n",
                 "    loss = torch.sum(sig)\n",
                 "    loss.backward()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Typical case with GPU"
             ]
         },
         {
@@ -389,14 +392,15 @@
                 "ax.set_title(f\"Depth={depth}, Size={size}, Platform={platform.upper()}\")\n",
                 "ax.set_yticks(range(len(names)))\n",
                 "ax.set_yticklabels(names)\n",
                 "fig.savefig(\"../assets/backward_gpu.png\", dpi=256)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Typical case with CPU\n",
                 "\n",
                 "NOTE: The below result is done by restarting the notebook and skipping GPU setting because JAX does not reload the platform"
             ]
```

### Comparing `signax-0.1.2/examples/fbm.py` & `signax-0.2.0/examples/fbm.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/examples/inversion.ipynb` & `signax-0.2.0/examples/estimate_hurst.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9295544617419618%*

 * *Differences: {"'cells'": "{0: {'source': ['## Learn Hurst exponent for fractional Brownian Motion\\n'], "*

 * *            "'attachments': OrderedDict()}, 1: {'source': {insert: [(1, 'import fbm\\n'), (6, "*

 * *            "'import nets\\n'), (7, 'import optax  # https://github.com/deepmind/optax\\n')], "*

 * *            "delete: [7, 6, 5]}}, 2: {'source': ['n_paths_train = 200\\n', 'n_paths_test = 50\\n', "*

 * *            "'dt = 1e-2 / 3.0  # 300 time steps\\n', 'hurst_exponent = "*

 * *            "jnp.around(jnp.linspace(0.2, 0.8, 7), de […]*

```diff
@@ -1,421 +1,296 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Signature Inversion\n",
-                "\n",
-                "This notebook follows Section 3.6 of [Deep Signature Transforms](https://arxiv.org/pdf/1905.08494.pdf). PyTorch code can be found at [this](https://github.com/patrick-kidger/Deep-Signature-Transforms/blob/master/src/example_signature_inversion.ipynb)"
+                "## Learn Hurst exponent for fractional Brownian Motion\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import equinox as eqx\n",
+                "import fbm\n",
                 "import jax\n",
                 "import jax.numpy as jnp\n",
                 "import jax.random as jrandom\n",
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "import optax\n",
-                "from signax.signature_flattened import signature\n",
+                "import nets\n",
+                "import optax  # https://github.com/deepmind/optax\n",
                 "\n",
                 "\n",
                 "jax.config.update(\"jax_platform_name\", \"cpu\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "seed = 1234\n",
-                "key = jrandom.PRNGKey(seed)\n",
-                "signature_depth = 12\n",
-                "learning_rate = 2 * 1e-3\n",
-                "num_training_iters = 5000"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Preprocessing data\n",
-                "Here we consider number 0"
+                "n_paths_train = 200\n",
+                "n_paths_test = 50\n",
+                "dt = 1e-2 / 3.0  # 300 time steps\n",
+                "hurst_exponent = jnp.around(jnp.linspace(0.2, 0.8, 7), decimals=7).tolist()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# number zero (PenDigit)\n",
-                "path = [29, 97, 0, 57, 22, 10, 68, 0, 100, 40, 83, 90, 37, 100, 12, 57]\n",
-                "path = np.array(path, dtype=float).reshape(-1, 2)\n",
-                "# rescale into range (-1,1)\n",
-                "path = -1.0 + 2 * (path - np.min(path)) / (np.max(path) - np.min(path))\n",
-                "path = jnp.array(path)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Let's visualize the data"
+                "def dataloader(arrays, batch_size, *, key):\n",
+                "    # this taken from equinox documentation\n",
+                "    dataset_size = arrays[0].shape[0]\n",
+                "    assert all(array.shape[0] == dataset_size for array in arrays)\n",
+                "    indices = jnp.arange(dataset_size)\n",
+                "    while True:\n",
+                "        perm = jrandom.permutation(key, indices)\n",
+                "        (key,) = jrandom.split(key, 1)\n",
+                "        start = 0\n",
+                "        end = batch_size\n",
+                "        while end < dataset_size:\n",
+                "            batch_perm = perm[start:end]\n",
+                "            yield tuple(array[batch_perm] for array in arrays)\n",
+                "            start = end\n",
+                "            end = start + batch_size"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "(-1.1, 1.1, -1.1, 1.1)"
-                        ]
-                    },
-                    "execution_count": 4,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                },
-                {
-                    "data": {
-                        "image/png": "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",
-                        "text/plain": [
-                            "<Figure size 432x288 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "plt.plot(*path.T, label=\"Original path\", linewidth=10, linestyle=\"-\")\n",
-                "plt.axis(\"off\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
+            "outputs": [],
             "source": [
-                "Compute signature of the given data"
+                "def generate_data(key):\n",
+                "    train_key, test_key = jrandom.split(key)\n",
+                "    X_train, Y_train = [], []\n",
+                "    X_test, Y_test = [], []\n",
+                "    # generate train\n",
+                "    for hurst in hurst_exponent:\n",
+                "        train_key, _ = jrandom.split(train_key)\n",
+                "        X = fbm.generate_fbm(\n",
+                "            hurst=hurst,\n",
+                "            n_paths=n_paths_train,\n",
+                "            dt=dt,\n",
+                "            key=train_key,\n",
+                "        )\n",
+                "        Y = jnp.array([hurst] * n_paths_train)\n",
+                "        X_train.append(X)\n",
+                "        Y_train.append(Y)\n",
+                "\n",
+                "    # generate test\n",
+                "    for hurst in hurst_exponent:\n",
+                "        test_key, _ = jrandom.split(test_key)\n",
+                "        X = fbm.generate_fbm(\n",
+                "            hurst=hurst,\n",
+                "            n_paths=n_paths_test,\n",
+                "            dt=dt,\n",
+                "            key=test_key,\n",
+                "        )\n",
+                "        Y = jnp.array([hurst] * n_paths_test)\n",
+                "        X_test.append(X)\n",
+                "        Y_test.append(Y)\n",
+                "\n",
+                "    X_train = jnp.concatenate(X_train)\n",
+                "    Y_train = jnp.concatenate(Y_train)\n",
+                "    X_test = jnp.concatenate(X_test)\n",
+                "    Y_test = jnp.concatenate(Y_test)\n",
+                "\n",
+                "    return (\n",
+                "        X_train[..., None],\n",
+                "        Y_train[..., None],\n",
+                "        X_test[..., None],\n",
+                "        Y_test[..., None],\n",
+                "    )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sig = signature(path, depth=signature_depth)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Model\n",
-                "\n",
-                "This model is quite simple: set of parameters (in `eqx.nn.Linear`) represents the path.\n",
-                "\n",
-                "The model outputs the signature of the learnable parameters."
+                "seed = 1234\n",
+                "key = jrandom.PRNGKey(seed)\n",
+                "data_key, loader_key, model_key = jrandom.split(key, 3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "class InvertSignature(eqx.Module):\n",
-                "    path_length: int\n",
-                "    signature_depth: int\n",
-                "\n",
-                "    # path represented as weight of linear layer\n",
-                "    # can instead use `jnp.ndarray`\n",
-                "    path: eqx.nn.Linear\n",
-                "\n",
-                "    def __init__(self, path_length, signature_depth, *, key) -> None:\n",
-                "        self.path_length = path_length\n",
-                "        self.signature_depth = signature_depth\n",
-                "\n",
-                "        self.path = eqx.nn.Linear(\n",
-                "            in_features=1,\n",
-                "            out_features=2 * path_length,\n",
-                "            use_bias=False,\n",
-                "            key=key,\n",
-                "        )\n",
-                "\n",
-                "    def generate_path(self, x):\n",
-                "        x = self.path(x)\n",
-                "        return jnp.reshape(x, (self.path_length, 2))\n",
-                "\n",
-                "    def __call__(self, x):\n",
-                "        x = self.generate_path(x)\n",
-                "        return signature(path=x, depth=signature_depth)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Model instantiation"
+                "X_train, Y_train, X_test, Y_test = generate_data(key=data_key)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
-                "model = InvertSignature(\n",
-                "    path_length=path.shape[0], signature_depth=signature_depth, key=key\n",
+                "model = nets.create_simple_net(\n",
+                "    dim=1,\n",
+                "    signature_depth=3,\n",
+                "    augment_layer_size=(3,),\n",
+                "    augmented_kernel_size=3,\n",
+                "    mlp_width=32,\n",
+                "    mlp_depth=5,\n",
+                "    output_size=1,\n",
+                "    final_activation=jax.nn.sigmoid,\n",
+                "    key=model_key,\n",
                 ")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Create optimizer"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "optim = optax.adam(learning_rate=learning_rate)\n",
+                "iter_data = dataloader((X_train, Y_train), batch_size=128, key=loader_key)\n",
+                "optim = optax.adam(learning_rate=1e-3)\n",
                 "opt_state = optim.init(eqx.filter(model, eqx.is_array))"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "A normalization term to compute the loss. The idea here is to penalize more higher order of signatures"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
-                "normalization = [\n",
-                "    np.floor(np.log(i + 1) / np.log(2))\n",
-                "    for i in range(1, 2 ** (signature_depth + 1) - 1)\n",
-                "]\n",
-                "normalization = jnp.array(normalization)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "In fact, the input of the model is fixed"
+                "@eqx.filter_value_and_grad\n",
+                "def compute_loss(model, x, y):\n",
+                "    pred_y = jax.vmap(model)(x)\n",
+                "    assert pred_y.shape[0] == y.shape[0]\n",
+                "    return jnp.mean(jnp.square(pred_y - y))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
-                "x = jnp.ones((1, 1))\n",
-                "y = sig"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Compute loss in Equinox style"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "@eqx.filter_value_and_grad\n",
-                "def compute_loss(model):\n",
-                "    pred_sig = model(x)\n",
-                "    diff = y - pred_sig\n",
-                "    diff = diff * normalization\n",
-                "    return jnp.log(jnp.mean(diff**2))\n",
-                "\n",
-                "\n",
                 "@eqx.filter_jit\n",
-                "def make_step(model, opt_state):\n",
-                "    loss, grads = compute_loss(model)\n",
+                "def make_step(model, x, y, opt_state):\n",
+                "    loss, grads = compute_loss(model, x, y)\n",
                 "    updates, opt_state = optim.update(grads, opt_state)\n",
                 "    model = eqx.apply_updates(model, updates)\n",
                 "    return loss, model, opt_state"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Training step"
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Iter=0 \t loss=2.1267\n",
-                        "Iter=500 \t loss=-7.2811\n",
-                        "Iter=1000 \t loss=-7.6965\n",
-                        "Iter=1500 \t loss=-8.0481\n",
-                        "Iter=2000 \t loss=-8.3618\n",
-                        "Iter=2500 \t loss=-8.6392\n",
-                        "Iter=3000 \t loss=-8.9132\n",
-                        "Iter=3500 \t loss=-9.1947\n",
-                        "Iter=4000 \t loss=-9.4898\n",
-                        "Iter=4500 \t loss=-9.7994\n"
+                        "step=0 \t loss=0.041261281818151474\n",
+                        "step=10 \t loss=0.03442611172795296\n",
+                        "step=20 \t loss=0.027970541268587112\n",
+                        "step=30 \t loss=0.02049068734049797\n",
+                        "step=40 \t loss=0.014842263422906399\n",
+                        "step=50 \t loss=0.01463926862925291\n",
+                        "step=60 \t loss=0.008735965006053448\n",
+                        "step=70 \t loss=0.0038531338796019554\n",
+                        "step=80 \t loss=0.0031830959487706423\n",
+                        "step=90 \t loss=0.0017226745840162039\n",
+                        "step=100 \t loss=0.0018800266552716494\n",
+                        "step=110 \t loss=0.0012469309149309993\n",
+                        "step=120 \t loss=0.001055217464454472\n",
+                        "step=130 \t loss=0.0011177064152434468\n",
+                        "step=140 \t loss=0.0009607287356629968\n",
+                        "step=150 \t loss=0.0007560442318208516\n",
+                        "step=160 \t loss=0.0006463633617386222\n",
+                        "step=170 \t loss=0.0007553303148597479\n",
+                        "step=180 \t loss=0.0006547534139826894\n",
+                        "step=190 \t loss=0.0005832671886309981\n",
+                        "step=200 \t loss=0.0005575551767833531\n",
+                        "step=210 \t loss=0.00035020316136069596\n",
+                        "step=220 \t loss=0.0004003815120086074\n",
+                        "step=230 \t loss=0.00045127380872145295\n",
+                        "step=240 \t loss=0.00031438778387382627\n",
+                        "step=250 \t loss=0.00036406281287781894\n",
+                        "step=260 \t loss=0.0002983828308060765\n",
+                        "step=270 \t loss=0.0002879476814996451\n",
+                        "step=280 \t loss=0.0002255685394629836\n",
+                        "step=290 \t loss=0.00022613670444115996\n",
+                        "step=300 \t loss=0.00024316016060765833\n",
+                        "step=310 \t loss=0.00021550750534515828\n",
+                        "step=320 \t loss=0.0002071917406283319\n",
+                        "step=330 \t loss=0.00019002672343049198\n",
+                        "step=340 \t loss=0.00013162200048100203\n",
+                        "step=350 \t loss=0.00012771754700224847\n",
+                        "step=360 \t loss=0.0001422253844793886\n",
+                        "step=370 \t loss=0.00019014824647456408\n",
+                        "step=380 \t loss=0.00012071082164766267\n",
+                        "step=390 \t loss=0.00010335109254810959\n",
+                        "step=400 \t loss=0.00016220123507082462\n",
+                        "step=410 \t loss=0.00010574463522061706\n",
+                        "step=420 \t loss=0.0001059367205016315\n",
+                        "step=430 \t loss=0.00015133402484934777\n",
+                        "step=440 \t loss=0.00012403847358655185\n",
+                        "step=450 \t loss=0.00010137465869775042\n",
+                        "step=460 \t loss=0.00010347012721467763\n",
+                        "step=470 \t loss=8.348895789822564e-05\n",
+                        "step=480 \t loss=9.372731437906623e-05\n",
+                        "step=490 \t loss=8.70665826369077e-05\n"
                     ]
                 }
             ],
             "source": [
-                "for i in range(num_training_iters):\n",
-                "    loss, model, opt_state = make_step(model, opt_state)\n",
+                "test_mse = []\n",
+                "for step, (x, y) in zip(range(500), iter_data):\n",
+                "    loss, model, opt_state = make_step(model, x, y, opt_state)\n",
                 "    loss = loss.item()\n",
-                "    if i % 500 == 0:\n",
-                "        print(f\"Iter={i} \\t loss={loss:.4f}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Helper function to refine path\n",
-                "The following two functions taken from [this file](https://github.com/patrick-kidger/Deep-Signature-Transforms/blob/master/src/signature_inversion.py)"
+                "    test_mse += [jnp.mean(jnp.square(jax.vmap(model)(X_test) - Y_test)).item()]\n",
+                "    if step % 10 == 0:\n",
+                "        print(f\"step={step} \\t loss={loss}\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "def _get_tree_reduced_steps(X, order=4, steps=4, tol=0.1):\n",
-                "    if len(X) < steps:\n",
-                "        return X\n",
-                "\n",
-                "    dim = X.shape[1]\n",
-                "\n",
-                "    # slide over a window size = `steps``\n",
-                "    for i in range(steps - 1, len(X)):\n",
-                "        # no redudancy in path -> compute its signature\n",
-                "        new_path = X[i - steps + 1 : i + 1]  # noqa: E203\n",
-                "        new_path_sig = signature(new_path, order)\n",
-                "\n",
-                "        # reduce the path with the first and the last\n",
-                "        new_path2 = jnp.r_[\n",
-                "            X[i - steps + 1].reshape(-1, dim),\n",
-                "            X[i].reshape(-1, dim),\n",
-                "        ]\n",
-                "        new_path2_sig = signature(new_path2, order)\n",
-                "\n",
-                "        # compute the difference between two signatures\n",
-                "        norm = jnp.linalg.norm(new_path_sig - new_path2_sig)\n",
-                "        if norm < tol:\n",
-                "            # if it is reducible, the perform the same procedure on the\n",
-                "            # next sub path\n",
-                "            return _get_tree_reduced_steps(np.r_[X[: i - steps + 2], X[i:]])\n",
-                "\n",
-                "    return X\n",
-                "\n",
-                "\n",
-                "def get_tree_reduced(X, order=4, tol=0.1):\n",
-                "    \"\"\"Removes tree-like pieces of the path.\"\"\"\n",
-                "    X = jnp.r_[X, [X[-1]]]\n",
-                "\n",
-                "    for step in range(3, len(X) + 1):\n",
-                "        X = _get_tree_reduced_steps(X, order, step, tol)\n",
-                "\n",
-                "    if (X[-1] == X[-2]).all():\n",
-                "        return X[:-1]\n",
-                "\n",
-                "    return X"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Plot result"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAi8AAAGdCAYAAADaPpOnAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABPeElEQVR4nO3de1xUdf4/8NeZGWa4Dle5g3hHBMELIpqZSXnLsntt37LLtltZW2u1a+12b7d2u7dR/bab7W5ll01ts4uG97uiKIgCKgjI/TYDAwzMzPn9MTDMcBGQy5kZXs/Hg8dj5pwzM+85mrz6XAVRFEUQEREROQiZ1AUQERER9QfDCxERETkUhhciIiJyKAwvRERE5FAYXoiIiMihMLwQERGRQ2F4ISIiIofC8EJEREQORSF1AYPNZDKhpKQEXl5eEARB6nKIiIioD0RRRH19PUJDQyGTXbhtxenCS0lJCSIiIqQug4iIiC5CUVERwsPDL3iN04UXLy8vAOYvr1arJa6GiIiI+kKr1SIiIsLye/xCnC68tHcVqdVqhhciIiIH05chHxywS0RERA7FacJLamoqYmJikJiYKHUpRERENIQEURRFqYsYTFqtFt7e3tBoNOw2IiIichD9+f3tNC0vRERENDIwvBAREZFDYXghIiIih8LwQkRERA6F4YWIiIgcCsMLERERORSGFyIiInIoDC9ERETkUBheiIiIyKEwvPSR3mDEvf86jO05FVKXQkRENKIxvPTRJ3sKsCW7HL/+9DA2HD0vdTlEREQjltOEl6HemPHuuWNwTUIoDCYRj3yZgQ93nR2SzyEiIqIL48aM/WAyiXj++2ys3VsAALh33hg8sWQyZDJhUD+HiIhopOHGjENEJhPwzPIYrFkSDQD4YFc+nlyfCZPJqfIfERGRXWN46SdBEHDf/HF47cZ4yARg3aEirPn2OAMMERHRMGF4uUjXzwjHGzcnQCYAXx0uxiubc6QuiYiIaERgeBmAaxLC8Pcb4gEA720/g88PFEpcERERkfNjeBmgG2aE45GUCQCApzdm4WhhrcQVEREROTeGl0Hw8MIJWDY1BAaTiIe+OApNU6vUJRERETkthpdBIAgCXrouDhF+biiubcKT32bCyWagExER2Q2Gl0GidnXBP26dDoVMwKbMUnxxsEjqkoiIiJwSw8sgSojwwR8Xm9eAeXFTNopqGiWuiIiIyPkwvAyyey4Zg1lRfmhsMeLJ9ew+IiIiGmwML4NMJhPw8vVxUClk2JVXhW/Si6UuiYiIyKkwvAyBsaM88fsrJgIAXvg+GxXaZokrIiIich4ML0Pk15eMQVyYN7TNBjy1MYvdR0RERIOE4WWIKOQy/O36qVDIBPx8ohw/nyiXuiQiIiKn4DThJTU1FTExMUhMTJS6FIuYUDV+O38sAHP3UVOLUeKKiIiIHJ8gOll/hlarhbe3NzQaDdRqtdTloKnFiJTXd+B8XRN+d/l4rL5yktQlERER2Z3+/P52mpYXe+WmlOPPyyYDAN7feRbnqnUSV0REROTYGF6GweLYYMybEIAWgwnP/y9b6nKIiIgcGsPLMBAEAc8snwKFTEDaqQqkneTgXSIioovF8DJMxgd64p5LxgAAnv8+G82tHLxLRER0MRhehtFDCycgSK3CuepGfLjrrNTlEBEROSSGl2HkqVLgyaXmwbvvbDuN4lpu3EhERNRfDC/D7Or4UCSN8UNzqwl/2XRS6nKIiIgcDsPLMBMEAc9dMwVymYAfs8qwK69S6pKIiIgcCsOLBKKD1bgjeTQAYM1/M1HX2CJxRURERI6D4UUij145CVH+7jhf14Q/fHOcGzcSERH1EcOLRDxVCvzj1ulwkQvYnF2Of+8/J3VJREREDoHhRUJx4d54Yol59tGL35/EiRKNxBURERHZP4YXid01NwopkwPRYjTh4XUZ3HmaiIioFwwvEhMEAX+/IR6BXiqcrmjAX37g3kdEREQXwvBiB/w8lHjtpngAwH/2F2JLNvc+IiIi6gnDi52YN2EU7p1n3vvoD98cQ2W9XuKKiIiI7BPDix15bNEkTA5Ro7axFc98lyV1OURERHaJ4cWOqBRyvHLDVChkAn7ILMMPmaVSl0RERGR3GF7sTGyYN+6/bBwA4OmNWajRcfVdIiIiawwvdujBy8djYpAnqhpa8Nz/TkhdDhERkV1heLFD5u6jeMgEYGNGCWcfERERWXGa8JKamoqYmBgkJiZKXcqgiI/wwb2XjgUAPPvdCTS3cvE6IiIiABBEJ9sRUKvVwtvbGxqNBmq1WupyBqSpxYiFr21HiaYZj105EQ9ePkHqkoiIiIZEf35/O03LizNyU8rxxyXRAIB3t59BubZZ4oqIiIikx/Bi566OD8W0SB80thjxys85UpdDREQkOYYXOycIAp6+KgYA8E16MTKLufM0ERGNbAwvDmBapC+unRYGAHj++xNwsmFKRERE/cLw4iD+sHgS3FzkOFRQi01ceZeIiEYwhhcHEeLtht/ON0+dfumHU5w6TUREIxbDiwP57aXjEOLtivN1Tfhod77U5RAREUmC4cWBuCnl+OPitqnT206jop5Tp4mIaORheHEwV8eHIj7CB7oWI177OVfqcoiIiIYdw4uDkck6pk5/lV6EEyWcOk1ERCMLw4sDmjHaF8vjQyGKwPP/y+bUaSIiGlEYXhzUHxdPgkohw4H8Gvx8grtOExHRyMHw4qDCfd3xm7Zdp1/68ST0Bk6dJiKikYHhxYHdN38cAr1UOFfdiE/3FkhdDhER0bBgeHFgHioFHl80CQDwj7TTqG7QS1wRERHR0GN4cXDXTw9HbJga9XoDXt/CqdNEROT8GF4cnEwm4Kll5qnTXxwsxKkyrcQVERERDS2GFyeQNNYfS+OCYRKBF78/yanTRETk1BhenMSaxZOhlMuw+3QVtp6qkLocIiKiIcPw4iQi/d1x9yVjAAB/2XQSrUaTxBURERENDYYXJ7JqwTgEeCpxtkqHf+87J3U5REREQ4LhxYl4ubrg0SvNU6ff/CUXtboWiSsiIiIafAwvTuammRGIDvaCttmAD3eflbocIiKiQcfw4mTkMgG/v2IiAODTvedQ18jWFyIici4ML07oislBiA72QoPegI9350tdDhER0aBieHFCMpmAhxdOAAB8sqcAmsZWiSsiIiIaPAwvTmrRlGBMCvJCvd6Aj/ew9YWIiJwHw4uTkskE/K6t9eXjPfnQNLH1hYiInAPDixNbEhuMCYGeqG824NO9BVKXQ0RENCgYXpyYTCbgobbWl49256O+ma0vRETk+BhenNyyuBCMG+UBTVMrW1+IiMgp2F14KSoqwmWXXYaYmBhMnToVX3/9tdQlOTS51diXtXsLoDcYJa6IiIhoYOwuvCgUCrz55pvIzs7G5s2b8cgjj0Cn00ldlkNbGheCYLUrqhpa8GNmmdTlEBERDYjdhZeQkBAkJCQAAIKDgxEQEICamhppi3JwLnIZbkuKBAB8uq9A2mKIiIgGqN/hZefOnVi+fDlCQ0MhCAI2bNjQ5ZrU1FRERUXB1dUVSUlJOHjw4EUVl56eDqPRiIiIiIt6PXW4ZVYkXOQCjhbWIbNYI3U5REREF63f4UWn0yE+Ph6pqandnv/yyy+xevVqPPPMMzhy5Aji4+OxaNEiVFRUWK5JSEhAbGxsl5+SkhLLNTU1Nbjjjjvwz3/+84L16PV6aLVamx/qapSXCkvjQgAA/2LrCxEROTBBFEXxol8sCFi/fj1WrFhhOZaUlITExES88847AACTyYSIiAg89NBDWLNmTZ/eV6/X44orrsC9996L22+//YLXPvvss3juuee6HNdoNFCr1X3/MiNA+rlaXP/eXigVMhx4YiF8PZRSl0RERAQA0Gq18Pb27tPv70Ed89LS0oL09HSkpKR0fIBMhpSUFOzbt69P7yGKIu68805cfvnlvQYXAHjiiSeg0WgsP0VFRRddv7ObHumD2DA1WgwmfJNeLHU5REREF2VQw0tVVRWMRiOCgoJsjgcFBaGsrG+zXPbs2YMvv/wSGzZsQEJCAhISEpCZmdnj9SqVCmq12uaHuicIAm5ONA/c/e5YSS9XExER2SeF1AV0dskll8BkMkldhtNaEhuMZzZmIfO8BgVVOkQFeEhdEhERUb8MastLQEAA5HI5ysvLbY6Xl5cjODh4MD+KLlKApwpzxgUAADZllkpcDRERUf8NanhRKpWYMWMG0tLSLMdMJhPS0tKQnJw8mB9FA3DVVPOso/+x64iIiBxQv8NLQ0MDMjIykJGRAQDIz89HRkYGCgsLAQCrV6/GBx98gE8//RQnT57E/fffD51Oh7vuumtQC+8sNTUVMTExSExMHNLPcQaLY4OhkAk4VVaP0xUNUpdDRETUL/2eKr19+3YsWLCgy/GVK1di7dq1AIB33nkHr7zyCsrKypCQkIC3334bSUlJg1Jwb/oz1Woku/OTg9ieU4lHUibgkZSJUpdDREQjXH9+fw9onRd7xPDSN9+kF+Oxr49hQqAntqyeL3U5REQ0wkm2zgs5jiunBEEplyGvogE5ZfVSl0NERNRnDC8jlNrVBZdOHAUA+P44B+4SEZHjYHgZwZbHm2cdfX+8FE7We0hERE6M4WUEWzg5CCqFDPlVOpwo4YaWRETkGJwmvHCqdP95qhS4PDoQgLn1hYiIyBE4TXhZtWoVsrOzcejQIalLcShXTQ0FYB73wq4jIiJyBE4TXujiXB4dCHelHMW1TThWrJG6HCIiol4xvIxwbko5Fk427wL+PbcLICIiB8DwQlgWZ551tCmzFCYTu46IiMi+MbwQLps0Cp4qBUo1zThSWCt1OURERBfE8EJwdZHjipi2riPOOiIiIjvnNOGFU6UH5qqpHV1HRnYdERGRHXOa8MKp0gMzb8IoqF0VqKzX41BBjdTlEBER9chpwgsNjFIhw6IpwQC41xEREdk3hheyuCrevGDdj5llMBhNEldDRETUPYYXspgzzh++7i6o1rVg/1l2HRERkX1ieCELF7kMi2Pbd5pm1xEREdknhheysbxt1tFPJ8rQyq4jIiKyQwwvZCNprD8CPFWoa2zF7tNVUpdDRETUBcML2ZDLBCyJNc862nyiTOJqiIiIunKa8MJF6gbP5dGBAICduVUQRS5YR0RE9sVpwgsXqRs8SWP9oJTLcL6uCWerdFKXQ0REZMNpwgsNHnelAoljfAEAO3MrJa6GiIjIFsMLdevSCaMAALvyOGiXiIjsC8MLdWteW3jZd6YaeoNR4mqIiIg6MLxQtyaHeGGUlwpNrUakF9RKXQ4REZEFwwt1SxAEzJsQAADYkcdxL0REZD8YXqhH8ye2jXvJ5bgXIiKyHwwv1KO5480tL9mlWlTUN0tcDRERkRnDC/UowFOF2DA1APPAXSIiInvgNOGFK+wOjTnjzK0ve08zvBARkX1wmvDCFXaHRvI4fwDA3rMc90JERPbBacILDY3EKD8oZAKKappQVNModTlEREQML3RhnioF4iN8AAD7zrLriIiIpMfwQr1KHmvuOuKgXSIisgcML9SrOe3jXs5UQRRFiashIqKRjuGFejV9tC+UChnKtXqcrdJJXQ4REY1wDC/UK1cXOWZE+gIA9rLriIiIJMbwQn3S3nW07wynTBMRkbQYXqhPksd1DNrluBciIpISwwv1ydRwH6gUMtQ2tiKf416IiEhCDC/UJ0qFDHFh3gCA9HO1EldDREQjGcML9dn00eZBu0cK66QthIiIRjSnCS/cmHHoTY/0AQAcLWTLCxERScdpwgs3Zhx609umS+eU16O+uVXiaoiIaKRymvBCQy9Q7YpwXzeIInCsSCN1OURENEIxvFC/tLe+cNAuERFJheGF+qV93Mvu05XSFkJERCMWwwv1y8LJQXCRCzhUUIttORVSl0NERCMQwwv1S4SfO+6cEwUAeGfraWmLISKiEYnhhfrt3nljoZAJSD9Xi5yyeqnLISKiEYbhhfotUO2KlMlBAID/HimWuBoiIhppGF7ooiyKNYeXwwU1EldCREQjDcMLXZRpEeYp01nntdAbjBJXQ0REIwnDC12U0f7u8PNQosVowokSrdTlEBHRCMLwQhdFEATLmi/sOiIiouHE8EIXbe74AADAL9lc74WIiIYPwwtdtEVTggEAh87VoKK+WeJqiIhopGB4oYsW6uOG+HBviCKQygXriIhomDhNeElNTUVMTAwSExOlLmVEeSRlIgDg033nsO9MtcTVEBHRSOA04WXVqlXIzs7GoUOHpC5lRFkQHYhfJUUCAN7dztYXIiIaek4TXkg6988fB7lMwK68KuRX6aQuh4iInBzDCw1YhJ87pkX4AACOFdVJWgsRETk/hhcaFFNC1QCA7FIuWEdEREOL4YUGRUxbeDlRopG4EiIicnYMLzQoYkK8AQDZJVqIoihxNURE5MwYXmhQTAz2hEImoLaxlYN2iYhoSDG80KBQKeSYPdYfALAlu1ziaoiIyJkxvNCgWTQlCADwr33noGlslbgaIiJyVgwvNGiunBIMpUKG83VNWPnJQY59ISKiIcHwQoMmSO2KD+6YCQDIKKrjtGkiIhoSDC80qOZPHIUlsebdpv93rFTiaoiIyBkxvNCgWx4fCgDYcPQ8DEaTxNUQEZGzYXihQbdwciD8PJQo0zYj7VSF1OUQEZGTYXihQadSyHHTzAgAwNMbs3CSY1+IiGgQMbzQkLh33hhMCPREuVaPBz8/Ar3BKHVJRETkJBheaEj4e6rw9X3JCPBU4UylDp/tL5S6JCIichIMLzRkfNyVWLVgHABgc3aZxNUQEZGzYHihIbVgUiAAIP1cLRr0BomrISIiZ8DwQkMqKsADkX7uaDWK2HO6SupyiIjICTC80JC7Isa859FXh4okroSIiJwBwwsNuduSIgEAW3MqcK5aJ3E1RETk6JwmvKSmpiImJgaJiYlSl0KdjB3lifkTR0EUzTtOExERDYTThJdVq1YhOzsbhw4dkroU6sadc6IAmLuOOHCXiIgGwmnCC9m3+RNHYWyAB+r1BsQ+8zPe33EGoihKXRYRETkghhcaFjKZgCeXTrY8f/nHU9icXY66xhY8+90J5JTVS1gdERE5EoYXGjYpMUGWResA4LnvTuDhdRlYu7cAd35yUMLKiIjIkTC80LB6fFE0Tj6/GGE+bijRNGNHbiUAoFTTjBaDSeLqiIjIETC80LBzU8rx3NVTuhw/Vlw3/MUQEZHDYXghSaTEBOHl6+LgrpRbju09XS1hRURE5CgYXkgyt8yKROazi/DiilgAwN4z3D6AiIh6x/BCkpLLBMwZ5w8AOFpYh6YWIwxGEzafKMP3x0skro6IiOyRQuoCiMYEeCBY7YoybTMmP/2TzblQHzdMj/SVqDIiIrJHbHkhyQmCgAXRo7o99+rPOcNcDRER2Tu2vJBdWLN4MhKj/OChUmDdwUJkFNWhtrEVe89UI79KhzEBHlKXSEREdoLhheyCt7sLrpseDgBYNCUYALDy44PYkVuJ7zJK8HDKBCnLIyIiO8JuI7JbV8eHAgC+PFSI+uZWiashIiJ7wfBCdmtJXLBlJd4Xvs+WuhwiIrITDC9kt9yVCrxxcwIA4KvDxXh3+2k06A3SFkVERJJjeCG7NmuMH25JjAAA/P2nHMz+axp2tu2HREREIxPDC9m9p66KwW8vHYswHzc06A34/ZcZqKzXS10WERFJhOGF7J6HSoEnlk5G2qPzER3shWpdC/7wzTE0txqhaeJAXiKikUYQRVGUuojBpNVq4e3tDY1GA7VaLXU5NMhOlWlx9Tt70GIwWY4tiwvBP26dBplMkLAyIiIaiP78/mbLCzmU6GA1XrlhKpSKjr+6mzJLkXaqQsKqiIhoOHGROnI41ySEYWq4D4pqGrE9pxIf78nHO1vzsDA6kK0vREQjAFteyCGNCfDApRNH4b7LxsJDKcexYg0eWncU5+uapC6NiIiGGFteyKEFernij0ui8fTGE9h0vBQ7cypx5ZRgmEQRjy2ahDAfN6lLJCKiQcbwQg7v9tmjoXZ1wQe7zuJEiRb/PVIMADhZqsW3D8yBu5J/zYmInAm7jcjhCYKAFdPCsP6BuXjrlgTcPns0AOBUWT3+/lOOxNUREdFgY3ghp6FUyHBNQhheWBGLf98zCwCwdm8BMorqpC2MiIgGFcMLOaV5E0bhuulhAIAXv89GYXUjanUtEldFRESDgeGFnNYjCydCIRNw+FwtLn1lG6a9sAVPb8ySuiwiIhoghhdyWpH+7njtpniM8lJZjq07WAQdd6YmInJoDC/k1K5JCMPBJxfi9F+WIMzHDS1GE/afrZa6LCIiGgCGF3J6giBAIZdhQfQoAMC2HG4lQETkyOwuvNTV1WHmzJlISEhAbGwsPvjgA6lLIiexMDoIAPBNejFOlWklroaIiC6W3e0qbTQaodfr4e7uDp1Oh9jYWBw+fBj+/v59ej13laaeiKKIX31wAPvauo0SInzwt+unYmKQJ0QR3BeJiEhCDr2rtFwuh7u7OwBAr9dDFEXYWb4iByUIAl69KR5zx/tDEICMojpc9+4eJDy/BZf8bSs0ja1Sl0hERH3Q7/Cyc+dOLF++HKGhoRAEARs2bOhyTWpqKqKiouDq6oqkpCQcPHiwX59RV1eH+Ph4hIeH4/HHH0dAQEB/yyTqVpiPGz779Wzsf2IhJgZ5QtdihKapFSWaZuw6XSl1eURE1Af9Di86nQ7x8fFITU3t9vyXX36J1atX45lnnsGRI0cQHx+PRYsWoaKiY5Bk+3iWzj8lJSUAAB8fHxw7dgz5+fn4/PPPUV5efpFfj6h7QWpXfHHvbCybGmI5djC/RsKKiIiorwY05kUQBKxfvx4rVqywHEtKSkJiYiLeeecdAIDJZEJERAQeeughrFmzpt+f8cADD+Dyyy/HDTfc0O15vV4PvV5vea7VahEREcExL9RnP2aW4v7PjiA62As/PjwPP2WVISZUjdH+HlKXRkQ0Ykg25qWlpQXp6elISUnp+ACZDCkpKdi3b1+f3qO8vBz19fUAAI1Gg507d2LSpEk9Xv/SSy/B29vb8hMRETGwL0EjTuIYPwDmjRzf3X4G9392BL/5V7rEVRERUU8GNbxUVVXBaDQiKCjI5nhQUBDKysr69B7nzp3DvHnzEB8fj3nz5uGhhx5CXFxcj9c/8cQT0Gg0lp+ioqIBfQcaeQI8VYgP9wYAvPKzeRfqnPJ6NLUYpSyLiIh6oJC6gM5mzZqFjIyMPl+vUqmgUql6v5DoApZNDcGxYo3NsawSDRKj/CSqiIiIejKoLS8BAQGQy+VdBtiWl5cjODh4MD+KaFAtjQuBUm77nwMH8BIR2adBDS9KpRIzZsxAWlqa5ZjJZEJaWhqSk5MH86OIBlW4rzu+ui8Z3z04F48vMo+xeuXnHPw3vVjiyoiIqLN+dxs1NDTg9OnTluf5+fnIyMiAn58fIiMjsXr1aqxcuRIzZ87ErFmz8Oabb0Kn0+Guu+4a1MKJBltChA8AwM9DifVHz+N0RQMe/foY3JVyLIkLufCLiYho2PR7qvT27duxYMGCLsdXrlyJtWvXAgDeeecdvPLKKygrK0NCQgLefvttJCUlDUrBPUlNTUVqaiqMRiNyc3M5VZoGxGQS8fR3WfjP/kLLFGpB4PYBRERDpT9Tpe1ub6OB4t5GNFg0ja1IfjkNjS1G/PP2GbhyCsdtERENFYfe24jIXni7u+D/Zo8GADz+zXEUVjdKXBEREQEML0QX9OiVExEf4QNNUyt+8+/DXPuFiMgOMLwQXYBKIcf7/zcdAZ5KnCqrx9Mbs9BiMEldFhHRiMbwQtSLEG83vHJDPADg6/RiLH5rJ8o0zRJXRUQ0cjlNeElNTUVMTAwSExOlLoWc0ILoQDx39RR4u7ngbKUOd35y0KYFpsVgQkU9Aw0R0XDgbCOifiiqacQ1qXtQo2vB3XPH4NZZERgT4IGnNmbhq8PF+PzXSUga6y91mUREDoezjYiGSISfO/60dDIA4OM9+bjijZ14cdNJfHGwCEaTiBc2ZUtcIRGR82N4Ieqn66aH4c/LJluer91bYHmcV96A+ubWC75+84kyvPlLLpys0ZOIaNgwvBD1kyAI+PW8sTjz16UI9Xa1Oac3mBD37Gbc/tGBbmcliaKI3/w7HW/+koe9Z6qHq2QiIqfC8EJ0keQyAf+XbF7ELszHDYutVuDdlVeFt9PycPlr25G6rWMvsKqGFqvH+uErlojIiTC8EA3A/fPH4ceH52HbY5dh5Zwom3PvbDuNs5U6fLjrLEwmcxfR6YoGy/laXYvN9SV1TXhtcw5nLRER9YLhhWgABEHA5BA1lAoZZkb5wkXedfPG2sZWnCzTAgBOV9Rbjpdp9diSXY6s8xoAwF2fHMI/tp7GH745PjzFExE5KKcJL1znhaTmIpdh46pL8K+7Z2FapI/NuR25lcgu0SLPquVl35kq3Puvw7jzk4MwGE3IKTcHm525lTav/flEGY4W1g55/UREjoLrvBANgWe/O2EzC6k3X9+XjBvf3wcA8HJV4M2bE3CsqA4rpoXh8td2AADyX1oKQejaskNE5Az68/tbMUw1EY0oo/3d+3X9luxyy2NRBO759LD5sdU15+uaEO7bv/clInJGTtNtRGRPbpwZgaQxfvjd5eP7dP3nBwotjxv0Bsvj3PKOMTKnSutBREQML0RDwlOlwJe/TcbqKychWG27Fszfb5ja5XrrwGItu1RreXyqTNvtNUREIw3DC9EQS71tOsYEeODd26Zj/QNzcNPMCEwO6ejP9VT13HtbVNNkeXyyjC0vREQAwwvRkJsx2hfbHrsMS+NCMC3SFwCwIiHUcv6mmRF9ep+88nq0Gk1IP1fb7eq9REQjBcMLkQSunR4GmWBemfexRRNx/2Xj8Lfr4y74mtK6Zry//Qyuf28v3vwlF4B5GvU7W/PQamSYIaKRw2mmSqempiI1NRVGoxG5ubmcKk1273xdE1xkAgKtxsRErdnU59cXvLwMsc/8jAa9AVfHh+LtW6cNRZlERMOiP1OlnablZdWqVcjOzsahQ4ekLoWoT8J83GyCS3/VN7daBvp+d6wEdY0tvbyCiMg5OE14IXImCRE+Ns993V26XJN13nb2Ubm2940e08/VoqBKN6DaiIikxvBCZEe+fWAOrp8ejv93+wzLsdH+7jazk9qlnSy3ed7bLtXn65pw/Xt7cdmr26E3GAenYCIiCTC8ENmR6ZG+eO2meASpXbFoShDGBnjg83tnd1krBgC+P15q87yy/sLhJcdqnZifssoGp2AiIglwewAiO/X/bp8JURQhCAKCvLuGlzJts81z65aXphYjXF1kNnshlWk6zn+TXoxrEsKGoGoioqHHlhciO9YePtSuHWNeXr8pHkp51/90X9+Si71nqvBLdjkmP/0TvjhYZHP+fF2j5XE+x70QkQNjeCFyALPH+gEAZkX54dppYVgcG2w5NyXUPB6mscWIX31wAL/+l3lTxyfXZ9q8R0ldR0tNrY4zk4jIcbHbiMgBTIv0Rdqj8xHu6wZBEPDCilgU1TbiRIkWV8QE4URJ9/semUwiZDJz6835uo6tBnQtRjS3GuHqIh+W+omIBhPDC5GDGDfK0/LY280F/71vDnQtBqSfq+3xNd8ePY/qBj1WzonC+domm3O1jS0I8XYbsnqJiIYKwwuRg5LJBHi5usDfQ9XjNY99fQwAcLxY02WAb42O4YWIHJPTjHlJTU1FTEwMEhMTpS6FaFhF+HUEkO6mVAPApsxSGE0iPJRyTAg0t+Ase3s3vjxUOCw1EhENJqfZ26hdf/ZGIHIWmcUaeKjk0OmNuP3jA/jtpePw3bESnCy1HQuzNC4YtbpW7DtbbTm26w8LEO7rhj9tyEJpXRP+ecdMuHQzm4mIaCj15/c3u42InEBcuLflccbTVwIAbp0Vgf1na+CulOOOjw8CAFImByHtZIXNaz/ZU4ApoWp8fsDcCpN5XoPpkb7DVDkRUf8xvBA5KR93JRbHBsNgNGF8oCfqGluwMDoIRwptB/juzKvEL1ZbDZwub0BzqxERvu6I8HO3uTbtZDnyKhrw20vH2iyAR0Q0nBheiJycQi7DhlVzYTSJ8HZzgaxT6Dhd0WDz/B/b8lBU04SJQZ7Y/Pv5Nufu+dS8hkxcmDfmjg/oVx16gxHpBbWYGeUHpYLdUkR08RheiEYAT1XHf+rW2wgkRPggo6jO5tqiGvOU6tzyBhRU6dDUasTbaXlo0Bss1+SV12NMgAc8XRU2q/9eyNo9BXjpx1OIDVPjv/fPwV83ncTJUvP7jA5wxwOXjR/ANySikYT/+0M0wlw3LRwAMHO0L1bOGW05njI5sMu1O3Ir8XZaHn7MKsOuvCrL8YMFNVjw6nZc/+5etBpNffrc48UaAEDWeS3+s78Qn+47h4MFNfjycBH+/lMOdFbhiIjoQtjyQjTCLJwciI2r5mJcoCc8VQrUNbbix6wyrFkyGb+0DeadHumDI4V12J5T0e3qvT9kmnelzqtowLdHinFzYmSvn6s3dIScDUfPdzl/okSLWWP8LvZrEdEIwvBCNMIIgoD4CB/L87vmjsFdc8cAAN66JQH6VhPiwr2x5K1d2JZT2ev7/Wd/YZ/CS42uo7sq87ymy/njxXUML0TUJwwvRGRxTUIYAEAURQR6qVBRbw4cAZ4qm7Ey1k6VadFiMPU6CLe2sfWC57sLNERE3eGYFyLqQhAEzJ84yvL8moTQHq9tNYrIq6jv8fyuvErsyK1ERaftCTrraXNJIqLOGF6IqFvXTQ+HUi7DwuhA/O7yCfjd5eMR5e+O/3f7DMs10yN9AADZbcHDZBLx6FfHcOUbO1CubUZmsQa3f3QQKz8+CF2L8YKf11u4+e5YyQU3oSSikcNpuo1SU1ORmpoKo/HC/0ASUd8kj/PHiecXWbYKWH3lJKy+chIA4MM7ZsLTVYHNJ8pxpLAOJ0q0WN5qxOtbcvHfI8UAgOe/z0byWP8+f5622YBWo8nyeSdKNDiUX4Pbk6NwslSL331xFACQ8+JiqBTywfyqRORgnCa8rFq1CqtWrbLsjUBEA9fTHkcpMUEAzGvGfLwHWLu3AGv3Fthcs+l4KZp6aW3prK6xFaO8zLtkL3t7NwAgUO1qM416d14VFk4O6tf7EpFzYbcREV20xVOCMSW0YwM1T5UCf702zjJraOupip5e2q3axhYAgLa5Y3BvQbXOZhXg74+XDqRkInICTtPyQkTDTyGX4a1bpuGNLbm4amoIrpwSDLlMQLm2GQfza/r9fjU6c3g5ZrXqr0wQkFPeMSCY416IiC0vRDQg4wM9kXrbdCyJC4FcZt43ac64vo91sVaja4GmqRVHztVZjlU36JFb1hFeSuqaYOjjqr5E5JwYXoho0CVE+iDE2xUAMDbAA+t+MxtuLnK8sCLWco3SajyN2tXcCPzWL3mIf24z3vgl13LuXHUjSjQdM5EMJhGlmgvPTCIi58ZuIyIadCqFHFsfvQzp52oRFeCOcF93ZD23CHKZgKc2ZAEA/DyUKGubHh0V4IHjxRqb7qF2x4rrAAC+7i7wdVfibJUORTWNiPBzH7bvQ0T2hS0vRDQk3JRyXDIhAOG+5pDR3qXUztdDaXkc2SmIrEgIxZ+WTgYAlGvNK/uG+rhZAktRbeOQ1U1E9o8tL0Q0rBQyAQaTiGVxwThZal7cbkyAh+X86zfF47rp4TaDdgFzeAlWm7uiCmsYXohGMoYXIhpWm39/KfacrsItsyIxLdIXrUYTMos79jVqX8PFz6plBgDCfNwQ5uMGwDwOhohGLnYbEdGwGjvKE7cnR8FFLsPc8QG4bFIgFseap1gvjQuGt5sLAMDf0za8hPq4YkKQJwAgq20TR53egJyynvdVKqppROq209A0XXhTSCJyLGx5ISLJTQjywqE/pcBT1fFPkrtSAXelHI1tq/SG+rhhWqQvBAEoqG7EztxKrPnvcZRomvHlb2YjqZutCFZ+fBBnq3Q4X9eEv14bN2zfh4iGFlteiMgu+HkooVTY/pM0PtDT8jjUxw3ebi6YFOQFALjj44OWKdSdV/LVNLbCaBJxtkoHANh8onwoSyeiYcbwQkR265nlMZbH7TOSZoz27XLd/vwanCrTIre8HpnFGkx/cQse/PyI5bxKwX/qiJwJu42IyG7NGO2HT++ehaYWIwI8zRs2Xjc9HJ8dKAQATAzyRG55A44V1WHxm7vgqVIgZXIgjCYRP2aVWd6nwWpjRyJyfPzfESKya/MnjsLi2GDL8xmjffHJnYmYM84fr9+UgLGjOqZZN+gN2JBR0uU9NE2t2JJdjm/Si2EyicNSNxENHUEURaf4Lzk1NRWpqakwGo3Izc2FRqOBWq3u/YVE5NAyizV4+MujOFupszkepFZZFriztiQ2GO/eNh2CIHQ51xdnKxtwplKHK2KCLur1RNQ9rVYLb2/vPv3+dprw0q4/X56InIMoilh/9DxWf3UMgLl15rNfJ+Fgfg3e2Xa6yw7XOx9fgEh/d4iiiNMVDRg7yrPLCsA9iXv2Z9Q3G/DJnYlYEB046N+FaKTqz+9vdhsRkcMTBAGXTQqEl6sCYT5uePPmBLi6yHHpxFG4YnLXFpL2PZS+OlyEK97Yife2n+7zZ9U3m8fPfHv0PHR6AxpbDCiqacT/fXgA23Mqenk1EQ0Ghhcicgp+Hkrs+sMC/LJ6vs2mjd117+SUmbcl+ON/MwEAr27O7XKNtbOVDXjoi6M4XdGxIN7x4jrM+/s2XPfuXrzwfTZ2n67CnZ8c6vLao4W1OFmqhckkYmduJTSNXDCPaKA424iInIaPu7LLsagAD4T7uqG4tgkpk4Pwy8lynCqrR2OL7Qykqga9ZUZTZytS90DbbMCRc7WWY+1bFNToWnCqh1V+i2sbce27ewEA/+/2Gfjtv9Nxw4xwvHpj/EV9PyIyY3ghIqf3zX1zUFjTCJ3egF9OliOnrB77z1bbXLPvTDWWx4d2ea3JJELb1lV0vq6p189qNZrgIjc3am/LqbQcb9+/iZtKEg0cu42IyOkFe7ti1hg/TA4xDwI8U9mA9Udtp1R3HtTbrn18TF+VWAWcjMI6y+MzlQ0AOsbMENHFY3ghohEj2NsVU0LVMInA/46Zw8vVba0tR4tqu33NvjPV3R7vSYHVjtfWrTvt4UXLTSKJBozhhYhGlKumdnQNKWQCHrx8PADgZGnXcTAAkNm2g3VfZZ3X4FhRHRpbDDbdTAVV5lCjbWZ4IRoohhciGlFWTAu17F49b0IAJgZ5IVjtCqNJ7DIOBug+vLjIe14T5pWfc3BN6h78c+dZm+MtRhMA8yrAXOWXaGAYXohoRAnxdsOeNZfj6/uS8eYt0wAAl0wIAACs+uwosku0WHewEBva1nFp7+6x3uE6Ptyn189585e8bo+LItDQTQsPEfUdZxsR0Yjj7eaCxCg/y/M/L5uMc9U6HCqoxYrUPZZWEh93F4iieauBpbHBeHureTG72WP9cfhc92Nk+qK+2QC1q8vAvgTRCMaWFyIa8XzclXj1xni4yAVLcAGAurYF5ZLG+OORlIn4aOVMvHxdHG6bHWm5JsCz69oyveGgXaKBYcsLERGA0f4eePuWacgorsM9l4zBydJ6PPj5EUwJVeOZ5TGQyQQsbNtqQBRFJI/1h0kUIQhAVUP306x7wunSRAPD8EJE1GZJXAiWxIUAAAK9XHHkqSssC85ZEwQBX/xmNkRR7HZLgN6w5YVoYNhtRETUg+6CizVBEHrdjTrMx63LsQtNl25uNeKLg4Wo0bX0rUiiEYjhhYhoAGTChcNLsLdrl2OrvzqGb48Ud3v9f48U44lvMzH/79sgipxSTdQdhhciogGwbpx5cmk0AOD9/5uBpDF+8HZzwby2adgA4OYitzxe/dWxbteVad+moF5vwM68qiGqmsixccwLEdEAKGQd6eXeeWNx44wI+HoocdmkUTCJIn7ILLOcb7WayQQAO3MrMXusP0wmEc9/n42xozxsuqHSTpZj/sRRQ/8liBwMW16IiAZgari35bEgCPD1ME+ddnWRw12pgKeqo7Xl6k67Vp8s1aKkrgk78iqxdm8Bnt54AmWaZsv5krpmEFFXbHkhIhqAu+aOQYvBhMsmBXZ73lPVsRjdE0snY9poXwR4KHH/Z0ewLacSc17eanO99e7WpZomvPlLLnbmVuKjlYmWYEQ00jG8EBENgFIhw0MLJ/R43qOt5cVLpcAoLxVunz0alfX6Hq83WO17dKJEixMlWgDAh7vP4v7Lxlv2ZSIaydhtREQ0hCaHqBEf7o2bEyMsxy5mVd7UbWew8LXt3JWaCE4UXlJTUxETE4PExESpSyEisnB1kWPjg5fgz1fFWI4JgoDFU4IBALdYhRpr3e1cXa7V47P9hUNTKJEDEUQnW0hAq9XC29sbGo0GarVa6nKIiLqlaWpFcW0jovw9cNmr2226klzkAlqNHf80P3DZOLy7/QwAINBLhf1PLISsm8XxNE2taDWaEOCpGvovQDTI+vP722laXoiIHIm3mwumhHrDQ6XATw/Pw9GnrrCcsw4uAPCHxdHIfXEJ3JVyVNTrkVNe3+X9RFHEte/uwby/bYOmkV1L5NwYXoiIJObvqYKvhxK3zx4NABgb4IGHLh8PAHhxRSwA88DgxCg/AMDeM10Xt6vWteBspQ5NrUbsO8vF7ci5cdg6EZGdeHp5DEb7u+PSiaMw2t8dV00NxaRgL8v5OeP8sSO3ErvyKnHPJWNsXltU02h5fLSoDotjzRtMGowmnCjRYlKwF1ytVvglcmRseSEishMuchl+PW8sJgZ5QaWQ2wQXAJg/ybza7vacSnx5yHbgblFtk+XxIau1Yj7YlY9rUvfg8le3o7i2Ec6qqcWI7BIt94MaIRheiIgcRHSwGr9rW1Pmtc25MFqtCWPd8pJ5XmPZimB7TgUAoETTjP848Uyl//voAJa+vQtbssulLoWGAcMLEZEDeXDBePi4u6CiXo/bPtyPCq15CwHrVpVWo4iSuiaYTKJlkTsA2HfGecfCpJ+rBQCsO1QkcSU0HBheiIgciFIhw7I483iW/WdrcE3qHhwqqMGpMtsZSOeqG3G2SocGvcFyLPO8Bpom556JJBO6TiEn58PwQkTkYO6bPw4TAj0BAKWaZtz4/j4cLawDYN6GAADO1TTieLH52MzRvhgb4AGTCOw/23WmkjOR87faiMA/ZiIiBxPh544tq+fj7zdMhbebC1xdzP+UJ0b54uoE887VhdU6/JBZCgCYGeWHSyeaB/tuPWkeAyOKIg4X1GD/2WrL+BgA+OfOM7jhvb04X9cER8SWl5GBU6WJiBzUTTMjcNPMCLQaTdDpDfBxV+LTvQUAgF15VchtW8zuhhnhKNU0Ye3eAvyQWYonlkbjoS+OYleeeQzMVVND8M6vpsNoEvHXH04BAG7/6AB++f38blfy7atDBTXIKKzDPZeMuej32ZlbiY925+Ol6+IQ6uPW7TXNrUbL44HUO5KIogjBgYMeW16IiByci1wGH3fzZo+Rfu4AgFNl9TCJQNIYP4wP9ETSGH94qhSo1xuQ8PwWS3ABgB+zylBZr0fWeY3l2NlKHbJLtRiIG9/fh7/8cBJbT1Vc9Hvc8fFB7MitxGNfH+vxmqHarPJctQ6ZxZreL3Qw720/g5kv/oKzlQ1Sl3LRGF6IiJzIlDA1VArzP+2TQ9R49cZ4AOaBvi+smAIvV3ODu4+7C75/6BLER/jAaBKxMeN8l5V78yq6bkNgMplnMvXGemBw0SCsL3O4oLbHc9qmjkHJTS3GHq9rl1+lw75uVinubP4r27H8nd19+r591dRixONfH8PGjPOD9p799befTqFa14K30vIkq2Gg2G1EROREAr1csePxBahrasGEQC/IrbpRrp0WjiWxISio1iHSzx3uSgVumBGOY0V1+PJQkc21AJBXbvt/5i0GE+7912HsyK3Ev+6eZRlH051TVq02Ta29B4retFiNy+nMuuWlodnQ43Xt7vn0EM5W6vDtA3MwPdK322usxwHlVTT02GXVX2v3FuDr9GJ8nV6MZXEhUEg4wlghc9z2C8etnIiIuhXs7YroYHWXMAIAri5yRAer4a40/7/r1VNDoVTIkFfRgFNl9fBxd8HDbQvhvbv9DJa+tQurPjuCbTkV+OfOM9iRWwnA3NV0IdZdTuWa5j7VXVClw7lqXY/nrRfls1ZvFVi0za0XbH2padsDCgA+u8CifVqrliNTH1ftPV5ch3Lthb/rjtyOLrTD53puTRoq1isQe6ocd7sIhhciohHM290FV8YEWZ7/aelkzBrjZ3meXarFpsxS/Hl9Fvac7uhqOVrY9RevTm/AP3eeQammCZlW42dK+xBeanUtWP6P3Zj/yna8tjnHclyp6Pg11VOwsQ4ap8rqMfdvW3scB3PSKlRtyizpcd2bOqvj2j6sjZNTVo+r39mDha/t6PGaWl0LDlpt3fBTLwFwKFh3sXmoHLfzheGFiGiE+9Oyybh99mj86+5ZuHFmBMa3rSFj7XxdE/ZZrRGTU14PTaPtL/WnNmThrz+cwpyXt2JjRonleG+tEQBwIL8G9W0L6q3dUwAA0BuMaDF0dN+cruh+gGnnoFKja+lxTIt1eGluNeG7Hsae1Fl9t1pdS6/178ozt0g16A097q9UUK2DdePRf/af6zYEDqXKho4/ix4ashwCwwsR0QgX4u2GF1bEWsawBHqpcEVMEGZF+eHUC4sxe2xHS4yLXECYjxtEEdhrtd1AYXUjvj1qDgKiaO7iGW+1kF5vrFsk6vUGaBpbu7SKlNfru32tdWtCu1pdC658Ywee2pBlczy7bbuEUG9XAOYxKNUNXd9X09QRWGo7hTSD0YRjRXUwWf32t56uXdND2Gk/HhfmjWVxITCYRLy7/Uy3116sqgY99pyu6jFAVVjdw+ZBGIskFYYXIiKyIQgCPrhjJr66LxmuLnLMm9AxMDfE2w1XTTVvT7D+aEerxZu/5Nq8h0Im4JM7EwEAlQ16ZBTVoaCq5/EshwpqbJ4X1TZ26a6p7KEFp7suonWHipBb3oB/7z+HeqvzeW2tN49cMRFqVwXOVOpw96eHu7zeuuWlrtE2jDz+zXFck7oH/zve0bp0vq6jtp7CWnVbePHzUOK++eMAAPvO2C4SOFBXvb0bt314AGknu5+eXmkVXvoyM8teMbwQEdEF3Tor0jL9eu54f1w3PRwAsPVUBSq0zdh2qgLr27pf/nZ9HFImB2LDqrkI83GDQiZAFIEVqXtw2avbuw0aza1GywDfQC8VAKC4tqlLy0tFNy0vJpPY7ZiUvPKOad7WrToV9eZgER3sha/uS4ZCJuBYUV2XNU9suo06dSG1h7bPDnQM+LXe1bush/BSaxVepoSq4evugga9ARlFdd1efzHK2gJeWg9r61iHl0a2vBARkbPy81Bi1x8W4PFFk/DQ5RMwKdgL0yN9YDCJSH55K+7912GIInDd9DDcnBiJD1cmIjbMGzKZgKgAD5v3SnzxF8v+SgajCZqmVuSW18NoEuHnoURi22DhvPJ6rN17zua17b94RVHEpuOl+OpwEaY887NNiGins2pVaB9obDKJqG4wB4gATxWig9WYPdYfALq0VFgP2K21ann51qq1yV3ZMVvnXE1Hq1Kppvt1YWqswotMJuCSthatbw4XD0rri/V79DSTiC0vREQ0YgSqXbFqwXjLeidPL58CQTCPbTGYRFyTEIq/XT+1y+tiQtQ2z/UGE275535c++4ezH4pDdNf2IJ/7zOHlOhgL0T4mlcIfm1LLv53rMTmte0tL9tyKrDq8yP4wzfH+7SGTHtY0jS1wtA2TsXf07wi8cLJgQCAtFPlNq+x7iqyboU5YTWLqrCttaXVaEJJP7uNAOBXsyIBAF8eLsKEP/2IMwNc8da6xUfewxou1q1XJ0o0fVqszx4xvBARUb8lRPjglRvicdXUEPx52WS8cVMCXLpZcC0mtCO8BKlVlsdHC+tQ1dACo0nE1+nFAIDoYDXCfbsuBtd+rL3LZ/OJ8i7X/HnZ5B5rzS2vR1FNIyrbBuaqXRVQKcwtE+2DlI8W1kFv6AhCtt1GHUEm32q6dnFNE4wmEQVVOps1aNpDRPq5Gjz+9TFLEGpvefFvCy/J4/xxR/Joy+s6r3DcX9YrGVsPOLZm3SpUqmnGrR/sR343Y5F25VXigc/SbVpq7InjTvImIiJJ3TAjHDfMCL/gNdYtL6/cEI/Kej0e/foYpoSqkRjlh7VtG0kCwOQQry7dTIB59hIAlGv1WHewEFWdZgf9edlk3HPJGGSe19hM0W5nMImY9/dtlvVsArw6QtTYAA/4eyhRrWtB1nkNZow2d1tZdxu1B5lTZVqcKOmYat1iNKFM22yzpg0AFLdtJ3D9e/ss1711y7QuLS8A8OzyKajQ6vHTiTKcr+15GwKTSURjqxGeF1ibpdjq9XWN3a9N012r0OmKBozpdN9v/+ggAMDHXYm/XhvX42dKhS0vREQ0ZKZYtbxEB3vh+hnh2PL7S7Fx1Vw8sTQaHlbjRmLDvDFztC8+vGMmdv1hgeW4j7uL5fGabzPxS6fxKdNH+0IQBLxxUwKOPHWFzbmp4d6Wx5uzzS02AZ4d4UUQBMyMMm8RcMhq/ySNVWtLg96AbTkVWPzmLsu6M+2tSOeqdZbwMm9CAADgyLlanLfaD6l9Y8oanTl0tXdZAeZdsGeMNn/++bomfLInHx/uOovO/vLDScQ9+zOOF9d1OdfOOry0txbpDR17KYmi2G14udBG3H1dHXm4MbwQEdGQ8fdU4a/XxuHFFbEIVJvXVpkQ5AWFXAaVQo6HFk5AdLAXnr9mCqKDvSAIAlJighDh545P7krE+EBPPH/NlAt+RnjbOByZTICfhxLPLo+BIAARfm6IDvbqcv0oq/ACAIlR5taWQ1azkqo7rdXy7HcnbJ7Hh/sAAD7dW2DZjXtFQhhiw9QwmEQ8/7+O6+ubDSipa0JN22BhX3elzXuFtXWLnSzV4rn/ZePFTSdtZj9pmlrxn/3nIIq44BgV6xWI21tePttfiK/Ti/HwugxU61psFv1r13nckPW6N95uLp0vtwvsNiIioiH1q6TIHs/dN3+cZc2TzhZMCsSCSYGW697f0f2CbgGdwsidc8fg8ugguCpl0OmNOF6swamyeqvrbcNDe3g5fK4WJpMIER2rAgd6qVBRr8e5atudsX+3cAK25VTgZ6vxN3Hh3liREIas81qb44B56nL7DCh/D9t62wdBW68gvC2nEmNHmRf5+9+xEujbQkdxD11LVQ16/JLd8ZntLS/WXVo97Y79/bFShPu6IyHCB0DHWjiAudXJHrHlhYiI7N6aJdH4+M6Z3Z6TddPvEenvjkAvV4wJ8MBPj1xqWVgPMLcGWZsSqoa7Ug5NUyvyKhpQ1aBHq1GEXCZgzjj/Lu/9+KJJiA3zxt2XjLEci/J3x7hRnlgcG2xzbVhbMPn3vgIA5pYMtZui22usbbNap+Wrw0WWx+c7BZDqBj1u/+gAZr74C3QtRst6PLWNrRBF0TLIGYBlvE6gl+33/+lEGVak7rGsGGy9Rk7n8UX2guGFiIgcwvRIX8vjPy6OBoBuZyd154HLxlsedw4LCrnM8t4HC2osrRvBaldMtOp2uiImCJnPXokHLjO3FP1m3li4usgs9chlAsLbpnq3+1PbLKjccnNrxuyxfhAE27AV4Km02YASAA7kV6NBb8DJUi2OF3e0nnQe1PvGL7nYldexTcOTS82f12IwoanViFOlHUHkSNsu1mNHdR0UDXQscGfd8lJpp+GF3UZEROQQfNyV+O/9cyCXCZga5o3R/u42geZCYkLV+PmRS7H1VAWWxoV0OZ8Y5Yfdp6ts9kIK83HDuFEdm1ReHR8KL9eOMSD+niqsvWsWztc22bS4/GHxJPz9pxzcPDMCc8cHQBA6ZkzNHR/Q5bMFQUC4rxvOVnaMWWk1itidV4XsEnNwmRTkhZzyehTXNkIURQiCgKoGPb46bJ5mnvqr6Zg91g9+Hkq88H02DCYRJ0vrbcbutE9JnxDohf1nbbdjAID8Kh1Cfdxspk5X1fe+KaUU2PJCREQOY8ZoXyRE+EAmE7A0LgTBbRss9sWkYC/cf9k4uCm7rj57/YywLsdCfVwxObhjtlTK5KAu18we64/rZ4TbtKb8Zt5YfHjHTDx3zRR4u7lgYXTH6+aM6xpeAOASq1DTPrtq26kKS1dPe326FqNl24R9Z6rRYjAhOtgLS+OC4e+pgiAI8GkbEHz7Rwe6fI6XSoGVc6K6raE9tFiHl6ZWI3R2OO6F4YWIiEa8cF933NhpzZpQHzdE+rvjkzsTsXHV3G5DT3cUchlSYoLg6mK+/p1fTcNfr43DGzfHW3ba7mzRlI6Wm/Y6tuVU4GTbnk8JEb6WgclFNeauo/aNLmPDvG3C06VtU7Ybu1n+//dXTOyxhvwqHZpbjV3G1ZjHAJlQXNuIxhYDanUtPQ7+HS52G14aGxsxevRoPPbYY1KXQkREI8CzV0/By9d1LMjWvmjuguhAxLfNxLkYri5y/CopEtdO63lBv1ltezoBwO2zo+CulKOiXo+StnVWokO8LNO+//rDSVRomy2r/XZeYO61m+IR2kOLlPXA5c4KqnQoqmmEKAKeKgUi/MxjgwprGpHy+g5c8rdtiHn6Z0x7YQte/vFUH7750LHb8PKXv/wFs2fPlroMIiIaITxUCtwyKxJ3zomCi1zodfXgweQil2H7Y5dh46q5iPR3txkbE+bjBrWrCx5fNAkyAdh3thoLX9+BjMI6AECUv214EQTBJgy1L9QX4KmyrLXTnbyKBnxx0DyzKSrAHWMDzC00t390sMtU8c47fg83uxywm5eXh1OnTmH58uXIysrq/QVERESD5KmrYvDk0sldZgANNeutERZGB2JL27ot7ftDxUf44K1bpuGhL46ivtmA+mbzWJTOLS8ALGvEAMDK5Ch4u7n02npUWNOIj/fkm2vx98BvLx2H3aerLPs2Pb5oEm6YEQ4PleKC2xQMh37/yezcuRPLly9HaGgoBEHAhg0bulyTmpqKqKgouLq6IikpCQcPHuzXZzz22GN46aWX+lsaERHRgMllwrAHl85WTAvDb+ePxa2zIvH4okmW48vjQ/FCpxWHowLcO7/cZjp0uK8bUmKCMMpqfZevfpvcZYyPzecnhCEu3BsvroiFSiGD2lWBG2eGI0jtKnlwAS6i5UWn0yE+Ph533303rrvuui7nv/zyS6xevRrvv/8+kpKS8Oabb2LRokXIyclBYKB5pcSEhAQYDF1HL2/evBmHDh3CxIkTMXHiROzdu/civhIREZFjc3WR44kl3e+UfXVCGN5Ky0NVQwvGBnjAXdn1V7l1a0xYN2vhzBrjh7GjPCzTp+eM87fsap3+5xTLQn63zorElTFBaDWKCPTq+8yuodbv8LJkyRIsWbKkx/Ovv/467r33Xtx1110AgPfffx+bNm3Cxx9/jDVr1gAAMjIyenz9/v37sW7dOnz99ddoaGhAa2sr1Go1nn766W6v1+v10Os7FtHRarXdXkdEROQMvN1c8Mvq+diRW2mza7e1caM8IQiASiFDcA/jXNRWa9Y8vmgS7vzkEK6fHt5lBeLOz+2BIIrtS+dcxIsFAevXr8eKFSsAAC0tLXB3d8c333xjOQYAK1euRF1dHTZu3Niv91+7di2ysrLw6quv9njNs88+i+eee67LcY1GA7W6+z9UIiIiZ1dR3wyZIHTZ+8najtxKGIwmLOxmDZvhptVq4e3t3aff34PaqVdVVQWj0YigINubEBQUhLKyssH8KIsnnngCGo3G8lNUVNT7i4iIiJxcoJfrBYMLAMyfOMougkt/ST/q5gLuvPPOXq9RqVRQqeyvSYuIiIiGxqC2vAQEBEAul6O83HYr8PLycgQHB/fwKiIiIqK+G9TwolQqMWPGDKSlpVmOmUwmpKWlITk5eTA/ioiIiEaofncbNTQ04PTp05bn+fn5yMjIgJ+fHyIjI7F69WqsXLkSM2fOxKxZs/Dmm29Cp9NZZh8RERERDUS/w8vhw4exYMECy/PVq1cDMM8oWrt2LW6++WZUVlbi6aefRllZGRISEvDTTz91GcQ72FJTU5GamgqjsetGVEREROQ8BjRV2h71Z6oVERER2QfJpkoTERERDTWGFyIiInIoDC9ERETkUBheiIiIyKEwvBAREZFDcZrwkpqaipiYGCQmJkpdChEREQ0hTpUmIiIiyfXn97ddb8x4MdqzmFarlbgSIiIi6qv239t9aVNxuvBSX18PAIiIiJC4EiIiIuqv+vp6eHt7X/Aap+s2MplMKCkpgZeXFwRBGNT31mq1iIiIQFFREbukhhDv8/DgfR4+vNfDg/d5+AzFvRZFEfX19QgNDYVMduEhuU7X8iKTyRAeHj6kn6FWq/kfxjDgfR4evM/Dh/d6ePA+D5/Bvte9tbi0c5rZRkRERDQyMLwQERGRQ2F46QeVSoVnnnkGKpVK6lKcGu/z8OB9Hj6818OD93n4SH2vnW7ALhERETk3trwQERGRQ2F4ISIiIofC8EJEREQOheGFiIiIHArDSx+lpqYiKioKrq6uSEpKwsGDB6UuyeHs3LkTy5cvR2hoKARBwIYNG2zOi6KIp59+GiEhIXBzc0NKSgry8vJsrqmpqcFtt90GtVoNHx8f3HPPPWhoaBjGb2HfXnrpJSQmJsLLywuBgYFYsWIFcnJybK5pbm7GqlWr4O/vD09PT1x//fUoLy+3uaawsBDLli2Du7s7AgMD8fjjj8NgMAznV7F77733HqZOnWpZpCs5ORk//vij5Tzv89B4+eWXIQgCHnnkEcsx3uvB8eyzz0IQBJuf6Ohoy3m7us8i9WrdunWiUqkUP/74Y/HEiRPivffeK/r4+Ijl5eVSl+ZQfvjhB/FPf/qT+O2334oAxPXr19ucf/nll0Vvb29xw4YN4rFjx8Srr75aHDNmjNjU1GS5ZvHixWJ8fLy4f/9+cdeuXeL48ePFW2+9dZi/if1atGiR+Mknn4hZWVliRkaGuHTpUjEyMlJsaGiwXHPfffeJERERYlpamnj48GFx9uzZ4pw5cyznDQaDGBsbK6akpIhHjx4Vf/jhBzEgIEB84oknpPhKduu7774TN23aJObm5oo5OTnik08+Kbq4uIhZWVmiKPI+D4WDBw+KUVFR4tSpU8WHH37Ycpz3enA888wz4pQpU8TS0lLLT2VlpeW8Pd1nhpc+mDVrlrhq1SrLc6PRKIaGhoovvfSShFU5ts7hxWQyicHBweIrr7xiOVZXVyeqVCrxiy++EEVRFLOzs0UA4qFDhyzX/Pjjj6IgCOL58+eHrXZHUlFRIQIQd+zYIYqi+Z66uLiIX3/9teWakydPigDEffv2iaJoDpkymUwsKyuzXPPee++JarVa1Ov1w/sFHIyvr6/44Ycf8j4Pgfr6enHChAnili1bxPnz51vCC+/14HnmmWfE+Pj4bs/Z231mt1EvWlpakJ6ejpSUFMsxmUyGlJQU7Nu3T8LKnEt+fj7Kysps7rO3tzeSkpIs93nfvn3w8fHBzJkzLdekpKRAJpPhwIEDw16zI9BoNAAAPz8/AEB6ejpaW1tt7nN0dDQiIyNt7nNcXByCgoIs1yxatAharRYnTpwYxuodh9FoxLp166DT6ZCcnMz7PARWrVqFZcuW2dxTgH+nB1teXh5CQ0MxduxY3HbbbSgsLARgf/fZ6TZmHGxVVVUwGo02fxgAEBQUhFOnTklUlfMpKysDgG7vc/u5srIyBAYG2pxXKBTw8/OzXEMdTCYTHnnkEcydOxexsbEAzPdQqVTCx8fH5trO97m7P4f2c9QhMzMTycnJaG5uhqenJ9avX4+YmBhkZGTwPg+idevW4ciRIzh06FCXc/w7PXiSkpKwdu1aTJo0CaWlpXjuuecwb948ZGVl2d19ZnghclKrVq1CVlYWdu/eLXUpTmvSpEnIyMiARqPBN998g5UrV2LHjh1Sl+VUioqK8PDDD2PLli1wdXWVuhyntmTJEsvjqVOnIikpCaNHj8ZXX30FNzc3CSvrit1GvQgICIBcLu8yorq8vBzBwcESVeV82u/lhe5zcHAwKioqbM4bDAbU1NTwz6KTBx98EN9//z22bduG8PBwy/Hg4GC0tLSgrq7O5vrO97m7P4f2c9RBqVRi/PjxmDFjBl566SXEx8fjrbfe4n0eROnp6aioqMD06dOhUCigUCiwY8cOvP3221AoFAgKCuK9HiI+Pj6YOHEiTp8+bXd/pxleeqFUKjFjxgykpaVZjplMJqSlpSE5OVnCypzLmDFjEBwcbHOftVotDhw4YLnPycnJqKurQ3p6uuWarVu3wmQyISkpadhrtkeiKOLBBx/E+vXrsXXrVowZM8bm/IwZM+Di4mJzn3NyclBYWGhznzMzM22C4pYtW6BWqxETEzM8X8RBmUwm6PV63udBtHDhQmRmZiIjI8PyM3PmTNx2222Wx7zXQ6OhoQFnzpxBSEiI/f2dHtThv05q3bp1okqlEteuXStmZ2eLv/nNb0QfHx+bEdXUu/r6evHo0aPi0aNHRQDi66+/Lh49elQ8d+6cKIrmqdI+Pj7ixo0bxePHj4vXXHNNt1Olp02bJh44cEDcvXu3OGHCBE6VtnL//feL3t7e4vbt222mOzY2Nlquue+++8TIyEhx69at4uHDh8Xk5GQxOTnZcr59uuOVV14pZmRkiD/99JM4atQoTivtZM2aNeKOHTvE/Px88fjx4+KaNWtEQRDEzZs3i6LI+zyUrGcbiSLv9WB59NFHxe3bt4v5+fninj17xJSUFDEgIECsqKgQRdG+7jPDSx/94x//ECMjI0WlUinOmjVL3L9/v9QlOZxt27aJALr8rFy5UhRF83Tpp556SgwKChJVKpW4cOFCMScnx+Y9qqurxVtvvVX09PQU1Wq1eNddd4n19fUSfBv71N39BSB+8sknlmuamprEBx54QPT19RXd3d3Fa6+9ViwtLbV5n4KCAnHJkiWim5ubGBAQID766KNia2vrMH8b+3b33XeLo0ePFpVKpThq1Chx4cKFluAiirzPQ6lzeOG9Hhw333yzGBISIiqVSjEsLEy8+eabxdOnT1vO29N9FkRRFAe3LYeIiIho6HDMCxERETkUhhciIiJyKAwvRERE5FAYXoiIiMihMLwQERGRQ2F4ISIiIofC8EJEREQOheGFiIiIHArDCxERETkUhhciIiJyKAwvRERE5FAYXoiIiMih/H/udGuMuqkIgQAAAABJRU5ErkJggg==",
                         "text/plain": [
-                            "(-1.1113732874393463, 1.1139612019062042, -1.1, 1.1)"
+                            "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
-                    "execution_count": 14,
                     "metadata": {},
-                    "output_type": "execute_result"
-                },
-                {
-                    "data": {
-                        "image/png": "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",
-                        "text/plain": [
-                            "<Figure size 432x288 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "generated_path = model.generate_path(x)\n",
-                "generated_path += path[0] - generated_path[0]\n",
-                "generated_path = get_tree_reduced(generated_path, tol=1e-2)\n",
-                "\n",
-                "plt.plot(\n",
-                "    *path.T,\n",
-                "    label=\"Original path\",\n",
-                "    linewidth=10,\n",
-                "    linestyle=\"-\",\n",
-                ")\n",
-                "plt.plot(\n",
-                "    *generated_path.T,\n",
-                "    label=\"Generated path\",\n",
-                "    linewidth=10,\n",
-                "    linestyle=\"--\",\n",
-                ")\n",
-                "plt.axis(\"off\")"
+                "plt.plot(test_mse)\n",
+                "plt.yscale(\"log\")"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.7 ('base')",
             "language": "python",
             "name": "python3"
@@ -426,15 +301,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "f7d1fba74dfd24f4e28e69f7ae18d3d17d4ecc25efd86b65572743c77fabf4a5"
             }
         }
```

### Comparing `signax-0.1.2/examples/nets.py` & `signax-0.2.0/examples/nets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Callable
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.random as jrandom
 
+from signax import signature, signature_combine
 from signax.module import SignatureTransform
-from signax.signature import signature, signature_combine
 from signax.utils import flatten
 
 
 def _make_convs(input_size: int, layer_sizes, kernel_size, *, key):
     """Make a stack of Conv1d:
 
     The first layer has kernel size = `kernel_size`.
@@ -66,14 +66,16 @@
         self.include_time = include_time
         self.kernel_size = kernel_size
         self.activation = activation
 
     def __call__(
         self,
         x: jnp.ndarray,
+        *,
+        key=None,
     ):
         """x size (length, dim)"""
         length, _ = x.shape
         ret = []
         if self.include_original:
             start_index = self.kernel_size - 1
             truncated_x = x[start_index:]
@@ -160,15 +162,15 @@
     def __init__(self, length, adjusted_length, signature_depth=2) -> None:
         # this make sure that windows will be expanded
         assert adjusted_length > 0
         self.length = length
         self.adjusted_length = adjusted_length
         self.signature_depth = signature_depth
 
-    def __call__(self, x):
+    def __call__(self, x, *, key=None):
         """
         Transform input `x` into a smaller window.
         Each window starts at index 0 with increasing size according
         to `adjusted_length`.
 
         Then, signature transform will be applied onto each window.
         The signature will be gathered in the output.
```

### Comparing `signax-0.1.2/examples/utils/brownian_motion.py` & `signax-0.2.0/examples/utils/brownian_motion.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/examples/utils/dataloader.py` & `signax-0.2.0/examples/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/examples/utils/ornstein_uhlenbeck.py` & `signax-0.2.0/examples/utils/ornstein_uhlenbeck.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/examples/utils/signature_normalization.py` & `signax-0.2.0/examples/utils/signature_normalization.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/src/signax/module.py` & `signax-0.2.0/src/signax/module.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 from __future__ import annotations
 
+from typing import Any
+
+__all__ = ("SignatureTransform", "LogSignatureTransform")
+
 import equinox as eqx
-import jax
+from jaxtyping import Array, Float
 
-from signax.signature_flattened import signature, signature_combine
+from signax.signatures import logsignature, signature
+from signax.utils import flatten
 
 
 class SignatureTransform(eqx.Module):
     depth: int
+    stream: bool
 
-    def __init__(self, depth: int):
+    def __init__(self, depth: int, stream: bool = False) -> None:
         self.depth = depth
+        self.stream = stream
 
     def __call__(
         self,
-        path: jax.Array,
-    ) -> jax.Array:
-        return signature(path, self.depth)
+        path: Float[Array, "path_len dim"],
+        *,
+        key: Any | None = None,
+    ) -> Array:
+        return flatten(signature(path, self.depth, self.stream))
 
 
-class SignatureCombine(eqx.Module):
-    dim: int
+class LogSignatureTransform(eqx.Module):
     depth: int
+    stream: bool
 
-    def __init__(self, dim: int, depth: int):
-        self.dim = dim
+    def __init__(self, depth: int, stream: bool = False) -> None:
         self.depth = depth
+        self.stream = stream
 
-    def __call__(self, signature1: jax.Array, signature2: jax.Array):
-        return signature_combine(signature1, signature2, self.dim, self.depth)
+    def __call__(
+        self,
+        path: Float[Array, "path_len dim"],
+        *,
+        key: Any | None = None,
+    ) -> Array:
+        return flatten(logsignature(path, self.depth, self.stream))
```

### Comparing `signax-0.1.2/src/signax/tensor_ops.py` & `signax-0.2.0/src/signax/tensor_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,21 +78,14 @@
     depth_index: int,
 ) -> list[jax.Array]:
     """
     Let `depth_index` = n
 
     this function returns
         $sum_{i=1}^n A_i x B_{n - i}$
-
-
-    Note this is hard to convert to `jax.lax.fori_loop`.
-    I don't know if it's possible. Several attempts but
-    `TracerIntergerConversionError` is encountered because
-    getting index of a list (it's okay to get index of ndarray
-    but not for lists)
     """
     return sum(
         [
             otimes(
                 A[i],
                 B[depth_index - i - 1],
             )
```

### Comparing `signax-0.1.2/src/signax/utils.py` & `signax-0.2.0/src/signax/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 from __future__ import annotations
 
+__all__ = (
+    "index_select",
+    "lyndon_words",
+    "compress",
+    "unravel_signature",
+    "flatten",
+    "term_at",
+)
+
 from collections import defaultdict
 from functools import partial
 from typing import cast
 
 import jax
 import jax.numpy as jnp
```

### Comparing `signax-0.1.2/tests/test_tensor_ops.py` & `signax-0.2.0/tests/test_tensor_ops.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import numpy as np
 import signatory
 
 # need to install torch and signatory for testing
 import torch
 from numpy.random import default_rng
 
-from signax.signature import signature, signature_to_logsignature
+from signax import signature, signature_to_logsignature
 from signax.tensor_ops import (
     addcmul,
     mult,
     mult_fused_restricted_exp,
     otimes,
     restricted_exp,
 )
 
 rng = default_rng()
 
 
 jax.config.update("jax_platform_name", "cpu")
+jax.config.update("jax_enable_x64", True)
 
 
 def test_otimes():
     # 1D x 1D
     x = jnp.array([1.0, 2.0])
     y = jnp.array([3.0, 4.0])
 
@@ -63,98 +64,90 @@
 
 
 def test_restricted_exp():
     depth = 4
     length, dim = 2, 3
     path = rng.standard_normal((length, dim))
 
-    signatory_output = (
-        signatory.signature(
-            torch.tensor(path)[None, ...],
-            depth=depth,
-        )
-        .sum()
-        .item()
+    signatory_output = signatory.signature(
+        torch.tensor(path)[None, ...],
+        depth=depth,
     )
+    signatory_output = jnp.array(signatory_output.numpy())
+
     jax_output = restricted_exp(jnp.diff(path, axis=0), depth=depth)
-    jax_output = sum([jnp.sum(x) for x in jax_output])
-    # only check the sum of output in two cases are the same
+    jax_output = jnp.concatenate([jnp.ravel(x) for x in jax_output])
+
     assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
 
 
 def test_mult_fused_restricted_exp():
     depth = 4
     length, dim = 3, 3
     path = rng.standard_normal((length, dim))
 
     # re-test restricted_exp() to make sure it run correctly
     test_restricted_exp()
 
-    signatory_output = (
-        signatory.signature(
-            torch.tensor(path)[None, ...],
-            depth=depth,
-        )
-        .sum()
-        .item()
+    signatory_output = signatory.signature(
+        torch.tensor(path)[None, ...],
+        depth=depth,
     )
+    signatory_output = jnp.array(signatory_output.numpy())
 
     # our computation
     increments = jnp.diff(path, axis=0)
     exp_term = restricted_exp(increments[0], depth)
     jax_output = mult_fused_restricted_exp(increments[1], exp_term)
-    jax_output = sum([jnp.sum(x) for x in jax_output])
-    # again, just check the sum
-    assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
+    jax_output = jnp.concatenate([jnp.ravel(x) for x in jax_output])
+
+    assert jnp.allclose(signatory_output, jax_output)
 
 
 def test_mult():
     depth = 4
     length, dim = 3, 4
     path = rng.standard_normal((length, dim))
 
     # use our implementation, need to compute exp first
     increments = jnp.diff(path, axis=0)
     exp1 = restricted_exp(increments[0], depth)
     exp2 = restricted_exp(increments[1], depth)
     combine = mult(exp1, exp2)
-    jax_output = sum(jnp.sum(x) for x in combine)
-    jax_output = jax_output.item()
+    jax_output = jnp.concatenate([jnp.ravel(x) for x in combine])
 
     # use signatory
     exp1 = torch.tensor(
         np.array(jnp.concatenate([x.ravel() for x in exp1])),
     )[None, :]
     exp2 = torch.tensor(
         np.array(jnp.concatenate([x.ravel() for x in exp2])),
     )[None, :]
-    signatory_output = signatory.signature_combine(exp2, exp1, dim, depth)
-    signatory_output = signatory_output.sum().item()
+    signatory_output = signatory.signature_combine(exp1, exp2, dim, depth)
+    signatory_output = jnp.array(signatory_output.numpy())
 
-    assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
+    assert jnp.allclose(signatory_output, jax_output)
 
 
 def test_log():
     """Test log via signature_to_logsignature"""
     depth = 4
     length, dim = 3, 2
     path = rng.standard_normal((length, dim))
     jax_path = jnp.array(path)
     jax_signature = signature(jax_path, depth)
     jax_logsignature = signature_to_logsignature(jax_signature)
-
-    jax_output = sum(jnp.sum(x) for x in jax_logsignature)
-    jax_output = jax_output.item()
+    jax_output = jnp.concatenate([jnp.ravel(x) for x in jax_logsignature])
 
     torch_signature = signatory.signature(
         torch.tensor(path)[None, ...],
         depth,
     )
     torch_logsignature = signatory.signature_to_logsignature(
         torch_signature,
         dim,
         depth,
     )
 
-    torch_output = torch_logsignature.sum().item()
+    torch_output = jnp.array(torch_logsignature.numpy())
 
-    assert jnp.allclose(torch_output, jax_output, rtol=1e-3, atol=1e-5)
+    assert jnp.allclose(torch_output, jax_output)
```

### Comparing `signax-0.1.2/tests/test_utils.py` & `signax-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/.gitignore` & `signax-0.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -152,7 +152,11 @@
 .Trashes
 ehthumbs.db
 Thumbs.db
 
 # Common editor files
 *~
 *.swp
+
+# notebooks
+Untitiled.ipynb
+t.ipynb
```

### Comparing `signax-0.1.2/LICENSE` & `signax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signax-0.1.2/README.md` & `signax-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Signax: Computing signatures in JAX
 
 [![Actions Status][actions-badge]][actions-link]
+[![Codecov Status][codecov-badge]][codecov-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/Anh-Tong/signax/workflows/CI/badge.svg
 [actions-link]:             https://github.com/Anh-Tong/signax/actions
+[codecov-badge]:            https://codecov.io/gh/anh-tong/signax/branch/main/graph/badge.svg?token=SU9HZ9NH70
+[codecov-link]:             https://codecov.io/gh/anh-tong/signax
 [pypi-link]:                https://pypi.org/project/signax/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/signax
 [pypi-version]:             https://img.shields.io/pypi/v/signax
 [rtd-badge]:                https://readthedocs.org/projects/signax/badge/?version=latest
 [rtd-link]:                 https://signax.readthedocs.io/en/latest/?badge=latest
 <!-- prettier-ignore-end -->
 
@@ -27,78 +30,80 @@
 ## Examples
 
 Basic usage
 
 ```python
 import jax
 import jax.random as jrandom
+import signax
 
-from signax.signature import signature
 
 key = jrandom.PRNGKey(0)
 depth = 3
 
 # compute signature for a single path
 length = 100
 dim = 20
 path = jrandom.normal(shape=(length, dim), key=key)
-output = signature(path, depth)
+output = signax.signature(path, depth)
 # output is a list of array representing tensor algebra
 
 # compute signature for batches (multiple) of paths
 # this is done via `jax.vmap`
 batch_size = 20
 path = jrandom.normal(shape=(batch_size, length, dim), key=key)
-output = jax.vmap(lambda x: signature(x, depth))(path)
+output = jax.vmap(lambda x: signax.signature(x, depth))(path)
 ```
 
-Integrate with [equinox](https://github.com/patrick-kidger/equinox) library
+Integrate with the [equinox](https://github.com/patrick-kidger/equinox) library
 
 ```python
 import equinox as eqx
 import jax.random as jrandom
 
 from signax.module import SignatureTransform
 
 # random generator key
 key = jrandom.PRNGKey(0)
 mlp_key, data_key = jrandom.split(key)
 
 depth = 3
 length, dim = 100, 3
 
-# we signature transfrom
+# create a signature transform at the specified depth
 signature_layer = SignatureTransform(depth=depth)
-# finally, getting output via a neural network
+
+# stack a MLP layer after that
 last_layer = eqx.nn.MLP(
     depth=1, in_size=3 + 3**2 + 3**3, width_size=4, out_size=1, key=mlp_key
 )
 
 model = eqx.nn.Sequential(layers=[signature_layer, last_layer])
 x = jrandom.normal(shape=(length, dim), key=data_key)
 output = model(x)
 ```
 
-Also, check notebooks in `examples` folder for some experiments of
+Also, check the notebooks in `examples` folder for some experiments that
+reproduce the results of the
 [deep signature transforms paper](https://arxiv.org/abs/1905.08494).
 
 ## Installation
 
 Via pip
 
 ```
-pip install signax
+python3 -m pip install signax
 ```
 
 Via source
 
 ```
 git clone https://github.com/anh-tong/signax.git
 cd signax
-python setup.py install .
+python3 -m pip install -v -e .
 ```
 
 ## Parallelism
 
 This implementation makes use of `jax.vmap` to perform the parallelism over
 batch dimension.
 
@@ -108,15 +113,15 @@
 Below plots are comparison of forward and backward pass in both GPU and CPU for
 path `size=(32, 128, 8)` and signature `depth=5`
 
 <table>
 <thead>
   <tr>
     <th >Forward</th>
-    <th > Backward</th>
+    <th >Backward</th>
   </tr>
 </thead>
 <tbody>
   <tr>
     <td>
         <img width="300" height="170" src="./assets/forward_gpu.png">
     </td>
```

### Comparing `signax-0.1.2/pyproject.toml` & `signax-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "typing_extensions >=3.7; python_version<'3.8'",
   "jax>=0.3.10",
   "equinox",
-  "jaxlib"
+  "jaxlib",
+  "jaxtyping"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
@@ -131,14 +132,15 @@
   "YTT",         # flake8-2020
   "EXE",         # flake8-executable
   "NPY",         # NumPy specific rules
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
+  "F722",   # Exclude due to jaxtyping
 ]
 target-version = "py38"
 typing-modules = ["signax._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
@@ -146,7 +148,9 @@
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
+"src/signax/module.py" = ["ARG002"]  # unused argument key in __call__ of Module (equinox)
+"examples/nets.py" = ["ARG002"]      # unused argument key in __call__ of Module (equinox)
```

### Comparing `signax-0.1.2/PKG-INFO` & `signax-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signax
-Version: 0.1.2
+Version: 0.2.0
 Summary: Differentiable signature calculations in JAX.
 Project-URL: Homepage, https://github.com/Anh-Tong/signax
 Project-URL: Bug Tracker, https://github.com/Anh-Tong/signax/issues
 Project-URL: Discussions, https://github.com/Anh-Tong/signax/discussions
 Project-URL: Changelog, https://github.com/Anh-Tong/signax/releases
 Author-email: Anh Tong <anh.h.tong@gmail.com>
 License-File: LICENSE
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: equinox
 Requires-Dist: jax>=0.3.10
 Requires-Dist: jaxlib
+Requires-Dist: jaxtyping
 Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
@@ -40,21 +41,24 @@
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Signax: Computing signatures in JAX
 
 [![Actions Status][actions-badge]][actions-link]
+[![Codecov Status][codecov-badge]][codecov-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/Anh-Tong/signax/workflows/CI/badge.svg
 [actions-link]:             https://github.com/Anh-Tong/signax/actions
+[codecov-badge]:            https://codecov.io/gh/anh-tong/signax/branch/main/graph/badge.svg?token=SU9HZ9NH70
+[codecov-link]:             https://codecov.io/gh/anh-tong/signax
 [pypi-link]:                https://pypi.org/project/signax/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/signax
 [pypi-version]:             https://img.shields.io/pypi/v/signax
 [rtd-badge]:                https://readthedocs.org/projects/signax/badge/?version=latest
 [rtd-link]:                 https://signax.readthedocs.io/en/latest/?badge=latest
 <!-- prettier-ignore-end -->
 
@@ -70,78 +74,80 @@
 ## Examples
 
 Basic usage
 
 ```python
 import jax
 import jax.random as jrandom
+import signax
 
-from signax.signature import signature
 
 key = jrandom.PRNGKey(0)
 depth = 3
 
 # compute signature for a single path
 length = 100
 dim = 20
 path = jrandom.normal(shape=(length, dim), key=key)
-output = signature(path, depth)
+output = signax.signature(path, depth)
 # output is a list of array representing tensor algebra
 
 # compute signature for batches (multiple) of paths
 # this is done via `jax.vmap`
 batch_size = 20
 path = jrandom.normal(shape=(batch_size, length, dim), key=key)
-output = jax.vmap(lambda x: signature(x, depth))(path)
+output = jax.vmap(lambda x: signax.signature(x, depth))(path)
 ```
 
-Integrate with [equinox](https://github.com/patrick-kidger/equinox) library
+Integrate with the [equinox](https://github.com/patrick-kidger/equinox) library
 
 ```python
 import equinox as eqx
 import jax.random as jrandom
 
 from signax.module import SignatureTransform
 
 # random generator key
 key = jrandom.PRNGKey(0)
 mlp_key, data_key = jrandom.split(key)
 
 depth = 3
 length, dim = 100, 3
 
-# we signature transfrom
+# create a signature transform at the specified depth
 signature_layer = SignatureTransform(depth=depth)
-# finally, getting output via a neural network
+
+# stack a MLP layer after that
 last_layer = eqx.nn.MLP(
     depth=1, in_size=3 + 3**2 + 3**3, width_size=4, out_size=1, key=mlp_key
 )
 
 model = eqx.nn.Sequential(layers=[signature_layer, last_layer])
 x = jrandom.normal(shape=(length, dim), key=data_key)
 output = model(x)
 ```
 
-Also, check notebooks in `examples` folder for some experiments of
+Also, check the notebooks in `examples` folder for some experiments that
+reproduce the results of the
 [deep signature transforms paper](https://arxiv.org/abs/1905.08494).
 
 ## Installation
 
 Via pip
 
 ```
-pip install signax
+python3 -m pip install signax
 ```
 
 Via source
 
 ```
 git clone https://github.com/anh-tong/signax.git
 cd signax
-python setup.py install .
+python3 -m pip install -v -e .
 ```
 
 ## Parallelism
 
 This implementation makes use of `jax.vmap` to perform the parallelism over
 batch dimension.
 
@@ -151,15 +157,15 @@
 Below plots are comparison of forward and backward pass in both GPU and CPU for
 path `size=(32, 128, 8)` and signature `depth=5`
 
 <table>
 <thead>
   <tr>
     <th >Forward</th>
-    <th > Backward</th>
+    <th >Backward</th>
   </tr>
 </thead>
 <tbody>
   <tr>
     <td>
         <img width="300" height="170" src="./assets/forward_gpu.png">
     </td>
```

