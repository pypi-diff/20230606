# Comparing `tmp/plotgen-0.7.8-py3-none-any.whl.zip` & `tmp/plotgen-0.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 36585 bytes, number of entries: 6
--rwxrwxr-x  2.0 unx   186712 b- defN 23-Feb-10 11:50 plotgen-0.7.8.data/scripts/plotgen
--rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-10 11:50 plotgen-0.7.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7014 b- defN 23-Feb-10 11:50 plotgen-0.7.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-10 11:50 plotgen-0.7.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-10 11:50 plotgen-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      478 b- defN 23-Feb-10 11:50 plotgen-0.7.8.dist-info/RECORD
-6 files, 195376 bytes uncompressed, 35721 bytes compressed:  81.7%
+Zip file size: 37511 bytes, number of entries: 6
+-rwxrwxr-x  2.0 unx   190232 b- defN 23-Feb-22 13:21 plotgen-0.7.9.data/scripts/plotgen
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-22 13:21 plotgen-0.7.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7014 b- defN 23-Feb-22 13:21 plotgen-0.7.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Feb-22 13:21 plotgen-0.7.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Feb-22 13:21 plotgen-0.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      478 b- defN 23-Feb-22 13:21 plotgen-0.7.9.dist-info/RECORD
+6 files, 198896 bytes uncompressed, 36647 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: plotgen-0.7.8.data/scripts/plotgen
+Filename: plotgen-0.7.9.data/scripts/plotgen
 Comment: 
 
-Filename: plotgen-0.7.8.dist-info/LICENSE
+Filename: plotgen-0.7.9.dist-info/LICENSE
 Comment: 
 
-Filename: plotgen-0.7.8.dist-info/METADATA
+Filename: plotgen-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: plotgen-0.7.8.dist-info/WHEEL
+Filename: plotgen-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: plotgen-0.7.8.dist-info/top_level.txt
+Filename: plotgen-0.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: plotgen-0.7.8.dist-info/RECORD
+Filename: plotgen-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `plotgen-0.7.8.data/scripts/plotgen` & `plotgen-0.7.9.data/scripts/plotgen`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,22 @@
 import textwrap
 import shutil
 import xopen
 import seaborn
 import plotly.figure_factory
 import scipy.cluster.hierarchy
 import scipy.spatial.distance
+import sklearn.cluster
 import multiprocessing
 
 # FUTURE: pyarrow
 # import csv.Sniffer
 
 __prog__ = 'plotgen'
-__version__ = '0.7.8'
+__version__ = '0.7.9'
 __url__ = 'https://github.com/bgottschall/plotgen'
 
 
 # All options that are forwared to the plotting script will be filtered through here
 def escapedStr(val: str):
     return val.translate(str.maketrans({
         "'": r"\'",
@@ -288,21 +289,42 @@
     return (0, 0)
   mean = numpy.average(values, weights=weights)
   variance = numpy.average((values - mean)**2, weights=weights)
   return (mean, numpy.sqrt(variance))
 
 class DataframeActions:
     functions = {
-        'pandasSelfFunctions': ['abs', 'cumsum', 'cummax', 'cummin', 'cumprod', 'rank', 'diff', 'round', 'floor', 'ceil'],
-        'specialSelfFunctions': ['set', 'cset', 'polyfit', 'append' , 'prepend', 'ljust', 'rjust', 'cjust'],
-        'amidComputeFunctions': ['add', 'sub', 'mul', 'div', 'truediv', 'floordiv', 'mod', 'pow', 'radd', 'rsub', 'rmul', 'rdiv', 'rtruediv', 'rfloordiv', 'rmod', 'rpow', 'lt', 'gt', 'le', 'ge', 'ne', 'eq', 'min', 'max'],
-        'onlyAmidComputeFunctions' : ['concat', 'copy'],
-        'soloComputeFunctions': ['sum', 'mean', 'median', 'std', 'var', 'count', 'skew', 'mad', 'min', 'max']
+      'pandasSelfFunctions': ['abs', 'cumsum', 'cummax', 'cummin', 'cumprod', 'rank', 'diff', 'round', 'floor', 'ceil'],
+      'specialSelfFunctions': ['set', 'cset', 'polyfit', 'append' , 'prepend', 'ljust', 'rjust', 'cjust', 'kmeans'],
+      'amidComputeFunctions': ['add', 'sub', 'mul', 'div', 'truediv', 'floordiv', 'mod', 'pow', 'radd', 'rsub', 'rmul', 'rdiv', 'rtruediv', 'rfloordiv', 'rmod', 'rpow', 'lt', 'gt', 'le', 'ge', 'ne', 'eq', 'min', 'max'],
+      'onlyAmidComputeFunctions' : ['concat', 'copy', 'kmeans_labels'],
+      'soloComputeFunctions': ['sum', 'mean', 'median', 'std', 'var', 'count', 'skew', 'mad', 'min', 'max'],
+      'specialGroupFunctions' : ['kmeans']
     }
 
+    def parseKMeansParameters(parameters: list):
+      res = { 'n_clusters' : 8, 'init': 'k-means++', 'n_init': 'auto', 'max_iter': 300, 'tol': 1e-4, 'algorithm': 'lloyd' , 'samples': 'yes'}
+      parameters = [str(p) for p in parameters]
+      if len(parameters) > 0:
+        if parameters[0].isnumeric():
+          res['n_clusters'] = parameters[0]
+          parameters = parameters[1:]
+        for p in parameters:
+          spl = p.split('=', 1)
+          if len(spl) != 2 or spl[0] not in res.keys():
+            raise Exception(f"Unknown KMeans parameter {p}, choose one of {', '.join(res.keys())}")
+          res[spl[0]] = spl[1]
+      for intk in ['n_clusters', 'max_iter']:
+        res[intk] = int(res[intk])
+      for floatk in ['tol']:
+        res[floatk] = float(res[floatk])
+      res['n_init'] = 'auto' if res['n_init'] == 'auto' else int(res['n_init'])
+      res['samples'] = True if res['samples'].lower() in ['yes', 'true', '1'] else False
+      return res
+
     floatTransformer = lambda x: float(x) if isFloat(x) else numpy.nan if str(x).lower() in considerAsNaN else x
 
     conditions = ['=', '!=', '<', '>', '<=', '>=', 'in', 'notin', 'xor', 'nor', 'and', 'nand']
 
     def filterFunction(frame, data, mode, quiet=False):
         filterMap = {
             '=': lambda x: any((pandas.isna(x) and pandas.isna(y)) or (float(x) == float(y) if isFloat([x, y]) else x == y) for y in data),
@@ -541,35 +563,39 @@
                     elif functionName == 'round':
                         decimals = 0 if len(functionParams) == 0 or not str(functionParams[0]).isdigit() else int(functionParams[0])
                         if len(functionParams) > 0 and not str(functionParams[0]).isdigit() and not quiet:
                             print('WARNING: round function parameter needs to be an integer', file=sys.stderr)
                         dataframe.iloc[:, applyColumnIds] = dataframe.iloc[:, applyColumnIds].round(decimals).values
                     else:
                         dataframe.iloc[:, applyColumnIds] = getattr(dataframe.iloc[:, applyColumnIds], functionName)(axis=0).values
+                elif functionName == 'kmeans':
+                  kmeanParams = DataframeActions.parseKMeansParameters(functionParams)
+                  kmeans = sklearn.cluster.KMeans(n_clusters=kmeanParams['n_clusters'], init=kmeanParams['init'], n_init=kmeanParams['n_init'], max_iter=kmeanParams['max_iter'], tol=kmeanParams['tol']).fit(dataframe.iloc[:, applyColumnIds].to_numpy())
+                  if kmeans.n_iter_ >= kmeanParams['max_iter'] and not quiet:
+                    print('WARNING: KMeans algorithm did not reach convergence. Adjust the tol and/or max_iter parameter!', file=sys.stderr)
+                  dataframe.iloc[:, applyColumnIds] = [kmeans.cluster_centers_[i] for i in kmeans.labels_]
                 elif functionName == 'append':
                     if len(functionParams) == 0:
-                        print('WARNING: no parameters given for function append, skipping', file=sys.stderr)
-                    else:
-                        dataframe.iloc[:, applyColumnIds] = (dataframe.iloc[:, applyColumnIds].astype(str) + ''.join([str(x) for x in functionParams])).apply(pandas.to_numeric, errors='ignore')
+                      raise Exception('ERROR: no parameters given for function append, skipping')
+                    dataframe.iloc[:, applyColumnIds] = (dataframe.iloc[:, applyColumnIds].astype(str) + ''.join([str(x) for x in functionParams])).apply(pandas.to_numeric, errors='ignore')
                 elif functionName == 'prepend':
                     if len(functionParams) == 0:
-                        print('WARNING: no parameters given for function prepend, skipping', file=sys.stderr)
-                    else:
-                        dataframe.iloc[:, applyColumnIds] = (''.join([str(x) for x in functionParams]) + dataframe.iloc[:, applyColumnIds].astype(str)).apply(pandas.to_numeric, errors='ignore')
+                      raise Exception('ERROR: no parameters given for function prepend, skipping')
+                    dataframe.iloc[:, applyColumnIds] = (''.join([str(x) for x in functionParams]) + dataframe.iloc[:, applyColumnIds].astype(str)).apply(pandas.to_numeric, errors='ignore')
                 elif functionName == 'set':
                     if len(functionParams) < 1:
-                        raise Exception('ERROR: function set requires a parameters')
+                      raise Exception('ERROR: function set requires a parameters')
                     dataframe.iloc[:, applyColumnIds] = functionParams[0]
                 elif functionName == 'cset':
                     if len(functionParams) < 3:
-                        raise Exception('ERROR: function conditional set requires 3 parameters')
+                      raise Exception('ERROR: function conditional set requires 3 parameters')
                     for columnId in applyColumnIds:
-                        mask = [i for (i, x) in enumerate(DataframeActions.filterFunction(dataframe.iloc[:, columnId], functionParams[1:-1], functionParams[0])) if x]
-                        if len(mask) > 0:
-                            dataframe.iloc[mask, columnId] = functionParams[-1]
+                      mask = [i for (i, x) in enumerate(DataframeActions.filterFunction(dataframe.iloc[:, columnId], functionParams[1:-1], functionParams[0])) if x]
+                      if len(mask) > 0:
+                        dataframe.iloc[mask, columnId] = functionParams[-1]
                 elif functionName in ['rjust', 'ljust', 'cjust']:
                     padWidth = functionParams[0] if len(functionParams) > 0  else None
                     padChar = str(functionParams[1]) if len(functionParams) > 1 else ' '
                     padFunc = functionName if functionName != 'cjust' else 'center'
                     dataframe.iloc[:, applyColumnIds] = dataframe.iloc[:, applyColumnIds].astype(str).apply(
                       lambda s: s.apply(lambda v: getattr(v, padFunc)(max(s.str.len()) if padWidth is None else padWidth, padChar))
                     )
@@ -644,60 +670,76 @@
         newCol.name = name
       return pandas.concat([dataframe, newCol], axis=1) if where == 'back' else pandas.concat([newCol, dataframe], axis=1)
 
     def groupNColumns(dataframe, n, function=['sum'], quiet=False):
       return DataframeActions.groupNRows(dataframe.T, n, quiet).T
 
     def groupNRows(dataframe, n, function=['sum'], quiet=False):
-      function = function[0]
+      functionName = function[0]
       treatIndexAsFloat = False
       indexName = dataframe.index.name
       index = None
+      if functionName == 'kmeans':
+        raise Exception('grouping n rows/columns is incompatible with the kmeans function')
       if all(isFloat(x) or x is numpy.nan for x in map(DataframeActions.floatTransformer, dataframe.index)):
         treatIndexAsFloat = True
         dataframe = DataframeActions.resetIndex(dataframe)
       else:
         print('WARNING: grouping n rows/columns with a non-numerical index will use a interpolated version', file=sys.stderr)
         index = dataframe.index
-      dataframe = getattr(dataframe.groupby(numpy.arange(len(dataframe.index)) // n, axis=0), function)()
+      dataframe = getattr(dataframe.groupby(numpy.arange(len(dataframe.index)) // n, axis=0), functionName)()
       if treatIndexAsFloat:
         dataframe = DataframeActions.dropColumnsByIds(DataframeActions.setIndexColumnByIdx(dataframe, 0), [0])
       else:
         dataframe.index = index[::n]
       dataframe.index.name = indexName
       return dataframe
 
     def groupAllColumns(dataframe, columnName, function=['sum']):
       return DataframeActions.groupAllRows(dataframe.T, columnName, function).T
 
     def groupAllRows(dataframe, rowName, function=['sum']):
       functionName = function[0]
+      if functionName == 'kmeans':
+        raise Exception('grouping to a single row/column is incompatible with the kmeans function')
       return getattr(dataframe.apply(pandas.to_numeric, errors='coerce').groupby(lambda _: rowName), functionName)()
 
-    def groupByRowIds(dataframe, rowIds, function=['sum']):
+    def groupByRowIds(dataframe, rowIds, function=['sum'], specialColumnPrefix='_'):
       rowIds = rowIds if isinstance(rowIds, list) else [rowIds]
       rowIds = ['index' if x == 'columns' else x for x in rowIds]
-      return DataframeActions.groupByColumnIds(dataframe.T, rowIds, function).T
+      return DataframeActions.groupByColumnIds(dataframe.T, rowIds, function, specialColumnPrefix).T
 
-    def groupByColumnIds(dataframe, columnIds, function=['sum']):
+    def groupByColumnIds(dataframe, columnIds, function=['sum'], specialColumnPrefix='_'):
         functionName = function[0]
+        functionParams = function[1:]
         if not isinstance(columnIds, list):
             columnIds = [columnIds]
         if 'index' in columnIds:
-            return getattr(dataframe.groupby(dataframe.index, axis=0), functionName)()
+          dataframe = DataframeActions.resetIndex(dataframe)
+          columnIds = [0] + [c + 1 for c in columnIds if c != 'index']
+
+        if functionName == 'kmeans':
+          kmeanParams = DataframeActions.parseKMeansParameters(functionParams)
+          kmeans = sklearn.cluster.KMeans(n_clusters=kmeanParams['n_clusters'], init=kmeanParams['init'], n_init=kmeanParams['n_init'], max_iter=kmeanParams['max_iter'], tol=kmeanParams['tol']).fit(dataframe.iloc[:, columnIds])
+          if kmeans.n_iter_ >= kmeanParams['max_iter'] and not quiet:
+            print('WARNING: KMeans algorithm did not reach convergence. Adjust the tol and/or max_iter parameter!', file=sys.stderr)
+          dataframe = pandas.DataFrame(kmeans.cluster_centers_, columns=kmeans.feature_names_in_)
+          if kmeanParams['samples']:
+            dataframe = pandas.concat([pandas.Series(numpy.unique(kmeans.labels_, return_counts=True)[1], name=specialColumnPrefix + 'samples'), dataframe], axis=1)
+          return DataframeActions.parseColumnIdsToString(dataframe, ['index'])
         else:
-            seen = set()
-            columnIds = [x for x in columnIds if x not in seen and not seen.add(x)]
-            newColumnLabels = [dataframe.columns[x] for x in columnIds] + [dataframe.columns[x] for x in range(dataframe.shape[1]) if x not in columnIds]
-            dataframe.columns = list(range(dataframe.shape[1]))
-            dataframe = getattr(dataframe.convert_dtypes().groupby(by=columnIds, as_index=False, sort=False), functionName)()
-            if len(dataframe.columns) != len(newColumnLabels):
-                raise Exception('Grouping dropped "nuisances" columns, and is considered not successful. This is probably due to incompatible data types in columns.')
-            dataframe.columns = newColumnLabels
-            return DataframeActions.parseColumnIdsToString(dataframe.set_index(dataframe.iloc[:, 0]).iloc[:, 1:], ['index'])
+          seen = set()
+          columnIds = [x for x in columnIds if x not in seen and not seen.add(x)]
+          newColumnLabels = [dataframe.columns[x] for x in columnIds] + [dataframe.columns[x] for x in range(dataframe.shape[1]) if x not in columnIds]
+          dataframe.columns = list(range(dataframe.shape[1]))
+          dataframe = getattr(dataframe.convert_dtypes().groupby(by=columnIds, as_index=False, sort=False), functionName)()
+          if len(dataframe.columns) != len(newColumnLabels):
+            raise Exception('Grouping dropped "nuisances" columns, and is considered not successful. This is probably due to incompatible data types in columns.')
+          dataframe.columns = newColumnLabels
+          return DataframeActions.parseColumnIdsToString(dataframe.set_index(dataframe.iloc[:, 0]).iloc[:, 1:], ['index'])
 
     def stackRowId(dataframe, rowId):
       if rowId == 'columns':
         l0Name = dataframe.index.name
         dataframe = dataframe.T.set_index(dataframe.T.iloc[:, 0], append=True).T
         dataframe = dataframe.iloc[1:, :].stack(0)
         dataframe = dataframe.to_frame() if not isinstance(dataframe, pandas.DataFrame) else dataframe
@@ -822,26 +864,26 @@
             print(f'Dataframes saved to {filename}')
         if (fFile != sys.stdout.buffer and fFile != sys.stdout.buffer):
             fFile.close()
 
 
 considerAsNaN = ['nan', 'none', 'null', 'zero', 'nodata', '']
 
-traceSpecialColumns = ['error', 'error-', 'error+', 'offset', 'label', 'colour']
+traceSpecialColumns = ['error', 'error-', 'error+', 'offset', 'label', 'colour', 'sizes']
 frameSpecialColumns = ['category']
 allSpecialColumns = traceSpecialColumns + frameSpecialColumns
 
 parser = argparse.ArgumentParser(description="Visualize your data the easy way")
 # Global Arguments
 
 parserFileOptions = parser.add_argument_group('file parsing options')
 
 inputFileArgument = parser.add_argument('-i', '--input', type=str, help="input file to parse", nargs="+", action=ParentAction, required=True)
 # Per File Parsing Arguments
-parserFileOptions.add_argument("--special-column-prefix", help="special columns (_label, _error, _offset, _colour) starting with (default %(default)s)", type=str, default='_', sticky_default=True, action=ChildAction, parent=inputFileArgument)
+parserFileOptions.add_argument("--special-column-prefix", help=f"special column prefix ({','.join(allSpecialColumns)}) starting with (default %(default)s)", type=str, default='_', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--comment", help="ignores lines starting with (default %(default)s)", type=str, default='#', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--delimiter", help="data delimiter (auto detected by default)", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--no-columns", help="do not use a column row", default=False, sticky_default=True, nargs=0, sub_action="store_true", action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--no-index", help="do not use a index column", default=False, sticky_default=True, nargs=0, sub_action="store_true", action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--threads", help="number of threads to decompress files", default=multiprocessing.cpu_count(), type=int, choices=Range(0, None), action=ChildAction, parent=inputFileArgument)
 
 
@@ -896,15 +938,15 @@
 parserFileOptions.add_argument("--normalise-to-row", help="normalise all rows to this row by name", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
 
 parserFileOptions.add_argument("--add-at", help="add rows or columns at the front or back of the frame", type=str, default='back', choices=['front', 'back'], action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--add-function", help=f"use this function to compute new row or column (default '{DataframeActions.functions['soloComputeFunctions'][0]}')", type=str, default=[DataframeActions.functions['soloComputeFunctions'][0]], nargs='+', action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--add-column", help="add a new column with name", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--add-row", help="add a new row with name", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
 
-parserFileOptions.add_argument("--group-function", help=f"use this function to group columns or rows (default '{DataframeActions.functions['soloComputeFunctions'][0]}')", type=str, default=[DataframeActions.functions['soloComputeFunctions'][0]], nargs='+', choices=DataframeActions.functions['soloComputeFunctions'], action=ChildAction, parent=inputFileArgument)
+parserFileOptions.add_argument("--group-function", help=f'function used to group columns or rows (default {DataframeActions.functions["soloComputeFunctions"][0]}), choose from {{{",".join(DataframeActions.functions["soloComputeFunctions"])}}} and for grouping by rows and columns also from {{{",".join(DataframeActions.functions["specialGroupFunctions"])}}}', type=str, default=[DataframeActions.functions['soloComputeFunctions'][0]], nargs='+', action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--group-by-icolumns", help="group by these column indexes (or slice, or frame index)", type=SliceType({'index': 'index', **defaultSliceTypeTranslator}), default=[], nargs='+', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--group-by-columns", help="group by these column names", type=str, default=[], nargs='+', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--group-by-irows", help="group by these row indexes (or slice, or frame columns)", type=SliceType({'columns': 'columns', **defaultSliceTypeTranslator}), default=[], nargs='+', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--group-by-rows", help="group by these row names", type=str, default=[], nargs='+', sticky_default=True, action=ChildAction, parent=inputFileArgument)
 
 parserFileOptions.add_argument("--group-to-column", help="group all columns into a single one", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
 parserFileOptions.add_argument("--group-to-row", help="group all rows into a single one", type=str, default=None, sticky_default=True, action=ChildAction, parent=inputFileArgument)
@@ -1649,33 +1691,25 @@
                     targetColumnIds = DataframeActions.sliceToColumnIds(frame, optionValue[1:]) if len(optionValue) > 1 else []
                     frame = DataframeActions.applyOnColumns(frame, applyColumnIds, targetColumnIds, applyFunction, applyMode)
                 elif optionName == 'apply_columns':
                     applyColumnIds = DataframeActions.getColumnIds(frame, optionValue[0])
                     targetColumnIds = DataframeActions.getColumnIds(frame, optionValue[1:]) if len(optionValue) > 1 else []
                     frame = DataframeActions.applyOnColumns(frame, applyColumnIds, targetColumnIds, applyFunction, applyMode)
                 elif optionName == 'group_by_irows':
-                    if 'columns' in optionValue:
-                      rowIds = [0] + [x + 1 for x in DataframeActions.sliceToRowIds(frame, [x for x in optionValue if x != 'columns'])]
-                      frame = DataframeActions.resetColumns(frame)
-                    else:
-                      rowIds = DataframeActions.sliceToRowIds(frame, optionValue)
-                    frame = DataframeActions.groupByRowIds(frame, rowIds, groupFunction)
+                    rowIds = DataframeActions.sliceToRowIds(frame, optionValue)
+                    frame = DataframeActions.groupByRowIds(frame, rowIds, groupFunction, options.special_column_prefix)
                 elif optionName == 'group_by_icolumns':
-                    if 'index' in optionValue:
-                      columnIds = [0] + [x + 1 for x in DataframeActions.sliceToColumnIds(frame, [x for x in optionValue if x != 'index'])]
-                      frame = DataframeActions.resetIndex(frame)
-                    else:
-                      columnIds = DataframeActions.sliceToColumnIds(frame, optionValue)
-                    frame = DataframeActions.groupByColumnIds(frame, columnIds, groupFunction)
+                    columnIds = DataframeActions.sliceToColumnIds(frame, optionValue)
+                    frame = DataframeActions.groupByColumnIds(frame, columnIds, groupFunction, options.special_column_prefix)
                 elif optionName == 'group_by_rows':
                     rowIds = DataframeActions.getRowIds(frame, optionValue, selectMode)
-                    frame = DataframeActions.groupByRowIds(frame, rowIds, groupFunction)
+                    frame = DataframeActions.groupByRowIds(frame, rowIds, groupFunction, options.special_column_prefix)
                 elif optionName == 'group_by_columns':
                     columnIds = DataframeActions.getColumnIds(frame, optionValue, selectMode)
-                    frame = DataframeActions.groupByColumnIds(frame, columnIds, groupFunction)
+                    frame = DataframeActions.groupByColumnIds(frame, columnIds, groupFunction, options.special_column_prefix)
                 elif optionName == 'group_to_column':
                   frame = DataframeActions.groupAllColumns(frame, optionValue, groupFunction)
                 elif optionName == 'group_to_row':
                     frame = DataframeActions.groupAllRows(frame, optionValue, groupFunction)
                 elif optionName == 'group_n_columns':
                   frame = DataframeActions.groupNColumns(frame, optionValue, groupFunction, args.quiet)
                 elif optionName == 'group_n_rows':
@@ -2153,14 +2187,15 @@
 
                 _errors_symmetric = True
                 _errors_pos = None
                 _errors_neg = None
                 _bases = None
                 _labels = None
                 _colours = None
+                _sizes = None
 
                 for nextColIndex in range(colIndex + 1, colIndex + 1 + len(options.traceSpecialColumns) if colIndex + 1 + len(options.traceSpecialColumns) <= len(frame.columns) else len(frame.columns)):
                   nextCol = str(frame.columns[nextColIndex])
                   if (nextCol not in options.traceSpecialColumns):
                     break
                   if (nextCol == options.special_column_prefix + 'error') and (_errors_pos is None):
                     _errors_pos = [x if (x is not None) else 0 for x in frame.iloc[:, nextColIndex].values.tolist()]
@@ -2170,14 +2205,16 @@
                   elif (nextCol == options.special_column_prefix + 'error-') and (_errors_neg is None):
                     _errors_symmetric = False
                     _errors_neg = [x if (x is not None) else 0 for x in frame.iloc[:, nextColIndex].values.tolist()]
                   elif (nextCol == options.special_column_prefix + 'offset') and (_bases is None):
                     _bases = [x if (x is not None) else 0 for x in frame.iloc[:, nextColIndex].values.tolist()]
                   elif (nextCol == options.special_column_prefix + 'label') and (_labels is None):
                     _labels = frame.iloc[:, nextColIndex].values.tolist()
+                  elif (nextCol == options.special_column_prefix + 'sizes') and (_sizes is None):
+                    _sizes = frame.iloc[:, nextColIndex].values.tolist()
                   elif (nextCol == options.special_column_prefix + 'colour') and (_colours is None) and (frameTraceIndex >= len(options.trace_colours)):
                     _colours = frame.iloc[:, nextColIndex].values.tolist()
                     _colours = [c if c is not None else fillcolour for c in _colours]
 
                 traceName = col
                 if (inputTraceIndex < len(options.trace_names)):
                     traceName = options.trace_names[inputTraceIndex]
@@ -2308,15 +2345,15 @@
                         plotScript.write(f"""
 {commentColour}    marker_color='{fillcolour}',""")
                     plotScript.write(f"""
 {commentColour}    line_color='{fillcolour}',
 {commentColour}    fillcolor='{fillcolour}', # Currently not supported through script, using default
     stackgroup='{'stackgroup-' + str(inputIndex) if options.line_stack else ''}',
     marker_symbol='{lineMarker}',
-    marker_size={options.line_marker_size},
+    marker_size={options.line_marker_size if _sizes is None else _sizes},
     fill='{options.line_fill}',
     line_dash='{options.line_dash}',
     line_shape='{options.line_shape}',
     line_width={options.line_width},
     y={ydata},
     x={xdata},""")
                     if (_labels is not None):
@@ -2662,14 +2699,16 @@
 plotScript.write(f"{'# ' if args.legend_y_anchor is None else ''}fig.update_layout(legend_yanchor='{'auto' if args.legend_y_anchor is None else args.legend_y_anchor}')\n")
 plotScript.write(f"{'# ' if args.legend_x_anchor is None else ''}fig.update_layout(legend_xanchor='{'auto' if args.legend_x_anchor is None else args.legend_x_anchor}')\n")
 plotScript.write(f"fig.update_layout(legend=dict(x={args.legend_x}, y={args.legend_y}, orientation='{'v' if args.legend_vertical else 'h'}', bgcolor='rgba(255,255,255,0)'))\n")
 
 plotScript.write("\n# Layout Plot and Background\n")
 plotScript.write(f"{commentBackgroundColour}fig.update_layout(paper_bgcolor='{args.background_colour}', plot_bgcolor='{args.background_colour}')\n")
 
+# If no explicit margin is set, the brwoser will recieve a top margin for the plotly option bar to not overlap
+browserTopMargin = args.margin_t if args.margin_t is not None else args.margins if args.margins is not None else 20
 args.margin_b = args.margin_b if args.margin_b is not None else args.margins if args.margins is not None else None if defaultBottomMargin else 0
 args.margin_l = args.margin_l if args.margin_l is not None else args.margins if args.margins is not None else None if defaultLeftMargin else 0
 args.margin_r = args.margin_r if args.margin_r is not None else args.margins if args.margins is not None else None if defaultRightMargin else 0
 args.margin_t = args.margin_t if args.margin_t is not None else args.margins if args.margins is not None else None if defaultTopMargin else 0
 args.margin_pad = args.margin_pad if args.margin_pad is not None else args.margins if args.margins is not None else None if defaultPadMargin else 0
 
 plotScript.write(f"fig.update_layout(margin=dict(t={args.margin_t}, l={args.margin_l}, r={args.margin_r}, b={args.margin_b}, pad={args.margin_pad}))\n")
@@ -2688,20 +2727,14 @@
   if args.addon_files is not None:
     for addonFile in args.addon_files:
       if os.path.exists(addonFile):
         exec(open(addonFile).read())
   elif os.path.exists(os.path.join(filepath,f'{filename}_addon{fileext}')):
         exec(open(os.path.join(filepath,f'{filename}_addon{fileext}')).read())
 
-""")
-
-plotScript.write("""
-
-if args.browser:
-    fig.show()
 if len(args.output) > 0:
     for output in args.output:
         outputFormat = output.lower().split('.')[-1]
         if outputFormat == 'html':
             fig.write_html(output)
         else:
             fig.write_image(output, width=args.width, height=args.height)
@@ -2712,14 +2745,24 @@
                 if sys.platform == "win32":
                     os.startfile(output)
                 else:
                     opener = "open" if sys.platform == "darwin" else "xdg-open"
                     subprocess.call([opener, output], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
             except Exception:
                 print(f'Could not open {output}!')
+
+if args.browser:
+    """)
+if browserTopMargin != args.margin_t:
+  plotScript.write(f"fig.update_layout(margin_t={browserTopMargin})")
+plotScript.write("""
+    fig.show(config={
+       'toImageButtonOptions': { 'height': None, 'width': None, 'format': 'svg' },
+       'displaylogo': False, 'modeBarButtonsToAdd': ['drawline', 'drawopenpath', 'drawclosedpath', 'drawcircle', 'drawrect', 'eraseshape'],
+    })
 """)
 
 plotScript.close()
 if args.browser or len(args.output) > 0:
     cmdLine = ['python3', plotScriptName]
     if args.browser:
         cmdLine.append('--browser')
```

## Comparing `plotgen-0.7.8.dist-info/LICENSE` & `plotgen-0.7.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plotgen-0.7.8.dist-info/METADATA` & `plotgen-0.7.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotgen
-Version: 0.7.8
+Version: 0.7.9
 Summary: A plotly plotting script generator and data parser
 Home-page: https://github.com/bgottschall/plotgen
 Author: Björn Gottschall
 Author-email: info@bgottschall.de
 License: MIT
 Keywords: tables graph plot parser plotly
 Classifier: Programming Language :: Python :: 3
```

