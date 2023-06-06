# Comparing `tmp/eodhd-1.0.8.tar.gz` & `tmp/eodhd-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodhd-1.0.8.tar", last modified: Sun Oct 23 16:35:47 2022, max compression
+gzip compressed data, was "eodhd-1.0.9.tar", last modified: Mon Jan 23 14:52:26 2023, max compression
```

## Comparing `eodhd-1.0.8.tar` & `eodhd-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:35:47.202745 eodhd-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-23 16:35:31.000000 eodhd-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 16:35:31.000000 eodhd-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-10-23 16:35:47.198745 eodhd-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-23 16:35:31.000000 eodhd-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:35:47.198745 eodhd-1.0.8/eodhd/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-10-23 16:35:31.000000 eodhd-1.0.8/eodhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13981 2022-10-23 16:35:31.000000 eodhd-1.0.8/eodhd/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-10-23 16:35:31.000000 eodhd-1.0.8/eodhd/eodhdgraphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-10-23 16:35:31.000000 eodhd-1.0.8/eodhd/websocketclient.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 16:35:47.198745 eodhd-1.0.8/eodhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-23 16:35:47.000000 eodhd-1.0.8/eodhd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 16:35:47.202745 eodhd-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-23 16:35:31.000000 eodhd-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-23 14:52:26.413909 eodhd-1.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-01-19 10:19:09.000000 eodhd-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-01-19 10:19:09.000000 eodhd-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      952 2023-01-23 14:52:26.413909 eodhd-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-01-19 10:19:09.000000 eodhd-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-23 14:52:26.397769 eodhd-1.0.9/eodhd/
+-rw-rw-rw-   0        0        0      252 2023-01-19 10:19:09.000000 eodhd-1.0.9/eodhd/__init__.py
+-rw-rw-rw-   0        0        0    14384 2023-01-19 10:19:09.000000 eodhd-1.0.9/eodhd/apiclient.py
+-rw-rw-rw-   0        0        0     4425 2023-01-19 10:19:09.000000 eodhd-1.0.9/eodhd/eodhdgraphs.py
+-rw-rw-rw-   0        0        0     5884 2023-01-19 10:19:09.000000 eodhd-1.0.9/eodhd/websocketclient.py
+drwxrwxrwx   0        0        0        0 2023-01-23 14:52:26.412909 eodhd-1.0.9/eodhd.egg-info/
+-rw-rw-rw-   0        0        0      952 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       99 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-01-23 14:52:26.000000 eodhd-1.0.9/eodhd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-23 14:52:26.413909 eodhd-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1592 2023-01-23 14:51:52.000000 eodhd-1.0.9/setup.py
```

### Comparing `eodhd-1.0.8/PKG-INFO` & `eodhd-1.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: eodhd
-Version: 1.0.8
-Summary: Official EODHD API Python Library
-Home-page: https://whittle.medium.com
-Author: Michael Whittle
-Author-email: michael@lifecycle-ps.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Official EODHD APIs Python Library
-https://eodhistoricaldata.com
-
-## Installation
-
-    python3 -m pip install eodhd
-
-## Note
-
-Demo API key below is provided by EOD Historial Data for testing purposes
-<https://eodhistoricaldata.com/financial-apis/new-real-time-data-api-websockets>
-
-## Sample code and examples
-
-* example_api.py
-* example_scanner.py
-* example_websockets.py
+Metadata-Version: 2.1
+Name: eodhd
+Version: 1.0.9
+Summary: Official EODHD API Python Library
+Home-page: https://whittle.medium.com
+Author: Michael Whittle, Ivanchenko Gleb
+Author-email: michael@lifecycle-ps.com, kross_10@mail.ru
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Official EODHD APIs Python Library
+https://eodhistoricaldata.com
+
+## Installation
+
+    python3 -m pip install eodhd
+
+## Note
+
+Demo API key below is provided by EOD Historial Data for testing purposes
+<https://eodhistoricaldata.com/financial-apis/new-real-time-data-api-websockets>
+
+## Sample code and examples
+
+* example_api.py
+* example_scanner.py
+* example_websockets.py
```

### Comparing `eodhd-1.0.8/eodhd/apiclient.py` & `eodhd-1.0.9/eodhd/apiclient.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,403 +1,403 @@
-"""apiclient.py"""
-
-from json.decoder import JSONDecodeError
-import sys
-from enum import Enum
-from datetime import datetime
-from datetime import timedelta
-from re import compile as re_compile
-import pandas as pd
-import numpy as np
-from requests import get as requests_get
-from requests import ConnectionError as requests_ConnectionError
-from requests import Timeout as requests_Timeout
-from requests.exceptions import HTTPError as requests_HTTPError
-from rich.console import Console
-from rich.progress import track
-
-# minimal traceback
-sys.tracebacklimit = 1
-
-
-class Interval(Enum):
-    """Enum: infraday"""
-
-    MINUTE = "1m"
-    FIVEMINUTES = "5m"
-    HOUR = "1h"
-    ONEDAY = "1d"
-
-
-class DateUtils:
-    """Utility class"""
-
-    @staticmethod
-    def str2datetime(_datetime: str):
-        """Convert yyyy-mm-dd hh:mm:ss to datetime"""
-
-        # Validate string datetime
-        prog = re_compile(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
-        if not prog.match(_datetime):
-            raise ValueError("Incorrect datetime format: yyyy-mm-dd hh:mm:ss")
-
-        return datetime.strptime(_datetime, "%Y-%m-%d %H:%M:%S")
-
-    @staticmethod
-    def str2epoch(_datetime: str):
-        """Convert yyyy-mm-dd hh:mm:ss to datetime"""
-
-        # Validate string datetime
-        prog = re_compile(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
-        if not prog.match(_datetime):
-            raise ValueError("Incorrect datetime format: yyyy-mm-dd hh:mm:ss")
-
-        return int(datetime.strptime(_datetime, "%Y-%m-%d %H:%M:%S").timestamp())
-
-    @staticmethod
-    def previous_day_last_second():
-        """Returns the last second of the previous day"""
-
-        yesterday = datetime.today() - timedelta(days=1)
-        return str(yesterday.date()) + " 23:59:59"
-
-    @staticmethod
-    def previous_day_last_minute():
-        """Returns the last minute of the previous day"""
-
-        yesterday = datetime.today() - timedelta(days=1)
-        return str(yesterday.date()) + " 23:59:00"
-
-
-class APIClient:
-    """API class"""
-
-    def __init__(self, api_key: str) -> None:
-        # Validate API key
-        prog = re_compile(r"^[A-z0-9.]{16,32}$")
-        if api_key != "demo" and not prog.match(api_key):
-            raise ValueError("API key is invalid")
-
-        self._api_key = api_key
-        self._api_url = "https://eodhistoricaldata.com/api"
-
-        self.console = Console()
-
-    def _rest_get(self, endpoint: str = "", uri: str = "", querystring: str = "") -> pd.DataFrame():
-        """Generic REST GET"""
-
-        if endpoint.strip() == "":
-            raise ValueError("endpoint is empty!")
-
-        try:
-            resp = requests_get(f"{self._api_url}/{endpoint}/{uri}?api_token={self._api_key}&fmt=json{querystring}")
-
-            if resp.status_code != 200:
-                try:
-                    if "message" in resp.json():
-                        resp_message = resp.json()["message"]
-                    elif "errors" in resp.json():
-                        self.console.log(resp.json())
-                        sys.exit(1)
-                    else:
-                        resp_message = ""
-
-                    message = f"({resp.status_code}) {self._api_url} - {resp_message}"
-                    self.console.log(message)
-
-                except JSONDecodeError as err:
-                    self.console.log(err)
-
-            try:
-                resp.raise_for_status()
-
-                if isinstance(resp.json(), list):
-                    return pd.DataFrame.from_dict(resp.json())
-                else:
-                    return pd.DataFrame(resp.json(), index=[0])
-
-            except ValueError as err:
-                self.console.log(err)
-
-        except requests_ConnectionError as err:
-            self.console.log(err)
-        except requests_HTTPError as err:
-            self.console.log(err)
-        except requests_Timeout as err:
-            self.console.log(err)
-        return pd.DataFrame()
-
-    def get_exchanges(self) -> pd.DataFrame:
-        """Get supported exchanges"""
-
-        return self._rest_get("exchanges-list")
-
-    def get_exchange_symbols(self, uri: str = "") -> pd.DataFrame:
-        """Get supported exchange symbols"""
-
-        try:
-            if uri.strip() == "":
-                raise ValueError("endpoint uri is empty!")
-
-            return self._rest_get("exchange-symbol-list", uri)
-        except ValueError as err:
-            self.console.log(err)
-            return pd.DataFrame()
-
-    def get_historical_data(
-        self,
-        symbol: str,
-        interval: str = Interval,
-        range_start: str = "",
-        range_end: str = "",
-    ) -> dict:
-        """Initiates a REST API call"""
-
-        # default set of results
-        results = 300
-
-        # validate symbol
-        prog = re_compile(r"^[A-z0-9-$\.+]{1,48}$")
-        if not prog.match(symbol):
-            raise ValueError(f"Symbol is invalid: {symbol}")
-
-        # replace "." with "-" in markets
-        if symbol.count(".") == 2:
-            symbol = symbol.replace(".", "-", 1)
-
-        minutes = 1
-        if interval == "5m":
-            minutes = 5
-        elif interval == "1h":
-            minutes = 60
-
-        # validate interval
-        try:
-            Interval(interval)
-        except ValueError as err:
-            self.console.log(err)
-            return pd.DataFrame()
-
-        if interval == "1d":
-            prog = re_compile(r"^\d{4}\-\d{2}-\d{2}$")
-
-            if range_end == "" or (range_end != "" and not prog.match(range_end)):
-                date_to = datetime.today().date()
-            else:
-                try:
-                    date_to = datetime.strptime(range_end, "%Y-%m-%d").date()
-                except ValueError:
-                    self.console.log("invalid end date (yyyy-mm-dd):", range_end)
-                    sys.exit()
-
-            if range_start == "" or (range_start != "" and not prog.match(range_start)):
-                date_from = date_to - timedelta(days=(results - 1))
-            else:
-                try:
-                    date_from = datetime.strptime(range_start, "%Y-%m-%d").date()
-                except ValueError:
-                    self.console.log("invalid start date (yyyy-mm-dd):", range_start)
-                    sys.exit()
-
-            df_data = self._rest_get(
-                "eod",
-                symbol,
-                f"&interval={interval}&from={str(date_from)}&to={str(date_to)}",
-            )
-
-        else:
-            prog = re_compile(r"^\d{4}\-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
-
-            if range_end == "" or (range_end != "" and not prog.match(range_end)):
-                epoch_to = ""
-            else:
-                try:
-                    epoch_to = int(datetime.strptime(range_end, "%Y-%m-%d %H:%M:%S").timestamp())
-                except ValueError:
-                    self.console.log("invalid end date (yyyy-mm-dd hh:mm:ss):", range_end)
-                    sys.exit()
-
-            if range_start == "" or (range_start != "" and not prog.match(range_start)):
-                if interval == "1m":
-                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=1)).split(".")[0]))
-                elif interval == "5m":
-                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=2)).split(".")[0]))
-                elif interval == "1h":
-                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=14)).split(".")[0]))
-                else:
-                    epoch_from = str(int(epoch_to) - (((60 * minutes) * results) - ((60 * minutes) + 1)))
-            else:
-                try:
-                    epoch_from = int(datetime.strptime(range_start, "%Y-%m-%d %H:%M:%S").timestamp())
-                except ValueError:
-                    self.console.log("invalid start date (yyyy-mm-dd hh:mm:ss):", range_start)
-                    sys.exit()
-
-            if epoch_to != "":
-                df_data = self._rest_get(
-                    "intraday",
-                    symbol,
-                    f"&interval={interval}&from={str(epoch_from)}&to={str(epoch_to)}",
-                )
-            else:
-                df_data = self._rest_get(
-                    "intraday",
-                    symbol,
-                    f"&interval={interval}&from={str(epoch_from)}",
-                )
-
-            if len(df_data) == 0:
-                return df_data[
-                    [
-                        "symbol",
-                        "interval",
-                        "open",
-                        "high",
-                        "low",
-                        "close",
-                        "adjusted_close",
-                        "volume",
-                    ]
-                ]
-
-            if range_start == "" and range_end == "":
-                df_data = df_data.tail(300)
-            elif range_start != "" and range_end == "":
-                df_data = df_data.head(300)
-
-        df_data["symbol"] = symbol
-        df_data["interval"] = interval
-
-        # convert dataframe to a time series
-        if interval == "1d":
-            tsidx = pd.DatetimeIndex(pd.to_datetime(df_data["date"]).dt.strftime("%Y-%m-%d"))
-            df_data.set_index(tsidx, inplace=True)
-            df_data = df_data.drop(columns=["date"])
-        else:
-            tsidx = pd.DatetimeIndex(pd.to_datetime(df_data["datetime"]).dt.strftime("%Y-%m-%d %H:%M:%S"))
-            df_data.set_index(tsidx, inplace=True)
-            df_data = df_data.drop(columns=["datetime"])
-
-        # rename columns
-        if interval != "1d":
-            df_data.columns = [
-                "epoch",
-                "gmtoffset",
-                "open",
-                "high",
-                "low",
-                "close",
-                "volume",
-                "symbol",
-                "interval",
-            ]
-
-        # return dataset
-        if interval == "1d":
-            df_data["adjusted_close"] = df_data["adjusted_close"].astype(object)
-            df_data.fillna(0, inplace=True)
-
-            return df_data[
-                [
-                    "symbol",
-                    "interval",
-                    "open",
-                    "high",
-                    "low",
-                    "close",
-                    "adjusted_close",
-                    "volume",
-                ]
-            ]
-
-        # set object type to display large floats
-        df_data.fillna(0, inplace=True)
-        df_data["gmtoffset"] = df_data["gmtoffset"].astype(object)
-        df_data["epoch"] = df_data["epoch"].astype(object)
-        df_data["open"] = df_data["open"].astype(object)
-        df_data["high"] = df_data["high"].astype(object)
-        df_data["low"] = df_data["low"].astype(object)
-        df_data["close"] = df_data["close"].astype(object)
-        df_data["volume"] = df_data["volume"].astype(object)
-
-        return df_data[
-            [
-                "epoch",
-                "gmtoffset",
-                "symbol",
-                "interval",
-                "open",
-                "high",
-                "low",
-                "close",
-                "volume",
-            ]
-        ]
-
-
-class ScannerClient:
-    """Scanner class"""
-
-    def __init__(self, api_key: str) -> None:
-        # Validate API key
-        prog = re_compile(r"^[A-z0-9.]{16,32}$")
-        if api_key != "demo" and not prog.match(api_key):
-            raise ValueError("API key is invalid")
-
-        self.api = APIClient(api_key)
-
-    def scan_markets(
-        self,
-        market_type: str = "CC",
-        interval: str = Interval,
-        quote_currency: str = "USD",
-        request_limit: int = 5000,
-    ):
-        """Scan markets"""
-
-        if request_limit < 0 or request_limit > 100000:
-            raise ValueError("request limit is out of bounds!")
-
-        df_dataset = pd.DataFrame()
-
-        resp = self.api.get_exchange_symbols(market_type)
-        symbol_list = resp[resp.Code.str.endswith(f"-{quote_currency}", na=False)].Code.to_numpy()
-
-        if request_limit > 0:
-            # truncate symbol list to request limit minus symbol list request
-            symbol_list = symbol_list[0 : request_limit - 1]
-
-        for symbol in track(symbol_list, description="Processing..."):
-            df_data = self.api.get_historical_data(f"{symbol}.{market_type}", interval)
-            if len(df_data) >= 200:
-
-                df_data["sma50"] = df_data.adjusted_close.rolling(50, min_periods=1).mean()
-                df_data["sma200"] = df_data.adjusted_close.rolling(200, min_periods=1).mean()
-                df_data["bull_market"] = df_data.sma50 >= df_data.sma200
-
-                df_data["ema12"] = df_data.adjusted_close.ewm(span=12, adjust=False).mean()
-                df_data["ema26"] = df_data.adjusted_close.ewm(span=26, adjust=False).mean()
-                df_data.loc[df_data["ema12"] > df_data["ema26"], "next_action"] = "sell"
-                df_data["next_action"].fillna("buy", inplace=True)
-
-                high_low = df_data["high"] - df_data["low"]
-                high_close = abs(df_data["high"] - df_data["adjusted_close"].shift())
-                low_close = abs(df_data["low"] - df_data["adjusted_close"].shift())
-                ranges = pd.concat([high_low, high_close, low_close], axis=1)
-                true_range = np.max(ranges, axis=1)
-                df_data["atr14"] = true_range.rolling(14).sum() / 14
-                df_data["atr14_pcnt"] = (df_data["atr14"] / df_data["adjusted_close"] * 100).round(2)
-
-                df_dataset = df_dataset.append(df_data.tail(1))
-
-        # drop infinite values
-        df_dataset.replace([np.inf, -np.inf], np.nan, inplace=True)
-        df_dataset.dropna(subset=["atr14_pcnt"], inplace=True)
-
-        df_dataset.sort_values(
-            by=["bull_market", "next_action", "volume", "atr14_pcnt"],
-            ascending=[False, True, False, False],
-            inplace=True,
-        )
-        df_dataset.to_csv("dataset.csv")
-
-        return df_dataset
+"""apiclient.py"""
+
+from json.decoder import JSONDecodeError
+import sys
+from enum import Enum
+from datetime import datetime
+from datetime import timedelta
+from re import compile as re_compile
+import pandas as pd
+import numpy as np
+from requests import get as requests_get
+from requests import ConnectionError as requests_ConnectionError
+from requests import Timeout as requests_Timeout
+from requests.exceptions import HTTPError as requests_HTTPError
+from rich.console import Console
+from rich.progress import track
+
+# minimal traceback
+sys.tracebacklimit = 1
+
+
+class Interval(Enum):
+    """Enum: infraday"""
+
+    MINUTE = "1m"
+    FIVEMINUTES = "5m"
+    HOUR = "1h"
+    ONEDAY = "1d"
+
+
+class DateUtils:
+    """Utility class"""
+
+    @staticmethod
+    def str2datetime(_datetime: str):
+        """Convert yyyy-mm-dd hh:mm:ss to datetime"""
+
+        # Validate string datetime
+        prog = re_compile(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
+        if not prog.match(_datetime):
+            raise ValueError("Incorrect datetime format: yyyy-mm-dd hh:mm:ss")
+
+        return datetime.strptime(_datetime, "%Y-%m-%d %H:%M:%S")
+
+    @staticmethod
+    def str2epoch(_datetime: str):
+        """Convert yyyy-mm-dd hh:mm:ss to datetime"""
+
+        # Validate string datetime
+        prog = re_compile(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
+        if not prog.match(_datetime):
+            raise ValueError("Incorrect datetime format: yyyy-mm-dd hh:mm:ss")
+
+        return int(datetime.strptime(_datetime, "%Y-%m-%d %H:%M:%S").timestamp())
+
+    @staticmethod
+    def previous_day_last_second():
+        """Returns the last second of the previous day"""
+
+        yesterday = datetime.today() - timedelta(days=1)
+        return str(yesterday.date()) + " 23:59:59"
+
+    @staticmethod
+    def previous_day_last_minute():
+        """Returns the last minute of the previous day"""
+
+        yesterday = datetime.today() - timedelta(days=1)
+        return str(yesterday.date()) + " 23:59:00"
+
+
+class APIClient:
+    """API class"""
+
+    def __init__(self, api_key: str) -> None:
+        # Validate API key
+        prog = re_compile(r"^[A-z0-9.]{16,32}$")
+        if api_key != "demo" and not prog.match(api_key):
+            raise ValueError("API key is invalid")
+
+        self._api_key = api_key
+        self._api_url = "https://eodhistoricaldata.com/api"
+
+        self.console = Console()
+
+    def _rest_get(self, endpoint: str = "", uri: str = "", querystring: str = "") -> pd.DataFrame():
+        """Generic REST GET"""
+
+        if endpoint.strip() == "":
+            raise ValueError("endpoint is empty!")
+
+        try:
+            resp = requests_get(f"{self._api_url}/{endpoint}/{uri}?api_token={self._api_key}&fmt=json{querystring}")
+
+            if resp.status_code != 200:
+                try:
+                    if "message" in resp.json():
+                        resp_message = resp.json()["message"]
+                    elif "errors" in resp.json():
+                        self.console.log(resp.json())
+                        sys.exit(1)
+                    else:
+                        resp_message = ""
+
+                    message = f"({resp.status_code}) {self._api_url} - {resp_message}"
+                    self.console.log(message)
+
+                except JSONDecodeError as err:
+                    self.console.log(err)
+
+            try:
+                resp.raise_for_status()
+
+                if isinstance(resp.json(), list):
+                    return pd.DataFrame.from_dict(resp.json())
+                else:
+                    return pd.DataFrame(resp.json(), index=[0])
+
+            except ValueError as err:
+                self.console.log(err)
+
+        except requests_ConnectionError as err:
+            self.console.log(err)
+        except requests_HTTPError as err:
+            self.console.log(err)
+        except requests_Timeout as err:
+            self.console.log(err)
+        return pd.DataFrame()
+
+    def get_exchanges(self) -> pd.DataFrame:
+        """Get supported exchanges"""
+
+        return self._rest_get("exchanges-list")
+
+    def get_exchange_symbols(self, uri: str = "") -> pd.DataFrame:
+        """Get supported exchange symbols"""
+
+        try:
+            if uri.strip() == "":
+                raise ValueError("endpoint uri is empty!")
+
+            return self._rest_get("exchange-symbol-list", uri)
+        except ValueError as err:
+            self.console.log(err)
+            return pd.DataFrame()
+
+    def get_historical_data(
+        self,
+        symbol: str,
+        interval: str = Interval,
+        range_start: str = "",
+        range_end: str = "",
+    ) -> dict:
+        """Initiates a REST API call"""
+
+        # default set of results
+        results = 300
+
+        # validate symbol
+        prog = re_compile(r"^[A-z0-9-$\.+]{1,48}$")
+        if not prog.match(symbol):
+            raise ValueError(f"Symbol is invalid: {symbol}")
+
+        # replace "." with "-" in markets
+        if symbol.count(".") == 2:
+            symbol = symbol.replace(".", "-", 1)
+
+        minutes = 1
+        if interval == "5m":
+            minutes = 5
+        elif interval == "1h":
+            minutes = 60
+
+        # validate interval
+        try:
+            Interval(interval)
+        except ValueError as err:
+            self.console.log(err)
+            return pd.DataFrame()
+
+        if interval == "1d":
+            prog = re_compile(r"^\d{4}\-\d{2}-\d{2}$")
+
+            if range_end == "" or (range_end != "" and not prog.match(range_end)):
+                date_to = datetime.today().date()
+            else:
+                try:
+                    date_to = datetime.strptime(range_end, "%Y-%m-%d").date()
+                except ValueError:
+                    self.console.log("invalid end date (yyyy-mm-dd):", range_end)
+                    sys.exit()
+
+            if range_start == "" or (range_start != "" and not prog.match(range_start)):
+                date_from = date_to - timedelta(days=(results - 1))
+            else:
+                try:
+                    date_from = datetime.strptime(range_start, "%Y-%m-%d").date()
+                except ValueError:
+                    self.console.log("invalid start date (yyyy-mm-dd):", range_start)
+                    sys.exit()
+
+            df_data = self._rest_get(
+                "eod",
+                symbol,
+                f"&interval={interval}&from={str(date_from)}&to={str(date_to)}",
+            )
+
+        else:
+            prog = re_compile(r"^\d{4}\-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
+
+            if range_end == "" or (range_end != "" and not prog.match(range_end)):
+                epoch_to = ""
+            else:
+                try:
+                    epoch_to = int(datetime.strptime(range_end, "%Y-%m-%d %H:%M:%S").timestamp())
+                except ValueError:
+                    self.console.log("invalid end date (yyyy-mm-dd hh:mm:ss):", range_end)
+                    sys.exit()
+
+            if range_start == "" or (range_start != "" and not prog.match(range_start)):
+                if interval == "1m":
+                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=1)).split(".")[0]))
+                elif interval == "5m":
+                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=2)).split(".")[0]))
+                elif interval == "1h":
+                    epoch_from = str(DateUtils.str2epoch(str(datetime.now() - timedelta(days=14)).split(".")[0]))
+                else:
+                    epoch_from = str(int(epoch_to) - (((60 * minutes) * results) - ((60 * minutes) + 1)))
+            else:
+                try:
+                    epoch_from = int(datetime.strptime(range_start, "%Y-%m-%d %H:%M:%S").timestamp())
+                except ValueError:
+                    self.console.log("invalid start date (yyyy-mm-dd hh:mm:ss):", range_start)
+                    sys.exit()
+
+            if epoch_to != "":
+                df_data = self._rest_get(
+                    "intraday",
+                    symbol,
+                    f"&interval={interval}&from={str(epoch_from)}&to={str(epoch_to)}",
+                )
+            else:
+                df_data = self._rest_get(
+                    "intraday",
+                    symbol,
+                    f"&interval={interval}&from={str(epoch_from)}",
+                )
+
+            if len(df_data) == 0:
+                return df_data[
+                    [
+                        "symbol",
+                        "interval",
+                        "open",
+                        "high",
+                        "low",
+                        "close",
+                        "adjusted_close",
+                        "volume",
+                    ]
+                ]
+
+            if range_start == "" and range_end == "":
+                df_data = df_data.tail(300)
+            elif range_start != "" and range_end == "":
+                df_data = df_data.head(300)
+
+        df_data["symbol"] = symbol
+        df_data["interval"] = interval
+
+        # convert dataframe to a time series
+        if interval == "1d":
+            tsidx = pd.DatetimeIndex(pd.to_datetime(df_data["date"]).dt.strftime("%Y-%m-%d"))
+            df_data.set_index(tsidx, inplace=True)
+            df_data = df_data.drop(columns=["date"])
+        else:
+            tsidx = pd.DatetimeIndex(pd.to_datetime(df_data["datetime"]).dt.strftime("%Y-%m-%d %H:%M:%S"))
+            df_data.set_index(tsidx, inplace=True)
+            df_data = df_data.drop(columns=["datetime"])
+
+        # rename columns
+        if interval != "1d":
+            df_data.columns = [
+                "epoch",
+                "gmtoffset",
+                "open",
+                "high",
+                "low",
+                "close",
+                "volume",
+                "symbol",
+                "interval",
+            ]
+
+        # return dataset
+        if interval == "1d":
+            df_data["adjusted_close"] = df_data["adjusted_close"].astype(object)
+            df_data.fillna(0, inplace=True)
+
+            return df_data[
+                [
+                    "symbol",
+                    "interval",
+                    "open",
+                    "high",
+                    "low",
+                    "close",
+                    "adjusted_close",
+                    "volume",
+                ]
+            ]
+
+        # set object type to display large floats
+        df_data.fillna(0, inplace=True)
+        df_data["gmtoffset"] = df_data["gmtoffset"].astype(object)
+        df_data["epoch"] = df_data["epoch"].astype(object)
+        df_data["open"] = df_data["open"].astype(object)
+        df_data["high"] = df_data["high"].astype(object)
+        df_data["low"] = df_data["low"].astype(object)
+        df_data["close"] = df_data["close"].astype(object)
+        df_data["volume"] = df_data["volume"].astype(object)
+
+        return df_data[
+            [
+                "epoch",
+                "gmtoffset",
+                "symbol",
+                "interval",
+                "open",
+                "high",
+                "low",
+                "close",
+                "volume",
+            ]
+        ]
+
+
+class ScannerClient:
+    """Scanner class"""
+
+    def __init__(self, api_key: str) -> None:
+        # Validate API key
+        prog = re_compile(r"^[A-z0-9.]{16,32}$")
+        if api_key != "demo" and not prog.match(api_key):
+            raise ValueError("API key is invalid")
+
+        self.api = APIClient(api_key)
+
+    def scan_markets(
+        self,
+        market_type: str = "CC",
+        interval: str = Interval,
+        quote_currency: str = "USD",
+        request_limit: int = 5000,
+    ):
+        """Scan markets"""
+
+        if request_limit < 0 or request_limit > 100000:
+            raise ValueError("request limit is out of bounds!")
+
+        df_dataset = pd.DataFrame()
+
+        resp = self.api.get_exchange_symbols(market_type)
+        symbol_list = resp[resp.Code.str.endswith(f"-{quote_currency}", na=False)].Code.to_numpy()
+
+        if request_limit > 0:
+            # truncate symbol list to request limit minus symbol list request
+            symbol_list = symbol_list[0 : request_limit - 1]
+
+        for symbol in track(symbol_list, description="Processing..."):
+            df_data = self.api.get_historical_data(f"{symbol}.{market_type}", interval)
+            if len(df_data) >= 200:
+
+                df_data["sma50"] = df_data.adjusted_close.rolling(50, min_periods=1).mean()
+                df_data["sma200"] = df_data.adjusted_close.rolling(200, min_periods=1).mean()
+                df_data["bull_market"] = df_data.sma50 >= df_data.sma200
+
+                df_data["ema12"] = df_data.adjusted_close.ewm(span=12, adjust=False).mean()
+                df_data["ema26"] = df_data.adjusted_close.ewm(span=26, adjust=False).mean()
+                df_data.loc[df_data["ema12"] > df_data["ema26"], "next_action"] = "sell"
+                df_data["next_action"].fillna("buy", inplace=True)
+
+                high_low = df_data["high"] - df_data["low"]
+                high_close = abs(df_data["high"] - df_data["adjusted_close"].shift())
+                low_close = abs(df_data["low"] - df_data["adjusted_close"].shift())
+                ranges = pd.concat([high_low, high_close, low_close], axis=1)
+                true_range = np.max(ranges, axis=1)
+                df_data["atr14"] = true_range.rolling(14).sum() / 14
+                df_data["atr14_pcnt"] = (df_data["atr14"] / df_data["adjusted_close"] * 100).round(2)
+
+                df_dataset = df_dataset.append(df_data.tail(1))
+
+        # drop infinite values
+        df_dataset.replace([np.inf, -np.inf], np.nan, inplace=True)
+        df_dataset.dropna(subset=["atr14_pcnt"], inplace=True)
+
+        df_dataset.sort_values(
+            by=["bull_market", "next_action", "volume", "atr14_pcnt"],
+            ascending=[False, True, False, False],
+            inplace=True,
+        )
+        df_dataset.to_csv("dataset.csv")
+
+        return df_dataset
```

### Comparing `eodhd-1.0.8/eodhd/eodhdgraphs.py` & `eodhd-1.0.9/eodhd/eodhdgraphs.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-"""graphs.py"""
-
-from operator import truediv
-import pandas as pd
-import matplotlib.pyplot as plt
-
-
-class EODHDGraphs:
-    """Graph class"""
-
-    @staticmethod
-    def fibonacci_extension(df: pd.DataFrame = None, trend_direction: str = "uptrend", price_field: str = "close", save_file: str = "", quiet: bool = False) -> None:
-        """Fibonacci retracement"""
-
-        if trend_direction not in ["uptrend", "downtrend"]:
-            raise ValueError("trend_direction must be either uptrend or downtrend")
-
-        if price_field not in ["close", "adjusted_close"]:
-            raise ValueError("price_field must be either close or adjusted_close")
-
-        low = df[price_field].min()
-        high = df[price_field].max()
-        diff = high - low
-
-        if trend_direction == "uptrend":
-            fib2618 = high + (diff * 2.618)
-            fib2000 = high + (diff * 2)
-            fib1618 = high + (diff * 1.618)
-            fib1382 = high + (diff * 1.382)
-            fib1000 = high + (diff * 1)
-            fib618 = high + (diff * 0.618)
-        elif trend_direction == "downtrend":
-            fib2618 = low - (diff * 2.618)
-            fib2000 = low - (diff * 2)
-            fib1618 = low - (diff * 1.618)
-            fib1382 = low - (diff * 1.382)
-            fib1000 = low - (diff * 1)
-            fib618 = low - (diff * 0.618)
-
-        plt.figure(figsize=(30, 10))
-        plt.plot(df["adjusted_close"], color="black", label="Price")
-        plt.axhline(y=fib2618, color="limegreen", linestyle="-", label="261.8%")
-        plt.axhline(y=fib2000, color="slateblue", linestyle="-", label="200%")
-        plt.axhline(y=fib1618, color="mediumvioletred", linestyle="-", label="161.8%")
-        plt.axhline(y=fib1382, color="gold", linestyle="-", label="138.2%")
-        plt.axhline(y=fib1000, color="dodgerblue", linestyle="-", label="100%")
-        plt.axhline(y=fib618, color="darkturquoise", linestyle="-", label="61.8%")
-
-        plt.ylabel("Price")
-        plt.xticks(rotation=90)
-        plt.title(f"Fibonacci Extension ({trend_direction})")
-        plt.legend()
-
-        if save_file:
-            plt.savefig(save_file)
-
-        if quiet is False:
-            plt.show()
-
-    @staticmethod
-    def fibonacci_retracement(df: pd.DataFrame = None, trend_direction: str = "uptrend", price_field: str = "close", save_file: str = "", quiet: bool = False) -> None:
-        """Fibonacci retracement"""
-
-        if trend_direction not in ["uptrend", "downtrend"]:
-            raise ValueError("trend_direction must be either uptrend or downtrend")
-
-        if price_field not in ["close", "adjusted_close"]:
-            raise ValueError("price_field must be either close or adjusted_close")
-
-        low = df[price_field].min()
-        high = df[price_field].max()
-        diff = high - low
-
-        if trend_direction == "uptrend":
-            fib0 = high
-            fib236 = high - (diff * 0.236)
-            fib382 = high - (diff * 0.382)
-            fib50 = high - (diff * 0.5)
-            fib618 = high - (diff * 0.618)
-            fib764 = high - (diff * 0.764)
-            fib100 = low
-        elif trend_direction == "downtrend":
-            fib100 = high
-            fib764 = low + (diff * 0.764)
-            fib618 = low + (diff * 0.618)
-            fib50 = low + (diff * 0.5)
-            fib382 = low + (diff * 0.382)
-            fib236 = low + (diff * 0.236)
-            fib0 = low
-
-        plt.figure(figsize=(30, 10))
-        plt.plot(df["adjusted_close"], color="black", label="Price")
-        plt.axhline(y=fib100, color="limegreen", linestyle="-", label="100%")
-        plt.axhline(y=fib764, color="slateblue", linestyle="-", label="76.4%")
-        plt.axhline(y=fib618, color="mediumvioletred", linestyle="-", label="61.8%")
-        plt.axhline(y=fib50, color="gold", linestyle="-", label="50%")
-        plt.axhline(y=fib382, color="dodgerblue", linestyle="-", label="38.2%")
-        plt.axhline(y=fib236, color="darkturquoise", linestyle="-", label="23.6%")
-        plt.axhline(y=fib0, color="lightcoral", linestyle="-", label="0%")
-
-        plt.ylabel("Price")
-        plt.xticks(rotation=90)
-        plt.title(f"Fibonacci Retracement ({trend_direction})")
-        plt.legend()
-
-        if save_file:
-            plt.savefig(save_file)
-
-        if quiet is False:
-            plt.show()
+"""graphs.py"""
+
+from operator import truediv
+import pandas as pd
+import matplotlib.pyplot as plt
+
+
+class EODHDGraphs:
+    """Graph class"""
+
+    @staticmethod
+    def fibonacci_extension(df: pd.DataFrame = None, trend_direction: str = "uptrend", price_field: str = "close", save_file: str = "", quiet: bool = False) -> None:
+        """Fibonacci retracement"""
+
+        if trend_direction not in ["uptrend", "downtrend"]:
+            raise ValueError("trend_direction must be either uptrend or downtrend")
+
+        if price_field not in ["close", "adjusted_close"]:
+            raise ValueError("price_field must be either close or adjusted_close")
+
+        low = df[price_field].min()
+        high = df[price_field].max()
+        diff = high - low
+
+        if trend_direction == "uptrend":
+            fib2618 = high + (diff * 2.618)
+            fib2000 = high + (diff * 2)
+            fib1618 = high + (diff * 1.618)
+            fib1382 = high + (diff * 1.382)
+            fib1000 = high + (diff * 1)
+            fib618 = high + (diff * 0.618)
+        elif trend_direction == "downtrend":
+            fib2618 = low - (diff * 2.618)
+            fib2000 = low - (diff * 2)
+            fib1618 = low - (diff * 1.618)
+            fib1382 = low - (diff * 1.382)
+            fib1000 = low - (diff * 1)
+            fib618 = low - (diff * 0.618)
+
+        plt.figure(figsize=(30, 10))
+        plt.plot(df["adjusted_close"], color="black", label="Price")
+        plt.axhline(y=fib2618, color="limegreen", linestyle="-", label="261.8%")
+        plt.axhline(y=fib2000, color="slateblue", linestyle="-", label="200%")
+        plt.axhline(y=fib1618, color="mediumvioletred", linestyle="-", label="161.8%")
+        plt.axhline(y=fib1382, color="gold", linestyle="-", label="138.2%")
+        plt.axhline(y=fib1000, color="dodgerblue", linestyle="-", label="100%")
+        plt.axhline(y=fib618, color="darkturquoise", linestyle="-", label="61.8%")
+
+        plt.ylabel("Price")
+        plt.xticks(rotation=90)
+        plt.title(f"Fibonacci Extension ({trend_direction})")
+        plt.legend()
+
+        if save_file:
+            plt.savefig(save_file)
+
+        if quiet is False:
+            plt.show()
+
+    @staticmethod
+    def fibonacci_retracement(df: pd.DataFrame = None, trend_direction: str = "uptrend", price_field: str = "close", save_file: str = "", quiet: bool = False) -> None:
+        """Fibonacci retracement"""
+
+        if trend_direction not in ["uptrend", "downtrend"]:
+            raise ValueError("trend_direction must be either uptrend or downtrend")
+
+        if price_field not in ["close", "adjusted_close"]:
+            raise ValueError("price_field must be either close or adjusted_close")
+
+        low = df[price_field].min()
+        high = df[price_field].max()
+        diff = high - low
+
+        if trend_direction == "uptrend":
+            fib0 = high
+            fib236 = high - (diff * 0.236)
+            fib382 = high - (diff * 0.382)
+            fib50 = high - (diff * 0.5)
+            fib618 = high - (diff * 0.618)
+            fib764 = high - (diff * 0.764)
+            fib100 = low
+        elif trend_direction == "downtrend":
+            fib100 = high
+            fib764 = low + (diff * 0.764)
+            fib618 = low + (diff * 0.618)
+            fib50 = low + (diff * 0.5)
+            fib382 = low + (diff * 0.382)
+            fib236 = low + (diff * 0.236)
+            fib0 = low
+
+        plt.figure(figsize=(30, 10))
+        plt.plot(df["adjusted_close"], color="black", label="Price")
+        plt.axhline(y=fib100, color="limegreen", linestyle="-", label="100%")
+        plt.axhline(y=fib764, color="slateblue", linestyle="-", label="76.4%")
+        plt.axhline(y=fib618, color="mediumvioletred", linestyle="-", label="61.8%")
+        plt.axhline(y=fib50, color="gold", linestyle="-", label="50%")
+        plt.axhline(y=fib382, color="dodgerblue", linestyle="-", label="38.2%")
+        plt.axhline(y=fib236, color="darkturquoise", linestyle="-", label="23.6%")
+        plt.axhline(y=fib0, color="lightcoral", linestyle="-", label="0%")
+
+        plt.ylabel("Price")
+        plt.xticks(rotation=90)
+        plt.title(f"Fibonacci Retracement ({trend_direction})")
+        plt.legend()
+
+        if save_file:
+            plt.savefig(save_file)
+
+        if quiet is False:
+            plt.show()
```

### Comparing `eodhd-1.0.8/eodhd/websocketclient.py` & `eodhd-1.0.9/eodhd/websocketclient.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-"""websocketclient.py"""
-
-import re
-import json
-from time import sleep
-from datetime import datetime
-from threading import Thread
-from websocket import create_connection, WebSocketConnectionClosedException
-
-class WebSocketClient():
-    """WebSocket class"""
-
-    # pylint: disable=too-many-instance-attributes
-    # Eleven is reasonable in this case
-
-    def __init__(
-        self,
-        api_key: str,
-        endpoint: str,
-        symbols: list,
-    ) -> None:
-        super().__init__()
-
-        # Validate API key
-        prog = re.compile(r"^[A-z0-9.]{16,32}$")
-        if not prog.match(api_key):
-            raise ValueError("API key is invalid")
-
-        # Validate endpoint
-        if endpoint not in ["us","us_quote","forex","crypto"]:
-            raise ValueError("Endpoint is invalid")
-
-        # Validate symbol list
-        if len(symbols) == 0:
-            raise ValueError("No symbol(s) provided")
-
-        # Validate individual symbols
-        prog = re.compile(r"^[A-z0-9-$]{1,48}$")
-        for symbol in symbols:
-            if not prog.match(symbol):
-                raise ValueError(f"Symbol is invalid: {symbol}")
-
-        # Validate max symbol subscriptions
-        if len(symbols) > 50:
-            raise ValueError("Max symbol subscription count is 50!")
-
-        # Map class arguments to private variables
-        self._api_key = api_key
-        self._endpoint = endpoint
-        self._symbols = symbols
-
-        # Statistical variables
-        self.start_time = None
-        self.time_elapsed = 0
-        self.message_count = 0
-
-        # WebSocket variables
-        self.stop = None
-        self.thread = None
-        self.keepalive = None
-        self.websocket = None
-        self.message = None
-
-    # Public functions
-
-    def start(self):
-        """Initialise websocket"""
-
-        def _go():
-            self._connect()
-            self._listen()
-            self._disconnect()
-
-        self.stop = False
-        self.on_open()
-        self.thread = Thread(target=_go)
-        self.keepalive = Thread(target=self._keepalive)
-        self.thread.start()
-
-    def close(self):
-        """Close websocket"""
-
-        self.stop = True
-        self.start_time = None
-        self.time_elapsed = 0
-        self._disconnect()
-        self.thread.join()
-
-    # Private functions
-
-    def _connect(self):
-        """Connect to websocket"""
-
-        self.websocket = create_connection(
-            f"wss://ws.eodhistoricaldata.com/ws/{self._endpoint}?api_token={self._api_key}"
-        )
-        self.websocket.send(
-            json.dumps(
-                {
-                    "action": "subscribe",
-                    "symbols": ",".join(self._symbols),
-                }
-            )
-        )
-        self.start_time = datetime.now()
-
-    def _listen(self):
-        """Listen to websocket"""
-
-        self.keepalive.start()
-        while not self.stop:
-            try:
-                data = self.websocket.recv()
-                if data != "":
-                    msg = json.loads(data)
-                else:
-                    msg = {}
-            except ValueError as error_msg:
-                self.on_error(error_msg)
-            except Exception as error_msg: # pylint: disable=broad-except
-                self.on_error(error_msg)
-            else:
-                self.on_message(msg)
-
-    def _keepalive(self, interval=30):
-        """WebSocket keepalive"""
-
-        while self.websocket.connected:
-            self.websocket.ping("keepalive")
-            sleep(interval)
-
-    def _disconnect(self):
-        """Disconnect websocket"""
-
-        try:
-            if self.websocket:
-                self.websocket.close()
-        except WebSocketConnectionClosedException:
-            pass
-        finally:
-            self.keepalive.join()
-
-    # Events
-
-    def on_close(self):
-        """WebSocket on-close event"""
-
-        print("-- WebSocket Closed --")
-
-    def on_error(self, error_msg, data=None):
-        """WebSocket on_error event"""
-
-        print(f"{error_msg} - data: {data}")
-
-        self.stop = True
-        try:
-            self.websocket = None
-            self.start_time = None
-            self.time_elapsed = 0
-        except: # pylint: disable=bare-except
-            pass
-
-    def on_open(self):
-        """WebSocket on-open event"""
-
-        self.message_count = 0
-
-    def on_message(self, msg):
-        """WebSocket on-message event"""
-
-        if self.start_time is not None:
-            self.time_elapsed = round(
-                (datetime.now()-self.start_time).total_seconds()
-            )
-        self.message_count += 1
-        self.message = msg
-        #print (self.message_count, msg)
-
-    # Getters
-
-    def get_start_time(self) -> datetime:
-        """Start time getter"""
-
-        return self.start_time
-
-    def get_time_elapsed(self) -> int:
-        """Time elapsed getter"""
-
-        return self.time_elapsed
-
-
-def main() -> None:
-    """Main"""
-
-    websocket = WebSocketClient(
-        # Demo API key for testing purposes
-        api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="crypto", symbols=["BTC-USD"]
-        #api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="forex", symbols=["EURUSD"]
-        #api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="us", symbols=["AAPL"]
-    )
-    websocket.start()
-
-    message_count = 0
-    while True:
-        if websocket:
-            if (
-                message_count != websocket.message_count
-            ):
-                print(websocket.message)
-                message_count = websocket.message_count
-                sleep(0.25)  # output every 1/4 second, websocket is realtime
-
-if __name__ == "__main__":
-    main()
+"""websocketclient.py"""
+
+import re
+import json
+from time import sleep
+from datetime import datetime
+from threading import Thread
+from websocket import create_connection, WebSocketConnectionClosedException
+
+class WebSocketClient():
+    """WebSocket class"""
+
+    # pylint: disable=too-many-instance-attributes
+    # Eleven is reasonable in this case
+
+    def __init__(
+        self,
+        api_key: str,
+        endpoint: str,
+        symbols: list,
+    ) -> None:
+        super().__init__()
+
+        # Validate API key
+        prog = re.compile(r"^[A-z0-9.]{16,32}$")
+        if not prog.match(api_key):
+            raise ValueError("API key is invalid")
+
+        # Validate endpoint
+        if endpoint not in ["us","us_quote","forex","crypto"]:
+            raise ValueError("Endpoint is invalid")
+
+        # Validate symbol list
+        if len(symbols) == 0:
+            raise ValueError("No symbol(s) provided")
+
+        # Validate individual symbols
+        prog = re.compile(r"^[A-z0-9-$]{1,48}$")
+        for symbol in symbols:
+            if not prog.match(symbol):
+                raise ValueError(f"Symbol is invalid: {symbol}")
+
+        # Validate max symbol subscriptions
+        if len(symbols) > 50:
+            raise ValueError("Max symbol subscription count is 50!")
+
+        # Map class arguments to private variables
+        self._api_key = api_key
+        self._endpoint = endpoint
+        self._symbols = symbols
+
+        # Statistical variables
+        self.start_time = None
+        self.time_elapsed = 0
+        self.message_count = 0
+
+        # WebSocket variables
+        self.stop = None
+        self.thread = None
+        self.keepalive = None
+        self.websocket = None
+        self.message = None
+
+    # Public functions
+
+    def start(self):
+        """Initialise websocket"""
+
+        def _go():
+            self._connect()
+            self._listen()
+            self._disconnect()
+
+        self.stop = False
+        self.on_open()
+        self.thread = Thread(target=_go)
+        self.keepalive = Thread(target=self._keepalive)
+        self.thread.start()
+
+    def close(self):
+        """Close websocket"""
+
+        self.stop = True
+        self.start_time = None
+        self.time_elapsed = 0
+        self._disconnect()
+        self.thread.join()
+
+    # Private functions
+
+    def _connect(self):
+        """Connect to websocket"""
+
+        self.websocket = create_connection(
+            f"wss://ws.eodhistoricaldata.com/ws/{self._endpoint}?api_token={self._api_key}"
+        )
+        self.websocket.send(
+            json.dumps(
+                {
+                    "action": "subscribe",
+                    "symbols": ",".join(self._symbols),
+                }
+            )
+        )
+        self.start_time = datetime.now()
+
+    def _listen(self):
+        """Listen to websocket"""
+
+        self.keepalive.start()
+        while not self.stop:
+            try:
+                data = self.websocket.recv()
+                if data != "":
+                    msg = json.loads(data)
+                else:
+                    msg = {}
+            except ValueError as error_msg:
+                self.on_error(error_msg)
+            except Exception as error_msg: # pylint: disable=broad-except
+                self.on_error(error_msg)
+            else:
+                self.on_message(msg)
+
+    def _keepalive(self, interval=30):
+        """WebSocket keepalive"""
+
+        while self.websocket.connected:
+            self.websocket.ping("keepalive")
+            sleep(interval)
+
+    def _disconnect(self):
+        """Disconnect websocket"""
+
+        try:
+            if self.websocket:
+                self.websocket.close()
+        except WebSocketConnectionClosedException:
+            pass
+        finally:
+            self.keepalive.join()
+
+    # Events
+
+    def on_close(self):
+        """WebSocket on-close event"""
+
+        print("-- WebSocket Closed --")
+
+    def on_error(self, error_msg, data=None):
+        """WebSocket on_error event"""
+
+        print(f"{error_msg} - data: {data}")
+
+        self.stop = True
+        try:
+            self.websocket = None
+            self.start_time = None
+            self.time_elapsed = 0
+        except: # pylint: disable=bare-except
+            pass
+
+    def on_open(self):
+        """WebSocket on-open event"""
+
+        self.message_count = 0
+
+    def on_message(self, msg):
+        """WebSocket on-message event"""
+
+        if self.start_time is not None:
+            self.time_elapsed = round(
+                (datetime.now()-self.start_time).total_seconds()
+            )
+        self.message_count += 1
+        self.message = msg
+        #print (self.message_count, msg)
+
+    # Getters
+
+    def get_start_time(self) -> datetime:
+        """Start time getter"""
+
+        return self.start_time
+
+    def get_time_elapsed(self) -> int:
+        """Time elapsed getter"""
+
+        return self.time_elapsed
+
+
+def main() -> None:
+    """Main"""
+
+    websocket = WebSocketClient(
+        # Demo API key for testing purposes
+        api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="crypto", symbols=["BTC-USD"]
+        #api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="forex", symbols=["EURUSD"]
+        #api_key="OeAFFmMliFG5orCUuwAKQ8l4WWFQ67YX", endpoint="us", symbols=["AAPL"]
+    )
+    websocket.start()
+
+    message_count = 0
+    while True:
+        if websocket:
+            if (
+                message_count != websocket.message_count
+            ):
+                print(websocket.message)
+                message_count = websocket.message_count
+                sleep(0.25)  # output every 1/4 second, websocket is realtime
+
+if __name__ == "__main__":
+    main()
```

### Comparing `eodhd-1.0.8/eodhd.egg-info/PKG-INFO` & `eodhd-1.0.9/eodhd.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: eodhd
-Version: 1.0.8
-Summary: Official EODHD API Python Library
-Home-page: https://whittle.medium.com
-Author: Michael Whittle
-Author-email: michael@lifecycle-ps.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Official EODHD APIs Python Library
-https://eodhistoricaldata.com
-
-## Installation
-
-    python3 -m pip install eodhd
-
-## Note
-
-Demo API key below is provided by EOD Historial Data for testing purposes
-<https://eodhistoricaldata.com/financial-apis/new-real-time-data-api-websockets>
-
-## Sample code and examples
-
-* example_api.py
-* example_scanner.py
-* example_websockets.py
+Metadata-Version: 2.1
+Name: eodhd
+Version: 1.0.9
+Summary: Official EODHD API Python Library
+Home-page: https://whittle.medium.com
+Author: Michael Whittle, Ivanchenko Gleb
+Author-email: michael@lifecycle-ps.com, kross_10@mail.ru
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Official EODHD APIs Python Library
+https://eodhistoricaldata.com
+
+## Installation
+
+    python3 -m pip install eodhd
+
+## Note
+
+Demo API key below is provided by EOD Historial Data for testing purposes
+<https://eodhistoricaldata.com/financial-apis/new-real-time-data-api-websockets>
+
+## Sample code and examples
+
+* example_api.py
+* example_scanner.py
+* example_websockets.py
```

### Comparing `eodhd-1.0.8/setup.py` & `eodhd-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""Setup file for PyPI"""
-
-# To use a consistent encoding
-from os import path
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-
-# The directory containing this file
-HERE = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-
-# This call to setup() does all the work
-setup(
-    name="eodhd",
-    version="1.0.8",
-    description="Official EODHD API Python Library",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://whittle.medium.com",
-    author="Michael Whittle",
-    author_email="michael@lifecycle-ps.com",
-    license="MIT",
-    classifiers=[
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(include=["eodhd"]),
-    include_package_data=True,
-    install_requires=[
-        "websockets==10.3",
-        "websocket-client==1.3.3",
-        "requests==2.28.1",
-        "rich==12.5.1",
-        "pandas==1.3.5",
-        "numpy==1.21.6",
-    ],
-    entry_points={
-        "console_scripts": [
-            "whittlem=eodhd.__main__:main",
-        ]
-    },
-    setup_requires=["pytest-runner==6.0.0"],
-    tests_require=["pytest==7.1.2"],
-    test_suite="tests",
-)
+"""Setup file for PyPI"""
+
+# To use a consistent encoding
+from os import path
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+
+# The directory containing this file
+HERE = path.abspath(path.dirname(__file__))
+
+# Get the long description from the README file
+with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
+
+# This call to setup() does all the work
+setup(
+    name="eodhd",
+    version="1.0.9",
+    description="Official EODHD API Python Library",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://whittle.medium.com",
+    author="Michael Whittle, Ivanchenko Gleb",
+    author_email="michael@lifecycle-ps.com, kross_10@mail.ru",
+    license="MIT",
+    classifiers=[
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Operating System :: OS Independent",
+    ],
+    packages=find_packages(include=["eodhd"]),
+    include_package_data=True,
+    install_requires=[
+        "websockets==10.3",
+        "websocket-client==1.3.3",
+        "requests==2.28.1",
+        "rich==12.5.1",
+        "pandas==1.5.1",
+        "numpy==1.24.1",
+    ],
+    entry_points={
+        "console_scripts": [
+            "whittlem=eodhd.__main__:main",
+        ]
+    },
+    setup_requires=["pytest-runner==6.0.0"],
+    tests_require=["pytest==7.1.2"],
+    test_suite="tests",
+)
```

