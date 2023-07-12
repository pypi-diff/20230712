# Comparing `tmp/estela-0.2.3.tar.gz` & `tmp/estela-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estela-0.2.3.tar", last modified: Thu Jun 15 21:56:57 2023, max compression
+gzip compressed data, was "estela-0.2.4.tar", last modified: Wed Jul 12 20:31:04 2023, max compression
```

## Comparing `estela-0.2.3.tar` & `estela-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 21:56:57.570462 estela-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 21:56:50.000000 estela-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 21:56:57.000000 estela-0.2.3/estela.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.566461 estela-0.2.3/estela_cli/create/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/create/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/data/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/data/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/delete/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/estela_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/list/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/list/spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/stop/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/stop/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:56:57.570462 estela-0.2.3/estela_cli/update/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/update/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-15 21:56:50.000000 estela-0.2.3/estela_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:56:57.570462 estela-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-15 21:56:50.000000 estela-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-12 20:31:04.117454 estela-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-12 20:30:55.000000 estela-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 20:31:04.000000 estela-0.2.4/estela.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/create/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/create/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/create/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/data/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/delete/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/estela_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/list/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/list/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/list/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/list/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/stop/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:04.117454 estela-0.2.4/estela_cli/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/update/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/update/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-12 20:30:55.000000 estela-0.2.4/estela_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:31:04.117454 estela-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-12 20:30:55.000000 estela-0.2.4/setup.py
```

### Comparing `estela-0.2.3/README.md` & `estela-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center"> estela CLI </h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![version](https://img.shields.io/badge/version-0.2.3-blue)](https://github.com/bitmakerla/estela-cli)
+[![version](https://img.shields.io/badge/version-0.2.4-blue)](https://github.com/bitmakerla/estela-cli)
 [![python-version](https://img.shields.io/badge/python-v3.10-orange)](https://www.python.org)
 
 
 estela CLI is a command line client to interact with the estela API. It allows the user to perform the following actions:
 - Link a Scrapy project with a project in estela.
 - Create projects, jobs, and cronjobs in estela.
 - Get the data of a job.
```

### Comparing `estela-0.2.3/estela.egg-info/SOURCES.txt` & `estela-0.2.4/estela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/__main__.py` & `estela-0.2.4/estela_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/context.py` & `estela-0.2.4/estela_cli/context.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/create/cronjob.py` & `estela-0.2.4/estela_cli/create/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/create/job.py` & `estela-0.2.4/estela_cli/create/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/data/job.py` & `estela-0.2.4/estela_cli/data/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/delete/project.py` & `estela-0.2.4/estela_cli/delete/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/deploy.py` & `estela-0.2.4/estela_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/estela_client.py` & `estela-0.2.4/estela_cli/estela_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,23 @@
 
     def create_project(self, name):
         endpoint = "projects"
         data = {"name": name}
         response = self.post(endpoint, data=data)
         self.check_status(response, 201)
         return response.json()
+    
+    def update_project(self, pid, **kwargs):
+        endpoint = "projects/{}".format(pid)
+        data = {
+            **kwargs,
+        }
+        response = self.put(endpoint, data=data)
+        self.check_status(response, 200)
+        return response.json()
 
     def delete_project(self, pid):
         endpoint = "projects/{}".format(pid)
         response = self.delete(endpoint)
         self.check_status(response, 204)
 
     def get_spiders(self, pid):
```

### Comparing `estela-0.2.3/estela_cli/init.py` & `estela-0.2.4/estela_cli/init.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,29 @@
     get_project_path,
     get_estela_yaml_path,
     get_estela_dockerfile_path,
 )
 from estela_cli.templates import (
     DATA_DIR,
     DOCKER_DEFAULT_ENTRYPOINT,
+    DOCKER_REQUESTS_ENTRYPOINT,
     DOCKERFILE,
     DOCKERFILE_NAME,
     ESTELA_YAML,
     ESTELA_YAML_NAME,
     DOCKER_DEFAULT_REQUIREMENTS,
     DOCKER_DEFAULT_PYTHON_VERSION,
     ESTELA_DIR,
 )
 
+ALLOWED_PLATFORMS = ["scrapy", "requests"]
+SHORT_HELP = "Initialize estela project for existing web scraping project"
 
-SHORT_HELP = "Initialize estela project for existing scrapy project"
 
-
-def gen_estela_yaml(estela_client, pid=None):
+def gen_estela_yaml(estela_client, entrypoint_path, pid=None):
     estela_yaml_path = get_estela_yaml_path()
 
     if os.path.exists(estela_yaml_path):
         raise click.ClickException("{} file already exists.".format(ESTELA_YAML_NAME))
 
     try:
         if pid is None:
@@ -42,25 +43,25 @@
 
     template = Template(ESTELA_YAML)
     values = {
         "project_pid": pid,
         "project_data_path": DATA_DIR,
         "python_version": DOCKER_DEFAULT_PYTHON_VERSION,
         "requirements_path": DOCKER_DEFAULT_REQUIREMENTS,
-        "entrypoint": DOCKER_DEFAULT_ENTRYPOINT,
+        "entrypoint": entrypoint_path,
     }
 
     result = template.substitute(values)
 
     with open(estela_yaml_path, "w") as estela_yaml:
         estela_yaml.write(result)
         click.echo("{} file created successfully.".format(ESTELA_YAML_NAME))
 
 
-def gen_dockerfile(requirements_path):
+def gen_dockerfile(requirements_path, entrypoint_path):
     dockerfile_path = get_estela_dockerfile_path()
 
     if os.path.exists(dockerfile_path):
         raise click.ClickException(
             "{}/{} already exists.".format(ESTELA_DIR, DOCKERFILE_NAME)
         )
 
@@ -70,37 +71,53 @@
         with open(requirements_local_path, "w") as requirementes:
             pass
 
     template = Template(DOCKERFILE)
     values = {
         "python_version": DOCKER_DEFAULT_PYTHON_VERSION,
         "requirements_path": requirements_path,
-        "entrypoint": DOCKER_DEFAULT_ENTRYPOINT,
+        "entrypoint": entrypoint_path,
     }
     result = template.substitute(values)
 
     with open(dockerfile_path, "w") as dockerfile:
         dockerfile.write(result)
         click.echo("{}/{} created successfully.".format(ESTELA_DIR, DOCKERFILE_NAME))
 
 
 @click.command(short_help=SHORT_HELP)
 @click.argument("pid", required=True)
 @click.option(
+    "-p",
+    "--platform",
+    type=click.Choice(ALLOWED_PLATFORMS, case_sensitive=False),
+    default="scrapy",
+    help="Platform to use, it can be 'scrapy' or 'requests'",
+    show_default=True,
+)
+@click.option(
     "-r",
     "--requirements",
     default=DOCKER_DEFAULT_REQUIREMENTS,
     help="Relative path to requirements inside your project",
     show_default=True,
 )
-def estela_command(pid, requirements):
+def estela_command(pid, platform, requirements):
     """Initialize estela project
 
     PID is the project's pid
     """
-
+    platform_map = {
+        "scrapy": DOCKER_DEFAULT_ENTRYPOINT,
+        "requests": DOCKER_REQUESTS_ENTRYPOINT,
+    }
     if not os.path.exists(ESTELA_DIR):
         os.makedirs(ESTELA_DIR)
-
     estela_client = login()
-    gen_estela_yaml(estela_client, pid)
-    gen_dockerfile(requirements)
+    try:
+        response = estela_client.update_project(pid, framework=platform.upper(), action="update")
+    except Exception as e:
+        raise click.ClickException("Could not update framework project: %s" % str(e))
+    finally:
+        click.echo(f"{pid} is initialized as a {platform.capitalize()} project.")
+    gen_estela_yaml(estela_client, platform_map[platform], pid)
+    gen_dockerfile(requirements, platform_map[platform])
```

### Comparing `estela-0.2.3/estela_cli/list/cronjob.py` & `estela-0.2.4/estela_cli/list/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/list/job.py` & `estela-0.2.4/estela_cli/list/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/list/spider.py` & `estela-0.2.4/estela_cli/list/spider.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/login.py` & `estela-0.2.4/estela_cli/login.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/logout.py` & `estela-0.2.4/estela_cli/logout.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/stop/job.py` & `estela-0.2.4/estela_cli/stop/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/templates.py` & `estela-0.2.4/estela_cli/templates.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 
 ESTELA_DIR = ".estela"
 
 DATA_DIR = "project_data"
 
 DOCKER_APP_DIR = "/usr/src/app"
 
-DOCKER_DEFAULT_PYTHON_VERSION = "3.6"
+DOCKER_DEFAULT_PYTHON_VERSION = "3.9"
 
 DOCKER_DEFAULT_REQUIREMENTS = "requirements.txt"
 
 DOCKER_DEFAULT_ENTRYPOINT = "git+https://github.com/bitmakerla/estela-entrypoint.git"
 
+DOCKER_REQUESTS_ENTRYPOINT = "git+https://github.com/bitmakerla/estela-requests-entrypoint"
+
 DOCKERFILE_NAME = "Dockerfile-estela"
 
 DOCKERFILE = """\
 FROM python:$python_version
 
 # must be in base image
 RUN pip install $entrypoint
```

### Comparing `estela-0.2.3/estela_cli/update/cronjob.py` & `estela-0.2.4/estela_cli/update/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/update/job.py` & `estela-0.2.4/estela_cli/update/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/estela_cli/utils.py` & `estela-0.2.4/estela_cli/utils.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.3/setup.py` & `estela-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="estela",
-    version="0.2.3",
+    version="0.2.4",
     description="Estela Command Line Interface",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "estela = estela_cli.__main__:cli",
         ],
     },
```

