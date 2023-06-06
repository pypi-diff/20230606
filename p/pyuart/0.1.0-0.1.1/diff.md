# Comparing `tmp/pyuart-0.1.0-py3-none-any.whl.zip` & `tmp/pyuart-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5083 bytes, number of entries: 5
+Zip file size: 5015 bytes, number of entries: 5
 -rw-r--r--  2.0 unx     4723 b- defN 23-Jun-06 09:04 pyuart/__init__.py
--rw-r--r--  2.0 unx     4831 b- defN 23-Jun-06 09:06 pyuart-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 09:06 pyuart-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-06 09:06 pyuart-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      368 b- defN 23-Jun-06 09:06 pyuart-0.1.0.dist-info/RECORD
-5 files, 10021 bytes uncompressed, 4397 bytes compressed:  56.1%
+-rw-r--r--  2.0 unx     4700 b- defN 23-Jun-06 09:14 pyuart-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 09:14 pyuart-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-06 09:14 pyuart-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      368 b- defN 23-Jun-06 09:14 pyuart-0.1.1.dist-info/RECORD
+5 files, 9890 bytes uncompressed, 4329 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pyuart/__init__.py
 Comment: 
 
-Filename: pyuart-0.1.0.dist-info/METADATA
+Filename: pyuart-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyuart-0.1.0.dist-info/WHEEL
+Filename: pyuart-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyuart-0.1.0.dist-info/top_level.txt
+Filename: pyuart-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyuart-0.1.0.dist-info/RECORD
+Filename: pyuart-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyuart-0.1.0.dist-info/METADATA` & `pyuart-0.1.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuart
-Version: 0.1.0
+Version: 0.1.1
 Summary: a simple UART library for python3
 Home-page: https://github.com/arkedge/pyuart
 Author: Tsuyoshi Hamada
 Author-email: hamada@arkedgespace.com
 License: MIT
 Keywords: pyuart uart
 Platform: UNKNOWN
@@ -39,86 +39,80 @@
 ## 前提
 
 ```1 Byte == 1 Octet == 8 bit```
 
 ## Installation
 
 ```
-make setup
-make chmod
-```
-
-OSS公開後には以下のインストール方法が使える予定
-```
 pip install pyuart
+sudo chmod 666 /dev/ttyUSB0
 ```
 
-```make chmod```は環境依存です。/dev/serial/* やlsusbなど駆使してUSB-TTL converterデバイスを探しましょう。 
-詳細はMakefileを読むと理解の助けになるでしょう。
+上記例のデバイスファイル名 ```/dev/ttyUSB0```は環境依存です。ご自身の環境に対応したデバイスファイル名をご指定ください。
 
 
 ## サンプル
 
-```aelib/uart```モジュールの操作方法のサンプルコードを以下にメモしておきます。
+```pyuart```モジュールの操作方法のサンプルコードを以下にメモしておきます。
 このサンプルを見るだけで動かすことができるはずですが、詳細な説明は後日記載する予定です。
 
 
 ### 例1: 1 octetづつTx(送信)したい場合
 
 ```:test_tx.py
-from aelib import uart
+from pyuart import uart
 
-u0 = uart.uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
+u0 = uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
 u0.open()
 
 u0.tx(1)
 u0.tx(2)
 u0.tx(77)
 
 u0.close()
 
 ```
 
 ### 例2: 1 octetづつRx(受信)したい場合
 
 ```:test_rx.py
-from aelib import uart
+from pyuart import uart
 
-u0 = uart.uart(dev='/dev/ttyS0', baudrate = 115200, timeout = 240)
+u0 = uart(dev='/dev/ttyS0', baudrate = 115200, timeout = 240)
 u0.open()
 
 for data in u0.rx():
     print (data)
 
 u0.close()
 
 ```
 
 ※: rx()メソッドはジェネレータです。
 
 ### 例3: ファイルをTx(送信)したい場合
 
 ```:sample.tx.file.py
-from aelib import uart
+from pyuart import uart
 
-u0 = uart.uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
+u0 = uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
 u0.open()
 
 u0.tx_file(filename = '/tmp/file.bin')
 
 u0.close()
 
 ```
 
 ### 例4: ファイルをRx(受信)したい場合
 
 ```sample.rx.file.py
-from aelib import uart
+from pyuart import uart
 
-u0 = uart.uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
+u0 = uart(dev='/dev/ttyUSB0', baudrate = 115200, timeout = 15)
 u0.open()
 
 u0.rx_file(filename = './recv.bin', n_byte = 1048576)
 
 u0.close()
 
 ```
@@ -134,25 +128,25 @@
 
 
 ### 例5: 並列Txの実行 (MPI利用)
 
 ```mpi.tx.py
 #!/usr/bin/env python3
 from mpi4py import MPI
-from aelib import uart
+from pyuart import uart
 
 comm = MPI.COMM_WORLD
 proc_id = comm.Get_rank()
 nproc = comm.Get_size()
 hostname = MPI.Get_processor_name()
 
 devfile = "/dev/ttyUSB%d" % proc_id
 print(devfile, flush=True)
 
-u0 = uart.uart(dev=devfile, baudrate = 115200, timeout = 15)
+u0 = uart(dev=devfile, baudrate = 115200, timeout = 15)
 u0.open()
 u0.tx(123)
 
 u0.close()
 
 ```
```

