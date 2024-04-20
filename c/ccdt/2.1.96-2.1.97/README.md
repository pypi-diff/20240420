# Comparing `tmp/ccdt-2.1.96.tar.gz` & `tmp/ccdt-2.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.96.tar", last modified: Wed Apr 17 08:35:42 2024, max compression
+gzip compressed data, was "ccdt-2.1.97.tar", last modified: Sat Apr 20 06:16:55 2024, max compression
```

## Comparing `ccdt-2.1.96.tar` & `ccdt-2.1.97.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.341248 ccdt-2.1.96/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.96/LICENSE
--rw-rw-rw-   0        0        0     4806 2024-04-17 08:35:42.340251 ccdt-2.1.96/PKG-INFO
--rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.96/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.190991 ccdt-2.1.96/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.96/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.198969 ccdt-2.1.96/ccdt/dataset/
--rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.96/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.200964 ccdt-2.1.96/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.96/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.96/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.219072 ccdt-2.1.96/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    15439 2024-04-17 03:45:32.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0   116306 2024-04-17 03:29:29.000000 ccdt-2.1.96/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.268930 ccdt-2.1.96/ccdt/dataset/base_voc/
--rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.96/ccdt/dataset/base_voc/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_sys.py
--rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_txt.py
--rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.96/ccdt/dataset/base_voc/base_voc.py
--rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.96/ccdt/dataset/base_voc/coco_to_labelme.py
--rw-rw-rw-   0        0        0    24241 2024-04-17 02:49:30.000000 ccdt-2.1.96/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.285530 ccdt-2.1.96/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.96/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.96/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    27118 2024-04-17 08:29:52.000000 ccdt-2.1.96/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.316315 ccdt-2.1.96/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.96/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.96/ccdt/video_tool/intercept.py
--rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.96/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.96/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.339253 ccdt-2.1.96/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4806 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 08:35:42.000000 ccdt-2.1.96/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 08:35:42.341248 ccdt-2.1.96/setup.cfg
--rw-rw-rw-   0        0        0     2524 2024-04-17 08:35:11.000000 ccdt-2.1.96/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:35:42.330277 ccdt-2.1.96/test/
--rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.96/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.679922 ccdt-2.1.97/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.97/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-20 06:16:55.677946 ccdt-2.1.97/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.97/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.512086 ccdt-2.1.97/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.97/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.521035 ccdt-2.1.97/ccdt/dataset/
+-rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.97/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.523059 ccdt-2.1.97/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.97/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.97/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.553484 ccdt-2.1.97/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.97/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    15439 2024-04-17 03:45:32.000000 ccdt-2.1.97/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0   116306 2024-04-17 03:29:29.000000 ccdt-2.1.97/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.615448 ccdt-2.1.97/ccdt/dataset/base_voc/
+-rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.97/ccdt/dataset/base_voc/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.97/ccdt/dataset/base_voc/base_sys.py
+-rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.97/ccdt/dataset/base_voc/base_txt.py
+-rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.97/ccdt/dataset/base_voc/base_voc.py
+-rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.97/ccdt/dataset/base_voc/coco_to_labelme.py
+-rw-rw-rw-   0        0        0    24566 2024-04-20 04:27:41.000000 ccdt-2.1.97/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.631537 ccdt-2.1.97/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.97/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.97/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    28515 2024-04-20 06:16:25.000000 ccdt-2.1.97/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.654018 ccdt-2.1.97/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.97/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.97/ccdt/video_tool/intercept.py
+-rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.97/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.97/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.676945 ccdt-2.1.97/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-20 06:16:55.000000 ccdt-2.1.97/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 06:16:55.679922 ccdt-2.1.97/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2024-04-20 06:16:38.000000 ccdt-2.1.97/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 06:16:55.667981 ccdt-2.1.97/test/
+-rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.97/test/test.py
```

### Comparing `ccdt-2.1.96/LICENSE` & `ccdt-2.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/PKG-INFO` & `ccdt-2.1.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.96
+Version: 2.1.97
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.96/README.md` & `ccdt-2.1.97/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.97/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.97/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.97/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_voc/base_sys.py` & `ccdt-2.1.97/ccdt/dataset/base_voc/base_sys.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_voc/base_txt.py` & `ccdt-2.1.97/ccdt/dataset/base_voc/base_txt.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_voc/base_voc.py` & `ccdt-2.1.97/ccdt/dataset/base_voc/base_voc.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/base_voc/coco_to_labelme.py` & `ccdt-2.1.97/ccdt/dataset/base_voc/coco_to_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/main.py` & `ccdt-2.1.97/ccdt/dataset/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,16 @@
         return args
     elif args.function == 'modify_flags':  # 修改flags字典值
         return args
     elif args.function == 'filter_flags_true':  # 筛选flags字典值为真的数据
         return args
     elif args.function == 'ratio':  # 筛选flags字典值为真的数据
         return args
+    elif args.function == 'pinyin_images':  # 针对分类图像数据，没有labelme的情况，把文件夹中文转换为拼音
+        return args
     else:
         assert not args.function, '传入的操作功能参数不对:{}'.format(args.function)
 
 
 def main():
     # async def main():
     args = parser_args()
@@ -177,14 +179,16 @@
             async_time = time.time()
             zip_package = data_info.compress_labelme()  # 封装压缩路径及压缩对象
             data_info.make_compress(zip_package)  # 开始压缩
             print('数据读取、压缩使用同步计算耗时')
             print(time.time() - async_time)
         if args.function == 'pinyin':
             data_info.hanzi_to_pinyin()  # 对中文路径转拼音后，重新输出
+        if args.function == 'pinyin_images':
+            data_info.hanzi_to_pinyin_images()  # 对中文路径转拼音后，只处理有图像的情况，没有labelme
         if args.function == 'check_format':  # 检查图像格式
             data_info.check_images_format()
     else:  # 异步读写数据处理，存在少部分同步写数据处理
         async_time = time.time()
         data_info = LabelmeLoad(args, input_datasets_list)  # 初始化输入参数
         # 获取当前正在运行的事件循环，从而可以将异步任务添加到事件循环中执行。在等待IO操作完成的同时，利用CPU计算力进行其他计算，从而提高计算效率
         dataset_info = asyncio.run(data_info.recursive_walk(input_datasets_list[0].get('input_dir'), args.function))
```

### Comparing `ccdt-2.1.96/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.97/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.97/ccdt/dataset/utils/labelme_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,28 +377,61 @@
             os.makedirs(rebuild_new_dir, exist_ok=True)
             try:
                 shutil.copy(rename_dir, rebuild_new_dir)
                 shutil.copy(src_json_file_path, labelme_dir)
             except Exception as e:
                 print(f"拷贝 {rename_dir} 失败: {e}")
 
+    def hanzi_to_pinyin_images(self):
+        """
+        重命名目录汉字为拼音
+        """
+        for root, dirs, files in tqdm(os.walk(self.type_args[0].get('input_dir'), topdown=True)):
+            for dirname in dirs:
+                original_dir = os.path.join(root, dirname)
+                pinyin_dirname = self.convert_chinese_to_pinyin(dirname)
+                new_dir = os.path.join(root, pinyin_dirname)
+                os.rename(original_dir, new_dir)
+            # 递归处理子目录
+            for dirpath, dirnames, filenames in os.walk(self.type_args[0].get('input_dir')):
+                for subdir in dirnames:
+                    self.convert_chinese_to_pinyin(os.path.join(dirpath, subdir))
+                # 重命名路径
+        print(f'重命名中文路径为英文开始')
+
+
     @staticmethod
     def convert_path_to_pinyin(path):
         """
         将给定路径中的汉字转换为拼音。
         path: 需要转换的路径。
         """
         # 获取路径的父目录和文件名
         parent_path, filename = os.path.split(path)
         # 将路径中的汉字转换为拼音并拼接成新的路径
         pinyin_list = pinyin(parent_path, style=Style.NORMAL)
         pinyin_path = ''.join([py[0] for py in pinyin_list])  # 提取每个汉字的首字母拼接成新的路径
         new_path = os.path.join(pinyin_path, filename)
         return new_path
 
+    @staticmethod
+    def convert_chinese_to_pinyin(chinese_text):
+        """
+        重命名目录的汉字为拼音
+        @param chinese_text:
+        @return:
+        """
+        pinyin_text = []
+        for char in chinese_text:
+            if isinstance(char, str):
+                pinyin_list = pinyin(char, style=Style.NORMAL)
+                pinyin_path = ''.join([py[0] for py in pinyin_list])  # 提取每个汉字的首字母拼接成新的路径
+                pinyin_text.append(pinyin_path)
+        return ''.join(pinyin_text)
+
     @classmethod
     def get_videos_path(cls, root_dir, file_formats):
         """
         视频帧提取组合路径
         :param root_dir:
         :param file_formats:
         :return:
```

### Comparing `ccdt-2.1.96/ccdt/video_tool/intercept.py` & `ccdt-2.1.97/ccdt/video_tool/intercept.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/video_tool/split.py` & `ccdt-2.1.97/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt/video_tool/video_main.py` & `ccdt-2.1.97/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.97/ccdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.96
+Version: 2.1.97
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.96/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.97/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.96/setup.py` & `ccdt-2.1.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.96',
+    version='2.1.97',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.96/test/test.py` & `ccdt-2.1.97/test/test.py`

 * *Files identical despite different names*

