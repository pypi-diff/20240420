# Comparing `tmp/pan_ztp_patcher-0.2.6.tar.gz` & `tmp/pan_ztp_patcher-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.6.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.7.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.6.tar` & `pan_ztp_patcher-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     3912 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/__init__.py
--rw-r--r--   0        0        0    13855 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1026 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    37511 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      597 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3524 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/__init__.py
+-rw-r--r--   0        0        0    13855 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1026 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    37511 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      597 2024-04-19 23:37:12.329777 pan_ztp_patcher-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.7/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.6/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.2.7/pan_ztp_patcher/app.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.6/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.7/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.6/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.7/pan_ztp_patcher/ztp_patcher.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.6/pyproject.toml` & `pan_ztp_patcher-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pan-ztp-patcher"
-version = "0.2.6"
+version = "0.2.7"
 description = "Update content version on PAN-OS firewalls"
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 ztp_patcher = "pan_ztp_patcher.app:main"
```

### Comparing `pan_ztp_patcher-0.2.6/PKG-INFO` & `pan_ztp_patcher-0.2.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,87 @@
-Metadata-Version: 2.1
-Name: pan-ztp-patcher
-Version: 0.2.6
-Summary: Update content version on PAN-OS firewalls
-License: Apache2.0
-Author: Calvin Remsburg
-Author-email: cremsburg.dev@gmail.com
-Requires-Python: >=3.8.1
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: paramiko (>=3.4.0,<4.0.0)
-Requires-Dist: python-dotenv (==0.21.1)
-Description-Content-Type: text/markdown
-
 # PAN-OS ZTP Patcher
 
-The PAN-OS ZTP Patcher is a utility designed to streamline the process of updating the content version on PAN-OS firewalls during the Zero Touch Provisioning (ZTP) process. It leverages a Raspberry Pi Zero appliance to automate the content update procedure, eliminating the need for manual intervention.
+The PAN-OS ZTP Patcher is a sophisticated Python utility designed to automate content version updates on PAN-OS firewalls during the Zero Touch Provisioning (ZTP) process. Utilizing a Raspberry Pi, this tool helps network administrators ensure their firewalls are always updated with the latest security features without manual intervention.
 
 ## Use Case
 
-When deploying PAN-OS firewalls in a network environment, it is often necessary to ensure that the firewalls have the latest content version installed. This content includes threat signatures, application definitions, and other critical updates that enhance the security posture of the firewalls.
-
-The PAN-OS ZTP Patcher simplifies this process by automating the content update during the ZTP workflow. By connecting a Raspberry Pi Zero appliance to the management interface of the firewall and running this utility, the content version can be seamlessly updated without requiring manual steps.
+Deploying PAN-OS firewalls typically requires ensuring they are updated with the latest content versions, including threat signatures and application definitions. The PAN-OS ZTP Patcher automates these updates during the ZTP process, interfacing directly through a Raspberry Pi connected to the firewall's management interface.
 
-Key benefits of using the PAN-OS ZTP Patcher:
+### Key Benefits
 
-- Automates the content update process during ZTP, saving time and effort.
-- Ensures that PAN-OS firewalls have the latest content version installed from the start.
-- Reduces the risk of human error associated with manual content updates.
-- Enables faster and more efficient deployment of PAN-OS firewalls in network environments.
+- **Automated Content Updates**: Streamlines the ZTP process by automating updates, reducing time and effort.
+- **Enhanced Security**: Ensures that firewalls receive the latest updates immediately upon deployment.
+- **Reduced Human Error**: Minimizes the risks associated with manual updates.
+- **Efficient Deployments**: Speeds up the setup process for PAN-OS firewalls with up-to-date configurations.
 
 ## Requirements
 
-To use the PAN-OS ZTP Patcher, you need the following:
-
-- Raspberry Pi Zero with Raspberry Pi OS and Python 3.7 or higher installed.
-- USB to Ethernet adapter to connect the Raspberry Pi Zero to the management interface of the PAN-OS firewall.
-- Ethernet interface on the Raspberry Pi Zero connected to the management interface of the PAN-OS firewall.
-- Local IP address of 192.168.1.2/24 assigned to the Ethernet interface of the Raspberry Pi Zero.
+- Raspberry Pi with the latest OS and Python 3.7 or higher.
+- USB to Ethernet adapter connecting the Raspberry Pi to the firewall's management interface.
+- Configured network settings on the Raspberry Pi's Ethernet interface to 192.168.1.2/24.
 
 ## Installation
 
-You can install the PAN-OS ZTP Patcher using pip:
+Install the PAN-OS ZTP Patcher via pip:
 
 ```bash
 pip install pan_ztp_patcher
 ```
 
 ## Usage
 
-To use the PAN-OS ZTP Patcher, run the following command:
+Run the ZTP Patcher with the following command structure, providing the necessary parameters:
+
+### Parameters
+
+- `--env_file`: Path to the `.env` file containing environment variables (default: `.env`).
+- `--pi_hostname`: Hostname or IP address of the Raspberry Pi.
+- `--pi_username`: Username for the Raspberry Pi.
+- `--pi_password`: Password for the Raspberry Pi.
+- `--pan_hostname`: Hostname or IP address of the PAN-OS firewall.
+- `--pan_username`: Username for the PAN-OS firewall.
+- `--pan_password_new`: New password to be set for the firewall user.
+- `--pan_password_old`: Current password for the firewall user.
+- `--content_path`: Path on the Raspberry Pi where the content file is located.
+- `--content_version`: Name of the content file to be installed.
+- `--log_level`: Set the log level for the application; options are "DEBUG", "INFO", "WARNING", "ERROR" (default: "INFO").
+
+### Example Commands
+
+Execute with an .env file in the current working directory:
 
 ```bash
-ztp_patcher --hostname <hostname> --username <username> --old-password <old_password> --new-password <new_password> [--pi-hostname <pi_hostname>] [--pi-content-path <pi_content_path>] [--content-file <content_version>]
+ztp_patcher --env_file .env
 ```
 
-- `<hostname>`: The hostname or IP address of the PAN-OS firewall.
-- `<username>`: The username for accessing the PAN-OS firewall.
-- `<old_password>`: The current password for the specified user on the PAN-OS firewall.
-- `<new_password>`: The new password to be set for the specified user on the PAN-OS firewall.
-- `<pi_hostname>` (optional): The hostname or IP address of the Raspberry Pi Zero appliance (default: 192.168.1.2).
-- `<pi_content_path>` (optional): The path on the Raspberry Pi Zero where the content file is located (default: /var/tmp/).
-- `<content_version>` (optional): The name of the content file to be installed on the PAN-OS firewall (default: panupv2-all-contents-8834-8684).
-
-Example:
+Execute by passing all values as arguments instead:
 
 ```bash
-ztp_patcher --hostname 192.168.1.1 --username admin --old-password admin --new-password PaloAlto123!
+ztp_patcher \
+--pi_hostname <pi_hostname> \
+--pi_username <pi_username> \
+--pi_password <pi_password> \
+--pan_hostname <pan_hostname> \
+--pan_username <pan_username> \
+--pan_password_new <new_password> \
+--pan_password_old <old_password> \
+--content_path <content_path> \
+--content_version <content_version> \
+--log_level <log_level>
 ```
 
-The PAN-OS ZTP Patcher will perform the following steps:
+### Operational Steps
 
-1. Change the password of the specified user on the PAN-OS firewall.
-2. Retrieve the API key from the PAN-OS firewall.
-3. Import the content file from the Raspberry Pi Zero to the PAN-OS firewall using SCP.
-4. Initiate the content update installation on the PAN-OS firewall using the API.
-5. Monitor the content update job progress until completion.
+1. Changes the specified user's password on the PAN-OS firewall.
+2. Retrieves the API key using the new credentials.
+3. Imports and installs the content update from the Raspberry Pi using SCP.
+4. Monitors the status of the content update job until completion.
 
-Note: Ensure that the Raspberry Pi Zero is properly connected to the management interface of the PAN-OS firewall and has the necessary network connectivity before running the PAN-OS ZTP Patcher.
+Ensure proper connectivity and configurations are set before initiating the ZTP Patcher.
 
-Please refer to the detailed documentation and examples provided with the PAN-OS ZTP Patcher for more information on its usage and advanced configuration options.
+## Contributing
 
-## License
+Contributions are welcome. Please fork the repository, make your changes, and submit a pull request.
 
-The PAN-OS ZTP Patcher is released under the Apache License 2.0. See the [LICENSE](LICENSE) file for more details.
+## License
 
+This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for more details.
```

