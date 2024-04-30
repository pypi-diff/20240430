# Comparing `tmp/txdpy-7.6.7.tar.gz` & `tmp/txdpy-7.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-i6__erk5\txdpy-7.6.7.tar", last modified: Wed Apr  3 08:59:06 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-hgmkh_o3\txdpy-7.6.8.tar", last modified: Tue Apr 30 09:31:44 2024, max compression
```

## Comparing `txdpy-7.6.7.tar` & `txdpy-7.6.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:59:06.000000 txdpy-7.6.7/
--rw-rw-rw-   0        0        0       71 2024-04-03 08:59:06.000000 txdpy-7.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-03 08:59:06.000000 txdpy-7.6.7/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-04-03 08:58:46.000000 txdpy-7.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2781 2024-03-25 09:27:18.000000 txdpy-7.6.7/txdpy/__init__.py
--rw-rw-rw-   0        0        0    27547 2024-03-28 06:02:54.000000 txdpy-7.6.7/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3854 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     3247 2024-04-02 13:47:33.000000 txdpy-7.6.7/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.7/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11803 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3002 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/str_category.py
--rw-rw-rw-   0        0        0     1044 2024-04-03 08:58:18.000000 txdpy-7.6.7/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.7/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-03 08:59:06.000000 txdpy-7.6.7/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/
+-rw-rw-rw-   0        0        0       71 2024-04-30 09:31:44.000000 txdpy-7.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:31:44.000000 txdpy-7.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-30 09:29:46.000000 txdpy-7.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2851 2024-04-29 03:32:28.000000 txdpy-7.6.8/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    28068 2024-04-30 09:29:05.000000 txdpy-7.6.8/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.6.8/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     3247 2024-04-03 01:19:42.000000 txdpy-7.6.8/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.6.8/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.8/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.6.8/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.6.8/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/str_category.py
+-rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.6.8/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/translate.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.6.7/txdpy/URLjoin.py` & `txdpy-7.6.8/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/__init__.py` & `txdpy-7.6.8/txdpy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __all__ = ['urljoin', 'headers_dict', 'PyMySQL', 'rl', 'si', 'liduel', 'param_dict',
            'is_num', 'is_Sletter', 'is_Bletter', 'is_letter', 'is_num_letter', 'is_chinese',
            'get_chinese', 'get_letter', 'get_Bletter', 'get_Sletter', 'get_Sletter', 'get_num', 'get_middle',
            'get_num_letter', 'webptablesl', 'req', 'dow_file', 'list_dupl', 'selenium_firefox', 'get_ssq','is_ssq',
            'excel_into_mysql', 'prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdmin',
            'txdperc', 'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'prvadepl', 'read_excel',
            'ExtractEnrollmentLabels', 'sortedlbys', 'UpdateName', 'optstr','progbar','text_similar'
-           'Recognit_Data_Process','gen_excel','translate','ReadData','get_ms_name','get_code_name','unify_keys'
+           'Recognit_Data_Process','gen_excel','translate','ReadData','get_major_name','GetSchoolName',
+           'get_code_name','unify_keys'
            # 'PyBloomFilter'
            ]
 
 from .URLjoin import urljoin
 from .requests_operation import headers_dict
 from .requests_operation import param_dict
 from .requests_operation import webptablesl
@@ -51,15 +52,16 @@
 from .bk_179 import exenla
 from .bk_179 import getexcelth
 from .bk_179 import prvadepl
 from .bk_179 import ExtractEnrollmentLabels
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
 from .bk_179 import optstr
-from .bk_179 import get_ms_name
+from .bk_179 import get_major_name
+from .bk_179 import GetSchoolName
 from .bk_179 import get_code_name
 from .bk_179 import unify_keys
 from .excel_easy import read_excel
 from .excel_easy import gen_excel
 from .translate import translate
 from .read_data import ReadData
 from .progress_display import progbar
```

### Comparing `txdpy-7.6.7/txdpy/bk_179.py` & `txdpy-7.6.8/txdpy/bk_179.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import sys,re,numpy,json,pymysql
 from loguru import logger
 from typing import Union
 from .read_data import ReadData
 from .pytmysql import PyMySQL
 from .str_category import is_num
+from .list_processing import list_dupl
 
 #老高考批次
 batch_dict1 = {'本科一批A': '本科一批', '专科': '专科', '本科一批A1': '本科一批', '本科一批B': '本科一批',
                  '本科二批A': '本科二批', '本科二批B': '本科二批', '本科二批C': '本科二批', '高本贯通批': '专科',
                  '本科提前A': '本科一批', '本科提前批A': '本科一批', '本科提前批B': '本科一批', '本科提前B': '本科一批',
                  '本科一批': '本科一批', '蒙授本科一批': '本科一批', '本科二批': '本科二批', '蒙授本科二批': '本科二批',
                  '专科提前': '专科', '专科提前批': '专科', '蒙授本科提前A': '本科一批', '蒙授本科提前批A': '本科一批',
@@ -60,15 +61,15 @@
                  '本科提前批精准扶贫专项（E段）': '特殊类型招生控制线', '本科提前批革命老区专项（F段）': '特殊类型招生控制线'}
 
 #返回省市区名称和地区编号
 def prurar_code(gkle='all',ssq=None):
     gkle=gkle.strip('省份')
     prurar_code={"北京": 11, "天津": 12, "河北": 13, "山西": 14, "内蒙古": 15, "辽宁": 21, "吉林": 22, "黑龙江": 23,
            "上海": 31, "江苏": 32, "浙江": 33, "安徽": 34, "福建": 35, "江西": 36, "山东": 37, "河南": 41, "湖北": 42,
-           "湖南": 43, "广东": 44, "广西": 45, "海南": 46, "重庆": 50, "四川": 51, "贵州": 52, "云南": 53, "西藏": 54,
+           "湖南": 43, "广东": 44, "广西": 45, "海南": 46, "重庆": 50, "四川": 51, "贵州": 52, "云南": 53,
            "陕西": 61, "甘肃": 62, "青海": 63, "宁夏": 64, "新疆": 65}
     prurar_dict={x[0]: x[1] for x in ReadData('各省份高考分类').data[1:]}
     if ssq:
         return prurar_code[ssq]
     if gkle in ('专业类','专业组','新高考','老高考','综合'):
         return json.loads(prurar_dict.get(gkle))
     return prurar_code
@@ -90,22 +91,21 @@
     else:
         return '特殊类'
 
 #转换科类名称
 def convert_kl(kl):
     if '不限' in kl:
         return '综合'
-    elif 'li' in kl or '物理' in kl or '理' in kl:
+    if 'li' in kl or '物理' in kl or '理' in kl:
         return '理工'
-    elif 'wen' in kl or '历史' in kl or '文' in kl:
+    if 'wen' in kl or '历史' in kl or '文' in kl:
         return '文史'
-    elif 'all' in kl or '综合' in kl:
+    if 'all' in kl or '综合' in kl:
         return '综合'
-    else:
-        return kl
+    return kl
 
 #删除了数据中判断为Flase(判断0的返回值为Flase)的数据
 def delete_flase_empty(ls):
     nls=[]
     for l in ls:
         type_l=type(l)
         if type_l!=int and type_l!=float and l:
@@ -157,15 +157,15 @@
     if ls:
         return min(ls)
     else:
         return None
 
 #将数字转换为百分比，默认百分比中数字保留两位小数
 def txdperc(num,dp=2):
-    return f'{round(num * 100, dp)}%'
+    return f'{round(num * 100, dp)}%' if is_num(num) else None
 
 class QueryScoreRank:
     """
     查询分数位次，省份批次线
     """
     def __init__(self,year,simplify_pcname=True):
         """
@@ -245,17 +245,16 @@
             if isrrp:
                 return None,(None,None,None)
             return None
 
         frac_rank=self.rfrac_rank1(prurar, pc, kl, frac)
         if isrrp:
             batch_xian,batch_xian_rank=self.rbx_rank(prurar,pc,kl)
-            return frac_rank,(batch_xian,batch_xian_rank,txdperc(frac_rank/batch_xian_rank))
-        else:
-            return frac_rank
+            return frac_rank, (batch_xian,batch_xian_rank,txdperc(frac_rank/batch_xian_rank) if batch_xian_rank and frac_rank else None)
+        return frac_rank
 
     #返回批次线和批次线位次
     def rbx_rank(self,prurar,pc,kl,rbxr=True):
         """
         :param prurar:省市区
         :param pc:批次
         :param kl:科类
@@ -350,22 +349,22 @@
 def exenla(major,maispb=False,return_string=False):
     """
     :param major:专业名称
     :param maispb:是否查找匹配标签
     :param return_string:返回字符串
     :return: 专业名称中的标签
     """
-    bqs={'招生标签':list(set([v for v in
-              ['联合培养', '中外合作', '校企合作', '国家专项', '高职本科', '地方专项', '高校专项', '联合办学','精准扶贫','少数民族', '民族班', '少民', '闽台', '优师', '公费', '订单', '双语', '定向', '预科']
+    bqs={'招生标签':list(list_dupl([v for v in
+              ['国家专项', '地方专项', '帮扶专项', '预科', '联合培养', '中外合作', '校企合作', '高职本科', '高校专项', '联合办学','精准扶贫','少数民族', '民族班', '少民', '闽台', '优师', '公费', '订单', '双语', '定向']
                 if v in major and f'非{v}' not in major])),
-    '匹配标签': list(set([v for v in
+    '匹配标签': list(list_dupl([v for v in
                        ['师范','苏区专项']
                     if v in major and f'非{v}' not in major]))
      }
-    zhonhwaihezuo=re.search('中.合作',major)
+    zhonhwaihezuo=re.search('中[^心]合作',major)
     if zhonhwaihezuo and '中外合作' not in bqs['招生标签']:
         bqs['招生标签'].append('中外合作')
     if return_string:
         return '、'.join(bqs['招生标签'])
     return bqs if maispb else bqs['招生标签']
 
 #获取表头中字段名称索引，表头以列表形式传入
@@ -407,15 +406,15 @@
     def exmana(self,major,batch,school_name):
         """
         :param major:专业名称
         :param batch:批次
         :param school_name:学校名称，学校名称中有“职业”关键字优先在职业本科查找专业名称信息
         :return:专业名称、专业名称逻辑代码、二级大类、二级大类逻辑代码、一级大类、一级大类逻辑代码
         """
-        major_name = get_ms_name(major)[0]
+        major_name = get_major_name(major)[0]
         if '专科' in batch:
             return self.data.get('专科' + '_' + major_name, [None] * 6)
         else:
             major_name = '本科预科班' if '预科' in major_name else major_name
             mana = self.data.get('本科' + '_' + major_name)
             if mana:
                 return mana
@@ -436,15 +435,15 @@
 
 class UpdateName():
     """
     更新院校名称和专业名称
     """
     def __init__(self):
         with open('c:/mysql_config.json', 'r', encoding='utf-8') as f:
-            mysql_config = json.load(f)
+            mysql_config = json.load(f)['1']
         db = pymysql.connect(host=mysql_config['host'], port=3306, user='root', password=mysql_config['password'],
                                   database=mysql_config['database'])
         cursor = db.cursor()
         cursor.execute('select * from 更新院校名称名单')
         schools=cursor.fetchall()
         self.schools = sorted(list(schools), key=lambda x: len(x[0]), reverse=True)
         zk_majors, bk_majors = [], []
@@ -499,22 +498,34 @@
     elif type(values)==dict:
         for i,value in enumerate(values.values()):
             value=prvadepl(value)
             if type(value) == str:
                 values.values()[i] = format_str(value)
     return values
 
-def get_ms_name(s):
+def get_major_name(s):
     """
-    获取专业或院校名称
+    获取专业名称
     """
     name=re.search('([\u4e00-\u9fa5、]+)(.*)',optstr(s))
     if name:
         return name.groups(1)
 
+class GetSchoolName:
+    """
+    获取院校名称
+    """
+    def __init__(self):
+        self.schools=sorted([x[0] for x in ReadData('院校名称').data[1:]], key=lambda x: len(x), reverse=True)
+    def __call__(self,school):
+        school=optstr(school)
+        for school_name in self.schools:
+            if school.startswith(school_name):
+                return [school_name,school.replace(school_name,'',1)]
+
 def get_code_name(s):
     """
     提取院校代码和名称或专业代码和名称
     """
     code = re.search('(^[0-9A-Za-z]+)', optstr(s)).group(1)
     name = optstr(s.lstrip(code))
     return [code,name]
```

### Comparing `txdpy-7.6.7/txdpy/easyreq.py` & `txdpy-7.6.8/txdpy/easyreq.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def req(url:str,param=None,data=None,json=None,headers=None,verify:bool=False,zhencod=True,**kwargs):
     """
     :param url: 请求的url
     :param param: get请求参数默认为空
     :param data: post请求参数默认为空
     :param json: post请求参数默认为空
     :param headers: 默认随机User-Agent
-    :param verify: 是否认证证书，默认为true
+    :param verify: 是否认证证书，默认为False
     :param tree: 是否直接返回etree.HTML()对象，默认为False
     :return: 返回reponese对象
     """
     if headers:
         if type(headers) == str:
             h=headers_dict(headers)
         else:
```

### Comparing `txdpy-7.6.7/txdpy/excel_easy.py` & `txdpy-7.6.8/txdpy/excel_easy.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/get_key.py` & `txdpy-7.6.8/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/list_processing.py` & `txdpy-7.6.8/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/lookup.py` & `txdpy-7.6.8/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/progress_display.py` & `txdpy-7.6.8/txdpy/progress_display.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/pytmysql.py` & `txdpy-7.6.8/txdpy/pytmysql.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/read_data.py` & `txdpy-7.6.8/txdpy/read_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             table_name = extract_table_name(name)
             self.table_name = table_name
             table_name = self.table_dict.get(table_name, table_name)
             sql = re.sub(r'(?i)(FROM\s+)[^\s]+', r'\1' + f'`{table_name}`', name, 1)
             logger.info(sql)
             table_th = re.search('select\s(.+?)\sfrom', name, re.IGNORECASE).group(1)
             if table_th == '*':
-                self.data.append(self.replace_th_name(self.get_th(table_name, self.table_dict)))
+                self.data.append(self.replace_th_name(self.get_th(table_name)))
             else:
                 self.data.append(
                     self.replace_th_name(table_th.replace('`', '').replace('"', '').replace("'", '').split(',')))
             self.data += [list(v) for v in self.select_mysql_data(sql)]
         else:
             self.table_name = name
             table_name = self.table_dict.get(name, name)
@@ -241,14 +241,17 @@
         workbook.close()
 
     def __str__(self):
         return '你很牛逼，你很棒！'
 
     def __del__(self):
         if self.db:
-            self.db.close()
-            self.cursor.close()
+            try:
+                self.db.close()
+                self.cursor.close()
+            except:
+                pass
 
 # 提取数据表名称
 extract_table_name = lambda sql: re.search('from\s([^\s]+)', sql, re.IGNORECASE).group(1).split('.')[-1].strip('`')
 # 判断是否为纯数字
 is_num = lambda s: type(s) == int or re.search('^([0-9]+)$', str(s))
```

### Comparing `txdpy-7.6.7/txdpy/requests_operation.py` & `txdpy-7.6.8/txdpy/requests_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     return result_dict
 
 def webptablesl(res,xpath,i=1):
     """
     :param res: url响应的html(例如response.text)
     :param xpath: 表格xpath(例如//table[1])
-    :param i: 多个表格索引
+    :param i: 多个表格索引，默认使用第一个xpath匹配到的表格
     :return: 拆分后的表格数据，以列表返回
     """
     tree=etree.HTML(res)
     tables = tree.xpath(xpath)
     if tables:
         table = tables[i-1]
     else:
```

### Comparing `txdpy-7.6.7/txdpy/selenium_Firefox.py` & `txdpy-7.6.8/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/str_category.py` & `txdpy-7.6.8/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.7/txdpy/text_similar.py` & `txdpy-7.6.8/txdpy/text_similar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests,json
 from time import sleep
 
 params = {"grant_type": "client_credentials", "client_id": "7eb6Ee3o8FLh9ce3ATX1MA1S",
               "client_secret": "O44grcUdKtKSXXAMTkgpoDamFeweeGy7"}
-
 access_token = str(
     requests.post("https://aip.baidubce.com/oauth/2.0/token", params=params).json().get("access_token"))
 
 def text_similar(text_1, text_2):
     i=0
     response,e=None,None
     while i<10:
```

### Comparing `txdpy-7.6.7/txdpy/translate.py` & `txdpy-7.6.8/txdpy/translate.py`

 * *Files identical despite different names*

