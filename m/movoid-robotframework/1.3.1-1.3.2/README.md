# Comparing `tmp/movoid_robotframework-1.3.1.tar.gz` & `tmp/movoid_robotframework-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.3.1.tar", last modified: Tue Mar 26 13:02:52 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.3.2.tar", last modified: Sat Apr 20 15:08:25 2024, max compression
```

## Comparing `movoid_robotframework-1.3.1.tar` & `movoid_robotframework-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 13:02:52.071550 movoid_robotframework-1.3.1/
--rw-rw-rw-   0        0        0      282 2024-03-26 13:02:52.070508 movoid_robotframework-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 13:02:52.057855 movoid_robotframework-1.3.1/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:02:52.060934 movoid_robotframework-1.3.1/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      220 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:25:58.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14416 2024-03-26 13:02:31.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      260 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.1/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:02:52.069508 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      282 2024-03-26 13:02:52.000000 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-03-26 13:02:52.000000 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 13:02:52.000000 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-03-26 13:02:52.000000 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-26 13:02:52.000000 movoid_robotframework-1.3.1/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 13:02:52.072572 movoid_robotframework-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      550 2024-03-26 13:02:31.000000 movoid_robotframework-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.146665 movoid_robotframework-1.3.2/
+-rw-rw-rw-   0        0        0      282 2024-04-20 15:08:25.145658 movoid_robotframework-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.136682 movoid_robotframework-1.3.2/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.139284 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      220 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     3715 2024-02-20 09:25:58.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      260 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.144652 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:08:25.146665 movoid_robotframework-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      550 2024-04-20 15:07:13.000000 movoid_robotframework-1.3.2/setup.py
```

### Comparing `movoid_robotframework-1.3.1/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.3.2/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.1/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.3.2/RobotFrameworkBasic/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.1/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.3.2/RobotFrameworkBasic/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,53 +99,50 @@
 else:
     def _robot_log_keyword(func):
         return func
 
 robot_log_keyword = _robot_log_keyword
 
 
-def do_until_check(do_function, check_function, timeout=30, init_check=True, init_check_function=None, init_sleep=0, wait_before_check=0, do_interval=1, check_timeout=1, check_interval=0.2, error=True):
+def do_until_check(do_function, check_function, timeout=30, init_check=True, init_check_function=None, init_sleep=0, wait_before_check=0, do_interval=1, check_interval=0.2, error=True):
     """
     通过操作某个函数，达成某个最终的目的。如果检查未通过，那么会循环进行操作
     这是一个装饰器，需要套在一个空函数上（仅函数名会被继承）
         当然了，你也可以套在一个有价值的函数上，但是这个函数的所有痕迹都会被抹除
     :param do_function:主动操作的函数，传入函数，不需要返回值
     :param check_function:检查函数，返回值必须是一个bool值，或者返回值会被强制转换为bool
     :param timeout:最大时常/超时。检查超过这个时常后，会认为操作失败.
     :param init_check:是否进行初始检查，如果为True，那么会在操作前进行检查，如果通过，那么会跳过操作，直接结束
     :param init_check_function:初始检查函数，返回值必须是一个bool值，或者返回值会被强制转换为bool，如果存在。那么初始检查会考虑使用这个。这个函数的参数必须和check_function完全一致，否则会报错
     :param init_sleep:初始的等待时间，在初始检查前进行的等待，不计入整体timeout时间，一般配合初始检查init_check=True使用
     :param wait_before_check:在常规检查前的等待时间，一般是和上一次的操作存在一定的等待时间，保证上次的操作可以真实地
     :param do_interval:两次操作之间地最小间隔。一般是检查结束后，到操作之前的时间。主要是为了保证不要进行太多次的循环
-    :param check_timeout:检查的超时时间，如果想要进行更多次的检查可以设置这个数值
     :param check_interval:连续两次检查之间的时间间隔，默认值为1，如果想要进行更细致的循环检查，可以将这个数值设置得更小
     :param error:当检查失败后，是否raise一个error。默认为True，会raise。
     :return: 返回是否判定成功，但是当error=True时，失败了会raise AssertionError，那也就不会有返回值了
     """
     _timeout = 30 if timeout is None else float(timeout)  # type:float
     _init_check = True if init_check is None else bool(init_check)  # type:bool
     init_check_function = check_function if init_check_function is None else init_check_function
     _init_sleep = 0 if init_sleep is None else float(init_sleep)  # type:float
     _wait_before_check = 1 if wait_before_check is None else float(wait_before_check)  # type:float
     _do_interval = 1 if do_interval is None else float(do_interval)  # type:float
-    _check_timeout = 0 if check_timeout is None else float(check_timeout)  # type:float
     _check_interval = 0.2 if check_interval is None else float(check_interval)  # type:float
     _error = True if error is None else bool(error)  # type:bool
 
     def dec(func):
         @wraps_func(func, do_function, check_function)
         def wrapper(self,
                     do_kwargs,
                     check_kwargs,
                     timeout=_timeout,  # noqa
                     init_check=_init_check,  # noqa
                     init_sleep=_init_sleep,  # noqa
                     wait_before_check=_wait_before_check,  # noqa
                     do_interval=_do_interval,  # noqa
-                    check_timeout=_check_timeout,  # noqa
                     check_interval=_check_interval,  # noqa
                     error=_error):  # noqa
             fail_print = []
             do_text = f'do {do_function.__name__}{do_kwargs}'
             check_text = f'check {check_function.__name__}{check_kwargs}'
             if init_check:
                 try:
@@ -173,15 +170,15 @@
                     print_text = '{:.3f} second {} time {} error:{}'.format(time.time() - start_time_point, loop_time, do_text, err)
                     self.print(print_text)
                     fail_print.append(print_text + '\n' + traceback.format_exc())
                 time.sleep(wait_before_check)
                 check_time = 0
                 check_time_point = time.time()
                 check_loop_time = 0
-                while check_time < check_timeout:
+                while check_time < do_interval:
                     check_interval_time_point = time.time()
                     check_loop_time += 1
                     try:
                         check_bool = check_function(**check_kwargs)
                         if check_bool:
                             self.print('{:.3f}/{:.3f} second {}-{} time {} pass.do until check end.'.format(time.time() - start_time_point, time.time() - check_time_point, loop_time, check_loop_time, check_text))
                             return True
```

### Comparing `movoid_robotframework-1.3.1/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.3.2/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.1/setup.py` & `movoid_robotframework-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.3.1',
+    version='1.3.2',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

