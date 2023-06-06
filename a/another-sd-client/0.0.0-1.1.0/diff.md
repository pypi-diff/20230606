# Comparing `tmp/another_sd_client-0.0.0.tar.gz` & `tmp/another_sd_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-0.0.0.tar", max compression
+gzip compressed data, was "another_sd_client-1.1.0.tar", max compression
```

## Comparing `another_sd_client-0.0.0.tar` & `another_sd_client-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     6296 2023-05-03 10:00:37.871563 another_sd_client-0.0.0/README.md
--rw-r--r--   0        0        0      928 2023-05-03 11:16:55.892993 another_sd_client-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 12:19:38.098523 another_sd_client-0.0.0/sdclient/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-03 11:28:12.353707 another_sd_client-0.0.0/sdclient/client.py
--rw-r--r--   0        0        0     3363 2023-05-10 10:55:22.137816 another_sd_client-0.0.0/sdclient/requests.py
--rw-r--r--   0        0        0     1331 2023-05-03 11:28:12.337707 another_sd_client-0.0.0/sdclient/responses.py
--rw-r--r--   0        0        0     7305 1970-01-01 00:00:00.000000 another_sd_client-0.0.0/setup.py
--rw-r--r--   0        0        0     7192 1970-01-01 00:00:00.000000 another_sd_client-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-06-06 11:49:40.431897 another_sd_client-1.1.0/README.md
+-rw-r--r--   0        0        0      898 2023-06-06 11:49:41.524998 another_sd_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 11:49:40.478902 another_sd_client-1.1.0/sdclient/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-06 11:49:40.432898 another_sd_client-1.1.0/sdclient/client.py
+-rw-r--r--   0        0        0     4905 2023-06-06 11:49:40.433898 another_sd_client-1.1.0/sdclient/requests.py
+-rw-r--r--   0        0        0     2697 2023-06-06 11:49:40.433898 another_sd_client-1.1.0/sdclient/responses.py
+-rw-r--r--   0        0        0     7229 1970-01-01 00:00:00.000000 another_sd_client-1.1.0/PKG-INFO
```

### Comparing `another_sd_client-0.0.0/README.md` & `another_sd_client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-0.0.0/pyproject.toml` & `another_sd_client-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 
 [tool.poetry]
 name = "another-sd-client"
-version = "0.0.0"  # versioning handled by conventional commits
+version = "1.1.0"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
@@ -20,14 +20,15 @@
 pre-commit = "^3.0.0"
 pytest-cov = "^4.0.0"
 click = "^8.1.3"
 pytest-asyncio = "^0.21.0"
 pytest-split = "^0.8.1"
 httpx = "^0.24.0"
 xmltodict = "^0.13.0"
+lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.pytest.ini_options]
 asyncio_mode="auto"
 
 [build-system]
```

### Comparing `another_sd_client-0.0.0/sdclient/client.py` & `another_sd_client-1.1.0/sdclient/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from typing import Tuple
 
 import httpx
 import xmltodict
 
 from sdclient.requests import GetDepartmentRequest
 from sdclient.requests import GetEmploymentRequest
+from sdclient.requests import GetOrganizationRequest
 from sdclient.requests import SDRequest
 from sdclient.responses import GetDepartmentResponse
 from sdclient.responses import GetEmploymentResponse
+from sdclient.responses import GetOrganizationResponse
 
 
 class SDClient:
     BASE_URL = "https://service.sd.dk/sdws/"
     ENDPOINT_SUFFIX = "20111201"
 
     def __init__(self, sd_username: str, sd_password: str, timeout: int = 120):
@@ -92,7 +94,25 @@
 
         Returns:
             XML response from SD converted to Pydantic
         """
 
         root_elem = self._call_sd(query_params, xml_force_list=("Person", "Employment"))
         return GetEmploymentResponse.parse_obj(root_elem)
+
+    def get_organization(
+        self, query_params: GetOrganizationRequest
+    ) -> GetOrganizationResponse:
+        """
+        Call the SD endpoint GetEmployment.
+
+        Args:
+            query_params: The HTTP query parameters to set in the request
+
+        Returns:
+            XML response from SD converted to Pydantic
+        """
+
+        root_elem = self._call_sd(
+            query_params, xml_force_list=("DepartmentReference", "Organization")
+        )
+        return GetOrganizationResponse.parse_obj(root_elem)
```

### Comparing `another_sd_client-0.0.0/sdclient/requests.py` & `another_sd_client-1.1.0/sdclient/requests.py`

 * *Files 27% similar despite different names*

```diff
@@ -97,7 +97,51 @@
     SalaryCodeGroupIndicator: bool = False
     WorkingTimeIndicator: bool = False
     UUIDIndicator: bool = False
 
     # TODO: add validator (not enough to set StatusActiveIndicator...)
     def get_name(self):
         return "GetEmployment"
+
+
+class GetOrganizationRequest(SDRequest):
+    """
+    Query parameters for SDs GetOrganization20111201 endpoint
+    """
+
+    InstitutionIdentifier: str | None = None
+    InstitutionUUIDIdentifier: UUID | None = None
+    ActivationDate: date
+    DeactivationDate: date
+    UUIDIndicator: bool = False
+
+    @root_validator
+    def check_values(cls, values):
+        institution_identifier = values.get("InstitutionIdentifier")
+        institution_uuid_identifier = values.get("InstitutionUUIDIdentifier")
+        activation_date = values.get("ActivationDate")
+        deactivation_date = values.get("DeactivationDate")
+
+        # Ensure that exactly one of "InstitutionIdentifier" and
+        # "InstitutionUUIDIdentifier" is set
+        if institution_identifier is None and institution_uuid_identifier is None:
+            raise ValueError(
+                "Exactly one of InstitutionIdentifier or InstitutionUUIDndentifier can be set"
+            )
+        if (
+            institution_identifier is not None
+            and institution_uuid_identifier is not None
+        ):
+            raise ValueError(
+                "Only one of InstitutionIdentifier and InstitutionUUIDIdentifier can be set"
+            )
+
+        # Ensure that "ActivationDate" is before "DeactivationDate"
+        if not activation_date <= deactivation_date:
+            raise ValueError(
+                "ActivationDate must be less than or equal to DeactivationDate"
+            )
+
+        return values
+
+    def get_name(self):
+        return "GetOrganization"
```

### Comparing `another_sd_client-0.0.0/setup.py` & `another_sd_client-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: another-sd-client
+Version: 1.1.0
+Summary: Client for communicating with SD Løn
+Home-page: https://magenta.dk/
+Keywords: os2mo,sd
+Author: Magenta ApS
+Author-email: info@magenta.dk
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
+Requires-Dist: pre-commit (>=3.0.0,<4.0.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
+Requires-Dist: pytest-split (>=0.8.1,<0.9.0)
+Requires-Dist: structlog (>=22.3.0,<23.0.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Project-URL: Repository, https://git.magenta.dk/rammearkitektur/another-sd-client
+Description-Content-Type: text/markdown
 
-packages = \
-['sdclient']
+# Another SD Client
 
-package_data = \
-{'': ['*']}
+SD client library for communicating with SD Løn
 
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'httpx>=0.24.0,<0.25.0',
- 'more-itertools>=9.0.0,<10.0.0',
- 'pre-commit>=3.0.0,<4.0.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'pytest-asyncio>=0.21.0,<0.22.0',
- 'pytest-cov>=4.0.0,<5.0.0',
- 'pytest-split>=0.8.1,<0.9.0',
- 'structlog>=22.3.0,<23.0.0',
- 'xmltodict>=0.13.0,<0.14.0']
-
-setup_kwargs = {
-    'name': 'another-sd-client',
-    'version': '0.0.0',
-    'description': 'Client for communicating with SD Løn',
-    'long_description': "# Another SD Client\n\nSD client library for communicating with SD Løn\n\n## Getting started\n\nTo make it easy for you to get started with GitLab, here's a list of recommended next steps.\n\nAlready a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!\n\n## Add your files\n\n- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files\n- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:\n\n```\ncd existing_repo\ngit remote add origin https://git.magenta.dk/rammearkitektur/another-sd-client.git\ngit branch -M master\ngit push -uf origin master\n```\n\n## Integrate with your tools\n\n- [ ] [Set up project integrations](https://git.magenta.dk/rammearkitektur/another-sd-client/-/settings/integrations)\n\n## Collaborate with your team\n\n- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)\n- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)\n- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)\n- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)\n- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)\n\n## Test and Deploy\n\nUse the built-in continuous integration in GitLab.\n\n- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)\n- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)\n- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)\n- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)\n- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)\n\n***\n\n# Editing this README\n\nWhen you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.\n\n## Suggestions for a good README\nEvery project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.\n\n## Name\nChoose a self-explaining name for your project.\n\n## Description\nLet people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.\n\n## Badges\nOn some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.\n\n## Visuals\nDepending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.\n\n## Installation\nWithin a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.\n\n## Usage\nUse examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.\n\n## Support\nTell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.\n\n## Roadmap\nIf you have ideas for releases in the future, it is a good idea to list them in the README.\n\n## Contributing\nState if you are open to contributions and what your requirements are for accepting them.\n\nFor people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.\n\nYou can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.\n\n## Authors and acknowledgment\nShow your appreciation to those who have contributed to the project.\n\n## License\nFor open source projects, say how it is licensed.\n\n## Project status\nIf you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.\n",
-    'author': 'Magenta ApS',
-    'author_email': 'info@magenta.dk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://magenta.dk/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
-}
+## Getting started
 
+To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+
+Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+
+## Add your files
+
+- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+
+```
+cd existing_repo
+git remote add origin https://git.magenta.dk/rammearkitektur/another-sd-client.git
+git branch -M master
+git push -uf origin master
+```
+
+## Integrate with your tools
+
+- [ ] [Set up project integrations](https://git.magenta.dk/rammearkitektur/another-sd-client/-/settings/integrations)
+
+## Collaborate with your team
+
+- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+
+## Test and Deploy
+
+Use the built-in continuous integration in GitLab.
+
+- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+
+***
+
+# Editing this README
+
+When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+
+## Suggestions for a good README
+Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+
+## Name
+Choose a self-explaining name for your project.
+
+## Description
+Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+
+## Badges
+On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+
+## Visuals
+Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+
+## Installation
+Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+
+## Usage
+Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+
+## Support
+Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+
+## Roadmap
+If you have ideas for releases in the future, it is a good idea to list them in the README.
+
+## Contributing
+State if you are open to contributions and what your requirements are for accepting them.
+
+For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+
+You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+
+## Authors and acknowledgment
+Show your appreciation to those who have contributed to the project.
+
+## License
+For open source projects, say how it is licensed.
+
+## Project status
+If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
 
-setup(**setup_kwargs)
```

