# Comparing `tmp/jupyverse-0.1.8.tar.gz` & `tmp/jupyverse-0.1.9.tar.gz`

## Comparing `jupyverse-0.1.8.tar` & `jupyverse-0.1.9.tar`

### file list

```diff
@@ -1,217 +1,218 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0    63500 2020-02-02 00:00:00.000000 jupyverse-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.8/config.yaml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.8/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.8/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.1.8/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.1.8/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    14935 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.8/README.md
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 jupyverse-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    64563 2020-02-02 00:00:00.000000 jupyverse-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.9/config.yaml
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.9/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.9/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.9/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.9/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.1.9/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.1.9/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 jupyverse-0.1.9/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_kernels.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.9/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.9/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.9/README.md
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 jupyverse-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.9/PKG-INFO
```

### Comparing `jupyverse-0.1.8/.pre-commit-config.yaml` & `jupyverse-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/CHANGELOG.md` & `jupyverse-0.1.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 0.1.8
+## 0.1.9
 
-No merged PRs
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.8...ab09a2ea41fcdab226ec55541a26329c3d5b7583))
+
+### Merged PRs
+
+- Fix fps-webdav logging config [#317](https://github.com/jupyter-server/jupyverse/pull/317) ([@davidbrochart](https://github.com/davidbrochart))
+- Fix fps-auth-fief [#316](https://github.com/jupyter-server/jupyverse/pull/316) ([@davidbrochart](https://github.com/davidbrochart))
+- Handle binary (base64-encoded) files [#315](https://github.com/jupyter-server/jupyverse/pull/315) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-05-31&to=2023-06-06&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-05-31..2023-06-06&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Atrungleduc+updated%3A2023-05-31..2023-06-06&type=Issues)
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 0.1.8
+
+No merged PRs
+
 ## 0.1.7
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.6...d1d54a22429136b87fd45b7540d43937b2e6b695))
 
 ### Merged PRs
 
 - Add WebDAV plugin [#312](https://github.com/jupyter-server/jupyverse/pull/312) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.1.8/CONTRIBUTING.md` & `jupyverse-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/config.yaml` & `jupyverse-0.1.9/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/mkdocs.yml` & `jupyverse-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/.devcontainer/devcontainer.json` & `jupyverse-0.1.9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/.github/workflows/check-release.yml` & `jupyverse-0.1.9/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/.github/workflows/main.yml` & `jupyverse-0.1.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/binder/jupyter_notebook_config.py` & `jupyverse-0.1.9/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/index.md` & `jupyverse-0.1.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/install.md` & `jupyverse-0.1.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/jupyter.svg` & `jupyverse-0.1.9/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/plugins/auth.md` & `jupyverse-0.1.9/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/usage/microservices.md` & `jupyverse-0.1.9/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/usage/multi_user.md` & `jupyverse-0.1.9/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/docs/usage/single_user.md` & `jupyverse-0.1.9/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/COPYING.md` & `jupyverse-0.1.9/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/pyproject.toml` & `jupyverse-0.1.9/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     @property
     @abstractmethod
     def file_id_manager(self) -> FileIdManager:
         ...
 
     @abstractmethod
     async def read_content(
-        self, path: Union[str, Path], get_content: bool, as_json: bool = False
+        self, path: Union[str, Path], get_content: bool, file_format: Optional[str] = None
     ) -> Content:
         ...
 
     @abstractmethod
     async def write_content(self, content: Union[SaveContent, Dict]) -> None:
         ...
```

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.1.9/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/notebooks/admin_users.ipynb` & `jupyverse-0.1.9/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/notebooks/admin_users.py` & `jupyverse-0.1.9/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/COPYING.md` & `jupyverse-0.1.9/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/pyproject.toml` & `jupyverse-0.1.9/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/fps_auth/backends.py` & `jupyverse-0.1.9/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/fps_auth/config.py` & `jupyverse-0.1.9/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/fps_auth/db.py` & `jupyverse-0.1.9/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/fps_auth/main.py` & `jupyverse-0.1.9/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth/fps_auth/routes.py` & `jupyverse-0.1.9/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth_fief/COPYING.md` & `jupyverse-0.1.9/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth_fief/pyproject.toml` & `jupyverse-0.1.9/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,110 @@
+from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 from fastapi import Depends, HTTPException, Request, Response, WebSocket, status
 from fastapi.security import APIKeyCookie
 from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
 from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
-class Backend:
-    def __init__(self, auth_fief_config: _AuthFiefConfig):
-        class CustomFiefAuth(FiefAuth):
-            client: FiefAsync
-
-            async def get_unauthorized_response(self, request: Request, response: Response):
-                redirect_uri = str(request.url_for("auth_callback"))
-                auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
-                raise HTTPException(
-                    status_code=status.HTTP_307_TEMPORARY_REDIRECT,
-                    headers={"Location": auth_url},
-                )
-
-        self.fief = FiefAsync(
-            auth_fief_config.base_url,
-            auth_fief_config.client_id,
-            auth_fief_config.client_secret,
+class CustomFiefAuth(FiefAuth):
+    client: FiefAsync
+
+    async def get_unauthorized_response(self, request: Request, response: Response):
+        redirect_uri = str(request.url_for("auth_callback"))
+        auth_url = await self.client.auth_url(redirect_uri, scope=["openid"])
+        raise HTTPException(
+            status_code=status.HTTP_307_TEMPORARY_REDIRECT,
+            headers={"Location": auth_url},
         )
 
-        self.SESSION_COOKIE_NAME = "fps_auth_fief_user_session"
-        scheme = APIKeyCookie(name=self.SESSION_COOKIE_NAME, auto_error=False)
-        self.auth = CustomFiefAuth(self.fief, scheme)
-
-        async def update_user(
-            user: FiefUserInfo = Depends(self.auth.current_user()),
-            access_token_info: FiefAccessTokenInfo = Depends(self.auth.authenticated()),
-        ):
-            async def _(data: Dict[str, Any]) -> FiefUserInfo:
-                user = await self.fief.update_profile(
-                    access_token_info["access_token"], {"fields": data}
-                )
-                return user
-
-            return _
-
-        def websocket_auth(permissions: Optional[Dict[str, List[str]]] = None):
-            async def _(
-                websocket: WebSocket,
-            ) -> Optional[Tuple[WebSocket, Optional[Dict[str, List[str]]]]]:
-                accept_websocket = False
-                checked_permissions: Optional[Dict[str, List[str]]] = None
-                if self.SESSION_COOKIE_NAME in websocket._cookies:
-                    access_token = websocket._cookies[self.SESSION_COOKIE_NAME]
-                    if permissions is None:
-                        accept_websocket = True
-                    else:
-                        checked_permissions = {}
-                        for resource, actions in permissions.items():
-                            allowed = checked_permissions[resource] = []
-                            for action in actions:
-                                try:
-                                    await self.fief.validate_access_token(
-                                        access_token, required_permissions=[f"{resource}:{action}"]
-                                    )
-                                except BaseException:
-                                    pass
-                                else:
-                                    allowed.append(action)
-                                    accept_websocket = True
-                if accept_websocket:
-                    return websocket, checked_permissions
+
+@dataclass
+class Res:
+    fief: FiefAsync
+    session_cookie_name: str
+    auth: CustomFiefAuth
+    current_user: Any
+    update_user: Any
+    websocket_auth: Any
+
+
+def get_backend(auth_fief_config: _AuthFiefConfig) -> Res:
+    fief = FiefAsync(
+        auth_fief_config.base_url,
+        auth_fief_config.client_id,
+        auth_fief_config.client_secret,
+    )
+
+    session_cookie_name = "fps_auth_fief_user_session"
+    scheme = APIKeyCookie(name=session_cookie_name, auto_error=False)
+    auth = CustomFiefAuth(fief, scheme)
+
+    async def update_user(
+        user: FiefUserInfo = Depends(auth.current_user()),
+        access_token_info: FiefAccessTokenInfo = Depends(auth.authenticated()),
+    ):
+        async def _(data: Dict[str, Any]) -> FiefUserInfo:
+            user = await fief.update_profile(access_token_info["access_token"], {"fields": data})
+            return user
+
+        return _
+
+    def websocket_auth(permissions: Optional[Dict[str, List[str]]] = None):
+        async def _(
+            websocket: WebSocket,
+        ) -> Optional[Tuple[WebSocket, Optional[Dict[str, List[str]]]]]:
+            accept_websocket = False
+            checked_permissions: Optional[Dict[str, List[str]]] = None
+            if session_cookie_name in websocket._cookies:
+                access_token = websocket._cookies[session_cookie_name]
+                if permissions is None:
+                    accept_websocket = True
                 else:
-                    await websocket.close(code=status.WS_1008_POLICY_VIOLATION)
-                    return None
+                    checked_permissions = {}
+                    for resource, actions in permissions.items():
+                        allowed = checked_permissions[resource] = []
+                        for action in actions:
+                            try:
+                                await fief.validate_access_token(
+                                    access_token, required_permissions=[f"{resource}:{action}"]
+                                )
+                            except BaseException:
+                                pass
+                            else:
+                                allowed.append(action)
+                                accept_websocket = True
+            if accept_websocket:
+                return websocket, checked_permissions
+            else:
+                await websocket.close(code=status.WS_1008_POLICY_VIOLATION)
+                return None
+
+        return _
+
+    def current_user(permissions=None):
+        if permissions is not None:
+            permissions = [
+                f"{resource}:{action}"
+                for resource, actions in permissions.items()
+                for action in actions
+            ]
+
+        async def _(
+            user: FiefUserInfo = Depends(auth.current_user(permissions=permissions)),
+        ):
+            return User(**user["fields"])
 
-            return _
+        return _
 
-        def current_user(permissions=None):
-            if permissions is not None:
-                permissions = [
-                    f"{resource}:{action}"
-                    for resource, actions in permissions.items()
-                    for action in actions
-                ]
-
-            async def _(
-                user: FiefUserInfo = Depends(self.auth.current_user(permissions=permissions)),
-            ):
-                return User(**user["fields"])
-
-            return _
-
-        self.current_user = current_user
-        self.update_user = update_user
-        self.websocket_auth = websocket_auth
+    return Res(
+        fief=fief,
+        session_cookie_name=session_cookie_name,
+        auth=auth,
+        current_user=current_user,
+        update_user=update_user,
+        websocket_auth=websocket_auth,
+    )
```

### Comparing `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from asphalt.core import Component, Context
 from jupyverse_api.auth import Auth, AuthConfig
 from jupyverse_api.app import App
 
 from .config import _AuthFiefConfig
-from .routes import _AuthFief
+from .routes import auth_factory
 
 
 class AuthFiefComponent(Component):
     def __init__(self, **kwargs):
         self.auth_fief_config = _AuthFiefConfig(**kwargs)
 
     async def start(
         self,
         ctx: Context,
     ) -> None:
         ctx.add_resource(self.auth_fief_config, types=AuthConfig)
 
         app = await ctx.request_resource(App)
 
-        auth_fief = _AuthFief(app, self.auth_fief_config)
+        auth_fief = auth_factory(app, self.auth_fief_config)
         ctx.add_resource(auth_fief, types=Auth)
```

### Comparing `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.1.9/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 import json
-from typing import Dict, List
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from fastapi import APIRouter, Depends, Query, Request, Response
 from fastapi.responses import RedirectResponse
 from fief_client import FiefAccessTokenInfo
 from jupyverse_api import Router
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 
-from .backend import Backend
+from .backend import get_backend
 from .config import _AuthFiefConfig
 
 
-class _AuthFief(Backend, Auth, Router):
-    def __init__(
-        self,
-        app: App,
-        auth_fief_config: _AuthFiefConfig,
-    ) -> None:
-        Router.__init__(self, app)
-        Backend.__init__(self, auth_fief_config)
-
-        router = APIRouter()
-
-        @router.get("/auth-callback", name="auth_callback")
-        async def auth_callback(request: Request, response: Response, code: str = Query(...)):
-            redirect_uri = str(request.url_for("auth_callback"))
-            tokens, _ = await self.fief.auth_callback(code, redirect_uri)
-
-            response = RedirectResponse(request.url_for("root"))
-            response.set_cookie(
-                self.SESSION_COOKIE_NAME,
-                tokens["access_token"],
-                max_age=tokens["expires_in"],
-                httponly=True,
-                secure=False,
-            )
-
-            return response
-
-        @router.get("/api/me")
-        async def get_api_me(
-            request: Request,
-            user: User = Depends(self.current_user()),
-            access_token_info: FiefAccessTokenInfo = Depends(self.auth.authenticated()),
-        ):
-            checked_permissions: Dict[str, List[str]] = {}
-            permissions = json.loads(
-                dict(request.query_params).get("permissions", "{}").replace("'", '"')
-            )
-            if permissions:
-                user_permissions: Dict[str, List[str]] = {}
-                for permission in access_token_info["permissions"]:
-                    resource, action = permission.split(":")
-                    if resource not in user_permissions:
-                        user_permissions[resource] = []
-                    user_permissions[resource].append(action)
-                for resource, actions in permissions.items():
-                    user_resource_permissions = user_permissions.get(resource, [])
-                    allowed = checked_permissions[resource] = []
-                    for action in actions:
-                        if action in user_resource_permissions:
-                            allowed.append(action)
-
-            keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
-            identity = {k: getattr(user, k) for k in keys}
-            return {
-                "identity": identity,
-                "permissions": checked_permissions,
-            }
+def auth_factory(
+    app: App,
+    auth_fief_config: _AuthFiefConfig,
+):
+    backend = get_backend(auth_fief_config)
+
+    class _AuthFief(Auth, Router):
+        def __init__(self) -> None:
+            super().__init__(app)
+
+            router = APIRouter()
+
+            @router.get("/auth-callback", name="auth_callback")
+            async def auth_callback(request: Request, response: Response, code: str = Query(...)):
+                redirect_uri = str(request.url_for("auth_callback"))
+                tokens, _ = await backend.fief.auth_callback(code, redirect_uri)
+
+                response = RedirectResponse(request.url_for("root"))
+                response.set_cookie(
+                    backend.session_cookie_name,
+                    tokens["access_token"],
+                    max_age=tokens["expires_in"],
+                    httponly=True,
+                    secure=False,
+                )
+
+                return response
+
+            @router.get("/api/me")
+            async def get_api_me(
+                request: Request,
+                user: User = Depends(self.current_user()),
+                access_token_info: FiefAccessTokenInfo = Depends(backend.auth.authenticated()),
+            ):
+                checked_permissions: Dict[str, List[str]] = {}
+                permissions = json.loads(
+                    dict(request.query_params).get("permissions", "{}").replace("'", '"')
+                )
+                if permissions:
+                    user_permissions: Dict[str, List[str]] = {}
+                    for permission in access_token_info["permissions"]:
+                        resource, action = permission.split(":")
+                        if resource not in user_permissions:
+                            user_permissions[resource] = []
+                        user_permissions[resource].append(action)
+                    for resource, actions in permissions.items():
+                        user_resource_permissions = user_permissions.get(resource, [])
+                        allowed = checked_permissions[resource] = []
+                        for action in actions:
+                            if action in user_resource_permissions:
+                                allowed.append(action)
+
+                keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
+                identity = {k: getattr(user, k) for k in keys}
+                return {
+                    "identity": identity,
+                    "permissions": checked_permissions,
+                }
+
+            self.include_router(router)
+
+        def current_user(self, permissions: Optional[Dict[str, List[str]]] = None) -> Callable:
+            return backend.current_user(permissions)
+
+        async def update_user(self, update_user=Depends(backend.update_user)) -> Callable:
+            return update_user
+
+        def websocket_auth(
+            self,
+            permissions: Optional[Dict[str, List[str]]] = None,
+        ) -> Callable[[], Tuple[Any, Dict[str, List[str]]]]:
+            return backend.websocket_auth(permissions)
 
-        self.include_router(router)
+    return _AuthFief()
```

### Comparing `jupyverse-0.1.8/plugins/contents/COPYING.md` & `jupyverse-0.1.9/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/contents/pyproject.toml` & `jupyverse-0.1.9/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.1.9/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/contents/fps_contents/routes.py` & `jupyverse-0.1.9/plugins/contents/fps_contents/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import json
 import os
 import shutil
 from datetime import datetime
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
@@ -133,32 +134,36 @@
         user: User,
     ):
         rename_content = RenameContent(**(await request.json()))
         Path(path).rename(rename_content.path)
         return await self.read_content(rename_content.path, False)
 
     async def read_content(
-        self, path: Union[str, Path], get_content: bool, as_json: bool = False
+        self, path: Union[str, Path], get_content: bool, file_format: Optional[str] = None
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
         if get_content:
             if path.is_dir():
                 content = [
                     (await self.read_content(subpath, get_content=False)).dict()
                     for subpath in path.iterdir()
                     if not subpath.name.startswith(".")
                 ]
             elif path.is_file() or path.is_symlink():
                 try:
-                    async with await open_file(path) as f:
-                        content = await f.read()
-                    if as_json:
-                        content = json.loads(content)
+                    async with await open_file(path, mode="rb") as f:
+                        content_bytes = await f.read()
+                    if file_format == "base64":
+                        content = base64.b64encode(content_bytes).decode("ascii")
+                    elif file_format == "json":
+                        content = json.loads(content_bytes)
+                    else:
+                        content = content_bytes.decode()
                 except Exception:
                     raise HTTPException(status_code=404, detail="Item not found")
         format: Optional[str] = None
         if path.is_dir():
             size = None
             type = "directory"
             format = "json"
@@ -167,25 +172,25 @@
             size = get_file_size(path)
             if path.suffix == ".ipynb":
                 type = "notebook"
                 format = None
                 mimetype = None
                 if content is not None:
                     nb: dict
-                    if as_json:
+                    if file_format == "json":
                         content = cast(Dict, content)
                         nb = content
                     else:
                         content = cast(str, content)
                         nb = json.loads(content)
                     for cell in nb["cells"]:
                         if "metadata" not in cell:
                             cell["metadata"] = {}
                         cell["metadata"].update({"trusted": False})
-                    if not as_json:
+                    if file_format != "json":
                         content = json.dumps(nb)
             elif path.suffix == ".json":
                 type = "json"
                 format = "text"
                 mimetype = "application/json"
             else:
                 type = "file"
@@ -208,32 +213,41 @@
                 "type": type,
             }
         )
 
     async def write_content(self, content: Union[SaveContent, Dict]) -> None:
         if not isinstance(content, SaveContent):
             content = SaveContent(**content)
-        async with await open_file(content.path, "w") as f:
-            if content.format == "json":
-                dict_content = cast(Dict, content.content)
-                if content.type == "notebook":
-                    # see https://github.com/jupyterlab/jupyterlab/issues/11005
-                    if "metadata" in dict_content and "orig_nbformat" in dict_content["metadata"]:
-                        del dict_content["metadata"]["orig_nbformat"]
-                await f.write(json.dumps(dict_content, indent=2))
-            else:
+        if content.format == "base64":
+            async with await open_file(content.path, "wb") as f:
                 content.content = cast(str, content.content)
-                await f.write(content.content)
+                content_bytes = content.content.encode("ascii")
+                await f.write(content_bytes)
+        else:
+            async with await open_file(content.path, "wt") as f:
+                if content.format == "json":
+                    dict_content = cast(Dict, content.content)
+                    if content.type == "notebook":
+                        # see https://github.com/jupyterlab/jupyterlab/issues/11005
+                        if (
+                            "metadata" in dict_content
+                            and "orig_nbformat" in dict_content["metadata"]
+                        ):
+                            del dict_content["metadata"]["orig_nbformat"]
+                    await f.write(json.dumps(dict_content, indent=2))
+                else:
+                    content.content = cast(str, content.content)
+                    await f.write(content.content)
 
     @property
     def file_id_manager(self):
         return FileIdManager()
 
 
-def get_available_path(path: Path, sep: str = ""):
+def get_available_path(path: Path, sep: str = "") -> Path:
     directory = path.parent
     name = Path(path.name)
     i = None
     while True:
         if i is None:
             i_str = ""
             i = 1
```

### Comparing `jupyverse-0.1.8/plugins/frontend/COPYING.md` & `jupyverse-0.1.9/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/frontend/pyproject.toml` & `jupyverse-0.1.9/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/jupyterlab/COPYING.md` & `jupyverse-0.1.9/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.1.9/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.1.9/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/COPYING.md` & `jupyverse-0.1.9/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/pyproject.toml` & `jupyverse-0.1.9/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.1.9/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/lab/COPYING.md` & `jupyverse-0.1.9/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/lab/pyproject.toml` & `jupyverse-0.1.9/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/lab/fps_lab/main.py` & `jupyverse-0.1.9/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/lab/fps_lab/routes.py` & `jupyverse-0.1.9/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.1.9/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/COPYING.md` & `jupyverse-0.1.9/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/pyproject.toml` & `jupyverse-0.1.9/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/routes.py` & `jupyverse-0.1.9/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/index.html` & `jupyverse-0.1.9/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.1.9/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.1.9/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.1.9/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.1.9/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/nbconvert/COPYING.md` & `jupyverse-0.1.9/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/nbconvert/pyproject.toml` & `jupyverse-0.1.9/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.1.9/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/noauth/COPYING.md` & `jupyverse-0.1.9/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/noauth/pyproject.toml` & `jupyverse-0.1.9/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.1.9/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/resource_usage/COPYING.md` & `jupyverse-0.1.9/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/resource_usage/pyproject.toml` & `jupyverse-0.1.9/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.1.9/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/retrolab/COPYING.md` & `jupyverse-0.1.9/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/retrolab/pyproject.toml` & `jupyverse-0.1.9/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.1.9/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.1.9/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/COPYING.md` & `jupyverse-0.1.9/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/pyproject.toml` & `jupyverse-0.1.9/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.1.9/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.1.9/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.1.9/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.1.9/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/webdav/COPYING.md` & `jupyverse-0.1.9/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/webdav/pyproject.toml` & `jupyverse-0.1.9/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.1.9/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/yjs/COPYING.md` & `jupyverse-0.1.9/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/yjs/pyproject.toml` & `jupyverse-0.1.9/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.1.9/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.1.9/plugins/yjs/fps_yjs/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,17 +171,16 @@
                 # cancel that since there is a new client
                 self.cleaners[room].cancel()
             if not room.ready:
                 file_path = await self.contents.file_id_manager.get_path(file_id)
                 logger.info(f"Opening collaboration room: {websocket.path} ({file_path})")
                 document = YDOCS.get(file_type, YFILE)(room.ydoc)
                 self.documents[websocket.path] = document
-                is_notebook = file_type == "notebook"
                 async with self.lock:
-                    model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                    model = await self.contents.read_content(file_path, True, file_format)
                 assert model.last_modified is not None
                 self.last_modified[file_id] = to_datetime(model.last_modified)
                 if not room.ready:
                     # try to apply Y updates from the YStore for this document
                     try:
                         await room.ystore.apply_updates(room.ydoc)
                         read_from_source = False
@@ -197,19 +196,21 @@
                     if read_from_source:
                         document.source = model.content
                         await room.ystore.encode_state_as_update(room.ydoc)
 
                     document.dirty = False
                     room.ready = True
                     # save the document to file when changed
-                    document.observe(partial(self.on_document_change, file_id, file_type, document))
+                    document.observe(
+                        partial(self.on_document_change, file_id, file_type, file_format, document)
+                    )
                     # update the document when file changes
                     if file_id not in self.watchers:
                         self.watchers[file_id] = asyncio.create_task(
-                            self.watch_file(file_type, file_id, document)
+                            self.watch_file(file_format, file_id, document)
                         )
 
         await self.websocket_server.serve(websocket)
 
         if is_stored_document and not room.clients:
             # no client in this room after we disconnect
             self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
@@ -241,91 +242,92 @@
         file_path = await self.contents.file_id_manager.get_path(file_id)
         if file_path is None:
             return
         if file_path != document.path:
             document.path = file_path
         return file_path
 
-    async def watch_file(self, file_type: str, file_id: str, document: YBaseDoc) -> None:
+    async def watch_file(self, file_format: str, file_id: str, document: YBaseDoc) -> None:
         file_path = await self.get_file_path(file_id, document)
         assert file_path is not None
         logger.debug(f"Watching file: {file_path}")
         while True:
             watcher = self.contents.file_id_manager.watch(file_path)
             async for changes in watcher:
                 new_file_path = await self.get_file_path(file_id, document)
                 if new_file_path is None:
                     continue
                 if new_file_path != file_path:
                     # file was renamed
                     self.contents.file_id_manager.unwatch(file_path, watcher)
                     file_path = new_file_path
                     # break
-                await self.maybe_load_file(file_type, file_path, file_id)
+                await self.maybe_load_file(file_format, file_path, file_id)
 
-    async def maybe_load_file(self, file_type: str, file_path: str, file_id: str) -> None:
+    async def maybe_load_file(self, file_format: str, file_path: str, file_id: str) -> None:
         async with self.lock:
             model = await self.contents.read_content(file_path, False)
         # do nothing if the file was saved by us
         assert model.last_modified is not None
         if self.last_modified[file_id] < to_datetime(model.last_modified):
             # the file was not saved by us, update the shared document(s)
-            is_notebook = file_type == "notebook"
             async with self.lock:
-                model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                model = await self.contents.read_content(file_path, True, file_format)
             assert model.last_modified is not None
             documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
             for document in documents:
                 document.source = model.content
             self.last_modified[file_id] = to_datetime(model.last_modified)
 
     def on_document_change(
-        self, file_id: str, file_type: str, document: YBaseDoc, target, event
+        self, file_id: str, file_type: str, file_format: str, document: YBaseDoc, target, event
     ) -> None:
         if target == "state" and "dirty" in event.keys:
             dirty = event.keys["dirty"]["newValue"]
             if not dirty:
                 # we cleared the dirty flag, nothing to save
                 return
         # unobserve and observe again because the structure of the document may have changed
         # e.g. a new cell added to a notebook
         document.unobserve()
-        document.observe(partial(self.on_document_change, file_id, file_type, document))
+        document.observe(
+            partial(self.on_document_change, file_id, file_type, file_format, document)
+        )
         if file_id in self.savers:
             self.savers[file_id].cancel()
         self.savers[file_id] = asyncio.create_task(
-            self.maybe_save_document(file_id, file_type, document)
+            self.maybe_save_document(file_id, file_type, file_format, document)
         )
 
-    async def maybe_save_document(self, file_id: str, file_type: str, document: YBaseDoc) -> None:
+    async def maybe_save_document(
+        self, file_id: str, file_type: str, file_format: str, document: YBaseDoc
+    ) -> None:
         # save after 1 second of inactivity to prevent too frequent saving
         await asyncio.sleep(1)  # FIXME: pass in config
         # if the room cannot be found, don't save
         try:
             file_path = await self.get_file_path(file_id, document)
         except BaseException:
             return
         assert file_path is not None
-        is_notebook = file_type == "notebook"
         async with self.lock:
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            model = await self.contents.read_content(file_path, True, file_format)
         assert model.last_modified is not None
         if self.last_modified[file_id] < to_datetime(model.last_modified):
             # file changed on disk, let's revert
             document.source = model.content
             self.last_modified[file_id] = to_datetime(model.last_modified)
             return
         if model.content != document.source:
             # don't save if not needed
             # this also prevents the dirty flag from bouncing between windows of
             # the same document opened as different types (e.g. notebook/text editor)
-            format = "json" if file_type == "notebook" else "text"
             content = {
                 "content": document.source,
-                "format": format,
+                "format": file_format,
                 "path": file_path,
                 "type": file_type,
             }
             async with self.lock:
                 await self.contents.write_content(content)
                 model = await self.contents.read_content(file_path, False)
             assert model.last_modified is not None
```

### Comparing `jupyverse-0.1.8/tests/conftest.py` & `jupyverse-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/test_auth.py` & `jupyverse-0.1.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/test_contents.py` & `jupyverse-0.1.9/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/test_kernels.py` & `jupyverse-0.1.9/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/test_server.py` & `jupyverse-0.1.9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/test_settings.py` & `jupyverse-0.1.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/utils.py` & `jupyverse-0.1.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/tests/data/notebook0.ipynb` & `jupyverse-0.1.9/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/.gitignore` & `jupyverse-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/COPYING.md` & `jupyverse-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/README.md` & `jupyverse-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/pyproject.toml` & `jupyverse-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.8/PKG-INFO` & `jupyverse-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

