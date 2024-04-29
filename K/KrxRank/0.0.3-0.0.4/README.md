# Comparing `tmp/krxrank-0.0.3.tar.gz` & `tmp/krxrank-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krxrank-0.0.3.tar", last modified: Mon Apr 29 22:03:31 2024, max compression
+gzip compressed data, was "krxrank-0.0.4.tar", last modified: Mon Apr 29 22:18:54 2024, max compression
```

## Comparing `krxrank-0.0.3.tar` & `krxrank-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.052602 krxrank-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-29 19:37:30.000000 krxrank-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1673 2024-04-29 22:03:31.051602 krxrank-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-04-29 20:42:29.000000 krxrank-0.0.3/README.md
--rw-rw-rw-   0        0        0      479 2024-04-29 22:02:20.000000 krxrank-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 22:03:31.052602 krxrank-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.019572 krxrank-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.026579 krxrank-0.0.3/src/KrxRank/
--rw-rw-rw-   0        0        0       21 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/__init__.py
--rw-rw-rw-   0        0        0     3119 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/etc.py
--rw-rw-rw-   0        0        0    22537 2024-04-29 19:48:12.000000 krxrank-0.0.3/src/KrxRank/rank.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:03:31.049599 krxrank-0.0.3/src/KrxRank.egg-info/
--rw-rw-rw-   0        0        0     1673 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 22:03:31.000000 krxrank-0.0.3/src/KrxRank.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 22:18:54.699892 krxrank-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 19:37:30.000000 krxrank-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1673 2024-04-29 22:18:54.698891 krxrank-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-04-29 20:42:29.000000 krxrank-0.0.4/README.md
+-rw-rw-rw-   0        0        0      479 2024-04-29 22:18:47.000000 krxrank-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:18:54.699892 krxrank-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 22:18:54.667291 krxrank-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:18:54.674111 krxrank-0.0.4/src/KrxRank/
+-rw-rw-rw-   0        0        0       21 2024-04-29 19:48:12.000000 krxrank-0.0.4/src/KrxRank/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 22:18:17.000000 krxrank-0.0.4/src/KrxRank/etc.py
+-rw-rw-rw-   0        0        0    25641 2024-04-29 22:18:17.000000 krxrank-0.0.4/src/KrxRank/rank.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:18:54.696890 krxrank-0.0.4/src/KrxRank.egg-info/
+-rw-rw-rw-   0        0        0     1673 2024-04-29 22:18:54.000000 krxrank-0.0.4/src/KrxRank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-29 22:18:54.000000 krxrank-0.0.4/src/KrxRank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:18:54.000000 krxrank-0.0.4/src/KrxRank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 22:18:54.000000 krxrank-0.0.4/src/KrxRank.egg-info/top_level.txt
```

### Comparing `krxrank-0.0.3/LICENSE` & `krxrank-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.3/PKG-INFO` & `krxrank-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KrxRank
-Version: 0.0.3
+Version: 0.0.4
 Summary: KRX 정보데이터시스템 순위 통계 데이터 얻어오기
 Author-email: FinPro <finpro1224@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `krxrank-0.0.3/README.md` & `krxrank-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `krxrank-0.0.3/src/KrxRank/rank.py` & `krxrank-0.0.4/src/KrxRank/rank.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import json
 import pandas as pd
-from etc import *
 
 def price_fluctuation_high(start_date, end_date, market="ALL"):
     df_list = []
     for mk in mktId(market):
         data = [('bld', 'dbms/MDC/EASY/ranking/MDCEASY01501'),
                 ('locale', 'ko_KR'),
                 ('mktId', str(mk)),
@@ -469,8 +468,85 @@
             ('itmTpCd', '2'),
             ('trdDd', str(date))]
     df_list.append(json.loads(requests.post(BASE_URL, headers=headers, data=data).text)['OutBlock_1'])
     col = ['종목코드', '종목명', '종', '등락률', '추정NAV', '거래량', '거래대금']
     df = make_dl(list_cb(df_list), col)
     df.sort(key=lambda x: float(x[4]), reverse=False)
     df = pd.DataFrame(df[:50], columns=col, index=[i for i in range(1, 51, 1)])
-    return df
+    return df
+
+# a 대비 b의 등락률을 소수점 3자리 float type으로 반환
+# 주가를 대상으로 하기에 0이 입력되면 작동 X
+def sp(a, b):
+    if a != 0 and b != 0:
+        return round((b - a) / a * 100, 3)
+
+# 가격의 콤마(,)를 제거 하고 정수형으로 반환해주는 함수
+# 변수의 type도 str에서 int로 변환
+# ex) 20,000 -> 20000
+def del_comma(n):
+    if ',' in list(n):
+        n = ''.join(n.split(','))
+        if '.' in n:
+            return float(n)
+        else:
+            return int(n)
+    else :
+
+        return n
+
+# market 입력 값을 스크래핑 활용 인수로 변경
+def mktId(market) :
+    if market == 'KOSPI':
+        market = ['STK']
+    elif market == 'KOSDAQ':
+        market = ['KSQ']
+    elif market == 'ALL':
+        market = ['STK', 'KSQ']
+    else :
+        market = []
+    return market
+
+# ex) [[1, 2, 3], [4, 5, 6]] -> [1, 2, 3, 4, 5, 6]
+def list_cb(l):
+    cb_list = []
+    for i in l:
+       for j in i:
+           cb_list.append(j)
+    return cb_list
+
+def make_dl(l, col):
+    data_list = []
+    # 여기서의 시가는 시작일 기준가, 종가는 종료일 기준가
+    d = {'종목코드': 'ISU_CD', '종목명': 'ISU_ABBRV', '시장구분': 'MKT_NM', '시가': 'BAS_PRC', '종가': 'CLSPRC',
+         '등락률': 'FLUC_RT', '거래량': 'ACC_TRDVOL', '거래대금': 'ACC_TRDVAL', '시가총액': 'MKTCAP', '회전율': 'TURNOVER_RT',
+         '시가총액비중': 'MKTCAP_WT', '상장주식수': 'LIST_SHRS', '환산주가': 'CONV_AMT', '액면가': 'PARVAL',
+         '외국인보유수량': 'HD_QTY', '외국인지분율': 'HD_RTO', '외국인한도수량': 'FORN_ORD_LMT_QTY', '외국인한도소진율': 'ITM_RTO',
+         '시': 'TDD_OPNPRC', '고': 'TDD_HGPRC', '저': 'TDD_LWPRC', '종': 'TDD_CLSPRC', '추정NAV': 'NUM_ITM_VAL1'
+         }
+    for i in l :
+        c = []
+        for j in range(len(col)):
+            if col[j] == '종목명':
+                if len(i[d[col[j]]]) <= 17:
+                    c.append(i[d[col[j]]])
+                else :
+                    c.append(i[d[col[j]]][:15]+'..')
+            elif col[j] == '시장구분':
+                c.append(i[d[col[j]]][:6])
+            else :
+                c.append(del_comma(i[d[col[j]]]))
+        data_list.append(c)
+    return data_list
+
+headers = {'Accept': 'application/json, text/javascript, */*; q=0.01',
+           'Accept-Encoding':'gzip, deflate',
+           'Accept-Language': 'ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7',
+           'Connection': 'keep-alive',
+           'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+           'Host': 'data.krx.co.kr', 'Origin': 'http://data.krx.co.kr',
+           'Referer': 'http://data.krx.co.kr/contents/MDC/MDI/mdiLoader/index.cmd?menuId=MDC0301',
+           'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 '
+                         '(KHTML, like Gecko) Chrome/124.0.0.0',
+           'X-Requested-With': 'XMLHttpRequest'}
+
+BASE_URL = 'http://data.krx.co.kr/comm/bldAttendant/getJsonData.cmd'
```

### Comparing `krxrank-0.0.3/src/KrxRank.egg-info/PKG-INFO` & `krxrank-0.0.4/src/KrxRank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KrxRank
-Version: 0.0.3
+Version: 0.0.4
 Summary: KRX 정보데이터시스템 순위 통계 데이터 얻어오기
 Author-email: FinPro <finpro1224@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

