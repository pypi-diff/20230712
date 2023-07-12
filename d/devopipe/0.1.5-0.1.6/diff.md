# Comparing `tmp/devopipe-0.1.5.tar.gz` & `tmp/devopipe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopipe-0.1.5.tar", max compression
+gzip compressed data, was "devopipe-0.1.6.tar", max compression
```

## Comparing `devopipe-0.1.5.tar` & `devopipe-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0        0 2023-07-11 21:36:42.178982 devopipe-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-11 21:36:42.178982 devopipe-0.1.5/devopipe/__init__.py
--rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.5/devopipe/src/downloaded_template.yaml
--rwxr-xr-x   0        0        0    19388 2023-07-11 21:33:34.471235 devopipe-0.1.5/devopipe/src/main.py
--rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.5/devopipe/src/setup_template.yaml
--rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
--rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
--rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.5/devopipe/src/templates/IaC/aws/blueprints.tf
--rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.5/devopipe/src/templates/IaC/aws/create-namespace.yaml
--rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.5/devopipe/src/templates/IaC/aws/create-vcluster.yaml
--rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.5/devopipe/src/templates/IaC/aws/developer-role.tf
--rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.5/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
--rwxr-xr-x   0        0        0     1818 2023-07-08 07:27:31.748556 devopipe-0.1.5/devopipe/src/templates/IaC/aws/main.tf
--rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/argocd.yaml
--rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
--rwxr-xr-x   0        0        0      191 2023-07-08 07:28:37.216100 devopipe-0.1.5/devopipe/src/templates/IaC/aws/variables.tf
--rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.5/devopipe/src/templates/IaC/aws/vpc-module.tf
--rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
--rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
--rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
--rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/get-artifact.yaml
--rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/set-artifact.yaml
--rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment.yaml
--rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
--rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
--rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
--rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
--rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
--rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/service-account.yaml
--rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/storage.yaml
--rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.5/devopipe/src/templates/tests/database-sonarqube.yaml
--rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.5/devopipe/src/templates/tests/deployment-sonarqube.yaml
--rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.5/devopipe/src/templates/tests/storage_sonarqube.yaml
--rw-r--r--   0        0        0      486 2023-07-11 21:36:44.118982 devopipe-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:11:22.230874 devopipe-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 16:11:22.230874 devopipe-0.1.6/devopipe/__init__.py
+-rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.6/devopipe/src/downloaded_template.yaml
+-rwxr-xr-x   0        0        0    21603 2023-07-12 15:44:35.909968 devopipe-0.1.6/devopipe/src/main.py
+-rwxr-xr-x   0        0        0     1702 2023-07-12 11:45:55.178536 devopipe-0.1.6/devopipe/src/runnable/terraform/aws/main.tf
+-rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.6/devopipe/src/setup_template.yaml
+-rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
+-rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
+-rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.6/devopipe/src/templates/IaC/aws/blueprints.tf
+-rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.6/devopipe/src/templates/IaC/aws/create-namespace.yaml
+-rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.6/devopipe/src/templates/IaC/aws/create-vcluster.yaml
+-rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.6/devopipe/src/templates/IaC/aws/developer-role.tf
+-rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.6/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
+-rwxr-xr-x   0        0        0     1793 2023-07-12 15:42:22.516547 devopipe-0.1.6/devopipe/src/templates/IaC/aws/main.tf
+-rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/argocd.yaml
+-rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
+-rwxr-xr-x   0        0        0      361 2023-07-12 15:42:45.256010 devopipe-0.1.6/devopipe/src/templates/IaC/aws/variables.tf
+-rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.6/devopipe/src/templates/IaC/aws/vpc-module.tf
+-rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
+-rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
+-rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
+-rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/get-artifact.yaml
+-rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/set-artifact.yaml
+-rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment.yaml
+-rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
+-rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
+-rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
+-rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
+-rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
+-rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/service-account.yaml
+-rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/storage.yaml
+-rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.6/devopipe/src/templates/tests/database-sonarqube.yaml
+-rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.6/devopipe/src/templates/tests/deployment-sonarqube.yaml
+-rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.6/devopipe/src/templates/tests/storage_sonarqube.yaml
+-rw-r--r--   0        0        0      486 2023-07-12 16:11:24.130874 devopipe-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.6/PKG-INFO
```

### Comparing `devopipe-0.1.5/devopipe/src/main.py` & `devopipe-0.1.6/devopipe/src/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import typer
 import os
 import shutil
 from pathlib import Path
 from string import Template
 from jinja2 import Environment, FileSystemLoader
 import yaml
+import subprocess
+import random
 
 
 app = typer.Typer()
 
 
 @app.command()
 def version():
@@ -171,15 +173,23 @@
 
     # mount Terraform, Kubernetes
     if service_provider == "AWS":
         template_dir_terra = ["templates", "IaC", "aws"]
         template_dir_kubernetes = ["templates", "kubernetes"]
         template_dir_kubernetes_apps = ["templates", "kubernetes", "apps/"]
         template_dir_kub_cloud = ["templates", "kubernetes", "aws/"]
-        mountTerraformAWS(name_cluster, environment_names, region, template_dir_terra)
+        
+        arr = ["runnable", "terraform", "aws"]
+        script_directory = os.path.dirname(os.path.abspath(__file__))
+        #template_dir = os.path.join(script_directory, "templates","ci-pipeline")
+        template_dir_source = os.path.join(script_directory, *arr)
+        bucket_name = name_cluster.lower() + "-state-bucket-" + "".join([str(random.randint(0, 9)) for _ in range(6)])
+        dynamodb_table = f'terraform-state-locking-{name_cluster.lower()}'
+        create_aws_resources(template_dir_source, bucket_name, dynamodb_table ,region, name_cluster)
+        mountTerraformAWS(name_cluster, environment_names, region, bucket_name, template_dir_terra)
         mountKubernetesAWS(name_cluster, environment_names, region, template_dir_kubernetes, template_dir_kubernetes_apps, template_dir_kub_cloud)
 
 
     # mount CD tool
     if cd_tool == "Argocd":
         template_dir_argocd = ["templates","IaC","aws", "argocd"]
         mountArgoCD(environment_names, template_dir_argocd)
@@ -261,22 +271,23 @@
         save_template(render_template(template_dir_kubernetes_apps, "deployment.yaml", {}), folder_path_env + "/deployment.yaml")
         save_template(render_template(template_dir_kubernetes_apps, "pgadmin-deploy.yaml", {}), folder_path_env + "/pgadmin-deploy.yaml")
         save_template(render_template(template_dir_kubernetes_apps, "pgadmin-secret.yaml", {}), folder_path_env + "/pgadmin-secret.yaml")
 
 
 
 
-def mountTerraformAWS(name_cluster, environment_names, region, template_dir):
+def mountTerraformAWS(name_cluster, environment_names, region, bucket_name, template_dir):
     folder_path = "./IaC/"
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
     rendered_template_variables = render_template(template_dir, "variables.tf", {
         'cluster_name': name_cluster,
-        'state_region': region
+        'state_region': region,
+        'bucket_name': bucket_name
     })
 
     rendered_template_namespaces = ""
     rendered_template_vclusters = ""
 
     for i, env_name in enumerate(environment_names):
         namespace_name = name_cluster.lower() + '-' + env_name.lower()
@@ -401,14 +412,37 @@
 #    filled_template = load_template(template_file, variables)
 #    output_file = f"{os.path.splitext(template_file)[0]}.yml"  # Output file name based on the template file
 #    save_template(filled_template, output_file)
 
 
 
 
+def create_aws_resources(file_path, bucket_name, dynamodb_table, region, project_name):
+    # Run the Terraform command as a subprocess
+    #subprocess.run(['terraform', 'apply', '-auto-approve', '-input=false', '-var', f'bucket_name={bucket_name}', '-var', f'region={region}', '-var', f'project_name={project_name}'], cwd=file_path)
+    typer.echo(bucket_name)
+    # Create S3 bucket
+    subprocess.run(['aws', 's3api', 'create-bucket', '--bucket', bucket_name, '--region', region])
+
+    # Enable versioning for the S3 bucket
+    subprocess.run(['aws', 's3api', 'put-bucket-versioning', '--bucket', bucket_name, '--versioning-configuration', 'Status=Enabled'])
+
+    # Create DynamoDB table
+    subprocess.run(['aws', 'dynamodb', 'create-table', '--table-name', dynamodb_table, '--attribute-definitions', 'AttributeName=LockID,AttributeType=S', '--key-schema', 'AttributeName=LockID,KeyType=HASH', '--billing-mode', 'PAY_PER_REQUEST'])
+
+    print(f'{project_name.lower()}_front')
+
+    # Create ECR repositories
+    subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_front'])
+    subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_back'])
+    subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_dbmigrations'])
+
+
+
+
 
 def read_yaml(file_path):
     with open(file_path, "r") as file:
         yaml_data = yaml.safe_load(file)
     return yaml_data
 
 
@@ -428,14 +462,20 @@
     rendered_template = template.render({
         'artifact_tar_name' : "artifact_tar",
         'artifact_pipeline_name': "artifact_name"
     })
     typer.echo(rendered_template)
 
 
+@app.command()
+def te():
+    random_numbers = ''.join([str(random.randint(0, 9)) for _ in range(6)])
+    print(random_numbers)
+    print(type(random_numbers))
+
 
 
 
 
 @app.command()
 def template():
     source_file = "setup_template.yaml"
```

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/argocd.yaml` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/argocd.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/blueprints.tf` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/blueprints.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/developer-role.tf` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/developer-role.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/kubernetes-addons.tf` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/kubernetes-addons.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/main.tf` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/main.tf`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 provider "aws" {
   region = "us-east-1"
 }
 
 terraform {
   backend "s3" {
-    bucket         = "terraform-state-bucket-devopipe"
+    bucket         = var.bucket_name
     key            = "global/s3/terraform.tfstate"
     region         = var.state_region
-    dynamodb_table = "terraform-state-locking"
+    dynamodb_table = var.dynamodb_table
     encrypt        = true
   }
 }
 
 # state-bucket-name = "terraform-state-bucket-devopipe"
 # state-region = "us-east-1"
```

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/IaC/aws/vpc-module.tf` & `devopipe-0.1.6/devopipe/src/templates/IaC/aws/vpc-module.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml` & `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml` & `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml` & `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/get-artifact.yaml` & `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/get-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/set-artifact.yaml` & `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/set-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment.yaml` & `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml` & `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_database.yaml` & `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_database.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml` & `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml` & `devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/tests/database-sonarqube.yaml` & `devopipe-0.1.6/devopipe/src/templates/tests/database-sonarqube.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.5/devopipe/src/templates/tests/deployment-sonarqube.yaml` & `devopipe-0.1.6/devopipe/src/templates/tests/deployment-sonarqube.yaml`

 * *Files identical despite different names*

