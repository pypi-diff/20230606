# Comparing `tmp/sbmltoodejax-0.2.tar.gz` & `tmp/sbmltoodejax-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmltoodejax-0.2.tar", last modified: Thu Mar 30 09:52:27 2023, max compression
+gzip compressed data, was "sbmltoodejax-0.3.tar", last modified: Tue Jun  6 15:07:25 2023, max compression
```

## Comparing `sbmltoodejax-0.2.tar` & `sbmltoodejax-0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2022-10-27 19:27:34.000000 sbmltoodejax-0.2/LICENSE
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1340 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      845 2022-11-15 20:10:26.000000 sbmltoodejax-0.2/README.md
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/sbmltoodejax/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      344 2022-11-15 15:57:38.000000 sbmltoodejax-0.2/sbmltoodejax/__init__.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5728 2022-11-09 16:36:25.000000 sbmltoodejax-0.2/sbmltoodejax/biomodels_api.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1036 2022-11-29 21:00:37.000000 sbmltoodejax-0.2/sbmltoodejax/jaxfuncs.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    25862 2023-01-24 10:02:24.000000 sbmltoodejax-0.2/sbmltoodejax/modulegeneration.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1185 2023-01-24 09:48:04.000000 sbmltoodejax-0.2/sbmltoodejax/parse.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/sbmltoodejax.egg-info/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1340 2023-03-30 09:52:27.000000 sbmltoodejax-0.2/sbmltoodejax.egg-info/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      370 2023-03-30 09:52:27.000000 sbmltoodejax-0.2/sbmltoodejax.egg-info/SOURCES.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2023-03-30 09:52:27.000000 sbmltoodejax-0.2/sbmltoodejax.egg-info/dependency_links.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2023-03-30 09:52:27.000000 sbmltoodejax-0.2/sbmltoodejax.egg-info/requires.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2023-03-30 09:52:27.000000 sbmltoodejax-0.2/sbmltoodejax.egg-info/top_level.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/setup.cfg
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      783 2023-03-30 09:50:54.000000 sbmltoodejax-0.2/setup.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-03-30 09:52:27.762655 sbmltoodejax-0.2/test/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     7391 2022-12-12 20:56:14.000000 sbmltoodejax-0.2/test/test_modulegeneration.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.018816 sbmltoodejax-0.3/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/LICENSE
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5037 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     4504 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/README.md
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/sbmltoodejax/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      344 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/__init__.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     6062 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/biomodels_api.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2552 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    25792 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/modulegeneration.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2689 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/parse.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     3054 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/utils.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/sbmltoodejax.egg-info/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5037 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      414 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/requires.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/top_level.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2023-06-06 15:07:25.018816 sbmltoodejax-0.3/setup.cfg
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      821 2023-06-06 15:07:18.000000 sbmltoodejax-0.3/setup.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/test/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1641 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/test/test_jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2461 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/test/test_modulegeneration.py
```

### Comparing `sbmltoodejax-0.2/LICENSE` & `sbmltoodejax-0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Mayalen Etcheverry
+Copyright (c) 2023 Mayalen Etcheverry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sbmltoodejax-0.2/sbmltoodejax/biomodels_api.py` & `sbmltoodejax-0.3/sbmltoodejax/biomodels_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """
-CREDIT: The biomodels_api code is copied (and slightly adapated) from the basico repository:
-<https://github.com/copasi/basico/blob/d058c10dd51f2c3e926efeaa29c6194f86bfdc90/basico/biomodels.py#L47>
-that is maintained by the COPASI group and under Artistic License 2.0
+This provides several utils functions for accessing the BioModels API as described on https://www.ebi.ac.uk/biomodels/docs/
+
+See Also:
+    The biomodels_api code and documentation is copied (and slightly adapated) from the basico repository that is maintained by the COPASI group and under Artistic License 2.0.
+    The original code can be found at https://github.com/copasi/basico/blob/master/basico/biomodels.py
+    
+Note:
+    The only (minor) modification with respect to original code is that we deal with special characters in :func:`~sbmltoodejax.biomodels_api.get_content_for_model` using ``urllib.parse.quote``
 
-This provides several utils functions for accessing the BioModels API as described on:
-    <https://www.ebi.ac.uk/biomodels/docs/>
 
 Examples:
-    >>>  # get info for a specific model
-    >>>  info = get_model_info(12)
-    >>>  print(info['name'], info['files']['main'][0]['name'])
-    >>>  # get all files for one model
-    >>>  files = get_files_for_model(12)
-    >>>  print(files['main'][0]['name'])
-    >>>  # get content of specific model
-    >>>  sbml = get_content_for_model(12)
-    >>>  print(sbml)
-    >>>  # search for model
-    >>>  models = search_for_model('repressilator')
-    >>>  for model in models:
-    >>>     print(model['id'], model['name'], model['format'])
+    .. code-block:: python
+    
+        # get info for a specific model
+        info = get_model_info(12)
+        print(info['name'], info['files']['main'][0]['name'])
+        # get all files for one model
+        files = get_files_for_model(12)
+        print(files['main'][0]['name'])
+        # get content of specific model
+        sbml = get_content_for_model(12)
+        print(sbml)
+        # search for model
+        models = search_for_model('repressilator')
+        for model in models:
+           print(model['id'], model['name'], model['format'])
 """
 
 try:
     import sys
     if sys.version_info.major == 2:
         import urllib as urllib2
         from urllib import quote_plus
@@ -41,91 +46,109 @@
 
 
 END_POINT = 'https://www.ebi.ac.uk/biomodels/'
 
 def download_from(url):
     """Convenience method reading content from a URL.
     This convenience method uses urlopen on either python 2.7 or 3.x
-    :param url: the url to read from
-    :type url: str
-    :return: the contents of the URL as str
-    :rtype: str
+
+    Args:
+        url (str): the url to read from
+
+    Returns:
+        str: the contents of the URL as str
     """
     if _use_urllib2:
         content = urllib2.urlopen(url).read()
     else:
         content = urllib.request.urlopen(url).read().decode('utf-8')
     return content
 
 
 def download_json(url):
     """Convenience method reading the content of the url as JSON.
-    :param url: the url to read from
-    :type url: str
-    :return: a python object representing the json content loaded
-    :rtype: dict
+
+    Args:
+        url (str): the url to read from
+
+    Returns:
+        dict: a python object representing the json content loaded
     """
     content = download_from(url)
     return json.loads(content)
 
 
 def get_model_info(model_id):
     """Return the model info for the provided `model_id`.
-    :param model_id: either an integer, or a valid model id
-    :return: a python object describing the model
+
+    Args:
+        model_id: either an integer, or a valid model id
+
+    Returns:
+        a python object describing the model
     """
     if type(model_id) is int:
         model_id = 'BIOMD{0:010d}'.format(model_id)
     result = download_json(END_POINT + model_id + '?format=json')
     return result
 
 
 def get_files_for_model(model_id):
     """Retrieves the json structure for all files for the given biomodel.
     The structure is of form:
-    >>> get_files_for_model(10)
-    {
-        'additional': [
-            {'description': 'Auto-generated Scilab file',
-             'fileSize': '3873',
-             'name': 'BIOMD0000000010.sci'},
-             ...
-        ],
-        'main': [
-            {'fileSize': '31568',
-             'name': 'BIOMD0000000010_url.xml'
-            }
-        ]
-    }
-    :param model_id: the model id (as int or string)
-    :return: json structure
+
+    .. code-block::
+
+        {
+            'additional': [
+                {'description': 'Auto-generated Scilab file',
+                 'fileSize': '3873',
+                 'name': 'BIOMD0000000010.sci'},
+                 ...
+            ],
+            'main': [
+                {'fileSize': '31568',
+                 'name': 'BIOMD0000000010_url.xml'
+                }
+            ]
+        }
+
+    Args:
+        model_id: either an integer, or a valid model id
+
+    Returns:
+        json structure
     """
     if type(model_id) is int:
         model_id = 'BIOMD{0:010d}'.format(model_id)
     result = download_json(END_POINT + 'model/files/' + model_id + '?format=json')
     return result
 
 
 def get_content_for_model(model_id, file_name=None):
     """Downloads the specified file from biomodels
-    :param model_id: the model id as int, or string
-    :param file_name: the filename to download (or None, to download the main file)
-    :return: the content of the specified file
+
+    Args:
+        model_id: either an integer, or a valid model id
+        file_name: the filename to download (or None, to download the main file)
+
+    Returns:
+        the content of the specified file
     """
     if type(model_id) is int:
         model_id = 'BIOMD{0:010d}'.format(model_id)
     if file_name is None:
         file_name = get_files_for_model(model_id)['main'][0]['name']
     return download_from(END_POINT + 'model/download/' + model_id + '?filename=' + urllib.parse.quote(file_name))
 
 
 def search_for_model(query, offset=0, num_results=10, sort='id-asc'):
     """Queries the biomodel database
-    Queries the database, for information about the query system see:
-    <https://www.ebi.ac.uk/biomodels-static/jummp-biomodels-help/model_search.html>
+    Queries the database, for information about the query system see: https://www.ebi.ac.uk/biomodels-static/jummp-biomodels-help/model_search.html
+
     Example:
         >>> search_for_model('glycolysis')
         [...,
             {
             'format': 'SBML',
             'id': 'BIOMD0000000206',
             'lastModified': '2012-07-04T23:00:00Z',
@@ -144,19 +167,23 @@
             'lastModified': '2012-02-02T00:00:00Z'',
             'name': 'Stewart2009_ActionPotential_PurkinjeFibreCells',
             'submissionDate': '2010-06-22T23:00:00Z',
             'submitter': 'Camille Laibe',
             'url': 'https://www.ebi.ac.uk/biomodels/MODEL1006230012'
             }
         ]
-    :param query: the query to use (it will be encoded with quote_plus before send out, so it is safe to use spaces)
-    :param offset: offset (defaults to 0)
-    :param num_results: number of results to obtain (defaults to 10)
-    :param sort: sort criteria to be used (defaults to id-asc)
-    :return: the search result as [{}]
+
+    Args:
+        query: the query to use (it will be encoded with quote_plus before send out, so it is safe to use spaces)
+        offset: offset (defaults to 0)
+        num_results: number of results to obtain (defaults to 10)
+        sort: sort criteria to be used (defaults to id-asc)
+
+    Returns:
+        the search result as [{}]
     """
     url = END_POINT + 'search?query=' + quote_plus(query)
     url += '&offset=' + str(offset)
     url += "&numResults=" + str(num_results)
     url += '&sort=' + sort
     result = download_json(url + '&format=json')
     return result['models']
```

### Comparing `sbmltoodejax-0.2/sbmltoodejax/modulegeneration.py` & `sbmltoodejax-0.3/sbmltoodejax/modulegeneration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 import jax.numpy as jnp
 from sbmltoodejax import jaxfuncs
 import re
 import sys
 
-def sec(x):
-    return jnp.reciprocal(jnp.cos(x))
-def csc(x):
-    return jnp.reciprocal(jnp.sin(x))
-def cot(x):
-    return jnp.reciprocal(jnp.tan(x))
-def sech(x):
-    return jnp.reciprocal(jnp.cosh(x))
-def csch(x):
-    return jnp.reciprocal(jnp.sinh(x))
-def coth(x):
-    return jnp.reciprocal(jnp.tanh(x))
-
 def GenerateModel(modelData, outputFilePath,
-                     RateofSpeciesChangeName: str ='RateofSpeciesChange',
-                     AssignmentRuleName: str='AssignmentRule',
-                     ModelStepName: str='ModelStep',
-                     ModelRolloutName: str='ModelRollout',
-                     deltaT: float =0.1,
-                     atol: float=1e-6,
-                     rtol: float = 1e-12,
-                     mxstep: int = 5000000,
-                     vmap_over_reactions: bool =False,
-                     ):
+                  RateofSpeciesChangeName: str ='RateofSpeciesChange',
+                  AssignmentRuleName: str='AssignmentRule',
+                  ModelStepName: str='ModelStep',
+                  ModelRolloutName: str='ModelRollout',
+                  deltaT: float =0.1,
+                  atol: float=1e-6,
+                  rtol: float = 1e-12,
+                  mxstep: int = 5000000
+                  ):
     """
-    This function takes model data, either from ParseSBMLFIle() or imported from a .json file,
-    and generates a Python file containing a class that implements the SBML model in Jax.
-    It is adapted from sbmltoodepy's GenerateModel function.
+    This function takes model data created by :func:`~sbmltoodejax.parse.ParseSBMLFile` and generates a python file containing
+    variables and modules that implement the SBML model.
+
+    Note:
+        This function is adapted from ``sbmltoodepy.modulegeneration.GenerateModel`` function, however the generated python file is
+        written in JAX and follows different conventions for the generated variables and modules, as detailed in :ref:`structure-of-the-generated-python-file`
+
+
+    Args:
+        modelData (sbmltoodepy.dataclasses.ModelData): An object containing all the model components and values.
+
+        outputFilePath (str): The desired file path of the resulting python file.
+
+        RateofSpeciesChangeName (str, optional): The name of the RateofSpeciesChange module defined in the resulting python file. Default to 'RateofSpeciesChange'.
+
+        AssignmentRuleName (str): The name of the AssignmentRule module defined in the resulting python file. Default to 'AssignmentRule'.
+
+        ModelStepName (str): The name of the ModelStep module defined in the resulting python file. Default to 'ModelStep'.
+
+        ModelRolloutName (str): The name of the ModelRollout module defined in the resulting python file. Default to'ModelRollout'.
+
+        deltaT (float): Time step size (in seconds). Default to 0.1.
+
+        atol (float): Absolute local error tolerance for ``jax.experimental.odeint`` solver. Default to 1e-6.
+
+        rtol (float): Relative local error tolerance for ``jax.experimental.odeint`` solver. Default to 1e-12.
+
+        mxstep (int): Maximum number of steps to take for each timepoint for ``jax.experimental.odeint`` solver. Default to 5000000.
+
 
-    In order to take advantage of jax main features the python class that simulates the model is written in functional paradigm style.
     """
 
     jnp.set_printoptions(threshold=sys.maxsize)
 
     outputFile = open(outputFilePath, "w")
 
     parameters = modelData.parameters
@@ -407,45 +418,24 @@
     outputFile.write('\t\trateOfSpeciesChange = self.stoichiometricMatrix @ reactionVelocities + rateRuleVector\n\n')
     outputFile.write('\t\treturn rateOfSpeciesChange\n\n')
 
     outputFile.write(f'\n\tdef calc_reaction_velocities(self, y, w, c, t):\n')
 
     reactionElements = ''
 
-    if vmap_over_reactions:
-        if reactions:
-            outputFile.write('\t\tcalc_reaction_velocities = vmap(lambda i, y, w, c, t: lax.switch(i, [')
-            for reactionId in reactions:
-                if reactionElements == '':
-                    reactionElements += ('self.' + str(reactionId))
-                else:
-                    reactionElements += (', self.' + str(reactionId))
-            outputFile.write(reactionElements + '], y, w, c, t), in_axes=0)\n\n')
-            outputFile.write(
-                f'\t\treactionVelocities = calc_reaction_velocities('
-                f'jnp.arange({len(reactions)}), '
-                f'jnp.tile(y, ({len(reactions)}, 1)), '
-                f'jnp.tile(t, ({len(reactions)}, 1)), '
-                f'jnp.tile(w, ({len(reactions)}, 1)))\n\n')
-
-        else:
-            outputFile.write(
-                '\t\treactionVelocities = jnp.array([0.0], dtype=jnp.float32)\n\n')
-
+    outputFile.write('\t\treactionVelocities = jnp.array([')
+    if reactions:
+        for reactionId in reactions:
+            if reactionElements == '':
+                reactionElements += ('self.' + str(reactionId) + '(y, w, c, t)')
+            else:
+                reactionElements += (', self.' + str(reactionId) + '(y, w, c, t)')
     else:
-        outputFile.write('\t\treactionVelocities = jnp.array([')
-        if reactions:
-            for reactionId in reactions:
-                if reactionElements == '':
-                    reactionElements += ('self.' + str(reactionId) + '(y, w, c, t)')
-                else:
-                    reactionElements += (', self.' + str(reactionId) + '(y, w, c, t)')
-        else:
-            reactionElements = '0'
-        outputFile.write(reactionElements + '], dtype=jnp.float32)\n\n')
+        reactionElements = '0'
+    outputFile.write(reactionElements + '], dtype=jnp.float32)\n\n')
 
     outputFile.write('\t\treturn reactionVelocities\n\n')
 
     for reaction_name in reactions.keys():
         outputFile.write(f'\n\tdef {reaction_name}(self, y, w, c, t):\n')
         rxnParamNames = [param[0] for param in reactions[reaction_name].rxnParameters]
         rateLaw = ParseRHS(reactions[reaction_name].rateLaw, extended_param_names=rxnParamNames, reaction_name=reaction_name, yvar="y", wvar="w", cvar="c")
```

### Comparing `sbmltoodejax-0.2/setup.py` & `sbmltoodejax-0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='sbmltoodejax',
-    version='0.2',
+    version='0.3',
     author='Mayalen Etcheverry',
     author_email='mayalen.etcheverry@inria.fr',
-    description='python software built upon jax, that allows to convert SBML models into python classes',
+    description='lightweight library that allows to automatically parse and convert SBML models into python models written end-to-end in JAX',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/flowersteam/autodiscjax',
+    url='https://github.com/flowersteam/sbmltoodejax',
     license='MIT',
     packages=['sbmltoodejax'],
     install_requires=['sbmltoodepy', 'jax[cpu]', 'equinox'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

