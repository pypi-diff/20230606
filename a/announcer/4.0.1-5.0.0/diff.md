# Comparing `tmp/announcer-4.0.1.tar.gz` & `tmp/announcer-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "announcer-4.0.1.tar", max compression
+gzip compressed data, was "announcer-5.0.0.tar", max compression
```

## Comparing `announcer-4.0.1.tar` & `announcer-5.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1089 2022-12-05 17:18:19.010224 announcer-4.0.1/LICENSE.md
--rw-r--r--   0        0        0     2491 2022-12-05 17:18:19.010224 announcer-4.0.1/README.md
--rw-r--r--   0        0        0     9819 2022-12-05 17:18:19.010224 announcer-4.0.1/announcer/__init__.py
--rw-r--r--   0        0        0     6926 2022-12-05 17:18:19.010224 announcer-4.0.1/announcer/changelogrenderer.py
--rw-r--r--   0        0        0     2991 2022-12-05 17:18:19.010224 announcer-4.0.1/announcer/teamschangelogrenderer.py
--rw-r--r--   0        0        0      770 2022-12-05 17:18:19.010224 announcer-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 announcer-4.0.1/setup.py
--rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 announcer-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-06 16:43:51.563922 announcer-5.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2682 2023-06-06 16:43:51.563922 announcer-5.0.0/README.md
+-rw-r--r--   0        0        0    10984 2023-06-06 16:43:51.563922 announcer-5.0.0/announcer/__init__.py
+-rw-r--r--   0        0        0     6923 2023-06-06 16:43:51.563922 announcer-5.0.0/announcer/changelogrenderer.py
+-rw-r--r--   0        0        0     2991 2023-06-06 16:43:51.563922 announcer-5.0.0/announcer/teamschangelogrenderer.py
+-rw-r--r--   0        0        0      825 2023-06-06 16:43:51.563922 announcer-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 announcer-5.0.0/PKG-INFO
```

### Comparing `announcer-4.0.1/LICENSE.md` & `announcer-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `announcer-4.0.1/README.md` & `announcer-5.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Github build](https://img.shields.io/github/workflow/status/metaswitch/announcer/Announcer)](https://github.com/Metaswitch/announcer)
+[![Github build](https://img.shields.io/github/actions/workflow/status/metaswitch/announcer/steps.yml?branch=main)](https://github.com/Metaswitch/announcer)
 [![pypi version](https://img.shields.io/pypi/v/announcer)](https://pypi.org/project/announcer/)
 [![docker pulls](https://img.shields.io/docker/pulls/metaswitch/announcer)](https://hub.docker.com/r/metaswitch/announcer)
 
 # announcer
 
 This tool:
 * takes an [keepachangelog](https://keepachangelog.com/en/1.0.0/)-style CHANGELOG.md file
@@ -18,15 +18,16 @@
 ```
 pip install announcer
 ```
 
 ## Tool usage
 
 ```
-usage: announce [-h] (--webhook WEBHOOK | --slackhook WEBHOOK) [--target {slack,teams}] --changelogversion CHANGELOGVERSION --changelogfile CHANGELOGFILE --projectname PROJECTNAME [--username USERNAME] [--iconurl ICONURL | --iconemoji ICONEMOJI]
+usage: announce [-h] (--webhook WEBHOOK | --slackhook WEBHOOK) [--target {slack,teams}] --changelogversion CHANGELOGVERSION --changelogfile CHANGELOGFILE --projectname PROJECTNAME
+                [--username USERNAME] [--compatibility-teams-sections] [--iconurl ICONURL | --iconemoji ICONEMOJI]
 
 Announce CHANGELOG changes on Slack and Microsoft Teams
 
 optional arguments:
   -h, --help            show this help message and exit
   --webhook WEBHOOK     The incoming webhook URL
   --slackhook WEBHOOK   The incoming webhook URL. (Deprecated)
@@ -35,27 +36,29 @@
   --changelogversion CHANGELOGVERSION
                         The changelog version to announce (e.g. 1.0.0)
   --changelogfile CHANGELOGFILE
                         The file containing changelog details (e.g. CHANGELOG.md)
   --projectname PROJECTNAME
                         The name of the project to announce (e.g. announcer)
   --username USERNAME   The username that the announcement will be made as (e.g. announcer). Valid for: Slack
+  --compatibility-teams-sections
+                        Compatibility option - sends Teams messages in multiple sections
   --iconurl ICONURL     A URL to use for the user icon in the announcement. Valid for: Slack
   --iconemoji ICONEMOJI
                         An emoji code to use for the user icon in the announcement (e.g. party_parrot). Valid for: Slack
 ```
 
 ## Gitlab Usage
 
 Announcer builds and publishes a Docker image that you can integrate into your `.gitlab-ci.yml`:
 
 ```
 announce:
   stage: announce
-  image: metaswitch/announcer:4.0.1
+  image: metaswitch/announcer:5.0.0
   script:
    - announce --webhook <webhook address>
               --changelogversion $CI_COMMIT_REF_NAME
               --changelogfile <CHANGELOG.md file>
               --projectname <Project name>
               --iconemoji party_parrot
   only:
```

### Comparing `announcer-4.0.1/announcer/__init__.py` & `announcer-5.0.0/announcer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,23 @@
    Teams channels"""
 
 import argparse
 import json
 import logging
 import re
 import sys
-from typing import Tuple, Optional, List, Dict, Any
 from enum import Enum
+from typing import Any, Dict, List, Optional, Tuple
 
-from .changelogrenderer import ChangeLogRenderer
-from .teamschangelogrenderer import TeamsChangeLogRenderer
 import mistletoe
 import requests
+from mistletoe.base_renderer import BaseRenderer
+
+from .changelogrenderer import ChangeLogRenderer
+from .teamschangelogrenderer import TeamsChangeLogRenderer
 
 log = logging.getLogger(__name__)
 
 
 DIFF_URL_RE = re.compile("^(.*)/compare/[^/]+[.][.][.]([^/]+)$")
 TREE_URL_RE = re.compile("^(.*)/tree/([^/]+)$")
 
@@ -65,27 +67,28 @@
     elif args.target is TargetTypes.TEAMS:
         log.info("Targeting Teams")
         announce_teams(
             args.webhook,
             args.changelogversion,
             args.changelogfile,
             args.projectname,
+            args.compatibility_teams_sections,
         )
     else:
         raise ValueError("Unknown target! {}".format(args.target))
 
 
 def announce_slack(
     webhook: str,
     changelogversion: str,
     changelogfile: str,
     projectname: str,
-    username: str = None,
-    icon_url: str = None,
-    icon_emoji: str = None,
+    username: Optional[str] = None,
+    icon_url: Optional[str] = None,
+    icon_emoji: Optional[str] = None,
 ):
     """Announce changelog changes to Slack"""
     # Get the changelog
     log.info("Querying changelog %s", changelogfile)
     changelog = Changelog(changelogfile, ChangeLogRenderer)
 
     # Get the version information
@@ -104,17 +107,17 @@
 
     # Make a message attachment.
     pretext = ["*{0} {1}*".format(projectname, changelogversion)]
 
     if base_url:
         pretext.append("({0})".format(base_url))
 
-    attachments = [
+    attachments: List[Dict[str, Any]] = [
         {"color": "good", "pretext": " ".join(pretext), "text": changelog_info}
-    ]  # type: List[Dict[str, Any]]
+    ]
 
     fallback = []
     actions = []
 
     if diff_url:
         # Add a button to view the changes at the diff URL
         fallback.append("View changes at {0}".format(diff_url))
@@ -130,48 +133,52 @@
 
     if actions:
         attachments.append(
             {"fallback": "\n".join(fallback), "color": "good", "actions": actions}
         )
 
     # Construct the data to send to the endpoint.
-    message_data = {"attachments": attachments}  # type: Dict[str, Any]
+    message_data: Dict[str, Any] = {"attachments": attachments}
 
     if username:
         message_data["username"] = username
 
     if icon_url:
         message_data["icon_url"] = icon_url
     elif icon_emoji:
         # Wrap the emoji name in colons to use that emoji
         message_data["icon_emoji"] = ":{}:".format(icon_emoji)
 
     log.debug("Sending info %s", message_data)
 
     # Send the data using requests to the webhook.
     r = requests.post(
-        webhook, json.dumps(message_data), headers={"Content-Type": "application/json"}
+        webhook,
+        json.dumps(message_data),
+        headers={"Content-Type": "application/json"},
+        timeout=10,
     )
     r.raise_for_status()
 
 
 def announce_teams(
     webhook: str,
     changelogversion: str,
     changelogfile: str,
     projectname: str,
+    compatibility_teams_sections: bool,
 ):
     """Announce changelog changes to Teams"""
     # Get the changelog
     log.info("Querying changelog %s", changelogfile)
     changelog = Changelog(changelogfile, TeamsChangeLogRenderer)
 
     # Get the version information
     log.info("Getting version %s info from changelog", changelogversion)
-    (changelog_info, diff_url, sections) = changelog.get_version_details(
+    (changelog_info, diff_url, compatibility_sections) = changelog.get_version_details(
         changelogversion
     )
 
     # Announce the information to Teams.
     log.info("Announcing information to Teams")
     log.debug("Webhook %s", webhook)
 
@@ -208,15 +215,20 @@
                         "os": "default",
                         "uri": changelog_url,
                     }
                 ],
             }
         )
 
-    if not sections:
+    if compatibility_teams_sections and compatibility_sections:
+        # Both compatibility has been requested and compatibility sections exist,
+        # use them.
+        sections = compatibility_sections
+    else:
+        # Use the generated HTML as the only section
         sections = [{"text": changelog_info}]
 
     message_data = {
         "@type": "MessageCard",
         "@context": "https://schema.org/extensions",
         "summary": "{0} {1}".format(projectname, changelogversion),
         "title": "{0} {1}".format(projectname, changelogversion),
@@ -226,21 +238,24 @@
     if actions:
         message_data["potentialAction"] = actions
 
     log.debug("Sending info %s", message_data)
 
     # Send the data using requests to the webhook.
     r = requests.post(
-        webhook, json.dumps(message_data), headers={"Content-Type": "application/json"}
+        webhook,
+        json.dumps(message_data),
+        headers={"Content-Type": "application/json"},
+        timeout=10,
     )
     r.raise_for_status()
 
 
 class Changelog(object):
-    def __init__(self, filename: str, renderer_class: mistletoe.BaseRenderer) -> None:
+    def __init__(self, filename: str, renderer_class: BaseRenderer) -> None:
         self.filename = filename
         self.renderer_class = renderer_class
 
     def get_version_details(
         self, version: str
     ) -> Tuple[str, Optional[str], List[Dict[str, str]]]:
         with open(self.filename, "r") as f:
@@ -254,21 +269,14 @@
         log.debug("Diff URL: %s", diff_url)
         return rendered, diff_url, sections
 
 
 def main():
     """Main handling function."""
 
-    # Set up basic logging
-    logging.basicConfig(
-        format="%(asctime)s %(levelname)-5.5s %(message)s",
-        stream=sys.stdout,
-        level=logging.DEBUG,
-    )
-
     # Run main script.
     parser = argparse.ArgumentParser(
         description="Announce CHANGELOG changes on Slack and Microsoft Teams"
     )
 
     # The new hook argument should just be called webhook.
     hook_group = parser.add_mutually_exclusive_group(required=True)
@@ -307,30 +315,64 @@
     )
     parser.add_argument(
         "--username",
         dest="username",
         help="The username that the announcement will be made as "
         "(e.g. announcer). Valid for: Slack",
     )
+    parser.add_argument(
+        "--compatibility-teams-sections",
+        action="store_true",
+        help="Compatibility option - sends Teams messages in multiple sections",
+    )
 
     icons = parser.add_mutually_exclusive_group()
     icons.add_argument(
         "--iconurl",
         dest="iconurl",
         help="A URL to use for the user icon in the announcement. Valid for: Slack",
     )
     icons.add_argument(
         "--iconemoji",
         dest="iconemoji",
         help="An emoji code to use for the user icon in the announcement "
         "(e.g. party_parrot). Valid for: Slack",
     )
 
+    volume = parser.add_mutually_exclusive_group()
+    volume.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Enable verbose logging",
+    )
+    volume.add_argument(
+        "-q",
+        "--quiet",
+        action="store_true",
+        help="Enable quiet output",
+    )
+
     args = parser.parse_args()
 
+    # Set up logging dependent on the options given
+    if args.verbose:
+        level = logging.DEBUG
+    elif args.quiet:
+        level = logging.WARNING
+    else:
+        level = logging.INFO
+
+    # Set up basic logging
+    logging.basicConfig(
+        format="%(asctime)s %(levelname)-5.5s %(message)s",
+        stream=sys.stdout,
+        level=level,
+    )
+
     try:
         announce(args)
     except Exception as e:
         log.exception(e)
         raise e
```

### Comparing `announcer-4.0.1/announcer/changelogrenderer.py` & `announcer-5.0.0/announcer/changelogrenderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         return token.content
 
     def render_heading(self, token):
         template = "*{}*\n" if token.level == 3 else "{}\n"
         return template.format(self.render_to_plaintext(token))
 
     def render_quote(self, token):
-        inner = self.render_to_inner(token)
+        inner = self.render_inner(token)
         return "> {}\n".format(inner)
 
     def render_paragraph(self, token):
         return self.render_inner(token)
 
     def render_block_code(self, token):
         template = "```\n{inner}```\n"
```

### Comparing `announcer-4.0.1/announcer/teamschangelogrenderer.py` & `announcer-5.0.0/announcer/teamschangelogrenderer.py`

 * *Files identical despite different names*

### Comparing `announcer-4.0.1/pyproject.toml` & `announcer-5.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [tool.poetry]
 name = "announcer"
-version = "4.0.1"
+version = "5.0.0"
 description = "Announce changes in keepachangelog-style CHANGELOG.md files to Slack and Microsoft Teams"
 authors = ["Max Dymond <max.dymond@metaswitch.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ['slack', 'teams']
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 requests = "^2.19"
-mistletoe = ">=0.7.1,<0.9.0"
+mistletoe = "^1"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13"
-wheel = "^0.38.4"
-mypy = "^0.982"
+wheel = "^0.40.0"
+mypy = "^1.3"
 yamllint = "^1.28"
 bandit = "^1.7"
 pytest = "^7.2"
-flake8 = "^5.0"
+flake8 = "^6.0"
 werkzeug = "^2.2.2"
 pytest-httpserver = "^1.0.6"
-tox = "^3.27"
-pytest-cov = "^4.0"
-types-requests = "^2.28.11"
+tox = "^4"
+pytest-cov = "^4.1"
+types-requests = "^2.31.0"
 
 [tool.poetry.scripts]
 announce = "announcer.__init__:main"
 
+[tool.poetry.group.dev.dependencies]
+flake8 = "^6.0.0"
+tox = "^4.5.1"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `announcer-4.0.1/setup.py` & `announcer-5.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,85 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: announcer
+Version: 5.0.0
+Summary: Announce changes in keepachangelog-style CHANGELOG.md files to Slack and Microsoft Teams
+License: MIT
+Keywords: slack,teams
+Author: Max Dymond
+Author-email: max.dymond@metaswitch.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: mistletoe (>=1,<2)
+Requires-Dist: requests (>=2.19,<3.0)
+Description-Content-Type: text/markdown
+
+[![Github build](https://img.shields.io/github/actions/workflow/status/metaswitch/announcer/steps.yml?branch=main)](https://github.com/Metaswitch/announcer)
+[![pypi version](https://img.shields.io/pypi/v/announcer)](https://pypi.org/project/announcer/)
+[![docker pulls](https://img.shields.io/docker/pulls/metaswitch/announcer)](https://hub.docker.com/r/metaswitch/announcer)
+
+# announcer
+
+This tool:
+* takes an [keepachangelog](https://keepachangelog.com/en/1.0.0/)-style CHANGELOG.md file
+* extracts all changes for a particular version
+* and sends a formatted message to a Slack or Microsoft Teams webhook.
+
+It is available as a Python package, or as a Docker container for use in CI.
+
+## Installation
+
+Install this tool using pip:
+
+```
+pip install announcer
+```
+
+## Tool usage
+
+```
+usage: announce [-h] (--webhook WEBHOOK | --slackhook WEBHOOK) [--target {slack,teams}] --changelogversion CHANGELOGVERSION --changelogfile CHANGELOGFILE --projectname PROJECTNAME
+                [--username USERNAME] [--compatibility-teams-sections] [--iconurl ICONURL | --iconemoji ICONEMOJI]
+
+Announce CHANGELOG changes on Slack and Microsoft Teams
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --webhook WEBHOOK     The incoming webhook URL
+  --slackhook WEBHOOK   The incoming webhook URL. (Deprecated)
+  --target {slack,teams}
+                        The type of announcement that should be sent to the webhook
+  --changelogversion CHANGELOGVERSION
+                        The changelog version to announce (e.g. 1.0.0)
+  --changelogfile CHANGELOGFILE
+                        The file containing changelog details (e.g. CHANGELOG.md)
+  --projectname PROJECTNAME
+                        The name of the project to announce (e.g. announcer)
+  --username USERNAME   The username that the announcement will be made as (e.g. announcer). Valid for: Slack
+  --compatibility-teams-sections
+                        Compatibility option - sends Teams messages in multiple sections
+  --iconurl ICONURL     A URL to use for the user icon in the announcement. Valid for: Slack
+  --iconemoji ICONEMOJI
+                        An emoji code to use for the user icon in the announcement (e.g. party_parrot). Valid for: Slack
+```
+
+## Gitlab Usage
+
+Announcer builds and publishes a Docker image that you can integrate into your `.gitlab-ci.yml`:
+
+```
+announce:
+  stage: announce
+  image: metaswitch/announcer:5.0.0
+  script:
+   - announce --webhook <webhook address>
+              --changelogversion $CI_COMMIT_REF_NAME
+              --changelogfile <CHANGELOG.md file>
+              --projectname <Project name>
+              --iconemoji party_parrot
+  only:
+    - tags
+```
 
-packages = \
-['announcer']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['mistletoe>=0.7.1,<0.9.0', 'requests>=2.19,<3.0']
-
-entry_points = \
-{'console_scripts': ['announce = announcer.__init__:main']}
-
-setup_kwargs = {
-    'name': 'announcer',
-    'version': '4.0.1',
-    'description': 'Announce changes in keepachangelog-style CHANGELOG.md files to Slack and Microsoft Teams',
-    'long_description': '[![Github build](https://img.shields.io/github/workflow/status/metaswitch/announcer/Announcer)](https://github.com/Metaswitch/announcer)\n[![pypi version](https://img.shields.io/pypi/v/announcer)](https://pypi.org/project/announcer/)\n[![docker pulls](https://img.shields.io/docker/pulls/metaswitch/announcer)](https://hub.docker.com/r/metaswitch/announcer)\n\n# announcer\n\nThis tool:\n* takes an [keepachangelog](https://keepachangelog.com/en/1.0.0/)-style CHANGELOG.md file\n* extracts all changes for a particular version\n* and sends a formatted message to a Slack or Microsoft Teams webhook.\n\nIt is available as a Python package, or as a Docker container for use in CI.\n\n## Installation\n\nInstall this tool using pip:\n\n```\npip install announcer\n```\n\n## Tool usage\n\n```\nusage: announce [-h] (--webhook WEBHOOK | --slackhook WEBHOOK) [--target {slack,teams}] --changelogversion CHANGELOGVERSION --changelogfile CHANGELOGFILE --projectname PROJECTNAME [--username USERNAME] [--iconurl ICONURL | --iconemoji ICONEMOJI]\n\nAnnounce CHANGELOG changes on Slack and Microsoft Teams\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --webhook WEBHOOK     The incoming webhook URL\n  --slackhook WEBHOOK   The incoming webhook URL. (Deprecated)\n  --target {slack,teams}\n                        The type of announcement that should be sent to the webhook\n  --changelogversion CHANGELOGVERSION\n                        The changelog version to announce (e.g. 1.0.0)\n  --changelogfile CHANGELOGFILE\n                        The file containing changelog details (e.g. CHANGELOG.md)\n  --projectname PROJECTNAME\n                        The name of the project to announce (e.g. announcer)\n  --username USERNAME   The username that the announcement will be made as (e.g. announcer). Valid for: Slack\n  --iconurl ICONURL     A URL to use for the user icon in the announcement. Valid for: Slack\n  --iconemoji ICONEMOJI\n                        An emoji code to use for the user icon in the announcement (e.g. party_parrot). Valid for: Slack\n```\n\n## Gitlab Usage\n\nAnnouncer builds and publishes a Docker image that you can integrate into your `.gitlab-ci.yml`:\n\n```\nannounce:\n  stage: announce\n  image: metaswitch/announcer:4.0.1\n  script:\n   - announce --webhook <webhook address>\n              --changelogversion $CI_COMMIT_REF_NAME\n              --changelogfile <CHANGELOG.md file>\n              --projectname <Project name>\n              --iconemoji party_parrot\n  only:\n    - tags\n```\n',
-    'author': 'Max Dymond',
-    'author_email': 'max.dymond@metaswitch.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

