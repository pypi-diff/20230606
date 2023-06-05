# Comparing `tmp/pebbles_bot-0.3.2.tar.gz` & `tmp/pebbles_bot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pebbles_bot-0.3.2.tar", last modified: Sun May 21 19:50:47 2023, max compression
+gzip compressed data, was "pebbles_bot-0.3.3.tar", last modified: Mon Jun  5 22:53:22 2023, max compression
```

## Comparing `pebbles_bot-0.3.2.tar` & `pebbles_bot-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.814683 pebbles_bot-0.3.2/pebbles_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pb_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pb_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pebbles_bot/pebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:50:47.814683 pebbles_bot-0.3.2/pebbles_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 19:50:47.000000 pebbles_bot-0.3.2/pebbles_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-21 19:50:47.818683 pebbles_bot-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:50:39.000000 pebbles_bot-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:53:22.079954 pebbles_bot-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-05 22:53:22.079954 pebbles_bot-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:53:22.075954 pebbles_bot-0.3.3/pebbles_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/pebbles_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/pebbles_bot/pb_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/pebbles_bot/pb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/pebbles_bot/pebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:53:22.079954 pebbles_bot-0.3.3/pebbles_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 22:53:22.000000 pebbles_bot-0.3.3/pebbles_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-05 22:53:22.079954 pebbles_bot-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:53:13.000000 pebbles_bot-0.3.3/setup.py
```

### Comparing `pebbles_bot-0.3.2/LICENSE` & `pebbles_bot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.2/PKG-INFO` & `pebbles_bot-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles_bot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,18 @@
     - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
 There are only 3 steps to get it up and running:
 1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
 2. Install the bot on the server where you wish to run commands using Python pip.
-3. Configure environment variables and run it!
+3. Configure environment variables and run it!  
+
+More about the usage of Pebbles can be found on my [blog post](https://labbrat.net/blog/pebbles_bot/).
+
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
 - Users whitelist - only whitelisted users can run commands on the bot.
```

### Comparing `pebbles_bot-0.3.2/README.md` & `pebbles_bot-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
 There are only 3 steps to get it up and running:
 1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
 2. Install the bot on the server where you wish to run commands using Python pip.
-3. Configure environment variables and run it!
+3. Configure environment variables and run it!  
+
+More about the usage of Pebbles can be found on my [blog post](https://labbrat.net/blog/pebbles_bot/).
+
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
 - Users whitelist - only whitelisted users can run commands on the bot.
```

### Comparing `pebbles_bot-0.3.2/pebbles_bot/pb_main.py` & `pebbles_bot-0.3.3/pebbles_bot/pb_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
         Start the bot and print a message.
         """
         self.logger.info("Pebbles is awakening...")
         self.logger.info("Awaiting commands")
         try:
             self.bot.polling(interval=0)
         except ApiTelegramException:
-            self.logger.exception(
-                "Unable to start Pebbles, check your API key"
-            )
+            self.logger.exception("Unable to start Pebbles, check your API key")
         self.logger.info("Pebbles is entering hibernation...")
 
     def log(self, info, log=""):
         """
         Simplifies the use of logger library,
         and makes logger look cleaner in the code.
         """
@@ -279,17 +277,15 @@
         elif call.data == "remote":
             self.pebbles_mode = "remote"
             self.bot.send_message(
                 call.message.chat.id, "Pebbles mode: Remote 🚀"
             )
         elif call.data == "local":
             self.pebbles_mode = "local"
-            self.bot.send_message(
-                call.message.chat.id, "Pebbles mode: Local 🏡"
-            )
+            self.bot.send_message(call.message.chat.id, "Pebbles mode: Local 🏡")
 
     def rest(self, message):
         """
         Process input that is not defined
         """
         self.bot.send_message(
             message.from_user.id,
```

### Comparing `pebbles_bot-0.3.2/pebbles_bot/pb_tools.py` & `pebbles_bot-0.3.3/pebbles_bot/pb_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import os
 from subprocess import PIPE, STDOUT, Popen
 from paramiko import SSHConfig, SSHClient, AutoAddPolicy
-from paramiko.ssh_exception import (
-    AuthenticationException,
-    NoValidConnectionsError,
-)
 
 
 def security_check(method):
     """
     Attempt to find user ID in uid whitelist,
     allow uid to run command if found,
     block if not found.
@@ -39,16 +35,20 @@
         self.client.set_missing_host_key_policy(AutoAddPolicy())
 
     def read_ssh_config(self):
         """
         Read SSH config file and return a dictionary
         """
         ssh_config_file = os.path.expanduser("~/.ssh/config")
-        with open(ssh_config_file) as f:
-            self.config.parse(f)
+        if not os.path.exists(ssh_config_file):
+            with open(ssh_config_file, "w"):
+                print(f"Empty SSH config created at {ssh_config_file}")
+
+        with open(ssh_config_file) as conf:
+            self.config.parse(conf)
 
     def ssh_connect(self, host):
         """
         Establish a SSH connection
         """
         try:
             host_config = self.config.lookup(host)
```

### Comparing `pebbles_bot-0.3.2/pebbles_bot/pebot.py` & `pebbles_bot-0.3.3/pebbles_bot/pebot.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     else:
         print(f"Config file {config} not found")
         return None
 
 
 def main():
     parser = argparse.ArgumentParser(description="Run Pebbles.")
-    parser.add_argument('--notify', action='store_true', help='Notification message to send')
+    parser.add_argument(
+        "--notify", action="store_true", help="Notification message to send"
+    )
     args = parser.parse_args()
 
     api_key = os.environ.get("PEBBLES_API_KEY")
     whitelist_ids = os.environ.get("PEBBLES_USER_WHITELIST")
 
     if not api_key:
         print("Pebbles API key not found")
@@ -53,9 +55,7 @@
         whitelist=whitelist_ids.split(","),
         notify=notify,
     )
 
 
 if __name__ == "__main__":
     main()
-
-
```

### Comparing `pebbles_bot-0.3.2/pebbles_bot.egg-info/PKG-INFO` & `pebbles_bot-0.3.3/pebbles_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles-bot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,18 @@
     - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
 There are only 3 steps to get it up and running:
 1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
 2. Install the bot on the server where you wish to run commands using Python pip.
-3. Configure environment variables and run it!
+3. Configure environment variables and run it!  
+
+More about the usage of Pebbles can be found on my [blog post](https://labbrat.net/blog/pebbles_bot/).
+
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
 - Users whitelist - only whitelisted users can run commands on the bot.
```

### Comparing `pebbles_bot-0.3.2/setup.cfg` & `pebbles_bot-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pebbles_bot
-version = 0.3.2
+version = 0.3.3
 description = Telegram bot that runs Linux shell commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

