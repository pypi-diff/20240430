# Comparing `tmp/tradelocker-0.40.0.tar.gz` & `tmp/tradelocker-0.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradelocker-0.40.0.tar", max compression
+gzip compressed data, was "tradelocker-0.41.0.tar", max compression
```

## Comparing `tradelocker-0.40.0.tar` & `tradelocker-0.41.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-28 19:44:48.930398 tradelocker-0.40.0/LICENSE.txt
--rw-r--r--   0        0        0     2829 2024-04-28 19:44:48.931056 tradelocker-0.40.0/README.md
--rw-r--r--   0        0        0     1476 2024-04-28 19:50:08.283720 tradelocker-0.40.0/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-28 19:44:48.950787 tradelocker-0.40.0/src/tradelocker/__about__.py
--rw-r--r--   0        0        0       85 2024-04-28 19:44:48.941751 tradelocker-0.40.0/src/tradelocker/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 19:44:48.950881 tradelocker-0.40.0/src/tradelocker/py.typed
--rw-r--r--   0        0        0    52279 2024-04-28 19:50:08.275201 tradelocker-0.40.0/src/tradelocker/tradelocker_api.py
--rw-r--r--   0        0        0     5342 2024-04-28 19:50:08.275982 tradelocker-0.40.0/src/tradelocker/types.py
--rw-r--r--   0        0        0     9168 2024-04-28 19:50:08.276686 tradelocker-0.40.0/src/tradelocker/utils.py
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 tradelocker-0.40.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-28 19:44:48.930398 tradelocker-0.41.0/LICENSE.txt
+-rw-r--r--   0        0        0     2829 2024-04-28 19:44:48.931056 tradelocker-0.41.0/README.md
+-rw-r--r--   0        0        0     1476 2024-04-30 07:42:37.704738 tradelocker-0.41.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-28 19:44:48.950787 tradelocker-0.41.0/src/tradelocker/__about__.py
+-rw-r--r--   0        0        0       85 2024-04-28 19:44:48.941751 tradelocker-0.41.0/src/tradelocker/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 19:44:48.950881 tradelocker-0.41.0/src/tradelocker/py.typed
+-rw-r--r--   0        0        0    55793 2024-04-30 07:42:37.705156 tradelocker-0.41.0/src/tradelocker/tradelocker_api.py
+-rw-r--r--   0        0        0     5350 2024-04-30 07:42:37.705578 tradelocker-0.41.0/src/tradelocker/types.py
+-rw-r--r--   0        0        0     9168 2024-04-29 12:27:29.894587 tradelocker-0.41.0/src/tradelocker/utils.py
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 tradelocker-0.41.0/PKG-INFO
```

### Comparing `tradelocker-0.40.0/LICENSE.txt` & `tradelocker-0.41.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tradelocker-0.40.0/README.md` & `tradelocker-0.41.0/README.md`

 * *Files identical despite different names*

### Comparing `tradelocker-0.40.0/pyproject.toml` & `tradelocker-0.41.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tradelocker"
-version = "0.40.0"
+version = "0.41.0"
 description = "TradeLocker Trading API support for Python"
 authors = ["TradeLocker <admin@tradelocker.com>"]
 license = "MIT"
 readme = "README.md"
 keywords=["tradelocker","api", "rest", "trading", "exchange", "algotrading", "algo", "bots", "strategies"]
 urls.Source = "https://github.com/tradelocker/tradelocker-python/"
 urls.Issues = "https://github.com/tradelocker/tradelocker-python/issues"
```

### Comparing `tradelocker-0.40.0/src/tradelocker/tradelocker_api.py` & `tradelocker-0.41.0/src/tradelocker/tradelocker_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     InstrumentDetailsType,
     LimitsType,
     LocaleType,
     LogLevelType,
     MarketDepthlistType,
     ModificationParamsType,
     OrderTypeType,
+    StopLossType,
+    TakeProfitType,
     RequestsMappingType,
     ResolutionType,
     RouteType,
     RouteTypeType,
     SessionDetailsType,
     SessionStatusDetailsType,
     TradeAccountsType,
@@ -765,15 +767,15 @@
     @lru_cache(maxsize=1)
     @log_func
     @tl_typechecked
     def get_all_accounts(self) -> pd.DataFrame:
         """Returns all accounts associated with the account used for authentication.
 
         Raises:
-            Exception: Will be raised if account informations could not be fetched
+            Exception: Will be raised if account information could not be fetched
 
         Returns:
             pd.DataFrame[AccountsColumnsTypes]: DataFrame with user's accounts
         """
         route_url = f"{self._base_url}/auth/jwt/all-accounts"
 
         # Make sure we don't try including accNum into the header, as it is not chosen yet
@@ -1142,30 +1144,47 @@
         self._apply_typing(bar_details, PriceHistoryColumns)
 
         return bar_details
 
     @log_func
     @tl_typechecked
     def get_latest_asking_price(self, instrument_id: int) -> float:
-        """Returns latest price informations for requested instrument.
+        """Returns latest asking price for requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
-            float: Latest price of the instrument
+            float: Latest asking price of the instrument
         """
         current_quotes: dict[str, float] = cast(
             dict[str, float], self.get_quotes(instrument_id)
         )
         current_ap: float = get_nested_key(current_quotes, ["ap"], float)
         return current_ap
 
     @log_func
     @tl_typechecked
+    def get_latest_bid_price(self, instrument_id: int) -> float:
+        """Returns latest bid price for requested instrument.
+
+        Args:
+            instrument_id (int): Instrument Id
+
+        Returns:
+            float: Latest bid price of the instrument
+        """
+        current_quotes: dict[str, float] = cast(
+            dict[str, float], self.get_quotes(instrument_id)
+        )
+        current_bp: float = get_nested_key(current_quotes, ["bp"], float)
+        return current_bp
+
+    @log_func
+    @tl_typechecked
     def get_quotes(self, instrument_id: int) -> QuotesType:
         """Returns price quotes for requested instrument.
 
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
@@ -1235,69 +1254,94 @@
                     self.log.debug(
                         "New position completely netted from opposite positions."
                     )
                     break
 
         return total_netted
 
+    # TODO: add tests for sl/tp
     @log_func
     @tl_typechecked
     def create_order(
         self,
         instrument_id: int,
         quantity: float,
         side: SideType,
-        price: float = 0,
+        price: Optional[float] = None,
         type_: OrderTypeType = "market",
         validity: Optional[ValidityType] = None,
         position_netting: bool = False,
-        stop_loss: Optional[float] = None,
         take_profit: Optional[float] = None,
+        take_profit_type: Optional[TakeProfitType] = None,
+        stop_loss: Optional[float] = None,
+        stop_loss_type: Optional[StopLossType] = None,
+        stop_price: Optional[float] = None,
     ) -> Optional[int]:
         """Creates an order.
 
         Args:
             instrument_id (int): Instrument Id
             quantity (float): Order size
             side (SideType): Order side
             price (float, optional): Price for non-market orders. Defaults to 0.
             type_ (OrderTypeType, optional): Order type. Defaults to "market".
             validity (ValidityType, optional): Validity type of order. Defaults to "IOC".
             position_netting (bool, optional): Should position netting be used. Defaults to False.
-            stop_loss (float, optional): Stop Loss. Defaults to None.
-            take_profit (float, optional): Take Profit. Defaults to None.
+            take_profit (float, optional): Take profit value. Defaults to None.
+            take_profit_type (_TakeProfitType, optional): Take profit type. Defaults to None.
+            stop_loss (float, optional): Stop loss value. Defaults to None.
+            stop_loss_type (_StopLossType, optional): Stop loss type. Defaults to None.
 
         Returns:
-            Optional[int]: order_id or None if order could not be placed
+            Optional[int]: Order Id if order created, otherwise None
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/orders"
 
-        if type_ == "market" and price != 0:
+        if type_ == "market" and price:
             self.log.warning("Price specified for a market order. Ignoring the price.")
-            price = 0
+            price = None
 
         if type_ == "market":
             if validity and validity != "IOC":
                 error_msg = (
                     f"Market orders must use IOC as validity. Not placing the order."
                 )
                 self.log.error(error_msg)
                 raise ValueError(error_msg)
             else:
                 validity = "IOC"
+        elif validity and validity != "GTC":
+            error_msg = (
+                f"{type_} orders must use GTC as validity. Not placing the order."
+            )
+            self.log.error(error_msg)
+            raise ValueError(error_msg)
 
-        if type_ == "limit":
-            if type_ in ["limit", "stop"] and validity and validity != "GTC":
-                error_msg = (
-                    f"{type_} orders must use GTC as validity. Not placing the order."
+        if stop_loss and not stop_loss_type:
+            warning_msg = "Stop loss value specified, but no stop loss type. Continuing with 'absolute'"
+            self.log.warning(warning_msg)
+            stop_loss_type = "absolute"
+
+        if take_profit and not take_profit_type:
+            warning_msg = "Take profit value specified, but no take profit type. Continuing with 'absolute'"
+            self.log.warning(warning_msg)
+            take_profit_type = "absolute"
+
+        if type == "stop" and stop_price == None:
+            if not price:
+                self.log.error(
+                    "Stop orders must have a stop price set. Not placing the order."
                 )
-                self.log.error(error_msg)
-                raise ValueError(error_msg)
-            else:
-                validity = "GTC"
+                return None
+
+            stop_price = price
+            price = None
+            self.log.warning(
+                f"Order of {type_ = } specified, but no stop_price set. Using price as stop price."
+            )
 
         # Make sure that quantity is positive. If not, switch the side of the order
         if quantity < 0:
             quantity = abs(quantity)
             side = "sell" if (side == "buy") else "buy"
             self.log.warning(
                 "Quantity was negative, Continuing by changing the side of the order."
@@ -1316,24 +1360,28 @@
         # If the quantity is smaller than the minimum lot size, return
         if quantity < _MIN_LOT_SIZE:
             self.log.warning(
                 "Unable to place an order with quantity smaller than min lot size of {_MIN_LOT_SIZE}"
             )
             return None
 
-        request_body: dict[str, str] = {
-            "price": str(price),
+        request_body = {
+            "price": price,
+            "stopPrice": stop_price,
             "qty": str(quantity),
             "routeId": self._get_trade_route_id(instrument_id),
             "side": side,
             "validity": validity,
             "tradableInstrumentId": str(instrument_id),
             "type": type_,
-            "stopLoss": stop_loss,
             "takeProfit": take_profit,
+            "takeProfitType": take_profit_type,
+            "stopLoss": stop_loss,
+            "stopLossType": stop_loss_type,
+            "stopPrice": stop_price,
         }
 
         if position_netting:
             # Try finding opposite orders to net against
             if type_ == "market":
                 total_netted = self._perform_order_netting(
                     instrument_id, side, quantity
@@ -1415,10 +1463,59 @@
         response = requests.patch(
             url=route_url,
             headers=self._get_headers({"Content-type": "application/json"}),
             json=modification_params,
             timeout=_TIMEOUT,
         )
         response_json = self._get_response_json(response)
-        self.log.info(f"Order modification response: {response_json}")
         response_status: str = get_nested_key(response_json, ["s"], str)
         return response_status == "ok"
+
+    @log_func
+    @tl_typechecked
+    def modify_position(
+        self, position_id: int, modification_params: ModificationParamsType
+    ) -> bool:
+        """Modifies an open position.
+
+        Args:
+            position_id (int): Position Id
+            modification_params (_ModificationParamsType): Position modification details
+
+        Returns:
+            bool: True on success, False on error
+        """
+        route_url = f"{self._base_url}/trade/positions/{position_id}"
+
+        self.log.info(f"Modifying the position with id {position_id}")
+
+        response = requests.patch(
+            url=route_url,
+            headers=self._get_headers({"Content-type": "application/json"}),
+            json=modification_params,
+            timeout=_TIMEOUT,
+        )
+        response_json = self._get_response_json(response)
+        response_status: str = get_nested_key(response_json, ["s"], str)
+        return response_status == "ok"
+
+    @log_func
+    @tl_typechecked
+    def get_position_id_from_order_id(self, order_id: int) -> Optional[int]:
+        """Retrieves position_id from the given order_id (if one exists).
+
+        Args:
+            order_id (int): An order id
+
+        Returns:
+            Optional[int]: position_id or None
+        """
+        self.log.info(f"Getting execution id from orders history")
+        orders_history = self.get_all_orders(history=True)
+
+        matching_orders = orders_history[orders_history["id"] == order_id]
+        if len(matching_orders) == 0:
+            self.log.info(f"No matching order found for order_id: {order_id}")
+            return None
+
+        position_id = int(matching_orders["positionId"].iloc[0])
+        return position_id
```

### Comparing `tradelocker-0.40.0/src/tradelocker/types.py` & `tradelocker-0.41.0/src/tradelocker/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Literal["rateLimits"],
         list[RateLimitsType],
     ]
 )
 
 ResolutionType: TA = Literal["1M", "1W", "1D", "4H", "1H", "30m", "15m", "5m", "1m"]
 ModificationParamsType: TA = dict[
-    str, str | StopLossType | TakeProfitType | ValidityType
+    str, str | float | StopLossType | TakeProfitType | ValidityType
 ]
 LocaleType: TA = Literal[
     "ar", "en", "es", "fr", "ja", "ko", "pl", "pt", "ru", "tr", "ua", "zh_sm", "zh_tr"
 ]
 EnvironmentsType: TA = Literal["demo", "live"]
 DevEnvironmentsType: TA = Literal["dev", "stg", "exp"]  # For internal use
 RouteType: TA = dict[Literal["id", "type"], int | str]
```

### Comparing `tradelocker-0.40.0/src/tradelocker/utils.py` & `tradelocker-0.41.0/src/tradelocker/utils.py`

 * *Files identical despite different names*

### Comparing `tradelocker-0.40.0/PKG-INFO` & `tradelocker-0.41.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradelocker
-Version: 0.40.0
+Version: 0.41.0
 Summary: TradeLocker Trading API support for Python
 License: MIT
 Keywords: tradelocker,api,rest,trading,exchange,algotrading,algo,bots,strategies
 Author: TradeLocker
 Author-email: admin@tradelocker.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

