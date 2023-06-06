# Comparing `tmp/jax-tools-1.0.32.tar.gz` & `tmp/jax-tools-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.32.tar", last modified: Fri Jun  2 08:48:37 2023, max compression
+gzip compressed data, was "jax-tools-1.0.47.tar", last modified: Tue Jun  6 03:59:01 2023, max compression
```

## Comparing `jax-tools-1.0.32.tar` & `jax-tools-1.0.47.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.616229 jax-tools-1.0.32/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-02 08:48:37.615968 jax-tools-1.0.32/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.32/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.611276 jax-tools-1.0.32/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.32/jax_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6222 2023-06-01 10:53:38.000000 jax-tools-1.0.32/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4387 2023-06-02 06:44:22.000000 jax-tools-1.0.32/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1733 2023-06-02 06:47:01.000000 jax-tools-1.0.32/jax_tools/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.32/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3385 2023-06-02 07:27:14.000000 jax-tools-1.0.32/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.32/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2780 2023-06-02 08:47:19.000000 jax-tools-1.0.32/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.615294 jax-tools-1.0.32/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.32/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.32/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 08:48:37.614236 jax-tools-1.0.32/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      453 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       92 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       66 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-02 08:48:37.000000 jax-tools-1.0.32/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-02 08:48:37.616323 jax-tools-1.0.32/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1712 2023-06-02 08:48:36.000000 jax-tools-1.0.32/setup.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.905187 jax-tools-1.0.47/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-06 03:59:01.904931 jax-tools-1.0.47/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.47/README.md
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.872582 jax-tools-1.0.47/jax_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.47/jax_tools/__init__.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.884536 jax-tools-1.0.47/jax_tools/cmd/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.47/jax_tools/cmd/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.47/jax_tools/cmd/jax.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.47/jax_tools/cmd/jax_encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.47/jax_tools/cmd/jax_fix.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.47/jax_tools/cmd/jax_nd.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1724 2023-06-06 03:38:17.000000 jax-tools-1.0.47/jax_tools/cmd/jax_pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.47/jax_tools/cmd/nd.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.902804 jax-tools-1.0.47/jax_tools/cmd_tools/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.47/jax_tools/cmd_tools/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4526 2023-06-06 03:38:17.000000 jax-tools-1.0.47/jax_tools/cmd_tools/pam.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     6223 2023-06-06 03:32:23.000000 jax-tools-1.0.47/jax_tools/colorful_font.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.47/jax_tools/encrypt.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1919 2023-06-01 08:32:18.000000 jax-tools-1.0.47/jax_tools/logger.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.47/jax_tools/network_test.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      651 2023-06-02 07:00:58.000000 jax-tools-1.0.47/jax_tools/proxies.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     2772 2023-06-06 03:34:47.000000 jax-tools-1.0.47/jax_tools/ssh.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.904528 jax-tools-1.0.47/jax_tools/utils/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.47/jax_tools/utils/__init__.py
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.47/jax_tools/utils/settings.py
+drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 03:59:01.877754 jax-tools-1.0.47/jax_tools.egg-info/
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      657 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)      224 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       83 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/requires.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-06-06 03:59:01.000000 jax-tools-1.0.47/jax_tools.egg-info/top_level.txt
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-06-06 03:59:01.905273 jax-tools-1.0.47/setup.cfg
+-rw-r--r--   0 cyber.anonym   (501) staff       (20)     1963 2023-06-06 03:59:01.000000 jax-tools-1.0.47/setup.py
```

### Comparing `jax-tools-1.0.32/PKG-INFO` & `jax-tools-1.0.47/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.32
+Version: 1.0.47
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.32/README.md` & `jax-tools-1.0.47/README.md`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.32/jax_tools/colorful_font.py` & `jax-tools-1.0.47/jax_tools/colorful_font.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -235,8 +235,8 @@
     print(ColorFont.colorful_text(ColorFont.STYLE_NORMAL, GetColor.score(6.5), '6.5 score'))
     print(bold_msg(GetColor.score(2.5), '2.5 score'))
     print(bold_msg(GetColor.date('2020-01-01'), '2020-01-01'))
     print(bold_msg(GetColor.date('2023-01-01'), '2023-01-01'))
     print(bold_msg(GetColor.date('2019-01-01'), '2019-01-01'))
     print(Yellow('hello'))
     print(Yellow.text('hello'))
-    print(Red.bold('hello'))
+    print(Red.bold('hello'))
```

### Comparing `jax-tools-1.0.32/jax_tools/encrypt.py` & `jax-tools-1.0.47/jax_tools/encrypt.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,46 @@
 from Crypto.Cipher import AES
 from base64 import b64encode
 from base64 import b64decode
 from Crypto.Util.Padding import pad, unpad
 from jax_tools.utils import settings as st
 
 
+def get_local_key():
+    """
+    Ensure that the encryption key exists locally, if not, generate a new one
+    Returns:
+
+    """
+    if os.path.exists(st.JAX_KEY_FILE):
+        encryption_key = open(st.JAX_KEY_FILE, 'r').read().strip()
+        if len(encryption_key) != 32:
+            msg = 'encryption key length must be 32, please check file {} correct, or delete this file and try again.' \
+                .format(st.JAX_KEY_FILE)
+            print(msg)
+            exit(1)
+    else:
+        # generate encryption key
+        encryption_key = ''.join(secrets.choice(string.ascii_letters + string.digits) for _ in range(32))
+        if os.path.exists(st.JAX_DATA_DIR) is False:
+            os.mkdir(st.JAX_DATA_DIR)
+        with open(st.JAX_KEY_FILE, 'w') as f:
+            f.write(encryption_key)
+    return encryption_key
+
+
 class AESCipher(object):
     """
     AES Encryption Class, can use CBC or GCM mode, default is GCM mode
     You can use encrypt_body and decrypt_body to encrypt and decrypt request body
     You can use encrypt_content and decrypt_content to encrypt and decrypt content
     """
 
     # key for encrypting sensitive data
-    def __init__(self, key='temp_secret_key.', cbc_mode=False):
+    def __init__(self, key=get_local_key(), cbc_mode=False):
         """
         Init method
         Args:
             key: give a token  as a key use for encrypting request body
         """
         if len(key) > 32:
             # Get the key from key 8:24
@@ -93,15 +116,15 @@
                                                        * 2:self.length * 2 + (AES.block_size - self.length)])
         cipher_text = "{0}{1}".format(
             data[self.length: self.length * 2], data[self.length + AES.block_size:])
         cipher = AES.new(key, self.encryption_mode, iv.encode('utf-8'))
         try:
             plaintext = unpad(cipher.decrypt(b64decode(cipher_text)), AES.block_size).decode()
         except ValueError:
-            plaintext = 'Invalid token'
+            plaintext = 'Failed decrypt, please give a correct encrypted string'
         return plaintext
 
 
 def encrypt_hmac_sha256(plaintext, secret_key):
     """
     Use HMAC-SHA256 to do irreversible encryption, such as encrypting user passwords
 
@@ -118,27 +141,7 @@
         hmac.new(
             secret_key,
             plaintext,
             digestmod=hashlib.sha256).digest())
     return cipher_data.decode()
 
 
-def ensure_local_key_exists():
-    """
-    Ensure that the encryption key exists locally, if not, generate a new one
-    Returns:
-
-    """
-    if os.path.exists(st.JAX_KEY_FILE):
-        encryption_key = open(st.JAX_KEY_FILE, 'r').read().strip()
-        if len(encryption_key) != 32:
-            msg = 'encryption key length must be 32, please check file {} correct, or delete this file and try again.' \
-                .format(st.JAX_KEY_FILE)
-            print(msg)
-            exit(1)
-    else:
-        # generate encryption key
-        encryption_key = ''.join(secrets.choice(string.ascii_letters + string.digits) for _ in range(32))
-        if os.path.exists(st.JAX_DATA_DIR) is False:
-            os.mkdir(st.JAX_DATA_DIR)
-        with open(st.JAX_KEY_FILE, 'w') as f:
-            f.write(encryption_key)
```

### Comparing `jax-tools-1.0.32/jax_tools/jax_encrypt.py` & `jax-tools-1.0.47/jax_tools/cmd/jax_encrypt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # -*- coding:utf-8 -*-
 """
-JAX encryption service
+jax-encrypt cmd, provide encryption and decryption functions
 """
 import sys
 import os
 import argparse
-sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-from jax_tools.utils import settings as st
+# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 from jax_tools.encrypt import AESCipher
-from jax_tools.encrypt import ensure_local_key_exists
+from jax_tools.encrypt import get_local_key
+
 
 # Ensure the existence of the encryption key file
-ensure_local_key_exists()
-JAX_ENCRYPTION_KEY = open(st.JAX_KEY_FILE, 'r').read()
-JAX_ENCRYPT = AESCipher(JAX_ENCRYPTION_KEY).encrypt
-JAX_DECRYPT = AESCipher(JAX_ENCRYPTION_KEY).decrypt
+JAX_ENCRYPT = AESCipher().encrypt
+JAX_DECRYPT = AESCipher().decrypt
 
 
 def main():
     """
     main
     Returns:
 
@@ -30,16 +28,16 @@
     parser.add_argument('-k', '--key', type=str, default=None, help='Specifies the encryption key')
     parser.add_argument('-t', '--type', type=str, default='gcm', help='Specifies the encryption type, cbc or gcm')
     parser.add_argument('-v', '--version', action='version', version='1.0')
     options = parser.parse_args()
     if options.key is not None:
         key = options.key
     else:
-        key = JAX_ENCRYPTION_KEY
-    if options.type.__contains__('cbc'):
+        key = get_local_key()
+    if options.type.lower().__contains__('cbc'):
         cbc_mode = True
     else:
         cbc_mode = False
     if options.decrypt is not None:
         print(AESCipher(key, cbc_mode).decrypt(options.decrypt))
     if options.encrypt is not None:
         print(AESCipher(key, cbc_mode).encrypt(options.encrypt))
```

### Comparing `jax-tools-1.0.32/jax_tools/logger.py` & `jax-tools-1.0.47/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.32/jax_tools/network_test.py` & `jax-tools-1.0.47/jax_tools/network_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 Check if the target IP and port is open
 """
 import socket
 import sys
 from ping3 import ping
+from jax_tools.colorful_font import Green as green
+from jax_tools.colorful_font import Red as red
+from jax_tools.colorful_font import Yellow as yellow
 
 
 def check_icmp_connectivity(ip):
     """
     Check if the target IP is reachable
     Args:
         ip(str): IP address or hostname
@@ -63,35 +66,35 @@
         # 创建一个socket对象
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.settimeout(5)  # 设置超时时间（单位：秒）
         if isinstance(port, str):
             try:
                 port = int(port)
                 if port < 0 or port > 65535:
-                    print_msg("The port must be between 0 and 65535")
+                    print_msg(yellow("The port must be between 0 and 65535"))
                     sys.exit(1)
             except ValueError:
-                print_msg("The port must be a number")
+                print_msg(yellow("The port must be a number"))
                 sys.exit(1)
         # 尝试连接到目标IP和端口
         result = s.connect_ex((ip, port))
         if result == 0:
-            print_msg("Connection success")
+            print_msg(green.bold("Connection success"))
             result = True
         elif result in result_dict.keys():
             if check_icmp_connectivity(ip):
-                print_msg("Connection error: " + result_dict[result])
+                print_msg(red("Connection error: " + result_dict[result]))
             else:
-                print_msg("Connection error: " + result_dict[result] + "and ping not work")
+                print_msg(red("Connection error: " + result_dict[result] + "and ping not work"))
             result = False
         else:
-            print_msg("Connection error：" + str(result))
+            print_msg(red("Connection error：" + str(result)))
             result = False
     except socket.error as e:
-        print_msg("Connection error：" + e)
+        print_msg(red("Connection error：" + e))
         result = False
     finally:
         if s:
             s.close()
     return result
 
 
@@ -101,25 +104,11 @@
     """
     need_print = True
 
     def __init__(self, msg):
         """
         Init
         Args:
-            msg (str): Message to print
+            msg : Message to print
         """
         if self.need_print:
             print(msg)
-
-
-def main():
-    """
-    Main function
-    Returns:
-
-    """
-    if len(sys.argv) == 3:
-        target_ip = sys.argv[1]
-        target_port = int(sys.argv[2])
-        check_connectivity(target_ip, target_port, True)
-    else:
-        print("Usage: nd <TargetIP> <TargetPort>")
```

### Comparing `jax-tools-1.0.32/jax_tools/proxies.py` & `jax-tools-1.0.47/jax_tools/proxies.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.32/jax_tools/ssh.py` & `jax-tools-1.0.47/jax_tools/ssh.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     SSH Connector
     """
 
     def __init__(self, host, port, username, password) -> None:
         """
         SSH Connector
         Args:
-            host (str): host
-            port (int): port
-            username (str): username
-            password (str): password
+            host (str): host for ssh connection
+            port (int): port for ssh connection
+            username (str): username for ssh connection
+            password (str): password for ssh connection
         """
         self.host = host
         self.username = username
         self.password = password
         self.port = port
         self.ssh_client = self.__get_ssh_client()
 
@@ -72,15 +72,15 @@
 
         """
         result = None
         if self.ssh_client is None:
             logger.warning('SSH connection failed')
             return result
         try:
-            std_in, std_out, std_err = self.ssh_client.exec_command(cmd, timeout=time_out)
+            _std_in, std_out, _std_err = self.ssh_client.exec_command(cmd, timeout=time_out)
             if read_line:
                 result = std_out.readlines()
             else:
                 result = std_out.read().decode('utf-8').rstrip()
         except Exception as e:
             logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
                          ' msg: %s' % e)
@@ -94,9 +94,7 @@
         """
         self.ssh_client.close()
 
     def __del__(self):
         if self.ssh_client:
             self.close()
 
-if __name__ == '__main__':
-    print(SSHClient('vm37',22,'root','').run_cmd('whoami'))
```

### Comparing `jax-tools-1.0.32/jax_tools.egg-info/PKG-INFO` & `jax-tools-1.0.47/jax_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-tools
-Version: 1.0.32
+Version: 1.0.47
 Summary: Jax common tools library
 Home-page: https://jax-arsenals.com
 Download-URL: https://jax-arsenals.com
 Author: Jax
 Author-email: alvin.wan.cn@hotmail.com
 License: MIT Licence
 Keywords: jax
```

### Comparing `jax-tools-1.0.32/setup.py` & `jax-tools-1.0.47/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     """
     with open(file_path, 'r') as f:
         return f.read()
 
 
 setuptools.setup(
     name="jax-tools",
-    version="1.0.32",
+    version="1.0.47",
     author=u"Jax",
     author_email='alvin.wan.cn@hotmail.com',
     description=u"Jax common tools library",
     platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
     long_description=read_file('README.md'),
     long_description_content_type="text/markdown",
     url="https://jax-arsenals.com",
     license="MIT Licence",
     python_requires=">=3.0.0",
     # 定义要构建到包中的文件列表，这些文件会放到/usr/local下
     data_files=[],
-    packages=['jax_tools', 'jax_tools.utils', ],
+    packages=['jax_tools', 'jax_tools.utils', 'jax_tools.cmd', 'jax_tools.cmd_tools'],
     exclude=['build.py'],
     package_dir={},
     package_data={
         # 'jax_tools': ['*.md'],
         '': ['CHANGELOG.md']
     },
     include_package_data=True,
@@ -47,16 +47,21 @@
     # 定义可以为哪些模块提供依赖
     provides=[],
     install_requires=[
         "ping3 >= 4.0.4",
         "paramiko >= 3.2.0",
         "colorlog >= 6.7.0",
         "pycryptodome >= 3.18.0",
+        "pyperclip >= 1.8.2"
     ],
     # 定义entry points, 前面的sta指的是命令，第二个sta表示模块名，也是目录名，第三个sta表示脚本名，最好那个main，表示sta.py中的main函数
     entry_points={
         'console_scripts': [
-            'nd=jax_tools.network_test:main',
-            'jax-encrypt=jax_tools.jax_encrypt:main',
+            'jax=jax_tools.cmd.jax:main',
+            'nd=jax_tools.cmd.nd:main',
+            'jax-nd=jax_tools.cmd.nd:main',
+            'jax-encrypt=jax_tools.cmd.jax_encrypt:main',
+            'jax-fix=jax_tools.cmd.jax_fix:main',
+            'jax-pam=jax_tools.cmd.jax_pam:main',
         ]
     }
 )
```

