# Comparing `tmp/inpost-0.1.1.tar.gz` & `tmp/inpost-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.1.1.tar", max compression
+gzip compressed data, was "inpost-0.1.2.tar", max compression
```

## Comparing `inpost-0.1.1.tar` & `inpost-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.1/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.1/inpost/__init__.py
--rw-r--r--   0        0        0    45431 2023-05-30 14:37:20.919384 inpost-0.1.1/inpost/api.py
--rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.1/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     2541 2023-05-30 13:20:30.662182 inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-311.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.1/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.1/inpost/static/__pycache__/friends.cpython-311.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.1/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.1/inpost/static/__pycache__/headers.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.1/inpost/static/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0    44670 2023-05-30 14:13:11.007453 inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-311.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0    11366 2023-05-30 13:20:30.648849 inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-311.pyc
--rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.1/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.1/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.1/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.1/inpost/static/headers.py
--rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.1/inpost/static/notifications.py
--rw-r--r--   0        0        0    28065 2023-05-30 13:26:22.527921 inpost-0.1.1/inpost/static/parcels.py
--rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.1/inpost/static/statuses.py
--rw-r--r--   0        0        0     1072 2023-05-30 14:42:01.554547 inpost-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.1/setup.py
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.2/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.2/inpost/__init__.py
+-rw-r--r--   0        0        0    45431 2023-05-30 14:37:20.919384 inpost-0.1.2/inpost/api.py
+-rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.2/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.2/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.2/inpost/static/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.2/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     2541 2023-05-30 13:20:30.662182 inpost-0.1.2/inpost/static/__pycache__/endpoints.cpython-311.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.2/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.2/inpost/static/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.2/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.2/inpost/static/__pycache__/friends.cpython-311.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.2/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.2/inpost/static/__pycache__/headers.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.2/inpost/static/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.2/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0    44670 2023-05-30 14:13:11.007453 inpost-0.1.2/inpost/static/__pycache__/parcels.cpython-311.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.2/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0    11366 2023-05-30 13:20:30.648849 inpost-0.1.2/inpost/static/__pycache__/statuses.cpython-311.pyc
+-rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.2/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.2/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.2/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.2/inpost/static/headers.py
+-rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.2/inpost/static/notifications.py
+-rw-r--r--   0        0        0    28065 2023-06-06 19:26:21.777511 inpost-0.1.2/inpost/static/parcels.py
+-rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.2/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1072 2023-06-06 19:29:23.915959 inpost-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.2/setup.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.2/PKG-INFO
```

### Comparing `inpost-0.1.1/README.md` & `inpost-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/api.py` & `inpost-0.1.2/inpost/api.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__init__.py` & `inpost-0.1.2/inpost/static/__init__.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/__init__.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/endpoints.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/endpoints.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/exceptions.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/friends.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/friends.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/notifications.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/notifications.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/parcels.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/parcels.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.1.2/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/__pycache__/statuses.cpython-311.pyc` & `inpost-0.1.2/inpost/static/__pycache__/statuses.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/endpoints.py` & `inpost-0.1.2/inpost/static/endpoints.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/exceptions.py` & `inpost-0.1.2/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/friends.py` & `inpost-0.1.2/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/notifications.py` & `inpost-0.1.2/inpost/static/notifications.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/inpost/static/parcels.py` & `inpost-0.1.2/inpost/static/parcels.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._open_code: str | None = parcel_data.get('openCode', None)
         self._qr_code: QRCode | None = QRCode(qrcode_data=parcel_data['qrCode'], logger=self._log) \
             if 'qrCode' in parcel_data else None
         self.stored_date: arrow | None = get(parcel_data['storedDate']) if 'storedDate' in parcel_data else None
         self.pickup_date: arrow | None = get(parcel_data['pickUpDate']) if 'pickUpDate' in parcel_data else None
         self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
             if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
-        self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log) if 'reveiver' in parcel_data else None
+        self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log) if 'receiver' in parcel_data else None
         self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log) if 'sender' in parcel_data else None
         self.pickup_point: PickupPoint = PickupPoint(pickuppoint_data=parcel_data['pickUpPoint'], logger=self._log) \
             if 'pickUpPoint' in parcel_data else None
         self.multi_compartment: MultiCompartment | None = MultiCompartment(
             parcel_data['multiCompartment'], logger=self._log) if 'multiCompartment' in parcel_data else None
         self.is_end_off_week_collection: bool | None = parcel_data.get('endOfWeekCollection', None)
         self.status: ParcelStatus = ParcelStatus[parcel_data['status']] if 'status' in parcel_data else None
```

### Comparing `inpost-0.1.1/inpost/static/statuses.py` & `inpost-0.1.2/inpost/static/statuses.py`

 * *Files identical despite different names*

### Comparing `inpost-0.1.1/pyproject.toml` & `inpost-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.1.1"
+version = "0.1.2"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
```

### Comparing `inpost-0.1.1/setup.py` & `inpost-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.4.0,<10.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'arrow>=1.2.3,<2.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'inpost',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
     'long_description': "\n# Inpost Python\n\nFully async Inpost library using Python 3.10.\n\n\n\n\n## Documentation\n\n[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)\n\n\n## Usage/Examples\n\n\n```python\nfrom inpost.api import Inpost\n\ninp = await Inpost.from_phone_number('555333444')\nawait inp.send_sms_code():\n...\nif await inp.confirm_sms_code(123321):\n   print('Congratulations, you initialized successfully!')\n```\n\n\n## Authors\n\n- [@loboda4450](https://www.github.com/loboda4450)\n- [@mrkazik99](https://www.github.com/mrkazik99)\n\n\n## Used By\n\nThis project is used by the following repos:\n\n[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)\n\n",
     'author': 'loboda4450',
     'author_email': 'loboda4450@gmail.com',
     'maintainer': 'loboda4450',
     'maintainer_email': 'loboda4450@gmail.com',
     'url': 'https://github.com/IFOSSA/inpost-python',
```

### Comparing `inpost-0.1.1/PKG-INFO` & `inpost-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
```

