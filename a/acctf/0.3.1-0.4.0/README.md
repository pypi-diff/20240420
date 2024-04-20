# Comparing `tmp/acctf-0.3.1.tar.gz` & `tmp/acctf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acctf-0.3.1.tar", last modified: Sat Apr 13 15:37:07 2024, max compression
+gzip compressed data, was "acctf-0.4.0.tar", last modified: Sat Apr 20 09:31:43 2024, max compression
```

## Comparing `acctf-0.3.1.tar` & `acctf-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.3.1/LICENSE
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-13 15:37:07.767055 acctf-0.3.1/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4021 2024-04-13 14:09:09.000000 acctf-0.3.1/README.md
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      471 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/bank/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      691 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/bank/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/bank/mizuho/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     5593 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/bank/mizuho/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.3.1/acctf/bank/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/bank/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     7958 2024-04-13 15:27:52.000000 acctf-0.3.1/acctf/bank/sbi/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/other/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.3.1/acctf/other/__init__.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/other/wealthnavi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2190 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/other/wealthnavi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.3.1/acctf/other/wealthnavi/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/securities/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      810 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/securities/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.3.1/acctf/securities/model.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/securities/sbi/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3951 2024-04-13 14:09:09.000000 acctf-0.3.1/acctf/securities/sbi/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.3.1/acctf/securities/sbi/utils.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf/utils/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.3.1/acctf/utils/__init__.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.3.1/acctf/utils/format.py
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.3.1/acctf/utils/totp.py
-drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-13 15:37:07.767055 acctf-0.3.1/acctf.egg-info/
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-13 15:37:07.000000 acctf-0.3.1/acctf.egg-info/PKG-INFO
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-04-13 15:37:07.000000 acctf-0.3.1/acctf.egg-info/SOURCES.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-04-13 15:37:07.000000 acctf-0.3.1/acctf.egg-info/dependency_links.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       63 2024-04-13 15:37:07.000000 acctf-0.3.1/acctf.egg-info/requires.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-04-13 15:37:07.000000 acctf-0.3.1/acctf.egg-info/top_level.txt
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-13 15:37:07.767055 acctf-0.3.1/setup.cfg
--rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      929 2024-04-13 15:36:55.000000 acctf-0.3.1/setup.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.833396 acctf-0.4.0/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1071 2024-02-11 09:23:25.000000 acctf-0.4.0/LICENSE
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-20 09:31:43.833396 acctf-0.4.0/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4021 2024-04-13 14:09:09.000000 acctf-0.4.0/README.md
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2671 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/bank/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      729 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/bank/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/bank/mizuho/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     6168 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/bank/mizuho/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     1492 2024-03-17 12:13:43.000000 acctf-0.4.0/acctf/bank/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/bank/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     8763 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/bank/sbi/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/other/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.0/acctf/other/__init__.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/other/wealthnavi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     2158 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/other/wealthnavi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      216 2024-02-11 09:23:25.000000 acctf-0.4.0/acctf/other/wealthnavi/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/securities/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      848 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/securities/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      346 2024-02-11 09:23:25.000000 acctf-0.4.0/acctf/securities/model.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.823396 acctf-0.4.0/acctf/securities/sbi/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     3933 2024-04-20 09:28:03.000000 acctf-0.4.0/acctf/securities/sbi/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      747 2024-02-11 09:23:25.000000 acctf-0.4.0/acctf/securities/sbi/utils.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.833396 acctf-0.4.0/acctf/utils/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        0 2024-02-11 09:23:25.000000 acctf-0.4.0/acctf/utils/__init__.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      105 2024-03-17 12:13:43.000000 acctf-0.4.0/acctf/utils/format.py
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       80 2024-04-06 13:38:11.000000 acctf-0.4.0/acctf/utils/totp.py
+drwxr-xr-x   0 hirano00o  (1000) hirano00o  (1000)        0 2024-04-20 09:31:43.833396 acctf-0.4.0/acctf.egg-info/
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)     4667 2024-04-20 09:31:43.000000 acctf-0.4.0/acctf.egg-info/PKG-INFO
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      573 2024-04-20 09:31:43.000000 acctf-0.4.0/acctf.egg-info/SOURCES.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        1 2024-04-20 09:31:43.000000 acctf-0.4.0/acctf.egg-info/dependency_links.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       63 2024-04-20 09:31:43.000000 acctf-0.4.0/acctf.egg-info/requires.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)        6 2024-04-20 09:31:43.000000 acctf-0.4.0/acctf.egg-info/top_level.txt
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)       74 2024-04-20 09:31:43.833396 acctf-0.4.0/setup.cfg
+-rw-r--r--   0 hirano00o  (1000) hirano00o  (1000)      929 2024-04-20 09:30:52.000000 acctf-0.4.0/setup.py
```

### Comparing `acctf-0.3.1/LICENSE` & `acctf-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acctf-0.3.1/PKG-INFO` & `acctf-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.3.1
+Version: 0.4.0
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.3.1/README.md` & `acctf-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `acctf-0.3.1/acctf/bank/__init__.py` & `acctf-0.4.0/acctf/bank/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from selenium import webdriver
 
 from acctf.bank.model import Transaction, Balance, CurrencyType
 from acctf import Base
 
 
 class Bank(Base, metaclass=ABCMeta):
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
 
     @abstractmethod
     def get_balance(self, account_number: str) -> list[Balance]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_transaction_history(
```

### Comparing `acctf-0.3.1/acctf/bank/mizuho/__init__.py` & `acctf-0.4.0/acctf/bank/mizuho/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,65 +2,71 @@
 from datetime import date, datetime
 from io import StringIO
 
 import pandas as pd
 from bs4 import BeautifulSoup
 from dateutil.relativedelta import relativedelta
 from selenium import webdriver
-from selenium.common import NoSuchElementException
+from selenium.common import NoSuchElementException, TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.select import Select
 
 from acctf.bank import Bank, Balance, Transaction
 from acctf.bank.model import str_to_deposit_type, CurrencyType
 
 
 class Mizuho(Bank, ABC):
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
         self.driver.get('https://web.ib.mizuhobank.co.jp/servlet/LOGBNK0000000B.do')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
-        user_id_elem = self.driver.find_element(By.NAME, 'txbCustNo')
+        user_id_elem = self.find_element(By.NAME, 'txbCustNo')
         user_id_elem.send_keys(user_id)
         self.driver.find_element(By.NAME, 'N00000-next').click()
 
-        user_pw_elem = self.driver.find_element(By.NAME, 'PASSWD_LoginPwdInput')
+        user_pw_elem = self.find_element(By.NAME, 'PASSWD_LoginPwdInput')
         user_pw_elem.send_keys(password)
         self.driver.find_element(By.ID, 'btn_login').click()
 
         try:
-            elem = self.driver.find_element(By.XPATH, '//*[@id="button-section"]/a/img')
-        except NoSuchElementException as e:
+            important_notification = '//*[@id="button-section"]/a/img'
+            elem = self.find_element(By.XPATH, important_notification)
+        except TimeoutException:
             pass
         else:
             elem.click()
 
         return self
 
 
     def logout(self):
         self.driver.find_element(By.XPATH, '//*[@id="side-menu"]/div[1]/a/img').click()
 
 
     def get_balance(self, account_number: str) -> list[Balance]:
-        self.driver.find_element(By.ID, 'MB_R011N030').click()
+        balance = 'MB_R011N030'
+        elem = self.find_element_to_be_clickable(By.ID, balance)
+        elem.click()
         # When there is the account select box
         try:
-            elem = self.driver.find_element(By.CLASS_NAME, 'n03000-t1')
+            select = 'n03000-t1'
+            elem = self.find_element(By.CLASS_NAME, select)
             tr = iter(elem.find_elements(By.TAG_NAME, "tr"))
             # skip header
             next(tr)
             for num, t in enumerate(tr):
                 if t.find_elements(By.TAG_NAME, "span")[2].text == account_number:
                     t.find_element(By.NAME, f"chkAccChkBx_{str(num).zfill(3)}").click()
                     break
             self.driver.find_element(By.XPATH, '//*[@id="main"]/section/input').click()
-        except NoSuchElementException as e:
+        except NoSuchElementException:
+            pass
+        except TimeoutException:
             pass
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find_all("table")
 
         df = pd.read_html(StringIO(str(table)))[0]
@@ -84,39 +90,50 @@
         """Gets the transaction history. If start or end parameter is empty, return the history of current month.
 
         :param account_number: specify an account number.
         :param start: start date of transaction history. After the 1st of the month before the previous month.
         :param end: end date of transaction history. Until today.
         :param currency: currency of transaction history. But this parameter currently doesn't affect.
         """
-        self.driver.find_element(By.ID, 'MB_R011N040').click()
+        transaction = 'MB_R011N040'
+        elem = self.find_element_to_be_clickable(By.ID, transaction)
+        elem.click()
         # When there is the account select box
         try:
-            elem = self.driver.find_element(By.NAME, 'lstAccSel')
+            select_account = 'lstAccSel'
+            elem = self.find_element(By.NAME, select_account)
             select = Select(elem)
             for o in select.options:
                 if o.text.endswith(account_number):
                     select.select_by_value(o.get_attribute("value"))
                     break
-        except NoSuchElementException as e:
+        except NoSuchElementException:
+            pass
+        except TimeoutException:
             pass
 
         if start is not None or end is not None:
             max_date = date.today()
             min_date = date(max_date.year, max_date.month, 1) + relativedelta(months=-2)
             if min_date <= start < end <= max_date:
-                self.driver.find_elements(By.NAME, 'rdoInqMtdSpec')[1].click()
+                period = 'rdoInqMtdSpec'
+                elem = self.find_elements(By.NAME, period)
+                elem[1].click()
                 Select(self.driver.find_element(By.NAME, 'lstDateFrmYear')).select_by_value(str(start.year))
                 Select(self.driver.find_element(By.NAME, 'lstDateFrmMnth')).select_by_value(str(start.month))
                 Select(self.driver.find_element(By.NAME, 'lstDateFrmDay')).select_by_value(str(start.day))
 
                 Select(self.driver.find_element(By.NAME, 'lstDateToYear')).select_by_value(str(end.year))
                 Select(self.driver.find_element(By.NAME, 'lstDateToMnth')).select_by_value(str(end.month))
                 Select(self.driver.find_element(By.NAME, 'lstDateToDay')).select_by_value(str(end.day))
-        self.driver.find_element(By.XPATH, '//*[@id="main"]/section[1]/input').click()
+            else:
+                raise AttributeError(f"date can be set between {min_date} and {max_date}")
+        inquiry_transaction = '//*[@id="main"]/section[1]/input'
+        elem = self.find_element(By.XPATH, inquiry_transaction)
+        elem.click()
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find("table", class_="n04110-t2")
 
         df = pd.read_html(StringIO(str(table)))[0]
         ret: list[Transaction] = []
```

### Comparing `acctf-0.3.1/acctf/bank/model.py` & `acctf-0.4.0/acctf/bank/model.py`

 * *Files identical despite different names*

### Comparing `acctf-0.3.1/acctf/bank/sbi/__init__.py` & `acctf-0.4.0/acctf/bank/sbi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,42 +14,45 @@
 from acctf.utils.format import format_displayed_money
 
 
 class SBI(Bank, ABC):
     account_number = ""
     branch_name = ""
 
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
         self.driver.get('https://www.netbk.co.jp/contents/pages/wpl010101/i010101CT/DI01010210')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
-        user_id_elem = self.driver.find_element(By.ID, 'userNameNewLogin')
+        user_id_elem = self.find_element(By.ID, 'userNameNewLogin')
         user_id_elem.send_keys(user_id)
 
-        user_pw_elem = self.driver.find_element(By.ID, 'loginPwdSet')
+        user_pw_elem = self.find_element(By.ID, 'loginPwdSet')
         user_pw_elem.send_keys(password)
         self.driver.find_element(By.TAG_NAME, 'button').click()
-        time.sleep(5)
         self.driver.set_window_size(1024, 1000)
         self._get_account_info()
 
         return self
 
 
     def logout(self):
         self.driver.find_element(By.CSS_SELECTOR, '.header_logout.ng-star-inserted').click()
 
 
     def get_balance(self, account_number: str) -> list[Balance]:
         if account_number != "" and account_number is not None:
             self.account_number = account_number
 
-        self.driver.find_element(By.CLASS_NAME, 'm-icon-ps_balance').click()
+        balance = 'm-icon-ps_balance'
+        elem = self.find_element_to_be_clickable(By.CLASS_NAME, balance)
+        elem.click()
+
+        self.wait_loading(By.CLASS_NAME, "loadingServer")
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find_all("table")
 
         df = pd.read_html(StringIO(str(table)))
         ret = []
@@ -83,27 +86,34 @@
         :param start: start date of transaction history. After the 1st of the month before the previous month.
         :param end: end date of transaction history. Until today.
         :param currency: currency of transaction history.
         """
         if account_number != "" and account_number is not None:
             self.account_number = account_number
 
-        self.driver.find_element(By.CLASS_NAME, 'm-icon-ps_details').click()
+        details = 'm-icon-ps_details'
+        elem = self.find_element_to_be_clickable(By.CLASS_NAME, details)
+        elem.click()
+
+        self.wait_loading(By.CLASS_NAME, "loadingServer")
 
         # 代表口座
         if currency is None:
             currency = CurrencyType.jpy
 
         df = self._get_transaction(start, end, currency)
         if currency == CurrencyType.jpy:
             # ハイブリッド預金(Only Yen)
-            e = self.driver.find_elements(By.XPATH, '//ng-component/section/div/div[3]/div[1]/div[1]/div[2]/nb-select/div/div[1]')
+            hybrid = '//ng-component/section/div/div[3]/div[1]/div[1]/div[2]/nb-select/div/div[1]'
+            e = self.find_elements(By.XPATH, hybrid)
             if len(e) > 0:
                 e[0].click()
-                self.driver.find_element(By.XPATH, '//*[@id="form3-menu"]/li[2]').click()
+                time.sleep(1)
+                elem = self.find_element(By.XPATH, '//*[@id="form3-menu"]/li[2]')
+                elem.click()
                 df = pd.concat([df, self._get_transaction(start, end)]).sort_values("日付")
 
         ret: list[Transaction] = []
         for d in df.iterrows():
             v: str = ""
             if pd.isnull(d[1].iloc[2]):
                 v = format_displayed_money(d[1].iloc[3])
@@ -133,59 +143,77 @@
         if start is not None:
             max_date = date.today()
             min_date = date(max_date.year-7, 1, 1)
             if end == None:
                 end = max_date
             if min_date <= start < end <= max_date:
                 # 期間指定選択
-                self.driver.find_element(By.XPATH, '//li[5]/label').click()
+                period = '//li[5]/label'
+                elem = self.find_element(By.XPATH, period)
+                elem.click()
+            else:
+                raise AttributeError(f"date can be set between {min_date} and {max_date}")
 
             # 開始日
-            self.driver.find_element(By.XPATH, '//p[1]/nb-simple-select/span/span[2]').click()
-            self.driver.find_element(By.XPATH, f'//li[contains(text(), "{start.year}年")]').click()
-            self.driver.find_element(By.XPATH, '//p[2]/nb-simple-select/span/span[2]').click()
-            self.driver.find_element(By.XPATH, f'//li[contains(text(), "{start.month}月")]').click()
-            self.driver.find_element(By.XPATH, '//p[3]/nb-simple-select/span/span[2]').click()
-            self.driver.find_element(By.XPATH, f'//li[contains(text(), "{start.day}日")]').click()
+            # Sleep until an animation ended
+            self.find_element(By.XPATH, '//p[1]/nb-simple-select/span/span[2]').click()
+            time.sleep(1)
+            self.find_element(By.XPATH, f'//li[contains(text(), "{start.year}年")]').click()
+            self.find_element(By.XPATH, '//p[2]/nb-simple-select/span/span[2]').click()
+            time.sleep(1)
+            self.find_element(By.XPATH, f'//li[contains(text(), "{start.month}月")]').click()
+            self.find_element(By.XPATH, '//p[3]/nb-simple-select/span/span[2]').click()
+            time.sleep(1)
+            self.find_element(By.XPATH, f'//li[contains(text(), "{start.day}日")]').click()
 
             # 終了日
-            self.driver.find_elements(By.XPATH, '//p[1]/nb-simple-select/span/span[2]')[1].click()
-            e = self.driver.find_elements(By.XPATH, f'//li[contains(text(), " {end.year}年 ")]')[1]
+            self.find_elements(By.XPATH, '//p[1]/nb-simple-select/span/span[2]')[1].click()
+            time.sleep(1)
+            e = self.find_elements(By.XPATH, f'//li[contains(text(), " {end.year}年 ")]')[1]
             ActionChains(self.driver).move_to_element(e).perform()
             e.click()
-            self.driver.find_elements(By.XPATH, '//p[2]/nb-simple-select/span/span[2]')[1].click()
-            e = self.driver.find_elements(By.XPATH, f'//li[contains(text(), " {end.month}月 ")]')[1]
+            self.find_elements(By.XPATH, '//p[2]/nb-simple-select/span/span[2]')[1].click()
+            time.sleep(1)
+            e = self.find_elements(By.XPATH, f'//li[contains(text(), " {end.month}月 ")]')[1]
             ActionChains(self.driver).move_to_element(e).perform()
             e.click()
-            self.driver.find_elements(By.XPATH, '//p[3]/nb-simple-select/span/span[2]')[1].click()
-            e = self.driver.find_elements(By.XPATH, f'//li[contains(text(), " {end.day}日 ")]')[1]
+            self.find_elements(By.XPATH, '//p[3]/nb-simple-select/span/span[2]')[1].click()
+            time.sleep(1)
+            e = self.find_elements(By.XPATH, f'//li[contains(text(), " {end.day}日 ")]')[1]
             ActionChains(self.driver).move_to_element(e).perform()
             e.click()
 
         # 通貨選択(代表口座のみ)
-        self.driver.find_elements(By.XPATH, '//nb-select/div/div[1]/span[2]')[1].click()
-        e = self.driver.find_elements(By.XPATH, currency_map[currency])[1]
+        select_currency = '//nb-select/div/div[1]/span[2]'
+        elem = self.find_elements(By.XPATH, select_currency)
+        elem[1].click()
+        e = self.find_elements(By.XPATH, currency_map[currency])[1]
         ActionChains(self.driver).move_to_element(e).perform()
         e.click()
 
         # 表示選択
-        self.driver.find_element(By.CSS_SELECTOR, '.m-btnEm-m.m-btnEffectAnc').click()
+        display = '.m-btnEm-m.m-btnEffectAnc'
+        self.find_element(By.CSS_SELECTOR, display).click()
 
-        continue_button = self.driver.find_elements(By.CSS_SELECTOR, '.m-btn_icon_txt.ng-tns-c3-3.ng-star-inserted')
-        while len(continue_button) > 0:
+        self.wait_loading(By.ID, "loadWrap")
+
+        _continue = '.m-btn_icon_txt.ng-tns-c3-3.ng-star-inserted'
+        continue_button = self.find_elements(By.CSS_SELECTOR, _continue, False)
+        while continue_button is not None:
             continue_button[0].click()
-            continue_button = self.driver.find_elements(By.CSS_SELECTOR, '.m-btn_icon_txt.ng-tns-c3-3.ng-star-inserted')
+            continue_button = self.find_elements(By.CSS_SELECTOR, _continue, False)
+            self.wait_loading(By.CSS_SELECTOR, '.show-loading.ng-tns-c3-3.ng-star-inserted')
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find("table")
 
         return pd.read_html(StringIO(str(table)))[0]
 
     def _get_account_info(self):
-        self.branch_name = self.driver.find_element(
-            By.XPATH,
-            '/html/body/app/div[1]/ng-component/div/main/ng-component/div[1]/div/div/div/div/div/span/span[1]').text
+        branch_name = '/html/body/app/div[1]/ng-component/div/main/ng-component/div[1]/div/div/div/div/div/span/span[1]'
+        elem = self.find_element(By.XPATH, branch_name)
+        self.branch_name = elem.text
 
         self.account_number= self.driver.find_element(
             By.XPATH,
             '/html/body/app/div[1]/ng-component/div/main/ng-component/div[1]/div/div/div/div/div/span/span[3]').text
```

### Comparing `acctf-0.3.1/acctf/other/wealthnavi/__init__.py` & `acctf-0.4.0/acctf/other/wealthnavi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,43 +8,41 @@
 from acctf import Base
 from acctf.other.wealthnavi.model import Asset
 from acctf.utils.format import format_displayed_money
 from acctf.utils.totp import get_code
 
 
 class WealthNavi(Base):
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
         self.driver.get('https://invest.wealthnavi.com/login')
 
     def login(self, user_id: str, password: str, totp: str | None = None):
-        user_id_elem = self.driver.find_element(By.ID, 'username')
+        user_id_elem = self.find_element(By.ID, 'username')
         user_id_elem.send_keys(user_id)
 
         user_pw_elem = self.driver.find_element(By.ID, 'password')
         user_pw_elem.send_keys(password)
 
         self.driver.find_element(By.ID, 'login').click()
 
         if totp is not None:
-            otp_elem = self.driver.find_element(By.ID, 'code')
+            otp_elem = self.find_element(By.ID, 'code')
             otp_elem.send_keys(int(get_code(totp)))
 
             self.driver.find_element(By.ID, 'authentication-code-login').click()
 
-        self.driver.set_window_size(1024, 1000)
-
         return self
 
     def logout(self):
         self.driver.find_element(By.CLASS_NAME, 'logout-submit').click()
 
     def get_valuation(self) -> list[Asset]:
         self.driver.set_window_size(1024, 600)
-        self.driver.find_element(By.PARTIAL_LINK_TEXT, 'ポートフォリオ').click()
+        self.find_element(By.PARTIAL_LINK_TEXT, 'ポートフォリオ').click()
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find("table", id="assets-class-data")
 
         df = pd.read_html(StringIO(str(table)), header=0)[0]
         df = df.iloc[:,0:3]
```

### Comparing `acctf-0.3.1/acctf/securities/__init__.py` & `acctf-0.4.0/acctf/securities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from selenium import webdriver
 
 from acctf import Base
 from acctf.securities.model import Value
 
 
 class Securities(Base, metaclass=ABCMeta):
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
 
     @abstractmethod
     def get_stock_specific(self) -> list[Value]:
         raise NotImplementedError()
 
     @abstractmethod
     def get_stock_specific_us(self) -> list[Value]:
```

### Comparing `acctf-0.3.1/acctf/securities/sbi/__init__.py` & `acctf-0.4.0/acctf/securities/sbi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,52 +12,52 @@
 
 
 class SBI(Securities, ABC):
     _df_fund_specific: pd.DataFrame = None
     _df_fund_nisa_accum: pd.DataFrame = None
     _df_fund_old_nisa_accum: pd.DataFrame = None
 
-    def __init__(self, driver: webdriver = None):
-        super().__init__(driver=driver)
+    def __init__(self, driver: webdriver = None, timeout: float = 30):
+        super().__init__(driver=driver, timeout=timeout)
         self.driver.get('https://www.sbisec.co.jp/ETGate')
 
 
     def login(self, user_id: str, password: str, totp: str | None = None):
-        user_id_elem = self.driver.find_element(By.NAME, 'user_id')
+        user_id_elem = self.find_element(By.NAME, 'user_id')
         user_id_elem.send_keys(user_id)
         user_pw_elem = self.driver.find_element(By.NAME, 'user_password')
         user_pw_elem.send_keys(password)
 
         self.driver.find_element(By.NAME, 'ACT_login').click()
         return self
 
     def logout(self):
         self.driver.find_element(By.XPATH, '//*[@id="logoutM"]/a/img').click()
 
     def get_stock_specific(self) -> list[Value]:
         # 口座管理ページ
-        self.driver.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
+        self.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
         # 株式(現物)タブ
-        self.driver.find_element(By.LINK_TEXT, '株式(現物)').click()
+        self.find_element(By.LINK_TEXT, '株式(現物)').click()
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find_all("table", border="0", cellpadding="1", cellspacing="1", width="400")
 
         df = pd.read_html(StringIO(str(table)), header=0)[0]
         return get_formatted(df, AccountType.jp)
 
 
     def get_stock_specific_us(self) -> list[Value]:
         # 口座管理ページ
-        self.driver.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
+        self.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
         # 口座(外貨建)ページ
-        self.driver.find_element(By.LINK_TEXT, '口座(外貨建)').click()
+        self.find_element(By.LINK_TEXT, '口座(外貨建)').click()
         # 株式（現物）タブ
-        self.driver.find_element(By.LINK_TEXT, '株式（現物）').click()
+        self.find_element(By.LINK_TEXT, '株式（現物）').click()
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find_all("table", border="0", cellpadding="1", cellspacing="1", width="100%")
 
         df = pd.read_html(StringIO(str(table)), header=0)[0]
         return get_formatted(df, AccountType.us)
 
@@ -78,17 +78,17 @@
         if self._df_fund_old_nisa_accum is None:
             self._get_fund_all()
         return get_formatted(self._df_fund_old_nisa_accum, AccountType.jp)
 
 
     def _get_fund_all(self):
         # 口座管理ページ
-        self.driver.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
+        self.find_element(By.XPATH, '//*[@id="link02M"]/ul/li[3]/a/img').click()
         # 投信タブ
-        self.driver.find_element(By.LINK_TEXT, '投信').click()
+        self.find_element(By.LINK_TEXT, '投信').click()
 
         html = self.driver.page_source.encode('utf-8')
         soup = BeautifulSoup(html, 'html.parser')
         table = soup.find_all("table", border="0", cellpadding="1", cellspacing="1", width="400")
 
         df = pd.read_html(StringIO(str(table)), header=0)
         for d in df:
```

### Comparing `acctf-0.3.1/acctf/securities/sbi/utils.py` & `acctf-0.4.0/acctf/securities/sbi/utils.py`

 * *Files identical despite different names*

### Comparing `acctf-0.3.1/acctf.egg-info/PKG-INFO` & `acctf-0.4.0/acctf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acctf
-Version: 0.3.1
+Version: 0.4.0
 Summary: library that scrapes the data from an account such as securities, bank
 Home-page: https://github.com/hirano00o/acctf
 Author: hirano00o
 Keywords: scrape,account,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `acctf-0.3.1/acctf.egg-info/SOURCES.txt` & `acctf-0.4.0/acctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acctf-0.3.1/setup.py` & `acctf-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="acctf",
-    version="0.3.1",
+    version="0.4.0",
     description="library that scrapes the data from an account such as securities, bank",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hirano00o/acctf",
     author="hirano00o",
     classifiers=[
         "Programming Language :: Python :: 3",
```

