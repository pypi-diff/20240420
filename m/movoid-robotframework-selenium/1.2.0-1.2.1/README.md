# Comparing `tmp/movoid_robotframework_selenium-1.2.0.tar.gz` & `tmp/movoid_robotframework_selenium-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_selenium-1.2.0.tar", last modified: Sun Mar 24 16:34:57 2024, max compression
+gzip compressed data, was "movoid_robotframework_selenium-1.2.1.tar", last modified: Sat Apr 20 10:57:17 2024, max compression
```

## Comparing `movoid_robotframework_selenium-1.2.0.tar` & `movoid_robotframework_selenium-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 16:34:57.834309 movoid_robotframework_selenium-1.2.0/
--rw-rw-rw-   0        0        0      439 2024-03-24 16:34:57.832242 movoid_robotframework_selenium-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 16:34:57.818972 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/
--rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:34:57.823038 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/
--rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/__init__.py
--rw-rw-rw-   0        0        0    10277 2024-03-24 16:15:24.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/action.py
--rw-rw-rw-   0        0        0     4671 2024-03-24 16:15:28.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/action.pyi
--rw-rw-rw-   0        0        0     7367 2024-03-24 16:01:08.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/common.py
--rw-rw-rw-   0        0        0     2530 2024-03-24 16:01:09.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/common.pyi
--rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/main.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:34:57.831054 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/
--rw-rw-rw-   0        0        0      439 2024-03-24 16:34:57.000000 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2024-03-24 16:34:57.000000 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 16:34:57.000000 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-03-24 16:34:57.000000 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-03-24 16:34:57.000000 movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 16:34:57.834309 movoid_robotframework_selenium-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-03-24 16:31:22.000000 movoid_robotframework_selenium-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:17.033418 movoid_robotframework_selenium-1.2.1/
+-rw-rw-rw-   0        0        0      439 2024-04-20 10:57:17.032421 movoid_robotframework_selenium-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_selenium-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:17.013913 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/
+-rw-rw-rw-   0        0        0      311 2024-02-20 17:47:42.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:17.016903 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/
+-rw-rw-rw-   0        0        0      218 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/__init__.py
+-rw-rw-rw-   0        0        0    12876 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/action.py
+-rw-rw-rw-   0        0        0     6600 2024-04-20 10:54:01.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/action.pyi
+-rw-rw-rw-   0        0        0     7367 2024-03-24 16:01:08.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/common.py
+-rw-rw-rw-   0        0        0     2530 2024-03-24 16:01:09.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/common.pyi
+-rw-rw-rw-   0        0        0      268 2024-02-20 05:59:20.000000 movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 10:57:17.031424 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/
+-rw-rw-rw-   0        0        0      439 2024-04-20 10:57:16.000000 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2024-04-20 10:57:17.000000 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 10:57:16.000000 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-20 10:57:16.000000 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-20 10:57:16.000000 movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 10:57:17.034414 movoid_robotframework_selenium-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      748 2024-04-20 10:51:34.000000 movoid_robotframework_selenium-1.2.1/setup.py
```

### Comparing `movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/action.py` & `movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/action.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,37 +9,44 @@
 
 import os
 import pathlib
 import re
 import time
 from typing import List, Union
 
-from movoid_function import reset_function_default_value
+import cv2
 from RobotFrameworkBasic import robot_log_keyword, do_until_check, do_when_error, RfError
+from movoid_function import reset_function_default_value
+from movoid_package import importing
 from selenium.webdriver import Keys
 from selenium.webdriver.remote.webelement import WebElement
 
-from movoid_package import importing
-
 BasicCommon = importing('..common', 'BasicCommon')
 
 
 class SeleniumAction(BasicCommon):
     def __init__(self):
         super().__init__()
         self._check_element_attribute_change_value: Union[str, None] = None
+        self._check_element_count_value: Union[int, None] = None
 
     def selenium_take_full_screenshot(self, screenshot_name='python-screenshot.png'):
         return self.selenium_take_screenshot(image_name=screenshot_name)
 
     def selenium_click_element(self, click_locator, operate='click'):
         self.selenium_click_element_with_offset(click_locator, 0, 0, operate)
         return True
 
     @robot_log_keyword
+    def selenium_get_element_color_list(self, screenshot_locator=None, image_name='catch-image-color.png', rename=True):
+        tar_name, tar_path = self.selenium_take_screenshot(screenshot_locator, image_name, rename)
+        self.print(f'try to read image:{tar_path}')
+        return cv2.imread(tar_path)
+
+    @robot_log_keyword
     def selenium_click_element_with_offset(self, click_locator, x=0, y=0, operate='click'):
         tar_element = self.selenium_analyse_element(click_locator)
         self.action_chains.move_to_element_with_offset(tar_element, x, y)
         if operate == 'click':
             self.action_chains.click()
         elif operate in ('double_click', 'doubleclick'):
             self.action_chains.double_click()
@@ -153,39 +160,68 @@
         check_count = int(check_count)
         find_elements = self.selenium_find_elements_by_locator(check_locator)
         find_elements_num = len(find_elements)
         self.print(f'we find {find_elements_num}→{check_count} {check_locator}')
         return find_elements_num == check_count
 
     @robot_log_keyword
-    def selenium_check_element_attribute_change_init(self, check_locator, check_attribute=''):
+    def selenium_check_element_attribute_change_init(self, check_locator, check_attribute='innerText'):
         tar_element = self.selenium_find_element_by_locator(check_locator)
         self._check_element_attribute_change_value = tar_element.get_attribute(check_attribute)
         self.print(f'we find {check_attribute} of {check_locator} is {self._check_element_attribute_change_value}')
         return False
 
     @robot_log_keyword
-    def selenium_check_element_attribute_change_loop(self, check_locator, check_attribute=''):
+    def selenium_check_element_attribute_change_loop(self, check_locator, check_attribute='innerText'):
         tar_element = self.selenium_find_element_by_locator(check_locator)
         temp_value = tar_element.get_attribute(check_attribute)
-        re_bool = self._check_element_attribute_change_value == temp_value
-        self.print(f'we find {check_attribute} of {check_locator} is {temp_value}{"==" if re_bool else "!="}{self._check_element_attribute_change_value}')
+        re_bool = self._check_element_attribute_change_value != temp_value
+        self.print(f'we find {check_attribute} of {check_locator} is {temp_value}{"!=" if re_bool else "=="}{self._check_element_attribute_change_value}')
+        return re_bool
+
+    @robot_log_keyword
+    def selenium_check_element_count_change_init(self, check_locator):
+        self._check_element_count_value = len(self.selenium_find_elements_by_locator(check_locator))
+        self.print(f'we find {check_locator} count of {self._check_element_count_value}')
+        return False
+
+    @robot_log_keyword
+    def selenium_check_element_count_change_loop(self, check_locator):
+        now_count = len(self.selenium_find_elements_by_locator(check_locator))
+        re_bool = now_count != self._check_element_count_value
+        self.print(f'we find {check_locator} count of {now_count} {"!=" if re_bool else "=="}{self._check_element_count_value}')
         return re_bool
 
     def always_true(self):
         return True
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
     @do_until_check(always_true, selenium_click_element_with_offset)
     def selenium_click_until_available(self):
         pass
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
+    @do_until_check(always_true, selenium_check_contain_element)
+    def selenium_wait_until_find_element(self):
+        pass
+
+    @reset_function_default_value(selenium_wait_until_find_element)
+    def selenium_wait_until_not_find_element(self, check_exist=False):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @do_until_check(always_true, selenium_check_contain_elements)
+    def selenium_click_until_find_elements(self):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
     @do_until_check(selenium_click_element_with_offset, selenium_check_contain_element)
     def selenium_click_until_find_element(self):
         pass
 
     @reset_function_default_value(selenium_click_until_find_element)
     def selenium_click_until_not_find_element(self, check_exist=False):
         pass
@@ -194,22 +230,40 @@
     @do_when_error(selenium_take_full_screenshot)
     @do_until_check(selenium_click_element_with_offset, selenium_check_contain_elements)
     def selenium_click_until_find_elements(self):
         pass
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
+    @do_until_check(always_true, selenium_find_element_with_attribute)
+    def selenium_wait_until_find_element_attribute(self):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
     @do_until_check(selenium_click_element_with_offset, selenium_find_element_with_attribute)
     def selenium_click_until_find_element_attribute(self):
         pass
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
-    @do_until_check(always_true, selenium_find_element_with_attribute)
-    def selenium_wait_until_find_element_attribute(self):
+    @do_until_check(always_true, selenium_check_element_attribute_change_loop, init_check_function=selenium_check_element_attribute_change_init)
+    def selenium_wait_until_attribute_change(self):
         pass
 
     @robot_log_keyword
     @do_when_error(selenium_take_full_screenshot)
     @do_until_check(selenium_click_element_with_offset, selenium_check_element_attribute_change_loop, init_check_function=selenium_check_element_attribute_change_init)
     def selenium_click_until_attribute_change(self):
         pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @do_until_check(always_true, selenium_check_element_count_change_loop, init_check_function=selenium_check_element_count_change_init)
+    def selenium_wait_until_element_count_change(self):
+        pass
+
+    @robot_log_keyword
+    @do_when_error(selenium_take_full_screenshot)
+    @do_until_check(selenium_click_element_with_offset, selenium_check_element_count_change_loop, init_check_function=selenium_check_element_count_change_init)
+    def selenium_click_until_element_count_change(self):
+        pass
```

### Comparing `movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/action/action.pyi` & `movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/action/action.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 # This is auto generated by code.
 ##################################################
 
 import os
 import pathlib
 import re
 import time
+import cv2
 import typing
 from ..common import BasicCommon
 
 class SeleniumAction(BasicCommon):
 	def __init__(self):
 		super().__init__()
 		self._check_element_attribute_change_value: typing.Union[str, None] =  None
+		self._check_element_count_value: typing.Union[int, None] =  None
 	def selenium_take_full_screenshot(self, screenshot_name = 'python-screenshot.png'):	...
 	def selenium_click_element(self, click_locator, operate = 'click'):	...
+	def selenium_get_element_color_list(self, screenshot_locator = None, image_name = 'catch-image-color.png', rename = True):	...
 	def selenium_click_element_with_offset(self, click_locator, x = 0, y = 0, operate = 'click'):	...
 	def selenium_check_element_attribute(self, check_locator, check_attribute = 'innerText', check_value = '', regex = True, check_bool = True):
 		"""
 		检查所有元素中，是否存在一个属性满足要求的元素
 		:param check_locator: 元素定位
 		:param check_attribute: 属性名
 		:param check_value: 属性值
@@ -31,40 +34,62 @@
 	def selenium_find_element_with_attribute(self, find_locator, find_value = '', find_attribute = 'innerText', regex = True, check_bool = True):	...
 	def selenium_get_locator_attribute(self, target_locator, target_attribute = 'innerText'):	...
 	def selenium_new_screenshot_folder(self):	...
 	def selenium_delete_elements(self, delete_locator):	...
 	def selenium_input_delete_all_and_input(self, input_locator, input_text):	...
 	def selenium_check_contain_element(self, check_locator, check_exist = True):	...
 	def selenium_check_contain_elements(self, check_locator, check_count = 1):	...
-	def selenium_check_element_attribute_change_init(self, check_locator, check_attribute = ''):	...
-	def selenium_check_element_attribute_change_loop(self, check_locator, check_attribute = ''):	...
+	def selenium_check_element_attribute_change_init(self, check_locator, check_attribute = 'innerText'):	...
+	def selenium_check_element_attribute_change_loop(self, check_locator, check_attribute = 'innerText'):	...
+	def selenium_check_element_count_change_init(self, check_locator):	...
+	def selenium_check_element_count_change_loop(self, check_locator):	...
 	def always_true(self):	...
-	def selenium_click_until_available(self, click_locator, x = 0, y = 0, operate = 'click', screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_click_until_available(self, click_locator, x = 0, y = 0, operate = 'click', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_click_until_find_element(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_exist = True, screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_wait_until_find_element(self, check_locator, check_exist = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_click_until_not_find_element(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_exist = False, screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_wait_until_not_find_element(self, check_locator, check_exist = False, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_click_until_find_elements(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_count = 1, screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_click_until_find_elements(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_count = 1, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_click_until_find_element_attribute(self, click_locator, find_locator, x = 0, y = 0, operate = 'click', find_value = '', find_attribute = 'innerText', regex = True, check_bool = True, screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_click_until_find_element(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_exist = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_wait_until_find_element_attribute(self, find_locator, find_value = '', find_attribute = 'innerText', regex = True, check_bool = True, screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_click_until_not_find_element(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_exist = False, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
-	def selenium_click_until_attribute_change(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_attribute = '', screenshot_name = 'python-screenshot.png', timeout = 5.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+	def selenium_wait_until_find_element_attribute(self, find_locator, find_value = '', find_attribute = 'innerText', regex = True, check_bool = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_click_until_find_element_attribute(self, click_locator, find_locator, x = 0, y = 0, operate = 'click', find_value = '', find_attribute = 'innerText', regex = True, check_bool = True, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_attribute_change(self, check_locator, check_attribute = 'innerText', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_click_until_attribute_change(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', check_attribute = 'innerText', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_wait_until_element_count_change(self, check_locator, screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
+		"""
+		"""
+		...
+	def selenium_click_until_element_count_change(self, click_locator, check_locator, x = 0, y = 0, operate = 'click', screenshot_name = 'python-screenshot.png', timeout = 30.0, init_check = True, init_sleep = 0.0, wait_before_check = 0.0, do_interval = 1.0, check_timeout = 1.0, check_interval = 0.2, error = True):
 		"""
 		"""
 		...
 	...
```

### Comparing `movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/common.py` & `movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.0/RobotFrameworkSelenium/common.pyi` & `movoid_robotframework_selenium-1.2.1/RobotFrameworkSelenium/common.pyi`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.0/movoid_robotframework_selenium.egg-info/SOURCES.txt` & `movoid_robotframework_selenium-1.2.1/movoid_robotframework_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework_selenium-1.2.0/setup.py` & `movoid_robotframework_selenium-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_selenium',
-    version='1.2.0',
+    version='1.2.1',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

