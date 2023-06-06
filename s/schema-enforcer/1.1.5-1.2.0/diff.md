# Comparing `tmp/schema-enforcer-1.1.5.tar.gz` & `tmp/schema_enforcer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-enforcer-1.1.5.tar", max compression
+gzip compressed data, was "schema_enforcer-1.2.0.tar", max compression
```

## Comparing `schema-enforcer-1.1.5.tar` & `schema_enforcer-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     2144 2022-07-27 14:43:24.858610 schema-enforcer-1.1.5/CHANGELOG.md
--rw-r--r--   0        0        0      602 2022-07-27 14:43:24.858610 schema-enforcer-1.1.5/LICENSE
--rwxr-xr-x   0        0        0    10111 2022-07-27 14:43:24.858610 schema-enforcer-1.1.5/README.md
--rwxr-xr-x   0        0        0     2131 2022-07-27 14:43:34.190734 schema-enforcer-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       86 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/__init__.py
--rw-r--r--   0        0        0    10605 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/ansible_inventory.py
--rw-r--r--   0        0        0    12629 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/cli.py
--rw-r--r--   0        0        0     4038 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/config.py
--rw-r--r--   0        0        0     1384 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/exceptions.py
--rw-r--r--   0        0        0     6980 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/instances/file.py
--rw-r--r--   0        0        0     6183 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/schemas/jsonschema.py
--rw-r--r--   0        0        0    13446 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/schemas/manager.py
--rw-r--r--   0        0        0     4022 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/schemas/validator.py
--rwxr-xr-x   0        0        0    18375 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/utils.py
--rw-r--r--   0        0        0     2608 2022-07-27 14:43:24.862610 schema-enforcer-1.1.5/schema_enforcer/validation.py
--rw-r--r--   0        0        0    11631 2022-07-27 14:43:35.076666 schema-enforcer-1.1.5/setup.py
--rw-r--r--   0        0        0    11455 2022-07-27 14:43:35.078065 schema-enforcer-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2303 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      602 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/LICENSE
+-rwxr-xr-x   0        0        0    10213 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/README.md
+-rwxr-xr-x   0        0        0     2125 2023-06-06 15:47:05.143261 schema_enforcer-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    10605 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/ansible_inventory.py
+-rw-r--r--   0        0        0    12629 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/cli.py
+-rw-r--r--   0        0        0     4038 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/config.py
+-rw-r--r--   0        0        0     1384 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/exceptions.py
+-rw-r--r--   0        0        0     6980 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/instances/file.py
+-rw-r--r--   0        0        0     6183 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/jsonschema.py
+-rw-r--r--   0        0        0    13446 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/manager.py
+-rw-r--r--   0        0        0     4022 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/validator.py
+-rwxr-xr-x   0        0        0    18375 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/utils.py
+-rw-r--r--   0        0        0     2608 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/validation.py
+-rw-r--r--   0        0        0    11611 1970-01-01 00:00:00.000000 schema_enforcer-1.2.0/PKG-INFO
```

### Comparing `schema-enforcer-1.1.5/CHANGELOG.md` & `schema_enforcer-1.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v1.2.0 - 2023-06-05
+
+### Adds
+
+- Support for versions of jsonschema >= 4.6
+
+### Removes
+
+- Support for versions of jsonschema < 4.6. See #141 for details.
+
 ## v1.1.5 - 2022-07-27
 
 ### Changes
 
 - Fixes #141 - Can not install schema-enforcer in environments which require a version of jsonschema < 4.6
 
 ## v1.1.4 - 2022-07-13
```

### Comparing `schema-enforcer-1.1.5/LICENSE` & `schema_enforcer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/README.md` & `schema_enforcer-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 'syslog.yml' = ['schemas/syslog_servers']
 ```
 
 > More information on available configuration settings can be found in the [configuration README](docs/configuration.md)
 
 ### Supported Formats
 
-By default, schema enforcer installs the jsonschema `format-nongpl` extra which allows the use of formats that can be used in schema definitions (e.g. ipv4, hostname...etc). The `format-nongpl` extra only installs transitive dependencies that are not licensed under GPL. The `iri` and `iri-reference` formats are defined by the `rfc3987` transitive dependency which is licensed under GPL. As such, `iri` and `iri-reference` formats are *not* supported by `format-nongpl`. If you have a need to use `iri` and/or `iri-reference` formats, you can do so by running the following pip command (or it's poetry equivalent):
+By default, schema enforcer installs the jsonschema `format_nongpl` extra (in version <1.2.0) or `format-nongpl` (in versions >=1.2.0). This extra allows the use of formats that can be used in schema definitions (e.g. ipv4, hostname...etc). The `format_nongpl` or `format-nongpl` extra only installs transitive dependencies that are not licensed under GPL. The `iri` and `iri-reference` formats are defined by the `rfc3987` transitive dependency which is licensed under GPL. As such, `iri` and `iri-reference` formats are *not* supported by `format-nongpl`/`format_nongpl`. If you have a need to use `iri` and/or `iri-reference` formats, you can do so by running the following pip command (or it's poetry equivalent):
 
 ```
 pip install 'jsonschema[rfc3987]'
 ```
 
 See the "Validating Formats" section in the [jsonschema documentation](https://github.com/python-jsonschema/jsonschema/blob/main/docs/validate.rst) for more information.
```

### Comparing `schema-enforcer-1.1.5/pyproject.toml` & `schema_enforcer-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schema-enforcer"
-version = "v1.1.5"
+version = "v1.2.0"
 description = "Tool/Framework for testing structured data against schema definitions"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode/schema-enforcer"
 repository = "https://github.com/networktocode/schema-enforcer"
 include = [
@@ -23,15 +23,15 @@
 jsonref = "^0.2"
 pydantic = "^1.6"
 rich = "^9.5"
 jsonpointer = "^2.1"
 jmespath = "^0.10"
 ansible = { version = "^2.10.0", optional = true }
 ansible-base = { version = "^2.10.0", optional = true }
-jsonschema = {version = ">3.2, <4.6", extras = ["format_nongpl"]}
+jsonschema = {version = "^4.6", extras = ["format-nongpl"]}
 
 [tool.poetry.extras]
 ansible = ["ansible"]
 ansible-base = ["ansible-base"]
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
```

### Comparing `schema-enforcer-1.1.5/schema_enforcer/ansible_inventory.py` & `schema_enforcer-1.2.0/schema_enforcer/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/cli.py` & `schema_enforcer-1.2.0/schema_enforcer/cli.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/config.py` & `schema_enforcer-1.2.0/schema_enforcer/config.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/exceptions.py` & `schema_enforcer-1.2.0/schema_enforcer/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/instances/file.py` & `schema_enforcer-1.2.0/schema_enforcer/instances/file.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/schemas/jsonschema.py` & `schema_enforcer-1.2.0/schema_enforcer/schemas/jsonschema.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/schemas/manager.py` & `schema_enforcer-1.2.0/schema_enforcer/schemas/manager.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/schemas/validator.py` & `schema_enforcer-1.2.0/schema_enforcer/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/utils.py` & `schema_enforcer-1.2.0/schema_enforcer/utils.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/schema_enforcer/validation.py` & `schema_enforcer-1.2.0/schema_enforcer/validation.py`

 * *Files identical despite different names*

### Comparing `schema-enforcer-1.1.5/setup.py` & `schema_enforcer-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,247 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: schema-enforcer
+Version: 1.2.0
+Summary: Tool/Framework for testing structured data against schema definitions
+Home-page: https://github.com/networktocode/schema-enforcer
+License: Apache-2.0
+Author: Network to Code, LLC
+Author-email: info@networktocode.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: ansible
+Provides-Extra: ansible-base
+Requires-Dist: ansible (>=2.10.0,<3.0.0) ; extra == "ansible"
+Requires-Dist: ansible-base (>=2.10.0,<3.0.0) ; extra == "ansible-base"
+Requires-Dist: click (>=7.1,<9.0)
+Requires-Dist: jinja2 (>=2.11)
+Requires-Dist: jmespath (>=0.10,<0.11)
+Requires-Dist: jsonpointer (>=2.1,<3.0)
+Requires-Dist: jsonref (>=0.2,<0.3)
+Requires-Dist: jsonschema[format-nongpl] (>=4.6,<5.0)
+Requires-Dist: pydantic (>=1.6,<2.0)
+Requires-Dist: rich (>=9.5,<10.0)
+Requires-Dist: ruamel.yaml (>=0.16,<0.18)
+Requires-Dist: termcolor (>=1.1,<2.0)
+Requires-Dist: toml (>=0.10,<0.11)
+Project-URL: Repository, https://github.com/networktocode/schema-enforcer
+Description-Content-Type: text/markdown
+
+# Schema Enforcer
+
+Schema Enforcer provides a framework for testing structured data against schema definitions. Right now, [JSONSchema](https://json-schema.org/understanding-json-schema/index.html) is the only schema definition language supported, but we are thinking about adding other schema definition languages at some point in the future.
+
+## Getting Started
+
+### Install
+
+Schema Enforcer is a python library which is available on PyPi. It requires a python version of 3.7 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.
+
+```cli
+bash$ python --version
+Python 3.7.9
+
+bash$ pip --version
+pip 20.1.1 from /usr/local/lib/python3.7/site-packages/pip (python 3.7)
+
+python -m pip install schema-enforcer
+```
+
+> Note: To determine the version of python your system is using, the command `python --version` can be run from a terminal emulator
+
+> Note: Pip is a package manager for python. While most recent versions of python come with pip installed, some do not. You can determine if pip is installed on your system using the command `pip --version`. If it is not, the instructions for installing it, once python has been installed, can be found [here](https://pip.pypa.io/en/stable/installing/)
+
+### Overview
+
+Schema Enforcer requires that two different elements be defined by the user:
+
+- Schema Definition Files: These are files which define the schema to which a given set of data should adhere.
+- Structured Data Files: These are files which contain data that should adhere to the schema defined in one (or multiple) of the schema definition files.
+
+> Note: Data which needs to be validated against a schema definition can come in the form of Structured Data Files or Ansible host vars. Ansible is not installed by default when schema-enforcer is installed. In order to use Ansible features, ansible must already be available or must be declared as an optional dependency when schema-enforcer upon installation. In the interest of brevity and simplicity, this README.md contains discussion only of Structured Data Files -- for more information on how to use `schema-enforcer` with ansible host vars, see [the ansible_command README](docs/ansible_command.md)
+
+When `schema-enforcer` runs, it assumes directory hierarchy which should be in place from the folder in which the tool is run.
+
+- `schema-enforcer` will search for **schema definition files** nested inside of `./schema/schemas/` which end in `.yml`, `.yaml`, or `.json`.
+- `schema-enforcer` will do a recursive search for **structured data files** starting in the current working diretory (`./`). It does this by searching all directories (including the current working directory) for files ending in `.yml`, `.yaml`, or `.json`. The `schema` folder and it's subdirectories are excluded from this search by default.
+
+```cli
+bash$ cd examples/example1
+bash$ tree
+.
+├── chi-beijing-rt1
+│   ├── dns.yml
+│   └── syslog.yml
+├── eng-london-rt1
+│   ├── dns.yml
+│   └── ntp.yml
+└── schema
+    └── schemas
+        ├── dns.yml
+        ├── ntp.yml
+        └── syslog.yml
+
+4 directories, 7 files
+```
+
+In the above example, `chi-beijing-rt1` is a directory with structured data files containing some configuration for a router named `chi-beijing-rt1`. There are two structured data files inside of this folder, `dns.yml` and `syslog.yml`. Similarly, the `eng-london-rt1` directory contains definition files for a router named `eng-london-rt1` -- `dns.yml` and `ntp.yml`.
+
+The file `chi-beijing-rt1/dns.yml` defines the DNS servers `chi-beijing.rt1` should use. The data in this file includes a simple hash-type data structure with a key of `dns_servers` and a value of an array. Each element in this array is a hash-type object with a key of `address` and a value which is the string of an IP address.
+
+```yaml
+bash$ cat chi-beijing-rt1/dns.yml
+# jsonschema: schemas/dns_servers
+---
+dns_servers:
+  - address: "10.1.1.1"
+  - address: "10.2.2.2"
+```
+> Note: The line `# jsonschema: schemas/dns_servers` tells `schema-enforcer` the ID of the schema which the structured data defined in the file should be validated against. The schema ID is defined by the `$id` top level key in a schema definition. More information on how the structured data is mapped to a schema ID to which it should adhere can be found in the [mapping_schemas README](./docs/mapping_schemas.md)
+
+The file `schema/schemas/dns.yml` is a schema definition file. It contains a schema definition for ntp servers written in JSONSchema. The data in `chi-beijing-rt1/dns.yml` and `eng-london-rt1/dns.yml` should adhere to the schema defined in this schema definition file.
+
+```yaml
+bash$ cat schema/schemas/dns.yml
+---
+$schema: "http://json-schema.org/draft-07/schema#"
+$id: "schemas/dns_servers"
+description: "DNS Server Configuration schema."
+type: "object"
+properties:
+  dns_servers:
+    type: "array"
+    items:
+      type: "object"
+      properties:
+        name:
+          type: "string"
+        address:
+          type: "string"
+          format: "ipv4"
+        vrf:
+          type: "string"
+      required:
+        - "address"
+      uniqueItems: true
+required:
+  - "dns_servers"
+```
+
+> Note: The cat of the schema definition file may be a little scary if you haven't seen JSONSchema before. Don't worry too much if it is difficult to parse right now. The important thing to note is that this file contains a schema definition to which the structured data in the files `chi-beijing-rt1/dns.yml` and `eng-london-rt1/dns.yml` should adhere.
+
+### Basic usage
+
+Once schema-enforcer has been installed, the `schema-enforcer validate` command can be used run schema validations of YAML/JSON instance files against the defined schema.
+
+```shell
+bash$ schema-enforcer --help
+Usage: schema-enforcer [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  ansible        Validate the hostvar for all hosts within an Ansible...
+  schema         Manage your schemas
+  validate       Validates instance files against defined schema
+```
+
+To run the schema validations, the command `schema-enforcer validate` can be run.
+
+```shell
+bash$ schema-enforcer validate
+schema-enforcer validate
+ALL SCHEMA VALIDATION CHECKS PASSED
+```
+
+To acquire more context regarding what files specifically passed schema validation, the `--show-pass` flag can be passed in.
+
+```shell
+bash$ schema-enforcer validate --show-pass
+PASS [FILE] ./eng-london-rt1/ntp.yml
+PASS [FILE] ./eng-london-rt1/dns.yml
+PASS [FILE] ./chi-beijing-rt1/syslog.yml
+PASS [FILE] ./chi-beijing-rt1/dns.yml
+ALL SCHEMA VALIDATION CHECKS PASSED
+```
+
+If we modify one of the addresses in the `chi-beijing-rt1/dns.yml` file so that it's value is the boolean `true` instead of an IP address string, then run the `schema-enforcer` tool, the validation will fail with an error message.
+
+```yaml
+bash$ cat chi-beijing-rt1/dns.yml
+# jsonschema: schemas/dns_servers
+---
+dns_servers:
+  - address: true
+  - address: "10.2.2.2"
+```
+```shell
+bash$ test-schema validate
+FAIL | [ERROR] True is not of type 'string' [FILE] ./chi-beijing-rt1/dns.yml [PROPERTY] dns_servers:0:address
+bash$ echo $?
+1
+```
+
+When a structured data file fails schema validation, `schema-enforcer` exits with a code of 1.
+
+### Configuration Settings
+
+Schema enforcer will work with default settings, however, a `pyproject.toml` file can be placed at the root of the path in which `schema-enforcer` is run in order to override default settings or declare configuration for more advanced features. Inside of this `pyproject.toml` file, `tool.schema_enforcer` sections can be used to declare settings for schema enforcer. Take for example the `pyproject.toml` file in example 2.
+
+```shell
+bash$ cd examples/example2 && tree -L 2
+.
+├── README.md
+├── hostvars
+│   ├── chi-beijing-rt1
+│   ├── eng-london-rt1
+│   └── ger-berlin-rt1
+├── invalid
+├── pyproject.toml
+└── schema
+    ├── definitions
+    └── schemas
+
+8 directories, 2 files
+```
+
+In this toml file, a schema mapping is declared which tells schema enforcer which structured data files should be checked by which schema IDs.
+
+
+```shell
+bash$ cat pyproject.toml
+[tool.schema_enforcer.schema_mapping]
+# Map structured data filename to schema IDs
+'dns_v1.yml' = ['schemas/dns_servers']
+'dns_v2.yml' = ['schemas/dns_servers_v2']
+'syslog.yml' = ['schemas/syslog_servers']
+```
+
+> More information on available configuration settings can be found in the [configuration README](docs/configuration.md)
+
+### Supported Formats
+
+By default, schema enforcer installs the jsonschema `format_nongpl` extra (in version <1.2.0) or `format-nongpl` (in versions >=1.2.0). This extra allows the use of formats that can be used in schema definitions (e.g. ipv4, hostname...etc). The `format_nongpl` or `format-nongpl` extra only installs transitive dependencies that are not licensed under GPL. The `iri` and `iri-reference` formats are defined by the `rfc3987` transitive dependency which is licensed under GPL. As such, `iri` and `iri-reference` formats are *not* supported by `format-nongpl`/`format_nongpl`. If you have a need to use `iri` and/or `iri-reference` formats, you can do so by running the following pip command (or it's poetry equivalent):
+
+```
+pip install 'jsonschema[rfc3987]'
+```
+
+See the "Validating Formats" section in the [jsonschema documentation](https://github.com/python-jsonschema/jsonschema/blob/main/docs/validate.rst) for more information.
+
+### Where To Go Next
+
+Detailed documentation can be found in the README.md files inside of the `docs/` directory.
+- ["Introducing Schema Enforcer" blog post](https://blog.networktocode.com/post/introducing_schema_enforcer/)
+- [Using a pyproject.toml file for configuration](docs/configuration.md)
+- [Mapping Structured Data Files to Schema Files](docs/mapping_data_files_to_schemas.md)
+- [The `ansible` command](docs/ansible_command.md)
+- [The `validate` command](docs/validate_command.md)
+- [The `schema` command](docs/schema_command.md)
+- [Implementing custom validators](docs/custom_validators.md)
 
-packages = \
-['schema_enforcer', 'schema_enforcer.instances', 'schema_enforcer.schemas']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=7.1,<9.0',
- 'jinja2>=2.11',
- 'jmespath>=0.10,<0.11',
- 'jsonpointer>=2.1,<3.0',
- 'jsonref>=0.2,<0.3',
- 'jsonschema[format_nongpl]>3.2,<4.6',
- 'pydantic>=1.6,<2.0',
- 'rich>=9.5,<10.0',
- 'ruamel.yaml>=0.16,<0.18',
- 'termcolor>=1.1,<2.0',
- 'toml>=0.10,<0.11']
-
-extras_require = \
-{'ansible': ['ansible>=2.10.0,<3.0.0'],
- 'ansible-base': ['ansible-base>=2.10.0,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['schema-enforcer = schema_enforcer.cli:main']}
-
-setup_kwargs = {
-    'name': 'schema-enforcer',
-    'version': '1.1.5',
-    'description': 'Tool/Framework for testing structured data against schema definitions',
-    'long_description': '# Schema Enforcer\n\nSchema Enforcer provides a framework for testing structured data against schema definitions. Right now, [JSONSchema](https://json-schema.org/understanding-json-schema/index.html) is the only schema definition language supported, but we are thinking about adding other schema definition languages at some point in the future.\n\n## Getting Started\n\n### Install\n\nSchema Enforcer is a python library which is available on PyPi. It requires a python version of 3.7 or greater. Once a supported version of python is installed on your machine, pip can be used to install the tool by using the command `python -m pip install schema-enforcer`.\n\n```cli\nbash$ python --version\nPython 3.7.9\n\nbash$ pip --version\npip 20.1.1 from /usr/local/lib/python3.7/site-packages/pip (python 3.7)\n\npython -m pip install schema-enforcer\n```\n\n> Note: To determine the version of python your system is using, the command `python --version` can be run from a terminal emulator\n\n> Note: Pip is a package manager for python. While most recent versions of python come with pip installed, some do not. You can determine if pip is installed on your system using the command `pip --version`. If it is not, the instructions for installing it, once python has been installed, can be found [here](https://pip.pypa.io/en/stable/installing/)\n\n### Overview\n\nSchema Enforcer requires that two different elements be defined by the user:\n\n- Schema Definition Files: These are files which define the schema to which a given set of data should adhere.\n- Structured Data Files: These are files which contain data that should adhere to the schema defined in one (or multiple) of the schema definition files.\n\n> Note: Data which needs to be validated against a schema definition can come in the form of Structured Data Files or Ansible host vars. Ansible is not installed by default when schema-enforcer is installed. In order to use Ansible features, ansible must already be available or must be declared as an optional dependency when schema-enforcer upon installation. In the interest of brevity and simplicity, this README.md contains discussion only of Structured Data Files -- for more information on how to use `schema-enforcer` with ansible host vars, see [the ansible_command README](docs/ansible_command.md)\n\nWhen `schema-enforcer` runs, it assumes directory hierarchy which should be in place from the folder in which the tool is run.\n\n- `schema-enforcer` will search for **schema definition files** nested inside of `./schema/schemas/` which end in `.yml`, `.yaml`, or `.json`.\n- `schema-enforcer` will do a recursive search for **structured data files** starting in the current working diretory (`./`). It does this by searching all directories (including the current working directory) for files ending in `.yml`, `.yaml`, or `.json`. The `schema` folder and it\'s subdirectories are excluded from this search by default.\n\n```cli\nbash$ cd examples/example1\nbash$ tree\n.\n├── chi-beijing-rt1\n│   ├── dns.yml\n│   └── syslog.yml\n├── eng-london-rt1\n│   ├── dns.yml\n│   └── ntp.yml\n└── schema\n    └── schemas\n        ├── dns.yml\n        ├── ntp.yml\n        └── syslog.yml\n\n4 directories, 7 files\n```\n\nIn the above example, `chi-beijing-rt1` is a directory with structured data files containing some configuration for a router named `chi-beijing-rt1`. There are two structured data files inside of this folder, `dns.yml` and `syslog.yml`. Similarly, the `eng-london-rt1` directory contains definition files for a router named `eng-london-rt1` -- `dns.yml` and `ntp.yml`.\n\nThe file `chi-beijing-rt1/dns.yml` defines the DNS servers `chi-beijing.rt1` should use. The data in this file includes a simple hash-type data structure with a key of `dns_servers` and a value of an array. Each element in this array is a hash-type object with a key of `address` and a value which is the string of an IP address.\n\n```yaml\nbash$ cat chi-beijing-rt1/dns.yml\n# jsonschema: schemas/dns_servers\n---\ndns_servers:\n  - address: "10.1.1.1"\n  - address: "10.2.2.2"\n```\n> Note: The line `# jsonschema: schemas/dns_servers` tells `schema-enforcer` the ID of the schema which the structured data defined in the file should be validated against. The schema ID is defined by the `$id` top level key in a schema definition. More information on how the structured data is mapped to a schema ID to which it should adhere can be found in the [mapping_schemas README](./docs/mapping_schemas.md)\n\nThe file `schema/schemas/dns.yml` is a schema definition file. It contains a schema definition for ntp servers written in JSONSchema. The data in `chi-beijing-rt1/dns.yml` and `eng-london-rt1/dns.yml` should adhere to the schema defined in this schema definition file.\n\n```yaml\nbash$ cat schema/schemas/dns.yml\n---\n$schema: "http://json-schema.org/draft-07/schema#"\n$id: "schemas/dns_servers"\ndescription: "DNS Server Configuration schema."\ntype: "object"\nproperties:\n  dns_servers:\n    type: "array"\n    items:\n      type: "object"\n      properties:\n        name:\n          type: "string"\n        address:\n          type: "string"\n          format: "ipv4"\n        vrf:\n          type: "string"\n      required:\n        - "address"\n      uniqueItems: true\nrequired:\n  - "dns_servers"\n```\n\n> Note: The cat of the schema definition file may be a little scary if you haven\'t seen JSONSchema before. Don\'t worry too much if it is difficult to parse right now. The important thing to note is that this file contains a schema definition to which the structured data in the files `chi-beijing-rt1/dns.yml` and `eng-london-rt1/dns.yml` should adhere.\n\n### Basic usage\n\nOnce schema-enforcer has been installed, the `schema-enforcer validate` command can be used run schema validations of YAML/JSON instance files against the defined schema.\n\n```shell\nbash$ schema-enforcer --help\nUsage: schema-enforcer [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  ansible        Validate the hostvar for all hosts within an Ansible...\n  schema         Manage your schemas\n  validate       Validates instance files against defined schema\n```\n\nTo run the schema validations, the command `schema-enforcer validate` can be run.\n\n```shell\nbash$ schema-enforcer validate\nschema-enforcer validate\nALL SCHEMA VALIDATION CHECKS PASSED\n```\n\nTo acquire more context regarding what files specifically passed schema validation, the `--show-pass` flag can be passed in.\n\n```shell\nbash$ schema-enforcer validate --show-pass\nPASS [FILE] ./eng-london-rt1/ntp.yml\nPASS [FILE] ./eng-london-rt1/dns.yml\nPASS [FILE] ./chi-beijing-rt1/syslog.yml\nPASS [FILE] ./chi-beijing-rt1/dns.yml\nALL SCHEMA VALIDATION CHECKS PASSED\n```\n\nIf we modify one of the addresses in the `chi-beijing-rt1/dns.yml` file so that it\'s value is the boolean `true` instead of an IP address string, then run the `schema-enforcer` tool, the validation will fail with an error message.\n\n```yaml\nbash$ cat chi-beijing-rt1/dns.yml\n# jsonschema: schemas/dns_servers\n---\ndns_servers:\n  - address: true\n  - address: "10.2.2.2"\n```\n```shell\nbash$ test-schema validate\nFAIL | [ERROR] True is not of type \'string\' [FILE] ./chi-beijing-rt1/dns.yml [PROPERTY] dns_servers:0:address\nbash$ echo $?\n1\n```\n\nWhen a structured data file fails schema validation, `schema-enforcer` exits with a code of 1.\n\n### Configuration Settings\n\nSchema enforcer will work with default settings, however, a `pyproject.toml` file can be placed at the root of the path in which `schema-enforcer` is run in order to override default settings or declare configuration for more advanced features. Inside of this `pyproject.toml` file, `tool.schema_enforcer` sections can be used to declare settings for schema enforcer. Take for example the `pyproject.toml` file in example 2.\n\n```shell\nbash$ cd examples/example2 && tree -L 2\n.\n├── README.md\n├── hostvars\n│   ├── chi-beijing-rt1\n│   ├── eng-london-rt1\n│   └── ger-berlin-rt1\n├── invalid\n├── pyproject.toml\n└── schema\n    ├── definitions\n    └── schemas\n\n8 directories, 2 files\n```\n\nIn this toml file, a schema mapping is declared which tells schema enforcer which structured data files should be checked by which schema IDs.\n\n\n```shell\nbash$ cat pyproject.toml\n[tool.schema_enforcer.schema_mapping]\n# Map structured data filename to schema IDs\n\'dns_v1.yml\' = [\'schemas/dns_servers\']\n\'dns_v2.yml\' = [\'schemas/dns_servers_v2\']\n\'syslog.yml\' = [\'schemas/syslog_servers\']\n```\n\n> More information on available configuration settings can be found in the [configuration README](docs/configuration.md)\n\n### Supported Formats\n\nBy default, schema enforcer installs the jsonschema `format-nongpl` extra which allows the use of formats that can be used in schema definitions (e.g. ipv4, hostname...etc). The `format-nongpl` extra only installs transitive dependencies that are not licensed under GPL. The `iri` and `iri-reference` formats are defined by the `rfc3987` transitive dependency which is licensed under GPL. As such, `iri` and `iri-reference` formats are *not* supported by `format-nongpl`. If you have a need to use `iri` and/or `iri-reference` formats, you can do so by running the following pip command (or it\'s poetry equivalent):\n\n```\npip install \'jsonschema[rfc3987]\'\n```\n\nSee the "Validating Formats" section in the [jsonschema documentation](https://github.com/python-jsonschema/jsonschema/blob/main/docs/validate.rst) for more information.\n\n### Where To Go Next\n\nDetailed documentation can be found in the README.md files inside of the `docs/` directory.\n- ["Introducing Schema Enforcer" blog post](https://blog.networktocode.com/post/introducing_schema_enforcer/)\n- [Using a pyproject.toml file for configuration](docs/configuration.md)\n- [Mapping Structured Data Files to Schema Files](docs/mapping_data_files_to_schemas.md)\n- [The `ansible` command](docs/ansible_command.md)\n- [The `validate` command](docs/validate_command.md)\n- [The `schema` command](docs/schema_command.md)\n- [Implementing custom validators](docs/custom_validators.md)\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'info@networktocode.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/networktocode/schema-enforcer',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

