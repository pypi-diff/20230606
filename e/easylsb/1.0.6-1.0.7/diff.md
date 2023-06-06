# Comparing `tmp/easylsb-1.0.6.tar.gz` & `tmp/easylsb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.6.tar", last modified: Tue Jun  6 06:28:45 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.7.tar", last modified: Tue Jun  6 07:05:58 2023, max compression
```

## Comparing `easylsb-1.0.6.tar` & `easylsb-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:28:45.000000 easylsb-1.0.6/
--rw-rw-rw-   0        0        0     1259 2023-06-06 06:28:45.000000 easylsb-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-06-06 06:28:23.000000 easylsb-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 06:28:45.000000 easylsb-1.0.6/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1259 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-06 06:28:45.000000 easylsb-1.0.6/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 06:28:44.000000 easylsb-1.0.6/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13569 2023-06-06 06:21:21.000000 easylsb-1.0.6/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-06 06:28:45.000000 easylsb-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-06-06 06:28:41.000000 easylsb-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:05:58.000000 easylsb-1.0.7/
+-rw-rw-rw-   0        0        0     1745 2023-06-06 07:05:58.000000 easylsb-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-06-06 07:05:31.000000 easylsb-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15819 2023-06-06 06:56:54.000000 easylsb-1.0.7/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:05:58.000000 easylsb-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-06-06 06:57:12.000000 easylsb-1.0.7/setup.py
```

### Comparing `easylsb-1.0.6/PKG-INFO` & `easylsb-1.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
-
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
@@ -29,8 +28,29 @@
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 img=np.array(img)
 info=lsb.lsbdec(img)
 print(info)
 ```
-It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES.
+#### RSA
+
+RSA is now supported in easylsb 1.0.7.
+Code:
+```python
+import lsb
+from PIL import Image
+import numpy as np
+import rsa
+pub,priv=rsa.newkeys(200)
+img=Image.open('test.png')
+img=np.array(img)
+info=b'Some information'
+# Hide
+hidden=lsb.lsbenc(img,info,rsakey=pub)
+img_hidden=Image.fromarray(hidden)
+img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
+# Recover
+info=lsb.lsbdec(hidden,rsakey=priv)
+print(info)# b'Some information'
+```
+It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
```

### Comparing `easylsb-1.0.6/README.md` & `easylsb-1.0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
-
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
@@ -23,8 +22,29 @@
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 img=np.array(img)
 info=lsb.lsbdec(img)
 print(info)
 ```
-It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES.
+#### RSA
+
+RSA is now supported in easylsb 1.0.7.
+Code:
+```python
+import lsb
+from PIL import Image
+import numpy as np
+import rsa
+pub,priv=rsa.newkeys(200)
+img=Image.open('test.png')
+img=np.array(img)
+info=b'Some information'
+# Hide
+hidden=lsb.lsbenc(img,info,rsakey=pub)
+img_hidden=Image.fromarray(hidden)
+img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
+# Recover
+info=lsb.lsbdec(hidden,rsakey=priv)
+print(info)# b'Some information'
+```
+It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
```

### Comparing `easylsb-1.0.6/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.7/easylsb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
-
 Code to hide information in the given image:
 ```python
 import lsb
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')
 img=np.array(img)
@@ -29,8 +28,29 @@
 from PIL import Image
 import numpy as np
 img=Image.open('test.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 img=np.array(img)
 info=lsb.lsbdec(img)
 print(info)
 ```
-It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES.
+#### RSA
+
+RSA is now supported in easylsb 1.0.7.
+Code:
+```python
+import lsb
+from PIL import Image
+import numpy as np
+import rsa
+pub,priv=rsa.newkeys(200)
+img=Image.open('test.png')
+img=np.array(img)
+info=b'Some information'
+# Hide
+hidden=lsb.lsbenc(img,info,rsakey=pub)
+img_hidden=Image.fromarray(hidden)
+img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
+# Recover
+info=lsb.lsbdec(hidden,rsakey=priv)
+print(info)# b'Some information'
+```
+It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
```

### Comparing `easylsb-1.0.6/lsb.py` & `easylsb-1.0.7/lsb.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from platform import system as _t
 from uuid import uuid4 as _8
 import os as _os
 import des as _d
 from base64 import b64encode as _b, b64decode as _bd
 from hashlib import md5 as _m
 from chardet import detect
-
+import rsa as _rsa
 def _4(*args, **kwargs):
     return str(_8(*args, **kwargs))
 
 
 try:
     import tkinter as _tk
 except:
@@ -80,29 +80,33 @@
     return (
         ([x >> 5, (x >> 2) & 7, x & 3], 3)
         if not dec
         else sum([x[i] << ([5, 2, 0][i]) for i in range(len([5, 2, 0]))])
     )
 
 
-def lsbenc(img, text, mode=mode_lsb1, key=b""):
+def lsbenc(img, text, mode=mode_lsb1, key=b"",rsakey=None):
     """
     Image steganography encryption
     :param img: Input image (as Numpy array)
     :param text: Text to hide (encoded as bytes)
     :param mode: Mode (lsb1,lsb2,lsb3)
     :param key: DES key (Optional)
+    :param rsakey: RSA public key (Optional)
     :return: Image with text hidden
     """
     if key:
         hasher = _m()
         hasher.update(key)
         md5_result = hasher.digest()
         des = _d.DesKey(md5_result)
         text = _b(des.encrypt(text, padding=True))
+    if rsakey:
+        text=_rsa.encrypt(text,rsakey)
+        text= _b(text)
     text += b"\0"
     bit = bytes(img)
     result = b""
     it = 0
     for i in text:
         res = mode(i, False)
         bits = res[1]
@@ -111,57 +115,65 @@
             result += bytes([((bit[it] >> bits) << bits) | data[j]])
             it += 1
     result += bit[it:]
     resulta = _r(_f(result, dtype=_u), newshape=img.shape)
     return resulta
 
 
-def lsbdec(img, mode=mode_lsb1, key=b""):
+def lsbdec(img, mode=mode_lsb1, key=b"",rsakey=None):
     """
     Image steganography encryption
     :param img:Input image (as Numpy array)
     :param mode:Mode (lsb1,lsb2,lsb3)
     :param key: DES key (Optional)
+    :param rsakey: RSA private key (Optional)
     :return:Text hidden in image (as bytes)
     """
     bits = len(mode(0, False)[0])
     res = b""
     bit = bytes(img)
     it = 0
     while 1:
         l = [f & ((1 << mode(0, False)[-1]) - 1) for f in bit[it : it + bits]]
         if not mode(l, True):
+            if rsakey:
+                res=_bd(res)
+                res=_rsa.decrypt(res,rsakey)
             if key:
                 hasher = _m()
                 hasher.update(key)
                 md5_result = hasher.digest()
                 des = _d.DesKey(md5_result)
                 res = des.decrypt(_bd(res), padding=True)
             return res
         res += bytes([mode(l, True)])
         it += bits
 
 
-def lsbenc_audio(audio, text, ofile, framerate=None, mode=mode_lsb1, key=b""):
+def lsbenc_audio(audio, text, ofile, framerate=None, mode=mode_lsb1, key=b"",rsakey=None):
     """
     Audio steganography encryption
     :param audio: Input audio (as wave.Wave_read object)
     :param text: Text to hide (encoded as bytes)
-    :param ofile:Output file name
+    :param ofile: Output file name
     :param framerate:Output file framerate
     :param mode: Mode (lsb1,lsb2,lsb3)
     :param key: DES key (Optional)
+    :param rsakey: RSA public key (Optional)
     :return: None
     """
     if key:
         hasher = _m()
         hasher.update(key)
         md5_result = hasher.digest()
         des = _d.DesKey(md5_result)
         text = _b(des.encrypt(text, padding=True))
+    if rsakey:
+        text=_rsa.encrypt(text,rsakey)
+        text= _b(text)
     text += b"\0"
     nf = audio.getnframes()
     ad = audio.readframes(nf)
     bit = list(_f(ad, dtype=_s))
     result = []
     it = 0
     for i in text:
@@ -186,30 +198,34 @@
     wf.setsampwidth(audio.getsampwidth())
     wf.setnchannels(1)
     wf.writeframes(bt)
     if not bak.endswith(".wav"):
         _os.system('ffmpeg -i "' + ofile + '" "' + bak + '"')
 
 
-def lsbdec_audio(audio, mode=mode_lsb1, key=b""):
+def lsbdec_audio(audio, mode=mode_lsb1, key=b"",rsakey=None):
     """
     Audio steganography decryption
     :param audio:Input audio (as wave.Wave_read object)
     :param mode:Mode (lsb1,lsb2,lsb3)
     :param key: DES key (Optional)
+    :param rsakey: RSA private key (Optional)
     :return:Text hidden in audio (as bytes)
     """
     bits = len(mode(0, False)[0])
     res = b""
     nf = audio.getnframes()
     bit = list(_f(audio.readframes(nf), dtype=_s))
     it = 0
     while 1:
         l = [f & ((1 << mode(0, False)[-1]) - 1) for f in bit[it : it + bits]]
         if not mode(l, True):
+            if rsakey:
+                res=_bd(res)
+                res=_rsa.decrypt(res,rsakey)
             if key:
                 hasher = _m()
                 hasher.update(key)
                 md5_result = hasher.digest()
                 des = _d.DesKey(md5_result)
                 res = des.decrypt(_bd(res), padding=True)
             return res
@@ -232,14 +248,16 @@
     parser.add_argument("-e", "--encoding", help="Encoding of text, default is 'ascii'", default="ascii")
     parser.add_argument("-o", "--output", help="Output file name, if the output file name is not configured, the output image will be shown in a Tkinter window")
     parser.add_argument(
         "-m", "--mode", help="mode (lsb1,lsb2,lsb3), default is lsb1", default="lsb1"
     )
     parser.add_argument("-k", "--key", help="DES Key (Optional)", default="")
     parser.add_argument("-a","--auto",help="Automatically detect the encoding of the text in decrypt mode",action='store_true')
+    parser.add_argument("-r", "--rsa",
+                        help="Use RSA to encrypt the text\nIf in encrypt mode, the program will create pub_(RSA).pem and priv_(RSA).pem\nIf in decrypt mode, the program will read the private key stored (RSA).pem")
     parser.add_argument("image", help="Input image")
     args = parser.parse_args()
     img = _i.open(args.image)
     if args.mode == "lsb1":
         mode = mode_lsb1
     elif args.mode == "lsb2":
         mode = mode_lsb2
@@ -248,19 +266,28 @@
     else:
         print("unknown mode: ", args.mode)
         return -1
     if args.operation == "e":
         if args.auto:
             print('--auto should only be used in decrypt mode.')
         if args.text:
+            if args.rsa:
+                pubkey, privkey = _rsa.newkeys(200)
+                with open('pub_' + args.rsa + '.pem', 'wb') as f:
+                    f.write(pubkey.save_pkcs1())
+                with open('priv_' + args.rsa + '.pem', 'wb') as f:
+                    f.write(privkey.save_pkcs1())
+            else:
+                pubkey = None
             enc = lsbenc(
                 _a(img),
                 args.text.encode(args.encoding),
                 mode=mode,
                 key=args.key.encode(args.encoding),
+                rsakey=pubkey
             )
             if args.output:
                 pilimg = _i.fromarray(enc)
                 pilimg.save(args.output)
             else:
                 if not tk_support:
                     print("The Python environment does not support Tkinter, so the image cannot be shown")
@@ -279,16 +306,21 @@
             print("Text to hide is not configured")
             return -1
     elif args.operation == "d":
         if args.text or args.output:
             print("Input text and output file should not be configured in decrypt mode")
             return -1
         else:
+            if args.rsa:
+                with open(args.rsa + '.pem', 'rb') as f:
+                    privkey = _rsa.PrivateKey.load_pkcs1(f.read())
+            else:
+                privkey = None
             img = _i.open(args.image)
-            dec = lsbdec(_a(img), mode=mode, key=args.key.encode(args.encoding))
+            dec = lsbdec(_a(img), mode=mode, key=args.key.encode(args.encoding),rsakey=privkey)
             if args.auto:
                 encoding=detect(dec)
             else:
                 encoding=args.encoding
             print(dec.decode(encoding))
     else:
         print("unkown operation: ", args.operation)
@@ -305,14 +337,15 @@
         "-m", "--mode", help="mode (lsb1,lsb2,lsb3), default is lsb1", default="lsb1"
     )
     parser.add_argument("-f", "--framerate", help="frame rate of output audio")
     parser.add_argument("-b", "--progressbar", help="Display progress bar when playing", action="store_true")
     parser.add_argument("-k", "--key", help="DES Key (Optional)", default="")
     parser.add_argument("-a", "--auto", help="Automatically detect the encoding of the text in decrypt mode",
                         action='store_true')
+    parser.add_argument("-r","--rsa",help="Use RSA to encrypt the text\nIf in encrypt mode, the program will create pub_(RSA).pem and priv_(RSA).pem\nIf in decrypt mode, the program will read the private key stored (RSA).pem")
     parser.add_argument("audio", help="Input audio")
     args = parser.parse_args()
     if args.mode == "lsb1":
         mode = mode_lsb1
     elif args.mode == "lsb2":
         mode = mode_lsb2
     elif args.mode == "lsb3":
@@ -320,14 +353,22 @@
     else:
         print("unknown mode: ", args.mode)
         return -1
     if args.operation == "e":
         if args.auto:
             print('--auto should only be used in decrypt mode.')
             return -1
+        if args.rsa:
+            pubkey,privkey=_rsa.newkeys(200)
+            with open('pub_'+args.rsa+'.pem','wb') as f:
+                f.write(pubkey.save_pkcs1())
+            with open('priv_'+args.rsa+'.pem','wb') as f:
+                f.write(privkey.save_pkcs1())
+        else:
+            pubkey=None
         if args.text:
             if args.audio.endswith(".wav"):
                 wav = wave.open(args.audio)
             else:
                 p = _os.path.join(_tmp(), _4() + ".wav")
                 _os.system('ffmpeg -i "' + args.audio + '" "' + p + '"')
                 wav = wave.open(p)
@@ -335,14 +376,15 @@
             lsbenc_audio(
                 wav,
                 args.text.encode(args.encoding),
                 _os.path.join(_tmp(), p) if not args.output else args.output,
                 framerate=int(args.framerate) if args.framerate else None,
                 mode=mode,
                 key=args.key.encode(args.encoding),
+                rsakey=pubkey
             )
             if not args.output:
                 if not pyaudio_support:
                     print("Cannot play the audio because PyAudio is not installed, you can install it via the 'pip install PyAudio' command")
                     return -1
                 else:
                     pa = _p.PyAudio()
@@ -370,16 +412,21 @@
         else:
             print("Text to hide is not configured")
             return -1
     elif args.operation == "d":
         if args.text or args.output or args.progressbar or args.framerate:
             print("Text, output file, progress bar and frame rate should not be configured in decrypt mode")
             return -1
+        if args.rsa:
+            with open(args.rsa+'.pem','rb') as f:
+                privkey=_rsa.PrivateKey.load_pkcs1(f.read())
+        else:
+            privkey=None
         wav = wave.open(args.audio)
-        dec = lsbdec_audio(wav, mode, key=args.key.encode(args.encoding))
+        dec = lsbdec_audio(wav, mode, key=args.key.encode(args.encoding),rsakey=privkey)
         if args.auto:
             encoding=detect(dec)['encoding']
         else:
             encoding=args.encoding
         print(dec.decode(encoding))
     else:
         print("Unknown operation: ", args.operation)
```

