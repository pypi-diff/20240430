# Comparing `tmp/vxquant-20231018.tar.gz` & `tmp/vxquant-20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxquant-20231018.tar", max compression
+gzip compressed data, was "vxquant-20240414.tar", max compression
```

## Comparing `vxquant-20231018.tar` & `vxquant-20240414.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1226 2023-10-18 05:53:49.882364 vxquant-20231018/pyproject.toml
--rw-r--r--   0        0        0        9 2023-09-21 10:18:49.426080 vxquant-20231018/README.md
--rw-r--r--   0        0        0     2016 2023-09-21 06:11:01.642913 vxquant-20231018/vxquant/__main__.py
--rw-r--r--   0        0        0     2709 2023-10-16 06:26:03.732989 vxquant-20231018/vxquant/config.py
--rw-r--r--   0        0        0        0 2023-08-25 01:52:40.649511 vxquant-20231018/vxquant/datamodels/__init__.py
--rw-r--r--   0        0        0     6748 2023-08-24 03:17:50.170954 vxquant-20231018/vxquant/datamodels/contants.py
--rw-r--r--   0        0        0    10788 2023-10-18 05:53:37.062305 vxquant-20231018/vxquant/datamodels/core.py
--rw-r--r--   0        0        0    12594 2023-10-04 11:24:57.348012 vxquant-20231018/vxquant/datamodels/instruments.py
--rw-r--r--   0        0        0    10479 2023-08-25 03:13:17.619511 vxquant-20231018/vxquant/datamodels/preset.py
--rw-r--r--   0        0        0        0 2023-08-31 11:46:29.033523 vxquant-20231018/vxquant/datamodels/tools/__init__.py
--rw-r--r--   0        0        0     3410 2023-09-12 10:15:52.878876 vxquant-20231018/vxquant/datamodels/tools/gmtrade.py
--rw-r--r--   0        0        0     3974 2023-09-01 05:51:24.589955 vxquant-20231018/vxquant/datamodels/tools/tdx.py
--rw-r--r--   0        0        0     2981 2023-10-04 11:20:59.702040 vxquant-20231018/vxquant/datamodels/utils.py
--rw-r--r--   0        0        0       50 2023-09-06 10:01:16.524778 vxquant-20231018/vxquant/mdapi/__init__.py
--rw-r--r--   0        0        0      473 2023-10-18 04:49:33.674243 vxquant-20231018/vxquant/mdapi/base.py
--rw-r--r--   0        0        0        0 2023-08-25 01:52:51.729789 vxquant-20231018/vxquant/providers/__init__.py
--rw-r--r--   0        0        0     1676 2023-10-04 11:32:10.670495 vxquant-20231018/vxquant/providers/__pycache__/baostock.cpython-310.pyc
--rw-r--r--   0        0        0     1758 2023-10-04 11:55:11.850841 vxquant-20231018/vxquant/providers/baostock_api.py
--rw-r--r--   0        0        0     8351 2023-10-16 06:28:15.735089 vxquant-20231018/vxquant/providers/base.py
--rw-r--r--   0        0        0     3750 2023-10-18 04:45:58.372758 vxquant-20231018/vxquant/providers/mqtt.py
--rw-r--r--   0        0        0    16982 2023-10-19 01:10:53.582473 vxquant-20231018/vxquant/providers/spiders.py
--rw-r--r--   0        0        0     1063 2023-09-20 02:53:38.746915 vxquant-20231018/vxquant/providers/sub.py
--rw-r--r--   0        0        0    19488 2023-09-26 12:00:59.406610 vxquant-20231018/vxquant/providers/tdx.py
--rw-r--r--   0        0        0        0 2023-09-20 01:08:09.278790 vxquant-20231018/vxquant/pubsub/__init__.py
--rw-r--r--   0        0        0       49 2023-09-06 10:01:27.249427 vxquant-20231018/vxquant/tdapi/__init__.py
--rw-r--r--   0        0        0      394 2023-10-16 06:09:32.620558 vxquant-20231018/vxquant/tdapi/base.py
--rw-r--r--   0        0        0     6916 2023-10-16 06:09:57.205099 vxquant-20231018/vxquant/tdapi/gmtrade.py
--rw-r--r--   0        0        0      930 2023-09-12 12:03:26.859714 vxquant-20231018/vxquant/tdapi/miniqmt.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 vxquant-20231018/PKG-INFO
+-rw-r--r--   0        0        0     1877 2024-04-24 04:34:07.271188 vxquant-20240414/pyproject.toml
+-rw-r--r--   0        0        0        9 2024-03-09 11:57:35.000000 vxquant-20240414/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 01:51:48.150714 vxquant-20240414/src/vxcollector/__init__.py
+-rw-r--r--   0        0        0     2296 2024-03-21 03:01:25.422696 vxquant-20240414/src/vxcollector/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:48:35.252540 vxquant-20240414/src/vxcollector/init_mod/__init__.py
+-rw-r--r--   0        0        0     7018 2024-03-31 05:46:55.667301 vxquant-20240414/src/vxcollector/init_mod/start_up.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:31.789778 vxquant-20240414/src/vxcollector/mod/__init__.py
+-rw-r--r--   0        0        0      407 2024-03-21 02:48:11.599024 vxquant-20240414/src/vxcollector/mod/start_up.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240414/src/vxcollector/py.typed
+-rw-r--r--   0        0        0        0 2024-03-01 13:26:50.522744 vxquant-20240414/src/vxquant/__init__.py
+-rw-r--r--   0        0        0     5322 2024-04-14 08:25:39.535966 vxquant-20240414/src/vxquant/__main__.py
+-rw-r--r--   0        0        0     1026 2024-03-02 03:35:54.729169 vxquant-20240414/src/vxquant/exceptions.py
+-rw-r--r--   0        0        0     7563 2024-04-14 07:10:13.802634 vxquant-20240414/src/vxquant/mdapi.py
+-rw-r--r--   0        0        0        1 2024-03-09 14:37:11.000000 vxquant-20240414/src/vxquant/models/__init__.py
+-rw-r--r--   0        0        0    11484 2024-04-25 07:03:19.266835 vxquant-20240414/src/vxquant/models/base.py
+-rw-r--r--   0        0        0     3910 2024-03-09 12:41:00.040710 vxquant-20240414/src/vxquant/models/constants.py
+-rw-r--r--   0        0        0     3736 2024-03-19 06:26:36.698404 vxquant-20240414/src/vxquant/models/industry.py
+-rw-r--r--   0        0        0    11658 2024-03-20 05:53:35.455372 vxquant-20240414/src/vxquant/models/instruments.py
+-rw-r--r--   0        0        0     3042 2024-04-30 06:06:01.702259 vxquant-20240414/src/vxquant/models/nomalize.py
+-rw-r--r--   0        0        0    12548 2024-04-30 06:09:51.332634 vxquant-20240414/src/vxquant/models/preset.py
+-rw-r--r--   0        0        0        0 2024-03-09 12:47:51.000000 vxquant-20240414/src/vxquant/providers/__init__.py
+-rw-r--r--   0        0        0     2997 2024-03-20 06:09:46.192349 vxquant-20240414/src/vxquant/providers/bsproviders.py
+-rw-r--r--   0        0        0        0 2024-04-15 01:28:38.285351 vxquant-20240414/src/vxquant/providers/miniqmt/__init__.py
+-rw-r--r--   0        0        0     7312 2024-04-25 06:59:35.557211 vxquant-20240414/src/vxquant/providers/miniqmt/adapters.py
+-rw-r--r--   0        0        0    10228 2024-04-30 06:35:35.543215 vxquant-20240414/src/vxquant/providers/miniqmt/base.py
+-rw-r--r--   0        0        0     1948 2024-03-31 06:22:33.395459 vxquant-20240414/src/vxquant/providers/spiders.py
+-rw-r--r--   0        0        0        0 2024-03-31 06:20:15.881547 vxquant-20240414/src/vxquant/providers/tsproviders.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxquant-20240414/src/vxquant/py.typed
+-rw-r--r--   0        0        0     7194 2024-04-26 03:17:05.458452 vxquant-20240414/src/vxquant/tdapi.py
+-rw-r--r--   0        0        0     8518 2024-04-07 01:35:53.845511 vxquant-20240414/src/vxquant/teller.py
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 vxquant-20240414/PKG-INFO
```

### Comparing `vxquant-20231018/vxquant/datamodels/instruments.py` & `vxquant-20240414/src/vxquant/models/instruments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,223 +1,202 @@
 """股票池"""
+
+import logging
 import datetime
 import polars as pl
 from pathlib import Path
-from typing import List, Union, Dict
-from vxutils import to_datetime, vxtime, to_timestamp, logger
-from vxquant.datamodels.utils import to_symbol, DateTimeType, InstrumentType
+from typing import List, Union, Dict, Tuple, Optional, Any, Literal
+from vxquant.models.nomalize import to_symbol as normalize_symbol
+from vxutils import Datetime, to_datetime
 
 
-__all__ = ["vxInstruments"]
+__all__ = ["VXInstruments"]
 
 
-def is_in_periods(dt, periods):
-    dt = to_timestamp(dt) * 1_000_000
+def is_in_periods(
+    dt: Datetime, periods: List[Tuple[datetime.datetime, datetime.datetime]]
+) -> bool:
+    """判断日期是否在时间段内"""
+    dt = to_datetime(dt)
     return any(period[0] <= dt <= period[1] for period in periods)
 
 
-class vxInstruments:
+class VXInstruments:
     """股票池类"""
 
-    def __init__(self, name: str, registrations: pl.DataFrame = None):
+    def __init__(self, name: str, registrations: Optional[pl.DataFrame] = None) -> None:
         self._name = name
         self._registrations = (
             registrations.with_columns(
                 [
-                    pl.col("start_date").apply(to_datetime),
-                    pl.col("end_date").apply(to_datetime),
+                    pl.col("start_date").cast(pl.Datetime),
+                    pl.col("end_date").cast(pl.Datetime),
                 ]
             )
             if registrations is not None
             else pl.DataFrame(
-                {"symbol": [], "start_date": [], "end_date": [], "weight": []},
+                # {"symbol": [], "start_date": [], "end_date": [], "weight": []},
+                {"symbol": [], "start_date": [], "end_date": []},
                 schema={
                     "symbol": pl.Utf8,
                     "start_date": pl.Datetime,
                     "end_date": pl.Datetime,
-                    "weight": pl.Float64,
                 },
             )
         )
         self._last_updated_dt = (
-            to_datetime(vxtime.today())
+            datetime.datetime.today()
             if self._registrations.height == 0
-            else self._registrations["end_date"].max()
+            else to_datetime(self._registrations["end_date"].max())
         )
 
     @property
     def name(self) -> str:
         """股票池名称"""
         return self._name
 
     def __str__(self) -> str:
-        return (
-            f"< 证券池({self._name}) 最近更新日期"
-            f":{self._last_updated_dt:%Y-%m-%d}"
-            f" 最新证券:\n {self.list_instruments(self._last_updated_dt)} >"
-        )
+        return f"< 证券池({self._name}) " f" 最新证券:\n {self.list_instruments()} >"
 
     @property
     def registrations(self) -> pl.DataFrame:
         """股票池出入注册表
 
         Returns:
             pl.DataFrame -- 注册表
         """
         return self._registrations
 
-    @property
-    def last_updated_dt(self) -> DateTimeType:
-        """最近更新日期
-
-        Returns:
-            DateTimeType -- 日期类型:datetime类型
-        """
-        return self._last_updated_dt
-
-    def list_instruments(self, trade_date: DateTimeType = None) -> List[InstrumentType]:
+    def list_instruments(
+        self, trade_date: Optional[Datetime] = None
+    ) -> List[datetime.datetime]:
         """列出股票池中的证券
 
         Keyword Arguments:
-            trade_date {DateTimeType} -- 交易日，若为空，则为当前日期 (default: {None})
+            trade_date {Datetime} -- 交易日，若为空，则为当前日期 (default: {None})
 
         Returns:
             List[InstrumentType] -- 股票列表
         """
-        trade_date = min(
-            to_datetime(trade_date or vxtime.today()), self._last_updated_dt
+        trade_date = (
+            to_datetime(trade_date)
+            if trade_date is not None
+            else datetime.datetime.today()
         )
 
         inst = self._registrations.filter(
-            ((pl.col("start_date") <= trade_date) & (pl.col("end_date") >= trade_date))
+            [(pl.col("start_date") <= trade_date), (pl.col("end_date") >= trade_date)]
         )
 
         return inst["symbol"].to_list()
 
-    def get_weights(self, trade_date: DateTimeType = None) -> Dict[str, float]:
-        """获取权重信息
-
-        Keyword Arguments:
-            trade_date {DateTimeType} -- 交易日，若为空，则为当前日期 (default: {None})
-
-        Returns:
-            Dict[str,float] -- 权重信息
-        """
-        trade_date = min(
-            to_datetime(trade_date or vxtime.today()), self._last_updated_dt
-        )
-
-        inst = self._registrations.filter(
-            ((pl.col("start_date") <= trade_date) & (pl.col("end_date") >= trade_date))
-        )
-        return dict(*inst.select(["symbol", "weight"]).to_struct().arr)
-
     def add_instrument(
         self,
-        symbol: InstrumentType,
-        start_date: DateTimeType,
-        end_date: DateTimeType = None,
-        weight: float = 1.0,
-    ):
+        symbol: str,
+        start_date: Datetime,
+        end_date: Optional[Datetime] = None,
+        #
+    ) -> "VXInstruments":
         try:
-            symbol = to_symbol(symbol)
+            symbol = normalize_symbol(symbol)
             start_date = to_datetime(start_date)
             end_date = to_datetime(end_date) if end_date else start_date
         except Exception as e:
-            logger.error(f"ValueError: {e}")
-            return
+            raise ValueError(f"参数错误: {e}")
 
         self._registrations.vstack(
             pl.DataFrame(
                 [
                     {
                         "symbol": symbol,
                         "start_date": start_date,
                         "end_date": end_date,
-                        "weight": weight,
                     }
-                ]
+                ],
+                schema={
+                    "symbol": str,
+                    "start_date": pl.Datetime,
+                    "end_date": pl.Datetime,
+                },
             ),
             in_place=True,
         )
         return self
 
     def update_components(
         self,
-        instruments: Union[List[InstrumentType], Dict[InstrumentType, float]],
-        updated_dt: DateTimeType = None,
-    ):
+        instruments: List[str],
+        start_date: Datetime,
+        end_date: Datetime,
+    ) -> "VXInstruments":
         """按增量更新股票池"""
 
-        updated_dt = to_datetime(updated_dt or vxtime.today())
-        if (not self._registrations.is_empty()) and self._last_updated_dt >= updated_dt:
-            raise ValueError(
-                f"updated_dt( {updated_dt:%Y-%m-%d} ) 小于当前更新时间:"
-                f" {self._last_updated_dt:%Y-%m-%d}"
-            )
+        end_date = to_datetime(end_date)
+        start_date = to_datetime(start_date)
 
-        if isinstance(instruments, (list, tuple)):
-            datas = [
-                {"symbol": symbol, "end_date": self._last_updated_dt, "weight": 1.0}
+        new_instruments = pl.DataFrame(
+            [
+                {
+                    "symbol": normalize_symbol(symbol),
+                    "start_date": start_date,
+                    "end_date": end_date,
+                }
                 for symbol in instruments
-            ]
-        elif isinstance(instruments, dict):
-            datas = [
-                {"symbol": symbol, "end_date": self._last_updated_dt, "weight": weight}
-                for symbol, weight in instruments.items()
-            ]
-        else:
-            raise ValueError("instruments must be list or dict")
-
-        new_instruments = pl.DataFrame(datas)
-
-        self._registrations = (
-            self._registrations.join(
-                new_instruments, on=["symbol", "end_date"], how="outer"
-            )
-            .with_columns(
-                [
-                    pl.col("start_date").fill_null(updated_dt),
-                    pl.when(
-                        (pl.col("end_date") == self._last_updated_dt)
-                        & (pl.col("symbol").is_in(new_instruments["symbol"]))
-                    )
-                    .then(pl.lit(updated_dt))
-                    .otherwise(pl.col("end_date"))
-                    .alias("end_date"),
-                    pl.when(
-                        (pl.col("end_date") == self._last_updated_dt)
-                        & (pl.col("symbol").is_in(new_instruments["symbol"]))
-                    )
-                    .then(pl.col("weight_right"))
-                    .otherwise(pl.col("weight"))
-                    .alias("weight"),
-                ]
-            )
-            .select(["symbol", "start_date", "end_date", "weight"])
-            .sort(by="end_date")
+            ],
+            schema={
+                "symbol": pl.Utf8,
+                "start_date": pl.Datetime,
+                "end_date": pl.Datetime,
+            },
         )
-        self._last_updated_dt = updated_dt
+
+        self._registrations = pl.concat([self._registrations, new_instruments])
+        self.rebuild()
         return self
 
     @classmethod
-    def load(cls, name, instruments_parquet: Union[str, Path]) -> "vxInstruments":
-        registrations = pl.read_parquet(instruments_parquet)
-        return vxInstruments(name, registrations)
+    def load(cls, name: str, instruments_file: Union[str, Path]) -> "VXInstruments":
+        if isinstance(instruments_file, str):
+            instruments_file = Path(instruments_file)
+
+        if not instruments_file.exists():
+            raise FileNotFoundError(f"{instruments_file} 不存在。")
+        if instruments_file.suffix in {".csv"}:
+            registrations = pl.read_csv(instruments_file)
+        elif instruments_file.suffix in {".parquet"}:
+            registrations = pl.read_parquet(instruments_file)
+        else:
+            raise ValueError(f"{instruments_file} 文件格式不支持。")
+
+        return VXInstruments(name, registrations)
 
-    def dump(self, instruments_parquet: Union[str, Path]) -> None:
+    def dump(
+        self,
+        instruments_file: Union[str, Path],
+        *,
+        file_suffix: Literal["csv", "parquet"] = "csv",
+    ) -> "VXInstruments":
         """保存相关信息"""
-        if Path(instruments_parquet).is_dir():
-            instruments_parquet = Path(instruments_parquet, f"{self._name}.parquet")
+        if isinstance(instruments_file, str):
+            instruments_file = Path(instruments_file)
+
+        if Path(instruments_file).is_dir():
+            instruments_file = Path(instruments_file, f"{self._name}.{file_suffix}")
 
-        self._registrations.write_parquet(instruments_parquet)
-        logger.info(f"股票池:{self._name} 保存{instruments_parquet.as_posix()} 完成。")
+        if file_suffix == "csv":
+            self._registrations.write_csv(instruments_file)
+            logging.info(f"股票池:{self._name} 保存{instruments_file} 完成。")
+        elif file_suffix == "parquet":
+            self._registrations.write_parquet(instruments_file)
+            logging.info(f"股票池:{self._name} 保存{instruments_file} 完成。")
+        else:
+            raise ValueError(f"{file_suffix} 文件格式不支持。")
         return self
 
-    def rebuild(self) -> "vxInstruments":
+    def rebuild(self) -> "VXInstruments":
         """重建登记表"""
 
         new_registrations = []
         temp_registrations = {}
 
         for rows in self._registrations.sort(by=["symbol", "start_date"]).iter_rows(
             named=True
@@ -235,74 +214,72 @@
 
             elif (temp_registrations[symbol]["end_date"]) < rows["start_date"]:
                 new_registrations.append(temp_registrations[symbol])
                 temp_registrations[symbol] = rows
 
         new_registrations.extend(temp_registrations.values())
         self._registrations = pl.DataFrame(new_registrations)
-        self._last_updated_dt = (
-            to_datetime(vxtime.today())
-            if self._registrations.height == 0
-            else self._registrations["end_date"].max()
-        )
+
         return self
 
-    def all_instruments(self) -> List[InstrumentType]:
-        return self._registrations["symbol"].to_list()
+    def all_instruments(self) -> List[str]:
+        return self._registrations["symbol"].unique().to_list()
 
-    def union(self, *others: "vxInstruments") -> "vxInstruments":
+    def union(self, *others: "VXInstruments") -> "VXInstruments":
         """合并另外一个股票池"""
         if len(others) == 1 and isinstance(others[0], (list, tuple)):
             others = others[0]
+
         registrations = [self._registrations] + [
             other._registrations for other in others
         ]
         self._registrations = pl.concat(registrations)
         self.rebuild()
         return self
 
-    def intersect(self, other: "vxInstruments") -> "vxInstruments":
+    def intersect(self, other: "VXInstruments") -> "VXInstruments":
         """交集"""
 
-        new_registrations = []
+        new_registrations: List[Dict[str, Any]] = []
         for rows in self.registrations.sort(["symbol", "start_date"]).iter_rows(
             named=True
         ):
             new_registrations.extend(
                 {
                     "symbol": rows["symbol"],
                     "start_date": max(rows["start_date"], other_rows["start_date"]),
                     "end_date": min(rows["end_date"], other_rows["end_date"]),
-                    "weight": rows["weight"],
+                    # "weight": rows["weight"],
                 }
                 for other_rows in other.registrations.filter(
                     (pl.col("start_date") < rows["end_date"])
                     & (pl.col("end_date") > rows["start_date"])
                     & (pl.col("symbol") == rows["symbol"])
                 ).iter_rows(named=True)
             )
 
         self._registrations = (
             pl.DataFrame(new_registrations)
             if new_registrations
             else pl.DataFrame(
+                # {"symbol": [], "start_date": [], "end_date": [], "weight": []},
                 {"symbol": [], "start_date": [], "end_date": [], "weight": []},
                 schema={
                     "symbol": pl.Utf8,
                     "start_date": pl.Datetime,
                     "end_date": pl.Datetime,
-                    "weight": pl.Float64,
+                    # "weight": pl.Float64,
                 },
             )
         )
 
         self.rebuild()
         return self
 
-    def difference(self, other: "vxInstruments") -> "vxInstruments":
+    def difference(self, other: "VXInstruments") -> "VXInstruments":
         """差集"""
         new_registrations = []
         for rows in self.registrations.sort(["symbol", "start_date"]).iter_rows(
             named=True
         ):
             for other_rows in (
                 other.registrations.filter(
@@ -316,15 +293,15 @@
                 if rows["start_date"] < other_rows["start_date"]:
                     new_registrations.append(
                         {
                             "symbol": rows["symbol"],
                             "start_date": rows["start_date"],
                             "end_date": other_rows["start_date"]
                             - datetime.timedelta(days=1),
-                            "weight": rows["weight"],
+                            # "weight": rows["weight"],
                         }
                     )
 
                 rows["start_date"] = other_rows["end_date"] + datetime.timedelta(days=1)
 
                 if rows["start_date"] > rows["end_date"]:
                     break
@@ -334,31 +311,39 @@
 
         self._registrations = pl.DataFrame(new_registrations)
         self.rebuild()
         return self
 
 
 if __name__ == "__main__":
-    a = vxInstruments("test")
+    a = VXInstruments("test")
+    print(a.registrations)
     a.add_instrument("SHSE.600000", "2022-01-01", "2022-02-28")
     a.add_instrument("SHSE.600000", "2022-03-6", "2022-04-30")
-    # a.add_instrument("SHSE.600000", "2022-02-01", "2022-03-05")
-    # a.add_instrument("SHSE.600001", "2022-01-01", "2022-02-28")
-    # a.add_instrument("SHSE.600001", "2022-03-12", "2022-04-30")
-    # print(a.registrations)
-    b = vxInstruments("b")
+    a.add_instrument("SHSE.600000", "2022-02-01", "2022-03-05")
+    a.add_instrument("SHSE.600001", "2022-01-01", "2022-02-28")
+    a.add_instrument("SHSE.600001", "2022-03-12", "2022-04-30")
+    a.update_components(
+        ["SHSE.600000", "SHSE.600001", "SHSE.600002"],
+        start_date="2022-05-01",
+        end_date="2023-05-01",
+    )
+    print(a.registrations)
+    a.rebuild()
+    print(a.registrations)
+    print("=" * 60)
+    b = VXInstruments("b")
 
     b.add_instrument("SHSE.600000", "2022-02-14", "2022-03-12")
     b.add_instrument("SHSE.600000", "2021-01-01", "2022-01-12")
 
     print("-" * 60)
     print(b.registrations)
     print("-" * 60)
 
     # print(b.registrations)
     # with vxtime.timeit(1):
     #    a.union(b)
     # print(a.registrations)
-    with vxtime.timeit():
-        a.difference(b)
-        # a.union(b)
+    a.difference(b)
+    # a.union(b)
     print(a.registrations)
```

### Comparing `vxquant-20231018/PKG-INFO` & `vxquant-20240414/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: vxquant
-Version: 20231018
-Summary: python 量化常用工具箱
-Home-page: https://gitee.com/vxquant/vxqtools
+Version: 20240414
+Summary: 一个简单、易用、面向中国股市实盘的python量化交易框架
+Home-page: https://gitee.com/vxquant/vxquant
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: gmtrade
-Requires-Dist: httpx
-Requires-Dist: paho-mqtt
-Requires-Dist: pandas
-Requires-Dist: pytdx
+Requires-Dist: polars
 Requires-Dist: tqdm
 Requires-Dist: vxutils
 Description-Content-Type: text/markdown
 
 # vxquant
```

