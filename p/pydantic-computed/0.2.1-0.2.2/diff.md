# Comparing `tmp/pydantic_computed-0.2.1.tar.gz` & `tmp/pydantic_computed-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_computed-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_computed-0.2.2.tar", max compression
```

## Comparing `pydantic_computed-0.2.1.tar` & `pydantic_computed-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-02-08 12:06:25.711698 pydantic_computed-0.2.1/LICENSE
--rw-r--r--   0        0        0      109 2023-02-08 12:06:25.714841 pydantic_computed-0.2.1/pydantic_computed/__init__.py
--rw-r--r--   0        0        0     2008 2023-03-10 20:19:19.598193 pydantic_computed-0.2.1/pydantic_computed/decorator.py
--rw-r--r--   0        0        0       50 2023-02-08 12:06:25.715841 pydantic_computed-0.2.1/pydantic_computed/types.py
--rw-r--r--   0        0        0      637 2023-03-10 20:19:56.569766 pydantic_computed-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4010 2023-03-10 20:19:19.598193 pydantic_computed-0.2.1/README.md
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 pydantic_computed-0.2.1/setup.py
--rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 pydantic_computed-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-08 12:06:25.711698 pydantic_computed-0.2.2/LICENSE
+-rw-r--r--   0        0        0      109 2023-02-08 12:06:25.714841 pydantic_computed-0.2.2/pydantic_computed/__init__.py
+-rw-r--r--   0        0        0     2008 2023-03-10 20:19:19.598193 pydantic_computed-0.2.2/pydantic_computed/decorator.py
+-rw-r--r--   0        0        0       50 2023-02-08 12:06:25.715841 pydantic_computed-0.2.2/pydantic_computed/types.py
+-rw-r--r--   0        0        0      637 2023-06-06 12:30:26.542125 pydantic_computed-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4010 2023-03-10 20:19:19.598193 pydantic_computed-0.2.2/README.md
+-rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 pydantic_computed-0.2.2/setup.py
+-rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 pydantic_computed-0.2.2/PKG-INFO
```

### Comparing `pydantic_computed-0.2.1/LICENSE` & `pydantic_computed-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_computed-0.2.1/pydantic_computed/decorator.py` & `pydantic_computed-0.2.2/pydantic_computed/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic_computed-0.2.1/pyproject.toml` & `pydantic_computed-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pydantic-computed"
-version = "0.2.1"
+version = "0.2.2"
 description = "A new decorator for pydantic allowing you to define dynamic fields that are computed from other properties"
 authors = ["Jakob Leibetseder <leibetsederjakob@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Maydmor/pydantic-computed"
 packages = [{include = "pydantic_computed"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.10.2"
-setuptools = "^65.6.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
+setuptools = "^67.8.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_computed-0.2.1/README.md` & `pydantic_computed-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_computed-0.2.1/setup.py` & `pydantic_computed-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pydantic_computed']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pydantic>=1.10.2,<2.0.0', 'setuptools>=65.6.3,<66.0.0']
+['pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'pydantic-computed',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A new decorator for pydantic allowing you to define dynamic fields that are computed from other properties',
     'long_description': '# pydantic-computed\nA new decorator for pydantic allowing you to define dynamic fields that are computed from other properties.\n\n## Installation\n\nInstall the package by running\n```bash\npip install pydantic_computed\n```\n\n## Examples and use cases\n\n\n### A computed integer property\n```python\nfrom pydantic import BaseModel\nfrom pydantic_computed import Computed, computed\n\nclass ComputedModelInt(BaseModel):\n    a: int\n    b: int\n    c: Computed[int]\n    @computed(\'c\')\n    def calculate_c(a: int, b: int, **kwargs):\n        return a + b\n\nmodel = ComputedModelInt(a=1, b=2)\nprint(model.c) # Outputs 3\n```\n\n### Multiple computed properties\n\n```python\nfrom pydantic import BaseModel\nfrom pydantic_computed import Computed, computed\n\nclass MultipleComputed(BaseModel):\n    a: int\n    b: int\n    c: Computed[int]\n    d: Computed[int]\n    e: Computed[int]\n    @computed(\'c\')\n    def calc_c(a: int, b: int, **kwargs):\n        return a + b\n\n    @computed(\'d\')\n    def calc_d(c: int, **kwargs): # Note that property d uses the value of the computed property c (The order of declaration matters!)\n        return c * 2\n\nmodel = MultipleComputed(a=1, b=2)\nprint(model.c) # Outputs 3\nprint(model.d) # Outputs 6\n```\n\nSince all properties are passed as **kwargs to calculate_c, we can use the property names for the parameters\n\n\n### Complex types\n\nSuppose you set up a FastAPI application where you have users and orders stored in a database.\nAll Models in the database have an automatically generated id.\nNow you want to be able to dynamically generate links to those objects.\nE.g. the user with id=3 is accessible on the endpoint http://my-api/users/3\nInstead of storing those links in the database you can simply generate them with the computed decorator.\nexample: \n\n```python\nfrom pydantic import BaseModel, Field\nfrom pydantic_computed import Computed, computed\n\nclass Link(BaseModel):\n    href: str\n    method: str\n\nclass SchemaLinked(BaseModel):\n    id: int\n    base_url: str\n    link: Computed[Link]\n    @computed(\'link\')\n    def compute_link( id: int, base_url: str, **kwargs):        \n        return Link(href=f\'{base_url}/{id}\', method=\'GET\')\n\nclass User(SchemaLinked):\n    base_url: str = Field(\'/users\', exclude=True)\n    username: str\n\nclass Order(SchemaLinked):\n    base_url: str = Field(\'/orders\', exclude=True)\n    user: User\n\nuser = User(id=3, username=\'exampleuser\') \nuser.json()\n"""\n{\n    id: 3,\n    username: "exampleuser",\n    link: {\n        href: "/users/3",\n        method: "GET"\n    }\n}\n"""\norder = Order(id=2, user=user)\norder.json()\n"""\n{\n    id: 2,\n    link: {\n        href: "/orders/2",\n        method: "GET"\n    },\n    user: {\n        id: 3,\n        username: "exampleuser",\n        link: {\n            href: "/users/3",\n            method: "GET"\n        }\n    }\n}\n"""\n``` \n\n\n### Vector example:\n\n```python\nfrom pydantic import BaseModel\nfrom pydantic_computed import computed, Computed\nimport math\n\nclass Point(BaseModel):\n    x: int\n    y: int\n\nclass Vector(BaseModel):\n    p1: Point\n    p2: Point\n    x: Computed[float]\n    y: Computed[float]\n    weight: Computed[float]\n\n    @computed(\'x\')\n    def compute_x(p1: Point, p2: Point, **kwargs):\n        return p2.x - p1.x\n    @computed(\'y\')\n    def compute_y(p1: Point, p2: Point, **kwargs):\n        return p2.y - p1.y\n    @computed(\'weight\')\n    def compute_weight(x: float, y: float, **kwargs):\n        return math.sqrt(x ** 2 + y ** 2)\n\nv1 = Vector(p1=Point(x=0,y=0), p2=Point(x=1,y=0))\nprint(v1.weight) # Outputs 1.0\nv1.p2 = Point(x=2,y=0)\nprint(v1.weight) # Outputs now 2.0 since p2 changed\n# NOTE: if we would have written v1.p2.x = 2 instead of v1.p2 = Point(x=2, y=0), it would not have worked, because of the way pydantic triggers validations\n# The computed field only gets updated if one of the fields in the same model changes (in this case it is property p1 of Vector)\n```\n',
     'author': 'Jakob Leibetseder',
     'author_email': 'leibetsederjakob@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Maydmor/pydantic-computed',
```

### Comparing `pydantic_computed-0.2.1/PKG-INFO` & `pydantic_computed-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pydantic-computed
-Version: 0.2.1
+Version: 0.2.2
 Summary: A new decorator for pydantic allowing you to define dynamic fields that are computed from other properties
 Home-page: https://github.com/Maydmor/pydantic-computed
 License: MIT
 Author: Jakob Leibetseder
 Author-email: leibetsederjakob@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: setuptools (>=65.6.3,<66.0.0)
 Project-URL: Repository, https://github.com/Maydmor/pydantic-computed
 Description-Content-Type: text/markdown
 
 # pydantic-computed
 A new decorator for pydantic allowing you to define dynamic fields that are computed from other properties.
 
 ## Installation
```

