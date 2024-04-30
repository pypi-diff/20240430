# Comparing `tmp/yunxiao-0.5.5.tar.gz` & `tmp/yunxiao-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.5.tar", last modified: Thu Apr 25 16:45:41 2024, max compression
+gzip compressed data, was "yunxiao-0.5.6.tar", last modified: Tue Apr 30 13:09:49 2024, max compression
```

## Comparing `yunxiao-0.5.5.tar` & `yunxiao-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:45:41.392689 yunxiao-0.5.5/
--rw-rw-rw-   0        0        0      509 2024-04-25 16:45:41.391689 yunxiao-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.5/README.md
--rw-rw-rw-   0        0        0     2301 2024-04-25 16:45:24.000000 yunxiao-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 16:45:41.392689 yunxiao-0.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 16:45:41.383101 yunxiao-0.5.5/yunxiao/
--rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.5/yunxiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:45:41.389690 yunxiao-0.5.5/yunxiao/schemas/
--rw-rw-rw-   0        0        0      124 2024-04-25 15:13:05.000000 yunxiao-0.5.5/yunxiao/schemas/__init__.py
--rw-rw-rw-   0        0        0     2607 2024-04-25 15:38:16.000000 yunxiao-0.5.5/yunxiao/schemas/teachers.py
--rw-rw-rw-   0        0        0    35843 2024-04-25 16:44:22.000000 yunxiao-0.5.5/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:45:41.390689 yunxiao-0.5.5/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-25 16:45:41.000000 yunxiao-0.5.5/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-04-25 16:45:41.000000 yunxiao-0.5.5/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:45:41.000000 yunxiao-0.5.5/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 16:45:41.000000 yunxiao-0.5.5/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 16:45:41.000000 yunxiao-0.5.5/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.462233 yunxiao-0.5.6/
+-rw-rw-rw-   0        0        0      509 2024-04-30 13:09:49.461234 yunxiao-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.6/README.md
+-rw-rw-rw-   0        0        0     2374 2024-04-30 13:09:27.000000 yunxiao-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:09:49.462233 yunxiao-0.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.444706 yunxiao-0.5.6/yunxiao/
+-rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.6/yunxiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.459233 yunxiao-0.5.6/yunxiao/schemas/
+-rw-rw-rw-   0        0        0      262 2024-04-30 12:13:09.000000 yunxiao-0.5.6/yunxiao/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.6/yunxiao/schemas/achievements.py
+-rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.6/yunxiao/schemas/page.py
+-rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.6/yunxiao/schemas/teachers.py
+-rw-rw-rw-   0        0        0    34806 2024-04-30 13:09:27.000000 yunxiao-0.5.6/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:09:49.460234 yunxiao-0.5.6/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 13:09:49.000000 yunxiao-0.5.6/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.5/pyproject.toml` & `yunxiao-0.5.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.5"
+version = "0.5.6"
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
+"0.5.6" = "新增: 对 achievements 引入 pydantic 做数据验证。"
 "0.5.5" = "新增: 对 teacher 引入 pydantic 做数据验证。"
 "0.5.4" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.3" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.1" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.5.0" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.4.9" = "新增: '账户明细'端点;\n改进: 尝试将会话重用"
```

### Comparing `yunxiao-0.5.5/yunxiao/schemas/teachers.py` & `yunxiao-0.5.6/yunxiao/schemas/teachers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 
 from pydantic import BaseModel, field_validator
 from typing import List, Optional
+from .page import Page
 
 
 class _CampusDto(BaseModel):
     id: int
     companyId: int
     teacherId: int
     campusId: int
@@ -70,26 +71,14 @@
     activated: bool
 
     @field_validator('name')
     def name(cls, v: str):
         return v.replace("\u200b", "")
 
 
-class Page(BaseModel):
-    """
-    Attributes:
-        pageNum: 页码.
-        pageSize: 每页数量.
-    """
-    pageNum: int = 1
-    pageSize: Optional[int] = 100
-    totalCount: Optional[int] = 1
-    totalPage: Optional[int] = 1
-
-
 class Teschers(BaseModel):
     data: List[Teacher] = []
     currentTimeMillis: int = 0
     code: int = 200
     msg: str = ""
     page: Page = Page()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yunxiao-0.5.5/yunxiao/yunxiao.py` & `yunxiao-0.5.6/yunxiao/yunxiao.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,20 +107,21 @@
                     page += 1  # 翻页
                 return data_list
 
             return wrapper
 
         return wrapper_func
 
-    def _loop_pages(self, endpoint, payload: [TeschersQueryPayload], schemas: [Teschers]) -> Teschers:
+    def _loop_pages(self, endpoint, payload, schemas):
         response = schemas()  # 结果列表
         while payload.page.pageNum <= response.page.totalPage:
             res = self.request(method="post", url=endpoint, json=payload.model_dump())
             try:
                 new = schemas(**res)
+                # print(new)
                 response.data.extend(new.data)
                 response.page.totalPage = new.page.totalPage
                 response.page.totalCount = new.page.totalCount
 
                 logging.debug(f"size: {payload.page.pageSize}, page: {payload.page.pageNum}/{response.page.totalPage}, "
                               f"{payload.page.pageNum * payload.page.pageSize}/{response.page.totalCount}")  # 汇报数量
 
@@ -849,46 +850,21 @@
             params={
                 "orderInfoId": orderinfo_id,
                 "_t_": timestamp()
             }
         )["data"]
 
     # 查询签单业绩
-    @loop_pages("achievementBelongerDetailItems")
-    def payments_query_achievements_datarange(self, page, size, startdate: str = "", enddate: str = "",
-                                              teacher_ids: tuple = (), order_types: tuple = ()):
+    def achievements_query(self, payload: AchievementsQueryPayload) -> Achievements:
         """
-        查询业绩归属，根据日期
-        :param order_types: **0** 收费 **1** 转课 **2** 退费 **3** 结转
-        :param teacher_ids:
-        :param size: 分页查询，每页数量
-        :param page: 分页查询，起始页码
-        :param enddate: YY-MM-DD
-        :param startdate: YY-MM-DD
-        :return:
+        查询业绩。
         """
-
-        return self.request(
-            method="post",
-            url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
-            json={
-                "_t_": timestamp(),
-                "page": {"pageNum": page, "pageSize": size},
-                "campusIds": self.campus,
-                "startDate": startdate,
-                "endDate": enddate,
-                "orderFlagIds": [],
-                "orderTypes": list(order_types),
-                "productTypes": [],
-                "orderNo": "",
-                "productName": "",
-                "studentId": "",
-                "teacherIds": list(teacher_ids)
-            }
-        )
+        return self._loop_pages(
+            f"https://{self.host}/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
+            payload, Achievements)
 
     # 查询招生来源
     def comefroms_query(self):
         return self.request(
             method="get",
             url=f"https://{self.host}/api/cs-crm/customField/get",
             params={"_t_": timestamp(), "customFieldId": "26118419"}
```

