# Comparing `tmp/havenpy-0.0.7.tar.gz` & `tmp/havenpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "havenpy-0.0.7.tar", last modified: Wed Jul  5 21:28:11 2023, max compression
+gzip compressed data, was "havenpy-0.2.0.tar", last modified: Wed Jul 12 00:07:24 2023, max compression
```

## Comparing `havenpy-0.0.7.tar` & `havenpy-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 21:28:11.367745 havenpy-0.0.7/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-05 21:28:11.367629 havenpy-0.0.7/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-30 05:08:05.000000 havenpy-0.0.7/README.md
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 21:28:11.366294 havenpy-0.0.7/havenpy/
--rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-30 05:08:05.000000 havenpy-0.0.7/havenpy/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-30 05:08:05.000000 havenpy-0.0.7/havenpy/interceptor.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 21:28:11.367350 havenpy-0.0.7/havenpy/pb/
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-07-05 19:42:02.000000 havenpy-0.0.7/havenpy/pb/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     4787 2023-07-05 19:42:02.000000 havenpy-0.0.7/havenpy/pb/manager_pb2.py
--rw-r--r--   0 konsti     (501) staff       (20)    13083 2023-07-05 19:42:02.000000 havenpy-0.0.7/havenpy/pb/manager_pb2_grpc.py
--rw-r--r--   0 konsti     (501) staff       (20)     2641 2023-07-05 19:48:33.000000 havenpy-0.0.7/havenpy/run.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-05 21:28:11.366929 havenpy-0.0.7/havenpy.egg-info/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-05 21:28:11.000000 havenpy-0.0.7/havenpy.egg-info/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)      310 2023-07-05 21:28:11.000000 havenpy-0.0.7/havenpy.egg-info/SOURCES.txt
--rw-r--r--   0 konsti     (501) staff       (20)        1 2023-07-05 21:28:11.000000 havenpy-0.0.7/havenpy.egg-info/dependency_links.txt
--rw-r--r--   0 konsti     (501) staff       (20)       32 2023-07-05 21:28:11.000000 havenpy-0.0.7/havenpy.egg-info/requires.txt
--rw-r--r--   0 konsti     (501) staff       (20)        8 2023-07-05 21:28:11.000000 havenpy-0.0.7/havenpy.egg-info/top_level.txt
--rw-r--r--   0 konsti     (501) staff       (20)       38 2023-07-05 21:28:11.367781 havenpy-0.0.7/setup.cfg
--rw-r--r--   0 konsti     (501) staff       (20)      314 2023-07-05 19:51:30.000000 havenpy-0.0.7/setup.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-12 00:07:24.186552 havenpy-0.2.0/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-12 00:07:24.186419 havenpy-0.2.0/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-30 05:08:05.000000 havenpy-0.2.0/README.md
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-12 00:07:24.184910 havenpy-0.2.0/havenpy/
+-rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-30 05:08:05.000000 havenpy-0.2.0/havenpy/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-30 05:08:05.000000 havenpy-0.2.0/havenpy/interceptor.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-12 00:07:24.185906 havenpy-0.2.0/havenpy/pb/
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-07-10 05:08:07.000000 havenpy-0.2.0/havenpy/pb/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     6230 2023-07-11 04:11:41.000000 havenpy-0.2.0/havenpy/pb/manager_pb2.py
+-rw-r--r--   0 konsti     (501) staff       (20)    17424 2023-07-11 04:11:41.000000 havenpy-0.2.0/havenpy/pb/manager_pb2_grpc.py
+-rw-r--r--   0 konsti     (501) staff       (20)     4420 2023-07-11 23:02:59.000000 havenpy-0.2.0/havenpy/run.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-07-12 00:07:24.185551 havenpy-0.2.0/havenpy.egg-info/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-07-12 00:07:24.000000 havenpy-0.2.0/havenpy.egg-info/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)      310 2023-07-12 00:07:24.000000 havenpy-0.2.0/havenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        1 2023-07-12 00:07:24.000000 havenpy-0.2.0/havenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       32 2023-07-12 00:07:24.000000 havenpy-0.2.0/havenpy.egg-info/requires.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        8 2023-07-12 00:07:24.000000 havenpy-0.2.0/havenpy.egg-info/top_level.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       38 2023-07-12 00:07:24.186592 havenpy-0.2.0/setup.cfg
+-rw-r--r--   0 konsti     (501) staff       (20)      314 2023-07-12 00:06:54.000000 havenpy-0.2.0/setup.py
```

### Comparing `havenpy-0.0.7/havenpy/interceptor.py` & `havenpy-0.2.0/havenpy/interceptor.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.7/havenpy/pb/manager_pb2.py` & `havenpy-0.2.0/havenpy/pb/manager_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,47 +9,51 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"1\n\rSetupResponse\x12\x14\n\x07message\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_message\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"\xdc\x01\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"&\n\x16\x43hatCompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xe8\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12\x11\n\x04zone\x18\x07 \x01(\tH\x03\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_countB\x07\n\x05_zone\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*<\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0f\n\x0bUNREACHABLE\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xbc\x04\n\x05Haven\x12\x34\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x14.haven.SetupResponse\"\x00\x12Q\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x1d.haven.ChatCompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rmanager.proto\x12\x05haven\"\x07\n\x05\x45mpty\"2\n\x0cSetupRequest\x12\x15\n\x08key_file\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_key_file\"1\n\rSetupResponse\x12\x14\n\x07message\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\n\n\x08_message\"5\n\x07Message\x12\x19\n\x04role\x18\x01 \x01(\x0e\x32\x0b.haven.Role\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"\xdc\x01\n\x15\x43hatCompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12 \n\x08messages\x18\x02 \x03(\x0b\x32\x0e.haven.Message\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"\xdb\x01\n\x11\x43ompletionRequest\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x0e\n\x06prompt\x18\x02 \x01(\t\x12\x13\n\x0bstop_tokens\x18\x07 \x03(\t\x12\x17\n\nmax_tokens\x18\x03 \x01(\x05H\x00\x88\x01\x01\x12\x12\n\x05top_p\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05top_k\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x18\n\x0btemperature\x18\x06 \x01(\x02H\x03\x88\x01\x01\x42\r\n\x0b_max_tokensB\x08\n\x06_top_pB\x08\n\x06_top_kB\x0e\n\x0c_temperature\"\"\n\x12\x43ompletionResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"\xbc\x02\n\x05Model\x12\x14\n\x0c\x61rchitecture\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x03 \x01(\t\x12\x1a\n\rsystem_prompt\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x1f\n\x12instruction_prefix\x18\x05 \x01(\tH\x01\x88\x01\x01\x12 \n\x13instruction_postfix\x18\x06 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\routput_prefix\x18\x07 \x01(\tH\x03\x88\x01\x01\x12\x1b\n\x0eoutput_postfix\x18\x08 \x01(\tH\x04\x88\x01\x01\x42\x10\n\x0e_system_promptB\x15\n\x13_instruction_prefixB\x16\n\x14_instruction_postfixB\x10\n\x0e_output_prefixB\x11\n\x0f_output_postfix\"\x19\n\tModelName\x12\x0c\n\x04name\x18\x01 \x01(\t\"2\n\x12ListModelsResponse\x12\x1c\n\x06models\x18\x01 \x03(\x0b\x32\x0c.haven.Model\"<\n\x06Worker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.haven.Status\"5\n\x13ListWorkersResponse\x12\x1e\n\x07workers\x18\x01 \x03(\x0b\x32\r.haven.Worker\"\xe8\x01\n\x1c\x43reateInferenceWorkerRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x14\n\x0cquantization\x18\x02 \x01(\t\x12\x18\n\x0bworker_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x12%\n\x08gpu_type\x18\x04 \x01(\x0e\x32\x0e.haven.GpuTypeH\x01\x88\x01\x01\x12\x16\n\tgpu_count\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12\x11\n\x04zone\x18\x07 \x01(\tH\x03\x88\x01\x01\x42\x0e\n\x0c_worker_nameB\x0b\n\t_gpu_typeB\x0c\n\n_gpu_countB\x07\n\x05_zone\"&\n\x0fInferenceWorker\x12\x13\n\x0bworker_name\x18\x01 \x01(\t*\x1f\n\x04Role\x12\r\n\tASSISTANT\x10\x00\x12\x08\n\x04USER\x10\x01*8\n\x06Status\x12\n\n\x06ONLINE\x10\x00\x12\x0b\n\x07LOADING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\t\n\x05\x45RROR\x10\x03**\n\x07GpuType\x12\x08\n\x04\x41\x31\x30\x30\x10\x00\x12\r\n\tA100_80GB\x10\x01\x12\x06\n\x02T4\x10\x02\x32\xda\x05\n\x05Haven\x12\x34\n\x05Setup\x12\x13.haven.SetupRequest\x1a\x14.haven.SetupResponse\"\x00\x12M\n\x0e\x43hatCompletion\x12\x1c.haven.ChatCompletionRequest\x1a\x19.haven.CompletionResponse\"\x00\x30\x01\x12\x45\n\nCompletion\x12\x18.haven.CompletionRequest\x1a\x19.haven.CompletionResponse\"\x00\x30\x01\x12\x37\n\nListModels\x12\x0c.haven.Empty\x1a\x19.haven.ListModelsResponse\"\x00\x12(\n\x08\x41\x64\x64Model\x12\x0c.haven.Model\x1a\x0c.haven.Empty\"\x00\x12/\n\x0b\x44\x65leteModel\x12\x10.haven.ModelName\x1a\x0c.haven.Empty\"\x00\x12\x39\n\x0bListWorkers\x12\x0c.haven.Empty\x1a\x1a.haven.ListWorkersResponse\"\x00\x12V\n\x15\x43reateInferenceWorker\x12#.haven.CreateInferenceWorkerRequest\x1a\x16.haven.InferenceWorker\"\x00\x12H\n\x14PauseInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15ResumeInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x12I\n\x15\x44\x65leteInferenceWorker\x12\x16.haven.InferenceWorker\x1a\x16.haven.InferenceWorker\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'manager_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ROLE._serialized_start=921
-  _ROLE._serialized_end=952
-  _STATUS._serialized_start=954
-  _STATUS._serialized_end=1014
-  _GPUTYPE._serialized_start=1016
-  _GPUTYPE._serialized_end=1058
+  _ROLE._serialized_start=1462
+  _ROLE._serialized_end=1493
+  _STATUS._serialized_start=1495
+  _STATUS._serialized_end=1551
+  _GPUTYPE._serialized_start=1553
+  _GPUTYPE._serialized_end=1595
   _EMPTY._serialized_start=24
   _EMPTY._serialized_end=31
   _SETUPREQUEST._serialized_start=33
   _SETUPREQUEST._serialized_end=83
   _SETUPRESPONSE._serialized_start=85
   _SETUPRESPONSE._serialized_end=134
   _MESSAGE._serialized_start=136
   _MESSAGE._serialized_end=189
   _CHATCOMPLETIONREQUEST._serialized_start=192
   _CHATCOMPLETIONREQUEST._serialized_end=412
-  _CHATCOMPLETIONRESPONSE._serialized_start=414
-  _CHATCOMPLETIONRESPONSE._serialized_end=452
-  _MODEL._serialized_start=454
-  _MODEL._serialized_end=475
-  _LISTMODELSRESPONSE._serialized_start=477
-  _LISTMODELSRESPONSE._serialized_end=527
-  _WORKER._serialized_start=529
-  _WORKER._serialized_end=589
-  _LISTWORKERSRESPONSE._serialized_start=591
-  _LISTWORKERSRESPONSE._serialized_end=644
-  _CREATEINFERENCEWORKERREQUEST._serialized_start=647
-  _CREATEINFERENCEWORKERREQUEST._serialized_end=879
-  _INFERENCEWORKER._serialized_start=881
-  _INFERENCEWORKER._serialized_end=919
-  _HAVEN._serialized_start=1061
-  _HAVEN._serialized_end=1633
+  _COMPLETIONREQUEST._serialized_start=415
+  _COMPLETIONREQUEST._serialized_end=634
+  _COMPLETIONRESPONSE._serialized_start=636
+  _COMPLETIONRESPONSE._serialized_end=670
+  _MODEL._serialized_start=673
+  _MODEL._serialized_end=989
+  _MODELNAME._serialized_start=991
+  _MODELNAME._serialized_end=1016
+  _LISTMODELSRESPONSE._serialized_start=1018
+  _LISTMODELSRESPONSE._serialized_end=1068
+  _WORKER._serialized_start=1070
+  _WORKER._serialized_end=1130
+  _LISTWORKERSRESPONSE._serialized_start=1132
+  _LISTWORKERSRESPONSE._serialized_end=1185
+  _CREATEINFERENCEWORKERREQUEST._serialized_start=1188
+  _CREATEINFERENCEWORKERREQUEST._serialized_end=1420
+  _INFERENCEWORKER._serialized_start=1422
+  _INFERENCEWORKER._serialized_end=1460
+  _HAVEN._serialized_start=1598
+  _HAVEN._serialized_end=2328
 # @@protoc_insertion_point(module_scope)
```

### Comparing `havenpy-0.0.7/havenpy/pb/manager_pb2_grpc.py` & `havenpy-0.2.0/havenpy/pb/manager_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,21 +18,36 @@
                 '/haven.Haven/Setup',
                 request_serializer=manager__pb2.SetupRequest.SerializeToString,
                 response_deserializer=manager__pb2.SetupResponse.FromString,
                 )
         self.ChatCompletion = channel.unary_stream(
                 '/haven.Haven/ChatCompletion',
                 request_serializer=manager__pb2.ChatCompletionRequest.SerializeToString,
-                response_deserializer=manager__pb2.ChatCompletionResponse.FromString,
+                response_deserializer=manager__pb2.CompletionResponse.FromString,
+                )
+        self.Completion = channel.unary_stream(
+                '/haven.Haven/Completion',
+                request_serializer=manager__pb2.CompletionRequest.SerializeToString,
+                response_deserializer=manager__pb2.CompletionResponse.FromString,
                 )
         self.ListModels = channel.unary_unary(
                 '/haven.Haven/ListModels',
                 request_serializer=manager__pb2.Empty.SerializeToString,
                 response_deserializer=manager__pb2.ListModelsResponse.FromString,
                 )
+        self.AddModel = channel.unary_unary(
+                '/haven.Haven/AddModel',
+                request_serializer=manager__pb2.Model.SerializeToString,
+                response_deserializer=manager__pb2.Empty.FromString,
+                )
+        self.DeleteModel = channel.unary_unary(
+                '/haven.Haven/DeleteModel',
+                request_serializer=manager__pb2.ModelName.SerializeToString,
+                response_deserializer=manager__pb2.Empty.FromString,
+                )
         self.ListWorkers = channel.unary_unary(
                 '/haven.Haven/ListWorkers',
                 request_serializer=manager__pb2.Empty.SerializeToString,
                 response_deserializer=manager__pb2.ListWorkersResponse.FromString,
                 )
         self.CreateInferenceWorker = channel.unary_unary(
                 '/haven.Haven/CreateInferenceWorker',
@@ -63,27 +78,45 @@
         """Setup (first time starting the manager)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ChatCompletion(self, request, context):
-        """Generate text from a prompt.
+        """Generate text.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def Completion(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListModels(self, request, context):
         """Get the list of models and their descriptions.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def AddModel(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteModel(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListWorkers(self, request, context):
         """Get the list of workers and their statuses.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -119,21 +152,36 @@
                     servicer.Setup,
                     request_deserializer=manager__pb2.SetupRequest.FromString,
                     response_serializer=manager__pb2.SetupResponse.SerializeToString,
             ),
             'ChatCompletion': grpc.unary_stream_rpc_method_handler(
                     servicer.ChatCompletion,
                     request_deserializer=manager__pb2.ChatCompletionRequest.FromString,
-                    response_serializer=manager__pb2.ChatCompletionResponse.SerializeToString,
+                    response_serializer=manager__pb2.CompletionResponse.SerializeToString,
+            ),
+            'Completion': grpc.unary_stream_rpc_method_handler(
+                    servicer.Completion,
+                    request_deserializer=manager__pb2.CompletionRequest.FromString,
+                    response_serializer=manager__pb2.CompletionResponse.SerializeToString,
             ),
             'ListModels': grpc.unary_unary_rpc_method_handler(
                     servicer.ListModels,
                     request_deserializer=manager__pb2.Empty.FromString,
                     response_serializer=manager__pb2.ListModelsResponse.SerializeToString,
             ),
+            'AddModel': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddModel,
+                    request_deserializer=manager__pb2.Model.FromString,
+                    response_serializer=manager__pb2.Empty.SerializeToString,
+            ),
+            'DeleteModel': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteModel,
+                    request_deserializer=manager__pb2.ModelName.FromString,
+                    response_serializer=manager__pb2.Empty.SerializeToString,
+            ),
             'ListWorkers': grpc.unary_unary_rpc_method_handler(
                     servicer.ListWorkers,
                     request_deserializer=manager__pb2.Empty.FromString,
                     response_serializer=manager__pb2.ListWorkersResponse.SerializeToString,
             ),
             'CreateInferenceWorker': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateInferenceWorker,
@@ -191,15 +239,32 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/haven.Haven/ChatCompletion',
             manager__pb2.ChatCompletionRequest.SerializeToString,
-            manager__pb2.ChatCompletionResponse.FromString,
+            manager__pb2.CompletionResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Completion(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/haven.Haven/Completion',
+            manager__pb2.CompletionRequest.SerializeToString,
+            manager__pb2.CompletionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListModels(request,
             target,
             options=(),
@@ -213,14 +278,48 @@
         return grpc.experimental.unary_unary(request, target, '/haven.Haven/ListModels',
             manager__pb2.Empty.SerializeToString,
             manager__pb2.ListModelsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def AddModel(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/haven.Haven/AddModel',
+            manager__pb2.Model.SerializeToString,
+            manager__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteModel(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/haven.Haven/DeleteModel',
+            manager__pb2.ModelName.SerializeToString,
+            manager__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListWorkers(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

