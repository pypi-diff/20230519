# Comparing `tmp/cvxsimulator-0.3.3.tar.gz` & `tmp/cvxsimulator-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.3.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.4.tar", max compression
```

## Comparing `cvxsimulator-0.3.3.tar` & `cvxsimulator-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1102 2023-05-17 06:36:29.470680 cvxsimulator-0.3.3/LICENSE
--rw-r--r--   0        0        0     4907 2023-05-17 06:36:29.470680 cvxsimulator-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     6722 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1163 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1422 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/month.py
--rw-r--r--   0        0        0    14504 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-17 06:36:29.554680 cvxsimulator-0.3.3/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      596 2023-05-17 06:37:03.414800 cvxsimulator-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-05-19 18:49:35.531294 cvxsimulator-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4907 2023-05-19 18:49:35.531294 cvxsimulator-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    14008 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/builder.py
+-rw-r--r--   0        0        0      990 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1163 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1422 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/month.py
+-rw-r--r--   0        0        0    18879 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-05-19 18:50:03.515740 cvxsimulator-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.4/PKG-INFO
```

### Comparing `cvxsimulator-0.3.3/README.md` & `cvxsimulator-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.3/cvx/simulator/metrics.py` & `cvxsimulator-0.3.4/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.3/cvx/simulator/month.py` & `cvxsimulator-0.3.4/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.3/cvx/simulator/portfolio.py` & `cvxsimulator-0.3.4/cvx/simulator/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,327 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import pandas as pd
 
+from cvx.simulator.portfolio import EquityPortfolio
 from cvx.simulator.trading_costs import TradingCostModel
 
 
-@dataclass(frozen=True)
-class EquityPortfolio:
-    """ A class that represents an equity portfolio
-    and contains dataframes for prices and stock holdings,
-    as well as optional parameters for trading cost models
-    and initial cash values.
-
+@dataclass
+class _State:
+    """The _State class defines a state object used to keep track of the current state of the portfolio.
     Attributes:
-        prices (pd.DataFrame): A pandas dataframe representing
-        the prices of various assets held by the portfolio over time.
-        stocks (pd.DataFrame): A pandas dataframe representing the number of shares
-        held for each asset in the portfolio over time.
-        trading_cost_model (TradingCostModel): An optional trading cost model
-        to use when trading assets in the portfolio.
-        initial_cash (float): An optional scalar float representing the initial
-        cash value available for the portfolio.
-
-    Notes: The EquityPortfolio class is designed to represent
-    a portfolio of assets where only equity positions are held.
-    The prices and stocks dataframes are assumed to have the same
-    index object representing the available time periods for which data is available.
-    If no trading cost model is provided, the trading_cost_model attribute
-    will be set to None by default.
-    If no initial cash value is provided, the initial_cash attribute
-    will be set to a default value of 1,000,000."""
 
-    prices: pd.DataFrame
-    stocks: pd.DataFrame
-    trading_cost_model: TradingCostModel = None
-    initial_cash: float = 1e6
-
-    def __post_init__(self):
-        """ A class method that performs input validation after object initialization.
-        Notes: The post_init method is called after an instance of the EquityPortfolio class has been initialized,
-        and performs a series of input validation checks to ensure that the prices
-        and stocks dataframes are in the expected format
-        with no duplicates or missing data,
-        and that the stocks dataframe represents valid equity positions
-        for the assets held in the portfolio.
-        Specifically, the method checks that both the prices and stocks dataframes
-        have a monotonic increasing and unique index,
-        and that the index and columns of the stocks dataframe are subsets
-        of the index and columns of the prices dataframe, respectively.
-        If any of these checks fail, an assertion error will be raised. """
-
-        assert self.prices.index.is_monotonic_increasing
-        assert self.prices.index.is_unique
-        assert self.stocks.index.is_monotonic_increasing
-        assert self.stocks.index.is_unique
-
-        assert set(self.stocks.index).issubset(set(self.prices.index))
-        assert set(self.stocks.columns).issubset(set(self.prices.columns))
+    prices: a pandas Series object containing the stock prices of the current portfolio state
+    position: a pandas Series object containing the current holdings of the portfolio
+    cash: the amount of cash available in the portfolio.
+
+    By default, prices and position are set to None, while cash is set to 1 million.
+    These attributes can be updated and accessed through setter and getter methods
+    """
+    prices: pd.Series = None
+    position: pd.Series = None
+    cash: float = 1e6
 
     @property
-    def index(self):
-        """ A property that returns the index of the EquityPortfolio instance,
-        which is the time period for which the portfolio data is available.
+    def value(self):
+        """
+        The value method computes the value of the portfolio at the current time,
+        taking into account the current holdings and current stock prices.
 
-        Returns: pd.Index: A pandas index representing the time period for which the
-        portfolio data is available.
 
-        Notes: The function extracts the index of the prices dataframe,
-        which represents the time periods for which data is available for the portfolio.
-        The resulting index will be a pandas index object with the same length
-        as the number of rows in the prices dataframe."""
-        return self.prices.index
+        Returns:
 
-    @property
-    def assets(self):
-        """ A property that returns a list of the assets held by the EquityPortfolio object.
+        the value of the portfolio as a float. If the value cannot be computed due to missing position
+        (they might be still None), zero is returned instead.
 
-        Returns: list: A list of the assets held by the EquityPortfolio object.
+        The method is a decorator-based getter method, using the @property decorator to access
+        the value attribute as if it were a method. The value of the portfolio is computed as the
+        product of the current stock prices and the current holdings, summed together.
+        Note that if the current position is missing, the multiplication will raise a TypeError.
+        In this case, zero is returned as the value of the portfolio.
+        """
+        # Note that the first position may not exist yet.
+        try:
+            return (self.prices * self.position).sum()
+        except TypeError:
+            return 0.0
 
-        Notes: The function extracts the column names of the prices dataframe,
-        which correspond to the assets held by the EquityPortfolio object.
-        The resulting list will contain the names of all assets held by the portfolio, without any duplicates. """
-        return self.prices.columns
+    @property
+    def nav(self):
+        """
+        The nav method computes the net asset value (NAV) of the portfolio,
+        which is the sum of the current value of the
+        portfolio as determined by the value method,
+        and the current amount of cash available in the portfolio.
+
+        Returns:
+
+        The net asset value of the portfolio as a float, computed as the sum of the current
+        value of the portfolio and the cash available in the portfolio.
+        The method is a decorator-based getter method using the @property decorator
+        to access the NAV attribute as if it were a method.
+        The NAV is computed as the sum of the current value (as computed by the value method)
+        and the amount of cash available.
+        """
+        return self.value + self.cash
 
     @property
     def weights(self):
-        """ A property that returns a pandas dataframe representing
-        the weights of various assets in the portfolio.
-
-        Returns: pd.DataFrame: A pandas dataframe representing the weights
-        of various assets in the portfolio.
+        """
+        The weights method computes the weighting of each asset in the current portfolio
+        as a fraction of the total portfolio value.
 
-        Notes: The function calculates the weights of various assets
-        in the portfolio by dividing the equity positions
-        for each asset (as represented in the equity dataframe)
-        by the total portfolio value (as represented in the nav dataframe).
-        Both dataframes are assumed to have the same dimensions.
-        The resulting dataframe will show the relative weight
-        of each asset in the portfolio at each point in time. """
-        return self.equity / self.nav
+        Returns:
 
-    def __getitem__(self, time):
-        return self.stocks.loc[time]
+        a pandas series object containing the weighting of each asset as a fraction
+        of the total portfolio value. If the positions are still missing, then a series of zeroes is returned.
+        The method is a decorator-based getter method using the @property decorator to access
+        the weights attribute as if it were a method. The weighting for each asset is computed
+        as the product of the current position and the current stock prices,
+        divided by the net asset value of the portfolio (as computed by the nav method).
+        Note that this weighting represents the fraction of the portfolio value allocated to a particular asset.
+        If the portfolio weighting cannot be computed due to missing positions,
+        then a series of zeroes with the same size as the prices attribute is returned instead.
+        """
+        try:
+            return (self.prices * self.position)/self.nav
+        except TypeError:
+            return 0 * self.prices
 
     @property
-    def trading_costs(self):
-        """ A property that returns a pandas dataframe
-        representing the trading costs incurred by the portfolio due to trades made.
-
-        Returns: pd.DataFrame: A pandas dataframe representing the trading
-        costs incurred by the portfolio due to trades made.
-
-        Notes: The function calculates the trading costs using the specified
-        trading cost model (if available) and the prices and trading
-        data represented by the prices and trades_stocks
-        dataframes, respectively. If no trading cost model is provided,
-        a dataframe with all zeros will be returned.
-        The resulting dataframe will have the same dimensions as
-        the prices and trades_stocks dataframes,
-        showing the trading costs incurred at each point in time for each asset traded. """
-        if self.trading_cost_model is None:
-            return 0.0 * self.prices
+    def leverage(self):
+        """
+        The `leverage` method computes the leverage of the portfolio,
+        which is the sum of the absolute values of the portfolio weights.
 
-        return self.trading_cost_model.eval(self.prices, self.trades_stocks)
+        Returns:
+        - the portfolio leverage as a float, computed as the sum of the
+        absolute values of the portfolio weights.
+
+        The method is a decorator-based getter method using the
+        `@property` decorator to access the leverage attribute
+        as if it were a method. The portfolio leverage is computed as
+        the sum of the absolute values of the portfolio weights,
+        which represents the total exposure of the portfolio to multiple assets.
+        """
+        return self.weights.abs().sum()
 
-    @property
-    def equity(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe
-        representing the equity positions of the portfolio,
-        which is the value of each asset held by the portfolio.
-        Returns: pd.DataFrame: A pandas dataframe representing
-        the equity positions of the portfolio.
-
-        Notes: The function calculates the equity of the portfolio
-        by multiplying the current prices of each asset
-        by the number of shares held by the portfolio.
-        The resulting values are filled forward to account
-        for any missing data or NaN values.
-        The equity dataframe will have the same dimensions
-        as the prices and stocks dataframes. """
+    def update(self, position, model=None, **kwargs):
+        """
+        The update method updates the current state of the portfolio with the new input position.
+        It calculates the trades made based on the new and the previous position,
+        updates the internal position and cash attributes,
+        and applies any applicable trading costs according to model parameter.
 
-        return (self.prices * self.stocks).ffill()
+        The method takes three input parameters:
 
-    @property
-    def trades_stocks(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe representing the trades made in the portfolio in terms of stocks.
+        position: a pandas series object representing the new position of the portfolio.
+        model: an optional trading cost model (e.g. slippage, fees) to be incorporated into the update.
+        If None, no trading costs will be applied.
+        **kwargs: additional keyword arguments to pass into the trading cost model.
 
-        Returns: pd.DataFrame: A pandas dataframe representing the trades made in the portfolio in terms of stocks.
+        Returns:
+        self: the _State instance with the updated position and cash.
 
-        Notes: The function calculates the trades made by the portfolio by taking
-        the difference between the current and previous values of the stocks dataframe.
-        The resulting values will represent the number of shares of each asset
-        bought or sold by the portfolio at each point in time.
-        The resulting dataframe will have the same dimensions
-        as the stocks dataframe, with NaN values filled with zeros. """
-        t = self.stocks.diff()
-        t.loc[self.index[0]] = self.stocks.loc[self.index[0]]
-        return t.fillna(0.0)
+        Updates:
 
-    @property
-    def trades_currency(self) -> pd.DataFrame:
-        """ A property that returns a pandas dataframe representing the trades made in the portfolio in terms of currency.
+        trades: the difference between positions in the old and new portfolio.
+        position: the new position of the portfolio.
+        cash: the new amount of cash in the portfolio after any trades and trading costs are applied.
 
-        Returns: pd.DataFrame: A pandas dataframe representing the trades made in the portfolio in terms of currency.
+        Note that the method does not return any value: instead,
+        it updates the internal state of the _State instance.
+        """
+        if self.position is None:
+            trades = position
+        else:
+            trades = position - self.position
+
+        self.position = position
+        self.cash -= (trades * self.prices).sum()
+
+        if model is not None:
+            self.cash -= model.eval(self.prices,  trades=trades, **kwargs).sum()
+
+        return self
+
+
+def builder(prices, weights=None, initial_cash=1e6, trading_cost_model=None):
+    """The builder function creates an instance of the _Builder class, which
+    is used to construct a portfolio of assets. The function takes in a pandas
+    DataFrame of historical prices for the assets in the portfolio, optional
+    weights for each asset, an initial cash value, and a trading cost model.
+    The function first asserts that the prices DataFrame has a monotonic
+    increasing and unique index. It then creates a DataFrame of zeros to hold
+    the number of shares of each asset owned at each time step. The function
+    initializes a _Builder object with the stocks DataFrame, the prices
+    DataFrame (forward-filled), the initial cash value, and the trading cost
+    model. If weights are provided, they are set for each time step using
+    set_weights method of the _Builder object. The final output is the
+    constructed _Builder object."""
+
+    assert isinstance(prices, pd.DataFrame)
+    assert prices.index.is_monotonic_increasing
+    assert prices.index.is_unique
+
+    stocks = pd.DataFrame(index=prices.index, columns=prices.columns, data=0.0, dtype=float)
+
+    trading_cost_model = trading_cost_model
+    builder = _Builder(stocks=stocks, prices=prices.ffill(), initial_cash=float(initial_cash),
+                    trading_cost_model=trading_cost_model)
+
+    if weights is not None:
+        for t, state in builder:
+            builder.set_weights(time=t[-1], weights=weights.loc[t[-1]])
 
-        Notes: The function calculates the trades made in currency by multiplying
-        the number of shares of each asset bought or sold (as represented in the trades_stocks dataframe)
-        with the current prices of each asset (as represented in the prices dataframe).
-        Uses pandas ffill() method to forward fill NaN values in the prices dataframe.
-        The resulting dataframe will have the same dimensions as the stocks and prices dataframes. """
-        return self.trades_stocks * self.prices.ffill()
+    return builder
 
-    @property
-    def cash(self) -> pd.Series:
-        """ A property that returns a pandas series representing the cash on hand in the portfolio.
 
-        Returns: pd.Series: A pandas series representing the cash on hand in the portfolio.
+@dataclass(frozen=True)
+class _Builder:
+    prices: pd.DataFrame
+    stocks: pd.DataFrame
+    trading_cost_model: TradingCostModel
+    initial_cash: float = 1e6
+    _state: _State = field(default_factory=_State)
 
-        Notes: The function calculates the cash available in the portfolio by subtracting
-        the sum of trades currency and cumulative trading costs from the initial cash value specified
-        when constructing the object. Uses pandas cumsum() method
-        to calculate the cumulative sum of trading costs and
-        trades currency along the time axis.
-        The resulting series will show how much money is available for further trades at each point in time.
+    def __post_init__(self):
         """
-        return self.initial_cash - self.trades_currency.sum(axis=1).cumsum() - self.trading_costs.sum(axis=1).cumsum()
-
-    @property
-    def nav(self) -> pd.Series:
-        """ Returns a pandas series representing the total value
-        of the portfolio's investments and cash.
-
-        Returns: pd.Series: A pandas series representing the
-                            total value of the portfolio's investments and cash.
+        The __post_init__ method is a special method of initialized instances
+        of the _Builder class and is called after initialization.
+        It sets the initial amount of cash in the portfolio to be equal to the input initial_cash parameter.
+
+        The method takes no input parameter. It initializes the cash attribute in the internal
+        _State object with the initial amount of cash in the portfolio, self.initial_cash.
+
+        Note that this method is often used in Python classes for additional initialization routines
+        that can only be performed after the object is fully initialized. __post_init__
+        is called automatically after the object initialization.
         """
-        return self.equity.sum(axis=1) + self.cash
+        self._state.cash = self.initial_cash
 
     @property
-    def profit(self) -> pd.Series:
-        """ A property that returns a pandas series representing the
-        profit gained or lost in the portfolio based on changes in asset prices.
+    def index(self):
+        """ A property that returns the index of the portfolio,
+        which is the time period for which the portfolio data is available.
 
-        Returns: pd.Series: A pandas series representing the profit
-        gained or lost in the portfolio based on changes in asset prices.
+        Returns: pd.Index: A pandas index representing the
+        time period for which the portfolio data is available.
 
-        Notes: The calculation is based on the difference between
-        the previous and current prices of the assets in the portfolio,
-        multiplied by the number of stocks in each asset previously held.
-        """
+        Notes: The function extracts the index of the prices dataframe,
+        which represents the time periods for which data is available for the portfolio.
+        The resulting index will be a pandas index object
+        with the same length as the number of rows in the prices dataframe. """
 
-        price_changes = self.prices.ffill().diff()
-        previous_stocks = self.stocks.shift(1).fillna(0.0)
-        return (previous_stocks * price_changes).dropna(axis=0, how="all").sum(axis=1)
+        return self.prices.index
 
     @property
-    def highwater(self) -> pd.Series:
-        """ A function that returns a pandas series representing
-        the high-water mark of the portfolio, which is the highest point
-        the portfolio value has reached over time.
-
-        Returns: pd.Series: A pandas series representing the
-        high-water mark of the portfolio.
-
-        Notes: The function performs a rolling computation based on
-        the cumulative maximum of the portfolio's value over time,
-        starting from the beginning of the time period being considered.
-        Min_periods argument is set to 1 to include the minimum period of one day.
-        The resulting series will show the highest value the portfolio has reached at each point in time. """
-        return self.nav.expanding(min_periods=1).max()
+    def assets(self):
+        """ A property that returns a list of the assets held by the portfolio.
 
-    @property
-    def drawdown(self) -> pd.Series:
-        """ A property that returns a pandas series representing the
-        drawdown of the portfolio, which measures the decline
-        in the portfolio's value from its (previously) highest
-        point to its current point.
+        Returns: list: A list of the assets held by the portfolio.
 
-        Returns: pd.Series: A pandas series representing the
-        drawdown of the portfolio.
+        Notes: The function extracts the column names of the prices dataframe,
+        which correspond to the assets held by the portfolio.
+        The resulting list will contain the names of all assets
+        held by the portfolio, without any duplicates. """
+        return self.prices.columns
 
-        Notes: The function calculates the ratio of the portfolio's current value
-        vs. its current high-water-mark and then subtracting the result from 1.
-        A positive drawdown means the portfolio is currently worth
-        less than its high-water mark. A drawdown of 0.1 implies that the nav is currently 0.9 times the high-water mark """
-        return 1.0 - self.nav / self.highwater
+    def set_weights(self, time, weights):
+        """
+        Set the position via weights (e.g. fractions of the nav)
 
-    def __mul__(self, scalar):
-        """ A method that allows multiplication of the EquityPortfolio object with a scalar constant.
+        :param time: time
+        :param weights: series of weights
+        """
+        self[time] = (self._state.nav * weights) / self._state.prices
 
-        Args: scalar: A scalar constant that multiplies the number of shares
-        of each asset held in the EquityPortfolio object.
+    def set_cashposition(self, time, cashposition):
+        """
+        Set the position via cash positions (e.g. USD invested per asset)
 
-        Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
+        :param time: time
+        :param cashposition: series of cash positions
+        """
+        self[time] = cashposition / self._state.prices
 
-        Notes: The mul method allows multiplication of an EquityPortfolio object
-        with a scalar constant to increase or decrease
-        the number of shares held for each asset in the portfolio accordingly.
-        The method returns a new EquityPortfolio object with the same prices
-        and trading cost model as the original object,
-        and with the number of shares for each asset multiplied by the scalar constant
-        (as represented in the stocks dataframe).
-        Additionally, the initial cash value is multiplied
-        by the scalar to maintain the same cash-to-equity ratio as the original portfolio. """
-        return EquityPortfolio(prices=self.prices, stocks=self.stocks * scalar, initial_cash=self.initial_cash * scalar, trading_cost_model=self.trading_cost_model)
+    def set_position(self, time, position):
+        """
+        Set the position via number of assets (e.g. number of stocks)
 
-    def __rmul__(self, scalar):
-        """ A method that allows multiplication of the EquityPortfolio object with a scalar constant in a reversed order.
+        :param time: time
+        :param position: series of number of stocks
+        """
+        self[time] = position
 
-        Args: scalar: A scalar constant that multiplies the EquityPortfolio object in a reversed order.
+    def __iter__(self):
+        """
+        The __iter__ method allows the object to be iterated over in a for loop,
+        yielding time and the current state of the portfolio.
+        The method yields a list of dates seen so far
+        (excluding the first date) and returns a tuple
+        containing the list of dates and the current portfolio state.
 
-        Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
+        Yield:
 
-        Notes: The rmul method allows multiplication of a scalar
-        constant with an EquityPortfolio object in a reversed order"""
-        return self.__mul__(scalar)
+        interval: a pandas DatetimeIndex object containing the dates seen so far.
 
-    def __add__(self, port_new):
-        assert isinstance(port_new, EquityPortfolio)
+        state: the current state of the portfolio,
+        taking into account the stock prices at each interval.
+        """
+        for t in self.index:
+            # valuation of the current position
+            self._state.prices = self.prices.loc[t]
+            yield self.index[self.index <= t], self._state
 
-        assets = self.assets.union(port_new.assets)
-        index = self.index.union(port_new.index)
+    def __setitem__(self, time, position):
+        """
+        The method __setitem__ updates the stock data in the dataframe for a specific time index with the input position. It first checks that position is a valid input, meaning it is a pandas Series object and has its index within the assets of the dataframe.
+        The method takes two input parameters:
 
-        left = pd.DataFrame(index=index, columns=assets)
-        left.update(self.stocks)
-        # this is a problem...
-        left = left.fillna(0.0)
+        time: time index for which to update the stock data
+        position: pandas series object containing the updated stock data
 
-        right = pd.DataFrame(index=index, columns=assets)
-        right.update(port_new.stocks)
-        right = right.fillna(0.0)
+        Returns: None
 
-        positions = left + right
+        Updates:
+        the stock data of the dataframe at the given time index with the input position
+        the internal state of the portfolio with the updated position, taking into account the trading cost model
 
-        prices_left = self.prices.combine_first(port_new.prices)
-        prices_right = port_new.prices.combine_first(self.prices)
+        Raises:
+        AssertionError: if the input position is not a pandas Series object
+        or its index is not a subset of the assets of the dataframe.
+        """
+        assert isinstance(position, pd.Series)
+        assert set(position.index).issubset(set(self.assets))
+
+        self.stocks.loc[time, position.index] = position
+        self._state.update(position, model=self.trading_cost_model)
+
+    def __getitem__(self, time):
+        """ The __getitem__ method retrieves the stock data for a specific time in the dataframe.
+        It returns the stock data for that time. The method takes one input parameter:
 
-        pd.testing.assert_frame_equal(prices_left, prices_right)
+        time: the time index for which to retrieve the stock data
+        Returns: stock data for the input time
 
-        return EquityPortfolio(prices=prices_right, stocks=positions,
-                               initial_cash=self.initial_cash + port_new.initial_cash,
+        Note that the input time must be in the index of the dataframe, otherwise a KeyError will be raised.
+        """
+        return self.stocks.loc[time]
+
+    def build(self):
+        """ A function that creates a new instance of the EquityPortfolio
+        class based on the internal state of the Portfolio builder object.
+
+        Returns: EquityPortfolio: A new instance of the EquityPortfolio class
+        with the attributes (prices, stocks, initial_cash, trading_cost_model) as specified in the Portfolio builder.
+
+        Notes: The function simply creates a new instance of the EquityPortfolio
+        class with the attributes (prices, stocks, initial_cash, trading_cost_model) equal
+        to the corresponding attributes in the Portfolio builder object.
+        The resulting EquityPortfolio object will have the same state as the Portfolio builder from which it was built. """
+
+        return EquityPortfolio(prices=self.prices,
+                               stocks=self.stocks,
+                               initial_cash=self.initial_cash,
                                trading_cost_model=self.trading_cost_model)
+
```

### Comparing `cvxsimulator-0.3.3/pyproject.toml` & `cvxsimulator-0.3.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.3"
+version = "v0.3.4"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
@@ -14,13 +14,14 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.0"
 pytest-cov = "4.0.0"
 yfinance = "*"
 quantstats = "*"
 plotly = "*"
+cvxpy = "*"
 jupyterlab = "*"
 loguru = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cvxsimulator-0.3.3/PKG-INFO` & `cvxsimulator-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

