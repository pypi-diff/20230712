# Comparing `tmp/spaces-0.7.0.tar.gz` & `tmp/spaces-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.7.0.tar", max compression
+gzip compressed data, was "spaces-0.8.0.tar", max compression
```

## Comparing `spaces-0.7.0.tar` & `spaces-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.7.0/README.md
--rw-r--r--   0        0        0     1524 2023-07-07 16:42:49.331263 spaces-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.7.0/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.7.0/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.7.0/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     2224 2023-07-07 16:19:13.425611 spaces-0.7.0/spaces/gpu/client.py
--rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.7.0/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.7.0/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6888 2023-07-07 16:28:48.625635 spaces-0.7.0/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.7.0/spaces/gradio.py
--rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.7.0/spaces/utils.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.7.0/setup.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.8.0/README.md
+-rw-r--r--   0        0        0     1524 2023-07-12 10:17:10.011073 spaces-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.8.0/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.8.0/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.8.0/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     2330 2023-07-12 09:59:29.756084 spaces-0.8.0/spaces/gpu/client.py
+-rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.8.0/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.8.0/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     7058 2023-07-12 10:03:26.126469 spaces-0.8.0/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.8.0/spaces/gradio.py
+-rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.8.0/spaces/utils.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.8.0/setup.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.8.0/PKG-INFO
```

### Comparing `spaces-0.7.0/pyproject.toml` & `spaces-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.7.0"
+version = "0.8.0"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
```

### Comparing `spaces-0.7.0/spaces/gpu/client.py` & `spaces-0.8.0/spaces/gpu/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 
 
 CGROUP_PATH = utils.self_cgroup_device_path()
 
 
 class ScheduleParams(BaseModel):
     cgroupPath: str
+    taskId: int
 
 class ScheduleResponse(BaseModel):
     idle: bool
     nvidiaIndex: int
     nvidiaUUID: str
 
 class ReleaseParams(BaseModel):
     cgroupPath: str
+    taskId: int
     nvidiaIndex: int
     fail: bool
 
 
 def base_url() -> str:
     assert Config.zero_device_api_url is not None
     return Config.zero_device_api_url
@@ -45,18 +47,19 @@
         time.sleep(1)
         if (retries := retries + 1) > max_retries:
             raise RuntimeError("Error while initializing ZeroGPU: NotFound")
     if status != HTTPStatus.OK: # pragma: no cover
         raise RuntimeError("Error while initializing ZeroGPU: Unknown")
 
 
-def schedule() -> ScheduleResponse:
+def schedule(task_id: int) -> ScheduleResponse:
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
+        taskId=task_id,
     ))
 
     if res.status_code == HTTPStatus.TOO_MANY_REQUESTS:
         raise gr.Error("No GPU is currently available")
 
     try:
         data = res.json()
@@ -65,18 +68,19 @@
 
     if not res.ok: # pragma: no cover
         raise RuntimeError(f"ZeroGPU API /schedule error: {data.get('detail')}")
 
     return ScheduleResponse(**data)
 
 
-def release(nvidia_index: int, fail: bool = False) -> None:
+def release(task_id: int, nvidia_index: int, fail: bool = False) -> None:
 
     res = post('/release', params=ReleaseParams(
         cgroupPath=CGROUP_PATH,
+        taskId=task_id,
         nvidiaIndex=nvidia_index,
         fail=fail,
     ))
 
     if not res.ok:
         try:
             data = res.json()
```

### Comparing `spaces-0.7.0/spaces/gpu/decorator.py` & `spaces-0.8.0/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.7.0/spaces/gpu/torch.py` & `spaces-0.8.0/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.7.0/spaces/gpu/wrappers.py` & `spaces-0.8.0/spaces/gpu/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,32 +58,33 @@
             target=target,
             args=args,
             daemon=True,
         )
         self.process.start()
         self._sentinel.start()
 
-    def _close_on_exit(self):
+    def _close_on_exit(self): # TODO: differentiate 137 (killed) vs. other return codes (internal errors)
         self.process.join()
         self.res_queue.close()
 
 
 def regular_function_wrapper(
     task:
      Callable[Param, Res],
 ) -> Callable[Param, Res]:
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception]] = {}
+    task_id = id(task)
 
     def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Res:
 
-        schedule_response = client.schedule()
+        schedule_response = client.schedule(task_id)
         nvidia_index = schedule_response.nvidiaIndex
         nvidia_uuid = schedule_response.nvidiaUUID
-        release = partial(client.release, nvidia_index=nvidia_index)
+        release = partial(client.release, task_id=task_id, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
             worker = Worker(thread_wrapper, nvidia_uuid)
             workers[nvidia_index] = worker
 
         try:
@@ -137,21 +138,22 @@
 
 def generator_function_wrapper(
     task:
      Callable[Param, Generator[Res, None, None]],
 ) -> Callable[Param, Generator[Res, None, None]]:
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception | None]] = {}
+    task_id = id(task)
 
     def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Generator[Res, None, None]:
 
-        schedule_response = client.schedule()
+        schedule_response = client.schedule(task_id)
         nvidia_index = schedule_response.nvidiaIndex
         nvidia_uuid = schedule_response.nvidiaUUID
-        release = partial(client.release, nvidia_index=nvidia_index)
+        release = partial(client.release, task_id=task_id, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
             worker = Worker(thread_wrapper, nvidia_uuid)
             workers[nvidia_index] = worker
 
         try:
```

### Comparing `spaces-0.7.0/spaces/gradio.py` & `spaces-0.8.0/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.7.0/spaces/utils.py` & `spaces-0.8.0/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.7.0/setup.py` & `spaces-0.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.7.0/PKG-INFO` & `spaces-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.7.0
+Version: 0.8.0
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

