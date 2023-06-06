# Comparing `tmp/cvxsimulator-0.4.1.tar.gz` & `tmp/cvxsimulator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.4.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.5.0.tar", max compression
```

## Comparing `cvxsimulator-0.4.1.tar` & `cvxsimulator-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-06-01 22:20:45.829135 cvxsimulator-0.4.1/LICENSE
--rw-r--r--   0        0        0     5064 2023-06-01 22:20:45.829135 cvxsimulator-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    14009 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1553 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1148 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1457 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/month.py
--rw-r--r--   0        0        0    19235 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      512 2023-06-01 22:20:45.913135 cvxsimulator-0.4.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-06-01 22:21:10.857277 cvxsimulator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 cvxsimulator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-06 05:24:40.839610 cvxsimulator-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5052 2023-06-06 05:24:40.839610 cvxsimulator-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    16264 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1209 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1457 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/month.py
+-rw-r--r--   0        0        0    19295 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-06-06 05:25:06.343972 cvxsimulator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5639 1970-01-01 00:00:00.000000 cvxsimulator-0.5.0/PKG-INFO
```

### Comparing `cvxsimulator-0.4.1/LICENSE` & `cvxsimulator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.4.1/README.md` & `cvxsimulator-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
-Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
+Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
 ## Modus operandi
 
@@ -20,63 +20,63 @@
 * [Loop through time](#loop-through-time)
 * [Analyse results](#analyse-results)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the builder object
 
-The user defines a builder object by loading a frame of prices 
+The user defines a builder object by loading a frame of prices
 and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.builder import builder
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
-It is also possible to specify a model for trading costs. 
+It is also possible to specify a model for trading costs.
 The builder helps to fill up the frame of positions. Only once done
 we construct the actual portfolio.
 
 ### Loop through time
 
-We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop. 
+We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop.
 Let's start with a first strategy. Each day we choose two names from the universe at random.
 Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
 
 ```python
 for t, state in b:
     # pick two assets at random
     pair = np.random.choice(b.assets, 2, replace=False)
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
-    # update the position 
+    # update the position
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
 t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
-A lot of magic is hidden in the state variable. 
+A lot of magic is hidden in the state variable.
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
-Note that we update the position at the last element in the t list 
+Note that we update the position at the last element in the t list
 using a series of actual stocks rather than weights or cashpositions.
 The builder class also exposes setters for such alternative conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
@@ -86,31 +86,31 @@
 
 ```python
 portfolio = b.build()
 ```
 
 ### Analyse results
 
-The loop above is filling up the desired positions. 
-After triggering the `build()` the resulting portfolio 
+The loop above is filling up the desired positions.
+After triggering the `build()` the resulting portfolio
 is ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ...
-``` 
+```
 
 ## Bypassing the builder
 
-Some may know the positions the portfolio shall enter for eternity. 
+Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
-It is possible to completely bypass this step by submitting 
+It is possible to completely bypass this step by submitting
 a frame of positions together with a frame of prices when creating the portfolio object.
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.portfolio import EquityPortfolio
```

### Comparing `cvxsimulator-0.4.1/cvx/simulator/builder.py` & `cvxsimulator-0.5.0/cvx/simulator/builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from dataclasses import dataclass, field
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from dataclasses import dataclass
+from dataclasses import field
+
 import pandas as pd
 
 from cvx.simulator.portfolio import EquityPortfolio
 from cvx.simulator.trading_costs import TradingCostModel
 
 
 @dataclass
@@ -102,14 +107,21 @@
         `@property` decorator to access the leverage attribute
         as if it were a method. The portfolio leverage is computed as
         the sum of the absolute values of the portfolio weights,
         which represents the total exposure of the portfolio to multiple assets.
         """
         return self.weights.abs().sum()
 
+    @property
+    def position_robust(self):
+        if self.position is None:
+            self.position = 0.0 * self.prices
+
+        return self.position
+
     def update(self, position, model=None, **kwargs):
         """
         The update method updates the current state of the portfolio with the new input position.
         It calculates the trades made based on the new and the previous position,
         updates the internal position and cash attributes,
         and applies any applicable trading costs according to model parameter.
 
@@ -128,30 +140,41 @@
         trades: the difference between positions in the old and new portfolio.
         position: the new position of the portfolio.
         cash: the new amount of cash in the portfolio after any trades and trading costs are applied.
 
         Note that the method does not return any value: instead,
         it updates the internal state of the _State instance.
         """
-        if self.position is None:
-            self.position = 0.0 * position
-            # trades = position
+        # if self.position is None:
+        #    self.position = 0.0 * position
+        # trades = position
         # else:
-        trades = position - self.position
+        trades = position - self.position_robust
 
         self.position = position
         self.cash -= (trades * self.prices).sum()
 
         if model is not None:
             self.cash -= model.eval(self.prices, trades=trades, **kwargs).sum()
 
         return self
 
 
-def builder(prices, weights=None, initial_cash=1e6, trading_cost_model=None):
+def builder(
+    prices,
+    weights=None,
+    market_cap=None,
+    trade_volume=None,
+    initial_cash=1e6,
+    trading_cost_model=None,
+    max_cap_fraction=None,
+    min_cap_fraction=None,
+    max_trade_fraction=None,
+    min_trade_fraction=None,
+):
     """The builder function creates an instance of the _Builder class, which
     is used to construct a portfolio of assets. The function takes in a pandas
     DataFrame of historical prices for the assets in the portfolio, optional
     weights for each asset, an initial cash value, and a trading cost model.
     The function first asserts that the prices DataFrame has a monotonic
     increasing and unique index. It then creates a DataFrame of zeros to hold
     the number of shares of each asset owned at each time step. The function
@@ -170,14 +193,20 @@
     )
 
     builder = _Builder(
         stocks=stocks,
         prices=prices.ffill(),
         initial_cash=float(initial_cash),
         trading_cost_model=trading_cost_model,
+        market_cap=market_cap,
+        trade_volume=trade_volume,
+        max_cap_fraction=max_cap_fraction,
+        min_cap_fraction=min_cap_fraction,
+        max_trade_fraction=max_trade_fraction,
+        min_trade_fraction=min_trade_fraction,
     )
 
     if weights is not None:
         for t, state in builder:
             builder.set_weights(time=t[-1], weights=weights.loc[t[-1]])
 
     return builder
@@ -186,14 +215,20 @@
 @dataclass(frozen=True)
 class _Builder:
     prices: pd.DataFrame
     stocks: pd.DataFrame
     trading_cost_model: TradingCostModel
     initial_cash: float = 1e6
     _state: _State = field(default_factory=_State)
+    market_cap: pd.DataFrame = None
+    trade_volume: pd.DataFrame = None
+    max_cap_fraction: float = None
+    min_cap_fraction: float = None
+    max_trade_fraction: float = None
+    min_trade_fraction: float = None
 
     def __post_init__(self):
         """
         The __post_init__ method is a special method of initialized instances
         of the _Builder class and is called after initialization.
         It sets the initial amount of cash in the portfolio to be equal to the input initial_cash parameter.
 
@@ -297,14 +332,48 @@
         Raises:
         AssertionError: if the input position is not a pandas Series object
         or its index is not a subset of the assets of the dataframe.
         """
         assert isinstance(position, pd.Series)
         assert set(position.index).issubset(set(self.assets))
 
+        if self.market_cap is not None:
+            # compute capitalization of desired position
+            cap = position * self._state.prices
+            # compute relative capitalization
+            rel_cap = cap / self.market_cap.loc[time]
+            # clip relative capitalization
+            rel_cap.clip(
+                lower=self.min_cap_fraction, upper=self.max_cap_fraction, inplace=True
+            )
+            # move back to capitalization
+            cap = rel_cap * self.market_cap.loc[time]
+            # compute position
+            position = cap / self._state.prices
+
+        if self.trade_volume is not None:
+            trade = position - self._state.position_robust
+
+            # move to trade in USD
+            trade = trade * self._state.prices
+            # compute relative trade volume
+            rel_trade = trade / self.trade_volume.loc[time]
+            # clip relative trade volume
+            rel_trade.clip(
+                lower=self.min_trade_fraction,
+                upper=self.max_trade_fraction,
+                inplace=True,
+            )
+            # move back to trade
+            trade = rel_trade * self.trade_volume.loc[time]
+            # move back to trade in number of stocks
+            trade = trade / self._state.prices
+            # compute position
+            position = self._state.position_robust + trade
+
         self.stocks.loc[time, position.index] = position
         self._state.update(position, model=self.trading_cost_model)
 
     def __getitem__(self, time):
         """The __getitem__ method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time. The method takes one input parameter:
```

### Comparing `cvxsimulator-0.4.1/cvx/simulator/grid.py` & `cvxsimulator-0.5.0/cvx/simulator/grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import pandas as pd
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import numpy as np
+import pandas as pd
 
 
 def iron_frame(frame, rule):
     """
     The iron_frame function takes a pandas DataFrame
     and keeps it constant on a coarser grid.
```

### Comparing `cvxsimulator-0.4.1/cvx/simulator/metrics.py` & `cvxsimulator-0.5.0/cvx/simulator/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from dataclasses import dataclass
+
 import numpy as np
 import pandas as pd
-from dataclasses import dataclass
 
 
 @dataclass(frozen=True)
 class Metrics:
     """
     Metrics class for a portfolio
     """
```

### Comparing `cvxsimulator-0.4.1/cvx/simulator/month.py` & `cvxsimulator-0.5.0/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.4.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.5.0/cvx/simulator/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from dataclasses import dataclass
 
 import pandas as pd
 
 from cvx.simulator.grid import iron_frame
 from cvx.simulator.trading_costs import TradingCostModel
```

### Comparing `cvxsimulator-0.4.1/pyproject.toml` & `cvxsimulator-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.4.1"
+version = "v0.5.0"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.4.1/PKG-INFO` & `cvxsimulator-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.4.1
+Version: 0.5.0
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
-Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
+Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
 ## Modus operandi
 
@@ -37,63 +37,63 @@
 * [Loop through time](#loop-through-time)
 * [Analyse results](#analyse-results)
 
 We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
 
 ### Create the builder object
 
-The user defines a builder object by loading a frame of prices 
+The user defines a builder object by loading a frame of prices
 and initialize the amount of cash used in our experiment:
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.builder import builder
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
-It is also possible to specify a model for trading costs. 
+It is also possible to specify a model for trading costs.
 The builder helps to fill up the frame of positions. Only once done
 we construct the actual portfolio.
 
 ### Loop through time
 
-We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop. 
+We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop.
 Let's start with a first strategy. Each day we choose two names from the universe at random.
 Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
 
 ```python
 for t, state in b:
     # pick two assets at random
     pair = np.random.choice(b.assets, 2, replace=False)
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
-    # update the position 
+    # update the position
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
 t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
-A lot of magic is hidden in the state variable. 
+A lot of magic is hidden in the state variable.
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
-Note that we update the position at the last element in the t list 
+Note that we update the position at the last element in the t list
 using a series of actual stocks rather than weights or cashpositions.
 The builder class also exposes setters for such alternative conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
@@ -103,31 +103,31 @@
 
 ```python
 portfolio = b.build()
 ```
 
 ### Analyse results
 
-The loop above is filling up the desired positions. 
-After triggering the `build()` the resulting portfolio 
+The loop above is filling up the desired positions.
+After triggering the `build()` the resulting portfolio
 is ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ...
-``` 
+```
 
 ## Bypassing the builder
 
-Some may know the positions the portfolio shall enter for eternity. 
+Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
-It is possible to completely bypass this step by submitting 
+It is possible to completely bypass this step by submitting
 a frame of positions together with a frame of prices when creating the portfolio object.
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.portfolio import EquityPortfolio
```

