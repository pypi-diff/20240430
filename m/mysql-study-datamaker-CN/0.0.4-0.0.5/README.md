# Comparing `tmp/mysql_study_datamaker_cn-0.0.4.tar.gz` & `tmp/mysql_study_datamaker_cn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_study_datamaker_cn-0.0.4.tar", last modified: Mon Apr 29 14:52:08 2024, max compression
+gzip compressed data, was "mysql_study_datamaker_cn-0.0.5.tar", last modified: Tue Apr 30 06:19:57 2024, max compression
```

## Comparing `mysql_study_datamaker_cn-0.0.4.tar` & `mysql_study_datamaker_cn-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:52:08.134266 mysql_study_datamaker_cn-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      805 2024-04-29 14:52:08.131026 mysql_study_datamaker_cn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-28 08:17:36.000000 mysql_study_datamaker_cn-0.0.4/README.md
--rw-rw-rw-   0        0        0      407 2024-04-29 14:51:42.000000 mysql_study_datamaker_cn-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 14:52:08.134266 mysql_study_datamaker_cn-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 14:52:08.065549 mysql_study_datamaker_cn-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:52:08.096712 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/
--rw-rw-rw-   0        0        0        0 2024-04-28 08:03:22.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/__init__.py
--rw-rw-rw-   0        0        0     9536 2024-04-29 14:32:20.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/datamaker.py
--rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/new_family.txt
--rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/new_names.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 14:52:08.128750 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN.egg-info/
--rw-rw-rw-   0        0        0      805 2024-04-29 14:52:08.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-04-29 14:52:08.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:52:08.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-29 14:52:08.000000 mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.794355 mysql_study_datamaker_cn-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      912 2024-04-30 06:19:57.791611 mysql_study_datamaker_cn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.5/README.md
+-rw-rw-rw-   0        0        0      407 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:19:57.794355 mysql_study_datamaker_cn-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.758290 mysql_study_datamaker_cn-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.774902 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/
+-rw-rw-rw-   0        0        0      112 2024-04-30 06:19:49.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/__init__.py
+-rw-rw-rw-   0        0        0     9784 2024-04-30 06:14:50.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/datamaker.py
+-rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_family.txt
+-rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_names.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.789129 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/
+-rw-rw-rw-   0        0        0      912 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/top_level.txt
```

### Comparing `mysql_study_datamaker_cn-0.0.4/LICENSE` & `mysql_study_datamaker_cn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/datamaker.py` & `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/datamaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         gender：
             int：默认是数字类型，0 和 1 代表不同性别，没有严格的去区分哪个数字代表男和女；
             cn：中文的 男 女
             en：英文的 M F
             english：英文的 Male  Female
         a：考试分数的随机，最小值；
         b:考试分数的随机，最大值；
+        分数只要识别前两个字符是分数就可以，如果想创建多个分数的学生信息，可以写成：
+        ("姓名", "年龄", "性别",  "分数1", "分数2", "分数3")
         考试分数默认是 ； 0~150 分，则 a 就是 0， b：就是 150，做了判定修改，支持 b < a
         """
         self.__informations = {}
 
         self.__N = N
         self.__args = args
         self.__left = left
@@ -155,40 +157,40 @@
         if a > b:
             a, b = b, a
         return (str(r.randint(a, b)) for _ in range(self.__N))
 
     def get_info(self):
         infos = "姓名,年龄,部门,生日,性别,分数".split(",")
         for info in self.__args:
-            if info not in infos:
+            if info[:2] not in infos:
                 raise ValueError(f"All must be in {infos}, {info} not in.")
 
         for item in self.__args:
             if item == "姓名":
                 self.__informations[item] = self.get_name()
             elif item == "年龄":
                 self.__informations[item] = self.get_birthday_age(left=self.__left, right=self.__right, types="age")
             elif item == "部门":
                 self.__informations[item] = self.get_department(department=self.__department)
             elif item == "生日":
                 self.__informations[item] = self.get_birthday_age(self.__left, self.__right, types="birthday")
             elif item == "性别":
                 self.__informations[item] = self.get_gender(self.__gender)
-            elif item == "分数":
+            elif item[:2] == "分数":
                 self.__informations[item] = self.get_score(self.__a, self.__b)
 
     def __iter__(self):
         return self
 
     def __next__(self):
 
         result = ""
         for v in self.__informations.values():
             result += next(v) + ","
-
+        result = result[:-1]
         if not result:
             raise StopIteration
         return result
 
     @classmethod
     def create_insertinto(cls, self, file="_mysql_insert.txt"):
         """
@@ -208,10 +210,10 @@
 
 if __name__ == '__main__':
     """
     下面是案例，直接运行可以获得测试代码，生成15个随机数据；
     """
     now = datetime.now()
     file_name = f"{now.year}{now.month:>02}{now.day:>02} {now.hour:>02}.{now.minute:>02}.{now.second:>02}.txt"
-    one = DataMaker(15, ("姓名", "年龄", "性别", "生日", "部门"), gender="cn")
+    one = DataMaker(15, ("姓名", "年龄", "性别",  "分数1", "分数2", "分数3"), gender="cn")
     DataMaker.create_insertinto(one, file_name)
```

### Comparing `mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/new_family.txt` & `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_family.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.4/src/mysql_study_datamaker_CN/new_names.txt` & `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_names.txt`

 * *Files identical despite different names*

