# Comparing `tmp/pypomes_scheduling-0.1.7.tar.gz` & `tmp/pypomes_scheduling-0.1.8.tar.gz`

## Comparing `pypomes_scheduling-0.1.7.tar` & `pypomes_scheduling-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/__threaded_scheduler.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.7/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.1.8/src/pypomes_scheduling/__threaded_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                                             jobstore_retry_interval=retry_interval)
         if self._logger is not None:
             self._logger.info("Instanced, with timezone "
                               f"'{timezone}' and retry interval '{retry_interval}'")
 
     def run(self):
         """
-        Start the scheduler in itas own thread.
+        Start the scheduler in its own thread.
         """
         # stay in loop until 'stop()' is invoked
         while not self._stopped:
             if self._logger is not None:
                 self._logger.info("Started")
 
             # start the scheduler, blocking the thread until it is interrupted
@@ -43,15 +43,16 @@
         self._scheduler.shutdown()
         if self._logger is not None:
             self._logger.info("Finished")
 
     def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str = None,
                      job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None):
         """
-        Schedule the given *job*, with the parameters
+        Schedule the given *job*, with the given parameters.
+
         :param job: the callable object to be scheduled
         :param job_id: the id of the scheduled job
         :param job_name: the name of the scheduled job
         :param job_cron: the CRON expression directing the execution times
         :param job_start: the start timestamp for the scheduling process
         :param job_args: the '*args' arguments to be passed to the scheduled job
         :param job_kwargs: the '**kwargs' arguments to be passed to the scheduled job
```

### Comparing `pypomes_scheduling-0.1.7/LICENSE` & `pypomes_scheduling-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.7/pyproject.toml` & `pypomes_scheduling-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.7/PKG-INFO` & `pypomes_scheduling-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

