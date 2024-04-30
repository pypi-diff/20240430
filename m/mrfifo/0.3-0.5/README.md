# Comparing `tmp/mrfifo-0.3.tar.gz` & `tmp/mrfifo-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrfifo-0.3.tar", last modified: Fri Mar  1 16:52:37 2024, max compression
+gzip compressed data, was "mrfifo-0.5.tar", last modified: Tue Apr 30 10:32:24 2024, max compression
```

## Comparing `mrfifo-0.3.tar` & `mrfifo-0.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.270680 mrfifo-0.3/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      115 2024-02-20 15:34:36.000000 mrfifo-0.3/.coveragerc
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.166680 mrfifo-0.3/.github/
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.238680 mrfifo-0.3/.github/workflows/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1362 2024-02-20 15:34:36.000000 mrfifo-0.3/.github/workflows/python-package.yml
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3078 2024-02-20 15:34:36.000000 mrfifo-0.3/.gitignore
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1068 2024-02-20 15:34:36.000000 mrfifo-0.3/LICENSE
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     8251 2024-03-01 16:52:37.270680 mrfifo-0.3/PKG-INFO
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     7733 2024-02-20 15:34:36.000000 mrfifo-0.3/README.md
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1398 2024-02-20 15:34:36.000000 mrfifo-0.3/ROADMAP.md
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      281 2024-02-20 15:34:36.000000 mrfifo-0.3/environment.yaml
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.262680 mrfifo-0.3/mrfifo/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    12985 2024-03-01 13:37:00.000000 mrfifo-0.3/mrfifo/__init__.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      106 2024-03-01 16:38:53.000000 mrfifo-0.3/mrfifo/contrib.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)   423976 2024-03-01 16:13:02.000000 mrfifo-0.3/mrfifo/fast_loops.c
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    10822 2024-03-01 16:12:56.000000 mrfifo-0.3/mrfifo/fast_loops.pyx
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1823 2024-02-20 15:34:36.000000 mrfifo-0.3/mrfifo/parallel.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     2905 2024-03-01 13:13:59.000000 mrfifo-0.3/mrfifo/parts.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1475 2024-03-01 13:20:46.000000 mrfifo-0.3/mrfifo/plumbing.py
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     2347 2024-02-20 15:34:36.000000 mrfifo-0.3/mrfifo/util.py
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.266680 mrfifo-0.3/mrfifo.egg-info/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     8251 2024-03-01 16:52:36.000000 mrfifo-0.3/mrfifo.egg-info/PKG-INFO
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      524 2024-03-01 16:52:37.000000 mrfifo-0.3/mrfifo.egg-info/SOURCES.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-03-01 16:52:36.000000 mrfifo-0.3/mrfifo.egg-info/dependency_links.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-02-20 15:34:58.000000 mrfifo-0.3/mrfifo.egg-info/not-zip-safe
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        7 2024-03-01 16:52:36.000000 mrfifo-0.3/mrfifo.egg-info/top_level.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       38 2024-02-20 15:34:36.000000 mrfifo-0.3/requirements.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      901 2024-03-01 16:52:37.270680 mrfifo-0.3/setup.cfg
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      974 2024-02-20 15:34:36.000000 mrfifo-0.3/setup.py
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.266680 mrfifo-0.3/test_data/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       41 2024-02-20 15:34:36.000000 mrfifo-0.3/test_data/simple.txt
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       50 2024-02-20 15:34:36.000000 mrfifo-0.3/test_data/simple.txt.gz
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3294 2024-02-20 15:34:36.000000 mrfifo-0.3/test_data/tiny_test.bam
-drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-03-01 16:52:37.266680 mrfifo-0.3/tests/
--rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    12485 2024-02-20 15:34:36.000000 mrfifo-0.3/tests/test_cy.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.356227 mrfifo-0.5/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      115 2024-02-20 15:34:36.000000 mrfifo-0.5/.coveragerc
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:23.972228 mrfifo-0.5/.github/
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.132228 mrfifo-0.5/.github/workflows/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1362 2024-02-20 15:34:36.000000 mrfifo-0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1084 2024-03-14 08:18:30.000000 mrfifo-0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3078 2024-02-20 15:34:36.000000 mrfifo-0.5/.gitignore
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1068 2024-02-20 15:34:36.000000 mrfifo-0.5/LICENSE
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     8251 2024-04-30 10:32:24.356227 mrfifo-0.5/PKG-INFO
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     7733 2024-02-20 15:34:36.000000 mrfifo-0.5/README.md
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1015 2024-04-15 12:46:55.000000 mrfifo-0.5/ROADMAP.md
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      281 2024-02-20 15:34:36.000000 mrfifo-0.5/environment.yaml
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.236227 mrfifo-0.5/mrfifo/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    14649 2024-04-17 14:37:36.000000 mrfifo-0.5/mrfifo/__init__.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      106 2024-04-24 13:40:07.000000 mrfifo-0.5/mrfifo/contrib.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)   452785 2024-04-30 10:27:22.000000 mrfifo-0.5/mrfifo/fast_loops.c
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    11119 2024-04-17 14:37:22.000000 mrfifo-0.5/mrfifo/fast_loops.pyx
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1823 2024-02-20 15:34:36.000000 mrfifo-0.5/mrfifo/parallel.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3351 2024-03-19 09:22:55.000000 mrfifo-0.5/mrfifo/parts.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     1475 2024-03-01 13:20:46.000000 mrfifo-0.5/mrfifo/plumbing.py
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     2410 2024-04-15 12:46:55.000000 mrfifo-0.5/mrfifo/util.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.284227 mrfifo-0.5/mrfifo.egg-info/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     8251 2024-04-30 10:32:23.000000 mrfifo-0.5/mrfifo.egg-info/PKG-INFO
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      576 2024-04-30 10:32:23.000000 mrfifo-0.5/mrfifo.egg-info/SOURCES.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-04-30 10:32:23.000000 mrfifo-0.5/mrfifo.egg-info/dependency_links.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        1 2024-02-20 15:34:58.000000 mrfifo-0.5/mrfifo.egg-info/not-zip-safe
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)        7 2024-04-30 10:32:23.000000 mrfifo-0.5/mrfifo.egg-info/top_level.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       59 2024-04-24 13:38:15.000000 mrfifo-0.5/pyproject.toml
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       50 2024-04-24 13:40:15.000000 mrfifo-0.5/requirements.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      901 2024-04-30 10:32:24.364227 mrfifo-0.5/setup.cfg
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)      974 2024-02-20 15:34:36.000000 mrfifo-0.5/setup.py
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.320227 mrfifo-0.5/test_data/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       41 2024-02-20 15:34:36.000000 mrfifo-0.5/test_data/simple.txt
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)       50 2024-02-20 15:34:36.000000 mrfifo-0.5/test_data/simple.txt.gz
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)     3294 2024-02-20 15:34:36.000000 mrfifo-0.5/test_data/tiny_test.bam
+drwxr-xr-x   0 marjens   (2364) marjens_usr  (2364)        0 2024-04-30 10:32:24.332227 mrfifo-0.5/tests/
+-rw-r--r--   0 marjens   (2364) marjens_usr  (2364)    13948 2024-04-17 14:44:56.000000 mrfifo-0.5/tests/test_cy.py
```

### Comparing `mrfifo-0.3/.github/workflows/python-package.yml` & `mrfifo-0.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/.gitignore` & `mrfifo-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/LICENSE` & `mrfifo-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/PKG-INFO` & `mrfifo-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfifo
-Version: 0.3
+Version: 0.5
 Summary: Map-Reduce parallelism over FIFOs (named pipes)
 Home-page: https://github.com/marvin-jens/mrfifo
 Author: Marvin Jens
 Author-email: marvin.jens@charite.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/marvin-jens/mrfifo/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mrfifo-0.3/README.md` & `mrfifo-0.5/README.md`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/ROADMAP.md` & `mrfifo-0.5/ROADMAP.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # Roadmap
 
 ## v1.0
 
 Must include everything that is needed for SPACEMAKE 2.0 (aka drop-dropseq), but also come with 
 sufficient examples & docs to allow others to re-use in other scenarios.
 
-  * look into dropping numpy requirement
-  * test-cases for SAM/BAM/CRAM input w header handling
-  * add examples that use mp primitives for shared state w low bandwidth requirements
-  * minimal sanity checking to detect stale inputs/outputs that would cause dead-locked workflows,
-      as well as violations of the point-to-point principle which would lead to undefined behaviour.
   * expanded documentation (split-by UMI or CB tag)
   * one round of adding doc-strings and auto-generating reference docs (sphinx?)
 
 ## v1.x
 
 Minor improvements in usability and documentation.
```

### Comparing `mrfifo-0.3/mrfifo/__init__.py` & `mrfifo-0.5/mrfifo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,31 +65,46 @@
     def close(self):
         for f in self.file_objects:
             self.logger.debug(f"closing {f}")
             f.flush()
             f.close()
             self.logger.debug(f"done closing {f}")
 
+        self.file_objects = []
+
     def __repr__(self):
         return f"FIFO({self.mode} names={self.get_names()}) n={self.n}"
 
 
+# class ITER(object):
+#     def __init__(self, iterable):
+#         self.iterable = iterable
+#         self.it = iter(self.iterable)
+
+#     def get(self):
+#         return next(self.it)  # this will eventually raise StopIteration
+
+
 def fifo_routed(
     f, pass_internals=False, fifo_name_format={}, _manage_fifos=True, **kwargs
 ):
     from functools import wraps
 
     fifo_vars = {}
     kw = {}
     for k, v in kwargs.items():
         # print(f"{k} : {v} {type(v)}")
         if type(v) is FIFO:
             if fifo_name_format:
                 v = v._format_name(fifo_name_format)
             fifo_vars[k] = v
+        # elif type(v) is ITER:
+        #     # replace the ITER object with whatever is returned at the current iteration
+        #     # this may raise a StopIteration
+        #     kw[k] = v.get()
         else:
             kw[k] = v
 
     @wraps(f)
     def wrapper(
         result_dict={}, pipe_dict={}, exc_dict={}, job_name="job", args=(), **kwds
     ):
@@ -154,37 +169,40 @@
     def __init__(self, name, n=4):
         self.name = name
         self.n = n
         self.logger = logging.getLogger(f"{self.name}.Workflow")
         self.job_count_by_pattern = defaultdict(int)
 
         self._jobs = []
+        self._subs = []
 
         self._fifo_readers = defaultdict(list)
         self._fifo_writers = defaultdict(list)
         self._fifo_balance = defaultdict(int)
 
         import multiprocessing as mp
 
         self.manager = mp.Manager()
         self.pipe_dict = self.manager.dict()
         self.result_dict = self.manager.dict()
         self.exc_dict = self.manager.dict()
 
-    def register_fifos(self, fifos, job_name):
+    def register_fifos(
+        self, fifos, job_name, n_reopen_inputs=1, n_reopen_outputs=1, **kwargs
+    ):
         n_readers = 0
         n_writers = 0
         for f in fifos:
             for name in f.get_names():
                 if f.is_reader():
-                    self._fifo_balance[name] += 1
+                    self._fifo_balance[name] += n_reopen_inputs
                     self._fifo_readers[name].append(job_name)
                     n_readers += 1
                 else:
-                    self._fifo_balance[name] -= 1
+                    self._fifo_balance[name] -= n_reopen_outputs
                     self._fifo_writers[name].append(job_name)
                     n_writers += 1
 
         return n_readers, n_writers
 
     def check(self):
         unbalanced = False
@@ -233,15 +251,15 @@
             result_dict=self.result_dict,
             pipe_dict=self.pipe_dict,
             exc_dict=self.exc_dict,
             name=job_name,
         )
 
         n_readers, n_writers = self.register_fifos(
-            fifo_vars.values(), job_name=job_name
+            fifo_vars.values(), job_name=job_name, **kwargs
         )
         self.logger.debug(
             f"add_job job={job} n_readers={n_readers} n_writers={n_writers} fifo_vars={fifo_vars}"
         )
         self._jobs.append(job)
 
         if assert_n_reader_ge:
@@ -251,19 +269,91 @@
         if assert_n_reader_le:
             assert n_readers <= assert_n_reader_le
         if assert_n_writer_le:
             assert n_writers <= assert_n_writer_le
 
         return self
 
+    def subworkflow(self, name="subworkflow"):
+        sub = Workflow(name)
+        # sub-workflows share the plumbing
+        sub.pipe_dict = self.pipe_dict
+        self._subs.append(sub)
+        self._jobs.append(sub)
+
+        return sub
+
     # presets/short-hands for more readable workflow compositions
     def reader(self, *argc, job_name="{workflow}.reader{n}", **kwargs):
-
         return self.add_job(*argc, job_name=job_name, assert_n_writer_ge=1, **kwargs)
 
+    def run(self, dry_run=False):
+        # shared plumbing between main and sub-workflows
+        for sub in self._subs:
+            for name, jobnames in sub._fifo_readers.items():
+                self._fifo_readers[name].extend(jobnames)
+
+            for name, jobnames in sub._fifo_writers.items():
+                self._fifo_writers[name].extend(jobnames)
+
+            for name, bal in sub._fifo_balance.items():
+                self._fifo_balance[name] += bal
+
+        # gather all named pipes that are required
+        pipe_names = self.get_pipe_list()
+        self.logger.debug(f"pipe_names={pipe_names}")
+        self.check()
+        if not dry_run:
+            with plumbing.create_named_pipes(pipe_names) as pipes:
+                self.pipe_dict.update(pipes)
+                # start all processes in reverse data-flow order
+                for job in reversed(self._jobs):
+                    if type(job) is Workflow:
+                        sub = job
+                        # we have a sub-workflow!
+                        for job in reversed(sub._jobs):
+                            job.start()
+
+                        # join jobs in data-flow order
+                        for job in sub._jobs:
+                            job.join()
+                    else:
+                        self.logger.debug(f"starting {job}")
+                        job.start()
+
+                # join jobs in data-flow order
+                for job in self._jobs:
+                    self.logger.debug(f"waiting for {job}")
+                    job.join()
+
+        # check for exceptions that occurred in child processes
+        caught_exc = False
+        for jobname, exc in sorted(self.exc_dict.items()):
+            for line in exc:
+                self.logger.error(f"exception in {jobname}: {line}")
+                caught_exc = True
+
+        if caught_exc:
+            raise WorkflowError(
+                "detected unhandled exceptions in jobs during workflow-execution"
+            )
+
+        return self
+
+    def __str__(self):
+        # TODO: make this more comprehensive and beautiful
+        buf = [f"Workflow({self.name})"]
+        for i, job in self._fifo_readers.items():
+            buf.append(f"I:{i} -> J:{job}")
+
+        for o, job in self._fifo_writers.items():
+            buf.append(f"J:{job} -> O:{o}")
+
+        return "\n".join(buf)
+
     def gz_reader(
         self,
         *argc,
         job_name="{workflow}.igzip_text_reader{n}",
         func=parts.igzip_reader,
         inputs=["/dev/stdin"],
         output=FIFO("input_text", "wb"),
@@ -400,50 +490,7 @@
 
         if caught_exc:
             raise WorkflowError(
                 "detected unhandled exceptions in jobs during workflow-execution"
             )
 
         return self
-
-    def run(self, dry_run=False):
-        # gather all named pipes that are required
-        pipe_names = self.get_pipe_list()
-        self.logger.debug(f"pipe_names={pipe_names}")
-        self.check()
-        if not dry_run:
-            with plumbing.create_named_pipes(pipe_names) as pipes:
-                self.pipe_dict.update(pipes)
-                # start all processes in reverse data-flow order
-                for job in reversed(self._jobs):
-                    self.logger.debug(f"starting {job}")
-                    job.start()
-
-                # join jobs in data-flow order
-                for job in self._jobs:
-                    self.logger.debug(f"waiting for {job}")
-                    job.join()
-
-        # check for exceptions that occurred in child processes
-        caught_exc = False
-        for jobname, exc in sorted(self.exc_dict.items()):
-            for line in exc:
-                self.logger.error(f"exception in {jobname}: {line}")
-                caught_exc = True
-
-        if caught_exc:
-            raise WorkflowError(
-                "detected unhandled exceptions in jobs during workflow-execution"
-            )
-
-        return self
-
-    def __str__(self):
-        # TODO: make this more comprehensive and beautiful
-        buf = [f"Workflow({self.name})"]
-        for i, job in self._fifo_readers.items():
-            buf.append(f"I:{i} -> J:{job}")
-
-        for o, job in self._fifo_writers.items():
-            buf.append(f"J:{job} -> O:{o}")
-
-        return "\n".join(buf)
```

### Comparing `mrfifo-0.3/mrfifo/fast_loops.c` & `mrfifo-0.5/mrfifo/fast_loops.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "mrfifo.fast_loops",
         "sources": [
@@ -28,18 +28,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0"
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
+#define __PYX_EXTRA_ABI_MODULE_NAME "limited"
+#else
+#define __PYX_EXTRA_ABI_MODULE_NAME ""
+#endif
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -64,14 +69,15 @@
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
+#define __PYX_LIMITED_VERSION_HEX PY_VERSION_HEX
 #if defined(GRAALVM_PYTHON)
   /* For very preliminary testing purposes. Most variables are set the same as PyPy.
      The existence of this section does not imply that anything works or is even tested */
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 1
@@ -122,24 +128,27 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 0
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -182,15 +191,21 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
+  #ifdef Py_LIMITED_API
+    #undef __PYX_LIMITED_VERSION_HEX
+    #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
+  #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 1
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_CLINE_IN_TRACEBACK
   #define CYTHON_CLINE_IN_TRACEBACK 0
@@ -230,69 +245,92 @@
     #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 1
   #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
+    #define CYTHON_USE_TP_FINALIZE 0
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -375,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -452,14 +493,22 @@
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
+#ifndef CYTHON_USE_CPP_STD_MOVE
+  #if defined(__cplusplus) && (\
+    __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600))
+    #define CYTHON_USE_CPP_STD_MOVE 1
+  #else
+    #define CYTHON_USE_CPP_STD_MOVE 0
+  #endif
+#endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
             typedef unsigned char     uint8_t;
             typedef unsigned short    uint16_t;
             typedef unsigned int      uint32_t;
@@ -551,67 +600,99 @@
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+#if CYTHON_COMPILING_IN_LIMITED_API
+    static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *exception_table = NULL;
+        PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
+        PyObject *py_minor_version = NULL;
+        #endif
+        long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
-        if (!(empty = PyTuple_New(0))) goto end;
-        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+        #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
+        minor_version = 11;
+        #else
+        if (!(version_info = PySys_GetObject("version_info"))) goto end;
+        if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
+        minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
+        if (minor_version == -1 && PyErr_Occurred()) goto end;
+        #endif
+        if (!(types_module = PyImport_ImportModule("types"))) goto end;
+        if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
+        if (minor_version <= 7) {
+            (void)p;
+            result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else if (minor_version <= 10) {
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else {
+            if (!(exception_table = PyBytes_FromStringAndSize(NULL, 0))) goto end;
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
+        }
     end:
-        Py_XDECREF((PyObject*) co);
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(empty);
+        Py_XDECREF(code_type);
+        Py_XDECREF(exception_table);
+        Py_XDECREF(types_module);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
+    #ifndef CO_OPTIMIZED
+    #define CO_OPTIMIZED 0x0001
+    #endif
+    #ifndef CO_NEWLOCALS
+    #define CO_NEWLOCALS 0x0002
+    #endif
+    #ifndef CO_VARARGS
+    #define CO_VARARGS 0x0004
+    #endif
+    #ifndef CO_VARKEYWORDS
+    #define CO_VARKEYWORDS 0x0008
+    #endif
+    #ifndef CO_ASYNC_GENERATOR
+    #define CO_ASYNC_GENERATOR 0x0200
+    #endif
+    #ifndef CO_GENERATOR
+    #define CO_GENERATOR 0x0020
+    #endif
+    #ifndef CO_COROUTINE
+    #define CO_COROUTINE 0x0080
+    #endif
+#elif PY_VERSION_HEX >= 0x030B0000
+  static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+    PyCodeObject *result;
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
+    if (!empty_bytes) return NULL;
+    result =
+      #if PY_VERSION_HEX >= 0x030C0000
+        PyUnstable_Code_NewWithPosOnlyArgs
+      #else
+        PyCode_NewWithPosOnlyArgs
+      #endif
+        (a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, name, fline, lnos, empty_bytes);
+    Py_DECREF(empty_bytes);
+    return result;
+  }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
@@ -678,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -703,15 +789,40 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
+#if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
 #ifndef METH_METHOD
@@ -729,14 +840,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -804,27 +917,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -853,17 +966,22 @@
   #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
 #else
   #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
   #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
+#else
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
+#endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -979,17 +1097,42 @@
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_ITEM(o, i)
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) (PyTuple_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyList_SET_ITEM(o, i, v) (PyList_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_GET_SIZE(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_GET_SIZE(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_GET_SIZE(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_GET_SIZE(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_GET_SIZE(o)
 #else
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_GetItem(o, i)
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) PyTuple_SetItem(o, i, v)
+  #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
+#endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
@@ -1061,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1136,17 +1279,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1166,32 +1310,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1233,15 +1360,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1254,14 +1381,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1304,14 +1432,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1520,33 +1649,55 @@
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* fastcall.proto */
-#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_VARARGS(args, i) PySequence_GetItem(args, i)
+#elif CYTHON_ASSUME_SAFE_MACROS
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#else
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
+#else
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
+#endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg) __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
@@ -1578,28 +1729,42 @@
 static CYTHON_INLINE PyObject* __Pyx_PyTuple_GetSlice(PyObject* src, Py_ssize_t start, Py_ssize_t stop);
 #else
 #define __Pyx_PyList_GetSlice(seq, start, stop)   PySequence_GetSlice(seq, start, stop)
 #define __Pyx_PyTuple_GetSlice(seq, start, stop)  PySequence_GetSlice(seq, start, stop)
 #endif
 
 /* AssertionsEnabled.proto */
-#define __Pyx_init_assertions_enabled()
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define __pyx_assertions_enabled() (1)
-#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
-  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
-#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  #define __Pyx_init_assertions_enabled()  (0)
+  #define __pyx_assertions_enabled()  (1)
+#elif CYTHON_COMPILING_IN_LIMITED_API  ||  (CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030C0000)
   static int __pyx_assertions_enabled_flag;
   #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
-  #undef __Pyx_init_assertions_enabled
-  static void __Pyx_init_assertions_enabled(void) {
-    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  static int __Pyx_init_assertions_enabled(void) {
+    PyObject *builtins, *debug, *debug_str;
+    int flag;
+    builtins = PyEval_GetBuiltins();
+    if (!builtins) goto bad;
+    debug_str = PyUnicode_FromStringAndSize("__debug__", 9);
+    if (!debug_str) goto bad;
+    debug = PyObject_GetItem(builtins, debug_str);
+    Py_DECREF(debug_str);
+    if (!debug) goto bad;
+    flag = PyObject_IsTrue(debug);
+    Py_DECREF(debug);
+    if (flag == -1) goto bad;
+    __pyx_assertions_enabled_flag = flag;
+    return 0;
+  bad:
+    __pyx_assertions_enabled_flag = 1;
+    return -1;
   }
 #else
-  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+  #define __Pyx_init_assertions_enabled()  (0)
+  #define __pyx_assertions_enabled()  (!Py_OptimizeFlag)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
@@ -1612,15 +1777,15 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if !CYTHON_VECTORCALL
 #if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
   #define __Pxy_PyFrame_Initialize_Offsets()
   #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
@@ -1673,16 +1838,26 @@
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* decode_bytes.proto */
 static CYTHON_INLINE PyObject* __Pyx_decode_bytes(
          PyObject* string, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
+    char* as_c_string;
+    Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+    as_c_string = PyBytes_AS_STRING(string);
+    size = PyBytes_GET_SIZE(string);
+#else
+    if (PyBytes_AsStringAndSize(string, &as_c_string, &size) < 0) {
+        return NULL;
+    }
+#endif
     return __Pyx_decode_c_bytes(
-        PyBytes_AS_STRING(string), PyBytes_GET_SIZE(string),
+        as_c_string, size,
         start, stop, encoding, errors, decode_func);
 }
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* PyObjectFormatSimple.proto */
@@ -1767,15 +1942,30 @@
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
 static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
 /* PyMethodNew.proto */
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    typesModule = PyImport_ImportModule("types");
+    if (!typesModule) return NULL;
+    methodType = PyObject_GetAttrString(typesModule, "MethodType");
+    Py_DECREF(typesModule);
+    if (!methodType) return NULL;
+    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
+    Py_DECREF(methodType);
+    return result;
+}
+#elif PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
     CYTHON_UNUSED_VAR(typ);
     if (!self)
         return __Pyx_NewRef(func);
     return PyMethod_New(func, self);
 }
 #else
@@ -1791,62 +1981,69 @@
 #define __Pyx_CyFunction_USED
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CYFUNCTION_COROUTINE     0x08
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_CyFunction_GetClassObj(f)\
       (((__pyx_CyFunctionObject *) (f))->func_classobj)
 #else
   #define __Pyx_CyFunction_GetClassObj(f)\
       ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
 #endif
 #define __Pyx_CyFunction_SetClassObj(f, classobj)\
     __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
 #define __Pyx_CyFunction_Defaults(type, f)\
     ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
 #define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
     ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
 typedef struct {
-#if PY_VERSION_HEX < 0x030900B1
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject_HEAD
+    PyObject *func;
+#elif PY_VERSION_HEX < 0x030900B1
     PyCFunctionObject func;
 #else
     PyCMethodObject func;
 #endif
 #if CYTHON_BACKPORT_VECTORCALL
     __pyx_vectorcallfunc func_vectorcall;
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_weakreflist;
 #endif
     PyObject *func_dict;
     PyObject *func_name;
     PyObject *func_qualname;
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -1982,15 +2179,16 @@
 #define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CStringEquals.proto */
 static CYTHON_INLINE int __Pyx_StrEq(const char *, const char *);
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
 /* Module declarations from "libc" */
@@ -2038,14 +2236,15 @@
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_types[] = "types";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_lead_n[] = "lead_n";
+static const char __pyx_k_n_loop[] = "n_loop";
 static const char __pyx_k_n_outs[] = "n_outs";
 static const char __pyx_k_n_read[] = "n_read";
 static const char __pyx_k_collect[] = "collect";
 static const char __pyx_k_fheader[] = "fheader";
 static const char __pyx_k_out_buf[] = "out_buf";
 static const char __pyx_k_fin_name[] = "fin_name";
 static const char __pyx_k_sub_lead[] = "sub_lead";
@@ -2069,25 +2268,26 @@
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_out_buf_size[] = "out_buf_size";
 static const char __pyx_k_custom_header[] = "custom_header";
 static const char __pyx_k_drained_fifos[] = "drained_fifos";
 static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_as_substring_in[] = " as substring in ";
+static const char __pyx_k_n_reopen_inputs[] = "n_reopen_inputs";
 static const char __pyx_k_header_broadcast[] = "header_broadcast";
 static const char __pyx_k_mrfifo_fast_loops[] = "mrfifo.fast_loops";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_header_detect_func[] = "header_detect_func";
 static const char __pyx_k_distribute_by_substr[] = "distribute_by_substr";
 static const char __pyx_k_mrfifo_fast_loops_pyx[] = "mrfifo/fast_loops.pyx";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast); /* proto */
 static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast); /* proto */
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header); /* proto */
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs); /* proto */
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2164,17 +2364,19 @@
   PyObject *__pyx_n_s_lead_n;
   PyObject *__pyx_n_s_line;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_mrfifo_fast_loops;
   PyObject *__pyx_kp_s_mrfifo_fast_loops_pyx;
   PyObject *__pyx_n_s_n;
   PyObject *__pyx_n_s_n_ins;
+  PyObject *__pyx_n_s_n_loop;
   PyObject *__pyx_n_s_n_out;
   PyObject *__pyx_n_s_n_outs;
   PyObject *__pyx_n_s_n_read;
+  PyObject *__pyx_n_s_n_reopen_inputs;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_out_buf;
   PyObject *__pyx_n_s_out_buf_size;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_stdin_buf;
   PyObject *__pyx_n_s_sub;
@@ -2280,17 +2482,19 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_lead_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_line);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_mrfifo_fast_loops);
   Py_CLEAR(clear_module_state->__pyx_kp_s_mrfifo_fast_loops_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_ins);
+  Py_CLEAR(clear_module_state->__pyx_n_s_n_loop);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_out);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_outs);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_read);
+  Py_CLEAR(clear_module_state->__pyx_n_s_n_reopen_inputs);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_out_buf);
   Py_CLEAR(clear_module_state->__pyx_n_s_out_buf_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_stdin_buf);
   Py_CLEAR(clear_module_state->__pyx_n_s_sub);
@@ -2374,17 +2578,19 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_lead_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_line);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_mrfifo_fast_loops);
   Py_VISIT(traverse_module_state->__pyx_kp_s_mrfifo_fast_loops_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_ins);
+  Py_VISIT(traverse_module_state->__pyx_n_s_n_loop);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_out);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_outs);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_read);
+  Py_VISIT(traverse_module_state->__pyx_n_s_n_reopen_inputs);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_out_buf);
   Py_VISIT(traverse_module_state->__pyx_n_s_out_buf_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_stdin_buf);
   Py_VISIT(traverse_module_state->__pyx_n_s_sub);
@@ -2486,17 +2692,19 @@
 #define __pyx_n_s_lead_n __pyx_mstate_global->__pyx_n_s_lead_n
 #define __pyx_n_s_line __pyx_mstate_global->__pyx_n_s_line
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_mrfifo_fast_loops __pyx_mstate_global->__pyx_n_s_mrfifo_fast_loops
 #define __pyx_kp_s_mrfifo_fast_loops_pyx __pyx_mstate_global->__pyx_kp_s_mrfifo_fast_loops_pyx
 #define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
 #define __pyx_n_s_n_ins __pyx_mstate_global->__pyx_n_s_n_ins
+#define __pyx_n_s_n_loop __pyx_mstate_global->__pyx_n_s_n_loop
 #define __pyx_n_s_n_out __pyx_mstate_global->__pyx_n_s_n_out
 #define __pyx_n_s_n_outs __pyx_mstate_global->__pyx_n_s_n_outs
 #define __pyx_n_s_n_read __pyx_mstate_global->__pyx_n_s_n_read
+#define __pyx_n_s_n_reopen_inputs __pyx_mstate_global->__pyx_n_s_n_reopen_inputs
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_out_buf __pyx_mstate_global->__pyx_n_s_out_buf
 #define __pyx_n_s_out_buf_size __pyx_mstate_global->__pyx_n_s_out_buf_size
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_stdin_buf __pyx_mstate_global->__pyx_n_s_stdin_buf
 #define __pyx_n_s_sub __pyx_mstate_global->__pyx_n_s_sub
@@ -2549,45 +2757,53 @@
   int __pyx_v_chunk_size;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_detect_func = 0;
   PyObject *__pyx_v_header_fifo = 0;
   PyObject *__pyx_v_header_broadcast = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[8] = {0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("distribute (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,0};
-    PyObject* values[8] = {0,0,0,0,0,0,0,0};
 
     /* "mrfifo/fast_loops.pyx":12
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",             # <<<<<<<<<<<<<<
  *                header_broadcast=False):
  * 
  */
-    values[5] = ((PyObject *)((PyObject *)Py_None));
-    values[6] = ((PyObject *)((PyObject*)__pyx_kp_u_));
+    values[5] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
+    values[6] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
 
     /* "mrfifo/fast_loops.pyx":13
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
  *                header_broadcast=False):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
-    values[7] = ((PyObject *)((PyObject *)Py_False));
+    values[7] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
@@ -2605,64 +2821,70 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fin_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fin_name)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 8, 1); __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_chunk_size);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_in_buf_size);
-          if (value) { values[3] = value; kw_args--; }
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_buf_size);
-          if (value) { values[4] = value; kw_args--; }
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_detect_func);
-          if (value) { values[5] = value; kw_args--; }
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_fifo);
-          if (value) { values[6] = value; kw_args--; }
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_broadcast);
-          if (value) { values[7] = value; kw_args--; }
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "distribute") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
       }
@@ -2703,18 +2925,26 @@
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x80000));
     }
     __pyx_v_header_detect_func = values[5];
     __pyx_v_header_fifo = values[6];
     __pyx_v_header_broadcast = values[7];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("distribute", 0, 2, 8, __pyx_nargs); __PYX_ERR(0, 10, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("mrfifo.fast_loops.distribute", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fin_name), (&PyUnicode_Type), 1, "fin_name", 1))) __PYX_ERR(0, 10, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_r = __pyx_pf_6mrfifo_10fast_loops_distribute(__pyx_self, __pyx_v_fin_name, __pyx_v_fifo_names, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_detect_func, __pyx_v_header_fifo, __pyx_v_header_broadcast);
@@ -2728,14 +2958,20 @@
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6mrfifo_10fast_loops_distribute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast) {
   size_t __pyx_v_i;
   size_t __pyx_v_j;
@@ -2844,15 +3080,15 @@
  *     cdef size_t n = 0
  *     cdef str line
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 23, __pyx_L1_error)
   }
-  __pyx_t_3 = PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_v_n_outs = __pyx_t_3;
 
   /* "mrfifo/fast_loops.pyx":24
  *     cdef size_t j = 0
  *     cdef size_t n_outs = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef str line
@@ -2964,24 +3200,26 @@
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 43, __pyx_L1_error)
     }
     __pyx_t_8 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
         __pyx_t_10 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
@@ -3027,24 +3265,26 @@
  * 
  *         while(True):
  */
       __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 50, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
           __pyx_t_10 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
@@ -3122,24 +3362,26 @@
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = __Pyx_decode_bytes(__pyx_t_9, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_INCREF(__pyx_v_header_detect_func);
       __pyx_t_9 = __pyx_v_header_detect_func; __pyx_t_11 = NULL;
       __pyx_t_10 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
           __pyx_t_10 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_t_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
@@ -3509,46 +3751,54 @@
   PyObject *__pyx_v_sub_lead = 0;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_detect_func = 0;
   PyObject *__pyx_v_header_fifo = 0;
   PyObject *__pyx_v_header_broadcast = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("distribute_by_substr (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fin_name,&__pyx_n_s_fifo_names,&__pyx_n_s_sub_lookup,&__pyx_n_s_sub_size,&__pyx_n_s_sub_lead,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_detect_func,&__pyx_n_s_header_fifo,&__pyx_n_s_header_broadcast,0};
-    PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
-    values[4] = ((PyObject*)((PyObject*)__pyx_kp_b_CB_Z));
+    values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_kp_b_CB_Z)));
 
     /* "mrfifo/fast_loops.pyx":104
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                          header_detect_func=None, header_fifo="",             # <<<<<<<<<<<<<<
  *                          header_broadcast=False):
  * 
  */
-    values[7] = ((PyObject *)((PyObject *)Py_None));
-    values[8] = ((PyObject *)((PyObject*)__pyx_kp_u_));
+    values[7] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
+    values[8] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
 
     /* "mrfifo/fast_loops.pyx":105
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                          header_detect_func=None, header_fifo="",
  *                          header_broadcast=False):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
-    values[9] = ((PyObject *)((PyObject *)Py_False));
+    values[9] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
@@ -3570,78 +3820,90 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fin_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fin_name)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 1); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_lookup)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_lookup)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 2); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_size)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_size)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, 3); __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sub_lead);
-          if (value) { values[4] = value; kw_args--; }
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_in_buf_size);
-          if (value) { values[5] = value; kw_args--; }
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_buf_size);
-          if (value) { values[6] = value; kw_args--; }
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_detect_func);
-          if (value) { values[7] = value; kw_args--; }
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_fifo);
-          if (value) { values[8] = value; kw_args--; }
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_broadcast);
-          if (value) { values[9] = value; kw_args--; }
+          if (value) { values[9] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "distribute_by_substr") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
       }
@@ -3682,18 +3944,26 @@
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x80000));
     }
     __pyx_v_header_detect_func = values[7];
     __pyx_v_header_fifo = values[8];
     __pyx_v_header_broadcast = values[9];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("distribute_by_substr", 0, 4, 10, __pyx_nargs); __PYX_ERR(0, 101, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("mrfifo.fast_loops.distribute_by_substr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fin_name), (&PyUnicode_Type), 1, "fin_name", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sub_lookup), (&PyDict_Type), 1, "sub_lookup", 1))) __PYX_ERR(0, 101, __pyx_L1_error)
@@ -3709,14 +3979,20 @@
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6mrfifo_10fast_loops_2distribute_by_substr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fin_name, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_sub_lookup, size_t __pyx_v_sub_size, PyObject *__pyx_v_sub_lead, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_detect_func, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_header_broadcast) {
   size_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
@@ -3833,15 +4109,15 @@
  *     cdef size_t n = 0
  *     cdef str line
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 116, __pyx_L1_error)
   }
-  __pyx_t_3 = PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 116, __pyx_L1_error)
   __pyx_v_n_outs = __pyx_t_3;
 
   /* "mrfifo/fast_loops.pyx":117
  * 
  *     cdef size_t n_outs = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef str line
@@ -3870,15 +4146,15 @@
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)
  *     cdef char* sub_match_c = NULL
  */
   if (unlikely(__pyx_v_sub_lead == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 121, __pyx_L1_error)
   }
-  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_sub_lead); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_GET_SIZE(__pyx_v_sub_lead); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 121, __pyx_L1_error)
   __pyx_v_lead_n = __pyx_t_3;
 
   /* "mrfifo/fast_loops.pyx":122
  *     cdef char* sub_lead_c = sub_lead
  *     cdef size_t lead_n = len(sub_lead)
  *     cdef char* sub_buffer = <char*>stdlib.malloc(sub_size)             # <<<<<<<<<<<<<<
  *     cdef char* sub_match_c = NULL
@@ -3999,24 +4275,26 @@
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 141, __pyx_L1_error)
     }
     __pyx_t_9 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = NULL;
     __pyx_t_11 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
         __pyx_t_11 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_utf_8};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
@@ -4062,24 +4340,26 @@
  * 
  *         while(True):
  */
       __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
           __pyx_t_11 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_utf_8};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
@@ -4157,24 +4437,26 @@
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = __Pyx_decode_bytes(__pyx_t_10, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_INCREF(__pyx_v_header_detect_func);
       __pyx_t_10 = __pyx_v_header_detect_func; __pyx_t_12 = NULL;
       __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_10, function);
           __pyx_t_11 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_9};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
@@ -4628,15 +4910,15 @@
 }
 
 /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6mrfifo_10fast_loops_5collect(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4654,40 +4936,51 @@
   PyObject *__pyx_v_fifo_names = 0;
   PyObject *__pyx_v_fout_name = 0;
   int __pyx_v_chunk_size;
   size_t __pyx_v_in_buf_size;
   size_t __pyx_v_out_buf_size;
   PyObject *__pyx_v_header_fifo = 0;
   PyObject *__pyx_v_custom_header = 0;
+  int __pyx_v_n_reopen_inputs;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[8] = {0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("collect (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fifo_names,&__pyx_n_s_fout_name,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_fifo,&__pyx_n_s_custom_header,0};
-    PyObject* values[7] = {0,0,0,0,0,0,0};
-    values[5] = ((PyObject *)((PyObject*)__pyx_kp_u_));
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fifo_names,&__pyx_n_s_fout_name,&__pyx_n_s_chunk_size,&__pyx_n_s_in_buf_size,&__pyx_n_s_out_buf_size,&__pyx_n_s_header_fifo,&__pyx_n_s_custom_header,&__pyx_n_s_n_reopen_inputs,0};
+    values[5] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_kp_u_)));
 
     /* "mrfifo/fast_loops.pyx":212
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):             # <<<<<<<<<<<<<<
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):             # <<<<<<<<<<<<<<
  * 
  *     if header_fifo == 0:
  */
-    values[6] = ((PyObject *)((PyObject *)Py_None));
+    values[6] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
@@ -4700,66 +4993,81 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fifo_names)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fout_name)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fout_name)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 7, 1); __PYX_ERR(0, 210, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 8, 1); __PYX_ERR(0, 210, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_chunk_size);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_in_buf_size);
-          if (value) { values[3] = value; kw_args--; }
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_out_buf_size);
-          if (value) { values[4] = value; kw_args--; }
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_header_fifo);
-          if (value) { values[5] = value; kw_args--; }
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_custom_header);
-          if (value) { values[6] = value; kw_args--; }
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_reopen_inputs);
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "collect") < 0)) __PYX_ERR(0, 210, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
         case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
@@ -4787,84 +5095,107 @@
     if (values[4]) {
       __pyx_v_out_buf_size = __Pyx_PyInt_As_size_t(values[4]); if (unlikely((__pyx_v_out_buf_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L3_error)
     } else {
       __pyx_v_out_buf_size = ((size_t)((size_t)0x100000));
     }
     __pyx_v_header_fifo = values[5];
     __pyx_v_custom_header = values[6];
+    if (values[7]) {
+      __pyx_v_n_reopen_inputs = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_n_reopen_inputs == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L3_error)
+    } else {
+      __pyx_v_n_reopen_inputs = ((int)((int)1));
+    }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 7, __pyx_nargs); __PYX_ERR(0, 210, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("collect", 0, 2, 8, __pyx_nargs); __PYX_ERR(0, 210, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("mrfifo.fast_loops.collect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fifo_names), (&PyList_Type), 1, "fifo_names", 1))) __PYX_ERR(0, 210, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_fout_name), (&PyUnicode_Type), 1, "fout_name", 1))) __PYX_ERR(0, 210, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_4collect(__pyx_self, __pyx_v_fifo_names, __pyx_v_fout_name, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_fifo, __pyx_v_custom_header);
+  __pyx_r = __pyx_pf_6mrfifo_10fast_loops_4collect(__pyx_self, __pyx_v_fifo_names, __pyx_v_fout_name, __pyx_v_chunk_size, __pyx_v_in_buf_size, __pyx_v_out_buf_size, __pyx_v_header_fifo, __pyx_v_custom_header, __pyx_v_n_reopen_inputs);
 
   /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header) {
+static PyObject *__pyx_pf_6mrfifo_10fast_loops_4collect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_fifo_names, PyObject *__pyx_v_fout_name, int __pyx_v_chunk_size, size_t __pyx_v_in_buf_size, size_t __pyx_v_out_buf_size, PyObject *__pyx_v_header_fifo, PyObject *__pyx_v_custom_header, int __pyx_v_n_reopen_inputs) {
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_v_k;
   size_t __pyx_v_n_ins;
   size_t __pyx_v_n;
   size_t __pyx_v_n_out;
   char *__pyx_v_buffer;
   Py_ssize_t __pyx_v_n_read;
   char *__pyx_v_fifo_buffers[0x80];
   CYTHON_UNUSED PyObject *__pyx_v_sys = NULL;
   FILE *__pyx_v_fifos[0x80];
   int __pyx_v_fifo_closed[0x80];
   size_t __pyx_v_drained_fifos;
+  CYTHON_UNUSED int __pyx_v_n_loop;
   char *__pyx_v_out_buf;
   FILE *__pyx_v_fout;
   PyObject *__pyx_v_header_bytes = NULL;
   FILE *__pyx_v_fheader;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
-  size_t __pyx_t_4;
-  size_t __pyx_t_5;
-  int __pyx_t_6;
-  char const *__pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  char const *__pyx_t_10;
-  int __pyx_t_11;
+  char const *__pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  char const *__pyx_t_8;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  size_t __pyx_t_11;
+  size_t __pyx_t_12;
+  int __pyx_t_13;
+  int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("collect", 0);
   __Pyx_INCREF(__pyx_v_fifo_names);
   __Pyx_INCREF(__pyx_v_header_fifo);
 
   /* "mrfifo/fast_loops.pyx":214
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data
  *         # and the other as round-robin inputs as usual
  */
   __pyx_t_1 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_header_fifo, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 214, __pyx_L1_error)
   if (__pyx_t_1) {
@@ -4898,15 +5229,15 @@
     }
     __pyx_t_2 = __Pyx_PyList_GetSlice(__pyx_v_fifo_names, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_fifo_names, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
     /* "mrfifo/fast_loops.pyx":214
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  * 
  *     if header_fifo == 0:             # <<<<<<<<<<<<<<
  *         # special mode: use the first fifo name for header data
  *         # and the other as round-robin inputs as usual
  */
   }
 
@@ -4944,15 +5275,15 @@
  *     cdef size_t n = 0
  *     cdef size_t n_out = 0
  */
   if (unlikely(__pyx_v_fifo_names == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(0, 223, __pyx_L1_error)
   }
-  __pyx_t_3 = PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_fifo_names); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
   __pyx_v_n_ins = __pyx_t_3;
 
   /* "mrfifo/fast_loops.pyx":224
  *     cdef int k = 0
  *     cdef size_t n_ins = len(fifo_names)
  *     cdef size_t n = 0             # <<<<<<<<<<<<<<
  *     cdef size_t n_out = 0
@@ -4982,560 +5313,597 @@
   __pyx_t_2 = 0;
 
   /* "mrfifo/fast_loops.pyx":235
  *     import sys
  *     # sys.stderr.write(f"collecting from {fifo_names} into {fout_name}")
  *     assert n <= 128             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fifos[128]
- *     cdef bint fifo_closed[128]
+ *     cdef bint[128] fifo_closed
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_n <= 0x80);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
       __PYX_ERR(0, 235, __pyx_L1_error)
     }
   }
   #else
   if ((1)); else __PYX_ERR(0, 235, __pyx_L1_error)
   #endif
 
-  /* "mrfifo/fast_loops.pyx":238
- *     cdef stdio.FILE *fifos[128]
- *     cdef bint fifo_closed[128]
- *     for i in range(n_ins):             # <<<<<<<<<<<<<<
- *         fifo_closed[i] = False
+  /* "mrfifo/fast_loops.pyx":239
+ *     cdef bint[128] fifo_closed
  * 
- */
-  __pyx_t_4 = __pyx_v_n_ins;
-  __pyx_t_5 = __pyx_t_4;
-  for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-    __pyx_v_i = __pyx_t_6;
-
-    /* "mrfifo/fast_loops.pyx":239
- *     cdef bint fifo_closed[128]
- *     for i in range(n_ins):
- *         fifo_closed[i] = False             # <<<<<<<<<<<<<<
+ *     cdef size_t drained_fifos = 0             # <<<<<<<<<<<<<<
+ *     cdef int n_loop = 0
  * 
- *     cdef size_t drained_fifos = 0
  */
-    (__pyx_v_fifo_closed[__pyx_v_i]) = 0;
-  }
+  __pyx_v_drained_fifos = 0;
 
-  /* "mrfifo/fast_loops.pyx":241
- *         fifo_closed[i] = False
+  /* "mrfifo/fast_loops.pyx":240
  * 
- *     cdef size_t drained_fifos = 0             # <<<<<<<<<<<<<<
+ *     cdef size_t drained_fifos = 0
+ *     cdef int n_loop = 0             # <<<<<<<<<<<<<<
  * 
  *     # line buffer
  */
-  __pyx_v_drained_fifos = 0;
+  __pyx_v_n_loop = 0;
 
-  /* "mrfifo/fast_loops.pyx":244
+  /* "mrfifo/fast_loops.pyx":243
  * 
  *     # line buffer
  *     buffer = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  */
   __pyx_v_buffer = ((char *)malloc(__pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":246
+  /* "mrfifo/fast_loops.pyx":245
  *     buffer = <char*>stdlib.malloc(out_buf_size)
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)             # <<<<<<<<<<<<<<
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)
  */
   __pyx_v_out_buf = ((char *)malloc(__pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":247
+  /* "mrfifo/fast_loops.pyx":246
  *     # prepare output file and buffer
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')             # <<<<<<<<<<<<<<
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)
  * 
  */
   if (unlikely(__pyx_v_fout_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 247, __pyx_L1_error)
+    __PYX_ERR(0, 246, __pyx_L1_error)
   }
-  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fout_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_AsUTF8String(__pyx_v_fout_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
-  __pyx_v_fout = fopen(__pyx_t_7, ((char const *)"w"));
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_v_fout = fopen(__pyx_t_4, ((char const *)"w"));
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mrfifo/fast_loops.pyx":248
+  /* "mrfifo/fast_loops.pyx":247
  *     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
  *     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')
  *     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)             # <<<<<<<<<<<<<<
  * 
  *     # cdef char * line_bytes
  */
   (void)(setvbuf(__pyx_v_fout, __pyx_v_out_buf, _IOFBF, __pyx_v_out_buf_size));
 
-  /* "mrfifo/fast_loops.pyx":251
+  /* "mrfifo/fast_loops.pyx":250
  * 
  *     # cdef char * line_bytes
  *     if custom_header is not None:             # <<<<<<<<<<<<<<
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  */
   __pyx_t_1 = (__pyx_v_custom_header != Py_None);
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":253
+    /* "mrfifo/fast_loops.pyx":252
  *     if custom_header is not None:
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')             # <<<<<<<<<<<<<<
  *         stdio.fwrite(<const char*>header_bytes, len(header_bytes), 1, fout)
  * 
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_custom_header, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = NULL;
-    __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_9);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_custom_header, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    __pyx_t_7 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_6 = 1;
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
       }
     }
+    #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 253, __pyx_L1_error)
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_header_bytes = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":254
+    /* "mrfifo/fast_loops.pyx":253
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  *         stdio.fwrite(<const char*>header_bytes, len(header_bytes), 1, fout)             # <<<<<<<<<<<<<<
  * 
  *     cdef stdio.FILE *fheader
  */
-    __pyx_t_10 = __Pyx_PyObject_AsString(__pyx_v_header_bytes); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 254, __pyx_L1_error)
-    __pyx_t_3 = PyObject_Length(__pyx_v_header_bytes); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 254, __pyx_L1_error)
-    (void)(fwrite(((char const *)__pyx_t_10), __pyx_t_3, 1, __pyx_v_fout));
+    __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_header_bytes); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_3 = PyObject_Length(__pyx_v_header_bytes); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 253, __pyx_L1_error)
+    (void)(fwrite(((char const *)__pyx_t_8), __pyx_t_3, 1, __pyx_v_fout));
 
-    /* "mrfifo/fast_loops.pyx":251
+    /* "mrfifo/fast_loops.pyx":250
  * 
  *     # cdef char * line_bytes
  *     if custom_header is not None:             # <<<<<<<<<<<<<<
  *         # we have a custom header string, write this first!
  *         header_bytes = custom_header.encode('utf-8')
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":257
+  /* "mrfifo/fast_loops.pyx":256
  * 
  *     cdef stdio.FILE *fheader
  *     if header_fifo:             # <<<<<<<<<<<<<<
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_header_fifo); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 256, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mrfifo/fast_loops.pyx":260
+    /* "mrfifo/fast_loops.pyx":259
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 260, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = NULL;
-    __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_9);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_header_fifo, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    __pyx_t_7 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_6 = 1;
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
       }
     }
+    #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 260, __pyx_L1_error)
-    __pyx_v_fheader = fopen(__pyx_t_7, ((char const *)"r"));
+    __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_v_fheader = fopen(__pyx_t_4, ((char const *)"r"));
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":261
+    /* "mrfifo/fast_loops.pyx":260
  *         # stuff first and write it to the output
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')
  *         while(True):             # <<<<<<<<<<<<<<
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:
  */
     while (1) {
 
-      /* "mrfifo/fast_loops.pyx":262
+      /* "mrfifo/fast_loops.pyx":261
  *         fheader = stdio.fopen(header_fifo.encode('utf-8'), 'r')
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)             # <<<<<<<<<<<<<<
  *             if n_read <= 0:
  *                 break
  */
       __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_out_buf_size), __pyx_v_fheader);
 
-      /* "mrfifo/fast_loops.pyx":263
+      /* "mrfifo/fast_loops.pyx":262
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       __pyx_t_1 = (__pyx_v_n_read <= 0);
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":264
+        /* "mrfifo/fast_loops.pyx":263
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             stdio.fwrite(buffer, n_read, 1, fout)
  */
-        goto __pyx_L9_break;
+        goto __pyx_L7_break;
 
-        /* "mrfifo/fast_loops.pyx":263
+        /* "mrfifo/fast_loops.pyx":262
  *         while(True):
  *             n_read = stdio.getline(&buffer, &out_buf_size, fheader)
  *             if n_read <= 0:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "mrfifo/fast_loops.pyx":266
+      /* "mrfifo/fast_loops.pyx":265
  *                 break
  * 
  *             stdio.fwrite(buffer, n_read, 1, fout)             # <<<<<<<<<<<<<<
  * 
  *         # all header data has been read! close this fifo's reading end
  */
       (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fout));
     }
-    __pyx_L9_break:;
+    __pyx_L7_break:;
 
-    /* "mrfifo/fast_loops.pyx":269
+    /* "mrfifo/fast_loops.pyx":268
  * 
  *         # all header data has been read! close this fifo's reading end
  *         stdio.fclose(fheader)             # <<<<<<<<<<<<<<
  * 
- *     # now prepare input from all the demuxed fifos
+ *     for n_loop in range(n_reopen_inputs):
  */
     (void)(fclose(__pyx_v_fheader));
 
-    /* "mrfifo/fast_loops.pyx":257
+    /* "mrfifo/fast_loops.pyx":256
  * 
  *     cdef stdio.FILE *fheader
  *     if header_fifo:             # <<<<<<<<<<<<<<
  *         # we have some special, un-multiplexed header data. Read this
  *         # stuff first and write it to the output
  */
   }
 
-  /* "mrfifo/fast_loops.pyx":272
+  /* "mrfifo/fast_loops.pyx":270
+ *         stdio.fclose(fheader)
  * 
- *     # now prepare input from all the demuxed fifos
- *     for i in range(n_ins):             # <<<<<<<<<<<<<<
- *         fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
- *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
- */
-  __pyx_t_4 = __pyx_v_n_ins;
-  __pyx_t_5 = __pyx_t_4;
-  for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-    __pyx_v_i = __pyx_t_6;
+ *     for n_loop in range(n_reopen_inputs):             # <<<<<<<<<<<<<<
+ *         #print(f"opening the input fifos for the {n_loop}th time: {fifo_names}")
+ *         # now prepare input from all the demuxed fifos
+ */
+  __pyx_t_7 = __pyx_v_n_reopen_inputs;
+  __pyx_t_9 = __pyx_t_7;
+  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+    __pyx_v_n_loop = __pyx_t_10;
 
     /* "mrfifo/fast_loops.pyx":273
- *     # now prepare input from all the demuxed fifos
- *     for i in range(n_ins):
- *         fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
- *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
- *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
- */
-    (__pyx_v_fifo_buffers[__pyx_v_i]) = ((char *)malloc(__pyx_v_in_buf_size));
-
-    /* "mrfifo/fast_loops.pyx":274
- *     for i in range(n_ins):
- *         fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
- *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
- *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
- * 
- */
-    if (unlikely(__pyx_v_fifo_names == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 274, __pyx_L1_error)
-    }
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 274, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = NULL;
-    __pyx_t_11 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-        __Pyx_INCREF(__pyx_t_9);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_11 = 1;
+ *         #print(f"opening the input fifos for the {n_loop}th time: {fifo_names}")
+ *         # now prepare input from all the demuxed fifos
+ *         for i in range(n_ins):             # <<<<<<<<<<<<<<
+ *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
+ *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
+ */
+    __pyx_t_11 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_11;
+    for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
+      __pyx_v_i = __pyx_t_13;
+
+      /* "mrfifo/fast_loops.pyx":274
+ *         # now prepare input from all the demuxed fifos
+ *         for i in range(n_ins):
+ *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)             # <<<<<<<<<<<<<<
+ *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
+ *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
+ */
+      (__pyx_v_fifo_buffers[__pyx_v_i]) = ((char *)malloc(__pyx_v_in_buf_size));
+
+      /* "mrfifo/fast_loops.pyx":275
+ *         for i in range(n_ins):
+ *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
+ *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')             # <<<<<<<<<<<<<<
+ *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
+ * 
+ */
+      if (unlikely(__pyx_v_fifo_names == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+        __PYX_ERR(0, 275, __pyx_L1_error)
       }
-    }
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_kp_u_utf_8};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    }
-    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 274, __pyx_L1_error)
-    (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_7, ((char const *)"r"));
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_fifo_names, __pyx_v_i), __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = NULL;
+      __pyx_t_14 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_14 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
+        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_14, 1+__pyx_t_14);
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
+      (__pyx_v_fifos[__pyx_v_i]) = fopen(__pyx_t_4, ((char const *)"r"));
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "mrfifo/fast_loops.pyx":275
- *         fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
- *         fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
- *         stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)             # <<<<<<<<<<<<<<
+      /* "mrfifo/fast_loops.pyx":276
+ *             fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
+ *             fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
+ *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)             # <<<<<<<<<<<<<<
  * 
- *     # main mutiplexing loop
+ *         drained_fifos = 0
  */
-    (void)(setvbuf((__pyx_v_fifos[__pyx_v_i]), (__pyx_v_fifo_buffers[__pyx_v_i]), _IOFBF, __pyx_v_in_buf_size));
-  }
+      (void)(setvbuf((__pyx_v_fifos[__pyx_v_i]), (__pyx_v_fifo_buffers[__pyx_v_i]), _IOFBF, __pyx_v_in_buf_size));
+    }
 
-  /* "mrfifo/fast_loops.pyx":278
+    /* "mrfifo/fast_loops.pyx":278
+ *             stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
  * 
- *     # main mutiplexing loop
- *     while(drained_fifos < n_ins):             # <<<<<<<<<<<<<<
- *         j = n // chunk_size
- *         k = j % n_ins # index of fifo
+ *         drained_fifos = 0             # <<<<<<<<<<<<<<
+ *         for i in range(n_ins):
+ *             fifo_closed[i] = False
  */
-  while (1) {
-    __pyx_t_1 = (__pyx_v_drained_fifos < __pyx_v_n_ins);
-    if (!__pyx_t_1) break;
+    __pyx_v_drained_fifos = 0;
 
     /* "mrfifo/fast_loops.pyx":279
- *     # main mutiplexing loop
- *     while(drained_fifos < n_ins):
- *         j = n // chunk_size             # <<<<<<<<<<<<<<
- *         k = j % n_ins # index of fifo
- *         if not fifo_closed[k]:
- */
-    __pyx_v_j = (__pyx_v_n / __pyx_v_chunk_size);
-
-    /* "mrfifo/fast_loops.pyx":280
- *     while(drained_fifos < n_ins):
- *         j = n // chunk_size
- *         k = j % n_ins # index of fifo             # <<<<<<<<<<<<<<
- *         if not fifo_closed[k]:
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ * 
+ *         drained_fifos = 0
+ *         for i in range(n_ins):             # <<<<<<<<<<<<<<
+ *             fifo_closed[i] = False
+ * 
  */
-    __pyx_v_k = (__pyx_v_j % __pyx_v_n_ins);
+    __pyx_t_11 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_11;
+    for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
+      __pyx_v_i = __pyx_t_13;
 
-    /* "mrfifo/fast_loops.pyx":281
- *         j = n // chunk_size
- *         k = j % n_ins # index of fifo
- *         if not fifo_closed[k]:             # <<<<<<<<<<<<<<
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
+      /* "mrfifo/fast_loops.pyx":280
+ *         drained_fifos = 0
+ *         for i in range(n_ins):
+ *             fifo_closed[i] = False             # <<<<<<<<<<<<<<
+ * 
+ *         # main mutiplexing loop
  */
-    __pyx_t_1 = (!(__pyx_v_fifo_closed[__pyx_v_k]));
-    if (__pyx_t_1) {
+      (__pyx_v_fifo_closed[__pyx_v_i]) = 0;
+    }
 
-      /* "mrfifo/fast_loops.pyx":283
- *         if not fifo_closed[k]:
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])             # <<<<<<<<<<<<<<
- *             if n_read <= 0:
- *                 fifo_closed[k] = True
+    /* "mrfifo/fast_loops.pyx":283
+ * 
+ *         # main mutiplexing loop
+ *         while(drained_fifos < n_ins):             # <<<<<<<<<<<<<<
+ *             j = n // chunk_size
+ *             k = j % n_ins # index of fifo
  */
-      __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_out_buf_size), (__pyx_v_fifos[__pyx_v_k]));
+    while (1) {
+      __pyx_t_1 = (__pyx_v_drained_fifos < __pyx_v_n_ins);
+      if (!__pyx_t_1) break;
 
       /* "mrfifo/fast_loops.pyx":284
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
- *             if n_read <= 0:             # <<<<<<<<<<<<<<
- *                 fifo_closed[k] = True
- *                 drained_fifos += 1
+ *         # main mutiplexing loop
+ *         while(drained_fifos < n_ins):
+ *             j = n // chunk_size             # <<<<<<<<<<<<<<
+ *             k = j % n_ins # index of fifo
+ *             if not fifo_closed[k]:
+ */
+      __pyx_v_j = (__pyx_v_n / __pyx_v_chunk_size);
+
+      /* "mrfifo/fast_loops.pyx":285
+ *         while(drained_fifos < n_ins):
+ *             j = n // chunk_size
+ *             k = j % n_ins # index of fifo             # <<<<<<<<<<<<<<
+ *             if not fifo_closed[k]:
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ */
+      __pyx_v_k = (__pyx_v_j % __pyx_v_n_ins);
+
+      /* "mrfifo/fast_loops.pyx":286
+ *             j = n // chunk_size
+ *             k = j % n_ins # index of fifo
+ *             if not fifo_closed[k]:             # <<<<<<<<<<<<<<
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  */
-      __pyx_t_1 = (__pyx_v_n_read <= 0);
+      __pyx_t_1 = (!(__pyx_v_fifo_closed[__pyx_v_k]));
       if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":285
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
- *             if n_read <= 0:
- *                 fifo_closed[k] = True             # <<<<<<<<<<<<<<
- *                 drained_fifos += 1
- *             else:
+        /* "mrfifo/fast_loops.pyx":288
+ *             if not fifo_closed[k]:
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])             # <<<<<<<<<<<<<<
+ *                 if n_read <= 0:
+ *                     fifo_closed[k] = True
+ */
+        __pyx_v_n_read = getline((&__pyx_v_buffer), (&__pyx_v_out_buf_size), (__pyx_v_fifos[__pyx_v_k]));
+
+        /* "mrfifo/fast_loops.pyx":289
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
+ *                 if n_read <= 0:             # <<<<<<<<<<<<<<
+ *                     fifo_closed[k] = True
+ *                     drained_fifos += 1
  */
-        (__pyx_v_fifo_closed[__pyx_v_k]) = 1;
+        __pyx_t_1 = (__pyx_v_n_read <= 0);
+        if (__pyx_t_1) {
 
-        /* "mrfifo/fast_loops.pyx":286
- *             if n_read <= 0:
- *                 fifo_closed[k] = True
- *                 drained_fifos += 1             # <<<<<<<<<<<<<<
- *             else:
- *                 # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
+          /* "mrfifo/fast_loops.pyx":290
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
+ *                 if n_read <= 0:
+ *                     fifo_closed[k] = True             # <<<<<<<<<<<<<<
+ *                     drained_fifos += 1
+ *                 else:
+ */
+          (__pyx_v_fifo_closed[__pyx_v_k]) = 1;
+
+          /* "mrfifo/fast_loops.pyx":291
+ *                 if n_read <= 0:
+ *                     fifo_closed[k] = True
+ *                     drained_fifos += 1             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
+ */
+          __pyx_v_drained_fifos = (__pyx_v_drained_fifos + 1);
+
+          /* "mrfifo/fast_loops.pyx":289
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
+ *                 if n_read <= 0:             # <<<<<<<<<<<<<<
+ *                     fifo_closed[k] = True
+ *                     drained_fifos += 1
+ */
+          goto __pyx_L18;
+        }
+
+        /* "mrfifo/fast_loops.pyx":294
+ *                 else:
+ *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
+ *                     stdio.fwrite(buffer, n_read, 1, fout)             # <<<<<<<<<<<<<<
+ *                     n_out += 1
+ *             n += 1
+ */
+        /*else*/ {
+          (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fout));
+
+          /* "mrfifo/fast_loops.pyx":295
+ *                     # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
+ *                     stdio.fwrite(buffer, n_read, 1, fout)
+ *                     n_out += 1             # <<<<<<<<<<<<<<
+ *             n += 1
+ * 
  */
-        __pyx_v_drained_fifos = (__pyx_v_drained_fifos + 1);
+          __pyx_v_n_out = (__pyx_v_n_out + 1);
+        }
+        __pyx_L18:;
 
-        /* "mrfifo/fast_loops.pyx":284
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
- *             if n_read <= 0:             # <<<<<<<<<<<<<<
- *                 fifo_closed[k] = True
- *                 drained_fifos += 1
+        /* "mrfifo/fast_loops.pyx":286
+ *             j = n // chunk_size
+ *             k = j % n_ins # index of fifo
+ *             if not fifo_closed[k]:             # <<<<<<<<<<<<<<
+ *                 # print(f"collection wants to read from {fifo_names[k]}. blocking")
+ *                 n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
  */
-        goto __pyx_L16;
       }
 
-      /* "mrfifo/fast_loops.pyx":289
- *             else:
- *                 # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
- *                 stdio.fwrite(buffer, n_read, 1, fout)             # <<<<<<<<<<<<<<
- *                 n_out += 1
- *         n += 1
- */
-      /*else*/ {
-        (void)(fwrite(__pyx_v_buffer, __pyx_v_n_read, 1, __pyx_v_fout));
-
-        /* "mrfifo/fast_loops.pyx":290
- *                 # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
- *                 stdio.fwrite(buffer, n_read, 1, fout)
- *                 n_out += 1             # <<<<<<<<<<<<<<
- *         n += 1
+      /* "mrfifo/fast_loops.pyx":296
+ *                     stdio.fwrite(buffer, n_read, 1, fout)
+ *                     n_out += 1
+ *             n += 1             # <<<<<<<<<<<<<<
  * 
+ *         for i in range(n_ins):
  */
-        __pyx_v_n_out = (__pyx_v_n_out + 1);
-      }
-      __pyx_L16:;
-
-      /* "mrfifo/fast_loops.pyx":281
- *         j = n // chunk_size
- *         k = j % n_ins # index of fifo
- *         if not fifo_closed[k]:             # <<<<<<<<<<<<<<
- *             # print(f"collection wants to read from {fifo_names[k]}. blocking")
- *             n_read = stdio.getline(&buffer, &out_buf_size, fifos[k])
- */
+      __pyx_v_n = (__pyx_v_n + 1);
     }
 
-    /* "mrfifo/fast_loops.pyx":291
- *                 stdio.fwrite(buffer, n_read, 1, fout)
- *                 n_out += 1
- *         n += 1             # <<<<<<<<<<<<<<
- * 
- *     for i in range(n_ins):
- */
-    __pyx_v_n = (__pyx_v_n + 1);
-  }
-
-  /* "mrfifo/fast_loops.pyx":293
- *         n += 1
+    /* "mrfifo/fast_loops.pyx":298
+ *             n += 1
  * 
- *     for i in range(n_ins):             # <<<<<<<<<<<<<<
- *         stdio.fclose(fifos[i])
- *         stdlib.free(fifo_buffers[i])
+ *         for i in range(n_ins):             # <<<<<<<<<<<<<<
+ *             stdio.fclose(fifos[i])
+ *             stdlib.free(fifo_buffers[i])
  */
-  __pyx_t_4 = __pyx_v_n_ins;
-  __pyx_t_5 = __pyx_t_4;
-  for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-    __pyx_v_i = __pyx_t_6;
+    __pyx_t_11 = __pyx_v_n_ins;
+    __pyx_t_12 = __pyx_t_11;
+    for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
+      __pyx_v_i = __pyx_t_13;
 
-    /* "mrfifo/fast_loops.pyx":294
+      /* "mrfifo/fast_loops.pyx":299
  * 
- *     for i in range(n_ins):
- *         stdio.fclose(fifos[i])             # <<<<<<<<<<<<<<
- *         stdlib.free(fifo_buffers[i])
+ *         for i in range(n_ins):
+ *             stdio.fclose(fifos[i])             # <<<<<<<<<<<<<<
+ *             stdlib.free(fifo_buffers[i])
  * 
  */
-    (void)(fclose((__pyx_v_fifos[__pyx_v_i])));
+      (void)(fclose((__pyx_v_fifos[__pyx_v_i])));
 
-    /* "mrfifo/fast_loops.pyx":295
- *     for i in range(n_ins):
- *         stdio.fclose(fifos[i])
- *         stdlib.free(fifo_buffers[i])             # <<<<<<<<<<<<<<
+      /* "mrfifo/fast_loops.pyx":300
+ *         for i in range(n_ins):
+ *             stdio.fclose(fifos[i])
+ *             stdlib.free(fifo_buffers[i])             # <<<<<<<<<<<<<<
  * 
  *     # free the line buffer, close the output, and free the output buffer
  */
-    free((__pyx_v_fifo_buffers[__pyx_v_i]));
+      free((__pyx_v_fifo_buffers[__pyx_v_i]));
+    }
   }
 
-  /* "mrfifo/fast_loops.pyx":298
+  /* "mrfifo/fast_loops.pyx":303
  * 
  *     # free the line buffer, close the output, and free the output buffer
  *     stdlib.free(buffer)             # <<<<<<<<<<<<<<
  *     stdio.fclose(fout)
  *     stdlib.free(out_buf)
  */
   free(__pyx_v_buffer);
 
-  /* "mrfifo/fast_loops.pyx":299
+  /* "mrfifo/fast_loops.pyx":304
  *     # free the line buffer, close the output, and free the output buffer
  *     stdlib.free(buffer)
  *     stdio.fclose(fout)             # <<<<<<<<<<<<<<
  *     stdlib.free(out_buf)
  * 
  */
   (void)(fclose(__pyx_v_fout));
 
-  /* "mrfifo/fast_loops.pyx":300
+  /* "mrfifo/fast_loops.pyx":305
  *     stdlib.free(buffer)
  *     stdio.fclose(fout)
  *     stdlib.free(out_buf)             # <<<<<<<<<<<<<<
  * 
  *     return n_out # total number of multiplexed lines (excluding header)
  */
   free(__pyx_v_out_buf);
 
-  /* "mrfifo/fast_loops.pyx":302
+  /* "mrfifo/fast_loops.pyx":307
  *     stdlib.free(out_buf)
  * 
  *     return n_out # total number of multiplexed lines (excluding header)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n_out); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("mrfifo.fast_loops.collect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_sys);
   __Pyx_XDECREF(__pyx_v_header_bytes);
   __Pyx_XDECREF(__pyx_v_fifo_names);
   __Pyx_XDECREF(__pyx_v_header_fifo);
@@ -5548,14 +5916,16 @@
   {0, 0, 0, 0}
 };
 
 static int __pyx_import_star_set(PyObject *o, PyObject* py_name, char *name) {
   static const char* internal_type_names[] = {
     "__pyx_ctuple_char__ptr",
     "__pyx_ctuple_char__ptr_struct",
+    "__pyx_ctuple_int",
+    "__pyx_ctuple_int_struct",
     "__pyx_ctuple_size_t",
     "__pyx_ctuple_size_t_struct",
     0
   };
   const char** type_name = internal_type_names;
   while (*type_name) {
     if (__Pyx_StrEq(name, *type_name)) {
@@ -5734,17 +6104,19 @@
     {&__pyx_n_s_lead_n, __pyx_k_lead_n, sizeof(__pyx_k_lead_n), 0, 0, 1, 1},
     {&__pyx_n_s_line, __pyx_k_line, sizeof(__pyx_k_line), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_mrfifo_fast_loops, __pyx_k_mrfifo_fast_loops, sizeof(__pyx_k_mrfifo_fast_loops), 0, 0, 1, 1},
     {&__pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_k_mrfifo_fast_loops_pyx, sizeof(__pyx_k_mrfifo_fast_loops_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
     {&__pyx_n_s_n_ins, __pyx_k_n_ins, sizeof(__pyx_k_n_ins), 0, 0, 1, 1},
+    {&__pyx_n_s_n_loop, __pyx_k_n_loop, sizeof(__pyx_k_n_loop), 0, 0, 1, 1},
     {&__pyx_n_s_n_out, __pyx_k_n_out, sizeof(__pyx_k_n_out), 0, 0, 1, 1},
     {&__pyx_n_s_n_outs, __pyx_k_n_outs, sizeof(__pyx_k_n_outs), 0, 0, 1, 1},
     {&__pyx_n_s_n_read, __pyx_k_n_read, sizeof(__pyx_k_n_read), 0, 0, 1, 1},
+    {&__pyx_n_s_n_reopen_inputs, __pyx_k_n_reopen_inputs, sizeof(__pyx_k_n_reopen_inputs), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_out_buf, __pyx_k_out_buf, sizeof(__pyx_k_out_buf), 0, 0, 1, 1},
     {&__pyx_n_s_out_buf_size, __pyx_k_out_buf_size, sizeof(__pyx_k_out_buf_size), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_stdin_buf, __pyx_k_stdin_buf, sizeof(__pyx_k_stdin_buf), 0, 0, 1, 1},
     {&__pyx_n_s_sub, __pyx_k_sub, sizeof(__pyx_k_sub), 0, 0, 1, 1},
@@ -5802,20 +6174,20 @@
   __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(10, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_distribute_by_substr, 101, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 101, __pyx_L1_error)
 
   /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
-  __pyx_tuple__7 = PyTuple_Pack(25, __pyx_n_s_fifo_names, __pyx_n_s_fout_name, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_fifo, __pyx_n_s_custom_header, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_n_ins, __pyx_n_s_n, __pyx_n_s_n_out, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_sys, __pyx_n_s_fifos, __pyx_n_s_fifo_closed, __pyx_n_s_drained_fifos, __pyx_n_s_out_buf, __pyx_n_s_fout, __pyx_n_s_header_bytes, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(27, __pyx_n_s_fifo_names, __pyx_n_s_fout_name, __pyx_n_s_chunk_size, __pyx_n_s_in_buf_size, __pyx_n_s_out_buf_size, __pyx_n_s_header_fifo, __pyx_n_s_custom_header, __pyx_n_s_n_reopen_inputs, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_n_ins, __pyx_n_s_n, __pyx_n_s_n_out, __pyx_n_s_line, __pyx_n_s_buffer, __pyx_n_s_n_read, __pyx_n_s_fifo_buffers, __pyx_n_s_sys, __pyx_n_s_fifos, __pyx_n_s_fifo_closed, __pyx_n_s_drained_fifos, __pyx_n_s_n_loop, __pyx_n_s_out_buf, __pyx_n_s_fout, __pyx_n_s_header_bytes, __pyx_n_s_fheader); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_collect, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(8, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_mrfifo_fast_loops_pyx, __pyx_n_s_collect, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -5830,15 +6202,15 @@
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   /* AssertionsEnabled.init */
-  __Pyx_init_assertions_enabled();
+  if (likely(__Pyx_init_assertions_enabled() == 0)); else
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -6070,14 +6442,15 @@
   int pystate_addmodule_run = 0;
   #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -6095,42 +6468,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("fast_loops", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to fast_loops pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "fast_loops" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fast_loops(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -6198,15 +6569,15 @@
  * from libc cimport stdlib, stdio
  * from libc.string cimport strstr
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s__2);
   __Pyx_GIVEREF(__pyx_n_s__2);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s__2);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s__2)) __PYX_ERR(0, 6, __pyx_L1_error);
   __pyx_t_3 = __Pyx_Import(__pyx_n_s_types, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_import_star(__pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "mrfifo/fast_loops.pyx":10
@@ -6237,28 +6608,28 @@
  * def distribute(str fin_name, list fifo_names, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *                size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  *                header_detect_func=None, header_fifo="",
  */
   __pyx_t_5 = PyTuple_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
-  __Pyx_INCREF(((PyObject *)Py_None));
-  __Pyx_GIVEREF(((PyObject *)Py_None));
-  PyTuple_SET_ITEM(__pyx_t_5, 3, ((PyObject *)Py_None));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 3, Py_None)) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  PyTuple_SET_ITEM(__pyx_t_5, 4, ((PyObject*)__pyx_kp_u_));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 10, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  PyTuple_SET_ITEM(__pyx_t_5, 5, ((PyObject *)Py_False));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 10, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_1distribute, 0, __pyx_n_s_distribute, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -6284,108 +6655,122 @@
  *                          size_t sub_size, bytes sub_lead=b"\tCB:Z:",
  *                          size_t in_buf_size=2**20, size_t out_buf_size=2**19,
  */
   __pyx_t_2 = PyTuple_New(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject*)__pyx_kp_b_CB_Z));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_b_CB_Z));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject*)__pyx_kp_b_CB_Z));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject*)__pyx_kp_b_CB_Z))) __PYX_ERR(0, 101, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
-  __Pyx_INCREF(((PyObject *)Py_None));
-  __Pyx_GIVEREF(((PyObject *)Py_None));
-  PyTuple_SET_ITEM(__pyx_t_2, 3, ((PyObject *)Py_None));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 3, Py_None)) __PYX_ERR(0, 101, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  PyTuple_SET_ITEM(__pyx_t_2, 4, ((PyObject*)__pyx_kp_u_));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 4, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 101, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  PyTuple_SET_ITEM(__pyx_t_2, 5, ((PyObject *)Py_False));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 5, ((PyObject *)Py_False))) __PYX_ERR(0, 101, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_3distribute_by_substr, 0, __pyx_n_s_distribute_by_substr, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_distribute_by_substr, __pyx_t_5) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
   __pyx_t_5 = __Pyx_PyInt_From_int(((int)0x2710)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
   /* "mrfifo/fast_loops.pyx":211
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,             # <<<<<<<<<<<<<<
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  * 
  */
   __pyx_t_2 = __Pyx_PyInt_FromSize_t(((size_t)0x80000)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyInt_FromSize_t(((size_t)0x100000)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
+  /* "mrfifo/fast_loops.pyx":212
+ * def collect(list fifo_names, str fout_name, int chunk_size=10000,
+ *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):             # <<<<<<<<<<<<<<
+ * 
+ *     if header_fifo == 0:
+ */
+  __pyx_t_3 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
   /* "mrfifo/fast_loops.pyx":210
  * 
  * 
  * def collect(list fifo_names, str fout_name, int chunk_size=10000,             # <<<<<<<<<<<<<<
  *             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
- *             header_fifo="", custom_header=None):
+ *             header_fifo="", custom_header=None, int n_reopen_inputs=1):
  */
-  __pyx_t_3 = PyTuple_New(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = PyTuple_New(6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_kp_u_));
   __Pyx_GIVEREF(((PyObject*)__pyx_kp_u_));
-  PyTuple_SET_ITEM(__pyx_t_3, 3, ((PyObject*)__pyx_kp_u_));
-  __Pyx_INCREF(((PyObject *)Py_None));
-  __Pyx_GIVEREF(((PyObject *)Py_None));
-  PyTuple_SET_ITEM(__pyx_t_3, 4, ((PyObject *)Py_None));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject*)__pyx_kp_u_))) __PYX_ERR(0, 210, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, Py_None)) __PYX_ERR(0, 210, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, __pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error);
   __pyx_t_5 = 0;
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_5collect, 0, __pyx_n_s_collect, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_t_3);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6mrfifo_10fast_loops_5collect, 0, __pyx_n_s_collect, NULL, __pyx_n_s_mrfifo_fast_loops, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_collect, __pyx_t_3) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_collect, __pyx_t_4) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "mrfifo/fast_loops.pyx":1
  * #cython: boundscheck=False, wraparound=False, initializedcheck=False, overflowcheck=False, cdivision=True             # <<<<<<<<<<<<<<
  * ###cython: boundscheck=True, wraparound=True, initializedcheck=True, overflowcheck=True, cdivision=False
  * #!python
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init mrfifo.fast_loops", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
@@ -6499,14 +6884,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -6556,33 +6943,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -6790,21 +7184,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -6854,37 +7266,70 @@
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
     int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
     while (1) {
+        Py_XDECREF(key); key = NULL;
+        Py_XDECREF(value); value = NULL;
         if (kwds_is_tuple) {
-            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(kwds);
+#else
+            size = PyTuple_Size(kwds);
+            if (size < 0) goto bad;
+#endif
+            if (pos >= size) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            key = __Pyx_PySequence_ITEM(kwds, pos);
+            if (!key) goto bad;
+#elif CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kwds, pos);
+#else
+            key = PyTuple_GetItem(kwds, pos);
+            if (!key) goto bad;
+#endif
             value = kwvalues[pos];
             pos++;
         }
         else
         {
             if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(key);
+#endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(value);
+            Py_DECREF(key);
+#endif
+            key = NULL;
+            value = NULL;
             continue;
         }
+#if !CYTHON_AVOID_BORROWED_REFS
+        Py_INCREF(key);
+#endif
+        Py_INCREF(value);
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -6906,14 +7351,17 @@
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -6932,14 +7380,16 @@
             goto invalid_keyword_type;
         if (kwds2) {
             if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
         } else {
             goto invalid_keyword;
         }
     }
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return 0;
 arg_passed_twice:
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
@@ -6951,14 +7401,16 @@
         function_name, PyString_AsString(key));
     #else
     PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return -1;
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     __Pyx_TypeName type_name;
@@ -7293,17 +7745,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -7372,16 +7830,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -7390,66 +7853,62 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
-    PyObject *result;
+    PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
         Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -7465,29 +7924,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* decode_c_bytes */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
          const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
@@ -7556,15 +8025,17 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            #if PY_VERSION_HEX >= 0x030d0000
+            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
+            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
                 __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
             }
@@ -7584,17 +8055,18 @@
     CYTHON_UNUSED_VAR(value_count);
     return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
 }
 
 /* UnpackUnboundCMethod */
 static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -7606,25 +8078,23 @@
     if (unlikely(!method))
         return -1;
     target->method = method;
 #if CYTHON_COMPILING_IN_CPYTHON
     #if PY_MAJOR_VERSION >= 3
     if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
     #else
-    if (likely(!PyCFunction_Check(method)))
+    if (likely(!__Pyx_CyOrPyCFunction_Check(method)))
     #endif
     {
         PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
         target->func = descr->d_method->ml_meth;
         target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
     } else
 #endif
-#if defined(CYTHON_COMPILING_IN_PYPY)
-#elif PY_VERSION_HEX >= 0x03090000
-    if (PyCFunction_CheckExact(method))
+#if CYTHON_COMPILING_IN_PYPY
 #else
     if (PyCFunction_Check(method))
 #endif
     {
         PyObject *self;
         int self_found;
 #if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
@@ -7806,22 +8276,17 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
-                #endif
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
@@ -7832,22 +8297,17 @@
             PyObject *py_level = PyInt_FromLong(level);
             if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
                 name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
             module = PyImport_ImportModuleLevelObject(
                 name, __pyx_d, empty_dict, from_list, level);
             #endif
-            #endif
         }
     }
 bad:
     Py_XDECREF(empty_dict);
     Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
@@ -8054,18 +8514,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -8218,42 +8675,61 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
         (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #endif
 }
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
 {
     CYTHON_UNUSED_VAR(closure);
     if (unlikely(op->func_doc == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
+        if (unlikely(!op->func_doc)) return NULL;
+#else
         if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #else
             op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #endif
             if (unlikely(op->func_doc == NULL))
                 return NULL;
         } else {
             Py_INCREF(Py_None);
             return Py_None;
         }
+#endif
     }
     Py_INCREF(op->func_doc);
     return op->func_doc;
 }
 static int
 __Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
 {
@@ -8266,15 +8742,17 @@
     return 0;
 }
 static PyObject *
 __Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
 {
     CYTHON_UNUSED_VAR(context);
     if (unlikely(op->func_name == NULL)) {
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_name = PyObject_GetAttrString(op->func, "__name__");
+#elif PY_MAJOR_VERSION >= 3
         op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #else
         op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #endif
         if (unlikely(op->func_name == NULL))
             return NULL;
     }
@@ -8385,18 +8863,18 @@
         return -1;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
     Py_INCREF(op->defaults_tuple);
     op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
     Py_INCREF(op->defaults_kwdict);
     #else
-    op->defaults_tuple = PySequence_ITEM(res, 0);
+    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
     if (unlikely(!op->defaults_tuple)) result = -1;
     else {
-        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
         if (unlikely(!op->defaults_kwdict)) result = -1;
     }
     #endif
     Py_DECREF(res);
     return result;
 }
 static int
@@ -8497,15 +8975,23 @@
     is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
 #if PY_VERSION_HEX >= 0x03050000
     if (is_coroutine) {
         PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
         fromlist = PyList_New(1);
         if (unlikely(!fromlist)) return NULL;
         Py_INCREF(marker);
+#if CYTHON_ASSUME_SAFE_MACROS
         PyList_SET_ITEM(fromlist, 0, marker);
+#else
+        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
+            Py_DECREF(marker);
+            Py_DECREF(fromlist);
+            return NULL;
+        }
+#endif
         module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
         Py_DECREF(fromlist);
         if (unlikely(!module)) goto ignore;
         op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
         Py_DECREF(module);
         if (likely(op->func_is_coroutine)) {
             return __Pyx_NewRef(op->func_is_coroutine);
@@ -8513,14 +8999,26 @@
 ignore:
         PyErr_Clear();
     }
 #endif
     op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
     return __Pyx_NewRef(op->func_is_coroutine);
 }
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *
+__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_GetAttrString(op->func, "__module__");
+}
+static int
+__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_SetAttrString(op->func, "__module__", value);
+}
+#endif
 static PyGetSetDef __pyx_CyFunction_getsets[] = {
     {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
     {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
@@ -8532,28 +9030,35 @@
     {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
     {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
     {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+#if CYTHON_COMPILING_IN_LIMITED_API
+    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyMemberDef __pyx_CyFunction_members[] = {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#endif
 #if CYTHON_USE_TYPE_SPECS
     {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
 #if CYTHON_METH_FASTCALL
 #if CYTHON_BACKPORT_VECTORCALL
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
 #else
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
 #endif
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
 #else
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
 #endif
 #endif
     {0, 0, 0,  0, 0}
 };
@@ -8568,38 +9073,48 @@
     return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
 };
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
 #endif
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
                                        PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     PyCFunctionObject *cf = (PyCFunctionObject*) op;
+#endif
     if (unlikely(op == NULL))
         return NULL;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
+    if (unlikely(!op->func)) return NULL;
+#endif
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     cf->m_ml = ml;
     cf->m_self = (PyObject *) op;
+#endif
     Py_XINCREF(closure);
     op->func_closure = closure;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_XINCREF(module);
     cf->m_module = module;
+#endif
     op->func_dict = NULL;
     op->func_name = NULL;
     Py_INCREF(qualname);
     op->func_qualname = qualname;
     op->func_doc = NULL;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     op->func_classobj = NULL;
 #else
     ((PyCMethodObject*)op)->mm_class = NULL;
 #endif
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
@@ -8637,30 +9152,36 @@
 #endif
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_CLEAR(m->func);
+#else
     Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_CLEAR(m->func_dict);
     Py_CLEAR(m->func_name);
     Py_CLEAR(m->func_qualname);
     Py_CLEAR(m->func_doc);
     Py_CLEAR(m->func_globals);
     Py_CLEAR(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
 #if PY_VERSION_HEX < 0x030900B1
     Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
 #else
     {
         PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
         ((PyCMethodObject *) (m))->mm_class = NULL;
         Py_XDECREF(cls);
     }
 #endif
+#endif
     Py_CLEAR(m->defaults_tuple);
     Py_CLEAR(m->defaults_kwdict);
     Py_CLEAR(m->func_annotations);
     Py_CLEAR(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
@@ -8682,22 +9203,28 @@
 {
     PyObject_GC_UnTrack(m);
     __Pyx__CyFunction_dealloc(m);
 }
 static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
 {
     Py_VISIT(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(m->func);
+#else
     Py_VISIT(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_VISIT(m->func_dict);
     Py_VISIT(m->func_name);
     Py_VISIT(m->func_qualname);
     Py_VISIT(m->func_doc);
     Py_VISIT(m->func_globals);
     Py_VISIT(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+#endif
     Py_VISIT(m->defaults_tuple);
     Py_VISIT(m->defaults_kwdict);
     Py_VISIT(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
         for (i = 0; i < m->defaults_pyobjects; i++)
@@ -8713,67 +9240,123 @@
                                 op->func_qualname, (void *)op);
 #else
     return PyString_FromFormat("<cyfunction %s at %p>",
                                PyString_AsString(op->func_qualname), (void *)op);
 #endif
 }
 static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
+    PyObject *py_name = NULL;
+    PyCFunction meth;
+    int flags;
+    meth = PyCFunction_GetFunction(f);
+    if (unlikely(!meth)) return NULL;
+    flags = PyCFunction_GetFlags(f);
+    if (unlikely(flags < 0)) return NULL;
+#else
     PyCFunctionObject* f = (PyCFunctionObject*)func;
     PyCFunction meth = f->m_ml->ml_meth;
+    int flags = f->m_ml->ml_flags;
+#endif
     Py_ssize_t size;
-    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
     case METH_VARARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0))
             return (*meth)(self, arg);
         break;
     case METH_VARARGS | METH_KEYWORDS:
         return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
     case METH_NOARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 0))
                 return (*meth)(self, NULL);
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     case METH_O:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 1)) {
                 PyObject *result, *arg0;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                 arg0 = PyTuple_GET_ITEM(arg, 0);
                 #else
-                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
                 #endif
                 result = (*meth)(self, arg0);
                 #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
                 Py_DECREF(arg0);
                 #endif
                 return result;
             }
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     default:
         PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
         return NULL;
     }
+#if CYTHON_COMPILING_IN_LIMITED_API
+    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+    if (!py_name) return NULL;
+    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
+                 py_name);
+    Py_DECREF(py_name);
+#else
     PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
                  f->m_ml->ml_name);
+#endif
     return NULL;
 }
 static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+    PyObject *self, *result;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
+    if (unlikely(!self) && PyErr_Occurred()) return NULL;
+#else
+    self = ((PyCFunctionObject*)func)->m_self;
+#endif
+    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
+    return result;
 }
 static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
     PyObject *result;
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
 #if CYTHON_METH_FASTCALL
      __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
     if (vc) {
@@ -8785,15 +9368,20 @@
 #endif
     }
 #endif
     if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
         Py_ssize_t argc;
         PyObject *new_args;
         PyObject *self;
+#if CYTHON_ASSUME_SAFE_MACROS
         argc = PyTuple_GET_SIZE(args);
+#else
+        argc = PyTuple_Size(args);
+        if (unlikely(!argc) < 0) return NULL;
+#endif
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
 #if PY_MAJOR_VERSION > 2
@@ -8910,15 +9498,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -8998,15 +9586,15 @@
     0,
     0,
     0,
     0,
 #ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
     Py_TPFLAGS_METHOD_DESCRIPTOR |
 #endif
-#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
     _Py_TPFLAGS_HAVE_VECTORCALL |
 #endif
     Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
     0,
     (traverseproc) __Pyx_CyFunction_traverse,
     (inquiry) __Pyx_CyFunction_clear,
     0,
@@ -9256,28 +9844,101 @@
 }
 #endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyCode_Replace_For_AddTraceback(PyObject *code, PyObject *scratch_dict,
+                                                       PyObject *firstlineno, PyObject *name) {
+    PyObject *replace = NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_firstlineno", firstlineno))) return NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_name", name))) return NULL;
+    replace = PyObject_GetAttrString(code, "replace");
+    if (likely(replace)) {
+        PyObject *result;
+        result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
+        Py_DECREF(replace);
+        return result;
+    }
+    PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
+    {
+        PyObject *compiled = NULL, *result = NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
+        compiled = Py_CompileString(
+            "out = type(code)(\n"
+            "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
+            "  code.co_flags, code.co_code, code.co_consts, code.co_names,\n"
+            "  code.co_varnames, code.co_filename, co_name, co_firstlineno,\n"
+            "  code.co_lnotab)\n", "<dummy>", Py_file_input);
+        if (!compiled) return NULL;
+        result = PyEval_EvalCode(compiled, scratch_dict, scratch_dict);
+        Py_DECREF(compiled);
+        if (!result) PyErr_Print();
+        Py_DECREF(result);
+        result = PyDict_GetItemString(scratch_dict, "out");
+        if (result) Py_INCREF(result);
+        return result;
+    }
+    #else
+    return NULL;
+    #endif
+}
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
+    PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
+    PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
+    PyObject *exc_type, *exc_value, *exc_traceback;
+    int success = 0;
     if (c_line) {
         (void) __pyx_cfilenm;
         (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
     }
-    _PyTraceback_Add(funcname, filename, py_line);
+    PyErr_Fetch(&exc_type, &exc_value, &exc_traceback);
+    code_object = Py_CompileString("_getframe()", filename, Py_eval_input);
+    if (unlikely(!code_object)) goto bad;
+    py_py_line = PyLong_FromLong(py_line);
+    if (unlikely(!py_py_line)) goto bad;
+    py_funcname = PyUnicode_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    dict = PyDict_New();
+    if (unlikely(!dict)) goto bad;
+    {
+        PyObject *old_code_object = code_object;
+        code_object = __Pyx_PyCode_Replace_For_AddTraceback(code_object, dict, py_py_line, py_funcname);
+        Py_DECREF(old_code_object);
+    }
+    if (unlikely(!code_object)) goto bad;
+    getframe = PySys_GetObject("_getframe");
+    if (unlikely(!getframe)) goto bad;
+    if (unlikely(PyDict_SetItemString(dict, "_getframe", getframe))) goto bad;
+    frame = PyEval_EvalCode(code_object, dict, dict);
+    if (unlikely(!frame) || frame == Py_None) goto bad;
+    success = 1;
+  bad:
+    PyErr_Restore(exc_type, exc_value, exc_traceback);
+    Py_XDECREF(code_object);
+    Py_XDECREF(py_py_line);
+    Py_XDECREF(py_funcname);
+    Py_XDECREF(dict);
+    Py_XDECREF(replace);
+    if (success) {
+        PyTraceBack_Here(
+            (struct _frame*)frame);
+    }
+    Py_XDECREF(frame);
 }
 #else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
@@ -9322,15 +9983,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -9563,15 +10224,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -9836,15 +10497,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -9972,16 +10633,42 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
     }
 }
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -10010,29 +10697,56 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
     }
 }
 
 /* FormatTypeName */
 #if CYTHON_COMPILING_IN_LIMITED_API
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__9));
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__9);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -10200,15 +10914,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -10426,49 +11140,58 @@
 /* CStringEquals */
 static CYTHON_INLINE int __Pyx_StrEq(const char *s1, const char *s2) {
     while (*s1 != '\0' && *s1 == *s2) { s1++; s2++; }
     return *s1 == *s2;
 }
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
 #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -10506,16 +11229,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `mrfifo-0.3/mrfifo/fast_loops.pyx` & `mrfifo-0.5/mrfifo/fast_loops.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     stdlib.free(buffer)
 
     return n # number of lines distributed (excluding header)
 
 
 def collect(list fifo_names, str fout_name, int chunk_size=10000, 
             size_t in_buf_size=2**19, size_t out_buf_size=2**20,
-            header_fifo="", custom_header=None):
+            header_fifo="", custom_header=None, int n_reopen_inputs=1):
 
     if header_fifo == 0:
         # special mode: use the first fifo name for header data 
         # and the other as round-robin inputs as usual
         header_fifo = fifo_names[0]
         fifo_names = fifo_names[1:]
 
@@ -230,19 +230,18 @@
     # support collecting and demuxing from up to 128 fifos
     cdef char* fifo_buffers[128]
 
     import sys
     # sys.stderr.write(f"collecting from {fifo_names} into {fout_name}")
     assert n <= 128
     cdef stdio.FILE *fifos[128]
-    cdef bint fifo_closed[128]
-    for i in range(n_ins):
-        fifo_closed[i] = False
+    cdef bint[128] fifo_closed
     
     cdef size_t drained_fifos = 0
+    cdef int n_loop = 0
     
     # line buffer
     buffer = <char*>stdlib.malloc(out_buf_size)
     # prepare output file and buffer
     cdef char* out_buf = <char*>stdlib.malloc(out_buf_size)
     cdef stdio.FILE *fout = stdio.fopen(fout_name.encode('utf-8'), 'w')
     stdio.setvbuf(fout, out_buf, stdio._IOFBF, out_buf_size)
@@ -264,39 +263,45 @@
                 break
             
             stdio.fwrite(buffer, n_read, 1, fout)
         
         # all header data has been read! close this fifo's reading end
         stdio.fclose(fheader)
 
-    # now prepare input from all the demuxed fifos
-    for i in range(n_ins):
-        fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
-        fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
-        stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
-
-    # main mutiplexing loop
-    while(drained_fifos < n_ins):
-        j = n // chunk_size
-        k = j % n_ins # index of fifo
-        if not fifo_closed[k]:
-            # print(f"collection wants to read from {fifo_names[k]}. blocking")
-            n_read = stdio.getline(&buffer, &out_buf_size, fifos[k]) 
-            if n_read <= 0:
-                fifo_closed[k] = True
-                drained_fifos += 1
-            else:
-                # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
-                stdio.fwrite(buffer, n_read, 1, fout)
-                n_out += 1
-        n += 1
-
-    for i in range(n_ins):
-        stdio.fclose(fifos[i])
-        stdlib.free(fifo_buffers[i])
+    for n_loop in range(n_reopen_inputs):
+        #print(f"opening the input fifos for the {n_loop}th time: {fifo_names}")
+        # now prepare input from all the demuxed fifos
+        for i in range(n_ins):
+            fifo_buffers[i] = <char*>stdlib.malloc(in_buf_size)
+            fifos[i] = stdio.fopen(fifo_names[i].encode('utf-8'), 'r')
+            stdio.setvbuf(fifos[i], fifo_buffers[i], stdio._IOFBF, in_buf_size)
+
+        drained_fifos = 0
+        for i in range(n_ins):
+            fifo_closed[i] = False
+
+        # main mutiplexing loop
+        while(drained_fifos < n_ins):
+            j = n // chunk_size
+            k = j % n_ins # index of fifo
+            if not fifo_closed[k]:
+                # print(f"collection wants to read from {fifo_names[k]}. blocking")
+                n_read = stdio.getline(&buffer, &out_buf_size, fifos[k]) 
+                if n_read <= 0:
+                    fifo_closed[k] = True
+                    drained_fifos += 1
+                else:
+                    # print(f"fifo {k} ({fifo_names[k]}). {n_read} bytes. writing to {fout_name}")
+                    stdio.fwrite(buffer, n_read, 1, fout)
+                    n_out += 1
+            n += 1
+
+        for i in range(n_ins):
+            stdio.fclose(fifos[i])
+            stdlib.free(fifo_buffers[i])
 
     # free the line buffer, close the output, and free the output buffer
     stdlib.free(buffer)
     stdio.fclose(fout)
     stdlib.free(out_buf)
 
     return n_out # total number of multiplexed lines (excluding header)
```

### Comparing `mrfifo-0.3/mrfifo/parallel.py` & `mrfifo-0.5/mrfifo/parallel.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/mrfifo/parts.py` & `mrfifo-0.5/mrfifo/parts.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,37 @@
     assert "b" in output.mode
     logger = logging.getLogger("mrfifo.parts.igzip_reader")
     n_bytes = 0
     from isal import igzip
 
     for fname in inputs:
         logger.info(f"reading from {fname}")
-        in_file = igzip.IGzipFile(fname, "r")
-        while True:
-            block = in_file.read(igzip.READ_BUFFER_SIZE)
-            if block == b"":
-                break
+        try:
+            in_file = igzip.IGzipFile(fname, "r")
+            while True:
+                block = in_file.read(igzip.READ_BUFFER_SIZE)
+                if block == b"":
+                    break
+
+                output.write(block)
+                n_bytes += len(block)
+
+        except igzip.BadGzipFile:
+            logger.warning(f"Not a proper gzip file: '{fname}'. Assuming text file.")
+            in_file = open(fname, "rb")
+            while True:
+                block = in_file.read(igzip.READ_BUFFER_SIZE)
+                if block == b"":
+                    break
 
-            output.write(block)
-            n_bytes += len(block)
+                output.write(block)
+                n_bytes += len(block)
 
-        in_file.close()
+        finally:
+            in_file.close()
 
     return n_bytes
 
 
 def bam_reader(input, output, threads=2, mode="Sh"):
     "ensure that the out FIFO is not managed"
     assert type(output) is str
@@ -57,36 +70,36 @@
     return os.system(f"cat {input} > {output}")
 
 
 def distributor(input, outputs, **kw):
     "ensure that the FIFOs are not managed"
     assert type(input) is str
     logger = logging.getLogger("mrfifo.parts.distributor")
-    logger.info(f"reading from {input}, writing to {outputs} kw={kw}")
+    logger.debug(f"reading from {input}, writing to {outputs} kw={kw}")
 
     from .fast_loops import distribute
 
     res = distribute(fin_name=input, fifo_names=outputs, **kw)
-    logger.info("distribution complete")
+    logger.debug("distribution complete")
     return res
 
 
 def collector(inputs, output, **kw):
     "ensure that the FIFOs are not managed"
     for inp in inputs:
         assert type(inp) is str
 
     assert type(output) is str
 
     logger = logging.getLogger("mrfifo.parts.collector")
-    logger.info(f"collecting from '{inputs}', writing to '{output}' kw={kw}")
+    logger.debug(f"collecting from '{inputs}', writing to '{output}' kw={kw}")
     from .fast_loops import collect
 
     res = collect(fifo_names=inputs, fout_name=output, **kw)
-    logger.info("collection complete")
+    logger.debug("collection complete")
     return res
 
 
 # def serializer(inputs, outputs, name="mrfifo.parts.serializser", **kw):
 #     assert len(inputs) > 0
 #     assert len(outputs) == 1
 #     fout = outputs.pop()
```

### Comparing `mrfifo-0.3/mrfifo/plumbing.py` & `mrfifo-0.5/mrfifo/plumbing.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/mrfifo/util.py` & `mrfifo-0.5/mrfifo/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
         from collections import defaultdict
 
         self.stats = defaultdict(float)
         for o in others:
             if type(o) is CountDict:
                 self.add_other_stats(o)
 
+    # @staticmethod
+    # def from_list_of_dicts(cls, dlist):
+
     def count(self, key, inc=1):
         self.stats[key] += inc
 
     def add_other_stats(self, other):
         for k, v in other.items():
             self.stats[k] += v
```

### Comparing `mrfifo-0.3/mrfifo.egg-info/PKG-INFO` & `mrfifo-0.5/mrfifo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfifo
-Version: 0.3
+Version: 0.5
 Summary: Map-Reduce parallelism over FIFOs (named pipes)
 Home-page: https://github.com/marvin-jens/mrfifo
 Author: Marvin Jens
 Author-email: marvin.jens@charite.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/marvin-jens/mrfifo/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mrfifo-0.3/setup.cfg` & `mrfifo-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/setup.py` & `mrfifo-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/test_data/tiny_test.bam` & `mrfifo-0.5/test_data/tiny_test.bam`

 * *Files identical despite different names*

### Comparing `mrfifo-0.3/tests/test_cy.py` & `mrfifo-0.5/tests/test_cy.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,20 @@
             raise ValueError(
                 f"{_job_name} was asked to raise an exception for testing purposes. Here we are..."
             )
 
     return i
 
 
-def turn_to_SAM(input, output, **kwargs):
+def turn_to_SAM(input, output, barcode=None, **kwargs):
     sam_line = "{qname}\t4\t*\t0\t0\t*\t*\t0\t0\t{seq}\t{qual}\t{tags}\n"
     tags = "RG:Z:A"
+    if barcode:
+        tags += f"\tBC:Z:{barcode}"
+
     for line in input:
         i = int(line)
         qname = f"read_{i}"
         seq = "ACTG" + "ACTG" * i
         qual = "E" * len(seq)
         output.write(sam_line.format(**locals()))
 
@@ -416,14 +419,61 @@
             fmt="Sbh",
         )
         .run()
     )
     print(str(w))
 
 
+def test_iterate(n=2, chunk_size=1):
+
+    inputs = [["test_data/simple.txt.gz"], ["test_data/simple.txt.gz"]]
+    settings = [{"barcode": "AAA"}, {"barcode": "AAC"}]
+
+    w = mf.Workflow("iterate")
+    for input, params in zip(inputs, settings):
+        (
+            w.subworkflow(f"input_loop.{params['barcode']}")
+            .gz_reader(inputs=input)
+            .distribute(
+                input=mf.FIFO("input_text", "rt"),
+                outputs=mf.FIFO("dist{n}", "wt", n=n),
+                chunk_size=chunk_size,
+            )
+            .workers(
+                input=mf.FIFO("dist{n}", "rt"),
+                output=mf.FIFO("out{n}", "wt"),
+                func=turn_to_SAM,
+                n=n,
+                **params,
+            )
+        )
+
+    (
+        w.collect(
+            inputs=mf.FIFO("out{n}", "rt", n=n),
+            n_reopen_inputs=len(inputs),
+            custom_header=mf.util.make_SAM_header(),
+            #     output="test.sam",
+            #     chunk_size=chunk_size,
+            # )
+            output=mf.FIFO("out_sam", "wt"),  # "test.sam",
+            chunk_size=chunk_size,
+        )
+        .funnel(
+            input=mf.FIFO("out_sam", "rt"),
+            output="test_data/new.bam",
+            _manage_fifos=False,
+            func=mf.parts.bam_writer,
+            fmt="Sbh",
+        )
+        .run()
+    )
+    print(str(w))
+
+
 if __name__ == "__main__":
     import logging
 
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(asctime)-20s\t%(name)-30s\t%(levelname)s\t%(message)s",
     )
@@ -434,8 +484,9 @@
     # test_dist_work_funnel()
     # test_dist_work_funnel_count()
     # test_dist_work_collect_funnel()
     # test_header_broadcast()
     # test_header_fifo()
     # test_bam_reconstruct()
     # test_fancy_counter()
-    test_BAM_creation()
+    # test_BAM_creation()
+    test_iterate()
```

