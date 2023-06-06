# Comparing `tmp/cmsis_stream-1.2.3-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 74872 bytes, number of entries: 66
+Zip file size: 76157 bytes, number of entries: 67
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -23,46 +23,47 @@
 -rw-rw-rw-  2.0 fat     2029 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSink.py
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
--rw-rw-rw-  2.0 fat     6615 b- defN 23-Jun-02 08:15 cmsis_stream/cg/scheduler/config.py
--rw-rw-rw-  2.0 fat    41560 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/description.py
+-rw-rw-rw-  2.0 fat     6665 b- defN 23-Jun-06 08:34 cmsis_stream/cg/scheduler/config.py
+-rw-rw-rw-  2.0 fat    41606 b- defN 23-Jun-05 08:22 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat     1784 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    29225 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat    36807 b- defN 23-Jun-06 05:54 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
--rw-rw-rw-  2.0 fat     8260 b- defN 23-Jun-01 13:08 cmsis_stream/cg/scheduler/standard.py
--rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt
--rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 09:40 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/Makefile.linux
--rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/Makefile.mac
--rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/templates/Makefile.windows
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 09:40 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-05 09:45 cmsis_stream/cg/scheduler/standard.py
+-rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
+-rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
+-rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
+-rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/example/main_board.c
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/example/run.bat
+-rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple.cproject.yml
+-rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
+-rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
+-rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
+-rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
+-rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/vht.clayer.yml
+-rw-rw-rw-  2.0 fat    16526 b- defN 23-Jun-06 08:40 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-06 08:40 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      431 b- defN 23-Jun-01 13:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-02 07:46 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      674 b- defN 23-Jun-01 13:13 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat      297 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
 -rw-rw-rw-  2.0 fat     1111 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
 -rw-rw-rw-  2.0 fat     3185 b- defN 23-Jun-01 11:18 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
 -rw-rw-rw-  2.0 fat     4482 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1051 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     4848 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/dot_template.dot
--rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/templates/main_board.c
--rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/templates/run.bat
--rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/simple.cproject.yml
--rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml
--rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/templates/start_project_appnodes.h
--rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/templates/start_project_custom.h
--rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/templates/start_project_graph.py
--rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/templates/start_project_main.c
--rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/vht.clayer.yml
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3275 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6384 b- defN 23-Jun-02 09:40 cmsis_stream-1.2.3.dist-info/RECORD
-66 files, 210874 bytes uncompressed, 64428 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3506 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6457 b- defN 23-Jun-06 08:40 cmsis_stream-1.3.0.dist-info/RECORD
+67 files, 221209 bytes uncompressed, 65603 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -96,104 +96,107 @@
 
 Filename: cmsis_stream/cg/scheduler/pythoncode.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/standard.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt
+Filename: cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/GenericNodes.h
+Filename: cmsis_stream/cg/scheduler/example/Makefile.linux
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/Makefile.linux
+Filename: cmsis_stream/cg/scheduler/example/Makefile.mac
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/Makefile.mac
+Filename: cmsis_stream/cg/scheduler/example/Makefile.windows
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/Makefile.windows
+Filename: cmsis_stream/cg/scheduler/example/README.md
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cg_status.h
+Filename: cmsis_stream/cg/scheduler/example/main_board.c
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cmsis.cpp
+Filename: cmsis_stream/cg/scheduler/example/run.bat
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cmsis.py
+Filename: cmsis_stream/cg/scheduler/example/simple.cproject.yml
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
+Filename: cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
+Filename: cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/code.cpp
+Filename: cmsis_stream/cg/scheduler/example/start_project_custom.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/code.h
+Filename: cmsis_stream/cg/scheduler/example/start_project_graph.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/code.py
+Filename: cmsis_stream/cg/scheduler/example/start_project_main.c
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
+Filename: cmsis_stream/cg/scheduler/example/vht.clayer.yml
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/commonc.cpp
+Filename: cmsis_stream/cg/scheduler/templates/GenericNodes.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
+Filename: cmsis_stream/cg/scheduler/templates/cg_status.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
+Filename: cmsis_stream/cg/scheduler/templates/cmsis.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/main_board.c
+Filename: cmsis_stream/cg/scheduler/templates/cmsis.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/run.bat
+Filename: cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/simple.cproject.yml
+Filename: cmsis_stream/cg/scheduler/templates/code.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml
+Filename: cmsis_stream/cg/scheduler/templates/code.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/start_project_appnodes.h
+Filename: cmsis_stream/cg/scheduler/templates/code.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/start_project_custom.h
+Filename: cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/start_project_graph.py
+Filename: cmsis_stream/cg/scheduler/templates/commonc.cpp
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/start_project_main.c
+Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/vht.clayer.yml
+Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/METADATA
+Filename: cmsis_stream-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/WHEEL
+Filename: cmsis_stream-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/entry_points.txt
+Filename: cmsis_stream-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/top_level.txt
+Filename: cmsis_stream-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.3.dist-info/RECORD
+Filename: cmsis_stream-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/config.py

```diff
@@ -175,15 +175,15 @@
     ctemplate = env.get_template("cg_status.h")
     path=os.path.join(folder,"cg_status.h")
     with open(path,"w") as f:
         print(ctemplate.render(),file=f)
 
 def createEmptyProject(project_name):
     env = Environment(
-       loader=PackageLoader("cmsis_stream.cg.scheduler"),
+       loader=PackageLoader("cmsis_stream.cg.scheduler","example"),
        autoescape=select_autoescape(),
        trim_blocks=True
     )
     try:
         os.mkdir(project_name)
     except Exception as e:
         pass
@@ -192,18 +192,19 @@
               ,"start_project_custom.h":"custom.h"
               ,"start_project_main.c":"main_host.c"
               ,"start_project_graph.py":"graph.py"
               ,"Makefile.linux":"Makefile.linux"
               ,"Makefile.mac":"Makefile.mac"
               ,"Makefile.windows":"Makefile.windows"
               ,"main_board.c":"main.c"
-              ,"simple.csolution_ac6.yml":"simple.csolution_ac6.yml"
+              ,"simple_ac6.csolution.yml":"simple_ac6.csolution.yml"
               ,"simple.cproject.yml":"simple.cproject.yml"
               ,"vht.clayer.yml":"vht.clayer.yml"
               ,"run.bat":"run_vht.bat"
-              ,"ARMCM55_FP_MVE_config.txt":"ARMCM55_FP_MVE_config.txt"};
+              ,"ARMCM55_FP_MVE_config.txt":"ARMCM55_FP_MVE_config.txt"
+              ,"README.md":"README.md"};
     for src_name in all_files:
         dst_name = all_files[src_name]
         ctemplate = env.get_template(src_name)
         path = os.path.join(project_name,dst_name)
         with open(path,"w") as f:
             print(ctemplate.render(),file=f)
```

## cmsis_stream/cg/scheduler/description.py

```diff
@@ -34,15 +34,15 @@
 
 from .graphviz import gengraph
 from .ccode import gencode as c_gencode
 from .pythoncode import gencode as p_gencode
 
 from .node import *
 from .config import *
-from .standard import Duplicate,ioName
+from .standard import Duplicate
 
 from ..types import *
 
 # To debug graph coloring for memory optimization
 #import matplotlib.pyplot as plt
 
 class IncompatibleIO(Exception):
@@ -344,15 +344,16 @@
                     # connection dup -> b
                     # And we create a new connection a -> dup
 
                     self.connect(output,dup.i,dupAllowed=False)
 
                     
                     for i in range(len(destinations)):
-                       self.connectDup(destinations,dup[ioName(i)],i)
+                       name = dup.outputNameFromIndex(i)
+                       self.connectDup(destinations,dup[name],i)
                         
 
                
 
     def connect(self,nodea,nodeb,dupAllowed=True,fifoClass=None,fifoScale = 1.0):
         if fifoClass is None:
             fifoClass = self.defaultFIFOClass
```

## cmsis_stream/cg/scheduler/node.py

```diff
@@ -433,44 +433,42 @@
                outputid = outputid + 1
                
 
         self._realInputs = inputid
         self._realOutputs = outputid
         
 
-    def ioTemplate(self):
-        """Template arguments for C
-           input type, input size ...
-           output type, output size ...
-
-           Some nodes may customize it
-        """
+    def getCTemplateArgumentsFor(self,orderedNames,ioDesc):
         ios=[] 
         # Use ordered io names
-        for io in self.inputNames:
-            x = self._inputs[io]
+        for io in orderedNames:
+            # Get IO description for this name
+            x = ioDesc[io]
             # For cyclo static scheduling, we may have a list
             # of samples
             if isinstance(x.nbSamples,int):
                ios.append("%s,%d" % (x.ctype,x.nbSamples))
             else:
                 # In case of a list of samples
                 # thne templaet is receiving only the
                 # max value
                 m = np.max(x.nbSamples)
                 ios.append("%s,%d" % (x.ctype,m))
+        return(ios)
 
-        for io in self.outputNames:
-            x = self._outputs[io]
-            if isinstance(x.nbSamples,int):
-               ios.append("%s,%d" % (x.ctype,x.nbSamples))
-            else:
-                m = np.max(x.nbSamples)
-                ios.append("%s,%d" % (x.ctype,m))
+    def ioTemplate(self):
+        """Template arguments for C
+           input type, input size ...
+           output type, output size ...
 
+           Some nodes may customize it
+        """
+        ios=[] 
+        ios += self.getCTemplateArgumentsFor(self.inputNames,self._inputs)
+        ios += self.getCTemplateArgumentsFor(self.outputNames,self._outputs)
         
         return("".join(joinit(ios,",")))
 
     def pythonIoTemplate(self):
         """Template arguments for Python
            input type, input size ...
            output type, output size ...
@@ -545,14 +543,16 @@
         # scheduler when we create on the fly a new class
         # for a function.
         # In this case, the arguments of the template must only be
         # fifos and not constant.
         templateargs=[]
         for x in fifoIDs:
           # If args is a FIFO we generate a name using fifo ids
+          # They have already been ordered (in calling function)
+          # using alphabetical order of input and output names
           if isinstance(x,int):
              if config.heapAllocation:
                 fifoArg = FifoPtrID(x,owner="fifos")
              else:
                 fifoArg = FifoID(x)
              res.append(fifoArg)
              templateargs.append(fifoArg)
@@ -664,14 +664,231 @@
 
     def addInput(self,name,theType,theLength):
         self._inputs[name]=Input(self,name,theType,theLength)
 
     def addOutput(self,name,theType,theLength):
         self._outputs[name]=Output(self,name,theType,theLength)
 
+class GenericToManyNode(BaseNode):
+    """A source in the dataflow graph""" 
+
+    def __init__(self,name):
+        BaseNode.__init__(self,name)
+        # Pure node is for instance a 
+        # CMSIS-DSP function.
+        # It is not packaged into an object
+        # and the code is generated directly
+        self._isPureNode = False
+    
+    @property
+    def isPureNode(self):
+        return self._isPureNode
+    
+    @property
+    def typeName(self):
+        return "void"
+
+    # Should be in alphabetical order so that the
+    # index used here is the index in the C code
+    def outputNameFromIndex(self,i):
+        return f"o{chr(ord('a')+i)}"
+
+    def addInput(self,name,theType,theLength):
+        self._inputs[name]=Input(self,name,theType,theLength)
+
+    def addManyOutput(self,theType,theLength,nb):
+        self._outputLength = theLength
+        self._outputType = theType
+        for i in range(nb):
+            name = self.outputNameFromIndex(i)
+            self._outputs[name]=Output(self,name,theType,theLength)
+
+    @property
+    def args(self):
+        """String of fifo args for object initialization
+            with literal argument and variable arguments"""
+        allArgs=self.listOfargs
+        theInputs = allArgs[:len(self._inputs)]
+        theOutputs = allArgs[len(self._inputs):]
+        
+        ioInputs = [x.reference for x in theInputs]
+        ioOutputs = ["{" + "".join(joinit([x.pointer for x in theOutputs],",")) + "}"]
+        # Add specific argrs after FIFOs
+        sched = []
+        if self.schedArgs:
+            for lit in self.schedArgs:
+                sched.append(lit.arg)
+        return "".join(joinit(ioInputs+ioOutputs+sched,","))
+
+    def ioTemplate(self):
+        """ioTemplate is different for window
+        """
+        ios=[] 
+        ios += self.getCTemplateArgumentsFor(self.inputNames,self._inputs)
+       
+        # Use the max in case of cyclo static
+        # scheduling on the output
+        if isinstance(self._outputLength,int):
+            nbOut = self._outputLength 
+        else:
+            nbOut = np.max(self._outputLength )
+        ios.append("%s,%d" % (self._outputType.ctype,nbOut))
+        return("".join(joinit(ios,",")))
+
+
+class GenericFromManyNode(BaseNode):
+    """A source in the dataflow graph""" 
+
+    def __init__(self,name):
+        BaseNode.__init__(self,name)
+        # Pure node is for instance a 
+        # CMSIS-DSP function.
+        # It is not packaged into an object
+        # and the code is generated directly
+        self._isPureNode = False
+    
+    @property
+    def isPureNode(self):
+        return self._isPureNode
+    
+    @property
+    def typeName(self):
+        return "void"
+
+    # Should be in alphabetical order so that the
+    # index used here is the index in the C code
+    def inputNameFromIndex(self,i):
+        return f"i{chr(ord('a')+i)}"
+
+    def addOutput(self,name,theType,theLength):
+        self._outputs[name]=Output(self,name,theType,theLength)
+
+    def addManyInput(self,theType,theLength,nb):
+        self._inputLength = theLength
+        self._inputType = theType
+        for i in range(nb):
+            name = self.inputNameFromIndex(i)
+            self._inputs[name]=Input(self,name,theType,theLength)
+
+    @property
+    def args(self):
+        """String of fifo args for object initialization
+            with literal argument and variable arguments"""
+        allArgs=self.listOfargs
+        theInputs = allArgs[:len(self._inputs)]
+        theOutputs = allArgs[len(self._inputs):]
+        
+        ioInputs = ["{" + "".join(joinit([x.pointer for x in theInputs],",")) + "}"]
+        ioOutputs = [x.reference for x in theOutputs]
+        # Add specific argrs after FIFOs
+        sched = []
+        if self.schedArgs:
+            for lit in self.schedArgs:
+                sched.append(lit.arg)
+        return "".join(joinit(ioInputs+ioOutputs+sched,","))
+
+    def ioTemplate(self):
+        """ioTemplate is different for window
+        """
+        ios=[] 
+       
+        # Use the max in case of cyclo static
+        # scheduling on the output
+        if isinstance(self._inputLength,int):
+            nbOut = self._inputLength 
+        else:
+            nbOut = np.max(self._inputLength )
+        ios.append("%s,%d" % (self._inputType.ctype,nbOut))
+        
+        ios += self.getCTemplateArgumentsFor(self.outputNames,self._outputs)
+
+
+        return("".join(joinit(ios,",")))
+
+class GenericManyToManyNode(BaseNode):
+    """A source in the dataflow graph""" 
+
+    def __init__(self,name):
+        BaseNode.__init__(self,name)
+        # Pure node is for instance a 
+        # CMSIS-DSP function.
+        # It is not packaged into an object
+        # and the code is generated directly
+        self._isPureNode = False
+    
+    @property
+    def isPureNode(self):
+        return self._isPureNode
+    
+    @property
+    def typeName(self):
+        return "void"
+
+    # Should be in alphabetical order so that the
+    # index used here is the index in the C code
+    def inputNameFromIndex(self,i):
+        return f"i{chr(ord('a')+i)}"
+
+    def outputNameFromIndex(self,i):
+        return f"o{chr(ord('a')+i)}"
+
+    def addManyOutput(self,theType,theLength,nb):
+        self._outputLength = theLength
+        self._outputType = theType
+        for i in range(nb):
+            name = self.outputNameFromIndex(i)
+            self._outputs[name]=Output(self,name,theType,theLength)
+
+    def addManyInput(self,theType,theLength,nb):
+        self._inputLength = theLength
+        self._inputType = theType
+        for i in range(nb):
+            name = self.inputNameFromIndex(i)
+            self._inputs[name]=Input(self,name,theType,theLength)
+
+    @property
+    def args(self):
+        """String of fifo args for object initialization
+            with literal argument and variable arguments"""
+        allArgs=self.listOfargs
+        theInputs = allArgs[:len(self._inputs)]
+        theOutputs = allArgs[len(self._inputs):]
+        
+        ioInputs = ["{" + "".join(joinit([x.pointer for x in theInputs],",")) + "}"]
+        ioOutputs = ["{" + "".join(joinit([x.pointer for x in theOutputs],",")) + "}"]
+        # Add specific argrs after FIFOs
+        sched = []
+        if self.schedArgs:
+            for lit in self.schedArgs:
+                sched.append(lit.arg)
+        return "".join(joinit(ioInputs+ioOutputs+sched,","))
+
+    def ioTemplate(self):
+        """ioTemplate is different for window
+        """
+        ios=[] 
+       
+        # Use the max in case of cyclo static
+        # scheduling on the output
+        if isinstance(self._inputLength,int):
+            nbOut = self._inputLength 
+        else:
+            nbOut = np.max(self._inputLength )
+        ios.append("%s,%d" % (self._inputType.ctype,nbOut))
+        
+
+        if isinstance(self._outputLength,int):
+            nbOut = self._outputLength 
+        else:
+            nbOut = np.max(self._outputLength )
+        ios.append("%s,%d" % (self._outputType.ctype,nbOut))
+        
+
+        return("".join(joinit(ios,",")))
+       
 class SlidingBuffer(GenericNode):
 
     def __init__(self,name,theType,length,overlap):
         GenericNode.__init__(self,name)
         self._length = length 
         self._overlap = overlap 
         self.addInput("i",theType,length-overlap)
@@ -953,57 +1170,57 @@
             outputs=params["outputs"],
             node=self
             )
        return(result)
 
     
 class Unary(GenericFunction):
-    def __init__(self,funcname,theType,length):
+    def __init__(self,funcname,theType,length,input_name="i",output_name="o"):
         GenericFunction.__init__(self,funcname,theType,length)
 
-        self.addInput("i",theType,length)
-        self.addOutput("o",theType,length)
+        self.addInput(input_name,theType,length)
+        self.addOutput(output_name,theType,length)
 
 
 class Binary(GenericFunction):
-    def __init__(self,funcname,theType,length):
+    def __init__(self,funcname,theType,length,input_names=["ia","ib"],output_name="o"):
         GenericFunction.__init__(self,funcname,theType,length)
 
-        self.addInput("ia",theType,length)
-        self.addInput("ib",theType,length)
+        self.addInput(input_names[0],theType,length)
+        self.addInput(input_names[1],theType,length)
         
-        self.addOutput("o",theType,length)
+        self.addOutput(output_name,theType,length)
 
 
     
 
 
 BINARYOP=["scale","add","and","mult","not","or","sub","xor","cmplx_mult_cmplx","cmplx_mult_real"
 ]
 
 class Dsp(GenericFunction):
 
-    def __init__(self,name,theType,length):
+    def __init__(self,name,theType,length,input_name="i",input_names=["ia","ib"],output_name="o"):
         # Some different graph functions correspond to the same
         # DSP function like IFFT
         # So we rename the cmsis function to call the same function
         
         cmsisname = "arm_%s_%s" % (name,theType.dspExtension)
         GenericFunction.__init__(self, cmsisname,theType,length)
         self._binary=True
         
         if name in BINARYOP:
-            self.addInput("ia",theType,length)
-            self.addInput("ib",theType,length)
+            self.addInput(input_names[0],theType,length)
+            self.addInput(input_names[1],theType,length)
             self._binary=True
         else:
-           self.addInput("i",theType,length)
+           self.addInput(input_name,theType,length)
            self._binary=False
         
-        self.addOutput("o",theType,length)
+        self.addOutput(output_name,theType,length)
 
     
 
     @property
     def typeName(self):
         return "CMSIS-DSP"
```

## cmsis_stream/cg/scheduler/standard.py

```diff
@@ -22,15 +22,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ############################################
 """Standard nodes available to describe a network in addition to the generic nodes"""
 
 from ..types import *
-from .node import GenericNode,GenericSource,GenericSink, joinit
+from .node import GenericNode,GenericToManyNode,GenericSource,GenericSink, joinit
 
 floatType=CType(F32)
 
 class Unzip(GenericNode):
 
     def __init__(self,name,theType,length):
         GenericNode.__init__(self,name)
@@ -143,61 +143,41 @@
         return [0]
     digits = []
     while n:
         digits.append(int(n % b))
         n //= b
     return digits[::-1]
 
-def ioName(nb):
-    return("".join([chr(x+ord('A')) for x in numberToBase(nb,26)]).rjust(6,"A"))
 
 
 # Duplicate node is working with a list of output nodes
 # in the C generated code so that we don't have to provide
 # different templates for different number of outputs.
 # As consequence, the formatting of the arguments in the
 # generated code must be modified.
 # The template only use one arguments covering all the list
 # And finally the arguments naming is following alphabetical
 # order
-class Duplicate(GenericNode):
+class Duplicate(GenericToManyNode):
     def __init__(self,name,theType,inLength,nb,className="Duplicate"):
-        GenericNode.__init__(self,name)
+        GenericToManyNode.__init__(self,name)
 
         self._className = className
-        self._length = inLength
 
         self.addInput("i",theType,inLength)
-        for i in range(nb):
-            self.addOutput(ioName(i),theType,inLength)
+        self.addManyOutput(theType,inLength,nb)
+
+    # Naming of output from index
+    # They are in alphabetical order
+    # so that the index used here is also the
+    # index in the C code
+    def outputNameFromIndex(self,nb):
+        r="".join([chr(x+ord('a')) for x in numberToBase(nb,26)]).rjust(6,"a")
+        return(r)
 
-    @property
-    def args(self):
-        """String of fifo args for object initialization
-            with literal argument and variable arguments"""
-        allArgs=self.listOfargs
-        theInput = allArgs[0]
-        nb = len(allArgs) - 1
-        others = ",{" + "".join(joinit([x.pointer for x in allArgs[1:]],",")) + "}"
-        # Add specific argrs after FIFOs
-        sched = []
-        if self.schedArgs:
-            for lit in self.schedArgs:
-                sched.append(lit.arg)
-        if sched:
-            return (theInput.reference + others + "," + "".join(joinit(sched,",")))
-        else:
-           return (theInput.reference + others)
-
-    def ioTemplate(self):
-        """ioTemplate is different for window
-        """
-        theType=self._inputs[self.inputNames[0]].ctype  
-        ios="%s,%d" % (theType,self._length)
-        return(ios)
 
     @property 
     def isDuplicateNode(self):
         return True
 
     @property
     def typeName(self):
```

## cmsis_stream/cg/scheduler/templates/GenericNodes.h

```diff
@@ -293,41 +293,112 @@
 template<typename IN, int inputSize,typename OUT, int outputSize>
 class GenericNode:public NodeBase
 {
 public:
      GenericNode(FIFOBase<IN> &src,FIFOBase<OUT> &dst):mSrc(src),mDst(dst){};
 
 protected:
-     OUT * getWriteBuffer(int nb = outputSize){return mDst.getWriteBuffer(nb);};
-     IN * getReadBuffer(int nb = inputSize){return mSrc.getReadBuffer(nb);};
+     OUT * getWriteBuffer(int nb = outputSize) {return mDst.getWriteBuffer(nb);};
+     IN * getReadBuffer(int nb = inputSize) {return mSrc.getReadBuffer(nb);};
 
-     bool willOverflow(int nb = outputSize){return mDst.willOverflowWith(nb);};
-     bool willUnderflow(int nb = inputSize){return mSrc.willUnderflowWith(nb);};
+     bool willOverflow(int nb = outputSize) const {return mDst.willOverflowWith(nb);};
+     bool willUnderflow(int nb = inputSize) const {return mSrc.willUnderflowWith(nb);};
 
 private:
     FIFOBase<IN> &mSrc;
     FIFOBase<OUT> &mDst;
 };
 
+template<typename IN, int inputSize,
+         typename OUT, int outputSize>
+class GenericToManyNode:public NodeBase
+{
+public:
+     GenericToManyNode(FIFOBase<IN> &src,
+                       std::initializer_list<FIFOBase<OUT>*> dst):mSrc(src),mDstList(dst){};
+
+
+protected:
+     size_t getNbOutputs() const {return(mDstList.size());};
+
+     IN * getReadBuffer(int nb = inputSize) {return mSrc.getReadBuffer(nb);};
+     OUT * getWriteBuffer(int id=0,int nb = outputSize) {return mDstList[id]->getWriteBuffer(nb);};
+
+     bool willUnderflow(int nb = inputSize) const {return mSrc.willUnderflowWith(nb);};
+     bool willOverflow(int id=0,int nb = outputSize) const {return mDstList[id]->willOverflowWith(nb);};
+
+private:
+    FIFOBase<IN> &mSrc;
+    const std::vector<FIFOBase<OUT>*> mDstList;
+};
+
+template<typename IN, int inputSize,
+         typename OUT, int outputSize>
+class GenericFromManyNode:public NodeBase
+{
+public:
+     GenericFromManyNode(std::initializer_list<FIFOBase<IN>*> src,
+                         FIFOBase<OUT> &dst):mSrcList(src),mDst(dst){};
+
+
+protected:
+     size_t getNbInputs() const {return(mSrcList.size());};
+
+     IN  *getReadBuffer(int id=0,int nb = inputSize) {return mSrcList[id]->getReadBuffer(nb);};
+     OUT *getWriteBuffer(int nb = outputSize) {return mDst.getWriteBuffer(nb);};
+
+     bool willUnderflow(int id=0,int nb = inputSize) const {return mSrcList[id]->willUnderflowWith(nb);};
+     bool willOverflow(int nb = outputSize) const {return mDst.willOverflowWith(nb);};
+
+private:
+    const std::vector<FIFOBase<IN>*> mSrcList;
+    FIFOBase<OUT> &mDst;
+
+};
+
+template<typename IN, int inputSize,
+         typename OUT, int outputSize>
+class GenericManyToManyNode:public NodeBase
+{
+public:
+     GenericManyToManyNode(std::initializer_list<FIFOBase<IN>*> src,
+                           std::initializer_list<FIFOBase<OUT>*> dst):mSrcList(src),mDstList(dst){};
+
+    
+protected:
+     size_t getNbInputs() const {return(mSrcList.size());};
+     size_t getNbOutputs() const {return(mDstList.size());};
+
+     IN  *getReadBuffer(int id=0,int nb = inputSize) {return mSrcList[id]->getReadBuffer(nb);};
+     OUT *getWriteBuffer(int id=0,int nb = outputSize) {return mDstList[id]->getWriteBuffer(nb);};
+
+     bool willUnderflow(int id=0,int nb = inputSize) const {return mSrcList[id]->willUnderflowWith(nb);};
+     bool willOverflow(int id=0,int nb = outputSize) const {return mDstList[id]->willOverflowWith(nb);};
+
+private:
+    const std::vector<FIFOBase<IN>*> mSrcList;
+    const std::vector<FIFOBase<OUT>*> mDstList;
+};
+
 template<typename IN, int inputSize,typename OUT1, int output1Size,typename OUT2, int output2Size>
 class GenericNode12:public NodeBase
 {
 public:
      GenericNode12(FIFOBase<IN> &src,FIFOBase<OUT1> &dst1,FIFOBase<OUT2> &dst2):mSrc(src),
      mDst1(dst1),mDst2(dst2){};
 
 protected:
-     OUT1 * getWriteBuffer1(int nb=output1Size){return mDst1.getWriteBuffer(nb);};
-     OUT2 * getWriteBuffer2(int nb=output2Size){return mDst2.getWriteBuffer(nb);};
-     IN * getReadBuffer(int nb=inputSize){return mSrc.getReadBuffer(nb);};
+     OUT1 * getWriteBuffer1(int nb=output1Size) {return mDst1.getWriteBuffer(nb);};
+     OUT2 * getWriteBuffer2(int nb=output2Size) {return mDst2.getWriteBuffer(nb);};
+     IN * getReadBuffer(int nb=inputSize) {return mSrc.getReadBuffer(nb);};
 
-     bool willOverflow1(int nb = output1Size){return mDst1.willOverflowWith(nb);};
-     bool willOverflow2(int nb = output2Size){return mDst2.willOverflowWith(nb);};
+     bool willOverflow1(int nb = output1Size) const {return mDst1.willOverflowWith(nb);};
+     bool willOverflow2(int nb = output2Size) const {return mDst2.willOverflowWith(nb);};
 
-     bool willUnderflow(int nb = inputSize){return mSrc.willUnderflowWith(nb);};
+     bool willUnderflow(int nb = inputSize) const {return mSrc.willUnderflowWith(nb);};
 
 private:
     FIFOBase<IN> &mSrc;
     FIFOBase<OUT1> &mDst1;
     FIFOBase<OUT2> &mDst2;
 };
 
@@ -342,25 +413,25 @@
                    FIFOBase<OUT1> &dst1,
                    FIFOBase<OUT2> &dst2,
                    FIFOBase<OUT3> &dst3
                    ):mSrc(src),
      mDst1(dst1),mDst2(dst2),mDst3(dst3){};
 
 protected:
-     OUT1 * getWriteBuffer1(int nb=output1Size){return mDst1.getWriteBuffer(nb);};
-     OUT2 * getWriteBuffer2(int nb=output2Size){return mDst2.getWriteBuffer(nb);};
-     OUT3 * getWriteBuffer3(int nb=output3Size){return mDst3.getWriteBuffer(nb);};
+     OUT1 * getWriteBuffer1(int nb=output1Size) {return mDst1.getWriteBuffer(nb);};
+     OUT2 * getWriteBuffer2(int nb=output2Size) {return mDst2.getWriteBuffer(nb);};
+     OUT3 * getWriteBuffer3(int nb=output3Size) {return mDst3.getWriteBuffer(nb);};
 
-     IN * getReadBuffer(int nb=inputSize){return mSrc.getReadBuffer(nb);};
+     IN * getReadBuffer(int nb=inputSize) {return mSrc.getReadBuffer(nb);};
 
-     bool willOverflow1(int nb = output1Size){return mDst1.willOverflowWith(nb);};
-     bool willOverflow2(int nb = output2Size){return mDst2.willOverflowWith(nb);};
-     bool willOverflow3(int nb = output3Size){return mDst3.willOverflowWith(nb);};
+     bool willOverflow1(int nb = output1Size) const {return mDst1.willOverflowWith(nb);};
+     bool willOverflow2(int nb = output2Size) const {return mDst2.willOverflowWith(nb);};
+     bool willOverflow3(int nb = output3Size) const {return mDst3.willOverflowWith(nb);};
 
-     bool willUnderflow(int nb = inputSize){return mSrc.willUnderflowWith(nb);};
+     bool willUnderflow(int nb = inputSize) const {return mSrc.willUnderflowWith(nb);};
 
 private:
     FIFOBase<IN> &mSrc;
     FIFOBase<OUT1> &mDst1;
     FIFOBase<OUT2> &mDst2;
     FIFOBase<OUT3> &mDst3;
 
@@ -371,21 +442,21 @@
 {
 public:
      GenericNode21(FIFOBase<IN1> &src1,FIFOBase<IN2> &src2,FIFOBase<OUT> &dst):mSrc1(src1),
      mSrc2(src2),
      mDst(dst){};
 
 protected:
-     OUT * getWriteBuffer(int nb=outputSize){return mDst.getWriteBuffer(nb);};
-     IN1 * getReadBuffer1(int nb=input1Size){return mSrc1.getReadBuffer(nb);};
-     IN2 * getReadBuffer2(int nb=input2Size){return mSrc2.getReadBuffer(nb);};
-
-     bool willOverflow(int nb = outputSize){return mDst.willOverflowWith(nb);};
-     bool willUnderflow1(int nb = input1Size){return mSrc1.willUnderflowWith(nb);};
-     bool willUnderflow2(int nb = input2Size){return mSrc2.willUnderflowWith(nb);};
+     OUT * getWriteBuffer(int nb=outputSize) {return mDst.getWriteBuffer(nb);};
+     IN1 * getReadBuffer1(int nb=input1Size) {return mSrc1.getReadBuffer(nb);};
+     IN2 * getReadBuffer2(int nb=input2Size) {return mSrc2.getReadBuffer(nb);};
+
+     bool willOverflow(int nb = outputSize) const {return mDst.willOverflowWith(nb);};
+     bool willUnderflow1(int nb = input1Size) const {return mSrc1.willUnderflowWith(nb);};
+     bool willUnderflow2(int nb = input2Size) const {return mSrc2.willUnderflowWith(nb);};
 
 private:
     FIFOBase<IN1> &mSrc1;
     FIFOBase<IN2> &mSrc2;
     FIFOBase<OUT> &mDst;
 };
 
@@ -394,91 +465,88 @@
 template<typename OUT, int outputSize>
 class GenericSource:public NodeBase
 {
 public:
      GenericSource(FIFOBase<OUT> &dst):mDst(dst){};
 
 protected:
-     OUT * getWriteBuffer(int nb=outputSize){return mDst.getWriteBuffer(nb);};
+     OUT * getWriteBuffer(int nb=outputSize) {return mDst.getWriteBuffer(nb);};
 
-     bool willOverflow(int nb = outputSize){return mDst.willOverflowWith(nb);};
+     bool willOverflow(int nb = outputSize) const {return mDst.willOverflowWith(nb);};
 
 private:
     FIFOBase<OUT> &mDst;
 };
 
 template<typename IN,int inputSize>
 class GenericSink:public NodeBase
 {
 public:
      GenericSink(FIFOBase<IN> &src):mSrc(src){};
 
 protected:
-     IN * getReadBuffer(int nb=inputSize){return mSrc.getReadBuffer(nb);};
+     IN * getReadBuffer(int nb=inputSize) {return mSrc.getReadBuffer(nb);};
 
-     bool willUnderflow(int nb = inputSize){return mSrc.willUnderflowWith(nb);};
+     bool willUnderflow(int nb = inputSize) const {return mSrc.willUnderflowWith(nb);};
 
 private:
     FIFOBase<IN> &mSrc;
 };
 
 
 #define REPEAT(N) for(int i=0;i<N;i++)
 
 
+template<typename IN, int inputSize,
+         typename OUT, int outputSize>
+class Duplicate;
+
 template<typename IO, int inputOutputSize>
-class Duplicate:public NodeBase
+class Duplicate<IO, inputOutputSize,
+                IO, inputOutputSize>:
+public GenericToManyNode<IO, inputOutputSize,
+                         IO, inputOutputSize>
 {
 public:
     Duplicate(FIFOBase<IO> &src,
-              std::initializer_list<FIFOBase<IO>*> dst):mSrc(src),mDstList(dst)
+              std::initializer_list<FIFOBase<IO>*> dst):
+    GenericToManyNode<IO, inputOutputSize,IO, inputOutputSize>(src,dst)
     {
     };
 
     int prepareForRunning() final
     {
         if (this->willUnderflow())
         {
            return(CG_SKIP_EXECUTION_ID_CODE); // Skip execution
         }
 
-        for(unsigned int i=0;i<mDstList.size();i++)
+        for(unsigned int i=0;i<this->getNbOutputs();i++)
         {
-           if (this->willOverflow(inputOutputSize,i))
+           if (this->willOverflow(i))
            {
               return(CG_SKIP_EXECUTION_ID_CODE); // Skip execution
            }
         }
 
 
         return(CG_SUCCESS_ID_CODE);
     };
 
     int run() final {
         IO *a=this->getReadBuffer();
         
-        for(unsigned int i=0;i<mDstList.size();i++)
+        for(unsigned int i=0;i<this->getNbOutputs();i++)
         {
-           IO *b=this->getWriteBuffer(inputOutputSize,i);
+           IO *b=this->getWriteBuffer(i);
            memcpy(b,a,sizeof(IO)*inputOutputSize);
         }
         
         return(CG_SUCCESS_ID_CODE);
     };
 
-protected:
-    IO * getWriteBuffer(int nb = inputOutputSize,int id=1){return mDstList[id]->getWriteBuffer(nb);};
-    IO * getReadBuffer(int nb = inputOutputSize){return mSrc.getReadBuffer(nb);};
-
-    bool willOverflow(int nb = inputOutputSize,int id=1){return mDstList[id]->willOverflowWith(nb);};
-    bool willUnderflow(int nb = inputOutputSize){return mSrc.willUnderflowWith(nb);};
-
-private:
-    FIFOBase<IO> &mSrc;
-    std::vector<FIFOBase<IO>*> mDstList;
-
 };
 
 
        
 
 #endif
```

## Comparing `cmsis_stream/cg/scheduler/templates/main_board.c` & `cmsis_stream/cg/scheduler/example/main_board.c`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/simple.cproject.yml` & `cmsis_stream/cg/scheduler/example/simple.cproject.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml` & `cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/start_project_appnodes.h` & `cmsis_stream/cg/scheduler/example/start_project_appnodes.h`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/start_project_graph.py` & `cmsis_stream/cg/scheduler/example/start_project_graph.py`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/vht.clayer.yml` & `cmsis_stream/cg/scheduler/example/vht.clayer.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.2.3.dist-info/LICENSE.txt` & `cmsis_stream-1.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.2.3.dist-info/METADATA` & `cmsis_stream-1.3.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.2.3
+Version: 1.3.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -41,14 +41,20 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate a C scheduler to run the graph on your target
 
 # Change history
 
+## Version 1.3.0:
+
+* New nodes `GenericToMany`, `GenericFromMany`, `GenericManyToMany`
+* `Duplicate` node implementation now using `GenericToMany`
+* Possibility to change the name of IOs in `Binary`, `Unary` and `Dsp` nodes
+
 ## Version 1.2.1:
 
 * Correct an issue in 1.2.0. Some templates needed
 by the new command line tool had not been included in the
 package.
 
 ## Version 1.2.0:
```

## Comparing `cmsis_stream-1.2.3.dist-info/RECORD` & `cmsis_stream-1.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -22,45 +22,46 @@
 cmsis_stream/cg/nodes/host/WavSink.py,sha256=ldo5e9wjaIp0Ef6GvRgZIICuuk3H1V7B-hn1et6S7Wo,2029
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=f57rHk2gtgkikywW_ZEkdXlibV4wnHbOQ5vi0fHRcME,3018
-cmsis_stream/cg/scheduler/config.py,sha256=IOnoVpfq6PuCgLyaOiUgnUPtuxq6w6txaWB4tZmg4NU,6615
-cmsis_stream/cg/scheduler/description.py,sha256=6ob9d7bfo1TXUBFWq9aPnnY1wFPklsqi7poXPECxFA4,41560
+cmsis_stream/cg/scheduler/config.py,sha256=J3W01wi-DO32EVKsgQ5ztUeNMBl0fDk2cXuOzySMM30,6665
+cmsis_stream/cg/scheduler/description.py,sha256=BJ0293P4bQL5iU1RxBJF_3mSJhGDIOjurS6eUTiBWCc,41606
 cmsis_stream/cg/scheduler/graphviz.py,sha256=wmbSzhIlOD9Z1E5NBsNklk4LvpaLQfs9Tmw-vAxwSPM,1784
-cmsis_stream/cg/scheduler/node.py,sha256=LJuuFbkWp8xJALM4aSXASaisYkhDQVfAfKlz0sQYnq4,29225
+cmsis_stream/cg/scheduler/node.py,sha256=kMeAhr109SCg77tbP6iTZGBvuKz7y4Md9AQa2OOkKP0,36807
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=bDtCVYvgtLO_wpl33HlyyAEZtfyW6wHyANQsdPvdlBA,1796
-cmsis_stream/cg/scheduler/standard.py,sha256=EEPGxII61ykghjLnVSkVV2s5DW2ZHfKI2ryhnDByhkU,8260
-cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
-cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=6r6w3HloYzH3u8WGz5mDjEyhOkdcumxf3o4qOjx2CM0,14002
-cmsis_stream/cg/scheduler/templates/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
-cmsis_stream/cg/scheduler/templates/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
-cmsis_stream/cg/scheduler/templates/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
+cmsis_stream/cg/scheduler/standard.py,sha256=VngMlAxV9n8HNPX50KDD_OLQvaTI4Q7iz_mxjRgHEWU,7523
+cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
+cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
+cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
+cmsis_stream/cg/scheduler/example/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
+cmsis_stream/cg/scheduler/example/README.md,sha256=_o0nMzYUELDms9o9Gh__4fuOTYqUAwabijVBSHkqsiA,566
+cmsis_stream/cg/scheduler/example/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
+cmsis_stream/cg/scheduler/example/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
+cmsis_stream/cg/scheduler/example/simple.cproject.yml,sha256=1Zpzt5Ebl30KDJ-5nh_9Ypg-igqrPiA_ek_2kGAJGzc,589
+cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
+cmsis_stream/cg/scheduler/example/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
+cmsis_stream/cg/scheduler/example/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
+cmsis_stream/cg/scheduler/example/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
+cmsis_stream/cg/scheduler/example/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
+cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
+cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=Xs7uGOL8YYvTaWc_L-07t029hiQiN5NqtV7g9V3s-gE,16526
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=yNiZSHN-riYPkzCenN6UUoZD9ZieCI8L9viXYkQCCz0,431
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=wbXrZ1fWz2YmD-yyvMshlaXvWXgTmfKokVEFu6SwAVk,279
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=bo05ISPFatzhi09c36ioA4HSJUtJc30k3T-z31oWN-8,674
 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp,sha256=luXUXScO1ncXx1m2kI2e40DyjobwbwVucCY0QernoGc,297
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
 cmsis_stream/cg/scheduler/templates/code.h,sha256=BULWyJn9FAU6laXpg6UjyP5TtHHMCW_3zTccu_EtjKU,1111
 cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=6fn_IVXZy77h8TQN2vSsuwMUVJFjyPtVzURjhnriAo0,3185
 cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=nmlbxVoBiujXLYerA056T_GPRL-LZSo0IFcz6BHdTHc,4482
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=h9R25-RcgG_kDKg4-xsGih4yPnffdNbZwkZMe5UXmhA,1051
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=GJyuIQkdt3RZvq2SRSBYrmuWj7QW9T4wVO-1GRGB8B0,4848
-cmsis_stream/cg/scheduler/templates/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
-cmsis_stream/cg/scheduler/templates/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
-cmsis_stream/cg/scheduler/templates/simple.cproject.yml,sha256=1Zpzt5Ebl30KDJ-5nh_9Ypg-igqrPiA_ek_2kGAJGzc,589
-cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
-cmsis_stream/cg/scheduler/templates/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
-cmsis_stream/cg/scheduler/templates/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
-cmsis_stream/cg/scheduler/templates/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
-cmsis_stream/cg/scheduler/templates/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
-cmsis_stream/cg/scheduler/templates/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
-cmsis_stream-1.2.3.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.2.3.dist-info/METADATA,sha256=zpt-t79_NwqaFPfuH7ADib011Z0jVEISaWolYnPyvls,3275
-cmsis_stream-1.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.2.3.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.2.3.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.2.3.dist-info/RECORD,,
+cmsis_stream-1.3.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.3.0.dist-info/METADATA,sha256=AoZOWEdgDMib_FLS4vv9CiikCpE60u-It-8Wt6RpJ_0,3506
+cmsis_stream-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.3.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.3.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.3.0.dist-info/RECORD,,
```

