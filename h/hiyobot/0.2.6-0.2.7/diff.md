# Comparing `tmp/hiyobot-0.2.6.tar.gz` & `tmp/hiyobot-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiyobot-0.2.6.tar", last modified: Fri May 26 14:40:41 2023, max compression
+gzip compressed data, was "hiyobot-0.2.7.tar", last modified: Tue Jun  6 13:06:28 2023, max compression
```

## Comparing `hiyobot-0.2.6.tar` & `hiyobot-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-26 14:40:28.000000 hiyobot-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-26 14:40:41.236904 hiyobot-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-26 14:40:28.000000 hiyobot-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/hackchat/
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/hackchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/hc-wait4inp.test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot/zhangchat/
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/zhangchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-26 14:40:28.000000 hiyobot-0.2.6/hiyobot/zhc-wait4inp.test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:40:41.236904 hiyobot-0.2.6/hiyobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 14:40:41.000000 hiyobot-0.2.6/hiyobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:40:41.236904 hiyobot-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-26 14:40:28.000000 hiyobot-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:06:28.091608 hiyobot-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-06 13:06:18.000000 hiyobot-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-06 13:06:28.091608 hiyobot-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-06 13:06:18.000000 hiyobot-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:06:28.087608 hiyobot-0.2.7/hiyobot/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 13:06:18.000000 hiyobot-0.2.7/hiyobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:06:28.091608 hiyobot-0.2.7/hiyobot/hackchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-06-06 13:06:18.000000 hiyobot-0.2.7/hiyobot/hackchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-06 13:06:18.000000 hiyobot-0.2.7/hiyobot/hc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:06:28.091608 hiyobot-0.2.7/hiyobot/zhangchat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-06-06 13:06:18.000000 hiyobot-0.2.7/hiyobot/zhangchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-06 13:06:18.000000 hiyobot-0.2.7/hiyobot/zhc-wait4inp.test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:06:28.091608 hiyobot-0.2.7/hiyobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-06 13:06:28.000000 hiyobot-0.2.7/hiyobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 13:06:28.000000 hiyobot-0.2.7/hiyobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:06:28.000000 hiyobot-0.2.7/hiyobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 13:06:28.000000 hiyobot-0.2.7/hiyobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 13:06:28.000000 hiyobot-0.2.7/hiyobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:06:28.091608 hiyobot-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-06 13:06:18.000000 hiyobot-0.2.7/setup.py
```

### Comparing `hiyobot-0.2.6/LICENSE` & `hiyobot-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.6/PKG-INFO` & `hiyobot-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -14,28 +14,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.3-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
 
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
 Installing collected packages: hiyobot
 Successfully installed hiyobot-<version>
 ```
 # 开发文档
-暂无
+ - [HackChat](HC_DOC.md)
 
 # 注释
  - HiyoBot PYPI版本取决于Hack.chat子集版本。
  - HiyoBot子集使用： 如在Hack.chat编写机器人:`from hiyobot import hackchat as hcbot`, 在ZhangChat(chat.zhangsoft.eu.org or chat.zhangsoft.cf)编写机器人:`from hiyobot import zhangchat as zhcbot`
  - 目前支持的聊天室： Hack.chat(hackchat),ZhangChat(zhangchat)
  - 如其他子集使用方式与Hack.chat集不同，即开设子文档。（暂无）
  - 我们会始终欢迎您的PR/Issues！
```

### Comparing `hiyobot-0.2.6/README.md` & `hiyobot-0.2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.3-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
 
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
 Installing collected packages: hiyobot
 Successfully installed hiyobot-<version>
 ```
 # 开发文档
-暂无
+ - [HackChat](HC_DOC.md)
 
 # 注释
  - HiyoBot PYPI版本取决于Hack.chat子集版本。
  - HiyoBot子集使用： 如在Hack.chat编写机器人:`from hiyobot import hackchat as hcbot`, 在ZhangChat(chat.zhangsoft.eu.org or chat.zhangsoft.cf)编写机器人:`from hiyobot import zhangchat as zhcbot`
  - 目前支持的聊天室： Hack.chat(hackchat),ZhangChat(zhangchat)
  - 如其他子集使用方式与Hack.chat集不同，即开设子文档。（暂无）
  - 我们会始终欢迎您的PR/Issues！
```

### Comparing `hiyobot-0.2.6/hiyobot/hackchat/__init__.py` & `hiyobot-0.2.7/hiyobot/hackchat/__init__.py`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.6/hiyobot/zhangchat/__init__.py` & `hiyobot-0.2.7/hiyobot/zhangchat/__init__.py`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.6/hiyobot.egg-info/PKG-INFO` & `hiyobot-0.2.7/hiyobot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -14,28 +14,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.3-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
 
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
 Installing collected packages: hiyobot
 Successfully installed hiyobot-<version>
 ```
 # 开发文档
-暂无
+ - [HackChat](HC_DOC.md)
 
 # 注释
  - HiyoBot PYPI版本取决于Hack.chat子集版本。
  - HiyoBot子集使用： 如在Hack.chat编写机器人:`from hiyobot import hackchat as hcbot`, 在ZhangChat(chat.zhangsoft.eu.org or chat.zhangsoft.cf)编写机器人:`from hiyobot import zhangchat as zhcbot`
  - 目前支持的聊天室： Hack.chat(hackchat),ZhangChat(zhangchat)
  - 如其他子集使用方式与Hack.chat集不同，即开设子文档。（暂无）
  - 我们会始终欢迎您的PR/Issues！
```

### Comparing `hiyobot-0.2.6/setup.py` & `hiyobot-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hiyobot', # 你的项目名称
-    version="0.2.6", # 你的项目版本
+    version="0.2.7", # 你的项目版本
     description='A simple bot framework for Hack.chat.', # 你的项目简介
     long_description=open('README.md').read(), # 你的项目详细介绍，一般从README.md文件中读取
     long_description_content_type='text/markdown', # 你的项目详细介绍的格式，一般为markdown格式
     url='https://github.com/Hiyoteam/hiyobot', # 你的项目主页，一般为github仓库地址
     author='MaggieLOL', # 你的姓名或者团队名称
     author_email='tanhanzesnd@gmail.com', # 你的邮箱或者团队邮箱
     license='GPL-2.0', # 你的项目使用的许可证，一般为MIT或者其他开源许可证
@@ -19,11 +19,11 @@
     ],
     keywords='bot hack.chat hack.chat-bot', # 一些关键词，用于描述你的项目特点或者功能
     packages=find_packages(include="*",exclude=["*.test.py"]), # 需要打包的python模块，一般使用find_packages函数自动查找，排除测试模块等不需要打包的模块
     install_requires="""cffi==1.15.1
 gevent==22.10.2
 greenlet==2.0.2
 pycparser==2.21
-websocket-client==1.3.2
+websocket-client
 zope.event==4.6
 zope.interface==6.0""".splitlines(),
 )
```

