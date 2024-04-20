# Comparing `tmp/pyuptech-0.1.2.tar.gz` & `tmp/pyuptech-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.2.tar", last modified: Thu Apr 18 11:06:03 2024, max compression
+gzip compressed data, was "pyuptech-0.1.3.tar", last modified: Sat Apr 20 11:58:25 2024, max compression
```

## Comparing `pyuptech-0.1.2.tar` & `pyuptech-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5865 2024-04-18 11:05:42.276506 pyuptech-0.1.2/README.md
--rw-r--r--   0        0        0      430 2024-04-18 11:06:03.152718 pyuptech-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      865 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/__init__.py
--rw-r--r--   0        0        0       35 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1007 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1659 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0     8701 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0        0 2024-04-18 11:05:42.276506 pyuptech-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-18 11:05:42.276506 pyuptech-0.1.2/tests/perf_tests.py
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 pyuptech-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-20 11:58:02.460636 pyuptech-0.1.3/README.md
+-rw-r--r--   0        0        0      460 2024-04-20 11:58:25.724696 pyuptech-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1095 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1096 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1659 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0     9833 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     4912 2024-04-20 11:58:02.460636 pyuptech-0.1.3/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0        0 2024-04-20 11:58:02.460636 pyuptech-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-20 11:58:02.460636 pyuptech-0.1.3/tests/perf_tests.py
+-rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 pyuptech-0.1.3/PKG-INFO
```

### Comparing `pyuptech-0.1.2/README.md` & `pyuptech-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # pyuptech
 
 > 一个API包装库，通过调用TechStar的二进制so库完成的功能
 ---
 
+# 安装
+
+使用`pdm`安装
+
+```shell
+pdm add pyuptech
+```
+
 ## OnBoardSensors
 
 **简介**
 
 `OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
 
 ### 类方法概览
@@ -35,32 +43,34 @@
 - 限制ADC采样频率，防止过采样。
 - 获取ADC和GPIO的数据。
 - 初始化和读取MPU6500六轴传感器数据。
 
 ### QUICKSTART
 
 ```python
-from pyuptech import OnBoardSensors, OUTPUT, LOW
+from pyuptech import OnBoardSensors
+from ctypes import c_uint8, Array
 
-# 创建OnBoardSensors对象
-sensor_controller = OnBoardSensors()
+# 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
+sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
-# 设置ADC最小采样间隔为10ms
+# 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
-gpio_levels = sensor_controller.io_all_channels()
+gpio_levels: c_uint8 = sensor_controller.io_all_channels()
+print(gpio_levels)
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
-acceleration_data = sensor_controller.acc_all()
+acceleration_data: Array = sensor_controller.acc_all()
 
 # 设置第3号GPIO引脚为输出并设置电平为低
-sensor_controller.set_io_mode(2, OUTPUT)
-sensor_controller.set_io_level(2, LOW)
+sensor_controller.set_io_mode(2, 1)
+sensor_controller.set_io_level(2, 0)
 ```
 
 ---
 
 # Screen
 
 本模块定义了一个名为 `Screen`
@@ -156,8 +166,57 @@
 """
 
 set_log_level(50)  # 将日志等级设为50，此时logger只会记录优先级高于CRITICAL级别的消息
 
 from logging import CRITICAL
 
 set_log_level(CRITICAL)  # 上述代码与上面设置效果一致，即只记录CRITICAL及其以上级别的日志信息
-```
+```
+
+---
+
+## 调试
+
+通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
+
+```python
+from pyuptech import (
+    mpu_display_on_lcd,
+    mpu_display_on_console,
+    adc_io_display_on_lcd,
+    adc_io_display_on_console)
+
+mpu_display_on_console()  # 将MPU6500数据打印到终端
+
+mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
+
+# 定义ADC标签索引字典，可以空缺部分键值
+adc_labels = {
+    6: 'EDGE_FL',
+    7: "EDGE_RL",
+    2: 'EDGE_FR',
+    1: 'EDGE_RR',
+    8: 'L1',
+    0: 'R1',
+    3: 'FB', 5: 'RB',
+    4: 'GRAY'
+}
+# 定义IO标签索引字典,可以空缺部分键值
+io_labels = {
+    3: "gray l",
+    2: "gray r",
+
+    7: 'ftl',
+    6: 'ftr',
+    5: 'rtr'
+}
+
+adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
+
+adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+
+
+
+
+```
+
+
```

### Comparing `pyuptech-0.1.2/src/pyuptech/__init__.py` & `pyuptech-0.1.3/src/pyuptech/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-from .modules.loader import load_lib
+from .modules.loader import load_lib, TECHSTAR_LIB
 from .modules.logger import set_log_level
 from .modules.pins import (
     pin_setter_constructor,
     pin_getter_constructor,
     pin_mode_setter_constructor,
     multiple_pin_mode_setter_constructor,
     PinGetter,
     PinSetter,
     PinModeSetter,
     IndexedGetter,
     IndexedSetter,
 )
 from .modules.screen import Screen, Color, FontSize
-from .modules.sensors import OnBoardSensors, HIGH, LOW, INPUT, OUTPUT
+from .modules.sensors import OnBoardSensors
+
+from .tools.display import (
+    adc_io_display_on_lcd,
+    adc_io_display_on_console,
+    mpu_display_on_lcd,
+    mpu_display_on_console,
+)
 
 __all__ = [
     "OnBoardSensors",
     "Screen",
     "Color",
     "FontSize",
+    "TECHSTAR_LIB",
     "load_lib",
     "set_log_level",
     "pin_getter_constructor",
     "pin_setter_constructor",
     "multiple_pin_mode_setter_constructor",
     "pin_mode_setter_constructor",
     # typing
-    "HIGH",
-    "LOW",
-    "INPUT",
-    "OUTPUT",
     "PinGetter",
     "PinSetter",
     "PinModeSetter",
     "IndexedGetter",
     "IndexedSetter",
+    # tools
+    "adc_io_display_on_lcd",
+    "adc_io_display_on_console",
+    "mpu_display_on_lcd",
+    "mpu_display_on_console",
 ]
```

### Comparing `pyuptech-0.1.2/src/pyuptech/modules/loader.py` & `pyuptech-0.1.3/src/pyuptech/modules/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ctypes
 from functools import lru_cache
 
+from .constant import LIB_FILE_PATH
 from .logger import _logger
 
 
 @lru_cache(maxsize=None)
 def load_lib(lib_file_path: str) -> ctypes.CDLL | None:
     """
     Load a dynamic library from the given file path and return a ctypes.CDLL object.
@@ -28,9 +29,11 @@
     except Exception as e:
         _logger.critical(f"Can't load lib [{lib_file_path}],{e}")
         return None
     _logger.info(f"Lib [{lib_file_path}] loaded")
     return obj
 
 
+TECHSTAR_LIB: ctypes.CDLL = load_lib(LIB_FILE_PATH)
+
 if __name__ == "__main__":
     pass
```

### Comparing `pyuptech-0.1.2/src/pyuptech/modules/logger.py` & `pyuptech-0.1.3/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.2/src/pyuptech/modules/pins.py` & `pyuptech-0.1.3/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.2/src/pyuptech/modules/screen.py` & `pyuptech-0.1.3/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.2/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.3/src/pyuptech/modules/sensors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 import ctypes
 from time import perf_counter_ns
-from typing import Self
+from typing import Self, Literal, Any
 
-from .constant import LIB_FILE_PATH
-from .loader import _logger
-from .loader import load_lib
+from .loader import TECHSTAR_LIB
+from .logger import _logger
 
 E6 = 1000000
 
+"""
 OUTPUT = 1
 INPUT = 0
 HIGH = 1
 LOW = 0
+"""
 
 
 class OnBoardSensors:
     """
     provides sealed methods accessing to the IOs and builtin sensors
     """
 
-    __lib = load_lib(LIB_FILE_PATH)
-
     __adc_data_list_type = ctypes.c_uint16 * 10
     __mpu_data_list_type = ctypes.c_float * 3
-    _adc_all = __adc_data_list_type()
-    _accel_all = __mpu_data_list_type()
-    _gyro_all = __mpu_data_list_type()
-    _atti_all = __mpu_data_list_type()
-
-    last_update_timestamp = perf_counter_ns()
-    __adc_min_sample_interval_ns = 5 * E6
 
-    def __init__(self):
+    def __init__(self, adc_min_sample_interval_ms: int = 5):
 
         success = self.adc_io_open()
-        self.set_all_io_mode(INPUT)
-        self.set_all_io_level(HIGH)
+        self.set_all_io_mode(0)
+        self.set_all_io_level(1)
+        self._adc_all: ctypes.Array = self.__adc_data_list_type()
+        self._accel_all: ctypes.Array = self.__mpu_data_list_type()
+        self._gyro_all: ctypes.Array = self.__mpu_data_list_type()
+        self._atti_all: ctypes.Array = self.__mpu_data_list_type()
+
+        self.__adc_last_sample_timestamp: int = perf_counter_ns()
+
+        self.__adc_min_sample_interval_ns: int = adc_min_sample_interval_ms * E6
         _logger.debug(f"Sensor channel have inited [{success}] times")
 
     @property
+    def last_sample_timestamp_ms(self) -> int:
+        return int(self.__adc_last_sample_timestamp / E6)
+
+    @property
     def adc_min_sample_interval_ms(self) -> int:
         """
         get the minimum interval between two consecutive samples, this is to prevent
         over-sampling, the value is in milliseconds。
 
         NOTE:
             the value is in milliseconds, but the unit is nanoseconds.
@@ -50,245 +54,257 @@
         """
         return int(self.__adc_min_sample_interval_ns / E6)
 
     @adc_min_sample_interval_ms.setter
     def adc_min_sample_interval_ms(self, value: int):
         self.__adc_min_sample_interval_ns = value * E6
 
-    @staticmethod
-    def adc_io_open():
+    def adc_io_open(self) -> Self:
         """
         open the adc-io plug
         """
         _logger.info("Initializing ADC-IO")
-        return OnBoardSensors.__lib.adc_io_open()
+        if TECHSTAR_LIB.adc_io_open():
+            _logger.error("Failed to open ADC-IO")
+        return self
 
-    @staticmethod
-    def adc_io_close():
+    def adc_io_close(self) -> Self:
         """
         close the adc-io plug
         """
         _logger.info("Closing ADC-IO")
-        OnBoardSensors.__lib.adc_io_close()
+        if TECHSTAR_LIB.adc_io_close():
+            _logger.error("Failed to close ADC-IO")
+        return self
 
-    @staticmethod
-    def adc_all_channels():
+    def adc_all_channels(self) -> ctypes.Array:
         """
-        这个函数的功能是从ADC（模拟到数字转换器）获取多个值，
-        并将这些值存储到指定的内存位置。它通过spi_xfer函数调用来与ADC进行通信，并将获取的结果转换为16位整数，
-        并存储到指定内存位置。函数的返回值为0表示操作成功，-1表示操作失败。
-
-        int __fastcall ADC_GetAll(int a1)
-        {
-          char *v2;        // 声明一个指向字符的指针v2
-          int v3;          // 声明一个整型变量v3
-          __int16 v4;      // 声明一个16位整型变量v4
-          __int16 v5;      // 声明一个16位整型变量v5
-          char v7;         // 声明一个字符变量v7，该变量会被按引用传递
-
-          if (pi_1 < 0)    // 检查一个全局变量pi_1是否小于0，如果是，则返回-1
-            return -1;
-
-          spi_xfer(pi_1);  // 调用spi_xfer函数，传递pi_1作为参数
-
-          v2 = &v7;        // 将v2指向变量v7的地址
-          v3 = a1 - 2;     // 将v3设置为a1减去2，表示指定内存位置的偏移量
-
-          do
-          {
-            v4 = (unsigned __int8)v2[2];        // 将v2[2]转换为8位无符号整型并赋值给v4
-            v5 = (unsigned __int8)v2[1];        // 将v2[1]转换为8位无符号整型并赋值给v5
-            v2 += 2;                            // 增加v2的偏移量
-            *(_WORD *)(v3 + 2) = v5 | (v4 << 8); // 将v5和v4的组合结果存储到指定内存位置
-            v3 += 2;                            // 增加v3的偏移量
-          }
-          while (a1 + 18 != v3);                 // 当a1和v3的和不等于18时循环
-
-          return 0;                             // 返回0表示操作成功
-        }
-        """
-        current = perf_counter_ns()
-        samp_interval = OnBoardSensors.__adc_min_sample_interval_ns
-        if current - OnBoardSensors.last_update_timestamp < samp_interval:
-            OnBoardSensors.last_update_timestamp = current
-            return OnBoardSensors.acc_all
-        OnBoardSensors.__lib.ADC_GetAll(OnBoardSensors._adc_all)
-
-        return OnBoardSensors._adc_all
-
-    def set_io_level(self, index: int, level: int) -> Self:
-        """
-        int __fastcall adc_io_Set(unsigned int a1, char a2)
-        {
-          char v3[12]; // [sp+4h] [bp-Ch] BYREF
-
-          if ( a1 > 7 )
-            return -1;
-          v3[0] = a1 + 24;
-          v3[1] = a2;
-          if ( pi_1 < 0 )
-            return -1;
-          spi_write(pi_1, hspi1, v3, 2);
-          return 0;
-        }
+        Get all the ADC channels. Length = 10
+
+        Returns:
+            ctypes.Array: An array containing the values of all the ADC channels.
         """
-        OnBoardSensors.__lib.adc_io_Set(index, level)
+
+        can_update_time = (
+            self.__adc_last_sample_timestamp + self.__adc_min_sample_interval_ns
+        )
+        if can_update_time > (current := perf_counter_ns()):
+
+            return self._adc_all
+        self.__adc_last_sample_timestamp = current
+        if TECHSTAR_LIB.ADC_GetAll(self._adc_all):
+            _logger.error("Failed to get all ADC channels")
+        return self._adc_all
+
+    def set_io_level(self, index: int, level: Literal[0, 1]) -> Self:
+        """
+        Set the level of the specified IO index.
+
+        Args:
+            index (int): The index of the IO.
+            level (Literal[0, 1]): The level to set.
+
+        Returns:
+            Self: The instance of the class.
+
+        Raises:
+            None
+
+        Description:
+            This function sets the level of the specified IO index using the `adc_io_Set` method from the `OnBoardSensors` class.
+            If the `adc_io_Set` method returns a truthy value, an error message is logged.
+            The function returns the instance of the class.
+        """
+        if TECHSTAR_LIB.adc_io_Set(index, level):
+            _logger.error(f"Failed to set IO level, index: {index}, level: {level}")
         return self
 
-    def set_all_io_level(self, level: int) -> Self:
+    def set_all_io_level(self, level: Literal[0, 1]) -> Self:
         """
-        int __fastcall adc_io_SetAll(unsigned int a1)
-        {
-          char *v1; // r3
-          char v3[8]; // [sp+4h] [bp-14h] BYREF
-          char v4; // [sp+Ch] [bp-Ch] BYREF
-
-          v1 = v3;
-          do
-          {
-            *++v1 = (a1 & 1) != 0;
-            a1 >>= 1;
-          }
-          while ( &v4 != v1 );
-          v3[0] = 24;
-          if ( pi_1 < 0 )
-            return -1;
-          spi_write(pi_1, hspi1, v3, 9);
-          return 0;
-        }
+        Sets the level of all IOs to the specified level.
+
+        Args:
+            level (Literal[0, 1]): The level to set for all IOs.
+
+        Returns:
+            Self: The instance of the class.
+
+        Raises:
+            None
+
+        Description:
+            This function sets the level of all IOs to the specified level using the `adc_io_SetAll` method from the `OnBoardSensors` class.
+            If the `adc_io_SetAll` method returns a truthy value, an error message is logged.
+            The function returns the instance of the class.
         """
-        OnBoardSensors.__lib.adc_io_SetAll(level)
+        if TECHSTAR_LIB.adc_io_SetAll(level):
+            _logger.error("Failed to set all IO level")
         return self
 
     @staticmethod
-    def get_all_io_mode(buffer: int):
+    def get_all_io_mode() -> bytes:
         """
-        int __fastcall adc_io_ModeGetAll(_BYTE *a1)
-        {
-          int result; // r0
-          char v3; // [sp+Dh] [bp-Bh]
-
-          if ( pi_1 < 0 )
-            return -1;
-          spi_xfer(pi_1);
-          result = 0;
-          *a1 = v3;
-          return result;
-        }
+        Get all IO modes. length = 8,store as bit0,bit1,bit2,bit3,bit4,bit5,bit6,bit7
+
+        Returns:
+            bytes: A buffer containing all IO modes.
         """
-        return OnBoardSensors.__lib.adc_io_ModeGetAll(buffer)
+        buffer = ctypes.c_char()
+        if TECHSTAR_LIB.adc_io_ModeGetAll(buffer):
+            _logger.error("Failed to get all IO mode")
+        return buffer.value
 
     @staticmethod
-    def get_io_level(index: int) -> int:
+    def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7]) -> int:
+        """
+        Get the level of the specified IO index.
 
-        return (OnBoardSensors.__lib.adc_io_InputGetAll() >> index) & 1
+        Args:
+            index (Literal[0, 1, 2, 3, 4, 5, 6, 7]): The index of the IO.
+
+        Returns:
+            int: The level of the specified IO index, which is calculated based on the result of adc_io_InputGetAll().
 
-    def set_all_io_mode(self, mode: int) -> Self:
         """
-        int __fastcall adc_io_ModeSetAll(char a1)
-        {
-          char v2[12]; // [sp+4h] [bp-Ch] BYREF
+        return (TECHSTAR_LIB.adc_io_InputGetAll() >> index) & 1
 
-          v2[1] = a1;
-          v2[0] = 21;
-          if ( pi_1 < 0 )
-            return -1;
-          spi_write(pi_1, hspi1, v2, 2);
-          return 0;
-        }
+    def set_all_io_mode(self, mode: Literal[0, 1]) -> Self:
         """
-        OnBoardSensors.__lib.adc_io_ModeSetAll(mode)
-        return self
+        Sets the mode of all IOs to the specified mode.
+
+        Args:
+            mode (Literal[0, 1]): The mode to set for all IOs. Must be either 0 or 1.
+
+        Returns:
+            Self: The instance of the class.
 
-    def set_io_mode(self, index: int, mode: int) -> Self:
+        Raises:
+            None
+
+        Description:
+            This function sets the mode of all IOs to the specified mode using the `adc_io_ModeSetAll` method from the `TECHSTAR_LIB` library.
+            If the `adc_io_ModeSetAll` method returns a truthy value, an error message is logged.
+            The function returns the instance of the class.
         """
-        change the mode of the adc-io plug at index,mode 1 for output, 0 for input
+        if TECHSTAR_LIB.adc_io_ModeSetAll(mode):
+            _logger.error(f"Failed to set all IO mode to {mode}")
+        return self
 
-        int __fastcall adc_io_ModeSet(unsigned int a1, int a2)
-        {
-          char v2; // r4
-          char v4[9]; // [sp+7h] [bp-9h] BYREF
-
-          if ( a1 > 7 )
-            return -1;
-          v2 = a1;
-          if ( a2 )
-          {
-            if ( !j_adc_io_ModeGetAll(v4) )
-            {
-              v4[0] |= 1 << v2;
-              return j_adc_io_ModeSetAll();
-            }
-            return -1;
-          }
-          if ( j_adc_io_ModeGetAll(v4) )
-            return -1;
-          v4[0] &= ~(1 << v2);
-          return j_adc_io_ModeSetAll();
-        }
+    def set_io_mode(
+        self, index: Literal[0, 1, 2, 3, 4, 5, 6, 7], mode: Literal[0, 1]
+    ) -> Self:
         """
+        Sets the mode of the specified IO index to the specified mode.
+
+        Args:
+            index (Literal[0, 1]): The index of the IO. Must be either 0 or 1.
+            mode (Literal[0, 1]): The mode to set for the IO. Must be either 0 or 1.
 
-        OnBoardSensors.__lib.adc_io_ModeSet(index, mode)
+        Returns:
+            Self: The instance of the class.
+
+        Raises:
+            None
+
+        Description:
+            This function sets the mode of the specified IO index to the specified mode using the `adc_io_ModeSet` method from the `TECHSTAR_LIB` library.
+            If the `adc_io_ModeSet` method returns a truthy value, an error message is logged.
+            The function returns the instance of the class.
+        """
+        if TECHSTAR_LIB.adc_io_ModeSet(index, mode):
+            _logger.error(f"Failed to set IO mode, index: {index}, mode: {mode}")
         return self
 
     @staticmethod
-    def io_all_channels():
+    def io_all_channels() -> ctypes.c_uint8:
         """
         get all io plug input levels
 
         uint8, each bit represents a channel, 1 for high, 0 for low
         """
-        updated_data = OnBoardSensors.__lib.adc_io_InputGetAll()
-        return tuple((updated_data >> i) & 1 for i in range(8))
+        return TECHSTAR_LIB.adc_io_InputGetAll()
 
     def MPU6500_Open(self) -> Self:
         """
         initialize the 6-axis enhancer MPU6500
         default settings:
             acceleration: -+8G
             gyro: -+2000 degree/s
             sampling rate: 1kHz
         """
-        _logger.info("initializing MPU6500")
-        success = OnBoardSensors.__lib.mpu6500_dmp_init()
-
-        if success:
+        if TECHSTAR_LIB.mpu6500_dmp_init():
             _logger.warning("Failed to initialize MPU6500")
         else:
             _logger.info("MPU6500 successfully initialized")
         return self
 
-    @staticmethod
-    def acc_all():
-        """
-        get the acceleration from MPU6500
+    def acc_all(self) -> ctypes.Array:
         """
-        OnBoardSensors.__lib.mpu6500_Get_Accel(OnBoardSensors._accel_all)
+        Retrieves the acceleration data from the MPU6500 sensor.
 
-        return OnBoardSensors._accel_all
-
-    @staticmethod
-    def gyro_all():
+        Returns:
+            ctypes.Array: An array containing the acceleration data.
+        Notes:
+            length = 3
+            [0] ==> axis X
+            [1] ==> axis Y
+            [2] ==> axis Z
         """
-        get gyro from MPU6500
+        TECHSTAR_LIB.mpu6500_Get_Accel(
+            self._accel_all
+        )  # this function return a C pointer to the self._accel_all
+        return self._accel_all
+
+    def gyro_all(self) -> ctypes.Array:
         """
-        OnBoardSensors.__lib.mpu6500_Get_Gyro(OnBoardSensors._gyro_all)
+        Retrieves the gyroscope data from the MPU6500 sensor.
 
-        return OnBoardSensors._gyro_all
+        Returns:
+            ctypes.Array: An array containing the gyroscope data.
 
-    @staticmethod
-    def atti_all():
+        Notes:
+            length = 3
+            [0] ==> axis X
+            [1] ==> axis Y
+            [2] ==> axis Z
         """
-        Get attitude from MPU6500
 
-        NOTE:
-            the sampling frequency of the attitude data updates every 10ms.
-            So, high sampling-frequency may not be a good option
+        TECHSTAR_LIB.mpu6500_Get_Gyro(
+            self._gyro_all
+        )  # this function return a C pointer to the self._gyro_all
+
+        return self._gyro_all
+
+    def atti_all(self) -> ctypes.Array:
         """
+        Retrieves the attitude data from the MPU6500 sensor.
 
-        OnBoardSensors.__lib.mpu6500_Get_Attitude(OnBoardSensors._atti_all)
+        Returns:
+            ctypes.Array: An array containing the attitude data.
 
-        return OnBoardSensors._atti_all
+        Notes:
+            length = 3
+            [0] ==> Pitch|axis X
+            [1] ==> Roll |axis Y
+            [2] ==> Yaw  |axis Z
+        """
+        TECHSTAR_LIB.mpu6500_Get_Attitude(
+            self._atti_all
+        )  # this function return a C pointer to the self._atti_all
+
+        return self._atti_all
 
     @staticmethod
-    def get_handle(attr_name: str):
-        return getattr(OnBoardSensors.__lib, attr_name)
+    def get_handle(attr_name: str) -> Any:
+        """
+        Returns the attribute value of the TECHSTAR_LIB object corresponding to the given attribute name.
+        Reserved to the user to harness other attributes of the TECHSTAR_LIB object.
+        Args:
+            attr_name (str): The name of the attribute to retrieve.
+
+        Returns:
+            Any: The value of the attribute.
+
+        Raises:
+            AttributeError: If the attribute does not exist in the TECHSTAR_LIB object.
+        """
+        return getattr(TECHSTAR_LIB, attr_name)
```

### Comparing `pyuptech-0.1.2/tests/perf_tests.py` & `pyuptech-0.1.3/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.2/PKG-INFO` & `pyuptech-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
 
 # pyuptech
 
 > 一个API包装库，通过调用TechStar的二进制so库完成的功能
 ---
 
+# 安装
+
+使用`pdm`安装
+
+```shell
+pdm add pyuptech
+```
+
 ## OnBoardSensors
 
 **简介**
 
 `OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
 
 ### 类方法概览
@@ -45,32 +54,34 @@
 - 限制ADC采样频率，防止过采样。
 - 获取ADC和GPIO的数据。
 - 初始化和读取MPU6500六轴传感器数据。
 
 ### QUICKSTART
 
 ```python
-from pyuptech import OnBoardSensors, OUTPUT, LOW
+from pyuptech import OnBoardSensors
+from ctypes import c_uint8, Array
 
-# 创建OnBoardSensors对象
-sensor_controller = OnBoardSensors()
+# 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
+sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
-# 设置ADC最小采样间隔为10ms
+# 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
-gpio_levels = sensor_controller.io_all_channels()
+gpio_levels: c_uint8 = sensor_controller.io_all_channels()
+print(gpio_levels)
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
-acceleration_data = sensor_controller.acc_all()
+acceleration_data: Array = sensor_controller.acc_all()
 
 # 设置第3号GPIO引脚为输出并设置电平为低
-sensor_controller.set_io_mode(2, OUTPUT)
-sensor_controller.set_io_level(2, LOW)
+sensor_controller.set_io_mode(2, 1)
+sensor_controller.set_io_level(2, 0)
 ```
 
 ---
 
 # Screen
 
 本模块定义了一个名为 `Screen`
@@ -166,8 +177,57 @@
 """
 
 set_log_level(50)  # 将日志等级设为50，此时logger只会记录优先级高于CRITICAL级别的消息
 
 from logging import CRITICAL
 
 set_log_level(CRITICAL)  # 上述代码与上面设置效果一致，即只记录CRITICAL及其以上级别的日志信息
-```
+```
+
+---
+
+## 调试
+
+通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
+
+```python
+from pyuptech import (
+    mpu_display_on_lcd,
+    mpu_display_on_console,
+    adc_io_display_on_lcd,
+    adc_io_display_on_console)
+
+mpu_display_on_console()  # 将MPU6500数据打印到终端
+
+mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
+
+# 定义ADC标签索引字典，可以空缺部分键值
+adc_labels = {
+    6: 'EDGE_FL',
+    7: "EDGE_RL",
+    2: 'EDGE_FR',
+    1: 'EDGE_RR',
+    8: 'L1',
+    0: 'R1',
+    3: 'FB', 5: 'RB',
+    4: 'GRAY'
+}
+# 定义IO标签索引字典,可以空缺部分键值
+io_labels = {
+    3: "gray l",
+    2: "gray r",
+
+    7: 'ftl',
+    6: 'ftr',
+    5: 'rtr'
+}
+
+adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
+
+adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+
+
+
+
+```
+
+
```

