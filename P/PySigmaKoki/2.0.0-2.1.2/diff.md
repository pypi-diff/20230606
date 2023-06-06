# Comparing `tmp/PySigmaKoki-2.0.0.tar.gz` & `tmp/PySigmaKoki-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PySigmaKoki-2.0.0.tar", last modified: Fri Jul 20 07:43:06 2018, max compression
+gzip compressed data, was "PySigmaKoki-2.1.2.tar", last modified: Mon May 22 09:07:39 2023, max compression
```

## Comparing `PySigmaKoki-2.0.0.tar` & `PySigmaKoki-2.1.2.tar`

### file list

```diff
@@ -1,4 +1,12 @@
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2018-07-20 07:43:06.000000 PySigmaKoki-2.0.0/
--rw-r--r--   0 oxon       (501) staff       (20)      536 2018-07-20 07:43:06.000000 PySigmaKoki-2.0.0/PKG-INFO
--rw-r--r--   0 oxon       (501) staff       (20)     7524 2018-07-20 01:09:58.000000 PySigmaKoki-2.0.0/sigma_koki.py
--rw-r--r--   0 oxon       (501) staff       (20)      691 2018-07-20 07:42:38.000000 PySigmaKoki-2.0.0/setup.py
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-05-22 09:07:39.504839 PySigmaKoki-2.1.2/
+-rw-r--r--   0 oxon       (501) staff       (20)      507 2023-05-22 09:07:39.504489 PySigmaKoki-2.1.2/PKG-INFO
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-05-22 09:07:39.503969 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/
+-rw-r--r--   0 oxon       (501) staff       (20)      507 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/PKG-INFO
+-rw-r--r--   0 oxon       (501) staff       (20)      206 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/SOURCES.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        1 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/dependency_links.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        9 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/requires.txt
+-rw-r--r--   0 oxon       (501) staff       (20)       11 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/top_level.txt
+-rw-r--r--   0 oxon       (501) staff       (20)      384 2018-07-20 01:12:39.000000 PySigmaKoki-2.1.2/README.md
+-rw-r--r--   0 oxon       (501) staff       (20)       38 2023-05-22 09:07:39.504943 PySigmaKoki-2.1.2/setup.cfg
+-rw-r--r--   0 oxon       (501) staff       (20)      691 2023-05-17 06:13:42.000000 PySigmaKoki-2.1.2/setup.py
+-rw-r--r--   0 oxon       (501) staff       (20)    10732 2023-05-17 06:00:32.000000 PySigmaKoki-2.1.2/sigma_koki.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PySigmaKoki-2.0.0/sigma_koki.py` & `PySigmaKoki-2.1.2/sigma_koki.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,248 @@
 """
 This is an interface module for instruments produced by Sigma Koki
 """
 
 try:
+    # It is not needed to import ValueError in newer Python versions
     from exceptions import ValueError
 except:
     pass
 import serial
 import sys
 
-class GSC02(object):
+class BaseStageController(object):
     """
-    Stage controller GSC-02
+    Stage controller class commonly used for Sigma Koki GSC02 and SHOT702
     """
-    def __init__(self):
-        self.__baudRate = 9600 # 9600 bps
+    def __init__(self, baudrate, product):
+        self.__baudRate = baudrate
         self.__parityBit = 'N' # None
         self.__dataBit = 8
         self.__stopBit = 1
         self.__rtscts = True
+        self.__product = product
+        self.__acknowledge =  True
 
     def setBaudRate(self, rate):
-        if rate in (2400, 4800, 9600, 19200):
+        if product == 'GSC-02' and rate in (2400, 4800, 9600, 19200):
+            self.__baudRate = rate
+        elif product == 'SHOT-702' and rate == 38400:
             self.__baudRate = rate
         else:
-            raise ValueError('Invalid buard rate %d was given. Must be chosen from 2400/4800/9600/19200.' % rate)
+            raise ValueError('Attempting to set an invalid buard rate %d to %s. Must be chosen from 2400/4800/9600/19200 for GSC-02 and 38400 for SHOT-702.' % (rate, self.__product))
+
+    def disableAcknowledge(self):
+        self.__acknowledge = False
+
+    def write(self, command, acknowledge=True):
+        # 'str' class needs be converted into 'bytes'
+        # e.g., 'command' -> b'command'
+        self.serial.write((command + '\r\n').encode())
+
+        if not self.__acknowledge or not acknowledge:
+            return
+        
+        ack = self.readline()
+        if ack == 'OK':
+            return
+        else:
+            raise RuntimeError('%s returned bad acknowledge "%s"' % (self.__product, ack))
+
+    def query(self, command):
+        self.write(command, False)
+        return self.readline()
+
+    def readline(self):
+        # convert 'bytes' to 'str'
+        result = str(self.serial.readline())
+        if result[:2] == "b'" and result[-1:] == "'":
+            result = result[2:-1] # drop byte code prefix and suffix
+        if result[-4:] == '\\r\\n':
+            result = result[:-4] # drop delimeter
+
+        return result
 
     def open(self, port, readTimeOut = 1, writeTimeOut = 1):
         self.serial = serial.Serial(port         = port,
                                     baudrate     = self.__baudRate,
                                     bytesize     = self.__dataBit,
                                     parity       = self.__parityBit,
                                     stopbits     = self.__stopBit,
                                     timeout      = readTimeOut,
                                     writeTimeout = writeTimeOut,
                                     rtscts       = self.__rtscts)
 
-    def write(self, command):
-        self.serial.write(command + b'\r\n')
-
-    def readline(self):
-        return self.serial.readline()[:-2]
+    def close(self):
+        self.serial.close()
 
     def returnToMechanicalOrigin(self, stage1, stage2):
         """
         Moves the stages to the +/- end points and reset the coordinate values
         to zero.
         """
-        if stage1 == b'+' and stage2 == b'+':
-            self.write(b'H:W++')
-        elif stage1 == b'+' and stage2 == b'-':
-            self.write(b'H:W+-')
-        elif stage1 == b'-' and stage2 == b'+':
-            self.write(b'H:W-+')
-        elif stage1 == b'-' and stage2 == b'-':
-            self.write(b'H:W--')
-        elif stage1 == b'+':
-            self.write(b'H:1+')
-        elif stage1 == b'-':
-            self.write(b'H:1-')
-        elif stage2 == b'+':
-            self.write(b'H:2+')
-        elif stage2 == b'-':
-            self.write(b'H:2-')
-        else:
-            return
+        if self.__product == 'GSC-02':
+            if stage1 == '+' and stage2 == '+':
+                self.write('H:W++')
+            elif stage1 == '+' and stage2 == '-':
+                self.write('H:W+-')
+            elif stage1 == '-' and stage2 == '+':
+                self.write('H:W-+')
+            elif stage1 == '-' and stage2 == '-':
+                self.write('H:W--')
+            elif stage1 == '+':
+                self.write('H:1+')
+            elif stage1 == '-':
+                self.write('H:1-')
+            elif stage2 == '+':
+                self.write('H:2+')
+            elif stage2 == '-':
+                self.write('H:2-')
+            else:
+                return
+        elif self.__product == 'SHOT-702':
+            if stage1 == True and stage2 == True:
+                self.write('H:W')
+            elif stage1 == True:
+                self.write('H:1')
+            elif stage2 == True:
+                self.write('H:2')
+            else:
+                return
 
     def move(self, stage1, stage2):
         """
         Moves the stages with the specified values. Since GSC-02 is a half-step
         stepping driver, 1 pulse corresponds to "half-step movement" in the
         stage catalogues.
         """
-        if not (-16777214 <= stage1 <= 16777214):
-            raise ValueError('stage1 must be between -16777214 and 16777214.')
+        if self.__product == 'GSC-02':
+            limit = 16777214
+        elif self.__product == 'SHOT-702':
+            limit = 268435455
+
+        if not (-limit <= stage1 <= limit):
+            raise ValueError('stage1 must be between -%d and %d.' % (limit, limit))
 
-        if not (-16777214 <= stage2 <= 16777214):
-            raise ValueError('stage2 must be between -16777214 and 16777214.')
+        if not (-limit <= stage2 <= limit):
+            raise ValueError('stage2 must be between -%d and %d.' % (limit, limit))
 
-        command = b'M:W'
+        command = 'M:W'
         if stage1 >= 0:
-            command += b'+P%d' % stage1
+            command += '+P%d' % stage1
         else:
-            command += b'-P%d' % -stage1
+            command += '-P%d' % -stage1
 
         if stage2 >= 0:
-            command += b'+P%d' % stage2
+            command += '+P%d' % stage2
         else:
-            command += b'-P%d' % -stage2
+            command += '-P%d' % -stage2
 
         self.write(command)
         self.go()
 
     def jog(self, stage1, stage2):
         """
         Moves the stages continuously at the minimum speed.
         stage1: '+' positive direction, '-' negative direction
         stage2: '+' positive direction, '-' negative direction
         If other values are given, stages will not move.
         """
-        if stage1 == b'+' and stage2 == b'+':
-            self.write(b'J:W++')
-        elif stage1 == b'+' and stage2 == b'-':
-            self.write(b'J:W+-')
-        elif stage1 == b'-' and stage2 == b'+':
-            self.write(b'J:W-+')
-        elif stage1 == b'-' and stage2 == b'-':
-            self.write(b'J:W--')
-        elif stage1 == b'+':
-            self.write(b'J:1+')
-        elif stage1 == b'-':
-            self.write(b'J:1-')
-        elif stage2 == b'+':
-            self.write(b'J:2+')
-        elif stage2 == b'-':
-            self.write(b'J:2-')
+        if stage1 == '+' and stage2 == '+':
+            self.write('J:W++')
+        elif stage1 == '+' and stage2 == '-':
+            self.write('J:W+-')
+        elif stage1 == '-' and stage2 == '+':
+            self.write('J:W-+')
+        elif stage1 == '-' and stage2 == '-':
+            self.write('J:W--')
+        elif stage1 == '+':
+            self.write('J:1+')
+        elif stage1 == '-':
+            self.write('J:1-')
+        elif stage2 == '+':
+            self.write('J:2+')
+        elif stage2 == '-':
+            self.write('J:2-')
         else:
             return
         
         self.go()
 
     def go(self):
         """
         Moves the stages. To be used internally.
         """
-        self.write(b'G')
+        self.write('G')
 
     def decelerate(self, stage1, stage2):
         """
         Decelerates and stop the stages. 
         """
         if stage1 and stage2:
-            self.write(b'L:W')
+            self.write('L:W')
         elif stage1:
-            self.write(b'L:1')
+            self.write('L:1')
         elif stage2:
-            self.write(b'L:2')
+            self.write('L:2')
 
     def stop(self):
         """
         Stops the stages immediately.
         """
-        self.write(b'L:E')
+        self.write('L:E')
 
     def initializeOrigin(self, stage1, stage2):
         """
         Sets the origin to the current position.
         stage1: If true, set the origin of the stage 1 to the current position
         stage2: If true, set the origin of the stage 1 to the current position
         """
         if stage1:
-            self.write(b'R:1')
+            self.write('R:1')
 
         if stage2:
-            self.write(b'R:2')
+            self.write('R:2')
+
+    def enableMotorExcitation(self, stage1 = True, stage2 = False):
+        """
+        Enables motor excitation
+        """
+        if stage1 in (True, False):
+            self.write('C:1%d' % stage1)
+
+        if stage2 in (True, False):
+            self.write('C:2%d' % stage2)
+
+    def getStatus(self):
+        """
+        Returns the status of the controller
+        """
+        return self.query('Q:')
+
+    def getACK3(self):
+        """
+        Returns the status of ACK3
+        """
+        return self.query('!:')
+
+    def getVersion(self):
+        """
+        Returns the ROM version
+        """
+        return self.query('?:V')
+
+class GSC02(BaseStageController):
+    """
+    Stage controller GSC-02
+    """
+    def __init__(self):
+        # 9600 bps the initial factory setting
+        BaseStageController.__init__(self, 9600, 'GSC-02')
+        self.disableAcknowledge()
 
     def setSpeed(self, highspeed, minSpeed1, maxSpeed1, accelerationTime1,
                  minSpeed2, maxSpeed2, accelerationTime2):
         """
         Sets the movement speeds of the stages
         highspeed: If true, speed range is 50-20000, else 1-200
         minSpeed1/2: Minimum speed (PPS)
@@ -182,47 +267,48 @@
         else:
             if not (50 <= minSpeed1 <= maxSpeed1 <= 20000):
                 raise ValueError('Must be 50 <= minSpeed1 <= maxSpeed1 <= 20000 in high speed range.')
             if not (50 <= minSpeed2 <= maxSpeed2 <= 20000):
                 raise ValueError('Must be 50 <= minSpeed2 <= maxSpeed2 <= 20000 in high speed range.')
 
         if not (0 <= accelerationTime1 <= 1000):
-            raise ValueError('Must be 00 <= accelerationTime1 <= 1000.')
+            raise ValueError('Must be 0 <= accelerationTime1 <= 1000.')
 
         if not (0 <= accelerationTime2 <= 1000):
-            raise ValueError('Must be 00 <= accelerationTime2 <= 1000.')
+            raise ValueError('Must be 0 <= accelerationTime2 <= 1000.')
 
         if highspeed:
-            self.write(b'D:2S%dF%dR%dS%dF%dR%d' % (minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2))
+            self.write('D:2S%dF%dR%dS%dF%dR%d' % (minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2))
         else:
-            self.write(b'D:1S%dF%dR%dS%dF%dR%d' % (minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2))
+            self.write('D:1S%dF%dR%dS%dF%dR%d' % (minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2))
 
-    def enableMotorExcitation(self, stage1 = True, stage2 = False):
+class SHOT702(BaseStageController):
+    """
+    Stage controller SHOT-702
+    """
+    def __init__(self):
+        # 9600 bps the initial factory setting
+        BaseStageController.__init__(self, 38400, 'SHOT-702')
+
+    def setSpeed(self, minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2):
         """
-        Enables motor excitation
+        Sets the movement speeds of the stages
+        minSpeed1/2: Minimum speed (PPS)
+        maxSpeed1/2: Maximum speed (PPS)
+        accelerationTime1/2: Acceleration time to be taken from min to max (ms)     
         """
-        if stage1 in (True, False):
-            self.write(b'C:1%d' % stage1)
+        if not (1 <= minSpeed1 <= maxSpeed1 <= 500000):
+            raise ValueError('Must be 1 <= minSpeed1 <= maxSpeed1 <= 500000.')
 
-        if stage2 in (True, False):
-            self.write(b'C:2%d' % stage2)
+        if not (1 <= minSpeed2 <= maxSpeed2 <= 500000):
+            raise ValueError('Must be 1 <= minSpeed2 <= maxSpeed2 <= 500000.')
 
-    def getStatus(self):
-        """
-        Returns the status of the controller
-        """
-        self.write(b'Q:')
-        return self.readline()
+        if not (0 <= accelerationTime1 <= 1000):
+            raise ValueError('Must be 0 <= accelerationTime <= 1000.')
 
-    def getACK3(self):
-        """
-        Returns the status of ACK3
-        """
-        self.write(b'!:')
-        return self.readline()
+        if not (0 <= accelerationTime2 <= 1000):
+            raise ValueError('Must be 0 <= accelerationTime <= 1000.')
 
-    def getVersion(self):
-        """
-        Returns the ROM version
-        """
-        self.write(b'?:V')
-        return self.readline()
+        self.write('D:WS%dF%dR%dS%dF%dR%d' % (minSpeed1, maxSpeed1, accelerationTime1, minSpeed2, maxSpeed2, accelerationTime2))
+
+    # Some query commands, ?:P, ?:S, ?:D, and ?:B, are not implemented yet
+
```

### Comparing `PySigmaKoki-2.0.0/setup.py` & `PySigmaKoki-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 import sigma_koki
 
 setup(name='PySigmaKoki',
-      version='2.0.0',
+      version='2.1.2',
       description='Python Interface for Instruments by Sigma Koki',
       author='Akira Okumura',
       author_email='oxon@mac.com',
       license='BSD License',
       platforms=['MacOS :: MacOS X', 'POSIX', 'Windows'],
       url='https://github.com/akira-okumura/PySigmaKoki',
       py_modules=['sigma_koki'],
```

