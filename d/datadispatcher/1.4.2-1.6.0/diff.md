# Comparing `tmp/datadispatcher-1.4.2.tar.gz` & `tmp/datadispatcher-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadispatcher-1.4.2.tar", last modified: Mon Apr 11 18:58:44 2022, max compression
+gzip compressed data, was "datadispatcher-1.6.0.tar", last modified: Tue Apr 19 12:19:47 2022, max compression
```

## Comparing `datadispatcher-1.4.2.tar` & `datadispatcher-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-11 18:58:44.243905 datadispatcher-1.4.2/
--rw-r--r--   0 ivm        (501) staff       (20)      336 2022-04-11 18:58:44.243698 datadispatcher-1.4.2/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)     2034 2022-03-28 14:09:36.000000 datadispatcher-1.4.2/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-11 18:58:44.238745 datadispatcher-1.4.2/data_dispatcher/
--rwxr-xr-x   0 ivm        (501) staff       (20)       52 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/data_dispatcher/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    14762 2022-04-08 19:52:34.000000 datadispatcher-1.4.2/data_dispatcher/api.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    41350 2022-04-11 15:35:51.000000 datadispatcher-1.4.2/data_dispatcher/db.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1455 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/data_dispatcher/logs.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1900 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/data_dispatcher/logs_oo.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2708 2022-04-05 11:13:17.000000 datadispatcher-1.4.2/data_dispatcher/timelib.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-11 18:58:44.241787 datadispatcher-1.4.2/data_dispatcher/ui/
--rwxr-xr-x   0 ivm        (501) staff       (20)       20 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/data_dispatcher/ui/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     7344 2022-04-07 14:55:39.000000 datadispatcher-1.4.2/data_dispatcher/ui/__main__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     7344 2022-04-07 14:55:39.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2197 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui_file.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1745 2022-04-08 19:52:55.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui_handle.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2021 2022-04-08 19:59:45.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui_lib.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     8222 2022-04-07 14:55:39.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui_project.py
--rw-r--r--   0 ivm        (501) staff       (20)     2090 2022-04-07 14:55:39.000000 datadispatcher-1.4.2/data_dispatcher/ui/ui_rse.py
--rw-r--r--   0 ivm        (501) staff       (20)       83 2022-04-11 18:53:46.000000 datadispatcher-1.4.2/data_dispatcher/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-11 18:58:44.243360 datadispatcher-1.4.2/datadispatcher.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      336 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      704 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)       48 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       44 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       16 2022-04-11 18:58:44.000000 datadispatcher-1.4.2/datadispatcher.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2022-04-11 18:58:44.243971 datadispatcher-1.4.2/setup.cfg
--rwxr-xr-x   0 ivm        (501) staff       (20)     1197 2022-03-28 13:50:13.000000 datadispatcher-1.4.2/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-19 12:19:47.232806 datadispatcher-1.6.0/
+-rw-r--r--   0 ivm        (501) staff       (20)      336 2022-04-19 12:19:47.232540 datadispatcher-1.6.0/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)     2034 2022-03-28 14:09:36.000000 datadispatcher-1.6.0/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-19 12:19:47.227530 datadispatcher-1.6.0/data_dispatcher/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       52 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/data_dispatcher/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    15040 2022-04-19 12:00:30.000000 datadispatcher-1.6.0/data_dispatcher/api.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    44799 2022-04-19 12:17:30.000000 datadispatcher-1.6.0/data_dispatcher/db.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1455 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/data_dispatcher/logs.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1900 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/data_dispatcher/logs_oo.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2708 2022-04-05 11:13:17.000000 datadispatcher-1.6.0/data_dispatcher/timelib.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-19 12:19:47.230229 datadispatcher-1.6.0/data_dispatcher/ui/
+-rwxr-xr-x   0 ivm        (501) staff       (20)       20 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/data_dispatcher/ui/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     8036 2022-04-19 11:59:10.000000 datadispatcher-1.6.0/data_dispatcher/ui/__main__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     8036 2022-04-19 11:59:10.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2197 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui_file.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1745 2022-04-08 19:52:55.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui_handle.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2021 2022-04-08 19:59:45.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui_lib.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     8223 2022-04-19 11:56:14.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui_project.py
+-rw-r--r--   0 ivm        (501) staff       (20)     2090 2022-04-07 14:55:39.000000 datadispatcher-1.6.0/data_dispatcher/ui/ui_rse.py
+-rw-r--r--   0 ivm        (501) staff       (20)       83 2022-04-19 12:19:03.000000 datadispatcher-1.6.0/data_dispatcher/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2022-04-19 12:19:47.232241 datadispatcher-1.6.0/datadispatcher.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      336 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      704 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       48 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       44 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       16 2022-04-19 12:19:47.000000 datadispatcher-1.6.0/datadispatcher.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2022-04-19 12:19:47.232896 datadispatcher-1.6.0/setup.cfg
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1197 2022-03-28 13:50:13.000000 datadispatcher-1.6.0/setup.py
```

### Comparing `datadispatcher-1.4.2/README.rst` & `datadispatcher-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/api.py` & `datadispatcher-1.6.0/data_dispatcher/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,25 @@
         """Deletes a project by id
 
         Args:
             project_id (str): project id
         """
         return self.get(f"delete_project?project_id={project_id}")
         
+    def cancel_project(self, project_id):
+        """Cancels a project by id
+
+        Args:
+            project_id (str): project id
+
+        Returns:
+            (dict) project information
+        """
+        return self.get(f"cancel_project?project_id={project_id}")
+        
     def get_project(self, project_id, with_files=True, with_replicas=False):
         """Gets information about the project
         
         Args:
             project_id (str): project id
 
         Keyword Arguments:
```

### Comparing `datadispatcher-1.4.2/data_dispatcher/db.py` & `datadispatcher-1.6.0/data_dispatcher/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,65 +179,100 @@
         return dict(
             type = self.Type,
             t = self.T.timestamp(),
             data = self.Data
         )
 
 class HasLogRecord(object):
-
-    def __init__(self, log_table, parent_id_columns):
-        self.LogTable = log_table
-        self.IDColumns = parent_id_columns
-        self.IDColumnsText = ",".join(parent_id_columns)
+    
+    #
+    # uses class attributes:
+    #
+    #   LogTable        - name of the table to store the log
+    #   LogIDColumns    - list of columns in the log table identifying the parent
+    #
 
     def add_log(self, type, data=None, **kwargs):
         #print("add_log:", type, data, kwargs)
         c = self.DB.cursor()
         data = (data or {}).copy()
         data.update(kwargs)
-        parent_pk_columns = self.IDColumnsText
+        parent_pk_columns = ",".join(self.LogIDColumns)
         parent_pk_values = ",".join([f"'{v}'" for v in self.pk()])
         c.execute(f"""
             begin;
             insert into {self.LogTable}({parent_pk_columns}, type, data)
                 values({parent_pk_values}, %s, %s);
             commit
         """, (type, json.dumps(data)))
 
+    @classmethod
+    def add_log_bulk(cls, db, records):
+        """
+            records: list of tuples:
+                (
+                    (
+                        id_column1_value,
+                        id_column2_value, ...
+                    ),
+                    type,
+                    { data }
+                )
+        """
+        csv = []
+        for id_values, type, data in records:
+            row = '\t'.join([str(v) for v in id_values] + [type, json.dumps(data)])
+            csv.append(row)
+        csv = io.StringIO("\n".join(csv))
+
+        table = cls.LogTable
+        columns = cls.LogIDColumns + ["type", "data"]
+        c = db.cursor()
+        try:
+            c.execute("begin")
+            c.copy_from(csv, table, columns=columns)
+            c.execute("commit")
+        except:
+            c.execute("rollback")
+            raise
+
     def get_log(self, type=None, since=None, reversed=False):
-        parent_pk_columns = self.IDColumnsText
-        parent_pk_values = ",".join(["'{v}'" for v in self.pk()])
+        parent_pk_columns = self.LogIDColumns
+        parent_pk_values = self.pk()
         wheres = [f"{c} = '{v}'" for c, v in zip(parent_pk_columns, parent_pk_values)]
         if isinstance(since, (float, int)):
             since = datetime.utcfromtimestamp(since).replace(tzinfo=timezone.utc)
             wheres.append(f"t >= {since}")
         if type is not None:
             wheres.append(f"type = '{type}'")
-        wheres = "" if not wheres else " and " + " and ".join(wheres)
+        wheres = " and ".join(wheres)
         desc = "desc" if reversed else ""
         sql = f"""
-            select type, t, message from {self.LogTable}
-                {wheres}
+            select type, t, data from {self.LogTable}
+                where {wheres}
                 order by t {desc}
         """
         c = self.DB.cursor()
         c.execute(sql)
-        return (DBLogRecord(type, t, message) for type, t, message in cursor_iterator())
-        
+        return (DBLogRecord(type, t, message) for type, t, message in cursor_iterator(c))
 
 class DBProject(DBObject, HasLogRecord):
     
     InitialState = "active"
+    States = ["active", "failed", "done", "cancelled", "held"]
+    EndStates = ["failed", "done", "cancelled"]
     
     Columns = "id,owner,created_timestamp,end_timestamp,state,retry_count,attributes".split(",")
     Table = "projects"
     PK = ["id"]
     
+    LogIDColumns = ["project_id"]
+    LogTable = "project_log"
+    
     def __init__(self, db, id, owner=None, created_timestamp=None, end_timestamp=None, state=None, retry_count=0, attributes={}):
-        HasLogRecord.__init__(self, "project_log", ["project_id"])
         self.DB = db
         self.ID = id
         self.Owner = owner
         self.State = state
         self.CreatedTimestamp = created_timestamp               # datetime
         self.RetryCount = retry_count
         self.Attributes = (attributes or {}).copy()
@@ -261,17 +296,18 @@
         out = dict(
             project_id = self.ID,
             owner = self.Owner,
             state = self.State,
             retry_count = self.RetryCount,
             attributes = self.Attributes or {},
             created_timestamp = self.CreatedTimestamp.timestamp(),
+            ended_timestamp = None if self.EndTimestamp is None else self.EndTimestamp.timestamp(),
             active = self.is_active()
         )
-        if with_handles:
+        if with_handles or with_replicas:
             out["file_handles"] = [h.as_jsonable(with_replicas=with_replicas) for h in self.handles()]
             #print("Project.as_jsonable: handles:", out["file_handles"])
         return out
 
     def attributes_as_json(self):
         return json.dumps(self.Attributes, indent=4)
         
@@ -376,40 +412,46 @@
                 p.HandleCounts[h_state] = count
             if p is not None:
                 yield p
         else:
             c.execute(f"""
                 select {columns}
                     from {table} p
-                    where {wheres}
+                    where {p_wheres}
             """)
             for tup in cursor_iterator(c):
                 yield DBProject.from_tuple(db, tup)
-        
+
     def save(self):
         c = self.DB.cursor()
         try:
             c.execute("begin")
             c.execute("""
                 update projects set state=%s, end_timestamp=%s
                     where id=%s
             """, (self.State, self.EndTimestamp, self.ID))
             self.DB.commit()
         except:
             self.DB.rollback()
             raise
-        
+
+    def cancel(self):
+        self.State = "cancelled"
+        self.EndTimestamp = datetime.now(timezone.utc)
+        self.save()
+        self.add_log("ended", state="cancelled")
+
     def handles(self, with_replicas=True, reload=False):
         if reload or self.Handles is None:
             self.Handles = list(DBFileHandle.list(self.DB, project_id=self.ID, with_replicas=with_replicas))
         return self.Handles
-        
+
     def handle(self, namespace, name):
         return DBFileHandle.get(self.DB, self.ID, namespace, name)
-            
+
     def add_files(self, files_descs):
         # files_descs is list of disctionaries: [{"namespace":..., "name":...}, ...]
         files_descs = list(files_descs)     # make sure it's not a generator
         DBFile.create_many(self.DB, files_descs)
         DBFileHandle.create_many(self.DB, self.ID, files_descs)
         
     def files(self):
@@ -439,15 +481,15 @@
 
             self.State = state
             self.EndTimestamp = datetime.now(timezone.utc)
             self.save()
         return handle
 
     def is_active(self, reload=False):
-        print("projet", self.ID, "  handle states:", [h.State for h in self.handles(reload=reload)])
+        #print("projet", self.ID, "  handle states:", [h.State for h in self.handles(reload=reload)])
         return self.State == "active" and not all(h.State in ("done", "failed") for h in self.handles(reload=reload))
             
     def reserve_next_file(self, worker_id):
         handle = DBFileHandle.reserve_next_available(self.DB, self.ID, worker_id)
         if handle is not None:
             did = handle.did()
         return handle
@@ -468,25 +510,46 @@
                 order by t, namespace, name
         """, (self.ID,))
         for tup in cursor_iterator(c):
             namespace, name, t, type, data = tup
             log_record = DBLogRecord(type, t, data)
             log_record.Namespace = namespace
             log_record.Name = name
-            print("log_record:", log_record)
+            #print("log_record:", log_record)
             yield log_record
+    
+    @staticmethod
+    def purge(db, retain=3600):
+        c = db.cursor()
+        table = DBProject.Table
+        t_retain = datetime.now(timezone.utc) - timedelta(seconds=retain)
+        c.execute("begin")
+        try:
+            c.execute(f"""
+                delete from {table}
+                    where state in ('done', 'failed', 'cancelled')
+                        and end_timestamp is not null
+                        and end_timestamp < %s
+            """, (t_retain,))
+            c.execute("commit")
+        except:
+            c.execute("rollback")
+            raise
+        return c.rowcount
 
 class DBFile(DBObject, HasLogRecord):
     
     Columns = ["namespace", "name"]
     PK = ["namespace", "name"]
     Table = "files"
     
+    LogIDColumns = ["namespace", "name"]
+    LogTable = "file_log"
+    
     def __init__(self, db, namespace, name):
-        HasLogRecord.__init__(self, "file_log", ["namespace", "name"])
         self.DB = db
         self.Namespace = namespace
         self.Name = name
         self.Replicas = None	# {rse -> DBReplica}
     
     def id(self):
         return f"{self.Namespace}:{self.Name}"
@@ -507,15 +570,19 @@
         if self.Replicas is None:
             self.Replicas = {r.RSE: r for r in DBReplica.list(self.DB, self.Namespace, self.Name)}
         return self.Replicas
 
     def create_replica(self, rse, path, url, preference=0, available=False):
         DBReplica.create(self.DB, self.Namespace, self.Name, rse, path, url, preference=preference, available=available)
         self.Replicas = None	# force re-load from the DB
-        
+        if False:
+            self.add_log("found", rse=rse, path=path, url=url)
+            if available:
+                self.add_log("available", rse=rse)
+
     def get_replica(self, rse):
         return self.replicas().get(rse)
         
     @staticmethod
     def create(db, namespace, name, error_if_exists=False):
         c = self.DB.cursor()
         try:
@@ -587,14 +654,34 @@
                     on conflict (namespace, name) do nothing;       -- in case some other projects still use it
                 drop table {temp_table};
                 commit
                 """)
         except Exception as e:
             c.execute("rollback")
             raise
+            
+    @staticmethod
+    def purge(db):
+        c = db.cursor()
+        table = DBFile.Table
+        c.execute("begin")
+        try:
+            c.execute(f"""
+                delete from {table} f
+                    where not exists (
+                            select * from file_handles h 
+                                where f.namespace = h.namespace
+                                    and f.name = h.name
+                    )
+            """, (t_retain,))
+            c.execute("commit")
+        except:
+            c.execute("rollback")
+            raise
+        return c.rowcount
     
 class DBReplica(DBObject):
     Table = "replicas"
     ViewWithRSEStatus = "replicas_with_rse_availability"
     
     Columns = ["namespace", "name", "rse", "path", "url", "preference", "available"]
     PK = ["namespace", "name", "rse"]
@@ -655,15 +742,15 @@
                 commit
             """, (namespace, name, rse, path, url, preference, available,
                     path, url, preference, available)
             )
         except:
             c.execute("rollback")
             raise
-            
+        
         return DBReplica.get(db, namespace, name, rse)
 
     def save(self):
         table = self.Table
         c = self.DB.cursor()
         try:
             c.execute(f"""
@@ -693,56 +780,80 @@
                     where rse=%s and namespace || ':' || name = any(%s);
                 commit
             """, (rse, dids))
         except:
             c.execute("rollback")
             raise
 
+        if False:
+            log_records = (
+                (
+                    did.split(":", 1),
+                    "removed",
+                    {
+                        "rse":  rse,
+                    }
+                )
+                for did in dids
+            )
+
+            DBFile.add_log_bulk(db, log_records)
+
     @staticmethod
     def create_bulk(db, rse, preference, replicas):
         # replicas: {(namespace, name) -> {"path":.., "url":..}}
         # do not touch availability, update if exists
 
         csv = ['%s\t%s\t%s\t%s\t%s\t%s' % (namespace, name, rse, info["path"], info["url"], preference) 
             for (namespace, name), info in replicas.items()]
         #print("DBReplica.create_bulk: csv:", csv)
-        data = io.StringIO("\n".join(csv))
+        csv = io.StringIO("\n".join(csv))
         table = DBReplica.Table
         columns = DBReplica.columns(as_text=True)
+        
         c = db.cursor()
         try:
             t = int(time.time()*1000)
             temp_table = f"file_replicas_temp_{t}"
             c.execute("begin")
             c.execute(f"create temp table {temp_table} (ns text, n text, r text, p text, u text, pr int)")
-            c.copy_from(data, temp_table)
+            c.copy_from(csv, temp_table)
+            csv = None         # to release memory
             c.execute(f"""
                 insert into {table}({columns}) 
                     select t.ns, t.n, t.r, t.p, t.u, t.pr, false from {temp_table} t
                     on conflict (namespace, name, rse)
                         do nothing;
                 """)
 
-            if False:
-                c.execute(f"""
-                    insert into file_log (namespace, name, type, data)
-                        select t.ns, t.n, 'replica added', ('{"rse":"' || t.r || '", "url":"' || t.u || '", "preference":' || t.pr::text || '}')::jsonb
-                        from {temp_table} t
-                        on conflict (namespace, name, t) do nothing
-                """)
-
             c.execute(f"""
                 drop table {temp_table};
                 commit
             """)
 
         except Exception as e:
             c.execute("rollback")
             raise
 
+        if False:
+            log_records = (
+                (
+                    (namespace, name),
+                    "found",
+                    {
+                        "url":  info["url"],
+                        "rse":  rse,
+                        "path": info["path"]
+                    }
+                )
+                for (namespace, name), info in replicas.items()
+            )
+
+            DBFile.add_log_bulk(db, log_records)
+
     @staticmethod
     def update_availability_bulk(db, available, rse, dids):
         # dids is list of dids: ["namespace:name", ...]
         if not dids:    return
         table = DBReplica.Table
         val = "true" if available else "false"
         undids = [did.split(":", 1) for did in dids]
@@ -757,14 +868,30 @@
             """
             c.execute(sql, (val, dids, rse))
             c.execute("commit")
         except:
             c.execute("rollback")
             raise
 
+        if False:
+            event = "available" if available else "unavailable"
+            log_records = (
+                (
+                    (namespace, name),
+                    event,
+                    {
+                        "rse":  rse
+                    }
+                )
+                for (namespace, name) in undids
+            )
+
+            DBFile.add_log_bulk(db, log_records)
+
+
 class DBFileHandle(DBObject, HasLogRecord):
 
     Columns = ["project_id", "namespace", "name", "state", "worker_id", "attempts", "attributes"]
     PK = ["project_id", "namespace", "name"]
     Table = "file_handles"
 
     InitialState = ReadyState = "initial"
@@ -776,16 +903,18 @@
             "available", 
             "reserved",
             "done",
             "failed"
         ]
 
 
+    LogIDColumns = ["project_id", "namespace", "name"]
+    LogTable = "file_handle_log"
+
     def __init__(self, db, project_id, namespace, name, state=None, worker_id=None, attempts=0, attributes={}):
-        HasLogRecord.__init__(self, "file_handle_log", ["project_id", "namespace", "name"])
         self.DB = db
         self.ProjectID = project_id
         self.Namespace = namespace
         self.Name = name
         self.State = state or self.InitialState
         self.WorkerID = worker_id
         self.Attempts = attempts
@@ -1028,21 +1157,21 @@
         return any(r.Available and r.RSEAvailable for r in self.replicas().values())
 
     def is_active(self):
         return self.State not in ("done", "failed")
 
     def done(self):
         self.State = "done"
+        self.add_log("done", worker=self.WorkerID)
         self.WorkerID = None
         self.save()
-        self.add_log("done", worker=self.WorkerID)
 
     def failed(self, retry=True):
         self.State = self.ReadyState if retry else "failed"
-        self.add_log("failed", worker=self.WorkerID or None, retry=retry)
+        self.add_log("failed", worker=self.WorkerID or None, final=not retry)
         self.WorkerID = None
         self.save()
 
     def reserved_by(self, worker_id):
         # just add a record to the log. Assume the actual reservation was done by reserve_next_available()
         self.add_log("reserved", worker=worker_id)
 
@@ -1100,20 +1229,21 @@
             raise
         
         return DBRSE.get(db, name)
 
     def save(self):
         c = self.DB.cursor()
         try:
+            print("saving urls:", self.PinURL, self.PollURL)
             c.execute("begin")
             c.execute("""
                 begin;
                 update rses 
                     set description=%s, is_available=%s, is_tape=%s, pin_url=%s, poll_url=%s, remove_prefix=%s, add_prefix=%s, preference=%s
                     where name=%s
                 """, (self.Description, self.Available, self.Tape, self.PinURL, self.PollURL, self.RemovePrefix, self.AddPrefix, self.Preference, self.Name)
             )
             c.execute("commit")
         except:
             c.execute("rollback")
             raise
-        
+
```

### Comparing `datadispatcher-1.4.2/data_dispatcher/logs.py` & `datadispatcher-1.6.0/data_dispatcher/logs.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/logs_oo.py` & `datadispatcher-1.6.0/data_dispatcher/logs_oo.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/timelib.py` & `datadispatcher-1.6.0/data_dispatcher/timelib.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/__main__.py` & `datadispatcher-1.6.0/data_dispatcher/ui/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,29 @@
 
     worker [-n|<worker id>]                                - set or print my worker_id 
                                                              -n generates new one
                                                              worker id will be saved in <CWD>/.worker_id
     create project ...
     show project ...
     list projects ...
-    
+
+    delete project <project_id>
+    cancel project [-j] <project_id>                       - cancel project, -j - print project info as JSON
+
     show file [-j] <namespace>:<name>
 
     show handle [-j] <project_id> <namespace>:<name>       - show file handle, -j - as JSON
 
     next [-j] [-t <timeout>] <project_id>                  - get next available file, 
                                                              -j - as JSON
                                                              -t - wait for next file until "timeout" seconds, 
                                                                   otherwise, wait until the project finishes
     done <project_id> <namespace>:<name>                   - mark the file as successfully processed
     failed [-f] <project_id> <namespace>:<name>            - mark the file as failed, -f means "final", no retries
 
-    delete project <project_id>
-    
     list rses [-j]                                         - list RSEs, -j: print as JSON
     show rse [-j] <rse>                                    - show information about RSE
     set rse -a (up|down) <rse>                             - set RSE availability (requires admin privileges)
     
     login x509 <user> <cert> <key>
     login password <user>
 """
@@ -131,20 +132,39 @@
         else:
             print(Usage)
             sys.exit(2)
         
     elif command == "delete":
         subcommand, rest = rest[0], rest[1:]
         if subcommand == "project":
-            project_id = rest[0]
+            if not rest:
+                print(Usage)
+                sys.exit(2)
+            project_id = int(rest[0])
             client.delete_project(project_id)
         else:
             print(Usage)
             sys.exit(2)
         
+    elif command == "cancel":
+        subcommand, rest = rest[0], rest[1:]
+        if subcommand == "project":
+            opts, args = getopt.getopt(rest, "j")
+            opts = dict(opts)
+            if not args:
+                print(Usage)
+                sys.exit(2)
+            project_id = int(args[0])
+            out = client.cancel_project(project_id)
+            if "-j" in opts:
+                print(pretty_json(out))
+        else:
+            print(Usage)
+            sys.exit(2)
+        
 
     elif command == "next":
         opts, args = getopt.getopt(rest, "jt:")
         opts = dict(opts)
         if not args:
             print(Usage)
             sys.exit(2)
```

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,29 @@
 
     worker [-n|<worker id>]                                - set or print my worker_id 
                                                              -n generates new one
                                                              worker id will be saved in <CWD>/.worker_id
     create project ...
     show project ...
     list projects ...
-    
+
+    delete project <project_id>
+    cancel project [-j] <project_id>                       - cancel project, -j - print project info as JSON
+
     show file [-j] <namespace>:<name>
 
     show handle [-j] <project_id> <namespace>:<name>       - show file handle, -j - as JSON
 
     next [-j] [-t <timeout>] <project_id>                  - get next available file, 
                                                              -j - as JSON
                                                              -t - wait for next file until "timeout" seconds, 
                                                                   otherwise, wait until the project finishes
     done <project_id> <namespace>:<name>                   - mark the file as successfully processed
     failed [-f] <project_id> <namespace>:<name>            - mark the file as failed, -f means "final", no retries
 
-    delete project <project_id>
-    
     list rses [-j]                                         - list RSEs, -j: print as JSON
     show rse [-j] <rse>                                    - show information about RSE
     set rse -a (up|down) <rse>                             - set RSE availability (requires admin privileges)
     
     login x509 <user> <cert> <key>
     login password <user>
 """
@@ -131,20 +132,39 @@
         else:
             print(Usage)
             sys.exit(2)
         
     elif command == "delete":
         subcommand, rest = rest[0], rest[1:]
         if subcommand == "project":
-            project_id = rest[0]
+            if not rest:
+                print(Usage)
+                sys.exit(2)
+            project_id = int(rest[0])
             client.delete_project(project_id)
         else:
             print(Usage)
             sys.exit(2)
         
+    elif command == "cancel":
+        subcommand, rest = rest[0], rest[1:]
+        if subcommand == "project":
+            opts, args = getopt.getopt(rest, "j")
+            opts = dict(opts)
+            if not args:
+                print(Usage)
+                sys.exit(2)
+            project_id = int(args[0])
+            out = client.cancel_project(project_id)
+            if "-j" in opts:
+                print(pretty_json(out))
+        else:
+            print(Usage)
+            sys.exit(2)
+        
 
     elif command == "next":
         opts, args = getopt.getopt(rest, "jt:")
         opts = dict(opts)
         if not args:
             print(Usage)
             sys.exit(2)
```

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui_file.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui_file.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui_handle.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui_handle.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui_lib.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui_lib.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui_project.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,7 +190,8 @@
                     done_files += 1
                 elif h["state"] == "failed":
                     failed_files += 1
             counts = "%d/%d/%d" % (done_files, failed_files, nfiles)
             print("%-15s %-15s %19s %15s %17s" % (prj["project_id"], prj["owner"], ct, prj["state"], counts))
         print("%s %s %s %s %s" % ("-"*15, "-"*15, "-"*19, "-"*15, "-"*17))
     
+
```

### Comparing `datadispatcher-1.4.2/data_dispatcher/ui/ui_rse.py` & `datadispatcher-1.6.0/data_dispatcher/ui/ui_rse.py`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/datadispatcher.egg-info/SOURCES.txt` & `datadispatcher-1.6.0/datadispatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datadispatcher-1.4.2/setup.py` & `datadispatcher-1.6.0/setup.py`

 * *Files identical despite different names*

