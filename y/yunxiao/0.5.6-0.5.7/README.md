# Comparing `tmp/yunxiao-0.5.6.tar.gz` & `tmp/yunxiao-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.6.tar", last modified: Tue Apr 30 13:09:49 2024, max compression
+gzip compressed data, was "yunxiao-0.5.7.tar", last modified: Tue Apr 30 16:12:00 2024, max compression
```

## Comparing `yunxiao-0.5.6.tar` & `yunxiao-0.5.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.462233 yunxiao-0.5.6/
--rw-rw-rw-   0        0        0      509 2024-04-30 13:09:49.461234 yunxiao-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.6/README.md
--rw-rw-rw-   0        0        0     2374 2024-04-30 13:09:27.000000 yunxiao-0.5.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 13:09:49.462233 yunxiao-0.5.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.444706 yunxiao-0.5.6/yunxiao/
--rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.6/yunxiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.459233 yunxiao-0.5.6/yunxiao/schemas/
--rw-rw-rw-   0        0        0      262 2024-04-30 12:13:09.000000 yunxiao-0.5.6/yunxiao/schemas/__init__.py
--rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.6/yunxiao/schemas/achievements.py
--rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.6/yunxiao/schemas/page.py
--rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.6/yunxiao/schemas/teachers.py
--rw-rw-rw-   0        0        0    34806 2024-04-30 13:09:27.000000 yunxiao-0.5.6/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.460234 yunxiao-0.5.6/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.957183 yunxiao-0.5.7/
+-rw-rw-rw-   0        0        0      509 2024-04-30 16:12:00.956184 yunxiao-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.7/README.md
+-rw-rw-rw-   0        0        0     2443 2024-04-30 16:11:30.000000 yunxiao-0.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:12:00.957183 yunxiao-0.5.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.926605 yunxiao-0.5.7/yunxiao/
+-rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.7/yunxiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.955184 yunxiao-0.5.7/yunxiao/schemas/
+-rw-rw-rw-   0        0        0      403 2024-04-30 15:15:40.000000 yunxiao-0.5.7/yunxiao/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.7/yunxiao/schemas/achievements.py
+-rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.7/yunxiao/schemas/page.py
+-rw-rw-rw-   0        0        0     4157 2024-04-30 15:41:58.000000 yunxiao-0.5.7/yunxiao/schemas/payments.py
+-rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.7/yunxiao/schemas/teachers.py
+-rw-rw-rw-   0        0        0    33659 2024-04-30 16:11:30.000000 yunxiao-0.5.7/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.956184 yunxiao-0.5.7/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.6/pyproject.toml` & `yunxiao-0.5.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.6"
+version = "0.5.7"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.5.7" = "新增: 对 payments 引入 pydantic 做数据验证。"
 "0.5.6" = "新增: 对 achievements 引入 pydantic 做数据验证。"
 "0.5.5" = "新增: 对 teacher 引入 pydantic 做数据验证。"
 "0.5.4" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.3" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.1" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.5.0" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
```

### Comparing `yunxiao-0.5.6/yunxiao/schemas/achievements.py` & `yunxiao-0.5.7/yunxiao/schemas/achievements.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.6/yunxiao/schemas/teachers.py` & `yunxiao-0.5.7/yunxiao/schemas/teachers.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.6/yunxiao/yunxiao.py` & `yunxiao-0.5.7/yunxiao/yunxiao.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,29 +109,31 @@
 
             return wrapper
 
         return wrapper_func
 
     def _loop_pages(self, endpoint, payload, schemas):
         response = schemas()  # 结果列表
+        response.page.pageSize = payload.page.pageSize
         while payload.page.pageNum <= response.page.totalPage:
             res = self.request(method="post", url=endpoint, json=payload.model_dump())
             try:
                 new = schemas(**res)
-                # print(new)
                 response.data.extend(new.data)
-                response.page.totalPage = new.page.totalPage
-                response.page.totalCount = new.page.totalCount
+                response.page = new.page
 
-                logging.debug(f"size: {payload.page.pageSize}, page: {payload.page.pageNum}/{response.page.totalPage}, "
-                              f"{payload.page.pageNum * payload.page.pageSize}/{response.page.totalCount}")  # 汇报数量
+                logging.info(f"SIZE-{payload.page.pageSize} "
+                             f"PAGE-{response.page.pageNum}/{response.page.totalPage} "
+                             f"COUNT-{response.page.pageNum * payload.page.pageSize}/{response.page.totalCount} "
+                             f"FROM-{endpoint}")  # 汇报数量
 
                 payload.page.pageNum += 1  # 翻页
             except TypeError:
                 logging.error(res)
+        response.page.pageSize = payload.page.pageSize
         return response
 
     # 查询机构指定日期范围业绩。
     def company_query_performance(self, startdate: str, enddate: str) -> list:
         """
         查询机构指定日期范围业绩。
         :param startdate: 起始日期
@@ -763,52 +765,14 @@
                 "cardName": "",
                 "refundMethodList": [],
                 "confirmStatusList": [],
                 "phone": ""
             }
         )
 
-    # 查询收支明细-收入
-    @loop_pages("paymentDetailDtos")
-    def payments_query(self, page, size, startdate: str = "", enddate: str = "", revenue_type: int = "",
-                       order_status: int = ""):
-        """
-        查询指定操作日期范围的所有收入
-        :param order_status: 订单状态： **1** 已付款 **4** 已作废
-        :param revenue_type: 收入类型： **0** 收费 **1** 转课
-        :param size: 分页查询，每页数量
-        :param page: 分页查询，起始页码，应设为 0
-        :param enddate: YY-MM-DD
-        :param startdate: YY-MM-DD
-        :return:
-        """
-        return self.request(
-            method="post",
-            url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentList",
-            json={
-                "_t_": timestamp(),
-                "page": {"pageNum": page, "pageSize": size},
-                "campusIds": self.campus,
-                "payStartTime": startdate,
-                "payEndTime": enddate,
-                "revenueType": revenue_type,
-                "payType": "",
-                "groupNo": "",
-                "btransactionId": "",
-                "cardName": "",
-                "orderNo": "",
-                "orderStatus": order_status,
-                "orderStartTime": "",
-                "orderEndTime": "",
-                "paymentAccountCustomIds": [],
-                "confirmStatusList": [],
-                "phone": ""
-            }
-        )
-
     # 查询收支明细-账户明细
     @loop_pages()
     def payments_account_record(self, page, size, startdate: str = "", enddate: str = "", displayInvalidOrder=False,
                                 typeList: tuple = (), paymentAccountCustomIds: tuple = ()):
         return self.request(
             method="post",
             url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentAccountCustomRecord",
@@ -858,14 +822,23 @@
         """
         查询业绩。
         """
         return self._loop_pages(
             f"https://{self.host}/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
             payload, Achievements)
 
+    # 查询收入明细
+    def payments_query(self, payload: PaymentsQueryPayload) -> Payments:
+        """
+        查询业绩。
+        """
+        return self._loop_pages(
+            f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentList",
+            payload, Payments)
+
     # 查询招生来源
     def comefroms_query(self):
         return self.request(
             method="get",
             url=f"https://{self.host}/api/cs-crm/customField/get",
             params={"_t_": timestamp(), "customFieldId": "26118419"}
         )["data"]["selectItemList"]
```

