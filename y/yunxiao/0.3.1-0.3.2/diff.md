# Comparing `tmp/yunxiao-0.3.1.tar.gz` & `tmp/yunxiao-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.3.1.tar", last modified: Thu Jun 22 20:24:52 2023, max compression
+gzip compressed data, was "yunxiao-0.3.2.tar", last modified: Fri Jun 23 20:56:53 2023, max compression
```

## Comparing `yunxiao-0.3.1.tar` & `yunxiao-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:24:52.001823 yunxiao-0.3.1/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-06-22 20:24:52.000814 yunxiao-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.1/README.md
--rw-rw-rw-   0        0        0     1290 2023-06-22 20:24:32.000000 yunxiao-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 20:24:52.001823 yunxiao-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.991678 yunxiao-0.3.1/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.1/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.994731 yunxiao-0.3.1/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.1/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    34197 2023-06-22 20:24:23.000000 yunxiao-0.3.1/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.1/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:24:51.999806 yunxiao-0.3.1/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 20:24:51.000000 yunxiao-0.3.1/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.436468 yunxiao-0.3.2/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-06-23 20:56:53.435459 yunxiao-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1378 2023-06-23 20:56:27.000000 yunxiao-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:56:53.436468 yunxiao-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.411895 yunxiao-0.3.2/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.414926 yunxiao-0.3.2/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.2/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    40861 2023-06-23 20:55:47.000000 yunxiao-0.3.2/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.2/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:56:53.434452 yunxiao-0.3.2/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 20:56:53.000000 yunxiao-0.3.2/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.3.1/LICENSE` & `yunxiao-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.1/PKG-INFO` & `yunxiao-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.1
+Version: 0.3.2
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.3.1/README.md` & `yunxiao-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.1/pyproject.toml` & `yunxiao-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.3.1"
+version = "0.3.2"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,16 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.3.2" = "更新参数，修复BUG，新增意向管理API"
+"0.3.1" = "修复整合"
 "0.2.9" = "删除其他，只使用V2"
 "0.2.6" = "V2 中更多使用分片读取。"
 "0.2.5" = "修复 V2 中的 API端点错误。新增 loop 装饰器便于分片提取大量数据。"
 "0.2.4" = "修复 v2 中一个API端点错误及鉴权更新错误"
 "0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
 "0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
```

### Comparing `yunxiao-0.3.1/yunxiao/v2.py` & `yunxiao-0.3.2/yunxiao/v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -218,14 +218,88 @@
                 "reserve": 0,
                 "displayCompletedClass": False,
                 "courseStatusList": [],
                 "page": {"pageNum": 1, "pageSize": 999}
             }
         )["data"]
 
+    # 查询意向
+    @loop("")
+    def intentions_query(self, page, size, distributeStatus: int = 1, keyWord: str = "", level: int = "",
+                         nonFollowUpDays: int = "", startNextTime: str = "", endNextTime: str = "",
+                         startLastCommunicateTime: str = "", endLastCommunicateTime: str = ""):
+        """
+        查询意向
+        :param size: 分页查询，每页数量
+        :param page: 分页查询，初始页码，应设为 0
+        :param distributeStatus: 是否分配跟进人。 **0** 无跟进人 **1** 有跟进人
+        :param level: 意向级别。 1-5
+        :param keyWord: 查询关键字
+        :param nonFollowUpDays: 未跟进天数
+        :param startNextTime: 计划跟进时间（查询起点）
+        :param endNextTime: 计划跟进时间（查询终点）
+        :param startLastCommunicateTime: 最近跟进时间（查询起点）
+        :param endLastCommunicateTime: 最近跟进时间（查询终点）
+        :return:
+        """
+        return self.request(
+            method="post",
+            url="https://yunxiao.xiaogj.com/api/cs-crm/intention/clue/allPage",
+            json={
+                "_t_": UsedTime.stamp,
+                "distributeStatus": distributeStatus,
+                "campusIds": self.campus,
+                "keyWord": keyWord,
+                "nonFollowUpDays": nonFollowUpDays,
+                "level": level,
+                "startNextTime": startNextTime,
+                "endNextTime": endNextTime,
+                "startLastCommunicateTime": startLastCommunicateTime,
+                "endLastCommunicateTime": endLastCommunicateTime,
+                "page": {"pageNum": page, "pageSize": size}
+            }
+        )
+
+    # 查询意向学员
+    @loop("")
+    def intentions_query_students(self, page, size, distributeStatus: int = 1, keyWord: str = "", level: int = "",
+                                  nonFollowUpDays: int = "", startNextTime: str = "", endNextTime: str = "",
+                                  startLastCommunicateTime: str = "", endLastCommunicateTime: str = ""):
+        """
+        查询意向学员
+        :param size: 分页查询，每页数量
+        :param page: 分页查询，初始页码，应设为 0
+        :param distributeStatus: 是否分配跟进人。 **0** 无跟进人 **1** 有跟进人
+        :param level: 意向级别。 1-5
+        :param keyWord: 查询关键字
+        :param nonFollowUpDays: 未跟进天数
+        :param startNextTime: 计划跟进时间（查询起点）
+        :param endNextTime: 计划跟进时间（查询终点）
+        :param startLastCommunicateTime: 最近跟进时间（查询起点）
+        :param endLastCommunicateTime: 最近跟进时间（查询终点）
+        :return:https://yunxiao.xiaogj.com/app/teacher/#/cluedetails?id=7127357
+        """
+        return self.request(
+            method="post",
+            url="https://yunxiao.xiaogj.com/api/cs-crm/student/listForIntentionManage",
+            json={
+                "_t_": UsedTime.stamp,
+                "distributeStatus": distributeStatus,
+                "campusIds": self.campus,
+                "keyWord": keyWord,
+                "nonFollowUpDays": nonFollowUpDays,
+                "level": level,
+                "startNextTime": startNextTime,
+                "endNextTime": endNextTime,
+                "startLastCommunicateTime": startLastCommunicateTime,
+                "endLastCommunicateTime": endLastCommunicateTime,
+                "page": {"pageNum": page, "pageSize": size}
+            }
+        )
+
     # 查询学生
     @loop("")
     def students_query(self, page, size, curriculumids: tuple = (), classids: tuple = (), name: str = "",
                        status: tuple = (1, 7), class_student_status: int = 0):
         """
         查询学生
         :param size: 分页查询，每页数量
@@ -241,25 +315,22 @@
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-crm/student/list",
             json={
                 "_t_": UsedTime.stamp,
                 "name": name,
                 "campusIds": self.campus,
                 "status": list(status),
-                "intentionStatus": 0,
                 "curriculumIds": list(curriculumids),
                 "classIds": list(classids),
                 "classStudentStatus": class_student_status,
                 "orgTag": 1,
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
-        # 学生数据 - 费用报表。
-
     # 学生数据费用报表。
     @loop("cardCourseTradedList")
     def students_query_course_fee(self, page: int, size: int, displayHistory: bool = True,
                                   status: tuple = (1, 7), studentName: str = ""):
         """
         学生数据费用报表。
         :param size: 分页查询，每页数量
@@ -610,44 +681,66 @@
                 "classId": classid,
                 "inout": inout
             }
         )["data"]
 
     # 列出指定上课日期范围的所有课消记录
     @loop("courseConsumeList")
-    def charges_query_record(self, page, size, startdate: str = "", enddate: str = ""):
+    def charges_query_record(self, page, size, startdate: str = None, enddate: str = None,
+                             before_today: int = 30, after_today: int = 30):
         """
+        列出指定上课日期范围的所有课消记录
         :param size: 每次取数据的分片量
         :param page: 从第几页开始取数据。应设为 0
         :param startdate: YY-MM-DD
         :param enddate: YY-MM-DD
+        :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
+        :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :return:
         """
+
+        startdate = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
+            if startdate is None else startdate
+
+        enddate = time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)) \
+            if enddate is None else enddate
+
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findCourseSignCharge",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "courseStartTime": startdate,
                 "courseEndTime": enddate
             }
         )
 
     # 列出指定上课日期范围的所有课消详情
     @loop("courseConsumeDetailList")
-    def charges_query_detail(self, page, size, startdate: str = "", enddate: str = ""):
+    def charges_query_detail(self, page, size, startdate: str = None, enddate: str = None,
+                             before_today: int = 30, after_today: int = 30):
         """
+        列出指定上课日期范围的所有课消详情
         :param size: 每次取数据的分片量
         :param page: 从第几页开始取数据。应设为 0
         :param startdate: YY-MM-DD
         :param enddate: YY-MM-DD
+        :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
+        :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :return:
         """
+
+        startdate = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
+            if startdate is None else startdate
+
+        enddate = time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)) \
+            if enddate is None else enddate
+
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findCourseSignChargeDetail",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page, "pageSize": size},
                 "assistantTeacherIds": [],
@@ -812,21 +905,31 @@
                 "orderInfoId": order_id,
                 "paymentGroupId": payment_group_id,
                 "_t_": UsedTime.stamp
             }
         )["data"]
 
     # 列出指定操作日期范围的所有账户收支记录
-    def payments_query_record(self, startdate: str = "", enddate: str = "") -> list:
+    def payments_query_record(self, startdate: str = None, enddate: str = None,
+                              before_today: int = 30, after_today: int = 30) -> list:
         """
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
+        :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
+        :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :return:
         """
+
+        startdate = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
+            if startdate is None else startdate
+
+        enddate = time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)) \
+            if enddate is None else enddate
+
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findPaymentAccountCustomRecord",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
@@ -834,46 +937,65 @@
                 "endTime": enddate,
                 "displayInvalidOrder": True
             }
         )["data"]
 
     # 查询业绩归属
     @loop("achievementBelongerDetailItems")
-    def payments_query_achievements_datarange(self, page, size, startdate: str = "", enddate: str = ""):
+    def payments_query_achievements_datarange(self, page, size, startdate: str = None, enddate: str = None,
+                                              before_today: int = 30, after_today: int = 30):
         """
         查询业绩归属，根据日期
         :param size: 分页查询，每页数量
         :param page: 分页查询，起始页码，应设为 0
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
+        :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
+        :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :return:
         """
+
+        startdate = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
+            if startdate is None else startdate
+
+        enddate = time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)) \
+            if enddate is None else enddate
+
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
-                "startTime": startdate,
-                "endTime": enddate
+                "startDate": startdate,
+                "endDate": enddate
             }
         )
 
     # 查询业绩归属
-    def payments_query_achievements(self, startdate: str = "", enddate: str = "", productName: str = "",
-                                    teacherIds: tuple = ()):
+    def payments_query_achievements(self, startdate: str = None, enddate: str = None, productName: str = "",
+                                    teacherIds: tuple = (), before_today: int = 30, after_today: int = 30):
         """
         查询业绩归属，根据信息
         :param teacherIds: 老师ID
         :param productName: 项目名称
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
+        :param before_today: 设定起始日期为今天之前的某天，当 starttime 留空时使用。
+        :param after_today: 设定起始日期为今天之后的某天，当 endtime 留空时使用。
         :return:
         """
+
+        startdate = time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)) \
+            if startdate is None else startdate
+
+        enddate = time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)) \
+            if enddate is None else enddate
+
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
```

### Comparing `yunxiao-0.3.1/yunxiao/yunxiao.py` & `yunxiao-0.3.2/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.1/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.2/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.1
+Version: 0.3.2
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

