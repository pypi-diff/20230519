# Comparing `tmp/okama-1.2.3.tar.gz` & `tmp/okama-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okama-1.2.3.tar", max compression
+gzip compressed data, was "okama-1.3.0.tar", max compression
```

## Comparing `okama-1.2.3.tar` & `okama-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1058 2021-06-16 07:17:39.219198 okama-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1876 2022-10-07 15:39:08.369280 okama-1.2.3/okama/__init__.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.317201 okama-1.2.3/okama/api/__init__.py
--rw-r--r--   0        0        0     6130 2022-07-29 14:30:04.739588 okama-1.2.3/okama/api/api_methods.py
--rw-r--r--   0        0        0     4083 2022-06-04 17:56:18.764145 okama-1.2.3/okama/api/data_queries.py
--rw-r--r--   0        0        0     1403 2022-06-04 17:56:18.766142 okama-1.2.3/okama/api/namespaces.py
--rw-r--r--   0        0        0     1384 2022-06-04 17:56:18.770175 okama-1.2.3/okama/api/search.py
--rw-r--r--   0        0        0     5985 2022-10-07 15:39:08.377282 okama-1.2.3/okama/asset.py
--rw-r--r--   0        0        0    56425 2022-10-07 14:22:37.505421 okama-1.2.3/okama/asset_list.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.333202 okama-1.2.3/okama/common/__init__.py
--rw-r--r--   0        0        0        0 2021-10-12 14:31:44.977602 okama-1.2.3/okama/common/helpers/__init__.py
--rw-r--r--   0        0        0    22528 2022-10-07 15:39:08.382276 okama-1.2.3/okama/common/helpers/helpers.py
--rw-r--r--   0        0        0      555 2022-01-30 15:06:03.393518 okama-1.2.3/okama/common/helpers/ratios.py
--rw-r--r--   0        0        0    21819 2022-10-07 15:39:08.384281 okama-1.2.3/okama/common/make_asset_list.py
--rw-r--r--   0        0        0     2857 2022-04-21 06:30:03.465033 okama-1.2.3/okama/common/validators.py
--rw-r--r--   0        0        0        0 2021-06-16 07:17:39.341199 okama-1.2.3/okama/frontier/__init__.py
--rw-r--r--   0        0        0    32119 2022-10-08 04:19:57.613536 okama-1.2.3/okama/frontier/multi_period.py
--rw-r--r--   0        0        0    46353 2022-10-08 03:55:56.095275 okama-1.2.3/okama/frontier/single_period.py
--rw-r--r--   0        0        0    19003 2022-06-05 13:19:20.083275 okama-1.2.3/okama/macro.py
--rw-r--r--   0        0        0    80387 2022-10-07 15:39:08.398281 okama-1.2.3/okama/portfolio.py
--rw-r--r--   0        0        0      387 2022-06-04 17:56:18.803142 okama-1.2.3/okama/settings.py
--rw-r--r--   0        0        0     2302 2022-10-07 15:39:08.413277 okama-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7781 2022-08-10 08:26:35.121856 okama-1.2.3/README.md
--rw-r--r--   0        0        0     8838 1970-01-01 00:00:00.000000 okama-1.2.3/setup.py
--rw-r--r--   0        0        0     9396 1970-01-01 00:00:00.000000 okama-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2021-06-16 07:17:39.219198 okama-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2157 2023-05-19 15:03:56.216688 okama-1.3.0/okama/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.317201 okama-1.3.0/okama/api/__init__.py
+-rw-r--r--   0        0        0     6130 2022-07-29 14:30:04.739588 okama-1.3.0/okama/api/api_methods.py
+-rw-r--r--   0        0        0     4083 2022-06-04 17:56:18.764145 okama-1.3.0/okama/api/data_queries.py
+-rw-r--r--   0        0        0     1409 2023-05-19 11:53:16.721825 okama-1.3.0/okama/api/namespaces.py
+-rw-r--r--   0        0        0     1384 2022-06-04 17:56:18.770175 okama-1.3.0/okama/api/search.py
+-rw-r--r--   0        0        0     5944 2023-05-19 11:53:16.724825 okama-1.3.0/okama/asset.py
+-rw-r--r--   0        0        0    57439 2023-05-19 11:53:16.727824 okama-1.3.0/okama/asset_list.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.333202 okama-1.3.0/okama/common/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-12 14:31:44.977602 okama-1.3.0/okama/common/helpers/__init__.py
+-rw-r--r--   0        0        0    23790 2023-05-19 11:53:16.732824 okama-1.3.0/okama/common/helpers/helpers.py
+-rw-r--r--   0        0        0      555 2022-01-30 15:06:03.393518 okama-1.3.0/okama/common/helpers/ratios.py
+-rw-r--r--   0        0        0    22059 2023-05-19 11:53:16.735825 okama-1.3.0/okama/common/make_asset_list.py
+-rw-r--r--   0        0        0     2857 2022-04-21 06:30:03.465033 okama-1.3.0/okama/common/validators.py
+-rw-r--r--   0        0        0        0 2021-06-16 07:17:39.341199 okama-1.3.0/okama/frontier/__init__.py
+-rw-r--r--   0        0        0    32120 2023-05-19 11:53:16.741829 okama-1.3.0/okama/frontier/multi_period.py
+-rw-r--r--   0        0        0    46553 2023-05-19 15:03:02.297773 okama-1.3.0/okama/frontier/single_period.py
+-rw-r--r--   0        0        0    19003 2022-06-05 13:19:20.083275 okama-1.3.0/okama/macro.py
+-rw-r--r--   0        0        0    80308 2023-05-19 11:53:16.747828 okama-1.3.0/okama/portfolio.py
+-rw-r--r--   0        0        0      387 2022-06-04 17:56:18.803142 okama-1.3.0/okama/settings.py
+-rw-r--r--   0        0        0     1907 2023-05-19 11:53:16.750828 okama-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7783 2023-05-19 14:52:52.231034 okama-1.3.0/README.md
+-rw-r--r--   0        0        0     9444 1970-01-01 00:00:00.000000 okama-1.3.0/PKG-INFO
```

### Comparing `okama-1.2.3/LICENSE.txt` & `okama-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/__init__.py` & `okama-1.3.0/okama/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,17 +26,23 @@
 from okama.portfolio import Portfolio
 from okama.macro import Inflation, Rate, Indicator
 from okama.frontier.multi_period import EfficientFrontierReb
 from okama.frontier.single_period import EfficientFrontier
 from okama.api.data_queries import QueryData
 from okama.api.search import search
 from okama.api.api_methods import API
-from okama.api.namespaces import (
-    namespaces,
-    assets_namespaces,
-    macro_namespaces,
-    symbols_in_namespace,
-)
+import okama.api.namespaces
 from okama.common.helpers.helpers import Float, Frame, Rebalance, Date
 import okama.settings
 
+
+def __getattr__(name):
+    if name == "namespaces":
+        return okama.api.namespaces.get_namespaces()
+    elif name == "assets_namespaces":
+        return okama.api.namespaces.get_assets_namespaces()
+    elif name == "macro_namespaces":
+        return okama.api.namespaces.get_macro_namespaces()
+    raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
+
+
 __version__ = version("okama")
```

### Comparing `okama-1.2.3/okama/api/api_methods.py` & `okama-1.3.0/okama/api/api_methods.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/api/data_queries.py` & `okama-1.3.0/okama/api/data_queries.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/api/namespaces.py` & `okama-1.3.0/okama/api/namespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 
 @lru_cache()
 def no_dividends_namespaces():
     string_response = api_methods.API.get_no_dividends_namespaces()
     return json.loads(string_response)
 
 
-namespaces = get_namespaces()
-assets_namespaces = get_assets_namespaces()
-macro_namespaces = get_macro_namespaces()
+# namespaces = get_namespaces()
+# assets_namespaces = get_assets_namespaces()
+# macro_namespaces = get_macro_namespaces()
```

### Comparing `okama-1.2.3/okama/api/search.py` & `okama-1.3.0/okama/api/search.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/asset.py` & `okama-1.3.0/okama/asset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 
 import pandas as pd
 import numpy as np
 
 from okama import settings
 from okama.api import data_queries, namespaces
-from okama.common.helpers import helpers
 
 
 class Asset:
     """
     A financial asset, that could be used in a list of assets or in portfolio.
 
     Parameters
@@ -45,15 +44,15 @@
             "first date": self.first_date.strftime("%Y-%m"),
             "last date": self.last_date.strftime("%Y-%m"),
             "period length": "{:.2f}".format(self.period_length),
         }
         return repr(pd.Series(dic))
 
     def _check_namespace(self):
-        namespace = self._symbol.split(".", 1)[-1]
+        namespace = self._symbol.split(".")[-1]
         allowed_namespaces = namespaces.get_assets_namespaces()
         if namespace not in allowed_namespaces:
             raise ValueError(f"{namespace} is not in allowed assets namespaces: {allowed_namespaces}")
 
     def _get_symbol_data(self, symbol) -> None:
         x = data_queries.QueryData.get_symbol_info(symbol)
         self.ticker: str = x["code"]
@@ -118,15 +117,15 @@
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> x = ok.Asset('VOO.US')
         >>> x.close_monthly.plot()
         >>> plt.show()
         """
-        return helpers.Frame.change_period_to_month(self.close_daily)
+        return data_queries.QueryData.get_close(self.symbol, period="M")
 
     @property
     def adj_close(self):
         """
         Return adjusted close price time series historical daily data.
 
         The adjusted closing price amends a stock's closing price after accounting
```

### Comparing `okama-1.2.3/okama/asset_list.py` & `okama-1.3.0/okama/asset_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -988,19 +988,19 @@
         DataFrame
             Annualized tracking diffirence time series for each asset.
 
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> x = ok.AssetList(['SP500TR.INDX', 'SPY.US', 'VOO.US'], last_date='2021-01')
-        >>> x.tracking_difference_annualized.plot()
+        >>> x.tracking_difference_annualized().plot()
 
         To calculate rolling annualized tracking difference set `rolling_window` to a number of months (moving window size):
 
-        >>> x.tracking_difference_annualized.plot(rolling_window = 12)
+        >>> x.tracking_difference_annualized(rolling_window = 12*5).plot()
         >>> plt.show()
         """
         if rolling_window:
             rolling_cagr = helpers.Frame.get_rolling_fn(
                 self.assets_ror,
                 window=rolling_window,
                 fn=helpers.Frame.get_cagr,
@@ -1036,112 +1036,117 @@
             df = x[1]
             wealth_index = helpers.Frame.get_wealth_indexes(df)
             row = helpers.Index.tracking_difference(wealth_index).iloc[[-1]]
             result = pd.concat([result, row], ignore_index=False)
         result.index = result.index.asfreq("Y")
         return result
 
-    @property
-    def tracking_error(self) -> pd.DataFrame:
+    def tracking_error(self, rolling_window: Optional[int] = None) -> pd.DataFrame:
         """
         Calculate tracking error time series for the rate of return of assets.
 
         Tracking error is defined as the standard deviation of the difference between the returns of the asset
         and the returns of the benchmark.
 
         Benchmark should be in the first position of the symbols list in AssetList parameters.
 
+        Parameters
+        ----------
+        rolling_window : int or None, default None
+            Size of the moving window in months. Must be at least 12 months.
+            If None calculate expanding tracking error.
+
         Returns
         -------
         DataFrame
-            Tracking error time series for each asset.
+            rolling or expanding tracking error time series for each asset.
 
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> x = ok.AssetList(['SP500TR.INDX', 'SPY.US', 'VOO.US'], last_date='2021-01')
-        >>> x.tracking_error.plot()
+        >>> x.tracking_error().plot()
         >>> plt.show()
-        """
-        return helpers.Index.tracking_error(self.assets_ror)
 
-    @property
-    def index_corr(self) -> pd.DataFrame:
-        """
-        Compute expanding correlation with the index (or benchmark) time series for the assets.
+        To calculate rolling tracking error set `rolling_window` to a number of months (moving window size):
 
-        Benchmark should be in the first position of the symbols list in AssetList parameters.
-        There should be at least 12 months of historical data.
-
-        Returns
-        -------
-        DataFrame
-            Expanding correlation with the index (or benchmark) time series for each asset.
-
-        Examples
-        --------
-        >>> import matplotlib.pyplot as plt
-        >>> sp = ok.AssetList(['SP500TR.INDX', 'VBMFX.US', 'GC.COMM', 'VNQ.US'])
-        >>> sp.names
-        {'SP500TR.INDX': 'S&P 500 (TR)',
-        'VBMFX.US': 'VANGUARD TOTAL BOND MARKET INDEX FUND INVESTOR SHARES',
-        'GC.COMM': 'Gold',
-        'VNQ.US': 'Vanguard Real Estate Index Fund ETF Shares'}
-        >>> sp.index_corr.plot()
+        >>> x.tracking_error(rolling_window = 12*5).plot()
         >>> plt.show()
         """
-        return helpers.Index.cov_cor(self.assets_ror, fn="corr")
+        if rolling_window:
+            return helpers.Index.rolling_fn(
+                df=self.assets_ror,
+                window=rolling_window,
+                fn=helpers.Index.tracking_error,
+                window_below_year=False,  # small windows below 12 months are not allowed
+            )
+        else:
+            return helpers.Index.tracking_error(self.assets_ror)
 
-    def index_rolling_corr(self, window: int = 60) -> pd.DataFrame:
+    def index_corr(self, rolling_window: Optional[int] = None) -> pd.DataFrame:
         """
-        Compute rolling correlation with the index (or benchmark) time series for the assets.
+        Compute correlation with the index (or benchmark) time series for the assets. Expanding or rolling correlation
+        is available.
 
         Index (benchmark) should be in the first position of the symbols list in AssetList parameters.
         There should be at least 12 months of historical data.
 
         Parameters
         ----------
-        window : int, default 60
-            Rolling window size in months. This is the number of observations used for calculating the statistic.
+        rolling_window : int or None, default None
+            Size of the moving window in months. Must be at least 12 months.
+            If None calculate expanding correlation with index.
 
         Returns
         -------
         DataFrame
-            Rolling correlation with the index (or benchmark) time series for each asset.
+            Rolling or expanding correlation with the index (or benchmark) time series for each asset.
 
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> sp = ok.AssetList(['SP500TR.INDX', 'VBMFX.US', 'GC.COMM'])
         >>> sp.names
         {'SP500TR.INDX': 'S&P 500 (TR)',
         'VBMFX.US': 'VANGUARD TOTAL BOND MARKET INDEX FUND INVESTOR SHARES',
         'GC.COMM': 'Gold'}
-        >>> sp.index_rolling_corr(window=24).plot()
+        >>> sp.index_corr().plot()  # expanding correlation with S&P 500
+        >>> plt.show()
+
+        To calculate rolling correlation with S&P 500 set `rolling_window` to a number of months (moving window size):
+
+        >>> sp.index_corr(rolling_window=24).plot()
         >>> plt.show()
         """
-        return helpers.Index.rolling_cov_cor(self.assets_ror, window=window, fn="corr")
+        if rolling_window:
+            return helpers.Index.rolling_cov_cor(self.assets_ror, window=rolling_window, fn="corr")
+        return helpers.Index.expanding_cov_cor(self.assets_ror, fn="corr")
 
-    @property
-    def index_beta(self) -> pd.DataFrame:
+    def index_beta(self, rolling_window: Optional[int] = None) -> pd.DataFrame:
         """
         Compute beta coefficient time series for the assets.
 
         Beta coefficient is defined in Capital Asset Pricing Model (CAPM). It is a measure of how
         an individual asset moves (on average) when the benchmark increases or decreases. When beta is positive,
         the asset price tends to move in the same direction as the benchmark,
         and the magnitude of beta tells by how much.
 
         Index (benchmark) should be in the first position of the symbols list in AssetList parameters.
         There should be at least 12 months of historical data.
 
+        Parameters
+        ----------
+        rolling_window : int or None, default None
+            Size of the moving window in months. Must be at least 12 months.
+            If None calculate expanding beta coefficient.
+
         Returns
         -------
         DataFrame
-            Beta coefficient time series for each asset.
+            rollinf or expanding beta coefficient time series for each asset.
 
         See Also
         --------
         index_corr : Compute correlation with the index (or benchmark).
         index_rolling_corr : Compute rolling correlation with the index (or benchmark).
         index_beta : Compute beta coefficient.
 
@@ -1150,17 +1155,29 @@
         >>> import matplotlib.pyplot as plt
         >>> sp = ok.AssetList(['SP500TR.INDX', 'VBMFX.US', 'GC.COMM', 'VNQ.US'])
         >>> sp.names
         {'SP500TR.INDX': 'S&P 500 (TR)',
         'VBMFX.US': 'VANGUARD TOTAL BOND MARKET INDEX FUND INVESTOR SHARES',
         'GC.COMM': 'Gold',
         'VNQ.US': 'Vanguard Real Estate Index Fund ETF Shares'}
-        >>> sp.index_beta.plot()
+        >>> sp.index_beta().plot()
+        >>> plt.show()
+
+        To calculate rolling beta set `rolling_window` to a number of months (moving window size):
+
+        >>> sp.index_beta(rolling_window = 12 * 5).plot()  # 5 years moving window
         >>> plt.show()
         """
+        if rolling_window:
+            return helpers.Index.rolling_fn(
+                df=self.assets_ror,
+                window=rolling_window,
+                fn=helpers.Index.beta,
+                window_below_year=False,  # small windows below 12 months are not allowed
+            )
         return helpers.Index.beta(self.assets_ror)
 
     # distributions
     @property
     def skewness(self) -> pd.DataFrame:
         """
         Compute expanding skewness of the return time series for each asset returns.
```

### Comparing `okama-1.2.3/okama/common/helpers/helpers.py` & `okama-1.3.0/okama/common/helpers/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,15 +361,15 @@
     """
 
     @staticmethod
     def wealth_ts(weights: list, ror: pd.DataFrame, *, period: str = "year") -> pd.Series:
         """
         Calculate wealth index time series of rebalanced portfolio given returns time series of the assets.
         Default rebalancing period is a Year (end of year)
-        For not rebalanced portfolio set Period to 'none'
+        For not rebalanced portfolio set Period to 'none'.
         """
         # Frame.weights_sum_is_one(weights)
         initial_inv = 1000
         wealth_index = pd.Series(dtype="float64")
         if period == "none":  # Not rebalanced portfolio
             inv_period_spread = np.asarray(weights) * initial_inv
             assets_wealth_indexes = inv_period_spread * (1 + ror).cumprod()
@@ -412,24 +412,14 @@
                 initial_inv = wealth_index.iloc[-1]
         return assets_wealth_indexes
 
     @staticmethod
     def assets_weights_ts(weights: list, ror: pd.DataFrame, *, period: str = "year") -> pd.DataFrame:
         """
         Calculate assets weights monthly time series for rebalanced portfolio.
-
-        Parameters
-        ----------
-        weights
-        ror
-        period
-
-        Returns
-        -------
-
         """
         assets_wealth_indexes = Rebalance.assets_wealth_ts(weights=weights, ror=ror, period=period)
         portfolio_wealth_index = Rebalance.wealth_ts(weights=weights, ror=ror, period=period)
         return assets_wealth_indexes.divide(portfolio_wealth_index, axis=0)
 
     @staticmethod
     def return_ts(weights: Union[list, np.ndarray], ror: pd.DataFrame, *, period: str = "year") -> pd.Series:
@@ -501,23 +491,25 @@
         """
         Returns tracking error for a rate of return time series.
         Assets are compared with the index or another benchmark.
         Index should be in the first position (first column).
         """
         if ror.shape[1] < 2:
             raise ValueError("At least 2 symbols should be provided to calculate Tracking Error.")
+        if ror.shape[0] < 12:
+            raise ValueError("Tracking Error is not defined for time periods < 1 year")
         cumsum = ror.subtract(ror.iloc[:, 0], axis=0).pow(2, axis=0).cumsum()
         cumsum.drop(cumsum.columns[0], axis=1, inplace=True)  # drop the first column (stock index data)
         tracking_error = cumsum.divide((1.0 + np.arange(ror.shape[0])), axis=0).pow(0.5, axis=0)
         return tracking_error * np.sqrt(12)
 
     @staticmethod
-    def cov_cor(ror: pd.DataFrame, fn: str) -> pd.DataFrame:
+    def expanding_cov_cor(ror: pd.DataFrame, fn: str) -> pd.DataFrame:
         """
-        Returns the accumulated correlation or covariance time series.
+        Returns the accumulated expanding correlation or covariance time series.
         The period should be at least 12 months.
         """
         if ror.shape[1] < 2:
             raise ValueError("At least 2 symbols should be provided.")
         if fn not in ["cov", "corr"]:
             raise ValueError("fn should be corr or cov")
         cov_matrix_ts = getattr(ror.expanding(), fn)()
@@ -531,25 +523,50 @@
         Returns the rolling correlation (or covariance) time series.
         The history period should be at least 12 months.
         """
         if ror.shape[1] < 2:
             raise ValueError("At least 2 symbols should be provided.")
         if fn not in ["cov", "corr"]:
             raise ValueError("fn should be corr or cov")
-        check_rolling_window(window, ror)
+        check_rolling_window(window=window, ror=ror, window_below_year=False)
         cov_matrix_ts = getattr(ror.rolling(window=window), fn)()
         cov_matrix_ts = cov_matrix_ts.drop(index=ror.columns[1:], level=1).droplevel(1)
         cov_matrix_ts.drop(columns=ror.columns[0], inplace=True)
         cov_matrix_ts.dropna(inplace=True)
         return cov_matrix_ts
 
     @staticmethod
     def beta(ror: pd.DataFrame) -> pd.DataFrame:
         """
         Calculate beta coefficient time series.
         Index (or benchmark) should be in the first position (first column).
         The period should be at least 12 months.
         """
-        cov = Index.cov_cor(ror, fn="cov")
-        var = ror.expanding().var().drop(columns=ror.columns[0])
-        var = var[settings._MONTHS_PER_YEAR :]
-        return cov / var
+        if ror.shape[1] < 2:
+            raise ValueError("At least 2 symbols should be provided to calculate beta coefficient.")
+        if ror.shape[0] < 12:
+            raise ValueError("Beta coefficient is not defined for time periods < 1 year")
+        cov = Index.expanding_cov_cor(ror, fn="cov")
+        benchmark_var = ror.loc[:, ror.columns[0]].expanding().var()
+        benchmark_var = benchmark_var.iloc[settings._MONTHS_PER_YEAR :]
+        return cov.divide(benchmark_var, axis=0)
+
+    @staticmethod
+    def rolling_fn(df: pd.DataFrame, window: int, fn: Callable, window_below_year: bool = False) -> pd.DataFrame:
+        """
+        Calculate the rolling custom function.
+
+        Apply a function to time series DataFrame with the rolling window.
+        The window should be in months.
+        """
+        check_rolling_window(window=window, ror=df, window_below_year=window_below_year)
+        output = pd.DataFrame()
+        for start_date in df.index:
+            end_date = start_date + window
+            df_window = df.loc[start_date:end_date, :]
+            end_date = df_window.index[-1]
+            period_length = end_date - start_date
+            if period_length.n < window:
+                break
+            windows_result = fn(df_window).iloc[-1, :]
+            output = pd.concat([output, windows_result.to_frame().T], copy=False)
+        return output
```

### Comparing `okama-1.2.3/okama/common/helpers/ratios.py` & `okama-1.3.0/okama/common/helpers/ratios.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/common/make_asset_list.py` & `okama-1.3.0/okama/common/make_asset_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,21 +87,27 @@
             self.assets_ror.shape[0] // settings._MONTHS_PER_YEAR,
             self.assets_ror.shape[0] % settings._MONTHS_PER_YEAR,
         )
         self._pl_txt = f"{self.pl.years} years, {self.pl.months} months"
         self._dividend_yield: pd.DataFrame = pd.DataFrame(dtype=float)
         self._assets_dividends_ts: pd.DataFrame = pd.DataFrame(dtype=float)
 
+    def __iter__(self):
+        return iter(self.asset_obj_dict.values())
+
     @abstractmethod
     def __repr__(self):
         pass
 
     def __len__(self):
         return len(self.symbols)
 
+    def __getitem__(self, item):
+        return list(self.asset_obj_dict.values())[item]
+
     def _make_list(self, ls: list, first_date, last_date) -> dict:
         """
         Make an asset list from a list of symbols.
         """
         base_currency_ticker: str = self._currency.ticker
         currency_first_date: pd.Timestamp = self._currency.first_date
         currency_last_date: pd.Timestamp = self._currency.last_date
@@ -257,15 +263,15 @@
         Get monthly dividend time series for a single symbol and adjust to the currency.
         """
         asset = self.asset_obj_dict[tick]
         s = asset.dividends[self.first_date : self.last_date]
         if asset.currency != self.currency:
             s = self._adjust_price_to_currency_monthly(s, asset.currency)
         if remove_forecast:
-            s = s[: pd.Period.now(freq="M")]
+            s = s[: pd.Period.now(freq="M")]  # Period.now() must be without arguments to be compatible with pandas 2.0
         # Create time series with zeros to pad the empty spaces in dividends time series
         index = pd.date_range(start=self.first_date, end=self.last_date, freq="MS")  # 'MS' to include the last period
         period = index.to_period("M")
         pad_s = pd.Series(data=0, index=period)
         return s.add(pad_s, fill_value=0)
 
     def _get_assets_dividends(self, remove_forecast=True) -> pd.DataFrame:
```

### Comparing `okama-1.2.3/okama/common/validators.py` & `okama-1.3.0/okama/common/validators.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/frontier/multi_period.py` & `okama-1.3.0/okama/frontier/multi_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def __init__(
         self,
         assets: Optional[List[str]] = None,
         *,
         first_date: Optional[str] = None,
         last_date: Optional[str] = None,
         ccy: str = "USD",
-        inflation: bool = True,
+        inflation: bool = False,
         full_frontier: bool = True,
         rebalancing_period: str = "year",
         n_points: int = 20,
         verbose: bool = False,
         ticker_names: bool = True,
     ):
         if len(assets) < 2:
```

### Comparing `okama-1.2.3/okama/frontier/single_period.py` & `okama-1.3.0/okama/frontier/single_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self,
         assets: Optional[List[str]] = None,
         *,
         first_date: Optional[str] = None,
         last_date: Optional[str] = None,
         ccy: str = "USD",
         bounds: Optional[Tuple[Tuple[float, ...], ...]] = None,
-        inflation: bool = True,
+        inflation: bool = False,
         full_frontier: bool = True,
         n_points: int = 20,
         ticker_names: bool = True,
     ):
         if len(assets) < 2:
             raise ValueError("The number of symbols cannot be less than two")
         super().__init__(
@@ -882,15 +882,15 @@
                 point["Return"] = mean_return
             else:
                 raise ValueError('kind should be "mean" or "cagr"')
             random_portfolios = pd.concat([random_portfolios, pd.DataFrame(point, index=[0])], ignore_index=True)
             random_portfolios = helpers.Frame.change_columns_order(random_portfolios, ["Risk", second_column])
         return random_portfolios
 
-    def plot_transition_map(self, cagr: bool = True, figsize: Optional[tuple] = None) -> plt.axes:
+    def plot_transition_map(self, x_axe: str = 'risk', figsize: Optional[tuple] = None) -> plt.axes:
         """
         Plot Transition Map for optimized portfolios on the single period Efficient Frontier.
 
         Transition Map shows the relation between asset weights and optimized portfolios properties:
 
         - CAGR (Compound annual growth rate)
         - Risk (annualized standard deviation of return)
@@ -908,52 +908,56 @@
         ----------
         bounds: tuple of ((float, float),...)
             Bounds for the assets weights. Each asset can have weights limitation from 0 to 1.0.
             If an asset has limitation for 10 to 20%, bounds are defined as (0.1, 0.2).
             bounds = ((0, .5), (0, 1)) shows that in Portfolio with two assets first one has weight limitations
             from 0 to 50%. The second asset has no limitations.
 
-        cagr : bool, default True
-            Show the relation between weights and CAGR (if True) or between weights and Risk (if False).
-            of - sets X axe to CAGR (if true) or to risk (if false).
+        x_axe : {'risk', 'cagr'}, default 'risk'
+            Show the relation between weights and CAGR (if 'cagr') or between weights and Risk (if 'risk').
             CAGR or Risk are displayed on the x-axis.
 
         figsize: (float, float), optional
             Figure size: width, height in inches.
             If None default matplotlib size is taken: [6.4, 4.8]
 
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> x = ok.EfficientFrontier(['SPY.US', 'AGG.US', 'GLD.US'], ccy='USD', inflation=False)
         >>> x.plot_transition_map()
         >>> plt.show()
 
-        Transition Map with default setting show the relation between Return (CAGR) and assets weights for optimized portfolios.
-        The same relation for Risk can be shown setting cagr=False.
+        Transition Map with default setting show the relation between Risk (stanrd deviation) and assets weights for
+        optimized portfolios.
+        The same relation for CAGR can be shown setting x_axe='cagr'.
 
-        >>> x.plot_transition_map(cagr=False)
+        >>> x.plot_transition_map(x_axe='cagr')
         >>> plt.show()
         """
         ef = self.ef_points
         linestyle = itertools.cycle(("-", "--", ":", "-."))
-        x_axe = "CAGR" if cagr else "Risk"
+        if x_axe.lower() == 'cagr':
+            xlabel = "CAGR (Compound Annual Growth Rate)"
+            x_axe = "CAGR"
+        elif x_axe.lower() == 'risk':
+            xlabel = "Risk (volatility)"
+            x_axe = "Risk"
+        else:
+            raise ValueError("x_axe parameter must be 'cagr' or 'risk'.")
         fig, ax = plt.subplots(figsize=figsize)
         for i in ef:
             if i not in (
                 "Risk",
                 "Mean return",
                 "CAGR",
             ):  # select only columns with tickers
                 ax.plot(ef[x_axe], ef.loc[:, i], linestyle=next(linestyle), label=i)
         ax.set_xlim(ef[x_axe].min(), ef[x_axe].max())
-        if cagr:
-            ax.set_xlabel("CAGR (Compound Annual Growth Rate)")
-        else:
-            ax.set_xlabel("Risk (volatility)")
+        ax.set_xlabel(xlabel)
         ax.set_ylabel("Weights of assets")
         ax.legend(loc="upper left", frameon=False)
         fig.tight_layout()
         return ax
 
     def plot_pair_ef(self, tickers="tickers", figsize: Optional[tuple] = None) -> plt.axes:
         """
@@ -1006,15 +1010,15 @@
         >>> # Plot the full Efficient Frontier for 4 asset portfolios.
         >>> ax.plot(df4['Risk'], df4['Mean return'], color = 'black', linestyle='--')
         >>> plt.show()
         """
         if len(self.symbols) < 3:
             raise ValueError("The number of symbols cannot be less than 3")
         # self._verify_axes()
-        bool_inflation = bool(self.inflation)
+        bool_inflation = hasattr(self, "inflation")
         fig, ax = plt.subplots(figsize=figsize)
         for i in itertools.combinations(self.symbols, 2):
             sym_pair = list(i)
             index0 = self.symbols.index(sym_pair[0])
             index1 = self.symbols.index(sym_pair[1])
             bounds_pair = (self.bounds[index0], self.bounds[index1])
             ef = EfficientFrontier(
@@ -1037,14 +1041,15 @@
         The Capital Market Line (CML) is the tangent line drawn from the point of the risk-free asset (volatility is
         zero) to the point of tangency portfolio or Maximum Sharpe Ratio (MSR) point.
 
         The slope of the CML is the Sharpe ratio of the tangency portfolio.
 
         Parameters
         ----------
+        TODO: add y_axe parameter (arithmetic_mean or cagr)
         rf_return : float, default 0
             Risk-free rate of return.
 
         figsize: (float, float), optional
             Figure size: width, height in inches.
             If None default matplotlib size is taken: [6.4, 4.8]
```

### Comparing `okama-1.2.3/okama/macro.py` & `okama-1.3.0/okama/macro.py`

 * *Files identical despite different names*

### Comparing `okama-1.2.3/okama/portfolio.py` & `okama-1.3.0/okama/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,23 +360,18 @@
         Examples
         --------
         >>> import matplotlib.pyplot as plt
         >>> pf = ok.Portfolio(['VOO.US', 'GLD.US'], weights=[0.8, 0.2])
         >>> pf.wealth_index_with_assets.plot()
         >>> plt.show()
         """
+        ls = [self.ror, self.assets_ror]
         if hasattr(self, "inflation"):
-            df = pd.concat(
-                [self.ror, self.assets_ror, self.inflation_ts],
-                axis=1,
-                join="inner",
-                copy="false",
-            )
-        else:
-            df = pd.concat([self.ror, self.assets_ror], axis=1, join="inner", copy="false")
+            ls.append(self.inflation_ts)
+        df = pd.concat(ls, axis=1, join="inner", copy="false")
         return helpers.Frame.get_wealth_indexes(df)
 
     @property
     def mean_return_monthly(self) -> float:
         """
         Calculate monthly mean return (arithmetic mean) for the portfolio rate of return time series.
 
@@ -480,14 +475,15 @@
 
         To get inflation adjusted return (real annualized return) add `real=True` option:
 
         >>> pf.get_cagr(period=5, real=True)
         portfolio_5625.PF    0.121265
         dtype: float64
         """
+        # TODO: add option assets=False
         ts = self._add_inflation()
         df = self._make_df_if_series(ts)
         dt0 = self.last_date
         if period is None:
             dt = self.first_date
         else:
             self._validate_period(period)
@@ -1257,15 +1253,15 @@
         --------
         >>> pf = ok.Portfolio(['SPY.US', 'AGG.US', 'GLD.US'], weights=[.60, .35, .05], rebalancing_period='year')
         >>> pf.percentile_inverse_cagr(distr='lognorm', score=0, years=1, n=5000)
         18.08
         The probability of getting negative result (score=0) in 1 year period for lognormal distribution.
         """
         if distr == "hist":
-            cagr_distr = self.get_rolling_cagr(years * settings._MONTHS_PER_YEAR)
+            cagr_distr = self.get_rolling_cagr(years * settings._MONTHS_PER_YEAR).loc[:, [self.symbol]].squeeze()
         elif distr in ["norm", "lognorm"]:
             if not n:
                 n = 1000
             cagr_distr = self._get_cagr_distribution(distr=distr, years=years, n=n)
         else:
             raise ValueError('distr should be one of "norm", "lognorm", "hist".')
         return scipy.stats.percentileofscore(cagr_distr, score, kind="rank")
```

### Comparing `okama-1.2.3/README.md` & `okama-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 ```
 ![](../images/images/readmi07.jpg?raw=true)   
 <nowiki>*</nowiki> - *rebalancing period is one year*.
 
 ### 4. Get a Transition Map for allocations
 ```python
 ls = ['SPY.US', 'GLD.US', 'BND.US']
-map = ok.EfficientFrontier(ls, ccy='USD').plot_transition_map(cagr=False)
+map = ok.EfficientFrontier(ls, ccy='USD').plot_transition_map(x_axe='risk')
 ```
 ![](../images/images/readmi08.jpg?v23-11-2020,raw=true "Transition map")  
 
 More examples are available in form of [Jupyter Notebooks](https://github.com/mbk-dev/okama/tree/master/examples).
 
 ## Documentation
```

### Comparing `okama-1.2.3/setup.py` & `okama-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,237 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: okama
+Version: 1.3.0
+Summary: Investment portfolio analyzing & optimization tools
+Home-page: https://okama.io
+License: MIT
+Keywords: finance,investments,efficient frontier,python,optimization
+Author: Sergey Kikevich
+Author-email: chilango74@gmail.com
+Requires-Python: >=3.8,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: joblib (>=1.1.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
+Requires-Dist: pandas (>=1.4.0,<=1.6.0)
+Requires-Dist: pillow (<=9.1.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Project-URL: Documentation, https://okama.readthedocs.io/en/master
+Project-URL: Repository, https://github.com/mbk-dev/okama
+Description-Content-Type: text/markdown
+
+
+[![Documentation Status](https://img.shields.io/readthedocs/okama.svg?style=popout)](http://okama.readthedocs.io/)
+[![Python](https://img.shields.io/badge/python-v3-brightgreen.svg)](https://www.python.org/)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/okama.svg)](https://pypi.org/project/okama/)
+[![Coverage](https://coveralls.io/repos/github/mbk-dev/okama/badge.svg?branch=master)](https://coveralls.io/github/mbk-dev/okama?branch=master)
+[![License](https://img.shields.io/pypi/l/okama.svg)](https://opensource.org/licenses/MIT)
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mbk-dev/okama/blob/master/examples/01%20howto.ipynb)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Okama
+
+_okama_ is a library with investment portfolio analyzing & optimization tools. CFA recommendations are used in quantitative finance.
+
+_okama_ goes with **free** «end of day» historical stock markets data and macroeconomic indicators through API.
+>...entities should not be multiplied without necessity
+>
+> -- <cite>William of Ockham (c. 1287–1347)</cite>
+
+## Table of contents
+
+- [Okama main features](#okama-main-features)
+- [Financial data and macroeconomic indicators](#financial-data-and-macroeconomic-indicators)
+  - [End of day historical data](#end-of-day-historical-data)
+  - [Macroeconomic indicators](#macroeconomic-indicators)
+  - [Other historical data](#other-historical-data)
+- [Installation](#installation)
+- [Getting started](#getting-started)
+- [Documentation](#documentation)
+- [Financial Widgets](#financial-widgets)
+- [RoadMap](#roadmap)
+- [Contributing to okama](#contributing-to-okama)
+- [Communication](#communication)
+
+## Okama main features
+
+- Investment portfolio constrained Markowitz Mean-Variance Analysis (MVA) and optimization
+- Rebalanced portfolio optimization with constraints (multi-period Efficient Frontier)
+- Monte Carlo Simulations for financial assets and investment portfolios
+- Popular risk metrics: VAR, CVaR, semi-deviation, variance and drawdowns
+- Different financial ratios: Sharpe ratio, Sortino ratio, Diversification ratio 
+- Forecasting models according to normal and lognormal distribution
+- Testing distribution on historical data
+- Dividend yield and other dividend indicators for stocks
+- Backtesting and comparing historical performance of broad range of assets and indexes in multiple currencies
+- Methods to track the performance of index funds (ETF) and compare them with benchmarks
+- Main macroeconomic indicators: inflation, central banks rates
+- Matplotlib visualization scripts for the Efficient Frontier, Transition map and assets risk / return performance
+
+## Financial data and macroeconomic indicators
+
+### End of day historical data
+
+- Stocks and ETF for main world markets
+- Mutual funds
+- Commodities
+- Stock indexes
+
+### Currencies
+
+- FX currencies
+- Crypto currencies
+- Central bank exchange rates
+
+### Macroeconomic indicators
+For many countries (USA, United Kingdom, European Union, Russia, Israel etc.):  
+
+- Inflation
+- Central bank rates
+- CAPE10 (Shiller P/E) Cyclically adjusted price-to-earnings ratios
+
+### Other historical data
+
+- Real estate prices
+- Top bank rates
+
+## Installation
+
+`pip install okama`
+
+The latest development version can be installed directly from GitHub:
+
+`pip install git+https://github.com/mbk-dev/okama@dev`
+
+
+## Getting started
+
+### 1. Compare several assets from different stock markets. Get USD-adjusted performance
+
+```python
+import okama as ok
+
+x = ok.AssetList(['SPY.US', 'BND.US', 'DBXD.XFRA'], ccy='USD')
+x  # all examples are for Jupyter Notebook/iPython. For raw Python interpreter use 'print(x)' instead.
+
+```
+![](../images/images/readmi01.jpg?raw=true) 
+
+Get the main parameters for the set:
+```python
+x.describe()
+```
+![](../images/images/readmi02.jpg?raw=true) 
+
+Get the assets accumulated return, plot it and compare with the USD inflation:
+```python
+x.wealth_indexes.plot()
+```
+![](../images/images/readmi03.jpg?raw=true) 
+
+### 2. Create a dividend stocks portfolio with base currency EUR
+
+```python
+weights = [0.3, 0.2, 0.2, 0.2, 0.1]
+assets = ['T.US', 'XOM.US', 'FRE.XFRA', 'SNW.XFRA', 'LKOH.MOEX']
+pf = ok.Portfolio(assets, weights=weights, ccy='EUR')
+pf.table
+```
+![](../images/images/readmi04.jpg?raw=true) 
+
+Plot the dividend yield of the portfolio (adjusted to the base currency).
+
+```python
+pf.dividend_yield.plot()
+```
+![](../images/images/readmi05.png?raw=true) 
+
+### 3. Draw an Efficient Frontier for 2 popular ETF: SPY and GLD
+```python
+ls = ['SPY.US', 'GLD.US']
+curr = 'USD'
+last_date='2020-10'
+# Rebalancing periods is one year (default value)
+frontier = ok.EfficientFrontierReb(ls, last_date=last_date, ccy=curr, rebalancing_period='year')
+frontier.names
+```
+![](../images/images/readmi06.jpg?raw=true) 
+
+Get the Efficient Frontier points for rebalanced portfolios and plot the chart with the assets risk/CAGR points:
+```python
+import matplotlib.pyplot as plt
+
+points = frontier.ef_points
+
+fig = plt.figure(figsize=(12,6))
+fig.subplots_adjust(bottom=0.2, top=1.5)
+frontier.plot_assets(kind='cagr')  # plots the assets points on the chart
+ax = plt.gca()
+ax.plot(points.Risk, points.CAGR) 
+```
+![](../images/images/readmi07.jpg?raw=true)   
+<nowiki>*</nowiki> - *rebalancing period is one year*.
+
+### 4. Get a Transition Map for allocations
+```python
+ls = ['SPY.US', 'GLD.US', 'BND.US']
+map = ok.EfficientFrontier(ls, ccy='USD').plot_transition_map(x_axe='risk')
+```
+![](../images/images/readmi08.jpg?v23-11-2020,raw=true "Transition map")  
+
+More examples are available in form of [Jupyter Notebooks](https://github.com/mbk-dev/okama/tree/master/examples).
+
+## Documentation
+
+The official documentation is hosted on readthedocs.org: [https://okama.readthedocs.io/](https://okama.readthedocs.io/)
+
+## Financial Widgets
+[okama-dash](https://github.com/mbk-dev/okama-dash) repository has interactive financial widgets (multi-page web application) 
+build with _okama_ package and [Dash (plotly)](https://github.com/plotly/dash) framework. Working example is available at 
+[okama.io](https://okama.io/).
+
+![](https://github.com/mbk-dev/okama-dash/blob/images/images/main_page.jpg?raw=true) 
+
+## RoadMap
+
+The plan for _okama_ is to add more functions that will be useful to investors and asset managers.
+
+- Add Omega ratio to EfficientFrontier, EfficientFrontierReb and Portfolio classes.
+- Add withdrawals as an attribute of Portfolio class.
+- Add Black-Litterman asset allocation 
+- Accelerate optimization for multi-period Efficient Frontier: minimize_risk and maximize_risk methods of EfficientFrontierReb class.
+- Make a single EfficientFrontier class for all optimizations: single-period or multu-period with rebalancing period as a parameter.
+- Add different utility functions for optimizers: semi-deviation, VaR, CVaR, drawdowns etc.
+- Add more functions based on suggestion of users.
+
+## Contributing to okama
+
+Contributions are *most welcome*. Have a look at the [Contribution Guide](https://github.com/mbk-dev/okama/blob/master/CONTRIBUTING.md) for more.  
+Feel free to ask questions on [Discussuions](https://github.com/mbk-dev/okama/discussions).  
+As contributors and maintainers to this project, you are expected to abide by okama' code of conduct. More information can be found at: [Contributor Code of Conduct](https://github.com/mbk-dev/okama/blob/master/CODE_OF_CONDUCT.md)
 
-packages = \
-['okama', 'okama.api', 'okama.common', 'okama.common.helpers', 'okama.frontier']
+## Communication
 
-package_data = \
-{'': ['*']}
+For basic usage questions (e.g., "_Is XXX currency supported by okama?_") and for sharing ideas please use [GitHub Discussions](https://github.com/mbk-dev/okama/discussions/3).
+Russian language community is available at [okama.io forums](https://community.okama.io/c/python-okama).
 
-install_requires = \
-['joblib>=1.1.0,<2.0.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'pandas>=1.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'scipy>=0.14.0']
-
-setup_kwargs = {
-    'name': 'okama',
-    'version': '1.2.3',
-    'description': 'Investment portfolio analyzing & optimization tools',
-    'long_description': '\n[![Documentation Status](https://img.shields.io/readthedocs/okama.svg?style=popout)](http://okama.readthedocs.io/)\n[![Python](https://img.shields.io/badge/python-v3-brightgreen.svg)](https://www.python.org/)\n[![PyPI Latest Release](https://img.shields.io/pypi/v/okama.svg)](https://pypi.org/project/okama/)\n[![Coverage](https://coveralls.io/repos/github/mbk-dev/okama/badge.svg?branch=master)](https://coveralls.io/github/mbk-dev/okama?branch=master)\n[![License](https://img.shields.io/pypi/l/okama.svg)](https://opensource.org/licenses/MIT)\n[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mbk-dev/okama/blob/master/examples/01%20howto.ipynb)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# Okama\n\n_okama_ is a library with investment portfolio analyzing & optimization tools. CFA recommendations are used in quantitative finance.\n\n_okama_ goes with **free** «end of day» historical stock markets data and macroeconomic indicators through API.\n>...entities should not be multiplied without necessity\n>\n> -- <cite>William of Ockham (c. 1287–1347)</cite>\n\n## Table of contents\n\n- [Okama main features](#okama-main-features)\n- [Financial data and macroeconomic indicators](#financial-data-and-macroeconomic-indicators)\n  - [End of day historical data](#end-of-day-historical-data)\n  - [Macroeconomic indicators](#macroeconomic-indicators)\n  - [Other historical data](#other-historical-data)\n- [Installation](#installation)\n- [Getting started](#getting-started)\n- [Documentation](#documentation)\n- [Financial Widgets](#financial-widgets)\n- [RoadMap](#roadmap)\n- [Contributing to okama](#contributing-to-okama)\n- [Communication](#communication)\n\n## Okama main features\n\n- Investment portfolio constrained Markowitz Mean-Variance Analysis (MVA) and optimization\n- Rebalanced portfolio optimization with constraints (multi-period Efficient Frontier)\n- Monte Carlo Simulations for financial assets and investment portfolios\n- Popular risk metrics: VAR, CVaR, semi-deviation, variance and drawdowns\n- Different financial ratios: Sharpe ratio, Sortino ratio, Diversification ratio \n- Forecasting models according to normal and lognormal distribution\n- Testing distribution on historical data\n- Dividend yield and other dividend indicators for stocks\n- Backtesting and comparing historical performance of broad range of assets and indexes in multiple currencies\n- Methods to track the performance of index funds (ETF) and compare them with benchmarks\n- Main macroeconomic indicators: inflation, central banks rates\n- Matplotlib visualization scripts for the Efficient Frontier, Transition map and assets risk / return performance\n\n## Financial data and macroeconomic indicators\n\n### End of day historical data\n\n- Stocks and ETF for main world markets\n- Mutual funds\n- Commodities\n- Stock indexes\n\n### Currencies\n\n- FX currencies\n- Crypto currencies\n- Central bank exchange rates\n\n### Macroeconomic indicators\nFor many countries (USA, United Kingdom, European Union, Russia, Israel etc.):  \n\n- Inflation\n- Central bank rates\n- CAPE10 (Shiller P/E) Cyclically adjusted price-to-earnings ratios\n\n### Other historical data\n\n- Real estate prices\n- Top bank rates\n\n## Installation\n\n`pip install okama`\n\nThe latest development version can be installed directly from GitHub:\n\n`pip install git+https://github.com/mbk-dev/okama@dev`\n\n\n## Getting started\n\n### 1. Compare several assets from different stock markets. Get USD-adjusted performance\n\n```python\nimport okama as ok\n\nx = ok.AssetList([\'SPY.US\', \'BND.US\', \'DBXD.XFRA\'], ccy=\'USD\')\nx  # all examples are for Jupyter Notebook/iPython. For raw Python interpreter use \'print(x)\' instead.\n\n```\n![](../images/images/readmi01.jpg?raw=true) \n\nGet the main parameters for the set:\n```python\nx.describe()\n```\n![](../images/images/readmi02.jpg?raw=true) \n\nGet the assets accumulated return, plot it and compare with the USD inflation:\n```python\nx.wealth_indexes.plot()\n```\n![](../images/images/readmi03.jpg?raw=true) \n\n### 2. Create a dividend stocks portfolio with base currency EUR\n\n```python\nweights = [0.3, 0.2, 0.2, 0.2, 0.1]\nassets = [\'T.US\', \'XOM.US\', \'FRE.XFRA\', \'SNW.XFRA\', \'LKOH.MOEX\']\npf = ok.Portfolio(assets, weights=weights, ccy=\'EUR\')\npf.table\n```\n![](../images/images/readmi04.jpg?raw=true) \n\nPlot the dividend yield of the portfolio (adjusted to the base currency).\n\n```python\npf.dividend_yield.plot()\n```\n![](../images/images/readmi05.png?raw=true) \n\n### 3. Draw an Efficient Frontier for 2 popular ETF: SPY and GLD\n```python\nls = [\'SPY.US\', \'GLD.US\']\ncurr = \'USD\'\nlast_date=\'2020-10\'\n# Rebalancing periods is one year (default value)\nfrontier = ok.EfficientFrontierReb(ls, last_date=last_date, ccy=curr, rebalancing_period=\'year\')\nfrontier.names\n```\n![](../images/images/readmi06.jpg?raw=true) \n\nGet the Efficient Frontier points for rebalanced portfolios and plot the chart with the assets risk/CAGR points:\n```python\nimport matplotlib.pyplot as plt\n\npoints = frontier.ef_points\n\nfig = plt.figure(figsize=(12,6))\nfig.subplots_adjust(bottom=0.2, top=1.5)\nfrontier.plot_assets(kind=\'cagr\')  # plots the assets points on the chart\nax = plt.gca()\nax.plot(points.Risk, points.CAGR) \n```\n![](../images/images/readmi07.jpg?raw=true)   \n<nowiki>*</nowiki> - *rebalancing period is one year*.\n\n### 4. Get a Transition Map for allocations\n```python\nls = [\'SPY.US\', \'GLD.US\', \'BND.US\']\nmap = ok.EfficientFrontier(ls, ccy=\'USD\').plot_transition_map(cagr=False)\n```\n![](../images/images/readmi08.jpg?v23-11-2020,raw=true "Transition map")  \n\nMore examples are available in form of [Jupyter Notebooks](https://github.com/mbk-dev/okama/tree/master/examples).\n\n## Documentation\n\nThe official documentation is hosted on readthedocs.org: [https://okama.readthedocs.io/](https://okama.readthedocs.io/)\n\n## Financial Widgets\n[okama-dash](https://github.com/mbk-dev/okama-dash) repository has interactive financial widgets (multi-page web application) \nbuild with _okama_ package and [Dash (plotly)](https://github.com/plotly/dash) framework. Working example is available at \n[okama.io](https://okama.io/).\n\n![](https://github.com/mbk-dev/okama-dash/blob/images/images/main_page.jpg?raw=true) \n\n## RoadMap\n\nThe plan for _okama_ is to add more functions that will be useful to investors and asset managers.\n\n- Add Omega ratio to EfficientFrontier, EfficientFrontierReb and Portfolio classes.\n- Add withdrawals as an attribute of Portfolio class.\n- Add Black-Litterman asset allocation \n- Accelerate optimization for multi-period Efficient Frontier: minimize_risk and maximize_risk methods of EfficientFrontierReb class.\n- Make a single EfficientFrontier class for all optimizations: single-period or multu-period with rebalancing period as a parameter.\n- Add different utility functions for optimizers: semi-deviation, VaR, CVaR, drawdowns etc.\n- Add more functions based on suggestion of users.\n\n## Contributing to okama\n\nContributions are *most welcome*. Have a look at the [Contribution Guide](https://github.com/mbk-dev/okama/blob/master/CONTRIBUTING.md) for more.  \nFeel free to ask questions on [Discussuions](https://github.com/mbk-dev/okama/discussions).  \nAs contributors and maintainers to this project, you are expected to abide by okama\' code of conduct. More information can be found at: [Contributor Code of Conduct](https://github.com/mbk-dev/okama/blob/master/CODE_OF_CONDUCT.md)\n\n## Communication\n\nFor basic usage questions (e.g., "_Is XXX currency supported by okama?_") and for sharing ideas please use [GitHub Discussions](https://github.com/mbk-dev/okama/discussions/3).\nRussian language community is available at [okama.io forums](https://community.okama.io/c/python-okama).\n\n## License\n\nMIT\n',
-    'author': 'Sergey Kikevich',
-    'author_email': 'chilango74@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://okama.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0.0',
-}
+## License
 
+MIT
 
-setup(**setup_kwargs)
```

