# Comparing `tmp/kagsa-1.1.1.tar.gz` & `tmp/kagsa-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kagsa-1.1.1.tar", last modified: Fri Sep  9 21:21:47 2022, max compression
+gzip compressed data, was "kagsa-1.2.0.tar", last modified: Tue Jun  6 19:25:16 2023, max compression
```

## Comparing `kagsa-1.1.1.tar` & `kagsa-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-09-09 21:21:47.047689 kagsa-1.1.1/
--rw-rw-rw-   0        0        0     1081 2022-05-25 15:47:04.000000 kagsa-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6438 2022-09-09 21:21:47.046736 kagsa-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5778 2022-09-09 21:18:04.000000 kagsa-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-09 21:21:46.988561 kagsa-1.1.1/kagsa.egg-info/
--rw-rw-rw-   0        0        0     6438 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-09 21:21:46.000000 kagsa-1.1.1/kagsa.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-09-09 21:21:47.044739 kagsa-1.1.1/kagsasrc/
--rw-rw-rw-   0        0        0      214 2022-07-06 16:20:02.000000 kagsa-1.1.1/kagsasrc/__init__.py
--rw-rw-rw-   0        0        0     8669 2022-09-09 21:16:20.000000 kagsa-1.1.1/kagsasrc/__main__.py
--rw-rw-rw-   0        0        0    19864 2022-09-02 22:28:33.000000 kagsa-1.1.1/kagsasrc/built_modules.py
--rw-rw-rw-   0        0        0     7082 2022-09-09 19:12:44.000000 kagsa-1.1.1/kagsasrc/compiler.py
--rw-rw-rw-   0        0        0     3070 2022-08-27 14:23:32.000000 kagsa-1.1.1/kagsasrc/errors.py
--rw-rw-rw-   0        0        0     7065 2022-09-09 21:16:35.000000 kagsa-1.1.1/kagsasrc/exec_data.py
--rw-rw-rw-   0        0        0     3910 2022-09-09 18:20:37.000000 kagsa-1.1.1/kagsasrc/lexer.py
--rw-rw-rw-   0        0        0    10961 2022-08-29 15:10:44.000000 kagsa-1.1.1/kagsasrc/methods.py
--rw-rw-rw-   0        0        0     1674 2022-09-04 11:14:58.000000 kagsa-1.1.1/kagsasrc/parse_assign.py
--rw-rw-rw-   0        0        0      158 2022-06-29 14:01:46.000000 kagsa-1.1.1/kagsasrc/parse_cmnt.py
--rw-rw-rw-   0        0        0     1627 2022-09-04 11:10:12.000000 kagsa-1.1.1/kagsasrc/parse_co.py
--rw-rw-rw-   0        0        0      518 2022-07-06 17:52:42.000000 kagsa-1.1.1/kagsasrc/parse_cparen.py
--rw-rw-rw-   0        0        0     1275 2022-09-09 19:21:19.000000 kagsa-1.1.1/kagsasrc/parse_dot_coma.py
--rw-rw-rw-   0        0        0     3915 2022-08-24 18:19:20.000000 kagsa-1.1.1/kagsasrc/parse_endl.py
--rw-rw-rw-   0        0        0     2386 2022-09-04 11:08:54.000000 kagsa-1.1.1/kagsasrc/parse_id.py
--rw-rw-rw-   0        0        0     2813 2022-09-09 19:22:32.000000 kagsa-1.1.1/kagsasrc/parse_keyword.py
--rw-rw-rw-   0        0        0     1293 2022-09-04 11:18:18.000000 kagsa-1.1.1/kagsasrc/parse_math.py
--rw-rw-rw-   0        0        0     1562 2022-09-04 11:07:11.000000 kagsa-1.1.1/kagsasrc/parse_number.py
--rw-rw-rw-   0        0        0     1255 2022-09-04 11:30:53.000000 kagsa-1.1.1/kagsasrc/parse_paren.py
--rw-rw-rw-   0        0        0      983 2022-09-04 09:43:16.000000 kagsa-1.1.1/kagsasrc/parse_sformat.py
--rw-rw-rw-   0        0        0     1872 2022-09-09 19:20:58.000000 kagsa-1.1.1/kagsasrc/parse_string.py
--rw-rw-rw-   0        0        0     2564 2022-08-24 17:57:45.000000 kagsa-1.1.1/kagsasrc/parser.py
--rw-rw-rw-   0        0        0      901 2022-08-31 15:32:50.000000 kagsa-1.1.1/kagsasrc/paths.py
--rw-rw-rw-   0        0        0     3197 2022-07-06 16:12:39.000000 kagsa-1.1.1/kagsasrc/syntax_checker.py
--rw-rw-rw-   0        0        0       42 2022-09-09 21:21:47.047689 kagsa-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1568 2022-09-09 21:21:24.000000 kagsa-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:25:16.278581 kagsa-1.2.0/
+-rw-rw-rw-   0        0        0     1081 2022-09-09 21:26:34.000000 kagsa-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3747 2023-06-06 19:25:16.277584 kagsa-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3096 2023-06-01 19:45:57.000000 kagsa-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 19:25:16.201787 kagsa-1.2.0/kagsa.egg-info/
+-rw-rw-rw-   0        0        0     3747 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 19:25:16.000000 kagsa-1.2.0/kagsa.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 19:25:16.273594 kagsa-1.2.0/kagsasrc/
+-rw-rw-rw-   0        0        0      184 2023-03-10 22:19:12.000000 kagsa-1.2.0/kagsasrc/__init__.py
+-rw-rw-rw-   0        0        0    11267 2023-06-02 16:47:04.000000 kagsa-1.2.0/kagsasrc/__main__.py
+-rw-rw-rw-   0        0        0    19796 2023-06-02 19:17:53.000000 kagsa-1.2.0/kagsasrc/built_modules.py
+-rw-rw-rw-   0        0        0     6286 2023-06-06 18:12:14.000000 kagsa-1.2.0/kagsasrc/compiler.py
+-rw-rw-rw-   0        0        0     2466 2023-03-23 13:21:18.000000 kagsa-1.2.0/kagsasrc/errors.py
+-rw-rw-rw-   0        0        0     8112 2023-06-06 18:27:24.000000 kagsa-1.2.0/kagsasrc/exec_data.py
+-rw-rw-rw-   0        0        0     4035 2023-03-24 20:17:32.000000 kagsa-1.2.0/kagsasrc/lexer.py
+-rw-rw-rw-   0        0        0     1098 2023-06-02 18:07:37.000000 kagsa-1.2.0/kagsasrc/libtemplate.py
+-rw-rw-rw-   0        0        0    10859 2023-06-02 17:15:33.000000 kagsa-1.2.0/kagsasrc/methods.py
+-rw-rw-rw-   0        0        0     1656 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_assign.py
+-rw-rw-rw-   0        0        0      193 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_cmnt.py
+-rw-rw-rw-   0        0        0     1639 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_co.py
+-rw-rw-rw-   0        0        0      532 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_cparen.py
+-rw-rw-rw-   0        0        0     1257 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_dot_coma.py
+-rw-rw-rw-   0        0        0     3655 2023-06-01 17:28:17.000000 kagsa-1.2.0/kagsasrc/parse_endl.py
+-rw-rw-rw-   0        0        0     2287 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_id.py
+-rw-rw-rw-   0        0        0     3576 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_keyword.py
+-rw-rw-rw-   0        0        0     1277 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_math.py
+-rw-rw-rw-   0        0        0     1587 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_number.py
+-rw-rw-rw-   0        0        0     1239 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_paren.py
+-rw-rw-rw-   0        0        0      969 2023-06-02 11:30:10.000000 kagsa-1.2.0/kagsasrc/parse_sformat.py
+-rw-rw-rw-   0        0        0     2010 2023-03-11 15:14:07.000000 kagsa-1.2.0/kagsasrc/parse_string.py
+-rw-rw-rw-   0        0        0     2756 2023-06-01 17:29:27.000000 kagsa-1.2.0/kagsasrc/parser.py
+-rw-rw-rw-   0        0        0      965 2023-06-02 17:12:55.000000 kagsa-1.2.0/kagsasrc/paths.py
+-rw-rw-rw-   0        0        0     3197 2022-09-09 21:26:34.000000 kagsa-1.2.0/kagsasrc/syntax_checker.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:25:16.278581 kagsa-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-06-06 18:57:53.000000 kagsa-1.2.0/setup.py
```

### Comparing `kagsa-1.1.1/LICENSE` & `kagsa-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kagsa-1.1.1/kagsa.egg-info/SOURCES.txt` & `kagsa-1.2.0/kagsa.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 kagsasrc/__init__.py
 kagsasrc/__main__.py
 kagsasrc/built_modules.py
 kagsasrc/compiler.py
 kagsasrc/errors.py
 kagsasrc/exec_data.py
 kagsasrc/lexer.py
+kagsasrc/libtemplate.py
 kagsasrc/methods.py
 kagsasrc/parse_assign.py
 kagsasrc/parse_cmnt.py
 kagsasrc/parse_co.py
 kagsasrc/parse_cparen.py
 kagsasrc/parse_dot_coma.py
 kagsasrc/parse_endl.py
```

### Comparing `kagsa-1.1.1/kagsasrc/built_modules.py` & `kagsa-1.2.0/kagsasrc/built_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os,platform,subprocess,base64,sys,re,requests,json,random,time,datetime,keyboard
-from .methods import *
+import sys,platform,base64,os,requests,re,json,random,time,datetime,keyboard,math
+try:
+    from .methods import *
+except:
+    from methods import *
 
 #
 
 P_A_T_H = sys.path
 
+
 class W_e_b:
     class HTMLError (Exception):pass
     def s_c_r_i_p_t (data):
         return f'<script>{data}</script>'
     def b_o_x (data):
         data = data.replace('"','\\"')
         print(f'<script>alert("{data}")</script>')
-    class H_T_M_L_E_l_e_m_e_n_t:
-        def __init__ (self,inner,outer):
-            self.i_n_n_e_r_H_T_M_L = C_o_d_e.b_a_s_e_6_4.d_e_c_o_d_e(inner)
-            self.o_u_t_e_r_H_T_M_L = C_o_d_e.b_a_s_e_6_4.d_e_c_o_d_e(outer)
     class E_l_e_m_e_n_t:
         def __init__ (self,tagName,n,innerHTML,**attrs):
             self.t_a_g_N_a_m_e = tagName
             if not(n in [1,2,'1','2']):
                 raise W_e_b.HTMLError('Element(tagName, n, innerHTML, **attrs) n must be 1 or 2')
             self.n = n
             self.a_t_t_r_s = attrs
@@ -69,21 +69,24 @@
     def n_e_w_H_o_t_k_e_y (text, func):
         try:
             keyboard.add_hotkey(text, func)
         except Exception as ee : raise K_e_y_b_o_a_r_d.KeyboardError(str(ee))
     class r_e_c_o_r_d:
         def __init__ (self,u_n_t_i_l=''):
             try:
-                self.record = keyboard.record(until= u_n_t_i_l)
                 self.g_e_t = []
-                for i in self.record:
+                self.recorded = []
+                keyboard.hook(self.recorded.append)
+                keyboard.wait(u_n_t_i_l)
+                keyboard.unhook(self.recorded.append)
+                for i in self.recorded:
                     self.g_e_t.append(str(i).replace('KeyboardEvent(','')[0:-1])
             except Exception as ee : raise K_e_y_b_o_a_r_d.KeyboardError(str(ee))
         def p_l_a_y_A_l_l (self,s_p_e_e_d=0.5):
-            keyboard.play(self.record, speed_factor = s_p_e_e_d)
+            keyboard.play(self.recorded, speed_factor = s_p_e_e_d)
     def p_r_e_s_s (text):
         try:
             keyboard.press_and_release(text)
         except Exception as ee : raise K_e_y_b_o_a_r_d.KeyboardError(str(ee))
 
 
 class M_a_t_h:
@@ -206,16 +209,16 @@
 
 
 class R_a_n_d_o_m:
     def s_t_r (length, a_b_c=True, c_a_p=True, n_u_m=True, a_d_d=''):
         chars = ''
         if a_b_c:
             chars+='qwertyuioplkjhgfdsazxcvbnm'
-            if c_a_p:
-                chars+='QWERTYUIOPLKJHGFDSAZXCVBNM'
+        if c_a_p:
+            chars+='QWERTYUIOPLKJHGFDSAZXCVBNM'
         if n_u_m:
             chars+='0123456789'
         chars+=a_d_d
         chars = chars * 2
         return ''.join(random.sample(chars,length))
     def i_n_t (s,e):
         return random.randint(s,e)
@@ -418,15 +421,15 @@
             return re.split(self.re_str,string,t_i_l_l)
     def r_e_p_l_a_c_e(self,string,join):
         return re.sub(self.re_str, join, string)
     
 
 class S_y_s_t_e_m:
     a_r_g_v = sys.argv[1:]
-    def i_n_p_u_t():
+    def r_e_a_d ():
         return sys.stdin.readline()
     class w_r_i_t_e :
         def o_u_t (*text):
             for i in text : sys.stdout.write(i)
             return 1
         def e_r_r (*text):
             print(*text, file = sys.stderr)
@@ -434,15 +437,15 @@
     def e_x_i_t (text):
         sys.exit(text)
     def c_m_d (command):
         os.system(command)
         return 0
     def e_x_e_c (command):
         popen = os.popen(command)
-        return o.read()
+        return popen.read()
     def p_a_t_h ():
         return os.getcwd()
     def i_n_f_o_r_m_a_t_i_o_n_s ():
         UNAME = platform.uname()
         out = {
             'system':UNAME.system,
             'node':UNAME.node,
```

### Comparing `kagsa-1.1.1/kagsasrc/compiler.py` & `kagsa-1.2.0/kagsasrc/compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,58 @@
 from .methods import *
 from .built_modules import *
 from .errors import __init__ as errors
 from .parse_id import __init__ as parse_id
 from .paths import Paths as Paths
-import re,zipfile,random,os,sys,traceback,requests
+import sys,re,zipfile,traceback,os,requests,copy
+
 
-Paths.init()
 
-def encodeString (string):
-    data = ''
-    for char in string:
-        data += chr(ord(char)+2)
-    return data
 
 def main (data,kagsa_file,lib=False,lib_name=None,memory=None):
     data = '\n'.join(data)
     # Replace ( Some Symbols Codes ) to ( Backslash + str sybmbols )
     data = data.replace('STR_SYM_TWO','\\"' ).replace('STR_SYM_ONE',"\\'" ).replace('STR_SYM_THREE',"``")
     #print(data)
     MEMORY = {
         'errors':errors,
         're':re,
         'os':os,
         'zipfile':zipfile,
         'sys':sys,
         'traceback':traceback,
         'parse_id':parse_id,
-        'requests':requests
+        'requests':requests,
+        'Paths':Paths,
+        'copy':copy
     }
     KAGSALINES=data
     kagsa_file = kagsa_file.replace('\\','\\\\')
     exec_data = Paths.getFile('exec_data.py','r').read().replace('[KAGSA-FILE]', kagsa_file)    
     data = exec_data + data
     if lib:
-        d1 =  encodeString('#\n#\n#\n#\n#\n#\n#\n' + data.replace('\\','\\\\').replace('"','\\"').replace("\n","\\n")).replace('"','\\"')
-        data = f'import re,zipfile,os,sys,traceback\nfrom __memory__ import *\ndef decodeString (string):\n\tdata = \'\'\n\tfor char in string: data += chr(ord(char)-2)\n\treturn data\nFullCodes = decodeString("{d1}")'  +  data
-
-        __memory__ = 'import os,platform,subprocess,base64,sys,re,requests,json,random,time,datetime\n\n'
-        __memory__+= Paths.getFile('errors.py','r').read().replace(
-            'def __init__ (theErr,get_value_back=False, lineno=None):',
-            'def errors (theErr,get_value_back=False, lineno=None):'
-        )+'\n'
-
-        __memory__+= Paths.getFile('methods.py','r').read()+'\n'
-        __memory__+= Paths.getFile('parse_id.py','r').read().replace(
-            'def __init__ (value,parseMemory):',
-            'def parse_id (value,parseMemory):'
-        )+'\n'
-        __memory__+= '\n'.join(Paths.getFile('built_modules.py','r').read().split('\n')[3:])
-
-
+        nl='\n'
+        kgl_text = Paths.getFile('libtemplate.py','r').read() + '\n' + f'KAGSA_FILE=Paths.__path__() + os.sep + "temp" + os.sep + "{kagsa_file}" \nKAGSA_FILE2 = "{kagsa_file}"\ntry: KAGSA_CODES=open(KAGSA_FILE).read() \nexcept: KAGSA_CODES=open(KAGSA_FILE2).read() \n' + data
         kgl = zipfile.ZipFile(lib_name,'w')
-        kgl.writestr('main.py', data)
-        kgl.writestr('__memory__.py', __memory__)
+        kgl.writestr( kagsa_file , open(kagsa_file).read())
+        kgl.writestr('main.py', kgl_text)
         kgl.close()
     # For Run a Code
     else:
         # 
         # Create a Memory for Run Python Codes
         #
         MEMORY = dict(globals() , **locals(), **MEMORY)
         if memory != None:
             for i,j in memory.items():
                 MEMORY[i]=j
-        MEMORY['FullCodes'] = data
-        MEMORY['kagsa_lines'] = KAGSALINES
+        MEMORY['KAGSA_CODES'] = KAGSALINES
+        MEMORY['KAGSA_FILE']  = kagsa_file
         try:
+            #print(KAGSALINES)
             exec(data,MEMORY)
             return MEMORY
         #
         # The Exception of Compiler Error
         #  How This Work ?
         #    1- Search For The Last Traceback
         #    2- Get The Line Thats Writed in The Translated Python Codes
```

### Comparing `kagsa-1.1.1/kagsasrc/errors.py` & `kagsa-1.2.0/kagsasrc/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,48 @@
 import re
 
 
-
 def __init__ (theErr,get_value_back=False, lineno=None):
-    # Get Error Text & Type
-    ErrStr=str(theErr).replace('<string>','<file>').replace('.',' . ')
+    ErrStr=str(theErr).replace('<string>','<file>')
     ErrStr=ErrStr.replace('expected an indented block after function definition' , 'empty code block')
     ErrStr=ErrStr.replace('print()' , 'write')
     ErrStr=ErrStr.replace('str()' , 'string variable')
     ErrStr=ErrStr.replace('float()' , 'float variable')
     ErrStr=ErrStr.replace('int()' , 'int variable')
     ErrStr=ErrStr.replace('JSONDecoder.__init__()' , 'json variable')
     ErrStr=ErrStr.replace('list()' , 'list variable')
     ErrStr=ErrStr.replace('input()' , 'input')
     ErrStr=ErrStr.replace('INCLUDE()' , 'include')
     ErrStr=ErrStr.replace('JUMP()' , 'jump')
-    ErrType=theErr.__class__.__name__.replace('error','ERR').replace('Error','ERR').replace('compiler.classes.__init__.','').replace('.',' . ')
-
+    ErrStr=ErrStr.replace('STR_SYM_TWO','\\"').replace("STR_SYM_ONE","\\'").replace("STR_SYM_THREE","\\``")
+    ErrType=theErr.__class__.__name__.replace('error','ERR').replace('Error','ERR').replace('compiler.classes.__init__.','')
     if lineno!=None:
         lll = re.findall(r'line \d+',ErrStr)
         for i in lll: ErrStr=ErrStr.replace(i , 'line '+lineno)
-    # Start Decoding Texts
-    #
-    ###########################################################################
-    text=ErrStr.replace('(','').replace(')','').replace('"','').replace('\'','')
-    text=text.replace('__','_C')
-    for c in list('1234567890qwertyuioplkjhgfdsazxcvbnmQWERTYUIOPLKJHGFDSAZXCVBNMأبتثج'):
-        text=text.replace(c,'C')
-    COUNT=-1
-    for i in text.split(' '):
-        COUNT+=1
-        i=i[1:]
-        i=i.replace('_C','')
-        if i =='':
-            ORG=ErrStr.split(' ')[COUNT]
-            Org=ErrStr.split(' ')[COUNT].replace('__','ة').replace('_','').replace('ة','_')
-            ErrStr=ErrStr.replace(ORG,Org)
-    #
-    ###########################################################################
-    text=ErrType.replace('(','').replace(')','').replace('"','').replace('\'','')
-    text=text.replace('__','_C')
-    for c in list('1234567890qwertyuioplkjhgfdsazxcvbnmQWERTYUIOPLKJHGFDSAZXCVBNMأبتثج'):
-        text=text.replace(c,'C')
-    COUNT=-1
-    for i in text.split(' '):
-        COUNT+=1
-        i=i[1:]
-        i=i.replace('_C','')
-        if i =='':
-            ORG=ErrType.split(' ')[COUNT]
-            Org=ErrType.split(' ')[COUNT].replace('__','ة').replace('_','').replace('ة','_')
-            ErrType=ErrType.replace(ORG,Org)
-    ###########################################################################
-    #
-    # Somethings..
+    #############################################
     Symbols = {
         'أ' : '@',
         'ب' : '$',
         'ت' : '^',
         'ث' : '~',
         'ج' : '?'
     }
     for i in Symbols.items():
         ErrStr = ErrStr.replace(i[0], i[1])
         ErrType = ErrType.replace(i[0], i[1])
-    ErrType=ErrType.replace(' . ','.')
-    ErrStr=ErrStr.replace(' . ','.').replace('STR_SYM_TWO','\\"').replace("STR_SYM_ONE","\\'").replace("STR_SYM_THREE","\\``")
-    # Return a Values or Print it
+    #############################################
+    ErrStr_tmp = ErrStr.replace('(','').replace(')','').replace('\'','').replace('"','').replace('.',' . ')
+    ErrType_tmp = ErrType.replace('.',' . ')
+    try:
+        for word in [word for word in ErrStr_tmp.split(' ') if not(word[0].isdigit() or word[0] == '_' and not word[1].isdigit() or any([len(char) > 1 for char in word.split('_')]))]:
+            new_word = ''.join(word.replace('__','ظ').split('_')).replace('ظ','_')
+            ErrStr = ErrStr.replace(word,new_word)
+        
+        for word in [word for word in ErrType_tmp.split(' ') if not(word[0].isdigit() or word[0] == '_' and not word[1].isdigit() or any([len(char) > 1 for char in word.split('_')]))]:
+            new_word = ''.join(word.replace('__','ظ').split('_')).replace('ظ','_')
+            ErrStr = ErrStr.replace(word,new_word)
+    except:None
+    #############################################
     if get_value_back:
         return [ErrType, ErrStr, f'{ErrType} : {ErrStr}']
     else:
         print(f'{ErrType} : {ErrStr}',end='')
```

### Comparing `kagsa-1.1.1/kagsasrc/exec_data.py` & `kagsa-1.2.0/kagsasrc/exec_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 class g_e_t_E_r_r_o_r ():
     def __init__ (self) :
         self.t_e_x_t     = ''
         self.l_i_n_e_n_o = ''
         self.l_i_n_e     = ''
         self.t_y_p_e     = ''
         self.f_i_l_e     = '[KAGSA-FILE]'
+        try:    errGet = globals()['ERROR']
+        except: errGet = locals()['ERROR']
 
         if self.f_i_l_e == '[stdin]':
             self.l_i_n_e_n_o = 1
-            E = errors(globals()['ERROR'], get_value_back=True)
+            E = errors(errGet, get_value_back=True)
             self.t_e_x_t = E[1]
             self.t_y_p_e = E[0]
             self.l_i_n_e = ''
             return
         the_tb = traceback.extract_tb(sys.exc_info()[2])
         tb_filename, tb_lineno, tb_func, tb_line = the_tb[-1]
         tb_filetype = 'py'
         # parse the error filename
         # error came from kagsa code
         if tb_filename == '<string>':
-            self.f_i_l_e = kagsa_file
+            self.f_i_l_e = KAGSA_FILE
             tb_filetype = 'kg'
         # form a library
         elif 'kgtmp' in tb_filename:
             self.f_i_l_e = tb_filename.split(os.sep)[-1].replace('_main.py','')
             self.f_i_l_e = self.f_i_l_e.replace('__','ة').replace('_','').replace('ة','_')
             self.f_i_l_e+= '.kgl'
         # something else
@@ -52,23 +54,23 @@
             for ttb in the_tb:
                 tb_fn, tb_lno, tb_f, _ = ttb
                 if (tb_fn == '<string>'):
                     tb_filename, tb_lineno, tb_func, _ = ttb
                     data_founded =True
                     break
             if not(data_founded):
-                tb_lineno = int(re.findall(r', line (\d+)',str(globals()['ERROR']))[0])
-            self.f_i_l_e = kagsa_file
+                tb_lineno = int(re.findall(r', line (\d+)',str(errGet))[0])
+            self.f_i_l_e = KAGSA_FILE
             tb_filetype = 'kg'
         
         try:
             if tb_filetype == 'kg':
-                tb_lineno = FullCodes.split('\n')[tb_lineno-1]
+                tb_lineno = KAGSA_CODES.split('\n')[tb_lineno-1]
                 tb_lineno = int(re.findall(r'    # line (\d+)',tb_lineno)[-1])
-                x = open(kagsa_file,'r')
+                x = open(KAGSA_FILE,'r')
                 file_lines = x.read().split('\n')
                 x.close()
                 file_lines_no = len( file_lines )
             else:
                 x = open(tb_filename, 'r')
                 file_lines = x.read().split('\n')
                 x.close()
@@ -83,15 +85,15 @@
                 self.l_i_n_e       = '?'
                 self.l_i_n_e_n_o   ='?'
         except:
             self.l_i_n_e       = '?'
             self.l_i_n_e_n_o   = '?'
         
 
-        E = errors(globals()['ERROR'], get_value_back=True)
+        E = errors(errGet, get_value_back=True)
         self.t_e_x_t = E[1]
         self.t_y_p_e = E[0]
 
 
 
 
 
@@ -99,48 +101,69 @@
 class IncludeError (Exception):
     pass
 
 def INCLUDE (lib):
     try:
         # check if input is string
         if not(lib.__class__.__name__ == 'str') :
-            raise IncludeError('libarary must be string')
+            raise IncludeError('library must be string')
         # check if input is .kgl file
         if not(lib.endswith('.kgl')):
             raise IncludeError('libarary must be ".kgl" file')
         if len(re.findall(r'[a-zA-Z_][a-zA-Z0-9_]*\.kgl|[a-zA-Z_]\.kgl', lib)) < 1 :
             raise IncludeError('filename must be writted as this syntax "[a-zA-Z_][a-zA-Z0-9_]*\.kgl|[a-zA-Z_]\.kgl"')
         if not(re.findall(r'[a-zA-Z_][a-zA-Z0-9_]*\.kgl|[a-zA-Z_]\.kgl', lib)[0] == lib):
             raise IncludeError('filename must be writted as this syntax "[a-zA-Z_][a-zA-Z0-9_]*\.kgl|[a-zA-Z_]\.kgl"')
         # try open file
-        open(lib,'r')
+        try:
+            open(lib)
+        except:
+            Paths.getFile('libs' + os.sep + lib,'r')
         if os.sep in lib:
             lib_name = lib.split(os.sep)[-1]
         lib_name = lib.replace('.kgl','')
         # parse lib_name
         if (len(lib_name)>2) or (len(lib_name)==2):
             lib_name='_'.join(list(lib_name))
         if lib_name[0] in '1234567890' :
             lib_name='_'+lib_name
         # end parse
         # read it :
-        # create "kgtmp"
-        try:os.mkdir('kgtmp')
-        except:pass
+
         # get "main.py"
-        archive = zipfile.ZipFile(lib,'r')
-        py_file = open(f'kgtmp{os.sep}{lib_name}_main.py','wb')
-        py_file.write(archive.read('main.py'))
-        py_file.close()
-        # get "__memory__.py"
-        archive.extract('__memory__.py', 'kgtmp')
+        try:
+            archive = zipfile.ZipFile(lib,'r')
+        except:
+            archive = zipfile.ZipFile(Paths.__path__() + os.sep + 'libs' + os.sep + lib,'r')
+        try:
+            KAGSA_TEMP = Paths.__path__() + os.sep + 'temp' + os.sep
+            # write python library
+            py_file = open(f'{KAGSA_TEMP}{lib_name}_main.py','wb')
+            py_file.write(archive.read('main.py'))
+            py_file.close()
+            # write the kg file
+            kg_file_name = [ff for ff in archive.namelist() if ff.endswith('.kg')]
+            kg_file = open(f'{KAGSA_TEMP}{kg_file_name[0]}','wb')
+            kg_file.write(archive.read(kg_file_name[0]))
+            kg_file.close()
+        except:
+            KAGSA_TEMP = Paths.__path__() + os.sep
+            # write python library
+            py_file = open(f'{KAGSA_TEMP}{lib_name}_main.py','wb')
+            py_file.write(archive.read('main.py'))
+            py_file.close()
+            # write the kg file
+            kg_file_name = [ff for ff in archive.namelist() if ff.endswith('.kg')]
+            kg_file = open(f'{KAGSA_TEMP}{kg_file_name[0]}','wb')
+            kg_file.write(archive.read(kg_file_name[0]))
+            kg_file.close()
         # import it
         global exec_scope
         exec_scope = {}
-        sys.path.insert(1, 'kgtmp')
+        #sys.path.insert(1, KAGSA_TEMP[0:-1])
         try:
             exec(f'import {lib_name}_main',exec_scope)
             exec(f'def send_to_globals () :\n\tglobal {lib_name}\n\t{lib_name} = exec_scope["{lib_name}_main"]',globals())
             send_to_globals()
         except Exception as e:
             raise IncludeError(str(e))
     except FileNotFoundError:
@@ -152,15 +175,15 @@
         d.append(i)
     return d
 
 class JumpingError (Exception):
     pass
 
 def JUMP (lineno):
-    lines = kagsa_lines
+    lines = KAGSA_CODES
     lines_dict = {}
     data_founded = 0
     data = ''
     
     # Create a dict with all lines -> {'2','print("hi")    # line 2'}
     last=''
     for j in lines.split('\n'):
```

### Comparing `kagsa-1.1.1/kagsasrc/lexer.py` & `kagsa-1.2.0/kagsasrc/lexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,17 +79,20 @@
         end.append(['ENDLINE','\n'])
         #print(end)
         return end
     except Exception as err:
         # Return a Illegal Character Error
         if 'Illegal character' in str(err):
             ERR=str(err)
+            # Get the illegal char
             try:
                 char=re.findall(r"'(.*?)'",ERR)[0]
             except:
                 char=re.findall(r'"(.*?)"',ERR)[0]
-            index=ERR[ERR.find('index '):].replace('index ','')
-            line=context.count('\n')+1
+            # Get the index
+            index=int(ERR[ERR.find('index '):].replace('index ',''))
+            # Get the line
+            line=context[0:index].count('\n')+1
             raise SyntaxError(f'illegal char "{char}" in index {index}, line {line}')
         # Return a Unknown Error
         else:
-            raise err
+            raise SyntaxError(str(err))
```

### Comparing `kagsa-1.1.1/kagsasrc/methods.py` & `kagsa-1.2.0/kagsasrc/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import forbiddenfruit,threading
-
+import threading,forbiddenfruit
 
 
 def SetMethod (datatypes, name, func):
     for datatype in datatypes:
         forbiddenfruit.curse(datatype,name,func)
 
 def t_o_I_n_t (value):
@@ -40,181 +39,173 @@
 def i_s_D_i_c_t (value):
     if value.__class__.__name__ == 'dict':
         return 1
     else:
         return 0
 
 def n_l_i_s_t (num, z_e_r_o=True):
-    d = []
     if z_e_r_o:
-        for i in range(0,num+1): d.append(i)
+        return range(0,num+1)
     else:
-        for i in range(1,num+1): d.append(i)
-    return d
+        return range(1,num+1)
 
 def d_i_r (data):
     lst = []
+    dd = ' '.join(dir(data))
     #print(dir(data))
-    for value in dir(data):
-        text=value.replace('__','_C')
-        for c in list('1234567890qwertyuioplkjhgfdsazxcvbnmQWERTYUIOPLKJHGFDSAZXCVBNMأبتثج'):
-            text=text.replace(c,'C')
-        text=text[1:]
-        text=text.replace('_C','')
-        #
-        if text == '':
-            value = value.replace('أ','@').replace('ب','$').replace('ت','^').replace('ث','~').replace('ج','?')
-            if (value[0]=='_') and (value[1] in '1234567890') :
-                value = value[1:]
-            value = value.replace('__','ة').replace('_','').replace('ة','_')
-            #
-            lst.append(value)
-        elif value in ['__init__','__str__','__repr__','self']:
-            dct = {'__init__':'@constructor','__str__':'@string','__repr__':'@repr','self':'@this'}
-            lst.append(dct[value])
+    for word in [word for word in dd.split(' ') if not(word[0].isdigit() or word[0] == '_' and not word[1].isdigit() or any([len(char) > 1 for char in word.split('_')]))]:
+        lst.append( ''.join(word.replace('__','ظ').split('_')).replace('ظ','_') )
     return lst
 
 
 n_l = '\n'
 n_o_n_e = None
 n_o_t = lambda co:not(co)
 
 # Methods Starts from Here...
 def r_e_p_l_a_c_e (DATA,v1,v2):
-    if 'str' in DATA.__class__.__name__:
+    if 'str' == DATA.__class__.__name__:
         return DATA.replace(v1,v2)
     else:
         raise ValueError('"replace()" function take only (str) value')
 def s_p_l_i_t (DATA,value):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.split(value)
     else:
         raise ValueError('"split()" function take only (str) value')
 def e_n_d (DATA,value):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.endswith(value)
     else:
         raise ValueError('"end()" function take only (str) value')
 def s_t_a_r_t (DATA,value):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.startswith(value)
     else:
         raise ValueError('"start()" function take only (str) value')
 def s_e_a_r_c_h (DATA,value):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.find(value)
     else:
         raise ValueError('"search()" function take only (str) value')
 def u_p_c_a_s_e (DATA):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.upper()
     else:
         raise ValueError('"upcase()" function take only (str) value')
 def d_o_w_n_c_a_s_e (DATA):
-    if ('str' in DATA.__class__.__name__):
+    if ('str' == DATA.__class__.__name__):
         return DATA.lower()
     else:
         raise ValueError('"downcase()" function take only (str) value')
 def s_t_r_i_p (DATA):
     if ('str' in DATA.__class__.__name__):
         return DATA.strip()
     else:
         raise ValueError('"delspace()" function take only (str) value')
-
+def r_e_v_e_r_s_e (DATA):
+    if ('str' == DATA.__class__.__name__) or ('list' == DATA.__class__.__name__): 
+        return DATA[::-1]
+    else:
+        ValueError('"reverse()" function take only (str,list) value')
 
 
 # List Function
 def l_i_s_t (*arg):
     d = []
     for i in arg: d.append(i)
     return d
 # LIST, DICT, STR
 def l_e_n_g_t_h (DATA):
-    if ('dict' in DATA.__class__.__name__) or ('list' in DATA.__class__.__name__) or ('str' in DATA.__class__.__name__):
+    if ('dict' == DATA.__class__.__name__) or ('list' == DATA.__class__.__name__) or ('str' == DATA.__class__.__name__):
         return len(DATA)
     else:
         raise ValueError('"length(DATA)" function take only (dict, list, str) value')
 # LIST, DICT, STR
 def g_e_t (DATA,*value):
-    if (('list' in DATA.__class__.__name__)) or (('dict' in DATA.__class__.__name__)) or ('str' in DATA.__class__.__name__) :
+    if (('list' == DATA.__class__.__name__)) or (('dict' == DATA.__class__.__name__)) or ('str' == DATA.__class__.__name__) :
         if len(value)>1:
-            if 'dict' in DATA.__class__.__name__: raise ValueError('"get(VAR , value)" function take only (list, str) value')
+            if 'dict' == DATA.__class__.__name__: raise ValueError('"get(VAR , value)" function take only (list, str) value')
             return DATA[value[0]:value[1]]
         else:
             return DATA[value[0]]
     else:
         raise ValueError('"get(VAR , *value)" function take only (dict, list, str) value')
 # LIST, DICT
 def a_p_p_e_n_d (DATA,*arguments):
-    if 'list' in DATA.__class__.__name__:
+    if 'list' == DATA.__class__.__name__:
         for i in arguments :
             DATA.append(i)
-    elif 'dict' in DATA.__class__.__name__:
+    elif 'dict' == DATA.__class__.__name__:
         DATA[arguments[0]]=arguments[1]
     else:
         raise ValueError('"append(VAR , value)" function take only (list, dict) value')
 # LIST, DICT
 def c_l_e_a_r (DATA):
-    if (('list' in DATA.__class__.__name__)) or (('dict' in DATA.__class__.__name__)):
+    if (('list' == DATA.__class__.__name__)) or (('dict' in DATA.__class__.__name__)):
         DATA.clear()
         return 1
     else:
         raise ValueError('"clear(VAR)" function take only (list, dict) value')
 # LIST, DICT
 def d_e_l_e_t_e (DATA,value,i_d_x=False):
-    if ('list' in DATA.__class__.__name__):
+    if ('list' == DATA.__class__.__name__):
         if i_d_x and (i_s_I_n_t(value)):
             DATA.pop(value)
         elif i_d_x==False:
             DATA.remove(value)
         else:
             raise ValueError('"dalete(VAR, value, idx=BOOL)" if "idx" = true -> value must be int')
-    elif (('dict' in DATA.__class__.__name__)):
+    elif (('dict' == DATA.__class__.__name__)):
         DATA.pop(value)
     else:
         raise ValueError('"delete(VAR , value, idx=BOOL)" function take only (list, dict) value')
     return 1
 # LIST, DICT
 def a_d_d (DATA,pos,value):
-    if (('list' in DATA.__class__.__name__)):
+    if (('list' == DATA.__class__.__name__)):
         if not(i_s_I_n_t(pos)):
             raise ValueError('"add(VAR, pos, val)" pos must be int')
         DATA.insert(pos,value)
-    elif (('dict' in DATA.__class__.__name__)):
+    elif (('dict' == DATA.__class__.__name__)):
         DATA[pos]=value
     else:
         raise ValueError('"add()" function take only (list, dict) value')
     return 1
 # LIST
 def i_n_d_e_x (DATA,value):
-    if (('list' in DATA.__class__.__name__)):
+    if (('list' == DATA.__class__.__name__)):
         return DATA.index(value)
     else:
         raise ValueError('"index(VAR , value)" function take only (list) value')
 # LIST
 def a_p_p_l_i_s_t (DATA,value):
-    if ('list' in DATA.__class__.__name__) and ('list' in value.__class__.__name__):
+    if ('list' == DATA.__class__.__name__) and ('list' == value.__class__.__name__):
         DATA.extend(value)
     else:
         raise ValueError('"applist(VAR , value)" function take only (list) values')
     return 1
 # LIST, STR
 def c_o_u_n_t (DATA,value):
-    if (('list' in DATA.__class__.__name__)) or (('str' in DATA.__class__.__name__)):
+    if (('list' == DATA.__class__.__name__)) or (('str' == DATA.__class__.__name__)):
         return DATA.count(value)
     else:
         raise ValueError('"count(VAR , value)" function take only (list) value')
 # LIST
 def j_o_i_n (DATA,value):
-    if (('list' in DATA.__class__.__name__)):
+    if (('list' == DATA.__class__.__name__)):
         return value.join(DATA)
     else:
         raise ValueError('"join(VAR , value)" function take only (list) value')
 
-
+def s_o_r_t_e_d (DATA):
+    if ('list' == DATA.__class__.__name__):
+        return sorted(DATA)
+    else:
+        raise ValueError('"join(VAR , value)" function take only (list) value')
 
 # Dict Function
 def d_i_c_t (**arg):
     dct={}
     for i in arg:
         text=i.replace('__','$').replace('_','').replace('$','_')
         dct[text]=arg[i]
@@ -238,22 +229,24 @@
     SetMethod([str],'e_n_d',e_n_d)
     SetMethod([str],'s_t_a_r_t',s_t_a_r_t)
     SetMethod([str],'s_e_a_r_c_h',s_e_a_r_c_h)
     SetMethod([str],'u_p_c_a_s_e',u_p_c_a_s_e)
     SetMethod([str],'d_o_w_n_c_a_s_e',d_o_w_n_c_a_s_e)
     SetMethod([str],'s_t_r_i_p',s_t_r_i_p)
     SetMethod([str,list,dict],'l_e_n_g_t_h',l_e_n_g_t_h)
+    SetMethod([str,list],'r_e_v_e_r_s_e',r_e_v_e_r_s_e)
     SetMethod([str,list,dict],'g_e_t',g_e_t)
     SetMethod([list,dict],'a_p_p_e_n_d',a_p_p_e_n_d)
     SetMethod([list,dict],'c_l_e_a_r',c_l_e_a_r)
     SetMethod([list,dict],'d_e_l_e_t_e',d_e_l_e_t_e)
     SetMethod([list,dict],'a_d_d',a_d_d)
     SetMethod([list],'i_n_d_e_x',i_n_d_e_x)
     SetMethod([list],'a_p_p_l_i_s_t',a_p_p_l_i_s_t)
     SetMethod([list],'j_o_i_n',j_o_i_n)
+    SetMethod([list],'s_o_r_t_e_d',s_o_r_t_e_d)
     SetMethod([str,list],'c_o_u_n_t',c_o_u_n_t)
     SetMethod([dict],'k_e_y_s',k_e_y_s)
     SetMethod([dict],'v_a_l_u_e_s',v_a_l_u_e_s)
     #SetMethod([str],'',)
 threading.Thread(target=buildMethods).start()
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_assign.py` & `kagsa-1.2.0/kagsasrc/parse_assign.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 
 def __init__ (value,parseMemory):
+
     # catch errors
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
     # if |DATA-P| is empty : close it
     if '|DATA-P|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA-P|','')
     # this mean the var is opened with assign
     if ('|DATA1|' in parseMemory[5]) and (parseMemory[6] == False):
         parseMemory[6] = True
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_co.py` & `kagsa-1.2.0/kagsasrc/parse_co.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 class ParseError(Exception):pass
 
 def __init__ (value,parseMemory):
+
     # errors
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {line})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {line})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {line})\nCan\'t add any arguments to try command')
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
     value=value.replace(' ','')
     newValues={
         '->':' in ',
         '<=':'<=',
         '>=':'>=',
         '==':'==',
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_cparen.py` & `kagsa-1.2.0/kagsasrc/parse_cparen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .parse_endl import __init__ as parse_endl
 
 def __init__ (value,parseMemory):
+
     parseMemory[5] = parseMemory[5].replace('|DATA-P|','')
     if value=='{':
         parseMemory[1]=True
     else:
         parseMemory[1] = False
         if parseMemory[0]==0:
             #print(parsed_input)
-            raise SyntaxError('invalid syntax (<file>, line '+str(line)+')\nUnknown place for }')
+            raise SyntaxError('invalid syntax (<file>, line '+ str(parseMemory[4]) +')\nunknown place for }')
         parseMemory[0]-=1
     
     parseMemory = parse_endl('\n',parseMemory,addline=False)
     return parseMemory
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_dot_coma.py` & `kagsa-1.2.0/kagsasrc/parse_paren.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-class ParseError (Exception):pass
 
-def __init__ (value,parseMemory):
-    # catch error
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+def __init__ (value, parseMemory):
+
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
-    # if |DATA-P| is empty : close it
+    if '|DATA_N|' in parseMemory[5]:
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete function sentence')
     if '|DATA-P|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA-P|','')
-    # if |DATA| found
     if '|DATA|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA|',f'{value}|DATA|')
-    #
-    elif ('|DATA1|' in parseMemory[5]) and (parseMemory[6] == False):
+    elif '|DATA0|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA0|',f'{value}|DATA0|')
-    # var items bar is opened
-    elif ('|DATA1|' in parseMemory[5]):
+    elif '|DATA1|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA1|',f'{value}|DATA1|')
     else:
-        raise ParseError(f'can\'t parsing (<file>, line {parseMemory[4]})')
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown place of paren')
     
     return parseMemory
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_endl.py` & `kagsa-1.2.0/kagsasrc/parse_endl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,64 @@
+
 def __init__ (value,parseMemory,addline=True):
+
     # catch some error
-    if ('while |DATA| :' in parseMemory[5]) :
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete while sentence')
-    if ('for |DATA| :' in parseMemory[5]) :
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete for sentence')
-    if ('if |DATA| :' in parseMemory[5]) :
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete if sentence')
-    if ('elif |DATA| :' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete elseif sentence')
-    if ('class |DATA-P| :' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete class sentence')
-    if ('def ' in parseMemory[5]) and('|DATA_N|' in parseMemory[5]) :
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete function sentence')
-    if  ('else' in parseMemory[5]) and not('else :' == parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown error in else sentence')
-    if ('except' in parseMemory[5]) and not('except Exception as ERROR :' == parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown error in catch sentence')
-    if ('try' in parseMemory[5]) and not('try :' == parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown error in try sentence')
-    if ('break' in parseMemory[5]) and not('break' == parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown error in break')
-    if ('continue' in parseMemory[5]) and not('continue' == parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown error in continue')
-    if ('|DATA0|' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete var sentence')
-    if ('= |DATA1|' in parseMemory[5]) or ((parseMemory[6] == False) and ('|DATA1|' in parseMemory[5])):
-        #print(parseMemory)
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete var sentence')
+    # ( "|DATA|" , " |DATA|" ) Space before |..| means there is nothing added to data
+
+    # while + for + if + elseif
+    co_in_end = ('True ' in parseMemory[5]) or ('False ' in parseMemory[5]) or ('or ' in parseMemory[5]) or ('and ' in parseMemory[5]) or ('in ' in parseMemory[5])
+    if (' |DATA|' in parseMemory[5]) and not(co_in_end) and (parseMemory[7] in ['while','for','if','elseif']) :
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\n{parseMemory[7]} sentence is not completed')
+    
+    # class + global + delvar
+    if ('|DATA-P|' in parseMemory[5]) and (parseMemory[7] in ['class','global','delvar']):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\n{parseMemory[7]} sentence is not completed')
+    
+    # func name
+    if (parseMemory[7] == 'func') and('|DATA_N|' in parseMemory[5]) :
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nfunction sentence is not completed')
+    
+    # else + try + catch
+    if  (parseMemory[7] in ['else','try','catch']) and not(f'{parseMemory[7]} :'.replace('catch','except Exception as ERROR') == parseMemory[5]):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nunknown error in {parseMemory[7]} sentence')
+    
+    # break + continue
+    if (parseMemory[5] in ['break','continue']) and not(parseMemory[7] == parseMemory[5]):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nunknown error in {parseMemory[7]}')
+    
+    # variable sentence
+    var_has_not_items = ('= |DATA1|' in parseMemory[5]) or ('= str(|DATA1|' in parseMemory[5]) or ('= int(|DATA1|' in parseMemory[5]) or ('= float(|DATA1|' in parseMemory[5]) or ('= json.loads(|DATA1|' in parseMemory[5]) or ('= list(|DATA1|' in parseMemory[5])
+       # variable didn't named yet                   # is var has an items     # var assign didn't writted
+    if (parseMemory[5].startswith('|DATA0|')) or      var_has_not_items     or (not(parseMemory[6]) and ('|DATA1|' in parseMemory[5])):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nvariable sentence is not completed')
+    
+
     if ('print(|DATA|,end=None)' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete write sentence')
-    if ('global |DATA-P|' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete global sentence')
-    if ('del |DATA-P|' in parseMemory[5]):
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete delvar sentence')
+        parseMemory[5] = parseMemory[5].replace('|DATA|','\n')
+    
     
 
     if parseMemory[1]:  # if There a Holder Add a new Block
         parseMemory[0]+=1
     parseMemory[1]=False
     parseMemory[6]=False
     # if There a Keyword Use a Code Block :
     # Add Line items to 'last_under_cmnd'
-    if parseMemory[5].startswith('while') or parseMemory[5].startswith('for') or parseMemory[5].startswith('if') or parseMemory[5].startswith('elseif') or parseMemory[5].startswith('else') or parseMemory[5].startswith('def') or parseMemory[5].startswith('class') or parseMemory[5].startswith('try') or parseMemory[5].startswith('except') :
+    if (parseMemory[7]==('while')) or parseMemory[7]==('for') or parseMemory[7]==('if') or parseMemory[7]==('elseif') or parseMemory[7]==('else') or parseMemory[7]==('def') or parseMemory[7]==('class') or parseMemory[7]==('try') or parseMemory[7]==('except') :
         parseMemory[2]=str(parseMemory[5])
     # Delete Somthings
     TheData= parseMemory[5].replace('|DATA|','').replace('|DATA1|','').replace('|DATA0|','').replace('|DATA-P|','').replace('|DATA_N|','')
+    n=0
+    for i in parseMemory[8]:
+        TheData=TheData.replace(f'"[{n}]"',i)
+        n+=1
     # Create Comment of The Kagsa Line in Python (this help to get the error from the compiler)
     if TheData.replace('\t','') !='':
         parseMemory[3].append('\t'*parseMemory[0] + TheData + f'    # line {parseMemory[4]}')
     parseMemory[5]='' # Clean Line items
+    parseMemory[7]='' # Clean Command Type
+    parseMemory[8]=[] # Clean Line Strings
     if addline:
         if value!=';':
             parseMemory[4]+=1 # Add New Line
 
     return parseMemory
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_id.py` & `kagsa-1.2.0/kagsasrc/parse_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 class ParseError (Exception):pass
 
 def __init__ (value,parseMemory):
+
     # Catch Error
-    if 'else :' in parseMemory[5]: # else can't take ID after
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]: # catch can't take ID after
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]: # try can't take ID after
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
     # Replace All The Symbols in The Var Name : @$^~:?
     value = value.replace('@','أ').replace('$','ب').replace('^','ت').replace('~','ث').replace('?','ج')
     
     # Variables that more than 1 Length :
     # my_name   or   my_age
     if (len(value)>2) or (len(value)==2 and not(value.startswith('#'))):
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_math.py` & `kagsa-1.2.0/kagsasrc/parse_math.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+
 def __init__ (value,parseMemory):
+
     value=value.replace(' ','')
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
     if '|DATA-P|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA-P|','')
     elif '|DATA|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA|',f'{value}|DATA|')
     elif ('|DATA1|' in parseMemory[5]) and (parseMemory[6] == False):
             raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nVariable opened without assign')
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_number.py` & `kagsa-1.2.0/kagsasrc/parse_number.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+class ParseError (Exception):pass
+
+
 def __init__ (value,parseMemory):
-    # catch errors
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
 
+    # catch errors
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
+    
     if value.replace('0','') != '':
         while True:
             if value.startswith('0'):
                 value = value[1:]
             else:
                 break
         if value=='':
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_paren.py` & `kagsa-1.2.0/kagsasrc/parse_dot_coma.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-def __init__ (value, parseMemory):
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+class ParseError (Exception):pass
+
+def __init__ (value,parseMemory):
+
+    # catch error
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
-    if '|DATA_N|' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nComplete function sentence')
+    # if |DATA-P| is empty : close it
     if '|DATA-P|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA-P|','')
+    # if |DATA| found
     if '|DATA|' in parseMemory[5]:
         parseMemory[5]=parseMemory[5].replace('|DATA|',f'{value}|DATA|')
-    elif '|DATA0|' in parseMemory[5]:
+    #
+    elif ('|DATA1|' in parseMemory[5]) and (parseMemory[6] == False):
         parseMemory[5]=parseMemory[5].replace('|DATA0|',f'{value}|DATA0|')
-    elif '|DATA1|' in parseMemory[5]:
+    # var items bar is opened
+    elif ('|DATA1|' in parseMemory[5]):
         parseMemory[5]=parseMemory[5].replace('|DATA1|',f'{value}|DATA1|')
     else:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nUnknown place of paren')
+        raise ParseError(f'can\'t parsing (<file>, line {parseMemory[4]})')
     
     return parseMemory
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_sformat.py` & `kagsa-1.2.0/kagsasrc/parse_sformat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .lexer import main as Lexer
 from .paths import Paths as Paths
 import re
 
-Paths.init()
 
 def __init__ (value):
     parse_string = Paths.getFile('parse_string.py','r').read().replace('from .parse_sformat import __init__ as parse_sformat','')
     space = dict(
         parse_sformat=globals()['__init__'],
         **globals()
     )
```

### Comparing `kagsa-1.1.1/kagsasrc/parse_string.py` & `kagsa-1.2.0/kagsasrc/parse_string.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .parse_id import __init__ as parse_id
 from .parse_sformat import __init__ as parse_sformat
 import re
+class ParseError (Exception) :pass
 
 def __init__ (value,parseMemory):
-    if 'else :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to else command')
-    if 'except Exception as ERROR :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to catch command')
-    if 'try :' in parseMemory[5]:
-        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\nCan\'t add any arguments to try command')
+
+    if (parseMemory[7] == 'else'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to else command')
+    if (parseMemory[7] == 'catch'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to catch command')
+    if (parseMemory[7] == 'try'):
+        raise SyntaxError(f'invalid syntax (<file>, line {parseMemory[4]})\ncan\'t add any arguments to try command')
     
     # parse the string that have more than 1 line
     if value.startswith('``'):
         value='"""'+value[2:-2]+'"""'
         parseMemory[4]+=value.count('\n')
     
     # Check Formats
@@ -23,22 +25,23 @@
             # d[0] : %{..}
             # d[1] :   ..
             format_id = parse_sformat(d[1])
             NEW='{'+format_id+'}'
             value=value.replace(d[0],NEW)
     
     value=value.replace('STR_SYM_ONE',"\\'").replace('STR_SYM_TWO','\\"')
-
+    string_idx = len(parseMemory[8])
     if '|DATA-P|' in parseMemory[5]:
-        parseMemory[5]=parseMemory[5].replace('|DATA-P|',value)
+        parseMemory[5]=parseMemory[5].replace('|DATA-P|',f'"[{string_idx}]"')
     elif '|DATA|' in parseMemory[5]:
-        parseMemory[5]=parseMemory[5].replace('|DATA|',f'{value}|DATA|')
+        parseMemory[5]=parseMemory[5].replace('|DATA|',f'"[{string_idx}]"|DATA|')
     elif ('|DATA0|' in parseMemory[5]):
-        parseMemory[5]=parseMemory[5].replace('|DATA0|',f'{value}|DATA0|')
+        parseMemory[5]=parseMemory[5].replace('|DATA0|',f'"[{string_idx}]"|DATA0|')
     elif ('|DATA1|' in parseMemory[5]):
-        parseMemory[5]=parseMemory[5].replace('|DATA1|',f'{value}|DATA1|')
+        parseMemory[5]=parseMemory[5].replace('|DATA1|',f'"[{string_idx}]"|DATA1|')
     elif parseMemory[5]=='':
-        parseMemory[5]+=f'{value}|DATA|'
+        parseMemory[5]+=f'"[{string_idx}]"|DATA|'
     else:
         raise ParseError(f'can\'t parsing (<file>, line {parseMemory[4]})')
+    parseMemory[8].append(value)
     #print(parseMemory[5])
     return parseMemory
```

### Comparing `kagsa-1.1.1/kagsasrc/parser.py` & `kagsa-1.2.0/kagsasrc/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 from .parse_endl import __init__ as parse_endl
 from .parse_cmnt import __init__ as parse_cmnt
 from .parse_keyword import __init__ as parse_keyword
 from .parse_id import __init__ as parse_id
 from .parse_dot_coma import __init__ as parse_dot_coma
 from .parse_number import __init__ as parse_number
 from .parse_assign import __init__ as parse_assign
@@ -12,21 +11,23 @@
 from .parse_cparen import __init__ as parse_cparen
 from .parse_co import __init__ as parse_co
 
 class ParseError (Exception) :pass
 
 def main (data):
     parseMemory = [
-        0,     # under_codes        : [0] : Current Codes Blocks (Tab)
-        False, # under_codes_holder : [1] : Holder to get a New Block ('if' ,'else' ,'while')
-        '',    # last_under_cmnd    : [2] : The Holder Value
-        [],    # parsed_input       : [3] : All The Translated Python Codes (list)
-        1,     # line               : [4] : The Current Line (used to print in errors)
-        '',    # line_items         : [5] : The Line Items (its will be edit and add it to 'parsed_input')
-        False  # variable close     : [6] : Is The Variable Assign Closed ?
+        0,       # under_codes        : [0] : Current Codes Blocks (Tab)
+        False,   # under_codes_holder : [1] : Holder to get a New Block ('if' ,'else' ,'while')
+        '',      # last_under_cmnd    : [2] : The Holder Value
+        [],      # parsed_input       : [3] : All The Translated Python Codes (list)
+        1,       # line               : [4] : The Current Line (used to print in errors)
+        '',      # line_items         : [5] : The Line Items (its will be edit and add it to 'parsed_input')
+        False,   # variable close     : [6] : Is The Variable Assign Writted ?
+        '',      # command type       : [7] : The Type of the Command in The Line (write,var,int,try)
+        []       # strings            : [8] : All The Strings That Used in The Line
     ]
     for key,value in data:          # Read All The Lexed Data ( [['key','value']..] )
         if    key == 'ENDLINE':
             parseMemory = parse_endl(value,parseMemory)
         elif  key == 'COMMENT':
             parseMemory = parse_cmnt(value,parseMemory)
         elif  key == 'KEYWORD':
```

### Comparing `kagsa-1.1.1/kagsasrc/paths.py` & `kagsa-1.2.0/kagsasrc/libtemplate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-import pkg_resources,os,sys
-
-# from .paths import Paths as Paths
-# Paths.init()
-# Paths.getFile(  )
+# import some modules for "exec_data"
+import re,os,sys,traceback,zipfile
 
+# add "kagsasrc" path to "sys.path"
 class Paths:
-    AsPackage = True
-    if getattr(sys, 'frozen', False):
-        __path__ = os.path.dirname(sys.executable)
-    # or a script file (e.g. `.py` / `.pyw`)
-    elif __file__:
-        __path__ = os.path.dirname(__file__)
+    def __path__ ():
+        if getattr(sys, 'frozen', False):
+            return os.path.dirname(sys.executable)
+        # or a script file (e.g. `.py` / `.pyw`)
+        elif __file__:
+            return os.path.dirname(__file__)
 
     def init () :
-        if not(Paths.AsPackage):
-            sys.path.append( os.getcwd() )
-            sys.path.append( __path__ )
+        sys.path.insert(1, os.getcwd() )
+        sys.path.insert(1, Paths.__path__() )
 
     def getFile (filen,mode):
-        if Paths.AsPackage:
+        '''if Paths.AsPackage:
             pkg_path = os.path.dirname( pkg_resources.resource_stream(__name__,'errors.py').name ) + os.sep
             return open(pkg_path + filen,mode,encoding='utf-8')
         else:
-            return open( __path__ + os.sep + filen, mode , encoding='utf-8')
+            return open( Paths.__path__() + os.sep + filen, mode , encoding='utf-8')'''
+        return open( Paths.__path__() + os.sep + filen, mode , encoding='utf-8')
+
+
+#os.path.append(os.path.dirname( Paths.__path__() ))
+
+from errors import __init__ as errors
+from parse_id import __init__ as parse_id
+from built_modules import *
+from methods import *
 
 
-#pkg_resources.resource_stream(__name__,'built_modules.py').read().decode('utf-8')
```

### Comparing `kagsa-1.1.1/kagsasrc/syntax_checker.py` & `kagsa-1.2.0/kagsasrc/syntax_checker.py`

 * *Files identical despite different names*

### Comparing `kagsa-1.1.1/setup.py` & `kagsa-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from setuptools import setup, find_packages
 
 __name__ = "kagsa"
-__version__ = "1.1.1"
-__author__ = "Kagsa Programming Language"
-__author_email__ = "kagsa.programming.lang@gmail.com"
-__date__ = "2022-9-10"
+__version__ = "1.2.0"
+__author__ = "KAGSA PROGRAMMING LANGUAGE"
+__author_email__ = "admin@kagsa.org"
+__date__ = "2023-6-6"
 
 
 readme = open("README.md", "r", encoding="utf-8")
 long_description =  readme.read()
 reqFile=open("requirements.txt", "r")
 requirements = reqFile.read().split('\n')
 
 readme.close()
 reqFile.close()
 
 setup(
     name=__name__,
     version=__version__,
-    description='Programming Language',
+    description='PROGRAMMING LANGUAGE',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='http://www.kagsa.org/',
+    url='https://www.kagsa.org/',
     author=__author__,
     author_email=__author_email__,
 
     project_urls={
       'Source': 'https://github.com/kagsa/kagsa',
       'Report Bugs': 'https://github.com/kagsa/kagsa/issues',
       'Download': 'https://pypi.org/project/kagsa/#files',
       'Documentation': 'https://github.com/kagsa/kagsa/blob/master/README.md',
-      'Website' : 'http://kagsa.org/'
+      'Website' : 'https://www.kagsa.org/'
     },
 
     license='MIT',
 
     keywords=[
         'programming', 'language', 'programming language',
         'kagsa', 'lang', 'kg', 'KG', 'KAGSA'
```

