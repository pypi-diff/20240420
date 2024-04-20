# Comparing `tmp/genericsuite-0.1.3.tar.gz` & `tmp/genericsuite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericsuite-0.1.3.tar", max compression
+gzip compressed data, was "genericsuite-0.1.4.tar", max compression
```

## Comparing `genericsuite-0.1.3.tar` & `genericsuite-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,59 @@
--rw-r--r--   0        0        0      747 2024-03-31 23:36:29.408323 genericsuite-0.1.3/LICENSE
--rw-r--r--   0        0        0    12258 2024-04-09 13:09:49.814521 genericsuite-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-03 23:49:07.732831 genericsuite-0.1.3/genericsuite/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:14.702977 genericsuite-0.1.3/genericsuite/chalicelib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 11:10:05.850616 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/__init__.py
--rw-r--r--   0        0        0     1096 2024-02-24 02:22:20.582188 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/menu_options.py
--rw-r--r--   0        0        0     2125 2024-02-24 02:14:13.742858 genericsuite-0.1.3/genericsuite/chalicelib/endpoints/users.py
--rw-r--r--   0        0        0     1482 2024-02-24 13:33:20.978316 genericsuite-0.1.3/genericsuite/chalicelib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:25.905045 genericsuite-0.1.3/genericsuite/chalicelib/util/__init__.py
--rw-r--r--   0        0        0     2751 2024-02-26 13:41:07.446923 genericsuite-0.1.3/genericsuite/chalicelib/util/create_app.py
--rw-r--r--   0        0        0     4647 2024-02-25 17:57:02.422438 genericsuite-0.1.3/genericsuite/chalicelib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.378538 genericsuite-0.1.3/genericsuite/config/__init__.py
--rw-r--r--   0        0        0     4304 2024-04-09 13:08:35.964005 genericsuite-0.1.3/genericsuite/config/config.py
--rw-r--r--   0        0        0     4646 2024-04-09 13:08:13.620684 genericsuite-0.1.3/genericsuite/config/config_from_db.py
--rw-r--r--   0        0        0      609 2024-02-18 20:15:35.895205 genericsuite-0.1.3/genericsuite/config/logging.conf.yml
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.895273 genericsuite-0.1.3/genericsuite/constants/__init__.py
--rw-r--r--   0        0        0     1443 2024-02-23 00:45:12.985504 genericsuite-0.1.3/genericsuite/constants/const_tables.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:32.204369 genericsuite-0.1.3/genericsuite/fastapilib/__init__.py
--rw-r--r--   0        0        0     1455 2024-02-24 13:33:13.552960 genericsuite-0.1.3/genericsuite/fastapilib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:35.347602 genericsuite-0.1.3/genericsuite/fastapilib/util/__init__.py
--rw-r--r--   0        0        0     1307 2024-02-18 20:15:35.911504 genericsuite-0.1.3/genericsuite/fastapilib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:50.817726 genericsuite-0.1.3/genericsuite/flasklib/__init__.py
--rw-r--r--   0        0        0     1708 2024-02-24 13:34:01.565559 genericsuite-0.1.3/genericsuite/flasklib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:42.207235 genericsuite-0.1.3/genericsuite/flasklib/util/__init__.py
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.903766 genericsuite-0.1.3/genericsuite/models/billing/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 02:47:22.334682 genericsuite-0.1.3/genericsuite/models/billing/billing_utilities.py
--rw-r--r--   0        0        0        0 2023-07-17 02:15:00.638430 genericsuite-0.1.3/genericsuite/models/menu_options/__init__.py
--rw-r--r--   0        0        0     2840 2024-02-24 02:14:13.741348 genericsuite-0.1.3/genericsuite/models/menu_options/menu_options.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.379886 genericsuite-0.1.3/genericsuite/models/users/__init__.py
--rw-r--r--   0        0        0     8650 2024-02-25 16:04:51.338589 genericsuite-0.1.3/genericsuite/models/users/users.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.380476 genericsuite-0.1.3/genericsuite/util/__init__.py
--rw-r--r--   0        0        0     5898 2024-02-29 11:32:04.042270 genericsuite-0.1.3/genericsuite/util/app_context.py
--rw-r--r--   0        0        0     1608 2024-02-23 01:37:50.489847 genericsuite-0.1.3/genericsuite/util/app_logger.py
--rw-r--r--   0        0        0     7160 2024-02-23 00:45:13.028977 genericsuite-0.1.3/genericsuite/util/aws.py
--rw-r--r--   0        0        0     4456 2024-04-09 12:56:04.586894 genericsuite-0.1.3/genericsuite/util/blueprint_one.py
--rw-r--r--   0        0        0     1797 2024-02-23 10:56:31.242663 genericsuite-0.1.3/genericsuite/util/config_dbdef_helpers.py
--rw-r--r--   0        0        0     1387 2024-02-27 16:04:59.642735 genericsuite-0.1.3/genericsuite/util/current_user_data.py
--rw-r--r--   0        0        0     4972 2024-03-02 04:46:29.973118 genericsuite-0.1.3/genericsuite/util/datetime_utilities.py
--rw-r--r--   0        0        0    35651 2024-02-25 15:25:41.529780 genericsuite-0.1.3/genericsuite/util/db_abstractor.py
--rw-r--r--   0        0        0      807 2024-02-21 16:28:35.421102 genericsuite-0.1.3/genericsuite/util/exceptions.py
--rw-r--r--   0        0        0     2287 2024-02-24 13:40:02.416560 genericsuite-0.1.3/genericsuite/util/framework_abs_layer.py
--rw-r--r--   0        0        0    47797 2024-02-25 17:57:22.042814 genericsuite-0.1.3/genericsuite/util/generic_db_helpers.py
--rw-r--r--   0        0        0     5889 2024-02-25 12:47:46.514099 genericsuite-0.1.3/genericsuite/util/generic_db_middleware.py
--rw-r--r--   0        0        0    10325 2024-02-27 16:04:16.316160 genericsuite-0.1.3/genericsuite/util/generic_endpoint_helpers.py
--rw-r--r--   0        0        0     4472 2024-04-09 12:10:28.048429 genericsuite-0.1.3/genericsuite/util/jwt.py
--rw-r--r--   0        0        0     3216 2024-02-23 00:45:13.032873 genericsuite-0.1.3/genericsuite/util/nav_helpers.py
--rw-r--r--   0        0        0     4421 2024-02-23 00:45:13.039348 genericsuite-0.1.3/genericsuite/util/parse_multipart.py
--rw-r--r--   0        0        0     1818 2024-02-23 01:37:50.488701 genericsuite-0.1.3/genericsuite/util/passwords.py
--rw-r--r--   0        0        0      585 2024-02-18 20:15:35.910549 genericsuite-0.1.3/genericsuite/util/request_handler.py
--rw-r--r--   0        0        0     6568 2024-02-23 00:45:13.032854 genericsuite-0.1.3/genericsuite/util/security.py
--rw-r--r--   0        0        0     3318 2024-02-25 11:52:22.059881 genericsuite-0.1.3/genericsuite/util/send_email.py
--rw-r--r--   0        0        0    16009 2024-03-02 15:00:06.343708 genericsuite-0.1.3/genericsuite/util/utilities.py
--rw-r--r--   0        0        0     1429 2024-04-09 13:15:41.911453 genericsuite-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    13455 1970-01-01 00:00:00.000000 genericsuite-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-04-09 22:31:29.440842 genericsuite-0.1.4/LICENSE
+-rw-r--r--   0        0        0    15614 2024-04-19 09:15:53.218346 genericsuite-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.506793 genericsuite-0.1.4/genericsuite/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.514431 genericsuite-0.1.4/genericsuite/chalicelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.507857 genericsuite-0.1.4/genericsuite/chalicelib/endpoints/__init__.py
+-rw-r--r--   0        0        0     1096 2024-04-09 22:31:29.510794 genericsuite-0.1.4/genericsuite/chalicelib/endpoints/menu_options.py
+-rw-r--r--   0        0        0     1781 2024-04-14 21:38:57.975038 genericsuite-0.1.4/genericsuite/chalicelib/endpoints/users.py
+-rw-r--r--   0        0        0     1482 2024-04-09 22:31:29.516266 genericsuite-0.1.4/genericsuite/chalicelib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.511648 genericsuite-0.1.4/genericsuite/chalicelib/util/__init__.py
+-rw-r--r--   0        0        0     2673 2024-04-14 17:30:48.284419 genericsuite-0.1.4/genericsuite/chalicelib/util/create_app.py
+-rw-r--r--   0        0        0     4639 2024-04-14 15:42:48.592048 genericsuite-0.1.4/genericsuite/chalicelib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.500540 genericsuite-0.1.4/genericsuite/config/__init__.py
+-rw-r--r--   0        0        0     4304 2024-04-09 22:31:29.499878 genericsuite-0.1.4/genericsuite/config/config.py
+-rw-r--r--   0        0        0     4646 2024-04-09 22:31:29.504217 genericsuite-0.1.4/genericsuite/config/config_from_db.py
+-rw-r--r--   0        0        0      609 2024-04-09 22:31:29.500443 genericsuite-0.1.4/genericsuite/config/logging.conf.yml
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.504842 genericsuite-0.1.4/genericsuite/constants/__init__.py
+-rw-r--r--   0        0        0     1443 2024-04-09 22:31:29.506699 genericsuite-0.1.4/genericsuite/constants/const_tables.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.532865 genericsuite-0.1.4/genericsuite/fastapilib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 18:54:28.977257 genericsuite-0.1.4/genericsuite/fastapilib/endpoints/__init__.py
+-rw-r--r--   0        0        0     1286 2024-04-20 13:14:10.353515 genericsuite-0.1.4/genericsuite/fastapilib/endpoints/menu_options.py
+-rw-r--r--   0        0        0     2025 2024-04-15 11:24:06.814912 genericsuite-0.1.4/genericsuite/fastapilib/endpoints/users.py
+-rw-r--r--   0        0        0     3563 2024-04-15 18:18:49.548500 genericsuite-0.1.4/genericsuite/fastapilib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.532709 genericsuite-0.1.4/genericsuite/fastapilib/util/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-15 16:37:35.970253 genericsuite-0.1.4/genericsuite/fastapilib/util/create_app.py
+-rw-r--r--   0        0        0     3340 2024-04-15 16:57:41.681759 genericsuite-0.1.4/genericsuite/fastapilib/util/dependencies.py
+-rw-r--r--   0        0        0    10374 2024-04-20 11:32:13.137877 genericsuite-0.1.4/genericsuite/fastapilib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.530151 genericsuite-0.1.4/genericsuite/flasklib/__init__.py
+-rw-r--r--   0        0        0     1708 2024-04-09 22:31:29.531122 genericsuite-0.1.4/genericsuite/flasklib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.529904 genericsuite-0.1.4/genericsuite/flasklib/util/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.519809 genericsuite-0.1.4/genericsuite/models/billing/__init__.py
+-rw-r--r--   0        0        0     1419 2024-04-09 22:31:29.520122 genericsuite-0.1.4/genericsuite/models/billing/billing_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.523313 genericsuite-0.1.4/genericsuite/models/menu_options/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-14 20:59:38.732817 genericsuite-0.1.4/genericsuite/models/menu_options/menu_options.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.517187 genericsuite-0.1.4/genericsuite/models/users/__init__.py
+-rw-r--r--   0        0        0     7808 2024-04-14 21:53:15.726872 genericsuite-0.1.4/genericsuite/models/users/users.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:31:29.453063 genericsuite-0.1.4/genericsuite/util/__init__.py
+-rw-r--r--   0        0        0     5898 2024-04-09 22:31:29.498504 genericsuite-0.1.4/genericsuite/util/app_context.py
+-rw-r--r--   0        0        0     1608 2024-04-09 22:31:29.495938 genericsuite-0.1.4/genericsuite/util/app_logger.py
+-rw-r--r--   0        0        0     7160 2024-04-09 22:31:29.495160 genericsuite-0.1.4/genericsuite/util/aws.py
+-rw-r--r--   0        0        0     4456 2024-04-09 22:31:29.453731 genericsuite-0.1.4/genericsuite/util/blueprint_one.py
+-rw-r--r--   0        0        0     1837 2024-04-15 16:46:06.050850 genericsuite-0.1.4/genericsuite/util/config_dbdef_helpers.py
+-rw-r--r--   0        0        0     1430 2024-04-15 16:34:17.439193 genericsuite-0.1.4/genericsuite/util/current_user_data.py
+-rw-r--r--   0        0        0     4972 2024-04-09 22:31:29.454396 genericsuite-0.1.4/genericsuite/util/datetime_utilities.py
+-rw-r--r--   0        0        0    35651 2024-04-09 22:31:29.451096 genericsuite-0.1.4/genericsuite/util/db_abstractor.py
+-rw-r--r--   0        0        0      807 2024-04-09 22:31:29.496512 genericsuite-0.1.4/genericsuite/util/exceptions.py
+-rw-r--r--   0        0        0     2287 2024-04-09 22:31:29.452339 genericsuite-0.1.4/genericsuite/util/framework_abs_layer.py
+-rw-r--r--   0        0        0    47797 2024-04-20 14:07:10.782285 genericsuite-0.1.4/genericsuite/util/generic_db_helpers.py
+-rw-r--r--   0        0        0     5889 2024-04-19 10:56:43.916162 genericsuite-0.1.4/genericsuite/util/generic_db_middleware.py
+-rw-r--r--   0        0        0    11344 2024-04-20 14:07:18.960557 genericsuite-0.1.4/genericsuite/util/generic_endpoint_helpers.py
+-rw-r--r--   0        0        0     4695 2024-04-15 16:31:19.147626 genericsuite-0.1.4/genericsuite/util/jwt.py
+-rw-r--r--   0        0        0     3216 2024-04-09 22:31:29.449832 genericsuite-0.1.4/genericsuite/util/nav_helpers.py
+-rw-r--r--   0        0        0     4421 2024-04-09 22:31:29.495546 genericsuite-0.1.4/genericsuite/util/parse_multipart.py
+-rw-r--r--   0        0        0     1818 2024-04-09 22:31:29.496834 genericsuite-0.1.4/genericsuite/util/passwords.py
+-rw-r--r--   0        0        0      585 2024-04-09 22:31:29.498803 genericsuite-0.1.4/genericsuite/util/request_handler.py
+-rw-r--r--   0        0        0     6584 2024-04-19 11:09:04.568210 genericsuite-0.1.4/genericsuite/util/security.py
+-rw-r--r--   0        0        0     3318 2024-04-09 22:31:29.498126 genericsuite-0.1.4/genericsuite/util/send_email.py
+-rw-r--r--   0        0        0    16009 2024-04-09 22:31:29.497408 genericsuite-0.1.4/genericsuite/util/utilities.py
+-rw-r--r--   0        0        0     1463 2024-04-19 10:34:26.552832 genericsuite-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    16811 1970-01-01 00:00:00.000000 genericsuite-0.1.4/PKG-INFO
```

### Comparing `genericsuite-0.1.3/LICENSE` & `genericsuite-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/README.md` & `genericsuite-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # The GenericSuite for Python (backend version)
 
-![GenericSuite Logo](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/lib/images/gs_logo_circle.png)
+<img 
+    align="right"
+    width="100"
+    height="100"
+    src="https://genericsuite.carlosjramirez.com/images/gs_logo_circle.svg"
+    title="GenericSuite logo by Carlos J. Ramirez"
+/>
 
 [GenericSuite](https://www.carlosjramirez.com/genericsuite) is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including FastAPI, Flask and Chalice, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
 
 ## Features
 
 - **Framework Agnostic**: Supports FastAPI, Flask, and Chalice frameworks.
 - **Database Support**: Includes abstracted database operations for both MongoDB and DynamoDB, offering flexibility in choosing the database.
@@ -165,15 +171,15 @@
 APP_STAGE=qa
 ```
 ```
 # PROD
 APP_DEBUG=0
 APP_STAGE=prod
 ```
-5. Application secret ket (to be used in password encryption)
+5. Application secret key (to be used in password encryption)
 ```
 APP_SECRET_KEY=xxxx
 ```
 6. Application super administrator email
 ```
 APP_SUPERADMIN_EMAIL=xxxx
 ```
@@ -260,33 +266,35 @@
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
 GIT_SUBMODULE_LOCAL_PATH=lib/config_dbdef
-GIT_SUBMODULE_URL=git://github.com/username/configs_repo_name.git
+GIT_SUBMODULE_URL=git://github.com/username/exampleapp_configs.git
 ```
 11. Frontend application path (to copy version file during big lambdas deployment)
 ```
 FRONTEND_PATH=../exampleapp_frontend
 ```
 12. Local python version
 ```
 PYTHON_VERSION=3.11.5
 # PYTHON_VERSION=3.10.12
 # PYTHON_VERSION=3.9.17
 ```
 13. AWS Configuration
 ```
-AWS_S3_BUCKET_NAME_FE=aws-s3-bucket-name
+AWS_S3_BUCKET_NAME_FE=exampleapp-frontend-website-[STAGE]
 AWS_REGION=aws-region
-AWS_API_GATEWAY_STAGE=aws-api-gateway-stage
-AWS_LAMBDA_FUNCTION_NAME=aws-lambda-function-name
-AWS_LAMBDA_FUNCTION_ROLE=aws-lambda-function-role
+AWS_LAMBDA_FUNCTION_NAME=exampleapp-backend
+AWS_LAMBDA_FUNCTION_ROLE_QA=exampleapp-api_handler-role-qa
+AWS_LAMBDA_FUNCTION_ROLE_STAGING=exampleapp-api_handler-role-staging
+AWS_LAMBDA_FUNCTION_ROLE_DEMO=exampleapp-api_handler-role-demo
+AWS_LAMBDA_FUNCTION_ROLE_PROD=exampleapp-api_handler-role-prod
 AWS_SSL_CERTIFICATE_ARN=arn:aws:acm:AWS-REGION:AWS-ACCOUNT:certificate/AWS-CERTIFICATE-UUID
 ```
 15. SMTP Mail configuration
 ```
 SMTP_SERVER=smtp_server
 SMTP_PORT=smtp_port
 SMTP_USER=smtp_user
@@ -305,23 +313,132 @@
 # RUN_METHOD="chalice"
 # https:
 RUN_METHOD="chalice_docker"
 ```
 18. Tests configuration
 ```
 # Testing enndpoint
-TEST_APP_URL=http://app.exampleapp.local:5002
+TEST_APP_URL=http://app.exampleapp.local:5001
 ```
-19. Flask configuration
-```
-FLASK_APP=index.py
+19. Run methods and framework App directory and entry point
 ```
+#
+# Default App main code directory
+# for Chalice:
+# https://aws.github.io/chalice/topics/packaging.html
+# APP_DIR='.'
+# for FastAPI:
+# https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure
+# APP_DIR='app'
+# for Flask:
+# https://flask.palletsprojects.com/en/2.3.x/tutorial/layout/
+# APP_DIR='flaskr'
+#
+# Default App entry point code file
+# for Chalice:
+# https://aws.github.io/chalice/topics/packaging.html
+# APP_MAIN_FILE='app'
+# for FastAPI:
+# https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure
+# APP_MAIN_FILE='main'
+# for Flask:
+# https://flask.palletsprojects.com/en/2.3.x/tutorial/factory/
+# APP_MAIN_FILE='__init__'
+#
+```
+20. Flask configuration
+```
+FLASK_APP=__init__.py
+```
+
+## Framework installation
+
+* [FastAPI installation](https://fastapi.tiangolo.com/#installation)
+* [Flask installation](https://flask.palletsprojects.com/en/2.3.x/installation/)
+* [Chalice installation](https://aws.github.io/chalice/quickstart.html)
 
 ## App structure
 
+Suggested directory structure by framework:
+
+* [FastAPI directory structure](https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure)
+* [Flask directory structure](https://flask.palletsprojects.com/en/2.3.x/tutorial/layout/)
+* [Chalice directory structure](https://aws.github.io/chalice/topics/packaging.html)
+
+This is a suggested App development repository structure for a FastAPI project:
+
+```
+.
+├── app
+│   ├── __init__.py
+│   ├── main.py
+│   ├── dependencies.py
+│   └── routers
+│   │   ├── __init__.py
+│   │   ├── items.py
+│   │   └── users.py
+│   └── internal
+│       ├── __init__.py
+│       └── admin.py
+├── logs
+│   └── .gitignore
+├── .env
+├── .env.example
+├── .gitignore
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+├── package-lock.json
+├── package.json
+├── requirements.txt
+├── tests
+│   ├── .env.for_test
+│   ├── __init__.py
+│   ├── assets
+│   ├── conftest.py
+│   └── pytest.ini
+└── version.txt
+```
+
+This is a suggested App development repository structure for a Flask project:
+
+```
+.
+├── flaskr/
+│   ├── __init__.py
+│   ├── items.py
+│   ├── users.py
+│   ├── admin.py
+│   └── index.py
+├── logs
+│   └── .gitignore
+├── package-lock.json
+├── package.json
+├── requirements.txt
+├── tests
+│   ├── .env.for_test
+│   ├── __init__.py
+│   ├── assets
+│   ├── conftest.py
+│   └── pytest.ini
+├── .env
+├── .env.example
+├── .gitignore
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+└── version.txt
+```
+
 This is a suggested App development repository structure for a Chalice project:
 
 ```
 .
 ├── .chalice
 │   ├── config-example.json
 │   ├── config.json
@@ -331,26 +448,19 @@
 │   │   └── prod.json
 │   ├── deployment
 │   │   ├── deployment.zip
 │   │   └── sam.json
 │   ├── deployments
 │   ├── dynamodb_cf_template.yaml
 │   └── policy-qa.json
-├── .env
-├── .env.example
-├── .gitignore
-├── CHANGELOG.md
-├── LICENSE
-├── Makefile
-├── Pipfile
-├── Pipfile.lock
-├── README.md
-├── app.py
 ├── chalicelib
 │   └── endpoints
+│       ├── items.py
+│       ├── users.py
+│       ├── admin.py
 │       └── __init__.py
 ├── lib
 │   ├── .gitignore
 │   ├── config
 │   │   ├── __init__.py
 │   │   └── config.py
 │   ├── config_dbdef
@@ -365,23 +475,33 @@
 │       │   ├── __init__.py
 │       │   └── ai_gpt_fn_index.py
 │       ├── external_apis
 │       │   └── __init__.py
 │       └── utilities
 ├── logs
 │   └── .gitignore
-├── package-lock.json
-├── package.json
-├── requirements.txt
 ├── tests
 │   ├── .env.for_test
 │   ├── __init__.py
 │   ├── assets
 │   ├── conftest.py
 │   └── pytest.ini
+├── .env
+├── .env.example
+├── .gitignore
+├── app.py
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── package-lock.json
+├── package.json
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+├── requirements.txt
 └── version.txt
 
 ```
 
 ## Code examples and JSON configuration files
 
 The main menu, API endpoints and CRUD editor configurations are defined in the JSON configuration files.
```

### Comparing `genericsuite-0.1.3/genericsuite/chalicelib/endpoints/menu_options.py` & `genericsuite-0.1.4/genericsuite/chalicelib/endpoints/menu_options.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/chalicelib/endpoints/users.py` & `genericsuite-0.1.4/genericsuite/chalicelib/endpoints/users.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,41 +6,40 @@
 # from chalice.app import Request, Response
 from genericsuite.util.framework_abs_layer import Request, Response
 
 from genericsuite.util.blueprint_one import BlueprintOne
 
 from genericsuite.util.jwt import (
     request_authentication,
-    AuthorizedRequest,
+    # AuthorizedRequest,
 )
 
 from genericsuite.models.users.users import (
-    users_crud as users_crud_model,
+    # users_crud as users_crud_model,
     test_connection_handler as test_connection_handler_model,
     login_user as login_user_model,
     super_admin_create as super_admin_create_model,
-    password_encripted as password_encripted_model,
 )
 
 bp = BlueprintOne(__name__)
 
 
 HEADER_CREDS_ENTRY_NAME = 'Authorization'
 DEBUG = False
 
 
-@bp.route(
-    '/',
-    methods=['GET', 'POST', 'PUT', 'DELETE'],
-    authorizor=request_authentication(),
-)
-def users_crud(request: AuthorizedRequest,
-    other_params: Optional[dict] = None) -> Response:
-    """ User's CRUD operations (create, read, update, delete) """
-    return users_crud_model(request, other_params)
+# @bp.route(
+#     '/',
+#     methods=['GET', 'POST', 'PUT', 'DELETE'],
+#     authorizor=request_authentication(),
+# )
+# def users_crud(request: AuthorizedRequest,
+#     other_params: Optional[dict] = None) -> Response:
+#     """ User's CRUD operations (create, read, update, delete) """
+#     return users_crud_model(request, other_params)
 
 
 @bp.route(
     '/test',
     authorizor=request_authentication(),
 )
 def test_connection_handler(request: Request,
@@ -63,19 +62,7 @@
     '/supad-create',
     methods=['POST']
 )
 def super_admin_create(request: Request,
     other_params: Optional[dict] = None) -> Response:
     """Super admin user emergency creation"""
     return super_admin_create_model(request, other_params)
-
-
-@bp.route(
-    '/pas-enc',
-    methods=['POST'],
-    # authorizor=request_authentication(),
-)
-def password_encripted(request: Request,
-    other_params: Optional[dict] = None) -> Response:
-    """Returns the given string as a encrypted password
-    """
-    return password_encripted_model(request, other_params)
```

### Comparing `genericsuite-0.1.3/genericsuite/chalicelib/framework_abstraction.py` & `genericsuite-0.1.4/genericsuite/chalicelib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/chalicelib/util/create_app.py` & `genericsuite-0.1.4/genericsuite/chalicelib/util/create_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 # from chalice import Chalice
 framework_class = importlib.import_module("chalice")
 
 DEBUG = False
 
 
-# def create_app(app_name: str, framework_class: Any, cors_config_class: Any,
 def create_app(app_name: str, settings = None) -> Any:
     """ Create the Chalice App """
 
     if settings is None:
         settings = Config()
 
     chalice_app = framework_class.Chalice(app_name=app_name)
```

### Comparing `genericsuite-0.1.3/genericsuite/chalicelib/util/generic_endpoint_builder.py` & `genericsuite-0.1.4/genericsuite/chalicelib/util/generic_endpoint_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     settings = Config()
     cnf_db_base_path = settings.GIT_SUBMODULE_LOCAL_PATH
     definitions = get_json_def(json_file, f'{cnf_db_base_path}/backend', [])
 
     for definition in definitions:
         bp_name = definition['name']
         url_prefix = f"/{definition.get('url_prefix', bp_name)}"
-        blueprint = BlueprintOne(definition['name'])
+        blueprint = BlueprintOne(bp_name)
 
         if DEBUG:
             log_debug(
                 'GENERATE_BLUEPRINTS_FROM_JSON |' +
                 f' bp_name: {bp_name}' +
                 f' url_prefix: {url_prefix}'
             )
@@ -62,15 +62,15 @@
             other_params = {
                 "name": bp_name
             }
             other_params["params"] = route['params']
             if route_handler_type == "GenericEndpointHelper":
                 route_handler = generic_route_handler
             else:
-                route_handler = route['view_func1']
+                route_handler = route['view_function']
 
             if DEBUG:
                 log_debug(
                     'GENERATE_BLUEPRINTS_FROM_JSON |' +
                     f' route_endpoint: {route_endpoint}' +
                     f' route_methods: {route_methods}' +
                     f' route_handler_type: {route_handler_type}' +
```

### Comparing `genericsuite-0.1.3/genericsuite/config/config.py` & `genericsuite-0.1.4/genericsuite/config/config.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/config/config_from_db.py` & `genericsuite-0.1.4/genericsuite/config/config_from_db.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/config/logging.conf.yml` & `genericsuite-0.1.4/genericsuite/config/logging.conf.yml`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/constants/const_tables.py` & `genericsuite-0.1.4/genericsuite/constants/const_tables.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/fastapilib/framework_abstraction.py` & `genericsuite-0.1.4/genericsuite/flasklib/framework_abstraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,54 @@
+
 """
-FastAPI abstraction layer
+Flask abstraction layer
 """
-# from fastapi import Request as FastAPIRequest, Response as FastAPIResponse,
-#     Blueprint as FastAPIBlueprint
+# from flask import Request as FlaskRequest, Response as FlaskResponse
 import os
 import importlib
 
 DEBUG = False
 FRAMEWORK_LOADED = False
 FRAMEWORK = os.environ.get('CURRENT_FRAMEWORK', '').lower()
-if FRAMEWORK == 'fastapi':
+if FRAMEWORK == 'flask':
     try:
         framework_module = importlib.import_module(FRAMEWORK)
         FRAMEWORK_LOADED = True
         if DEBUG:
-            print(f'FastAPI abstraction | framework_module: {framework_module}')
+            print(f'Flask abstraction | framework_module: {framework_module}')
 
 
-        class FrameworkClass(framework_module.FastAPI):
+        class FrameworkClass(framework_module.Flask):
             """
             Framkework class cloned from the selected framework super class.
             """
 
 
-        class Request():
+        class Request(framework_module.request):
             """
             Request class cloned from the selected Request framework super class.
             This class is the one to be imported by the project modules
             """
 
 
-        class Response():
+        class Response(framework_module.response):
             """
             Response class cloned from the selected Response framework super class.
             This class is the one to be imported by the project modules
             """
 
 
-        class Blueprint(framework_module.APIRouter):
+        class Blueprint(framework_module.Blueprint):
             """
             Blueprint class cloned from the selected Blueprint framework super class.
             This class is the one to be imported by the project modules
             """
 
+
+        # class CORSConfig(framework_module.CORS):
+        #     """
+        #     CORSConfig class cloned from the selected CORSConfig framework super class.
+        #     This class is the one to be imported by the project modules.
+        #     """
+
     except ImportError as err:
         raise ImportError(f"Unable to import '{FRAMEWORK}': {err}") from None
```

### Comparing `genericsuite-0.1.3/genericsuite/flasklib/framework_abstraction.py` & `genericsuite-0.1.4/genericsuite/util/framework_abs_layer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-
 """
-Flask abstraction layer
+Framework abstraction layer
 """
-# from flask import Request as FlaskRequest, Response as FlaskResponse
 import os
 import importlib
 
-DEBUG = False
-FRAMEWORK_LOADED = False
-FRAMEWORK = os.environ.get('CURRENT_FRAMEWORK', '').lower()
-if FRAMEWORK == 'flask':
-    try:
-        framework_module = importlib.import_module(FRAMEWORK)
-        FRAMEWORK_LOADED = True
-        if DEBUG:
-            print(f'Flask abstraction | framework_module: {framework_module}')
-
-
-        class FrameworkClass(framework_module.Flask):
-            """
-            Framkework class cloned from the selected framework super class.
-            """
-
-
-        class Request(framework_module.request):
-            """
-            Request class cloned from the selected Request framework super class.
-            This class is the one to be imported by the project modules
-            """
-
-
-        class Response(framework_module.response):
-            """
-            Response class cloned from the selected Response framework super class.
-            This class is the one to be imported by the project modules
-            """
-
-
-        class Blueprint(framework_module.Blueprint):
-            """
-            Blueprint class cloned from the selected Blueprint framework super class.
-            This class is the one to be imported by the project modules
-            """
-
-
-        # class CORSConfig(framework_module.CORS):
-        #     """
-        #     CORSConfig class cloned from the selected CORSConfig framework super class.
-        #     This class is the one to be imported by the project modules.
-        #     """
+DEFAULT_FRAMEWORK = ''
 
-    except ImportError as err:
-        raise ImportError(f"Unable to import '{FRAMEWORK}': {err}") from None
+framework = os.environ.get('CURRENT_FRAMEWORK', DEFAULT_FRAMEWORK).lower()
+if framework not in ['chalice', 'fastapi', 'flask']:
+    raise ValueError("Unsupported or undefined CURRENT_FRAMEWORK:" +
+                     f" '{framework}'")
+
+module_base_path = f"genericsuite.{framework}lib"
+module_path = f"{module_base_path}.framework_abstraction"
+
+try:
+    framework_module = importlib.import_module(module_path)
+    if not framework_module or not framework_module.FRAMEWORK_LOADED:
+        raise ImportError(f"Framework '{module_path}' could no be loaded" +
+            " [FAL-E010]" +
+            f" | FRAMEWORK_LOADED={framework_module.FRAMEWORK_LOADED}")
+except ImportError as err:
+    raise ImportError(f"Unable to import module [1]: {err}") from None
+
+try:
+    create_app_path = f'{module_base_path}.util.create_app'
+    module_create_app = importlib.import_module(create_app_path)
+except ImportError as err:
+    raise ImportError(f"Unable to import module [2]: {err}") from None
+
+
+class FrameworkClass(framework_module.FrameworkClass):
+    """
+    Framkework class cloned from the selected framework super class.
+    E.g. chalice, fastapi, flask:
+        from flask import Flask
+        from fastapi import FastAPI
+        from chalice import Chalice
+    Will be:
+        from genericsuite.util.framework_abs_layer import FrameworkClass as Flask
+        from genericsuite.util.framework_abs_layer import FrameworkClass as FastAPI
+        from genericsuite.util.framework_abs_layer import FrameworkClass as Chalice
+    This class is the one to be imported by the project modules.
+    """
+
+
+class Request(framework_module.Request):
+    """
+    Request class cloned from the selected Request framework super class.
+    This class is the one to be imported by the project modules.
+    """
+
+
+class Response(framework_module.Response):
+    """
+    Response class cloned from the selected Response framework super class.
+    This class is the one to be imported by the project modules.
+    """
+
+
+class Blueprint(framework_module.Blueprint):
+    """
+    Blueprint class cloned from the selected Blueprint framework super class.
+    This class is the one to be imported by the project modules.
+    """
```

### Comparing `genericsuite-0.1.3/genericsuite/models/billing/billing_utilities.py` & `genericsuite-0.1.4/genericsuite/models/billing/billing_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/models/users/users.py` & `genericsuite-0.1.4/genericsuite/models/users/users.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 System users operations (CRUD, login, database test, super-admin creation)
 """
 from typing import Optional
 import json
 
-# from chalice.app import Request, Response
 from genericsuite.util.framework_abs_layer import Request, Response
 
-# from genericsuite.util.blueprint_one import BlueprintOne
 from genericsuite.util.db_abstractor import (
     set_db_request,
     test_connection,
 )
 from genericsuite.util.generic_db_helpers import (
     GenericDbHelper,
 )
 from genericsuite.util.app_logger import log_debug
 from genericsuite.util.jwt import (
-    # request_authentication,
     token_encode,
     get_basic_auth,
     AuthorizedRequest,
 )
 from genericsuite.util.passwords import Passwords
 from genericsuite.util.utilities import (
     return_resultset_jsonified_or_exception,
@@ -31,26 +28,18 @@
 )
 from genericsuite.config.config import Config
 from genericsuite.util.generic_endpoint_helpers import GenericEndpointHelper
 from genericsuite.config.config_from_db import app_context_and_set_env
 from genericsuite.constants.const_tables import get_constant
 
 
-# bp = BlueprintOne(__name__)
-
-
 HEADER_CREDS_ENTRY_NAME = 'Authorization'
 DEBUG = False
 
 
-# @bp.route(
-#     '/',
-#     methods=['GET', 'POST', 'PUT', 'DELETE'],
-#     authorizor=request_authentication(),
-# )
 def users_crud(request: AuthorizedRequest,
     other_params: Optional[dict] = None) -> Response:
     """ User's CRUD operations (create, read, update, delete) """
     if not other_params:
         other_params = {}
     # Set environment variables from the database configurations.
     app_context = app_context_and_set_env(request)
@@ -63,61 +52,58 @@
         app_context=app_context,
         json_file="users",
         url_prefix=__name__,
     )
     return ep_helper.generic_crud_main()
 
 
-# @bp.route(
-#     '/test',
-#     authorizor=request_authentication(),
-# )
 def test_connection_handler(request: Request,
     other_params: Optional[dict] = None) -> Response:
     """Connection handler test"""
     if not other_params:
         other_params = {}
     result = get_default_resultset()
     set_db_request(request)
     result['resultset']['collections'] = json.loads(test_connection())
     if DEBUG:
         log_debug(f'Test DB connection | request: {request}')
     return return_resultset_jsonified_or_exception(result)
 
 
-# @bp.route(
-#     '/login',
-#     methods=['GET', 'POST']
-# )
 def login_user(request: Request,
     other_params: Optional[dict] = None) -> Response:
     """User login"""
     if not other_params:
         other_params = {}
     psw_class = Passwords()
     dbo = GenericDbHelper(json_file="users", request=request)
     if DEBUG:
         log_debug(f'login_user | request: {request}')
         # log_debug('login_user | bp.current_request.to_dict(): ' +
         #           f'{bp.current_request.to_dict()}')
     result = get_default_resultset()
-    basic_auth_data = get_basic_auth(
-        request.headers.get(HEADER_CREDS_ENTRY_NAME, '')
-    )
-    if DEBUG:
-        log_debug(f'login_user | basic_auth_data: {basic_auth_data}')
-    if basic_auth_data['error']:
-        # 'Could not verify [L1]'
-        result['error_message'] = basic_auth_data['error_message']
-        return return_resultset_jsonified_or_exception(
-            result=result,
-            http_error=basic_auth_data['status_code']
+    if other_params.get('username') and other_params.get('password'):
+        username = other_params.get('username')
+        password = other_params.get('password')
+    else:
+        basic_auth_data = get_basic_auth(
+            request.headers.get(HEADER_CREDS_ENTRY_NAME, '')
         )
-    username = basic_auth_data['resultset']['user']
-    password = basic_auth_data['resultset']['password']
+        if DEBUG:
+            log_debug(f'login_user | basic_auth_data: {basic_auth_data}')
+        if basic_auth_data['error']:
+            # 'Could not verify [L1]'
+            result['error_message'] = basic_auth_data['error_message']
+            return return_resultset_jsonified_or_exception(
+                result=result,
+                http_error=basic_auth_data['status_code']
+            )
+        username = basic_auth_data['resultset']['user']
+        password = basic_auth_data['resultset']['password']
+
     user = dbo.fetch_row_by_entryname_raw('email', username)
     if user['error']:
         return return_resultset_jsonified_or_exception(user)
     if DEBUG:
         log_debug(f'login_user | user[resultset]: {user}')
     if user['resultset']:
         if 'passcode' in user['resultset']:
@@ -144,18 +130,14 @@
     else:
         result['error_message'] = 'Could not verify [L2]'
     if DEBUG:
         log_debug(f'login_user | FINAL result: {result}')
     return return_resultset_jsonified_or_exception(result, 401)
 
 
-# @bp.route(
-#     '/supad-create',
-#     methods=['POST']
-# )
 def super_admin_create(request: Request,
     other_params: Optional[dict] = None) -> Response:
     """Super admin user emergency creation"""
     # Set environment variables from the database configurations.
     app_context = app_context_and_set_env(request)
     if app_context.has_error():
         return return_resultset_jsonified_or_exception(
@@ -163,28 +145,34 @@
         )
     settings = Config(app_context)
     if not other_params:
         other_params = {}
     psw_class = Passwords()
     dbo = GenericDbHelper(json_file="users", request=request)
     result = get_default_resultset()
-    basic_auth_data = get_basic_auth(
-        request.headers.get(HEADER_CREDS_ENTRY_NAME, '')
-    )
-    if DEBUG:
-        log_debug(f'supad-create | basic_auth_data: {basic_auth_data}')
-    if basic_auth_data['error']:
-        result['error_message'] = basic_auth_data['error_message']
-        return return_resultset_jsonified_or_exception(
-            result=result,
-            http_error=basic_auth_data['status_code']
+
+    if other_params.get('username') and other_params.get('password'):
+        username = other_params.get('username')
+        password = other_params.get('password')
+    else:
+        basic_auth_data = get_basic_auth(
+            request.headers.get(HEADER_CREDS_ENTRY_NAME, '')
         )
+        if DEBUG:
+            log_debug(f'supad-create | basic_auth_data: {basic_auth_data}')
+        if basic_auth_data['error']:
+            result['error_message'] = basic_auth_data['error_message']
+            return return_resultset_jsonified_or_exception(
+                result=result,
+                http_error=basic_auth_data['status_code']
+            )
+
+        username = basic_auth_data['resultset']['user']
+        password = basic_auth_data['resultset']['password']
 
-    username = basic_auth_data['resultset']['user']
-    password = basic_auth_data['resultset']['password']
     if not username or not password:
         result['error_message'] = 'Could not verify [SAC1]'
     elif username != settings.APP_SUPERADMIN_EMAIL:
         result['error_message'] = 'Could not verify [SAC2]'
     elif not psw_class.verify_password(
          psw_class.encrypt_password(settings.APP_SECRET_KEY), password
          ):
@@ -216,32 +204,7 @@
         for field in dbo.get_mandatory_fields(record=request_body,
                                               is_create=True):
             if field not in request_body:
                 request_body[field] = ''
         result = dbo.create_row(request_body)
 
     return return_resultset_jsonified_or_exception(result)
-
-
-# @bp.route(
-#     '/pas-enc',
-#     methods=['POST'],
-#     # authorizor=request_authentication(),
-# )
-def password_encripted(request: Request,
-    other_params: Optional[dict] = None) -> Response:
-    """Returns the given string as a encrypted password
-    """
-    if not other_params:
-        other_params = {}
-    psw_class = Passwords()
-    request_body = get_request_body(request)
-    result = get_default_resultset()
-    result['resultset'] = {}
-    if request_body.get('passwd', None) is not None:
-        result['resultset'] = {
-            # 'orig_pass': request_body.get('passwd'),
-            'enc_pass': psw_class.encrypt_password(request_body.get('passwd'))
-        }
-    else:
-        result['error_message'] = 'Parameter not received [PSEN1]'
-    return return_resultset_jsonified_or_exception(result)
```

### Comparing `genericsuite-0.1.3/genericsuite/util/app_context.py` & `genericsuite-0.1.4/genericsuite/util/app_context.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/app_logger.py` & `genericsuite-0.1.4/genericsuite/util/app_logger.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/aws.py` & `genericsuite-0.1.4/genericsuite/util/aws.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/blueprint_one.py` & `genericsuite-0.1.4/genericsuite/util/blueprint_one.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/config_dbdef_helpers.py` & `genericsuite-0.1.4/genericsuite/util/config_dbdef_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     Returns:
         dict: JSON definition.
     """
     if not default_value:
         default_value = {}
 
-    # app_path = os.path.dirname(__file__)
     app_path = os.getcwd()
     filename = f'{app_path}/{dir_name}/{json_file_name}.json'
     if not os.path.isfile(filename):
         if DEBUG:
             log_debug(f'File {filename} not found.')
         return default_value
     with open(filename, encoding="utf-8") as json_file:
@@ -57,8 +56,9 @@
             cnf_db = second_json.copy()
         elif isinstance(cnf_db, dict):
             cnf_db.update(second_json)
         else:
             cnf_db += second_json
     if not cnf_db:
         cnf_db = {}
+    # print(f'>>> CNF_DB\n| json_file_name: {json_file_name}\n| cnf_db: {cnf_db}')
     return cnf_db
```

### Comparing `genericsuite-0.1.3/genericsuite/util/current_user_data.py` & `genericsuite-0.1.4/genericsuite/util/current_user_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 NON_AUTH_REQUEST_USER_ID = "[N/A/R]"
 
 def get_curr_user_id(request: AuthorizedRequest) -> str:
     """Get the current user ID"""
     user_id = None
     authorized_request = hasattr(request, 'user') and request.user
     if authorized_request:
-        user_id = request.user.get("public_id")
+        # user_id = request.user.get("public_id")
+        user_id = request.user.public_id
     else:
         # Is a non-authorization request, so returns the identificator
         # 'N/A/R' meaning "Non-Authorization Request"
         user_id = NON_AUTH_REQUEST_USER_ID
     return user_id
```

### Comparing `genericsuite-0.1.3/genericsuite/util/datetime_utilities.py` & `genericsuite-0.1.4/genericsuite/util/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/db_abstractor.py` & `genericsuite-0.1.4/genericsuite/util/db_abstractor.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/exceptions.py` & `genericsuite-0.1.4/genericsuite/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/generic_db_helpers.py` & `genericsuite-0.1.4/genericsuite/util/generic_db_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/generic_db_middleware.py` & `genericsuite-0.1.4/genericsuite/util/generic_db_middleware.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/generic_endpoint_helpers.py` & `genericsuite-0.1.4/genericsuite/util/generic_endpoint_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,69 +86,83 @@
             f' | query_params: {self.query_params}'
             f' | request_body: {self.request_body}')
 
         if self.dbo.error_message:
             return error_resultset(self.dbo.error_message)
 
         row_id = self.query_params.get('id')
-        additional_query_params = self.dbo.cnf_db.get('additional_query_params')
         like_param = self.get_like_param()
         comb_param = self.get_comb_param()
 
+        additional_query_params = self.dbo.cnf_db.get('additional_query_params')
+
         (limit, skip, page) = get_navigation_params(self.request)
 
         _ = DEBUG and log_debug(f' | row_id: {row_id}' +
             f' | additional_query_params: {additional_query_params}' +
             f' | limit: {limit} | skip: {skip} | page: {page}' + 
+            f' | like_param: {like_param} | comb_param: {comb_param}' + 
             f'\n | request_body: {self.request_body}')
 
-        if self.request.method == 'POST':
+        if self.request.method.upper() == 'POST':
             # Create
+            _ = DEBUG and \
+                log_debug(f'GCM-1.1) CREATE {self.data["name"]}...')
             result = self.dbo.create_row(self.request_body)
             _ = DEBUG and \
-                log_debug(f'GCM-1) CREATE {self.data["name"]}' +
+                log_debug(f'GCM-1.2) CREATE {self.data["name"]}' +
                 f'\n | request_body: {self.request_body}' +
                 f'\n | result: {result}')
-        elif self.request.method == 'PUT':
+        elif self.request.method.upper() == 'PUT':
             # Update
+            _ = DEBUG and log_debug(f'GCM-2.1) UPDATE {self.data["name"]}...')
             options = {"update_item": self.query_params.get("update_item", "0")}
             result = self.dbo.update_row(record=self.request_body,
                                          options=options)
-            _ = DEBUG and log_debug(f'GCM-2) UPDATE {self.data["name"]}' +
+            _ = DEBUG and log_debug(f'GCM-2.2) UPDATE {self.data["name"]}' +
                 f'\n | request_body: {self.request_body}' +
                 f'\n | result: {result}')
-        elif self.request.method == 'DELETE' and row_id is not None:
+        elif self.request.method.upper() == 'DELETE' and row_id is not None:
             # Delete
+            _ = DEBUG and log_debug(f'GCM-3.1) DELETE {self.data["name"]}' +
+                f' | row_id: {row_id}...')
             result = self.dbo.delete_row(row_id)
-            _ = DEBUG and log_debug(f'GCM-3) DELETE {self.data["name"]}' +
+            _ = DEBUG and log_debug(f'GCM-3.2) DELETE {self.data["name"]}' +
                 f' | row_id: {row_id}\n | result: {result}')
         elif row_id is not None:
             # Get one row by _id
+            _ = DEBUG and log_debug(f'GCM-4.1) GET ROW {self.data["name"]}' +
+                f' BY ID: {row_id}...')
             result = self.dbo.fetch_row(row_id)
-            _ = DEBUG and log_debug(f'GCM-4) GET ROW {self.data["name"]}' +
+            _ = DEBUG and log_debug(f'GCM-4.2) GET ROW {self.data["name"]}' +
                 f' BY ID: {row_id}\n | result: {result}')
         elif like_param == "1":
             # Like Search
+            _ = DEBUG and log_debug(f'GCM-5.1) LIKE SEARCH {self.data["name"]}' +
+                f'\n | {like_query_params}...')
             like_query_params = self.get_like_query_params()
             result = self.dbo.fetch_list(
                 skip=skip,
                 limit=limit,
                 like_query_params=like_query_params,
                 combinator=comb_param
             )
             if not result['resultset']:
                 result = error_resultset(
                     f'Error: {self.data["name"]} {like_query_params} ' + \
                     "doesn't exist", "GEM3")
-            _ = DEBUG and log_debug(f'GCM-5) LIKE SEARCH {self.data["name"]}' +
+            _ = DEBUG and log_debug(f'GCM-5.2) LIKE SEARCH {self.data["name"]}' +
                 f'\n | {like_query_params}\n | result: {result}')
         elif additional_query_params is not None and \
              all(param in self.query_params
              for param in additional_query_params):
             # Get one row by additional_query_params
+            _ = DEBUG and log_debug('GCM-6.1) SEARCH BY ATTRIBUTE' +
+                f' {self.data["name"]} BY {param_name}: {param_value}' +
+                '...')
             result = get_default_resultset()
             param_name = None
             param_value = None
             for key in additional_query_params:
                 if not self.query_params.get(key):
                     continue
                 param_name = key
@@ -160,21 +174,24 @@
                 if not result['resultset']:
                     result = error_resultset(
                         f'ERROR: {self.data["name"]} {param_value} ' + \
                         "doesn't exist", "GEM1")
                 else:
                     result['resultset'] = dumps(result['resultset'])
                 break
-            _ = DEBUG and log_debug('GCM-6) SEARCH BY ATTRIBUTE' +
+            _ = DEBUG and log_debug('GCM-6.2) SEARCH BY ATTRIBUTE' +
                 f' {self.data["name"]} BY {param_name}: {param_value}' +
                 f'\n | result: {result}')
         else:
             # Fetch row list
+            _ = DEBUG and log_debug(f'GCM-7.1) {self.data["name"]} list |' +
+                f' skip: {skip}, limit: {limit}, page: {page}' +
+                f'...')
             result = self.dbo.fetch_list(skip, limit, self.query_params)
-            _ = DEBUG and log_debug(f'GCM-7) {self.data["name"]} list |' +
+            _ = DEBUG and log_debug(f'GCM-7.2) {self.data["name"]} list |' +
                 f' skip: {skip}, limit: {limit}, page: {page}' +
                 f'\n | result {result}')
         return return_resultset_jsonified_or_exception(result)
 
     def generic_raw_json(self) -> dict:
         """
         Get the raw JSON data.
@@ -206,37 +223,37 @@
         filters = {}
         if array_child_id_value is not None:
             filters[self.dbo.array_field_key] = array_child_id_value
         like_param = self.get_like_param()
         comb_param = self.get_comb_param()
         result = None
         # Create
-        if self.request.method == 'POST':
+        if self.request.method.upper() == 'POST':
             _ = DEBUG and log_debug(f'>>> {self.data["name"]}_crud | ' +
                 f'PUT request_body = {self.request_body}')
             result = self.dbo.add_array_item_to_row(self.request_body)
         # Delete
-        elif self.request.method == 'DELETE':
+        elif self.request.method.upper() == 'DELETE':
             _ = DEBUG and log_debug(f'>>> {self.data["name"]}_crud | ' +
                 f'DELETE request_body = {self.request_body}')
             result = self.dbo.remove_array_item_from_row(self.request_body)
         # Modify
-        elif self.request.method == 'PUT':
+        elif self.request.method.upper() == 'PUT':
             # When one element needs to be modified, first remove it,
             # then add it again
             _ = DEBUG and log_debug(f'>>> {self.data["name"]}_crud | ' +
                 f'POST request_body = {self.request_body}')
             remove_operation_result = \
                 self.dbo.remove_array_item_from_row(self.request_body)
             if remove_operation_result['error']:
                 result = remove_operation_result
             else:
                 result = self.dbo.add_array_item_to_row(self.request_body)
         # List
-        elif self.request.method == 'GET':
+        elif self.request.method.upper() == 'GET':
             # Get the list (paginated) or one especific element
             like_query_params = (
                 self.get_like_query_params() if like_param == "1" else {})
             _ = DEBUG and log_debug(f'>>> {self.data["name"]}_crud | GET' +
                 f' array_parent_id_value: {array_parent_id_value}' +
                 f'\n | filters: {filters}, skip: {skip}, limit: {limit}' +
                 f', page: {page}, like_query_params: {like_query_params}' +
```

### Comparing `genericsuite-0.1.3/genericsuite/util/jwt.py` & `genericsuite-0.1.4/genericsuite/util/jwt.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 JWT Library
 """
 import base64
 from typing import Callable
 import datetime
 
 import jwt
+from pydantic import BaseModel
 
 from genericsuite.util.framework_abs_layer import Request
 
 from genericsuite.util.app_logger import log_debug, log_error
 from genericsuite.util.utilities import (
     standard_error_return,
     get_default_resultset,
@@ -21,15 +22,15 @@
 
 # ----------------------- JWT -----------------------
 
 EXPIRATION_MINUTES = 30
 DEBUG = False
 
 
-class AuthTokenPayload:
+class AuthTokenPayload(BaseModel):
     """
     Represents the user's payload structure of the JWT token.
     """
     public_id: str
 
 
 class AuthorizedRequest(Request):
@@ -49,53 +50,66 @@
         None
 
     Returns:
         Callable[[Request], AuthorizedRequest]: A function that performs
         request authentication.
     """
     def create_auth_request(request: Request) -> AuthorizedRequest:
-        if settings.HEADER_TOKEN_ENTRY_NAME not in request.headers:
-            return standard_error_return('A valid token is missing')
-        try:
-            token_raw = request.headers[settings.HEADER_TOKEN_ENTRY_NAME]
-            jwt_token = token_raw.replace('Bearer ', '')
-            if DEBUG:
-                log_debug('||| REQUEST_AUTHENTICATION' +
-                    '\n | HEADER_TOKEN_ENTRY_NAME: ' +
-                    f'{settings.HEADER_TOKEN_ENTRY_NAME}' +
-                    f'\n | token_raw: {token_raw}' +
-                    f'\n | jwt_token: {jwt_token}' +
-                    # f'\n | settings.APP_SECRET_KEY: {settings.APP_SECRET_KEY}' +
-                    '\n')
-            jws_token_data = jwt.decode(
-                jwt_token,
-                settings.APP_SECRET_KEY,
-                algorithms="HS256",
-            )
-            if DEBUG:
-                log_debug('||| REQUEST_AUTHENTICATION' +
-                    f' | jws_token_data = {jws_token_data}')
-            authorized_request = AuthorizedRequest(
-                # type: ignore[attr-defined]
-                request.to_original_event(),
-                # type: ignore[attr-defined]
-                lambda_context=request.lambda_context
-            )
-            authorized_request.user = jws_token_data
-            if DEBUG:
-                log_debug('||| REQUEST_AUTHENTICATION' +
-                    f' | authorized_request = {authorized_request}')
-        except Exception as err:
-            log_error('REQUEST_AUTHENTICATION' +
-                f' | Exception = {str(err)}')
-            return standard_error_return('Token is invalid')
-        return authorized_request
+        return get_general_authorized_request(request)
     return create_auth_request
 
 
+def get_general_authorized_request(request: Request) -> AuthorizedRequest:
+    """
+    Get the authorized request from the request object.
+
+    Args:
+        request (Request): The request object.
+
+    Returns:
+        AuthorizedRequest: The authorized request.
+    """
+    if settings.HEADER_TOKEN_ENTRY_NAME not in request.headers:
+        return standard_error_return('A valid token is missing')
+    try:
+        token_raw = request.headers[settings.HEADER_TOKEN_ENTRY_NAME]
+        jwt_token = token_raw.replace('Bearer ', '')
+        if DEBUG:
+            log_debug('||| REQUEST_AUTHENTICATION' +
+                '\n | HEADER_TOKEN_ENTRY_NAME: ' +
+                f'{settings.HEADER_TOKEN_ENTRY_NAME}' +
+                f'\n | token_raw: {token_raw}' +
+                f'\n | jwt_token: {jwt_token}' +
+                # f'\n | settings.APP_SECRET_KEY: {settings.APP_SECRET_KEY}' +
+                '\n')
+        jws_token_data = jwt.decode(
+            jwt_token,
+            settings.APP_SECRET_KEY,
+            algorithms="HS256",
+        )
+        if DEBUG:
+            log_debug('||| REQUEST_AUTHENTICATION' +
+                f' | jws_token_data = {jws_token_data}')
+        authorized_request = AuthorizedRequest(
+            # type: ignore[attr-defined]
+            event_dict=request.to_original_event(),
+            # type: ignore[attr-defined]
+            lambda_context=request.lambda_context,
+            user = jws_token_data,
+        )
+        if DEBUG:
+            log_debug('||| REQUEST_AUTHENTICATION' +
+                f' | authorized_request = {authorized_request}')
+    except Exception as err:
+        log_error('REQUEST_AUTHENTICATION' +
+            f' | Exception = {str(err)}')
+        return standard_error_return('Token is invalid')
+    return authorized_request
+
+
 def token_encode(user):
     """
     Encode a JWT token for the given user.
 
     Args:
         user: The user for whom the token is being encoded.
```

### Comparing `genericsuite-0.1.3/genericsuite/util/nav_helpers.py` & `genericsuite-0.1.4/genericsuite/util/nav_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/parse_multipart.py` & `genericsuite-0.1.4/genericsuite/util/parse_multipart.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/passwords.py` & `genericsuite-0.1.4/genericsuite/util/passwords.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/request_handler.py` & `genericsuite-0.1.4/genericsuite/util/request_handler.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/security.py` & `genericsuite-0.1.4/genericsuite/util/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,18 +161,18 @@
 def verify_user_filter(app_context: AppContext) -> dict:
     """
     Verify the user filter in the endpoints that requires the user_id
     parameter.
     """
     request = app_context.get_request()
     vuf_response = get_default_resultset()
-    if request.method in ['GET', 'DELETE']:
+    if request.method.upper() in ['GET', 'DELETE']:
         query_params = get_query_params(request)
         user_id = query_params.get('user_id')
-    else:  # request.method in ['POST', 'PUT']:
+    else:  # request.method.upper() in ['POST', 'PUT']:
         form_data = get_request_body(request)
         user_id = form_data.get('user_id')
     if DEBUG:
         log_debug(f'VUF-1) VERIFY_USER_FILTER | user_id: {user_id}')
     if not user_id:
         vuf_response['error'] = True
         # Elements to build the Response()
```

### Comparing `genericsuite-0.1.3/genericsuite/util/send_email.py` & `genericsuite-0.1.4/genericsuite/util/send_email.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/genericsuite/util/utilities.py` & `genericsuite-0.1.4/genericsuite/util/utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.3/pyproject.toml` & `genericsuite-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "genericsuite"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="Carlos J. Ramirez", email="<tomkat_cr@yahoo.com>" }
 ]
 description = "The GenericSuite for Python (backend version)"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/tomkat-cr/genericsuite-be"
+Homepage = "https://genericsuite.carlosjramirez.com/Backend-Development/GenericSuite-Core/"
 Issues = "https://github.com/tomkat-cr/genericsuite-be/issues"
 
 [tool.poetry]
 name = "genericsuite"
-version = "0.1.3"
+version = "0.1.4"
 description = "The GenericSuite for Python (backend version)"
 authors = ["Carlos J. Ramirez <tomkat_cr@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tomkat-cr/genericsuite-be.git"
 packages = [
     { include = "genericsuite" }
```

### Comparing `genericsuite-0.1.3/PKG-INFO` & `genericsuite-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genericsuite
-Version: 0.1.3
+Version: 0.1.4
 Summary: The GenericSuite for Python (backend version)
 Home-page: https://github.com/tomkat-cr/genericsuite-be.git
 License: MIT
 Author: Carlos J. Ramirez
 Author-email: tomkat_cr@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,21 @@
 Requires-Dist: werkzeug (>=3.0.1,<4.0.0)
 Requires-Dist: wheel (>=0.41.3,<0.42.0)
 Project-URL: Repository, https://github.com/tomkat-cr/genericsuite-be.git
 Description-Content-Type: text/markdown
 
 # The GenericSuite for Python (backend version)
 
-![GenericSuite Logo](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/lib/images/gs_logo_circle.png)
+<img 
+    align="right"
+    width="100"
+    height="100"
+    src="https://genericsuite.carlosjramirez.com/images/gs_logo_circle.svg"
+    title="GenericSuite logo by Carlos J. Ramirez"
+/>
 
 [GenericSuite](https://www.carlosjramirez.com/genericsuite) is a versatile backend solution, designed to provide a comprehensive suite of features for Python APIs. It supports various frameworks including FastAPI, Flask and Chalice, making it adaptable to a range of projects. This repository contains the backend logic, utilities, and configurations necessary to build and deploy scalable and maintainable applications.
 
 ## Features
 
 - **Framework Agnostic**: Supports FastAPI, Flask, and Chalice frameworks.
 - **Database Support**: Includes abstracted database operations for both MongoDB and DynamoDB, offering flexibility in choosing the database.
@@ -195,15 +201,15 @@
 APP_STAGE=qa
 ```
 ```
 # PROD
 APP_DEBUG=0
 APP_STAGE=prod
 ```
-5. Application secret ket (to be used in password encryption)
+5. Application secret key (to be used in password encryption)
 ```
 APP_SECRET_KEY=xxxx
 ```
 6. Application super administrator email
 ```
 APP_SUPERADMIN_EMAIL=xxxx
 ```
@@ -290,33 +296,35 @@
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
 GIT_SUBMODULE_LOCAL_PATH=lib/config_dbdef
-GIT_SUBMODULE_URL=git://github.com/username/configs_repo_name.git
+GIT_SUBMODULE_URL=git://github.com/username/exampleapp_configs.git
 ```
 11. Frontend application path (to copy version file during big lambdas deployment)
 ```
 FRONTEND_PATH=../exampleapp_frontend
 ```
 12. Local python version
 ```
 PYTHON_VERSION=3.11.5
 # PYTHON_VERSION=3.10.12
 # PYTHON_VERSION=3.9.17
 ```
 13. AWS Configuration
 ```
-AWS_S3_BUCKET_NAME_FE=aws-s3-bucket-name
+AWS_S3_BUCKET_NAME_FE=exampleapp-frontend-website-[STAGE]
 AWS_REGION=aws-region
-AWS_API_GATEWAY_STAGE=aws-api-gateway-stage
-AWS_LAMBDA_FUNCTION_NAME=aws-lambda-function-name
-AWS_LAMBDA_FUNCTION_ROLE=aws-lambda-function-role
+AWS_LAMBDA_FUNCTION_NAME=exampleapp-backend
+AWS_LAMBDA_FUNCTION_ROLE_QA=exampleapp-api_handler-role-qa
+AWS_LAMBDA_FUNCTION_ROLE_STAGING=exampleapp-api_handler-role-staging
+AWS_LAMBDA_FUNCTION_ROLE_DEMO=exampleapp-api_handler-role-demo
+AWS_LAMBDA_FUNCTION_ROLE_PROD=exampleapp-api_handler-role-prod
 AWS_SSL_CERTIFICATE_ARN=arn:aws:acm:AWS-REGION:AWS-ACCOUNT:certificate/AWS-CERTIFICATE-UUID
 ```
 15. SMTP Mail configuration
 ```
 SMTP_SERVER=smtp_server
 SMTP_PORT=smtp_port
 SMTP_USER=smtp_user
@@ -335,23 +343,132 @@
 # RUN_METHOD="chalice"
 # https:
 RUN_METHOD="chalice_docker"
 ```
 18. Tests configuration
 ```
 # Testing enndpoint
-TEST_APP_URL=http://app.exampleapp.local:5002
+TEST_APP_URL=http://app.exampleapp.local:5001
 ```
-19. Flask configuration
-```
-FLASK_APP=index.py
+19. Run methods and framework App directory and entry point
 ```
+#
+# Default App main code directory
+# for Chalice:
+# https://aws.github.io/chalice/topics/packaging.html
+# APP_DIR='.'
+# for FastAPI:
+# https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure
+# APP_DIR='app'
+# for Flask:
+# https://flask.palletsprojects.com/en/2.3.x/tutorial/layout/
+# APP_DIR='flaskr'
+#
+# Default App entry point code file
+# for Chalice:
+# https://aws.github.io/chalice/topics/packaging.html
+# APP_MAIN_FILE='app'
+# for FastAPI:
+# https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure
+# APP_MAIN_FILE='main'
+# for Flask:
+# https://flask.palletsprojects.com/en/2.3.x/tutorial/factory/
+# APP_MAIN_FILE='__init__'
+#
+```
+20. Flask configuration
+```
+FLASK_APP=__init__.py
+```
+
+## Framework installation
+
+* [FastAPI installation](https://fastapi.tiangolo.com/#installation)
+* [Flask installation](https://flask.palletsprojects.com/en/2.3.x/installation/)
+* [Chalice installation](https://aws.github.io/chalice/quickstart.html)
 
 ## App structure
 
+Suggested directory structure by framework:
+
+* [FastAPI directory structure](https://fastapi.tiangolo.com/tutorial/bigger-applications/?h=directory+structure#an-example-file-structure)
+* [Flask directory structure](https://flask.palletsprojects.com/en/2.3.x/tutorial/layout/)
+* [Chalice directory structure](https://aws.github.io/chalice/topics/packaging.html)
+
+This is a suggested App development repository structure for a FastAPI project:
+
+```
+.
+├── app
+│   ├── __init__.py
+│   ├── main.py
+│   ├── dependencies.py
+│   └── routers
+│   │   ├── __init__.py
+│   │   ├── items.py
+│   │   └── users.py
+│   └── internal
+│       ├── __init__.py
+│       └── admin.py
+├── logs
+│   └── .gitignore
+├── .env
+├── .env.example
+├── .gitignore
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+├── package-lock.json
+├── package.json
+├── requirements.txt
+├── tests
+│   ├── .env.for_test
+│   ├── __init__.py
+│   ├── assets
+│   ├── conftest.py
+│   └── pytest.ini
+└── version.txt
+```
+
+This is a suggested App development repository structure for a Flask project:
+
+```
+.
+├── flaskr/
+│   ├── __init__.py
+│   ├── items.py
+│   ├── users.py
+│   ├── admin.py
+│   └── index.py
+├── logs
+│   └── .gitignore
+├── package-lock.json
+├── package.json
+├── requirements.txt
+├── tests
+│   ├── .env.for_test
+│   ├── __init__.py
+│   ├── assets
+│   ├── conftest.py
+│   └── pytest.ini
+├── .env
+├── .env.example
+├── .gitignore
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+└── version.txt
+```
+
 This is a suggested App development repository structure for a Chalice project:
 
 ```
 .
 ├── .chalice
 │   ├── config-example.json
 │   ├── config.json
@@ -361,26 +478,19 @@
 │   │   └── prod.json
 │   ├── deployment
 │   │   ├── deployment.zip
 │   │   └── sam.json
 │   ├── deployments
 │   ├── dynamodb_cf_template.yaml
 │   └── policy-qa.json
-├── .env
-├── .env.example
-├── .gitignore
-├── CHANGELOG.md
-├── LICENSE
-├── Makefile
-├── Pipfile
-├── Pipfile.lock
-├── README.md
-├── app.py
 ├── chalicelib
 │   └── endpoints
+│       ├── items.py
+│       ├── users.py
+│       ├── admin.py
 │       └── __init__.py
 ├── lib
 │   ├── .gitignore
 │   ├── config
 │   │   ├── __init__.py
 │   │   └── config.py
 │   ├── config_dbdef
@@ -395,23 +505,33 @@
 │       │   ├── __init__.py
 │       │   └── ai_gpt_fn_index.py
 │       ├── external_apis
 │       │   └── __init__.py
 │       └── utilities
 ├── logs
 │   └── .gitignore
-├── package-lock.json
-├── package.json
-├── requirements.txt
 ├── tests
 │   ├── .env.for_test
 │   ├── __init__.py
 │   ├── assets
 │   ├── conftest.py
 │   └── pytest.ini
+├── .env
+├── .env.example
+├── .gitignore
+├── app.py
+├── CHANGELOG.md
+├── LICENSE
+├── Makefile
+├── package-lock.json
+├── package.json
+├── Pipfile
+├── Pipfile.lock
+├── README.md
+├── requirements.txt
 └── version.txt
 
 ```
 
 ## Code examples and JSON configuration files
 
 The main menu, API endpoints and CRUD editor configurations are defined in the JSON configuration files.
```

