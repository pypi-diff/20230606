# Comparing `tmp/zipline_norgatedata-2.4.2-py3-none-any.whl.zip` & `tmp/zipline_norgatedata-2.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 36977 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     9474 b- defN 23-May-08 07:24 zipline_norgatedata/CHANGES.txt
+Zip file size: 37179 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     9650 b- defN 23-Jun-06 03:29 zipline_norgatedata/CHANGES.txt
 -rw-rw-rw-  2.0 fat    16020 b- defN 20-Sep-09 09:35 zipline_norgatedata/LICENSE.txt
 -rw-rw-rw-  2.0 fat       62 b- defN 19-Aug-27 04:23 zipline_norgatedata/__init__.py
 -rw-rw-rw-  2.0 fat    10981 b- defN 23-May-01 11:22 zipline_norgatedata/pipelines.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-09 12:01 zipline_norgatedata/version.py
--rw-rw-rw-  2.0 fat    43970 b- defN 23-May-05 08:06 zipline_norgatedata/zipline_norgatedata.py
--rw-rw-rw-  2.0 fat    16020 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    28339 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      990 b- defN 23-May-09 12:02 zipline_norgatedata-2.4.2.dist-info/RECORD
-11 files, 125991 bytes uncompressed, 35279 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-06 03:28 zipline_norgatedata/version.py
+-rw-rw-rw-  2.0 fat    43449 b- defN 23-Jun-06 04:52 zipline_norgatedata/zipline_norgatedata.py
+-rw-rw-rw-  2.0 fat    16020 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    29504 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      990 b- defN 23-Jun-06 05:03 zipline_norgatedata-2.4.3.dist-info/RECORD
+11 files, 126811 bytes uncompressed, 35481 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: zipline_norgatedata/version.py
 Comment: 
 
 Filename: zipline_norgatedata/zipline_norgatedata.py
 Comment: 
 
-Filename: zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT
+Filename: zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: zipline_norgatedata-2.4.2.dist-info/METADATA
+Filename: zipline_norgatedata-2.4.3.dist-info/METADATA
 Comment: 
 
-Filename: zipline_norgatedata-2.4.2.dist-info/WHEEL
+Filename: zipline_norgatedata-2.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: zipline_norgatedata-2.4.2.dist-info/top_level.txt
+Filename: zipline_norgatedata-2.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zipline_norgatedata-2.4.2.dist-info/RECORD
+Filename: zipline_norgatedata-2.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zipline_norgatedata/CHANGES.txt

```diff
@@ -112,8 +112,8 @@
 v2.3.2 20221114 Notes on Juneteenth holiday patch
 v2.3.3 20230122 Notes on TSXFailures patch
 v2.3.4 20230222 Update documentation to specify sqlalchemy<2
 v2.4.0 20230506 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
 v2.4.1 20230507 Minor documentation fixes on installation method
 v2.4.1 20230507 Documentation fixes
 v2.4.2 20230507 Documentation fixes, revised Clenow scripts
-
+v2.4.3 20230606 Revised information on extending backtests to 1970 by patching Zipline, better start/end session handling so that you don't have to be on an actual trading date
```

## zipline_norgatedata/version.py

```diff
@@ -1 +1 @@
-__version__ = '2.4.2'
+__version__ = '2.4.3'
```

## zipline_norgatedata/zipline_norgatedata.py

```diff
@@ -106,37 +106,24 @@
     "FOAT4": "O4", # French govt bond (OAT) - day
     "FOAT9": "O9", # French govt bond (OAT) - Official Close
     "HTW": "TW",  # MSCI Taiwan 
     "HTW4": "T4",  # MSCI Taiwan (Day session)
 
 }
 
-def normalize_daily_start_end_session_OLD(calendar_name, start_session, end_session):
-    if zl.__version__ < '2.2.0':
-        cal = get_calendar(calendar_name)
-    else:
-        cal = get_calendar(calendar_name,start=start_session.strftime("%Y-%m-%d"))
-    if not (cal.is_session(start_session)):
-        # use next close instead of next open due to futures markets that start on Sundays
-        # and we only want daily data
-        start_session = cal.next_close(start_session).floor(freq="D")
-    if not (cal.is_session(end_session)):
-        end_session = cal.previous_close(end_session).floor(freq="D")
-    return start_session, end_session
-
 def normalize_daily_start_end_session(calendar_name, start_session, end_session):
     cal = get_calendar(calendar_name,start=start_session.strftime("%Y-%m-%d"))
-
-    if not (cal.is_session(start_session)):
-        # use next close instead of next open due to futures markets that start on Sundays
-        # and we only want daily data
-        start_session = cal.next_close(start_session).floor(freq="D")
+    if start_session < cal.first_session: # eg. Starts on 1 Jan will be realigned to the first trading day of the year
+        start_session = cal.first_session
+        if start_session.weekday() == 6: # Don't start on Sundays, this helps with futures testing...
+            start_session = cal.next_close(start_session).floor(freq="D")
+        #logger.info("  Realigning start to " + start_session.strftime("%Y-%m-%d"))
     if not (cal.is_session(end_session)):
         end_session = cal.previous_close(end_session).floor(freq="D")
-
+        #logger.info("  Realigning end to " + end_session.strftime("%Y-%m-%d"))
     return start_session, end_session
 
 def define_non_US_country_code(exchanges):
     aulist = ('ASX','AU IDX')
     for exchange in aulist:
         #if exchanges.index.contains(exchange):
         if exchange in exchanges.index:
@@ -698,16 +685,14 @@
 ):
 
     with maybe_show_progress(
         symbols, show_progress, label="Loading Norgate equities:", 
         item_show_func=lambda a:_progress_symbol(a),
     ) as it:
         for sid, symbol in enumerate(it):
-            # 1990 is the maximum here - anything before is not defined as a
-            # session apparently (!)
             # Padding must be all markte days, otherwise it will bork zipline's
             # expection that there's a bar for every day
             asset_name = norgatedata.security_name(symbol)
             exchange = norgatedata.exchange_name(symbol)
             exchange_full = norgatedata.exchange_name_full(symbol)
             df = norgatedata.price_timeseries(
                 symbol,
@@ -991,15 +976,15 @@
             )
             yield sid, df
 
 
 def register_norgatedata_equities_bundle(
     bundlename,
     stock_price_adjustment_setting=norgatedata.StockPriceAdjustmentType.TOTALRETURN,
-    start_session="1990-01-01",
+    start_session="1970-01-01",
     end_session="now",
     calendar_name="NYSE",
     symbol_list=None,
     watchlists=None,
     excluded_symbol_list=None,
 ):
     if not isinstance(start_session, pd.Timestamp):
@@ -1028,15 +1013,15 @@
         end_session=end_session,
         calendar_name=calendar_name,
     )
 
 
 def register_norgatedata_futures_bundle(
     bundlename,
-    start_session="1990-01-01",
+    start_session="1970-01-01",
     end_session="now",
     calendar_name="us_futures",
     symbol_list=None,
     session_symbols=None,
     watchlists=None,
     excluded_symbol_list=None,
 ):
```

## Comparing `zipline_norgatedata-2.4.2.dist-info/LICENSE.TXT` & `zipline_norgatedata-2.4.3.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

## Comparing `zipline_norgatedata-2.4.2.dist-info/METADATA` & `zipline_norgatedata-2.4.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-norgatedata
-Version: 2.4.2
+Version: 2.4.3
 Summary: Zipline extension to provide bundles of data from Norgate Data into the Zipline algorithmic trading library for the Python programming language
 Home-page: https://norgatedata.com
 Author: NorgateData Pty Ltd
 Author-email: support@norgatedata.com
 License: EULA
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Development Status :: 5 - Production/Stable
@@ -95,19 +95,40 @@
 
 Edit exchange_calendars.py
 
 Go to line 51 and change:
 ```
 GLOBAL_DEFAULT_START = pd.Timestamp.now().floor("D") - pd.DateOffset(years=20)
 ```
-to the following (or your desired date)
+to the following:
 ```
-GLOBAL_DEFAULT_START = pd.Timestamp('1950-01-03')
+GLOBAL_DEFAULT_START = pd.Timestamp('1970-01-01')
 ```
 
+
+## Additional patch to allow backtesting before 1990
+
+In addition to the "20 year" patch above if you want to do backtesting prior to 1990 you will need to patch Zipline to handle that too.
+
+Navigate to the zipline folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\ziplines**
+
+Navigate to the subfolder utils.
+
+Edit calendar_utils.py
+
+Go to line 31 and change:
+```
+        return ec_get_calendar(*args, side="right", start=pd.Timestamp("1990-01-01"))
+```
+to the following:
+```
+        return ec_get_calendar(*args, side="right", start=pd.Timestamp("1970-01-01"))
+```
+
+
 ## Patch to allow calendars other than US calendars for backtesting
 
 If you see the message "AssertionError: All readers must share target trading_calendar." then you probably need this patch.  Our testing shows that AU and CA stocks users need this.
 
 Navigate to the zipline folder within site packages.  This is typically located at **C:\Users\<your username>\miniconda3\envs\zip310\Lib\site-packages\zipline**
 
 Navigate to the data subfolder and edit the file dipatch_bar_reader.py
@@ -214,18 +235,19 @@
     bundlename = 'norgatedata-aapl',
     symbol_list = ['AAPL','$SPXTR',], 
     start_session = '1990-01-01',
     end_session = '2020-12-01'
 )
 
 # FANG stocks (Facebook, Amazon, Netflix, Google) - 2012-05-18 until now
+# (is now really MANG !)
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-fang',
-    symbol_list = ['FB','AMZN','NFLX','GOOGL','$SPXTR',], 
-    start_session = '2012-05-18',  # This is that FB first traded
+    symbol_list = ['META','AMZN','NFLX','GOOGL','$SPXTR',], 
+    start_session = '2012-05-18',  # This is that FB (now META) first traded
 )
 
 # A small set of selected ETFs
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-selected-etfs',
     symbol_list = ['SPY','GLD','USO','$SPXTR',],
     start_session = '2006-04-10', # This is the USO first trading date
@@ -234,15 +256,15 @@
 # S&P 500 Bundle for backtesting including all current & past constituents back to 1990
 # and the S&P 500 Total Return index (useful for benchmarking and/or index trend filtering)
 # (around 1800 securities)
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-sp500',
     symbol_list = ['$SPXTR'],
     watchlists = ['S&P 500 Current & Past'],
-    start_session = '1990-01-01',
+    start_session = '1970-01-01',
 )
 
 # Russell 3000 bundle containing all ccurrent & past constituents back to 1990
 # and the Russell 3000 Total Return Index (useful for benchmarking and/or index trend filtering)
 # (about 11000 securities)
 
 register_norgatedata_equities_bundle(
@@ -255,83 +277,32 @@
 # And now a watchlist excluding a given list of symbols
 
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-russell3000-exfroth',
     watchlists = ['Russell 3000 Current & Past'],
     symbol_list = ['$RUATR'],
     start_session = '1990-01-01' ,
-    excluded_symbol_list = ['TSLA','AMZN','FB','NFLX','GOOGL',]
+    excluded_symbol_list = ['TSLA','AMZN','META','NFLX','GOOGL',]
 )
 
 # FUTURES BUNDLES
 
 # Example bundle for all of the individual contracts from three futures markets:
 # E-mini S&P 500, E-mini Nasdaq 100, E-mini Russell 2000,
 # with $SPXTR added for benchmark reference
 register_norgatedata_futures_bundle(
     bundlename = 'norgatedata-selected-index-futures',
     session_symbols = ['ES','NQ','RTY'],
     symbol_list = ['$SPXTR'],
     start_session = '2000-01-01',
 )
-
-
-# Bundle of futures used in Andreas Clenow's Trading Evolved book
-# (contains 6000+ individual futures contracts/deliveries)
-bundlename = 'norgatedata-tradingevolved-futures'
-symbol_list = ['$SPXTR',]
-session_symbols = [
-	'6A', # AUD
-	'6B', # GBP
-	'6C', # CAD
-	'6E', # EUR
-	'DX', # USDX
-	'6J', # JPY
-	'6N', # NZD
-	'6S', # CHF
-	'LBS', # Lumber
-	'ZC', # Corn
-	'CT', # Cotton
-	'GF', # Feeder Cattle
-	'KC', # Coffee
-	'LRC', # Robusta Coffee
-	'LSU', # White Sugar
-	'ZO', # Oats
-	'ZS', # Soybeans
-	'SB', # Sugar
-	'ZM', # Soybean Meal
-	'ZW', # Wheat
-	'CL', # Crude Oil
-	'GC', # Gold
-	'HG', # Copper
-	'HO', # NY Harbor ULSD 
-	'GAS', # Gas Oil
-	'NG', # Henry Hub Natural Gas
-	'PA', # Palladium
-	'PL', # Platinum
-	'RB', # RBOB Gasoline
-	'SI', # Silver
-	'ES', # E-mini S&P 500
-	'NKD', # Nikkei 225 Dollar
-	'NQ', # E-mini Nasdaq-100
-	'STW', # MSCI Taiwan 
-	'VX', # Cboe Volatility Index
-	'YM', # E-mini Dow
-	'GE', # Eurodollar
-	'ZF', # 5-Year US T-Note
-	'ZT', # 2-Year US T-Note
-	'ZN', # 10-Year US T-Note
-	'ZB', # 30-Year US T-Bond        
-]
-start_session = '2000-01-01',
-
-register_norgatedata_futures_bundle(bundlename,start_session,session_symbols = session_symbols, symbol_list = symbol_list )
-
 ```
 
+For more bundle examples, scroll down to "Books/publications that use Zipline, adapted for Norgate Data use" below and download the Trading Evolved examples.
+
 To ingest a bundle:
 
 ```sh
 zipline ingest -b <bundlename>
 ```
 
 # Benchmark against a symbol
@@ -575,14 +546,15 @@
 import norgatedata
 for session_symbol in norgatedata.futures_market_session_symbols():
     print (session_symbol + " " + norgatedata.futures_market_session_name(session_symbol)) 
 ```
 
 # Zipline Limitations/Quirks
 
+- Zipline 2.4.2 is hardcoded ignore dates prior to 1990-01-01.  It can be patched to 1970-01-01, but no cannot go any further since it uses the Unix Epoch (1970-01-01) as the underlying time storage mechanism.
 - Zipline doesn't define all futures markets and doesn't provide any runtime extensibility in this area - you will need to add them to <your_environment>\lib\site-packages\zipline\finance\constants.py if they are not defined.  Be sure to backup this file as it will be overwritten any time you update zipline.
 - Zipline assumes that there are bars for every day of trading.  If a security doesn't trade for a given day (e.g. it was halted/suspended, or simply nobody wanted to trade it), it will be padded with the previous close repeated in the OHLC fields, with volume set to zero.  Consider how this might affect your trading calculations.  
 - Index volumes cannot be accurately ingested due to Zipline trying to convert large volumes to UINTs which are out-of-bounds for UINT32.  Index volumes will be divided by 1000.
 - Any stock whose adjusted volume exceeds the upper bound of UINT32 will be set to the maximum UINT32 value (4294967295).  This only occurs for stocks with a lot of splits and/or very large special dsitributions.
 - Some stocks have adjusted volume values that fall below the boundaries used by winsorize_uint32 (e.g. volume of 8.225255e-05).  You'll see a warning when those stocks are ingested "UserWarning: Ignoring 12911 values because they are out of bounds for uint32".   These are  There's not much we can do here.  For now, just ignore those warnings.
 - Ingestion times could be improved significantly with multiprocessing (this would require Zipline enhancements)
 - Zipline cannot handle negative prices (eg. Crude Oil in 2020) - any such prices will be set to zero.  Most systems would have rolled prior to this strange event anyway.
@@ -649,14 +621,38 @@
 
 ### During a backtest I receive an error ValueError: 'Time Period' is not in list.  How do I fix this?
 
 This can occur when the items in the bundle do not match the latest data in the Norgate Data database.  For stocks, if there are symbol changes within the database then the bundle will have the old symbol but the Norgate database will have the new symbol.    For Futures, there may have been additional futures contracts listed since your previous ingestion and the roll-over algorithm is trying to roll into them.  
 
 The solution is simple:  Ingest the bundle with fresh data.
 
+Also consider putting Norgate Data Updater into manual mode for updating and using the NDU Trigger app to explicitly start NDU and obtain updates.  More information on this can be found here:
+https://norgatedata.com/ndu-usage.php
+
+
+### During a backtest, an error message is shown for index_constituent_timeseries
+
+For example, an error such as this is shown:
+
+```
+[2023-06-05 07:39:25.720989] INFO: Norgate Data: Populating NorgateDataIndexConstituent pipeline populating with $DJI on 3638 securities from 2000-01-03 to 2023-06-02....
+[2023-06-05 07:39:34.734116] ERROR: Norgate Data: index_constituent_timeseries: DBD not found
+---------------------------------------------------------------------------
+KeyError Traceback (most recent call last)
+(lots of irrelevant trace messages thereafter)
+```
+
+The Norgate Data database has been updated since you last performed an ingest, and there have been some symbol changes.  In the above example, since the ingest occurred, DBD has been demoted to OTC and has a new symbol of DBDQQ.
+
+The solution is simple:  Ingest the bundle with fresh data.
+
+Also consider putting Norgate Data Updater into manual mode for updating and using the NDU Trigger app to explicitly start NDU and obtain updates.  More information on this can be found here:
+https://norgatedata.com/ndu-usage.php
+
+
 # Change log
 
 Released versions and release dates can be seen here:
 https://pypi.org/project/zipline-norgatedata/#history
 
 The CHANGES.TXT within the package details the changes.
```

