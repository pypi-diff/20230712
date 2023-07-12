# Comparing `tmp/1stcaptcha-1.0.2.tar.gz` & `tmp/1stcaptcha-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1stcaptcha-1.0.2.tar", max compression
+gzip compressed data, was "1stcaptcha-1.0.3.tar", max compression
```

## Comparing `1stcaptcha-1.0.2.tar` & `1stcaptcha-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1508 2023-07-02 11:06:39.282921 1stcaptcha-1.0.2/README.md
--rw-r--r--   0        0        0     5910 2023-07-12 15:30:30.128050 1stcaptcha-1.0.2/onest_captcha/__init__.py
--rw-r--r--   0        0        0      724 2023-07-12 15:33:20.344160 1stcaptcha-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 1stcaptcha-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1869 2023-07-12 15:35:58.431699 1stcaptcha-1.0.3/README.md
+-rw-r--r--   0        0        0     5910 2023-07-12 15:30:30.128050 1stcaptcha-1.0.3/onest_captcha/__init__.py
+-rw-r--r--   0        0        0      724 2023-07-12 15:36:35.386056 1stcaptcha-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 1stcaptcha-1.0.3/PKG-INFO
```

### Comparing `1stcaptcha-1.0.2/README.md` & `1stcaptcha-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,26 @@
 result = client.recaptcha_v2_task_proxyless(site_url, site_key, invisible=invisible)
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
+## solver recaptcha v3:
+
+```python
+token = client.recaptcha_v3_task_proxyless(site_key="YOUR_SITE_KEY",
+                                           site_url="YOUR_SITE_URL",
+                                           page_action="YOUR_PAGE_ACTION")
+if result["code"] == 0:  # success:
+    print(result["token"])
+else:  # wrong
+    print(result["messeage"])
+```
+
 ## solve image2text
 
 ```python
 
 result = client.image_to_text(file="1.jpg")
 if result["code"] == 0:  # success:
     print(result["token"])
```

### Comparing `1stcaptcha-1.0.2/onest_captcha/__init__.py` & `1stcaptcha-1.0.3/onest_captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `1stcaptcha-1.0.2/pyproject.toml` & `1stcaptcha-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "1stcaptcha"
 packages = [
     { include = "onest_captcha" },
 ]
-version = "1.0.2"
+version = "1.0.3"
 description = "Solver recaptchaV2, recaptchaV3, hcaptcha, funcaptcha, imageToText, Zalo Captcha,.... Super fast and cheapest"
 authors = ["NguyenLinhUET <nguyenlinh.uet@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/1stcaptcha/1stcaptcha-python"
 homepage = "https://github.com/1stcaptcha/1stcaptcha-python"
 license = "MIT"
 keywords = ["1stcaptcha", "recaptcha", "recaptchav3", "hcaptcha", "funcaptcha", "imagetotext", "zalo captcha", "solver captcha"]
```

### Comparing `1stcaptcha-1.0.2/PKG-INFO` & `1stcaptcha-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1stcaptcha
-Version: 1.0.2
+Version: 1.0.3
 Summary: Solver recaptchaV2, recaptchaV3, hcaptcha, funcaptcha, imageToText, Zalo Captcha,.... Super fast and cheapest
 Home-page: https://github.com/1stcaptcha/1stcaptcha-python
 License: MIT
 Keywords: 1stcaptcha,recaptcha,recaptchav3,hcaptcha,funcaptcha,imagetotext,zalo captcha,solver captcha
 Author: NguyenLinhUET
 Author-email: nguyenlinh.uet@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -51,14 +51,26 @@
 result = client.recaptcha_v2_task_proxyless(site_url, site_key, invisible=invisible)
 if result["code"] == 0:  # success:
     print(result["token"])
 else:  # wrong
     print(result["messeage"])
 ```
 
+## solver recaptcha v3:
+
+```python
+token = client.recaptcha_v3_task_proxyless(site_key="YOUR_SITE_KEY",
+                                           site_url="YOUR_SITE_URL",
+                                           page_action="YOUR_PAGE_ACTION")
+if result["code"] == 0:  # success:
+    print(result["token"])
+else:  # wrong
+    print(result["messeage"])
+```
+
 ## solve image2text
 
 ```python
 
 result = client.image_to_text(file="1.jpg")
 if result["code"] == 0:  # success:
     print(result["token"])
```

