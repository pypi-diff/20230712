# Comparing `tmp/devopipe-0.1.6.tar.gz` & `tmp/devopipe-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopipe-0.1.6.tar", max compression
+gzip compressed data, was "devopipe-0.1.7.tar", max compression
```

## Comparing `devopipe-0.1.6.tar` & `devopipe-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:11:22.230874 devopipe-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-12 16:11:22.230874 devopipe-0.1.6/devopipe/__init__.py
--rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.6/devopipe/src/downloaded_template.yaml
--rwxr-xr-x   0        0        0    21603 2023-07-12 15:44:35.909968 devopipe-0.1.6/devopipe/src/main.py
--rwxr-xr-x   0        0        0     1702 2023-07-12 11:45:55.178536 devopipe-0.1.6/devopipe/src/runnable/terraform/aws/main.tf
--rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.6/devopipe/src/setup_template.yaml
--rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
--rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
--rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.6/devopipe/src/templates/IaC/aws/blueprints.tf
--rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.6/devopipe/src/templates/IaC/aws/create-namespace.yaml
--rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.6/devopipe/src/templates/IaC/aws/create-vcluster.yaml
--rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.6/devopipe/src/templates/IaC/aws/developer-role.tf
--rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.6/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
--rwxr-xr-x   0        0        0     1793 2023-07-12 15:42:22.516547 devopipe-0.1.6/devopipe/src/templates/IaC/aws/main.tf
--rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/argocd.yaml
--rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
--rwxr-xr-x   0        0        0      361 2023-07-12 15:42:45.256010 devopipe-0.1.6/devopipe/src/templates/IaC/aws/variables.tf
--rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.6/devopipe/src/templates/IaC/aws/vpc-module.tf
--rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
--rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
--rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
--rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/get-artifact.yaml
--rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.6/devopipe/src/templates/ci-pipeline/set-artifact.yaml
--rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment.yaml
--rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
--rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
--rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
--rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
--rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
--rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/service-account.yaml
--rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/storage.yaml
--rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.6/devopipe/src/templates/tests/database-sonarqube.yaml
--rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.6/devopipe/src/templates/tests/deployment-sonarqube.yaml
--rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.6/devopipe/src/templates/tests/storage_sonarqube.yaml
--rw-r--r--   0        0        0      486 2023-07-12 16:11:24.130874 devopipe-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 19:15:53.567697 devopipe-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 19:15:53.567697 devopipe-0.1.7/devopipe/__init__.py
+-rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.7/devopipe/src/downloaded_template.yaml
+-rwxr-xr-x   0        0        0    23128 2023-07-12 19:09:03.758289 devopipe-0.1.7/devopipe/src/main.py
+-rwxr-xr-x   0        0        0     1702 2023-07-12 11:45:55.178536 devopipe-0.1.7/devopipe/src/runnable/terraform/aws/main.tf
+-rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.7/devopipe/src/setup_template.yaml
+-rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.7/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
+-rwxr-xr-x   0        0        0      437 2023-07-12 17:02:03.879302 devopipe-0.1.7/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
+-rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.7/devopipe/src/templates/IaC/aws/blueprints.tf
+-rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.7/devopipe/src/templates/IaC/aws/create-namespace.yaml
+-rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.7/devopipe/src/templates/IaC/aws/create-vcluster.yaml
+-rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.7/devopipe/src/templates/IaC/aws/developer-role.tf
+-rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.7/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
+-rwxr-xr-x   0        0        0     1793 2023-07-12 15:42:22.516547 devopipe-0.1.7/devopipe/src/templates/IaC/aws/main.tf
+-rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.7/devopipe/src/templates/IaC/aws/values/argocd.yaml
+-rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.7/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
+-rwxr-xr-x   0        0        0      361 2023-07-12 15:42:45.256010 devopipe-0.1.7/devopipe/src/templates/IaC/aws/variables.tf
+-rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.7/devopipe/src/templates/IaC/aws/vpc-module.tf
+-rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.7/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
+-rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.7/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
+-rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.7/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
+-rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.7/devopipe/src/templates/ci-pipeline/get-artifact.yaml
+-rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.7/devopipe/src/templates/ci-pipeline/set-artifact.yaml
+-rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment.yaml
+-rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
+-rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
+-rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
+-rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
+-rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.7/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
+-rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.7/devopipe/src/templates/kubernetes/aws/service-account.yaml
+-rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.7/devopipe/src/templates/kubernetes/aws/storage.yaml
+-rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.7/devopipe/src/templates/tests/database-sonarqube.yaml
+-rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.7/devopipe/src/templates/tests/deployment-sonarqube.yaml
+-rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.7/devopipe/src/templates/tests/storage_sonarqube.yaml
+-rw-r--r--   0        0        0      486 2023-07-12 19:15:56.003865 devopipe-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.7/PKG-INFO
```

### Comparing `devopipe-0.1.6/devopipe/src/main.py` & `devopipe-0.1.7/devopipe/src/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,42 +91,42 @@
         database = yaml_values["init"]["database"]
         cd_tool = yaml_values["init"]["cd_tool"]
         monitoring_stack = yaml_values["init"]["monitoring_stack"]
 
 
     else:
         print("else")
-        ###########Give me: name of frontend, backend, databse, flyway image on docker compose,
-        ########### What type of migration tool are you using
-        ##########typer.echo("What CI will you use?")
-        ##########ci_system = choose_option(["Azure Pipelines", "GitHub Actions"]) # For Pipeline
-        ##########typer.echo("What tests plataform will you use?")
-        ##########tests = choose_option(["Sonarqube", "Codacy"]) # For Kubernetes or Pipeline
-        ##########typer.echo("What service provider will you use?")
-        ##########service_provider = choose_option(["On-prem", "AWS", "Azure", "GCP"]) # For Kubernetes and Terraform
-        ##########region = typer.prompt("Wich cloud region do you wanna use? ")
-        ######################num_environments = int(typer.prompt("How many environments will you have? ")) # For kubernetes and Terraform
-        ##########environment_names = typer.prompt("What are the names of your environments (separated by commas)? ") # For kubernetes and Terraform
-        ##########registry = choose_option(["ECR (Elastic Container Registry)", "ACR (Azure Container Registry)", "Docker Hub"]) # For Pipeline and Kubernetes
-        ##########typer.echo("Your repositories are:")
-        ##########repository_type = choose_option(["Public", "Private"]) # For Pipeline and Terraform 
-        ##########typer.echo("What migration tool will you use?")
-        ##########monitoring_stack = choose_option(["Flyway", "Liquibase"]) # For Terraform
-        ##########typer.echo("What stack do you wanna use for monitorization?")
-        ###########Ask for Argocd
-        ########### Bitbucket or github
-        ##########typer.echo("What Source Control will you use?")
-        ##########source_control = choose_option(["Bitbucket", "GitHub"]) # For Source Control
-        ########### Qual base de dados
-        ##########typer.echo("What Database will you use?")
-        ##########database = choose_option(["Postgres"]) # For Source Control
-        ##########typer.echo("Which Delievery tool will you use?")
-        ##########cd_tool = choose_option(["Argocd"]) # For Source Control
-        ##########typer.echo("Which Monitoring Stack will you use?")
-        ##########monitoring_stack = choose_option(["ELK", "Prometheus + Loki"]) # For Terraform
+        #Give me: name of frontend, backend, databse, flyway image on docker compose,
+        # What type of migration tool are you using
+        typer.echo("What CI will you use?")
+        ci_system = choose_option(["Azure Pipelines", "GitHub Actions"]) # For Pipeline
+        typer.echo("What tests plataform will you use?")
+        tests = choose_option(["Sonarqube", "Codacy"]) # For Kubernetes or Pipeline
+        typer.echo("What service provider will you use?")
+        service_provider = choose_option(["On-prem", "AWS", "Azure", "GCP"]) # For Kubernetes and Terraform
+        region = typer.prompt("Wich cloud region do you wanna use? ")
+        ############num_environments = int(typer.prompt("How many environments will you have? ")) # For kubernetes and Terraform
+        environment_names = typer.prompt("What are the names of your environments (separated by commas)? ") # For kubernetes and Terraform
+        registry = choose_option(["ECR (Elastic Container Registry)", "ACR (Azure Container Registry)", "Docker Hub"]) # For Pipeline and Kubernetes
+        typer.echo("Your repositories are:")
+        repository_type = choose_option(["Public", "Private"]) # For Pipeline and Terraform 
+        typer.echo("What migration tool will you use?")
+        monitoring_stack = choose_option(["Flyway", "Liquibase"]) # For Terraform
+        typer.echo("What stack do you wanna use for monitorization?")
+        #Ask for Argocd
+        # Bitbucket or github
+        typer.echo("What Source Control will you use?")
+        source_control = choose_option(["Bitbucket", "GitHub"]) # For Source Control
+        # Qual base de dados
+        typer.echo("What Database will you use?")
+        database = choose_option(["Postgres"]) # For Source Control
+        typer.echo("Which Delievery tool will you use?")
+        cd_tool = choose_option(["Argocd"]) # For Source Control
+        typer.echo("Which Monitoring Stack will you use?")
+        monitoring_stack = choose_option(["ELK", "Prometheus + Loki"]) # For Terraform
 
     ## Create a template object
     #template = Template(template_content)
 
     ## Define the parameters
     #params = {'name': 'John', 'day': 'Monday'}
 
@@ -151,15 +151,14 @@
     typer.echo(f"Database: {database}")
     typer.echo(f"Continuous Delievery Tool: {cd_tool}")
     typer.echo(f"Monitorization: {monitoring_stack}")
 
     if ci_system == "Azure Pipelines":
         template_dir = ["templates","ci-pipeline"]
         pipeline_frontend = mountAzurePipelineFrontend(registry, template_dir)
-        typer.echo(type(pipeline_frontend))
         pipeline_backend = mountAzurePipelineBackend(registry, template_dir)
         #mountAzurePipeline(registry)
     folder_path = "./.azure-pipelines/"
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
     #pipeline_frontend = ruamel.yaml.safe_load(pipeline_frontend)
@@ -196,14 +195,41 @@
 
     # mount test tool
     if tests == "Sonarqube":
         template_dir_sonarqube = ["templates", "tests"]
         mountSonarqube(service_provider, template_dir_sonarqube)
 
 
+    # Generate instructions
+    body = f"""
+        State of IaC already created.
+        Now, execute the next steps:
+        1 - Copy pipelines files to frontend and backend repositories.
+        2 - Go to Azure DevOps, click in Library and add the next variables to a variable_group with name 'AWS_job':
+            - AWS_ACCESS_KEY_ID: AKIAUU3D6KGYQS6JAQSP
+            - AWS_ACCOUNT_ID: 319647797681
+            - AWS_API_REPOSITORY: devopipe_back
+            - AWS_FLYWAY_REPOSITORY: devopipe_dbmigrations
+            - AWS_FRONTEND_REPOSITORY: devopipe_front
+            - AWS_REGION: us-east-1
+            - AWS_SECRET_ACCESS_KEY: <your-token>
+        3 - Commit and push both repositories.
+        4 - Navigate to IaC folder and execute each command:
+            - terraform init
+            - terraform plan
+            - terraform apply --auto-approve
+        5 - Go to the kubernetes repository, commit and push the changes.
+        6 - Connect to argocd container and change password with the next steps:
+            - kubectl get secrets argocd-initial-admin-secret -o yaml -n argocd
+            - echo "password" | base64 -d
+            - Copy the password on the terminal and paste on the argocd values, substitute where is '<your-password>'
+
+    """
+    save_template(body, "./INSTRUCTIONS.TXT")
+
 
 def mountSonarqube(service_provider, template_dir):
     if service_provider == "AWS":
         folder_path = "./kubernetes/aws/"
     
     if not os.path.exists(folder_path):
             os.makedirs(folder_path)
@@ -216,28 +242,35 @@
 def mountArgoCD(environment_names, template_dir):
     template_dir_vcluster_values = ["templates", "IaC", "aws", "values"]
     folder_path = "./IaC/"
     folder_path_argocd = folder_path + "argocd/"
     if not os.path.exists(folder_path_argocd):
         os.makedirs(folder_path_argocd)
 
-    save_template(render_template(template_dir, "argocd.yaml", {}), folder_path_argocd + "argocd.yaml")
-    save_template(render_template(template_dir, "git-repo-secret.yaml", {}), folder_path_argocd + "git-repo-secret.yaml")
+    save_template(render_template(template_dir, "argocd.yaml", {
+        'repoURL': 'https://bitbucket.org/dvtpt/devops-kubernetes/src/main/',
+        'path' : 'environments/aws',
+    }), folder_path_argocd + "argocd.yaml")
+    save_template(render_template(template_dir, "git-repo-secret.yaml", {
+        'url': 'https://bitbucket.org/dvtpt/devops-kubernetes/src/main/',
+        'username': 'danielrodriguesdevo',
+        'password': '<your-password>',
+    }), folder_path_argocd + "git-repo-secret.yaml")
 
     folder_path_values = folder_path + "values/"
     if not os.path.exists(folder_path_values):
         os.makedirs(folder_path_values)
     
     save_template(render_template(template_dir, "argocd.yaml", {}), folder_path_values + "argocd.yaml")
 
     for i, env_name in enumerate(environment_names):
         save_template(render_template(template_dir_vcluster_values, "vcluster-config-init.yaml", {
-            'url': "url_kubernetes",
-            'username': "username",
-            'password': "password",
+            'url': "https://bitbucket.org/dvtpt/devops-kubernetes/src/main/",
+            'username': "danielrodriguesdevo",
+            'password': "<your-password>",
             'argocd_name': env_name.lower() + "-apps",
             'argocd_path':  "environments/" + env_name.lower() + "/apps"
         }), folder_path_values + "vcluster-" + env_name.lower() + ".yaml")
 
 
 
 def mountKubernetesAWS(name_cluster, environment_names, region, template_dir, template_dir_kubernetes_apps, template_dir_cloud):
@@ -321,30 +354,30 @@
 
     rendered_template_frontend = render_template(template_dir, "azure-pipelines.yaml", {
         'set_artifacts_build': phases_frontend[0],
         'get_artifacts_deploy': phases_frontend[1],
         'deploy_artifact': phases_frontend[2]
     })
     
-    typer.echo(rendered_template_frontend)
+    #typer.echo(rendered_template_frontend)
 
     return rendered_template_frontend
 
 
 def mountAzurePipelineBackend(registry, template_dir):
     phases_api = mountAzurePipeline(template_dir, registry, 'backend_fastapi', 'Fastapi_Artifact', ['AWS_API_REPOSITORY', 'backend_fastapi'] )
     phases_data_migration = mountAzurePipeline(template_dir, registry, 'frontend_image', 'frontend_artifact', ['AWS_FLYWAY_REPOSITORY', 'migrations_flyway'] )
 
     rendered_template_backend = render_template(template_dir, "azure-pipelines.yaml", {
         'set_artifacts_build': phases_api[0] + phases_data_migration[0],
         'get_artifacts_deploy': phases_api[1] + phases_data_migration[1],
         'deploy_artifact': phases_api[2] + phases_data_migration[2]
     })
     
-    typer.echo(rendered_template_backend)
+    #typer.echo(rendered_template_backend)
 
     return rendered_template_backend
 
 
 
 
 def mountAzurePipeline(template_dir, registry, artifact_tar, artifact_name, registry_variables ):
@@ -415,59 +448,62 @@
 
 
 
 
 def create_aws_resources(file_path, bucket_name, dynamodb_table, region, project_name):
     # Run the Terraform command as a subprocess
     #subprocess.run(['terraform', 'apply', '-auto-approve', '-input=false', '-var', f'bucket_name={bucket_name}', '-var', f'region={region}', '-var', f'project_name={project_name}'], cwd=file_path)
-    typer.echo(bucket_name)
     # Create S3 bucket
     subprocess.run(['aws', 's3api', 'create-bucket', '--bucket', bucket_name, '--region', region])
 
+    typer.echo("Bucket created with name " + bucket_name)
+
     # Enable versioning for the S3 bucket
     subprocess.run(['aws', 's3api', 'put-bucket-versioning', '--bucket', bucket_name, '--versioning-configuration', 'Status=Enabled'])
 
+    
     # Create DynamoDB table
     subprocess.run(['aws', 'dynamodb', 'create-table', '--table-name', dynamodb_table, '--attribute-definitions', 'AttributeName=LockID,AttributeType=S', '--key-schema', 'AttributeName=LockID,KeyType=HASH', '--billing-mode', 'PAY_PER_REQUEST'])
 
-    print(f'{project_name.lower()}_front')
+    typer.echo("DynamoDB table created with name " + dynamodb_table)
+    #print(f'{project_name.lower()}_front')
 
     # Create ECR repositories
     subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_front'])
     subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_back'])
     subprocess.run(['aws', 'ecr', 'create-repository', '--repository-name', f'{project_name.lower()}_dbmigrations'])
-
+    typer.echo("ECR's created")
 
 
 
 
 def read_yaml(file_path):
     with open(file_path, "r") as file:
         yaml_data = yaml.safe_load(file)
     return yaml_data
 
 
-@app.command()
-def testee():
-    arr = ["templates","ci-pipeline"]
-    script_directory = os.path.dirname(os.path.abspath(__file__))
-    #template_dir = os.path.join(script_directory, "templates","ci-pipeline")
-    template_dir_source = os.path.join(script_directory, *arr)
-    typer.echo(script_directory)
-    typer.echo(template_dir_source)
-
-    file_loader = FileSystemLoader(template_dir_source)
-    env = Environment(loader=file_loader)
-    #current_directory_source = os.path.dirname(os.path.abspath(__file__))
-    template = env.get_template("set-artifact.yaml")
-    rendered_template = template.render({
-        'artifact_tar_name' : "artifact_tar",
-        'artifact_pipeline_name': "artifact_name"
-    })
-    typer.echo(rendered_template)
+#@app.command()
+#def testee():
+#    arr = ["templates","ci-pipeline"]
+#    script_directory = os.path.dirname(os.path.abspath(__file__))
+#    #template_dir = os.path.join(script_directory, "templates","ci-pipeline")
+#    template_dir_source = os.path.join(script_directory, *arr)
+#    #typer.echo(script_directory)
+#    #typer.echo(template_dir_source)
+#
+#    file_loader = FileSystemLoader(template_dir_source)
+#    env = Environment(loader=file_loader)
+#    #current_directory_source = os.path.dirname(os.path.abspath(__file__))
+#    template = env.get_template("set-artifact.yaml")
+#    rendered_template = template.render({
+#        'artifact_tar_name' : "artifact_tar",
+#        'artifact_pipeline_name': "artifact_name"
+#    })
+#    #typer.echo(rendered_template)
 
 
 @app.command()
 def te():
     random_numbers = ''.join([str(random.randint(0, 9)) for _ in range(6)])
     print(random_numbers)
     print(type(random_numbers))
```

### Comparing `devopipe-0.1.6/devopipe/src/runnable/terraform/aws/main.tf` & `devopipe-0.1.7/devopipe/src/runnable/terraform/aws/main.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/argocd/argocd.yaml` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/argocd/argocd.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/blueprints.tf` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/blueprints.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/developer-role.tf` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/developer-role.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/kubernetes-addons.tf` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/kubernetes-addons.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/main.tf` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/main.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/IaC/aws/vpc-module.tf` & `devopipe-0.1.7/devopipe/src/templates/IaC/aws/vpc-module.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml` & `devopipe-0.1.7/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml` & `devopipe-0.1.7/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml` & `devopipe-0.1.7/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/get-artifact.yaml` & `devopipe-0.1.7/devopipe/src/templates/ci-pipeline/get-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/ci-pipeline/set-artifact.yaml` & `devopipe-0.1.7/devopipe/src/templates/ci-pipeline/set-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment.yaml` & `devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml` & `devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/deployment_database.yaml` & `devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/deployment_database.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml` & `devopipe-0.1.7/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml` & `devopipe-0.1.7/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/tests/database-sonarqube.yaml` & `devopipe-0.1.7/devopipe/src/templates/tests/database-sonarqube.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.6/devopipe/src/templates/tests/deployment-sonarqube.yaml` & `devopipe-0.1.7/devopipe/src/templates/tests/deployment-sonarqube.yaml`

 * *Files identical despite different names*

