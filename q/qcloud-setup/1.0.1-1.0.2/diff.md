# Comparing `tmp/qcloud_setup-1.0.1.tar.gz` & `tmp/qcloud_setup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.1.tar", last modified: Fri Jun 30 01:18:13 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.2.tar", last modified: Wed Jul 12 11:16:17 2023, max compression
```

## Comparing `qcloud_setup-1.0.1.tar` & `qcloud_setup-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.629621 qcloud_setup-1.0.1/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.1/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    15417 2023-06-30 01:18:13.629401 qcloud_setup-1.0.1/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    14390 2023-06-30 01:18:08.000000 qcloud_setup-1.0.1/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-06-30 01:17:39.000000 qcloud_setup-1.0.1/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.628588 qcloud_setup-1.0.1/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    15417 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-30 01:18:13.629661 qcloud_setup-1.0.1/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      913 2023-06-30 01:17:50.000000 qcloud_setup-1.0.1/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.627412 qcloud_setup-1.0.1/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.629195 qcloud_setup-1.0.1/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.1/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6125 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    53484 2023-06-29 02:23:13.000000 qcloud_setup-1.0.1/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.199137 qcloud_setup-1.0.2/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.2/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)    15720 2023-07-12 11:16:17.198858 qcloud_setup-1.0.2/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    14693 2023-07-12 11:14:59.000000 qcloud_setup-1.0.2/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-12 11:15:50.000000 qcloud_setup-1.0.2/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.196915 qcloud_setup-1.0.2/qcloud_setup.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)    15720 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-12 11:16:17.199181 qcloud_setup-1.0.2/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-12 11:15:35.000000 qcloud_setup-1.0.2/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.195692 qcloud_setup-1.0.2/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.198281 qcloud_setup-1.0.2/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.2/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6125 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    53484 2023-06-29 02:23:13.000000 qcloud_setup-1.0.2/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.1/LICENSE.txt` & `qcloud_setup-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.1/PKG-INFO` & `qcloud_setup-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_setup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -29,68 +29,116 @@
 
 -----------------------------------------------------------------------
 
 
 ## Introduction
 
 Q-Cloud is a framework that allows users to easily launch elastic compute
-clusters on AWS and run Q-Chem calculations on them.  
+clusters on AWS and submit Q-Chem calculations to them.  The clusters will
+automatically expand with demand, up to the maximum size determined by
+the type of Q-Cloud license purchased, and idle nodes will shut down to 
+minimize running costs.
 
 Q-Cloud clusters are built around three separate AWS service stacks with the
 following names and purposes:
-1. _qcloud-users_: This stack is optional and controls access to the cluster.  It
+1. _qcloud-users_: This stack controls user access to the cluster.  It
    launches a Cognito service which manages users, passwords and access tokens.
 2. _qcloud-api-gateway_: This stack provides the REST endpoints for submitting jobs to
    the cluster and for accessing the results from calculations.  
 3. _qcloud-cluster_: This is the actual compute cluster and consists of a head node
    (which can be just a t2.micro instance) running a SLURM workload manager.
    The head node is responsible for launching the compute instances which run
    the Q-Chem calculations.  The head node runs for the lifetime of the
    cluster, but the compute nodes run on-demand and automatically terminate
    when there are no jobs in the queue.
 
-The cluster administrator will need to have a valid AWS account in order to
-launch a cluster, however, users of the cluster can be configured separately
-and do not require an AWS account. See the Adding users section below for
-further details on setting up users.
-
 **Note:** Charges apply to many AWS services.  See the Costs section for
 further details and information on how to minimise the running costs of the
 cluster.
 
 
-## AWS User and Credentials
+## Prerequisites
+
+The cluster administrator will need to have a valid AWS account and be able to
+log into their account via the [console](https://signin.aws.amazon.com/).
+However, users of the cluster do not require AWS accounts as their access to the
+cluster is configured separately, (see the Adding users section below for
+further details on setting up user accounts).
+
+The Q-Cloud infrastructure requires you to have python (v3.7 or later)
+installed.  You can install the package, along with its dependencies, using the
+following:
+```
+python3 -m pip install qcloud_setup
+```
+Ensure pcluster is on your path by typing the following:
+```
+which pcluster
+```
+If it is not, you will need to find the pcluster script within your python
+environment and add its location to your path.
+
+Additionally, Node.js is required and can be installed via:
+```
+curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
+. ~/.nvm/nvm.sh
+nvm install --lts
+```
+
+The following steps are required to set up a Q-Cloud cluster.
+
+
+## 1) Create Q-Cloud administrator account
 
 It is recommended that you create a separate qcloud user to manage the cluster:
 
 1. Open your web browser and log into the [AWS console](https://signin.aws.amazon.com/).  
 2. Ensure you are in the correct region (this is displayed in the the top right
    of the console).
 3. In the search box type IAM and select the first hit.
 4. Select 'Users' in the left hand panel under Access Management and click the
    'Add users' button.
 5. Enter the name of the Q-Cloud administrator (e.g. qcloud) and click 'Next'.
 6. An IAM policy to manage permissions will be created later, so in the 'Set
    Permissions' panel, just click 'Next'.
 7. Click 'Create user'.
 
-The new user will require an access key for authentication:
+
+## 2) Generate access key
+
+The newly created qcloud account user will require an access key for
+authentication:
 
 1. In the IAM panel click on the qcloud user name in the list of users.
 2. Select the 'Security credentials' tab and scroll down to the 'Access keys'
    section and click the 'Create access key' button.
 3. Select the 'Local code' option in the 'Access key best practices &
    alternatives' panel and click 'Next'.
 4. Enter a description for the key and click 'Create access key'.
 5. Make a note of both the access key and the secret access key.  You will not
    have another opportunity to see the secret key, so if you misplace it you
    will need to deactivate the key and generate a new one.
 
-We will now add IAM permissions to the user via a custom policy.  The policy is 
-most easily created via CloudFormation and the template file can be generated with:
+To install the access key, run the following command and enter both the access key
+and the secret key:
+```
+qcloud_setup  --configure-aws
+```
+You will need to enter a supported AWS region (currently us-east-1) which will
+determine where the cluster resources are located.  Please contact Q-Chem
+support (support@q-chem.com) if you require a different region.
+
+These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+
+
+## 3) Create IAM policy 
+
+We will now add IAM permissions to the qcloud user via a custom policy.  The
+policy is most easily created via a CloudFormation template that can be
+generated with:
 ```
 qcloud_setup --gen-policy
 ```
 This will create the file iam-policy.yaml in the working directory.
 
 1. In the AWS console, search for CloudFormation and click the first hit. 
    Select 'Stacks' in the left hand panel.
@@ -109,48 +157,16 @@
 2. In the 'Permissions policies' section, click the 'Add permissions' button.
 3. Select the 'Attach policies directly' option at the top and search for
    Q-CloudIamPolicy.  Select the Q-CloudIamPolicy just created and click
    'Next'.
 4. Click 'Add permissions' on the Review page.
 
 
-## Prequisites
-
-The Q-Cloud infrastructure requires you to have python (v3.7 or later)
-installed.  You can install the package, along with its dependencies, using the
-following:
-```
-python3 -m pip install qcloud_setup
-```
-Ensure plcuster is on your path by typing the following:
-```
-which pcluster
-```
-If it is not, you will need to find the pcluster script within your python
-environment and add its location to your path.
 
-Additionally, Node.js is required and can be installed via:
-```
-curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
-. ~/.nvm/nvm.sh
-nvm install --lts
-```
-
-In order that qcloud\_setup can access AWS resources, you will neeed to add the 
-previously created access keys.  Navigate to the directory containing the Q-Cloud 
-download and type the following:
-```
-qcloud_setup  --configure-aws
-```
-
-Enter the AWS region, access key and secret key that you noted down earlier.  The 
-region entered(e.g. us-east-1) will determine the location of the resources.
-
-
-## Cluster Configuration
+## 4) Configure cluster
 Cluster configuration files are generated with the command: 
 ```
 qcloud_setup --configure
 ```
 This takes the user through an interactive setup process which produces a
 configuration file with the name *qcloud-cluster.config* which can be viewed
 before launching the cluster.  Do not modify the contents of the configuration
@@ -160,30 +176,31 @@
 the `--name <cluster_name>` option.  This allows for multiple clusters to run
 at the same time, if required.  Note that if a non-default name is specified
 then this name must be passed using the `--name` option to subsequent commands
 (e.g. `--launch`) in order that they operate on the correct cluster.
 
 The options specified in the configuration process are discussed in detail below.
 
-#### 1) AWS Credentials
+
+#### 4.1) AWS Credentials
 
 These should have been configured previously and, if so, are automatically
-detected.  Make sure you are using a profile with the Q-CloudIamPolicies
-attached, such as the  qlcoud user created above.  If you have more than one
+detected.  Make sure you are using a profile with the Q-CloudIamPolicy
+attached, such as the  qcloud user created above.  If you have more than one
 profile, you can select between them using the `--profile <profile_name>`
 option.  The selected profile will determine the region in which the cluster is
 launched.  
 
 A new SSH key pair will be created and the private key will be saved in the
 qcloud\_\<region\>\_keypair.pem file.  You can copy this key file to the location
 of your other key files (e.g. the ~/.ssh directory), if desired.  Do not lose
 this private key as you will be unable to connect to the head node without it.
 
 
-#### 2) VPC setup
+#### 4.2) VPC setup
 
 The Q-Cloud cluster runs inside a Virtual Private Cloud (VPC) and it is
 recommended that a new VPC be created for running the Q-Cloud cluster.
 However, because there is a limit on the number of VPCs per AWS account, this may
 not be possible for some users. Please select whichever of the following 
 options is best for your case:
 
@@ -192,55 +209,55 @@
 - Use existing: If available.  The setup script will look for a previously
   configured Q-Cloud VPC.  This will have both public (for the head node) 
   and private (compute nodes) subnets configured.
 - Create new: This will create a new VPC with public and private subnets.  
   The availability zone of the subnets does not matter.
 
 
-#### 3) Compute instance types
+#### 4.3) Compute instance types
 
 The costs shown are indicative only and are for running each instance. They
 do not include storage or network costs.
 
-#### 4) Maximum compute nodes
+#### 4.4) Maximum compute nodes
 This determines the maximum number of compute instances that can run concurrently. 
 If more jobs are submitted than this value, they will be queued until the resources
 become available.
 
 This value should be set to the same number as the number of seats purchased as
 part of your license.
 
 
-#### 5) Job files
+#### 4.5) Job files
 This is the space allocated for the jobs volume which is attached to the head
 node and shared between compute instances.  This volume is used for output
 files only and can be quite small.  Output files are automatically deleted
 after they have been copied to the S3 bucket.
 
-#### 6) Scratch files
+#### 4.6) Scratch files
 
 This determines the scratch volume size per instance. As an indicative cost,
 100Gb costs around $10/month.
 
 
-## Launching a cluster
+## 5) Launching the cluster
+
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
-Cognito is used to manage user access to the REST API. 
 
-The launch option updates the configuration file with the placeholder values.
+The launch option updates the configuration file with values for the placeholders.
 
 **Note:** Progress of the stack launch is printed to the terminal and will take
 several minutes.
 
-Once launched, you will need to send the following information to Q-Chem to obtain 
-your license activation key:
+Once launched, you will need to send the following information to
+license@q-chem.com to obtain your license activation key:
 
 - Elastic IP address 
 - Order number
 - Name 
 - University / Institution
 
 Once you have your activation key you can install it as follows:
@@ -270,51 +287,51 @@
 ...
 ```
 
 A message will be sent to the user's email address with their user name and a
 temporary password, which will need to be changed when first attempting to
 submit a job.
 
-Note that the number of users able to be added each day is set to 50 due to
+Note that the number of users able to be added each day is limited to 50 due to
 email limits in the Cognito service.  If you need to add more than this you
-will need to configure Cognito with the Simple Email Service' (SES) and add 
-a validated administrator email.
+will need to configure Cognito with the Simple Email Service' (SES) and add a
+validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
 CognitoUserPoolId                us-east-1_KbkatQIpW
 CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
 ApiGatewayId                     fkkfolduo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
-python3 -m pip install --trusted-host 44.211.208.71 --index-url http://44.211.208.71:8080 qcloud_user
+python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
 ```
 qcloud --configure
 ```
 The first time a user interacts with the cluster they will need to enter the temporary
 password emailed to them before resetting their password.
 
-See the README.md file distributed with the qcloud_user module for further
+See the README.md file distributed with the qcloud\_user module for further
 details on interacting with the server.
 
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration and license files.
+cluster, make sure you keep a copy of the configuration file and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
@@ -325,18 +342,17 @@
 archived in an S3 bucket.  You will, of course, be unable to submit further
 jobs until the cluster has been restarted.
 
 To re-launch the cluster, issue the following command in the same directory as
 the configuration and license files:
 
 ```
-qcloud_setup  --launch --install-license <license_file>
+qcloud_setup  --launch 
+qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
-The `--install-license` option automatically updates the license file with the private IP
-of the new host.
 
 **Note:** In order to restart a cluster, you must have configured the cluster to
 use an elastic IP (EIP) address allocated to your AWS account. This EIP must be
 available for reuse when re-launching the cluster, otherwise the Q-Chem license
 will no longer be valid.
 
 If you need to update the EIP of your host, please contact our support team at 
@@ -364,15 +380,14 @@
 ```
 qcloud_setup  --help
 qcloud_setup  --info
 qcloud_setup  --list
 ```
 
 You can also open an ssh connection to the head node using the following:
-
 ```
 qcloud_setup  --shell
 ```
 
 
 ## Troubleshooting
```

### Comparing `qcloud_setup-1.0.1/README.md` & `qcloud_setup-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,68 +4,116 @@
 
 -----------------------------------------------------------------------
 
 
 ## Introduction
 
 Q-Cloud is a framework that allows users to easily launch elastic compute
-clusters on AWS and run Q-Chem calculations on them.  
+clusters on AWS and submit Q-Chem calculations to them.  The clusters will
+automatically expand with demand, up to the maximum size determined by
+the type of Q-Cloud license purchased, and idle nodes will shut down to 
+minimize running costs.
 
 Q-Cloud clusters are built around three separate AWS service stacks with the
 following names and purposes:
-1. _qcloud-users_: This stack is optional and controls access to the cluster.  It
+1. _qcloud-users_: This stack controls user access to the cluster.  It
    launches a Cognito service which manages users, passwords and access tokens.
 2. _qcloud-api-gateway_: This stack provides the REST endpoints for submitting jobs to
    the cluster and for accessing the results from calculations.  
 3. _qcloud-cluster_: This is the actual compute cluster and consists of a head node
    (which can be just a t2.micro instance) running a SLURM workload manager.
    The head node is responsible for launching the compute instances which run
    the Q-Chem calculations.  The head node runs for the lifetime of the
    cluster, but the compute nodes run on-demand and automatically terminate
    when there are no jobs in the queue.
 
-The cluster administrator will need to have a valid AWS account in order to
-launch a cluster, however, users of the cluster can be configured separately
-and do not require an AWS account. See the Adding users section below for
-further details on setting up users.
-
 **Note:** Charges apply to many AWS services.  See the Costs section for
 further details and information on how to minimise the running costs of the
 cluster.
 
 
-## AWS User and Credentials
+## Prerequisites
+
+The cluster administrator will need to have a valid AWS account and be able to
+log into their account via the [console](https://signin.aws.amazon.com/).
+However, users of the cluster do not require AWS accounts as their access to the
+cluster is configured separately, (see the Adding users section below for
+further details on setting up user accounts).
+
+The Q-Cloud infrastructure requires you to have python (v3.7 or later)
+installed.  You can install the package, along with its dependencies, using the
+following:
+```
+python3 -m pip install qcloud_setup
+```
+Ensure pcluster is on your path by typing the following:
+```
+which pcluster
+```
+If it is not, you will need to find the pcluster script within your python
+environment and add its location to your path.
+
+Additionally, Node.js is required and can be installed via:
+```
+curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
+. ~/.nvm/nvm.sh
+nvm install --lts
+```
+
+The following steps are required to set up a Q-Cloud cluster.
+
+
+## 1) Create Q-Cloud administrator account
 
 It is recommended that you create a separate qcloud user to manage the cluster:
 
 1. Open your web browser and log into the [AWS console](https://signin.aws.amazon.com/).  
 2. Ensure you are in the correct region (this is displayed in the the top right
    of the console).
 3. In the search box type IAM and select the first hit.
 4. Select 'Users' in the left hand panel under Access Management and click the
    'Add users' button.
 5. Enter the name of the Q-Cloud administrator (e.g. qcloud) and click 'Next'.
 6. An IAM policy to manage permissions will be created later, so in the 'Set
    Permissions' panel, just click 'Next'.
 7. Click 'Create user'.
 
-The new user will require an access key for authentication:
+
+## 2) Generate access key
+
+The newly created qcloud account user will require an access key for
+authentication:
 
 1. In the IAM panel click on the qcloud user name in the list of users.
 2. Select the 'Security credentials' tab and scroll down to the 'Access keys'
    section and click the 'Create access key' button.
 3. Select the 'Local code' option in the 'Access key best practices &
    alternatives' panel and click 'Next'.
 4. Enter a description for the key and click 'Create access key'.
 5. Make a note of both the access key and the secret access key.  You will not
    have another opportunity to see the secret key, so if you misplace it you
    will need to deactivate the key and generate a new one.
 
-We will now add IAM permissions to the user via a custom policy.  The policy is 
-most easily created via CloudFormation and the template file can be generated with:
+To install the access key, run the following command and enter both the access key
+and the secret key:
+```
+qcloud_setup  --configure-aws
+```
+You will need to enter a supported AWS region (currently us-east-1) which will
+determine where the cluster resources are located.  Please contact Q-Chem
+support (support@q-chem.com) if you require a different region.
+
+These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+
+
+## 3) Create IAM policy 
+
+We will now add IAM permissions to the qcloud user via a custom policy.  The
+policy is most easily created via a CloudFormation template that can be
+generated with:
 ```
 qcloud_setup --gen-policy
 ```
 This will create the file iam-policy.yaml in the working directory.
 
 1. In the AWS console, search for CloudFormation and click the first hit. 
    Select 'Stacks' in the left hand panel.
@@ -84,48 +132,16 @@
 2. In the 'Permissions policies' section, click the 'Add permissions' button.
 3. Select the 'Attach policies directly' option at the top and search for
    Q-CloudIamPolicy.  Select the Q-CloudIamPolicy just created and click
    'Next'.
 4. Click 'Add permissions' on the Review page.
 
 
-## Prequisites
-
-The Q-Cloud infrastructure requires you to have python (v3.7 or later)
-installed.  You can install the package, along with its dependencies, using the
-following:
-```
-python3 -m pip install qcloud_setup
-```
-Ensure plcuster is on your path by typing the following:
-```
-which pcluster
-```
-If it is not, you will need to find the pcluster script within your python
-environment and add its location to your path.
 
-Additionally, Node.js is required and can be installed via:
-```
-curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
-. ~/.nvm/nvm.sh
-nvm install --lts
-```
-
-In order that qcloud\_setup can access AWS resources, you will neeed to add the 
-previously created access keys.  Navigate to the directory containing the Q-Cloud 
-download and type the following:
-```
-qcloud_setup  --configure-aws
-```
-
-Enter the AWS region, access key and secret key that you noted down earlier.  The 
-region entered(e.g. us-east-1) will determine the location of the resources.
-
-
-## Cluster Configuration
+## 4) Configure cluster
 Cluster configuration files are generated with the command: 
 ```
 qcloud_setup --configure
 ```
 This takes the user through an interactive setup process which produces a
 configuration file with the name *qcloud-cluster.config* which can be viewed
 before launching the cluster.  Do not modify the contents of the configuration
@@ -135,30 +151,31 @@
 the `--name <cluster_name>` option.  This allows for multiple clusters to run
 at the same time, if required.  Note that if a non-default name is specified
 then this name must be passed using the `--name` option to subsequent commands
 (e.g. `--launch`) in order that they operate on the correct cluster.
 
 The options specified in the configuration process are discussed in detail below.
 
-#### 1) AWS Credentials
+
+#### 4.1) AWS Credentials
 
 These should have been configured previously and, if so, are automatically
-detected.  Make sure you are using a profile with the Q-CloudIamPolicies
-attached, such as the  qlcoud user created above.  If you have more than one
+detected.  Make sure you are using a profile with the Q-CloudIamPolicy
+attached, such as the  qcloud user created above.  If you have more than one
 profile, you can select between them using the `--profile <profile_name>`
 option.  The selected profile will determine the region in which the cluster is
 launched.  
 
 A new SSH key pair will be created and the private key will be saved in the
 qcloud\_\<region\>\_keypair.pem file.  You can copy this key file to the location
 of your other key files (e.g. the ~/.ssh directory), if desired.  Do not lose
 this private key as you will be unable to connect to the head node without it.
 
 
-#### 2) VPC setup
+#### 4.2) VPC setup
 
 The Q-Cloud cluster runs inside a Virtual Private Cloud (VPC) and it is
 recommended that a new VPC be created for running the Q-Cloud cluster.
 However, because there is a limit on the number of VPCs per AWS account, this may
 not be possible for some users. Please select whichever of the following 
 options is best for your case:
 
@@ -167,55 +184,55 @@
 - Use existing: If available.  The setup script will look for a previously
   configured Q-Cloud VPC.  This will have both public (for the head node) 
   and private (compute nodes) subnets configured.
 - Create new: This will create a new VPC with public and private subnets.  
   The availability zone of the subnets does not matter.
 
 
-#### 3) Compute instance types
+#### 4.3) Compute instance types
 
 The costs shown are indicative only and are for running each instance. They
 do not include storage or network costs.
 
-#### 4) Maximum compute nodes
+#### 4.4) Maximum compute nodes
 This determines the maximum number of compute instances that can run concurrently. 
 If more jobs are submitted than this value, they will be queued until the resources
 become available.
 
 This value should be set to the same number as the number of seats purchased as
 part of your license.
 
 
-#### 5) Job files
+#### 4.5) Job files
 This is the space allocated for the jobs volume which is attached to the head
 node and shared between compute instances.  This volume is used for output
 files only and can be quite small.  Output files are automatically deleted
 after they have been copied to the S3 bucket.
 
-#### 6) Scratch files
+#### 4.6) Scratch files
 
 This determines the scratch volume size per instance. As an indicative cost,
 100Gb costs around $10/month.
 
 
-## Launching a cluster
+## 5) Launching the cluster
+
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
-Cognito is used to manage user access to the REST API. 
 
-The launch option updates the configuration file with the placeholder values.
+The launch option updates the configuration file with values for the placeholders.
 
 **Note:** Progress of the stack launch is printed to the terminal and will take
 several minutes.
 
-Once launched, you will need to send the following information to Q-Chem to obtain 
-your license activation key:
+Once launched, you will need to send the following information to
+license@q-chem.com to obtain your license activation key:
 
 - Elastic IP address 
 - Order number
 - Name 
 - University / Institution
 
 Once you have your activation key you can install it as follows:
@@ -245,51 +262,51 @@
 ...
 ```
 
 A message will be sent to the user's email address with their user name and a
 temporary password, which will need to be changed when first attempting to
 submit a job.
 
-Note that the number of users able to be added each day is set to 50 due to
+Note that the number of users able to be added each day is limited to 50 due to
 email limits in the Cognito service.  If you need to add more than this you
-will need to configure Cognito with the Simple Email Service' (SES) and add 
-a validated administrator email.
+will need to configure Cognito with the Simple Email Service' (SES) and add a
+validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
 CognitoUserPoolId                us-east-1_KbkatQIpW
 CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
 ApiGatewayId                     fkkfolduo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
-python3 -m pip install --trusted-host 44.211.208.71 --index-url http://44.211.208.71:8080 qcloud_user
+python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
 ```
 qcloud --configure
 ```
 The first time a user interacts with the cluster they will need to enter the temporary
 password emailed to them before resetting their password.
 
-See the README.md file distributed with the qcloud_user module for further
+See the README.md file distributed with the qcloud\_user module for further
 details on interacting with the server.
 
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration and license files.
+cluster, make sure you keep a copy of the configuration file and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
@@ -300,18 +317,17 @@
 archived in an S3 bucket.  You will, of course, be unable to submit further
 jobs until the cluster has been restarted.
 
 To re-launch the cluster, issue the following command in the same directory as
 the configuration and license files:
 
 ```
-qcloud_setup  --launch --install-license <license_file>
+qcloud_setup  --launch 
+qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
-The `--install-license` option automatically updates the license file with the private IP
-of the new host.
 
 **Note:** In order to restart a cluster, you must have configured the cluster to
 use an elastic IP (EIP) address allocated to your AWS account. This EIP must be
 available for reuse when re-launching the cluster, otherwise the Q-Chem license
 will no longer be valid.
 
 If you need to update the EIP of your host, please contact our support team at 
@@ -339,15 +355,14 @@
 ```
 qcloud_setup  --help
 qcloud_setup  --info
 qcloud_setup  --list
 ```
 
 You can also open an ssh connection to the head node using the following:
-
 ```
 qcloud_setup  --shell
 ```
 
 
 ## Troubleshooting
```

### Comparing `qcloud_setup-1.0.1/pyproject.toml` & `qcloud_setup-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.1"
+version = "1.0.2"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_setup-1.0.1/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.2/qcloud_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-setup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -29,68 +29,116 @@
 
 -----------------------------------------------------------------------
 
 
 ## Introduction
 
 Q-Cloud is a framework that allows users to easily launch elastic compute
-clusters on AWS and run Q-Chem calculations on them.  
+clusters on AWS and submit Q-Chem calculations to them.  The clusters will
+automatically expand with demand, up to the maximum size determined by
+the type of Q-Cloud license purchased, and idle nodes will shut down to 
+minimize running costs.
 
 Q-Cloud clusters are built around three separate AWS service stacks with the
 following names and purposes:
-1. _qcloud-users_: This stack is optional and controls access to the cluster.  It
+1. _qcloud-users_: This stack controls user access to the cluster.  It
    launches a Cognito service which manages users, passwords and access tokens.
 2. _qcloud-api-gateway_: This stack provides the REST endpoints for submitting jobs to
    the cluster and for accessing the results from calculations.  
 3. _qcloud-cluster_: This is the actual compute cluster and consists of a head node
    (which can be just a t2.micro instance) running a SLURM workload manager.
    The head node is responsible for launching the compute instances which run
    the Q-Chem calculations.  The head node runs for the lifetime of the
    cluster, but the compute nodes run on-demand and automatically terminate
    when there are no jobs in the queue.
 
-The cluster administrator will need to have a valid AWS account in order to
-launch a cluster, however, users of the cluster can be configured separately
-and do not require an AWS account. See the Adding users section below for
-further details on setting up users.
-
 **Note:** Charges apply to many AWS services.  See the Costs section for
 further details and information on how to minimise the running costs of the
 cluster.
 
 
-## AWS User and Credentials
+## Prerequisites
+
+The cluster administrator will need to have a valid AWS account and be able to
+log into their account via the [console](https://signin.aws.amazon.com/).
+However, users of the cluster do not require AWS accounts as their access to the
+cluster is configured separately, (see the Adding users section below for
+further details on setting up user accounts).
+
+The Q-Cloud infrastructure requires you to have python (v3.7 or later)
+installed.  You can install the package, along with its dependencies, using the
+following:
+```
+python3 -m pip install qcloud_setup
+```
+Ensure pcluster is on your path by typing the following:
+```
+which pcluster
+```
+If it is not, you will need to find the pcluster script within your python
+environment and add its location to your path.
+
+Additionally, Node.js is required and can be installed via:
+```
+curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
+. ~/.nvm/nvm.sh
+nvm install --lts
+```
+
+The following steps are required to set up a Q-Cloud cluster.
+
+
+## 1) Create Q-Cloud administrator account
 
 It is recommended that you create a separate qcloud user to manage the cluster:
 
 1. Open your web browser and log into the [AWS console](https://signin.aws.amazon.com/).  
 2. Ensure you are in the correct region (this is displayed in the the top right
    of the console).
 3. In the search box type IAM and select the first hit.
 4. Select 'Users' in the left hand panel under Access Management and click the
    'Add users' button.
 5. Enter the name of the Q-Cloud administrator (e.g. qcloud) and click 'Next'.
 6. An IAM policy to manage permissions will be created later, so in the 'Set
    Permissions' panel, just click 'Next'.
 7. Click 'Create user'.
 
-The new user will require an access key for authentication:
+
+## 2) Generate access key
+
+The newly created qcloud account user will require an access key for
+authentication:
 
 1. In the IAM panel click on the qcloud user name in the list of users.
 2. Select the 'Security credentials' tab and scroll down to the 'Access keys'
    section and click the 'Create access key' button.
 3. Select the 'Local code' option in the 'Access key best practices &
    alternatives' panel and click 'Next'.
 4. Enter a description for the key and click 'Create access key'.
 5. Make a note of both the access key and the secret access key.  You will not
    have another opportunity to see the secret key, so if you misplace it you
    will need to deactivate the key and generate a new one.
 
-We will now add IAM permissions to the user via a custom policy.  The policy is 
-most easily created via CloudFormation and the template file can be generated with:
+To install the access key, run the following command and enter both the access key
+and the secret key:
+```
+qcloud_setup  --configure-aws
+```
+You will need to enter a supported AWS region (currently us-east-1) which will
+determine where the cluster resources are located.  Please contact Q-Chem
+support (support@q-chem.com) if you require a different region.
+
+These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+
+
+## 3) Create IAM policy 
+
+We will now add IAM permissions to the qcloud user via a custom policy.  The
+policy is most easily created via a CloudFormation template that can be
+generated with:
 ```
 qcloud_setup --gen-policy
 ```
 This will create the file iam-policy.yaml in the working directory.
 
 1. In the AWS console, search for CloudFormation and click the first hit. 
    Select 'Stacks' in the left hand panel.
@@ -109,48 +157,16 @@
 2. In the 'Permissions policies' section, click the 'Add permissions' button.
 3. Select the 'Attach policies directly' option at the top and search for
    Q-CloudIamPolicy.  Select the Q-CloudIamPolicy just created and click
    'Next'.
 4. Click 'Add permissions' on the Review page.
 
 
-## Prequisites
-
-The Q-Cloud infrastructure requires you to have python (v3.7 or later)
-installed.  You can install the package, along with its dependencies, using the
-following:
-```
-python3 -m pip install qcloud_setup
-```
-Ensure plcuster is on your path by typing the following:
-```
-which pcluster
-```
-If it is not, you will need to find the pcluster script within your python
-environment and add its location to your path.
 
-Additionally, Node.js is required and can be installed via:
-```
-curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
-. ~/.nvm/nvm.sh
-nvm install --lts
-```
-
-In order that qcloud\_setup can access AWS resources, you will neeed to add the 
-previously created access keys.  Navigate to the directory containing the Q-Cloud 
-download and type the following:
-```
-qcloud_setup  --configure-aws
-```
-
-Enter the AWS region, access key and secret key that you noted down earlier.  The 
-region entered(e.g. us-east-1) will determine the location of the resources.
-
-
-## Cluster Configuration
+## 4) Configure cluster
 Cluster configuration files are generated with the command: 
 ```
 qcloud_setup --configure
 ```
 This takes the user through an interactive setup process which produces a
 configuration file with the name *qcloud-cluster.config* which can be viewed
 before launching the cluster.  Do not modify the contents of the configuration
@@ -160,30 +176,31 @@
 the `--name <cluster_name>` option.  This allows for multiple clusters to run
 at the same time, if required.  Note that if a non-default name is specified
 then this name must be passed using the `--name` option to subsequent commands
 (e.g. `--launch`) in order that they operate on the correct cluster.
 
 The options specified in the configuration process are discussed in detail below.
 
-#### 1) AWS Credentials
+
+#### 4.1) AWS Credentials
 
 These should have been configured previously and, if so, are automatically
-detected.  Make sure you are using a profile with the Q-CloudIamPolicies
-attached, such as the  qlcoud user created above.  If you have more than one
+detected.  Make sure you are using a profile with the Q-CloudIamPolicy
+attached, such as the  qcloud user created above.  If you have more than one
 profile, you can select between them using the `--profile <profile_name>`
 option.  The selected profile will determine the region in which the cluster is
 launched.  
 
 A new SSH key pair will be created and the private key will be saved in the
 qcloud\_\<region\>\_keypair.pem file.  You can copy this key file to the location
 of your other key files (e.g. the ~/.ssh directory), if desired.  Do not lose
 this private key as you will be unable to connect to the head node without it.
 
 
-#### 2) VPC setup
+#### 4.2) VPC setup
 
 The Q-Cloud cluster runs inside a Virtual Private Cloud (VPC) and it is
 recommended that a new VPC be created for running the Q-Cloud cluster.
 However, because there is a limit on the number of VPCs per AWS account, this may
 not be possible for some users. Please select whichever of the following 
 options is best for your case:
 
@@ -192,55 +209,55 @@
 - Use existing: If available.  The setup script will look for a previously
   configured Q-Cloud VPC.  This will have both public (for the head node) 
   and private (compute nodes) subnets configured.
 - Create new: This will create a new VPC with public and private subnets.  
   The availability zone of the subnets does not matter.
 
 
-#### 3) Compute instance types
+#### 4.3) Compute instance types
 
 The costs shown are indicative only and are for running each instance. They
 do not include storage or network costs.
 
-#### 4) Maximum compute nodes
+#### 4.4) Maximum compute nodes
 This determines the maximum number of compute instances that can run concurrently. 
 If more jobs are submitted than this value, they will be queued until the resources
 become available.
 
 This value should be set to the same number as the number of seats purchased as
 part of your license.
 
 
-#### 5) Job files
+#### 4.5) Job files
 This is the space allocated for the jobs volume which is attached to the head
 node and shared between compute instances.  This volume is used for output
 files only and can be quite small.  Output files are automatically deleted
 after they have been copied to the S3 bucket.
 
-#### 6) Scratch files
+#### 4.6) Scratch files
 
 This determines the scratch volume size per instance. As an indicative cost,
 100Gb costs around $10/month.
 
 
-## Launching a cluster
+## 5) Launching the cluster
+
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
-Cognito is used to manage user access to the REST API. 
 
-The launch option updates the configuration file with the placeholder values.
+The launch option updates the configuration file with values for the placeholders.
 
 **Note:** Progress of the stack launch is printed to the terminal and will take
 several minutes.
 
-Once launched, you will need to send the following information to Q-Chem to obtain 
-your license activation key:
+Once launched, you will need to send the following information to
+license@q-chem.com to obtain your license activation key:
 
 - Elastic IP address 
 - Order number
 - Name 
 - University / Institution
 
 Once you have your activation key you can install it as follows:
@@ -270,51 +287,51 @@
 ...
 ```
 
 A message will be sent to the user's email address with their user name and a
 temporary password, which will need to be changed when first attempting to
 submit a job.
 
-Note that the number of users able to be added each day is set to 50 due to
+Note that the number of users able to be added each day is limited to 50 due to
 email limits in the Cognito service.  If you need to add more than this you
-will need to configure Cognito with the Simple Email Service' (SES) and add 
-a validated administrator email.
+will need to configure Cognito with the Simple Email Service' (SES) and add a
+validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
 CognitoUserPoolId                us-east-1_KbkatQIpW
 CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
 ApiGatewayId                     fkkfolduo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
-python3 -m pip install --trusted-host 44.211.208.71 --index-url http://44.211.208.71:8080 qcloud_user
+python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
 ```
 qcloud --configure
 ```
 The first time a user interacts with the cluster they will need to enter the temporary
 password emailed to them before resetting their password.
 
-See the README.md file distributed with the qcloud_user module for further
+See the README.md file distributed with the qcloud\_user module for further
 details on interacting with the server.
 
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration and license files.
+cluster, make sure you keep a copy of the configuration file and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
@@ -325,18 +342,17 @@
 archived in an S3 bucket.  You will, of course, be unable to submit further
 jobs until the cluster has been restarted.
 
 To re-launch the cluster, issue the following command in the same directory as
 the configuration and license files:
 
 ```
-qcloud_setup  --launch --install-license <license_file>
+qcloud_setup  --launch 
+qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
-The `--install-license` option automatically updates the license file with the private IP
-of the new host.
 
 **Note:** In order to restart a cluster, you must have configured the cluster to
 use an elastic IP (EIP) address allocated to your AWS account. This EIP must be
 available for reuse when re-launching the cluster, otherwise the Q-Chem license
 will no longer be valid.
 
 If you need to update the EIP of your host, please contact our support team at 
@@ -364,15 +380,14 @@
 ```
 qcloud_setup  --help
 qcloud_setup  --info
 qcloud_setup  --list
 ```
 
 You can also open an ssh connection to the head node using the following:
-
 ```
 qcloud_setup  --shell
 ```
 
 
 ## Troubleshooting
```

### Comparing `qcloud_setup-1.0.1/setup.py` & `qcloud_setup-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.1",
+    version="1.0.2",
     url="https://q-chem.com",
     author="Andrew Gilbert",
-    author_email="suppor@q-chem.com",
+    author_email="support@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"), 
     package_dir={'qcloud_setup': 'src/qcloud_setup'},
     package_data={'qcloud_setup': ['*.yaml']},
     include_package_data=True,
```

### Comparing `qcloud_setup-1.0.1/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.2/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.1/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.2/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.1/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.2/src/qcloud_setup/iam-policy.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.1/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.2/src/qcloud_setup/qcloud_admin.py`

 * *Files identical despite different names*

