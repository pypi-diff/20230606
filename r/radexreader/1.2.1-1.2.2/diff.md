# Comparing `tmp/radexreader-1.2.1.tar.gz` & `tmp/radexreader-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radexreader-1.2.1.tar", last modified: Thu Sep  9 20:07:26 2021, max compression
+gzip compressed data, was "radexreader-1.2.2.tar", last modified: Tue Jun  6 20:08:49 2023, max compression
```

## Comparing `radexreader-1.2.1.tar` & `radexreader-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-09-09 20:07:26.631296 radexreader-1.2.1/
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)    18092 2021-09-09 20:07:15.000000 radexreader-1.2.1/LICENSE
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)     4247 2021-09-09 20:07:26.631296 radexreader-1.2.1/PKG-INFO
--rw-r-----   0 fabrice   (1000) fabrice   (1000)     3487 2021-09-09 20:07:15.000000 radexreader-1.2.1/README.md
-drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-09-09 20:07:26.631296 radexreader-1.2.1/radexreader/
--rw-r-----   0 fabrice   (1000) fabrice   (1000)     9342 2021-09-09 20:07:15.000000 radexreader-1.2.1/radexreader/__init__.py
--rw-r-----   0 fabrice   (1000) fabrice   (1000)     4824 2021-09-09 20:07:15.000000 radexreader-1.2.1/radexreader/radexreader.py
-drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-09-09 20:07:26.631296 radexreader-1.2.1/radexreader.egg-info/
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)     4247 2021-09-09 20:07:26.000000 radexreader-1.2.1/radexreader.egg-info/PKG-INFO
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)      251 2021-09-09 20:07:26.000000 radexreader-1.2.1/radexreader.egg-info/SOURCES.txt
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)        1 2021-09-09 20:07:26.000000 radexreader-1.2.1/radexreader.egg-info/dependency_links.txt
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)       15 2021-09-09 20:07:26.000000 radexreader-1.2.1/radexreader.egg-info/requires.txt
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)       12 2021-09-09 20:07:26.000000 radexreader-1.2.1/radexreader.egg-info/top_level.txt
--rw-r--r--   0 fabrice   (1000) fabrice   (1000)       38 2021-09-09 20:07:26.631296 radexreader-1.2.1/setup.cfg
--rw-r-----   0 fabrice   (1000) fabrice   (1000)     1806 2021-09-09 20:07:15.000000 radexreader-1.2.1/setup.py
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2023-06-06 20:08:49.403148 radexreader-1.2.2/
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)    18092 2023-06-06 20:08:47.000000 radexreader-1.2.2/LICENSE
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)     4199 2023-06-06 20:08:49.403148 radexreader-1.2.2/PKG-INFO
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)     3459 2023-06-06 20:08:47.000000 radexreader-1.2.2/README.md
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2023-06-06 20:08:49.395148 radexreader-1.2.2/radexreader/
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)    10067 2023-06-06 20:08:47.000000 radexreader-1.2.2/radexreader/__init__.py
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)     4988 2023-06-06 20:08:47.000000 radexreader-1.2.2/radexreader/radexreader.py
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2023-06-06 20:08:49.399148 radexreader-1.2.2/radexreader.egg-info/
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)     4199 2023-06-06 20:08:49.000000 radexreader-1.2.2/radexreader.egg-info/PKG-INFO
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)      251 2023-06-06 20:08:49.000000 radexreader-1.2.2/radexreader.egg-info/SOURCES.txt
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)        1 2023-06-06 20:08:49.000000 radexreader-1.2.2/radexreader.egg-info/dependency_links.txt
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)       15 2023-06-06 20:08:49.000000 radexreader-1.2.2/radexreader.egg-info/requires.txt
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)       12 2023-06-06 20:08:49.000000 radexreader-1.2.2/radexreader.egg-info/top_level.txt
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)       38 2023-06-06 20:08:49.403148 radexreader-1.2.2/setup.cfg
+-rw-r-----   0 fabrice   (1000) fabrice   (1000)     1761 2023-06-06 20:08:47.000000 radexreader-1.2.2/setup.py
```

### Comparing `radexreader-1.2.1/LICENSE` & `radexreader-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `radexreader-1.2.1/PKG-INFO` & `radexreader-1.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 Metadata-Version: 2.1
 Name: radexreader
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python library for the RADEX RD1212 and the RADEX ONE Geiger counters.
 Home-page: https://github.com/luigifab/python-radexreader
 Author: Fabrice Creuzot
 Author-email: code@luigifab.fr
 License: GPL 2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RadexReader
 
-The RadexReader is an user-space driver for the [RADEX RD1212](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+The RadexReader is an user-space driver for the [RADEX RD1212 v1/v2](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+
+This tool was initially developed with RD1212 v2.48.
 
 ![RADEX RD1212](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/RD1212.jpg?raw=true)
 ![RADEX ONE](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/ONE.jpg?raw=true)
 
-## Screenshots
+## Screenshots and Usage
 
 [![Screnshot 1](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/thumbs/read.png?raw=true)](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/read.png?raw=true)
 [![Screnshot 2](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/thumbs/compare.png?raw=true)](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/compare.png?raw=true)
 
 * Read `src/radexreader.py` for examples.
 * Run the command `radexreader` available with DEB/RPM packages.
-* Run the command `radexreader.py` available with PYPI package.
+* Run the command `.../radexreader.py` available with PYPI package.
 
 ## Installation
 
 It require *libusb*, *pyusb* and *pyserial*.
 
-* Debian and Ubuntu: `sudo apt install python3-radexreader radexreader` (coming soon or via [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages))
+#### Installation for Debian and Ubuntu
+
+* `sudo apt install python3-radexreader radexreader`
+
+#### Installation for Fedora
 
-* Fedora: `sudo dnf install python3-radexreader`
+* `sudo dnf install python3-radexreader`
 
-* openSUSE: `sudo zypper install python3-radexreader`
+#### Installation for openSUSE
 
-* Linux: `sudo python3 -m pip install radexreader` (+libusb)
+* `sudo zypper install python3-radexreader`
 
-* Mac: `sudo pip install radexreader` (+libusb)
+#### Installation with PIP
 
-* Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
+* With Linux: `sudo python3 -m pip install radexreader` (+libusb)
+* With Mac: `sudo pip install radexreader` (+libusb)
+* With Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
 
-* Docker Alpine: `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
+#### Installation with Docker
 
-## PPA
+* `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
+
+#### Alternative installation for Debian and Ubuntu
 
-Installation for Debian and Ubuntu with [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages):
 ```bash
+# https://launchpad.net/~luigifab/+archive/ubuntu/packages
 sudo add-apt-repository ppa:luigifab/packages
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys FFE5BD439356DF7D
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo wget -O /etc/apt/trusted.gpg.d/luigifab.gpg https://www.luigifab.fr/apt.gpg
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 ```
 ```bash
 # sha256sum /etc/apt/trusted.gpg.d/luigifab.gpg
 578c89a677048e38007462d543686b53587efba9f93814601169253c45ff9213
 # apt-key list
 /etc/apt/trusted.gpg.d/luigifab.gpg
 pub   rsa4096 2020-10-31 [SC]
       458B 0C46 D024 FD8C B8BC  99CD FFE5 BD43 9356 DF7D
 ```
 
 ## Copyright
 
-- Current version: 1.2.1 (09/09/2021)
-- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10
+- Current version: 1.2.2 (06/06/2023)
+- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10 / 3.11
 - Links: [luigifab.fr](https://www.luigifab.fr/python/radexreader) - [github.com](https://github.com/luigifab/python-radexreader) - [pypi.org](https://pypi.org/project/radexreader/)\
-[Debian python-radexreader.deb](https://tracker.debian.org/pkg/python3-radexreader)
-  *([ITP](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=973447),
-   [RFS](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=974217))*\
-[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python3-radexreader)\
+[Debian python-radexreader.deb](https://packages.debian.org/python3-radexreader)\
+[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python-radexreader)\
 [openSUSE python-radexreader.rpm](https://software.opensuse.org/package/python-radexreader)\
 [Ubuntu PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages)
 
 This program is provided under the terms of the **GNU GPLv2+** license.\
 If you like, take some of your time to improve some translations, go to https://bit.ly/2HyCCEc.
-
-
```

### Comparing `radexreader-1.2.1/README.md` & `radexreader-1.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,83 @@
 # RadexReader
 
-The RadexReader is an user-space driver for the [RADEX RD1212](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+The RadexReader is an user-space driver for the [RADEX RD1212 v1/v2](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+
+This tool was initially developed with RD1212 v2.48.
 
 ![RADEX RD1212](images/RD1212.jpg?raw=true)
 ![RADEX ONE](images/ONE.jpg?raw=true)
 
-## Screenshots
+## Screenshots and Usage
 
 [![Screnshot 1](images/thumbs/read.png?raw=true)](images/read.png?raw=true)
 [![Screnshot 2](images/thumbs/compare.png?raw=true)](images/compare.png?raw=true)
 
 * Read `src/radexreader.py` for examples.
 * Run the command `radexreader` available with DEB/RPM packages.
-* Run the command `radexreader.py` available with PYPI package.
+* Run the command `.../radexreader.py` available with PYPI package.
 
 ## Installation
 
 It require *libusb*, *pyusb* and *pyserial*.
 
-* Debian and Ubuntu: `sudo apt install python3-radexreader radexreader` (coming soon or via [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages))
+#### Installation for Debian and Ubuntu
+
+* `sudo apt install python3-radexreader radexreader`
+
+#### Installation for Fedora
+
+* `sudo dnf install python3-radexreader`
 
-* Fedora: `sudo dnf install python3-radexreader`
+#### Installation for openSUSE
 
-* openSUSE: `sudo zypper install python3-radexreader`
+* `sudo zypper install python3-radexreader`
 
-* Linux: `sudo python3 -m pip install radexreader` (+libusb)
+#### Installation with PIP
 
-* Mac: `sudo pip install radexreader` (+libusb)
+* With Linux: `sudo python3 -m pip install radexreader` (+libusb)
+* With Mac: `sudo pip install radexreader` (+libusb)
+* With Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
 
-* Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
+#### Installation with Docker
 
-* Docker Alpine: `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
+* `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
 
-## PPA
+#### Alternative installation for Debian and Ubuntu
 
-Installation for Debian and Ubuntu with [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages):
 ```bash
+# https://launchpad.net/~luigifab/+archive/ubuntu/packages
 sudo add-apt-repository ppa:luigifab/packages
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys FFE5BD439356DF7D
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo wget -O /etc/apt/trusted.gpg.d/luigifab.gpg https://www.luigifab.fr/apt.gpg
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 ```
 ```bash
 # sha256sum /etc/apt/trusted.gpg.d/luigifab.gpg
 578c89a677048e38007462d543686b53587efba9f93814601169253c45ff9213
 # apt-key list
 /etc/apt/trusted.gpg.d/luigifab.gpg
 pub   rsa4096 2020-10-31 [SC]
       458B 0C46 D024 FD8C B8BC  99CD FFE5 BD43 9356 DF7D
 ```
 
 ## Copyright
 
-- Current version: 1.2.1 (09/09/2021)
-- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10
+- Current version: 1.2.2 (06/06/2023)
+- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10 / 3.11
 - Links: [luigifab.fr](https://www.luigifab.fr/python/radexreader) - [github.com](https://github.com/luigifab/python-radexreader) - [pypi.org](https://pypi.org/project/radexreader/)\
-[Debian python-radexreader.deb](https://tracker.debian.org/pkg/python3-radexreader)
-  *([ITP](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=973447),
-   [RFS](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=974217))*\
-[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python3-radexreader)\
+[Debian python-radexreader.deb](https://packages.debian.org/python3-radexreader)\
+[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python-radexreader)\
 [openSUSE python-radexreader.rpm](https://software.opensuse.org/package/python-radexreader)\
 [Ubuntu PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages)
 
 This program is provided under the terms of the **GNU GPLv2+** license.\
 If you like, take some of your time to improve some translations, go to https://bit.ly/2HyCCEc.
```

### Comparing `radexreader-1.2.1/radexreader/__init__.py` & `radexreader-1.2.2/radexreader/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf8 -*-
 # Created L/19/10/2020
-# Updated M/10/08/2021
+# Updated S/04/03/2023
 #
-# Copyright 2020-2021 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
+# Copyright 2020-2023 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
 # https://github.com/luigifab/python-radexreader
-# https://www.luigifab.fr/python/radexreader
 #
 # This program is free software, you can redistribute it or modify
 # it under the terms of the GNU General Public License (GPL) as published
 # by the free software foundation, either version 2 of the license, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -24,15 +23,15 @@
 import usb.core
 import usb.util
 import usb.backend.libusb1
 # pyserial
 import serial
 import serial.tools.list_ports
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 class RadexReader():
 
 	com = None
 	usb = None
 	serial = None
 	keyA = None
@@ -41,51 +40,55 @@
 	keyD = None
 
 	def __init__(self):
 
 		# backend only for alpine with docker?
 		backend = usb.backend.libusb1.get_backend(find_library=lambda x: '/usr/lib/libusb-1.0.so.0')
 
-		# RADEX RD1212 v2
-		# search usb device (03EB/5603)
-		self.usb = usb.core.find(idVendor=0x03eb, idProduct=0x5603, backend=backend)
+		# RADEX ONE v1
+		# search usb device (ABBA/A011)
+		self.usb = usb.core.find(idVendor=0xabba, idProduct=0xa011, backend=backend)
 		if self.usb is not None:
-			self.com = 'RD1212v2'
-			# usb reset
-			self.usb.reset()
-			if sys.platform != 'win32' and sys.platform != 'cygwin' and self.usb.is_kernel_driver_active(0):
-				self.usb.detach_kernel_driver(0)
-			self.usb.set_configuration()
-			return # device found
+			self.com = 'ONEv1'
+			# search usb serial device (https://stackoverflow.com/a/25112066/2980105)
+			devices = serial.tools.list_ports.grep('RADEX')
+			for device in devices:
+				self.serial = serial.Serial(port=device.device, baudrate=9600, timeout=0.5)
+				return # device found
+			if self.serial is None:
+				raise ValueError('Error: RADEX ONE (serial) not found')
 
 		# RADEX RD1212 v1
-		# search usb device (10C4/EA60 = Silicon labs USB to UART bridge)
+		# search usb device (10C4/EA60 = Silicon labs USB to UART bridge or CP2102 USB to UART Bridge Controller)
 		self.usb = usb.core.find(idVendor=0x10c4, idProduct=0xea60, backend=backend)
 		if self.usb is not None:
 			self.com = 'RD1212v1'
 			# search usb serial device (https://stackoverflow.com/a/25112066/2980105)
-			devices  = serial.tools.list_ports.grep('RADEX')
+			devices = serial.tools.list_ports.grep('RADEX')
+			for device in devices:
+				self.serial = serial.Serial(port=device.device, baudrate=115200, timeout=0.5)
+				return # device found
+			devices = serial.tools.list_ports.grep('CP2102')
 			for device in devices:
-				self.serial = serial.Serial(port = device.device, baudrate = 115200, timeout = 0.5)
+				self.serial = serial.Serial(port=device.device, baudrate=115200, timeout=0.5)
 				return # device found
 			if self.serial is None:
 				raise ValueError('Error: RADEX RD1212 (serial) not found')
 
-		# RADEX ONE v1
-		# search usb device (ABBA/A011)
-		self.usb = usb.core.find(idVendor=0xabba, idProduct=0xa011, backend=backend)
+ 		# RADEX RD1212 v2
+		# search usb device (03EB/5603)
+		self.usb = usb.core.find(idVendor=0x03eb, idProduct=0x5603, backend=backend)
 		if self.usb is not None:
-			self.com = 'ONEv1'
-			# search usb serial device (https://stackoverflow.com/a/25112066/2980105)
-			devices  = serial.tools.list_ports.grep('RADEX')
-			for device in devices:
-				self.serial = serial.Serial(port = device.device, baudrate = 9600, timeout = 0.5)
-				return # device found
-			if self.serial is None:
-				raise ValueError('Error: RADEX ONE (serial) not found')
+			self.com = 'RD1212v2'
+			# usb reset
+			self.usb.reset()
+			if sys.platform != 'win32' and sys.platform != 'cygwin' and self.usb.is_kernel_driver_active(0):
+				self.usb.detach_kernel_driver(0)
+			self.usb.set_configuration()
+			return # device found
 
 		# no devices found
 		if self.usb is None:
 			raise ValueError('Error: RADEX RD1212 (usb) and RADEX ONE (usb) not plugged?')
 
 	def get_device(self, getusb=False):
 		if not getusb and self.serial is not None:
@@ -93,52 +96,55 @@
 		return self.usb
 
 	def print_info(self):
 		if self.com == 'RD1212v2':
 			print('Manufacturer  ' + hex(self.usb.idVendor).ljust(7, ' ')  + ' ' + usb.util.get_string(self.usb, self.usb.iManufacturer))
 			print('Product       ' + hex(self.usb.idProduct).ljust(7, ' ') + ' ' + usb.util.get_string(self.usb, self.usb.iProduct))
 			print()
+			# https://www.criirad.org/laboratoire/radiametres/compteur-geiger.html
 			print('[info] Sensor: Geiger-Müller tube SBM 20-1')
 			print('[info] Measuring range: 0.05 - 999 µSv/h')
 			print('[info] Uncertainty of the result: ±(15+6/D)%')
 			print('[info]   D is the value after a complete cycle of 100 seconds')
 			print()
-			print('[warn] The values displayed are only an approximation.')
+			print('[warn] The values shown are only approximations.')
 			print('[warn] The actual value can only be measured with suitable professional device.')
 			print('[warn] For now, not tested with measured values greater than 0.25 µSv/h.')
 			print()
 		elif self.com == 'RD1212v1':
 			print('Manufacturer  ' + hex(self.usb.idVendor).ljust(7, ' ')  + ' ' + usb.util.get_string(self.usb, self.usb.iManufacturer))
 			print('Product       ' + hex(self.usb.idProduct).ljust(7, ' ') + ' ' + usb.util.get_string(self.usb, self.usb.iProduct))
 			print('ComPort       ' + self.serial.port)
 			print()
+			# source?
 			print('[info] Sensor: Geiger-Müller tube SBM 20-1')
 			print('[info] Measuring range: 0.05 - 999 µSv/h')
 			print('[info] Uncertainty of the result: ±(15+6/D)%')
 			print('[info]   D is the value after a complete cycle of 100 seconds')
 			print()
-			print('[warn] The values displayed are only an approximation.')
+			print('[warn] The values shown are only approximations.')
 			print('[warn] The actual value can only be measured with suitable professional device.')
 			print('[warn] For now, not tested with measured values greater than 0.25 µSv/h.')
 			print()
 		elif self.com == 'ONEv1':
 			if sys.platform != 'win32' and sys.platform != 'cygwin':
 				print('Manufacturer  ' + hex(self.usb.idVendor).ljust(7, ' ')  + ' ' + usb.util.get_string(self.usb, self.usb.iManufacturer))
 				print('Product       ' + hex(self.usb.idProduct).ljust(7, ' ') + ' ' + usb.util.get_string(self.usb, self.usb.iProduct))
 			else:
 				print('Manufacturer  -x----  QUARTA-RAD')
 				print('Product       -x----  RADEX ONE')
 			print('ComPort       ' + self.serial.port)
 			print()
+			# source?
 			print('[info] Sensor: Geiger-Müller tube SBM 20-1')
 			print('[info] Measuring range: 0.05 - 999 µSv/h')
 			print('[info] Uncertainty of the result: ±(15+6/D)%')
 			print('[info]   D is the value after a complete cycle of 100? seconds')
 			print()
-			print('[warn] The values displayed are only an approximation.')
+			print('[warn] The values shown are only approximations.')
 			print('[warn] The actual value can only be measured with suitable professional device.')
 			print('[warn] For now, not tested with measured values greater than 0.25 µSv/h.')
 			print()
 
 	def hid_set_report(self, report):
 		if self.com == 'RD1212v2':
 			# https://stackoverflow.com/a/52368526/2980105
@@ -171,40 +177,57 @@
 
 	def read(self, last=False):
 
 		if self.com == 'ONEv1':
 			return self.readOne()
 
 		values = {}
+		# from 0x0 to 0xb3
 		if last:
 			keys = [0x0]
+		elif last and self.com == 'RD1212v1':
+			keys = list(reversed(range(0x0, 0xb4)))
 		else:
-			keys = list(range(0x0, 0xb4)) # from 0x0 to 0xb3
+			keys = list(range(0x0, 0xb4))
+
+		# 1 min, 5 min, 10 min, 30 min, 1 hour, 2 hours, 4 hours, 6 hours, 12 hours, 24 hours
+		interval = {0: 1, 1: 5, 2: 10, 3: 30, 4: 60, 5: 120, 6: 240, 7: 360, 8: 720, 9: 1440}
 
 		for key in keys:
 			self.hid_set_report((0x12, 0x12, 0x01, 0x02, key, 0, 0, 0, 0, 0, 0, 0, 0x3c, 0x84))
 			hexa = self.hid_get_report()
-			if hexa[0] != 0:
+			if hexa != b'' and hexa[0] != 0:
 				# timestamp = 01/01/2016 00:00:44 = 1451606444
 				# timestamp = 01/01/2016 00:00:44 = 172 + 193 (×256) + 133 (×256×256) + 86 (×256×256×256)
 				timestamp   = (hexa[2] + hexa[3] * 256 + hexa[4] * 256 * 256 + hexa[5] * 256 * 256 * 256)
 				# measure   = 0.15 µSv/h = 15
-				measure     = (hexa[6] + hexa[7] * 256 + hexa[8] * 256 * 256) / 100
+				measure     = (hexa[6] + hexa[7] * 256) / 100
 				# uncertainty of the result
 				percent     = 15 + 6 / measure
 				measure_min = measure * (1 - percent / 100)
 				measure_max = measure * (1 + percent / 100)
 				if measure_min < 0:
 					measure_min = 0
 				if percent > 99.9:
 					percent = 99.9
 				# memorize
-				values[timestamp] = { 'pct': percent, 'min': measure_min, 'val': measure, 'max': measure_max }
+				values[timestamp] = {
+					'pct': percent,
+					'min': measure_min,
+					'val': measure,
+					'max': measure_max,
+					'time': timestamp,
+					'interval': interval[hexa[8]]
+				}
+				# to get last measure with RD1212v1
+				if last and self.com == 'RD1212v1':
+					break
 
-		return dict(sorted(values.items(), key=operator.itemgetter(0))) # sort by date
+		# sort by date
+		return dict(sorted(values.items(), key=operator.itemgetter(0)))
 
 	def readOne(self):
 
 		if self.keyA is None:
 			self.keyA = 0x04 - 0x04
 			self.keyB = 0x00
 			self.keyC = 0x5a + 0x04
@@ -237,14 +260,22 @@
 		measure_max = measure * (1 + percent / 100)
 		if measure_min < 0:
 			measure_min = 0
 		if percent > 99.9:
 			percent = 99.9
 
 		timestamp = int(time.time())
-		return { timestamp: { 'pct': percent, 'min': measure_min, 'val': measure, 'max': measure_max, 'acc': measure_acc, 'cpm': measure_cpm } }
+		return { timestamp: {
+			'pct': percent,
+			'min': measure_min,
+			'val': measure,
+			'max': measure_max,
+			'acc': measure_acc,
+			'cpm': measure_cpm,
+			'time': timestamp
+		} }
 
 	def erase(self):
 		if self.com == 'RD1212v2':
 			self.hid_set_report((0x12, 0x12, 0x01, 0x03, 0, 0, 0, 0, 0, 0, 0, 0, 0x3c, 0x84))
 		elif self.com == 'RD1212v1':
 			self.hid_set_report((0x12, 0x12, 0x01, 0x03, 0, 0, 0, 0, 0, 0, 0, 0, 0x3c, 0x84))
```

### Comparing `radexreader-1.2.1/radexreader/radexreader.py` & `radexreader-1.2.2/radexreader/radexreader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf8 -*-
 # Created L/19/10/2020
-# Updated J/06/05/2021
+# Updated D/01/01/2023
 #
-# Copyright 2020-2021 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
+# Copyright 2020-2023 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
 # https://github.com/luigifab/python-radexreader
-# https://www.luigifab.fr/python/radexreader
 #
 # This program is free software, you can redistribute it or modify
 # it under the terms of the GNU General Public License (GPL) as published
 # by the free software foundation, either version 2 of the license, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -21,27 +20,29 @@
 from platform import python_version
 import sys
 import time
 import usb
 import serial
 
 # https://stackoverflow.com/a/62804772/2980105
-# prevent auto import for "import radexreader"when filename is "radexreader.py"
+# prevent auto import for "import radexreader" when filename is "radexreader.py"
 sys.path = sys.path[1:]
 
-try:
-	import radexreader
-	msg = 'Information   python3-radexreader-pypi ' + radexreader.__version__
-	msg += ' with python ' + python_version() + ' + pyusb ' + usb.__version__ + ' + pyserial ' + serial.__version__
-except:
+# python3 .../src/radexreader.py when radexreader is installed or not
+if ".py" in sys.argv[0]:
 	import os
-	sys.path.append(os.path.abspath(__file__).replace('radexreader.py', ''))
+	sys.path.insert(0, os.path.abspath(sys.argv[0]).replace('radexreader.py', ''))
 	import radexreader
 	msg = 'Information   radexreader ' + radexreader.__version__
 	msg += ' with python ' + python_version() + ' + pyusb ' + usb.__version__ + ' + pyserial ' + serial.__version__
+# standard command radexreader
+else:
+	import radexreader
+	msg = 'Information   python3-radexreader-pypi ' + radexreader.__version__
+	msg += ' with python ' + python_version() + ' + pyusb ' + usb.__version__ + ' + pyserial ' + serial.__version__
 
 if len(sys.argv) > 1:
 
 	if sys.argv[1] == 'erase':
 		print(msg)
 		reader = radexreader.RadexReader()
 		reader.print_info()
@@ -72,28 +73,28 @@
 							str('{:.0f}'.format(measure['cpm'])).rjust(6, ' '),
 							str(int(measure['pct']))
 						))
 				prev = timestamp
 			time.sleep(10)
 		exit(0)
 
-	if sys.argv[1] == 'tailjson':
+	if sys.argv[1] == 'jsontail' or sys.argv[1] == 'tailjson':
 		import json
 		reader = radexreader.RadexReader()
 		prev   = None
 		while True:
 			measures = reader.read(True)
 			for timestamp, measure in measures.items():
 				if timestamp != prev:
-					print(json.dumps(measure))
+					print(json.dumps({timestamp: measure}))
 				prev = timestamp
 			time.sleep(10)
 		exit(0)
 
-	if sys.argv[1] == 'readlast':
+	if sys.argv[1] == 'last' or sys.argv[1] == 'readlast':
 		print(msg)
 		reader = radexreader.RadexReader()
 		reader.print_info()
 		measures = reader.read(True)
 		for timestamp, measure in measures.items():
 			print('%s  %s µSv/h  ±%s%% (%s ≤ %s ≤ %s)' % (
 				str(datetime.utcfromtimestamp(timestamp)),
@@ -114,15 +115,15 @@
 		exit(0)
 
 	if sys.argv[1] == 'jsonlast':
 		import json
 		print(json.dumps(radexreader.RadexReader().read(True)))
 		exit(0)
 
-	if sys.argv[1] == 'readall':
+	if sys.argv[1] == 'all' or sys.argv[1] == 'readall':
 		print(msg)
 		reader = radexreader.RadexReader()
 		reader.print_info()
 		measures = reader.read(False)
 		for timestamp, measure in measures.items():
 			print('%s  %s µSv/h  ±%s%% (%s ≤ %s ≤ %s)' % (
 				str(datetime.utcfromtimestamp(timestamp)),
@@ -143,9 +144,9 @@
 		exit(0)
 
 	if sys.argv[1] == 'jsonall':
 		import json
 		print(json.dumps(radexreader.RadexReader().read(False)))
 		exit(0)
 
-print('Usage: radexreader.py erase|tail|tailjson|readlast|jsonlast|readall|jsonall')
+print('Usage: radexreader.py erase|tail|jsontail|last|jsonlast|all|jsonall')
 exit(-1)
```

### Comparing `radexreader-1.2.1/radexreader.egg-info/PKG-INFO` & `radexreader-1.2.2/radexreader.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 Metadata-Version: 2.1
 Name: radexreader
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python library for the RADEX RD1212 and the RADEX ONE Geiger counters.
 Home-page: https://github.com/luigifab/python-radexreader
 Author: Fabrice Creuzot
 Author-email: code@luigifab.fr
 License: GPL 2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RadexReader
 
-The RadexReader is an user-space driver for the [RADEX RD1212](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+The RadexReader is an user-space driver for the [RADEX RD1212 v1/v2](https://quartarad.com/product-category/radiation-detector/) and the [RADEX ONE](https://quartarad.com/product-category/radiation-detector/) Geiger counters. It allow to read and clear stored data via USB. Warning! This tool is completely unrelated with QuartaRad.
+
+This tool was initially developed with RD1212 v2.48.
 
 ![RADEX RD1212](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/RD1212.jpg?raw=true)
 ![RADEX ONE](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/ONE.jpg?raw=true)
 
-## Screenshots
+## Screenshots and Usage
 
 [![Screnshot 1](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/thumbs/read.png?raw=true)](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/read.png?raw=true)
 [![Screnshot 2](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/thumbs/compare.png?raw=true)](https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/compare.png?raw=true)
 
 * Read `src/radexreader.py` for examples.
 * Run the command `radexreader` available with DEB/RPM packages.
-* Run the command `radexreader.py` available with PYPI package.
+* Run the command `.../radexreader.py` available with PYPI package.
 
 ## Installation
 
 It require *libusb*, *pyusb* and *pyserial*.
 
-* Debian and Ubuntu: `sudo apt install python3-radexreader radexreader` (coming soon or via [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages))
+#### Installation for Debian and Ubuntu
+
+* `sudo apt install python3-radexreader radexreader`
+
+#### Installation for Fedora
 
-* Fedora: `sudo dnf install python3-radexreader`
+* `sudo dnf install python3-radexreader`
 
-* openSUSE: `sudo zypper install python3-radexreader`
+#### Installation for openSUSE
 
-* Linux: `sudo python3 -m pip install radexreader` (+libusb)
+* `sudo zypper install python3-radexreader`
 
-* Mac: `sudo pip install radexreader` (+libusb)
+#### Installation with PIP
 
-* Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
+* With Linux: `sudo python3 -m pip install radexreader` (+libusb)
+* With Mac: `sudo pip install radexreader` (+libusb)
+* With Windows: `python -m pip install radexreader` (+[libusb](https://libusb.info/), put libusb-1.0.dll in system32)
 
-* Docker Alpine: `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
+#### Installation with Docker
 
-## PPA
+* `sudo docker run --rm --user root -it --privileged -v /dev:/dev python:3.x-alpine /bin/sh` then: `apk update ; apk add libusb ; python3 -m pip install radexreader`
+
+#### Alternative installation for Debian and Ubuntu
 
-Installation for Debian and Ubuntu with [PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages):
 ```bash
+# https://launchpad.net/~luigifab/+archive/ubuntu/packages
 sudo add-apt-repository ppa:luigifab/packages
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys FFE5BD439356DF7D
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 # or
 sudo wget -O /etc/apt/trusted.gpg.d/luigifab.gpg https://www.luigifab.fr/apt.gpg
-echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu hirsute main" | sudo tee -a /etc/apt/sources.list
+echo "deb http://ppa.launchpad.net/luigifab/packages/ubuntu focal main" | sudo tee -a /etc/apt/sources.list
 sudo apt update
 sudo apt install python3-radexreader radexreader
 ```
 ```bash
 # sha256sum /etc/apt/trusted.gpg.d/luigifab.gpg
 578c89a677048e38007462d543686b53587efba9f93814601169253c45ff9213
 # apt-key list
 /etc/apt/trusted.gpg.d/luigifab.gpg
 pub   rsa4096 2020-10-31 [SC]
       458B 0C46 D024 FD8C B8BC  99CD FFE5 BD43 9356 DF7D
 ```
 
 ## Copyright
 
-- Current version: 1.2.1 (09/09/2021)
-- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10
+- Current version: 1.2.2 (06/06/2023)
+- Compatibility: Python 3.3 / 3.4 / 3.5 / 3.6 / 3.7 / 3.8 / 3.9 / 3.10 / 3.11
 - Links: [luigifab.fr](https://www.luigifab.fr/python/radexreader) - [github.com](https://github.com/luigifab/python-radexreader) - [pypi.org](https://pypi.org/project/radexreader/)\
-[Debian python-radexreader.deb](https://tracker.debian.org/pkg/python3-radexreader)
-  *([ITP](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=973447),
-   [RFS](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=974217))*\
-[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python3-radexreader)\
+[Debian python-radexreader.deb](https://packages.debian.org/python3-radexreader)\
+[Fedora python-radexreader.rpm](https://src.fedoraproject.org/rpms/python-radexreader)\
 [openSUSE python-radexreader.rpm](https://software.opensuse.org/package/python-radexreader)\
 [Ubuntu PPA](https://launchpad.net/~luigifab/+archive/ubuntu/packages)
 
 This program is provided under the terms of the **GNU GPLv2+** license.\
 If you like, take some of your time to improve some translations, go to https://bit.ly/2HyCCEc.
-
-
```

### Comparing `radexreader-1.2.1/setup.py` & `radexreader-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf8 -*-
 # Created L/19/10/2020
-# Updated M/10/08/2021
+# Updated V/24/12/2021
 #
-# Copyright 2020-2021 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
+# Copyright 2020-2023 | Fabrice Creuzot (luigifab) <code~luigifab~fr>
 # https://github.com/luigifab/python-radexreader
-# https://www.luigifab.fr/python/radexreader
 #
 # This program is free software, you can redistribute it or modify
 # it under the terms of the GNU General Public License (GPL) as published
 # by the free software foundation, either version 2 of the license, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -23,29 +22,29 @@
 	from distutils.core import setup
 
 try:
 	with open('README.md', 'r') as fh:
 		long_description = fh.read().replace('(images/', '(https://raw.githubusercontent.com/luigifab/python-radexreader/master/images/')
 	setup(
 		name='radexreader',
-		version='1.2.1',
+		version='1.2.2',
 		description='Python library for the RADEX RD1212 and the RADEX ONE Geiger counters.',
 		long_description=long_description,
 		long_description_content_type='text/markdown',
 		license='GPL 2',
 		author='Fabrice Creuzot',
 		author_email='code@luigifab.fr',
 		url='https://github.com/luigifab/python-radexreader',
 		packages=['radexreader'],
 		install_requires=['pyusb', 'pyserial']
 	)
 except:
 	setup(
 		name='radexreader',
-		version='1.2.1',
+		version='1.2.2',
 		description='Python library for the RADEX RD1212 and the RADEX ONE Geiger counters.',
 		license='GPL 2',
 		author='Fabrice Creuzot',
 		author_email='code@luigifab.fr',
 		url='https://github.com/luigifab/python-radexreader',
 		packages=['radexreader'],
 		install_requires=['pyusb', 'pyserial']
```

