# Comparing `tmp/asgebsmanager-1.3.tar.gz` & `tmp/asgebsmanager-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-1.3.tar", last modified: Sun Apr 14 11:52:24 2024, max compression
+gzip compressed data, was "asgebsmanager-1.4.tar", last modified: Sat Apr 20 12:37:05 2024, max compression
```

## Comparing `asgebsmanager-1.3.tar` & `asgebsmanager-1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 11:52:24.987923 asgebsmanager-1.3/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 11:52:24.987430 asgebsmanager-1.3/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 11:52:24.986830 asgebsmanager-1.3/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 11:52:24.000000 asgebsmanager-1.3/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 11:52:24.988066 asgebsmanager-1.3/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 11:52:20.000000 asgebsmanager-1.3/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 11:52:24.981288 asgebsmanager-1.3/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 11:52:24.986067 asgebsmanager-1.3/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.3/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1289 2024-04-14 11:27:15.000000 asgebsmanager-1.3/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     7720 2024-04-14 11:14:20.000000 asgebsmanager-1.3/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.3/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.625118 asgebsmanager-1.4/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-20 12:37:05.624597 asgebsmanager-1.4/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.623998 asgebsmanager-1.4/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      388 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-20 12:37:05.000000 asgebsmanager-1.4/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-20 12:37:05.625221 asgebsmanager-1.4/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-20 08:28:52.000000 asgebsmanager-1.4/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.615452 asgebsmanager-1.4/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-20 12:37:05.622754 asgebsmanager-1.4/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.4/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1530 2024-04-20 09:16:10.000000 asgebsmanager-1.4/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     9846 2024-04-20 09:14:58.000000 asgebsmanager-1.4/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1508 2024-04-20 09:22:56.000000 asgebsmanager-1.4/src/asgebsmanager/file_utils.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.4/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-1.3/setup.py` & `asgebsmanager-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "1.3",
+    version = "1.4",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
```

### Comparing `asgebsmanager-1.3/src/asgebsmanager/__main__.py` & `asgebsmanager-1.4/src/asgebsmanager/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import argparse
 
 from asgebsmanager.ebs_manager import manage_ebs
 
 def main():
-    parser = argparse.ArgumentParser("asgebsmanager",description="Manages the ebs volume in autoscaling environment")
-    parser.add_argument("--asg_name",type=str,required=True,help="Name of the asg to be used as the tag to identify the volume to be attached")
+    parser = argparse.ArgumentParser("asgebsmanager",formatter_class=argparse.ArgumentDefaultsHelpFormatter,description="Manages the ebs volume in autoscaling environment")
+    parser.add_argument("--asg-name",type=str,required=True,help="Name of the asg to be used as the tag to identify the volume to be attached")
     parser.add_argument("--region",type=str,default="ap-south-1",help="AWS region")
     parser.add_argument("--size",type=int,default=200,help="Size of the volume")
     parser.add_argument("--iops",type=int,default=3000,help="Iops of the volume")
     parser.add_argument("--throughput",type=int,default=125,help="Throughput of the volume")
+    parser.add_argument("--fs-type",type=str,default="xfs",help="File system type")
     parser.add_argument("--device",type=str,default="/dev/xvdg",help="Device name to be used")
-    parser.add_argument("--check_timeout",type=int,default=5,help="Timeout for each volume retry operation")
+    parser.add_argument("--mount-point",type=str,default="/data",help="Mount Point path")
+    parser.add_argument("--check-timeout",type=int,default=5,help="Timeout in minutes for each ebs api retry operation")
     parser.add_argument("--force",action='store_true',help="Set it to true, so that a new volume will be created if no existing volume is found")
     parser.add_argument("--delete",action='store_true',help="Set it to true, so that a old volume/snapshot will be deleted if a new volume is created from snapshot")
 
     args = parser.parse_args()
 
     manage_ebs(args)
```

### Comparing `asgebsmanager-1.3/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-1.4/src/asgebsmanager/ebs_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import boto3
 from time import sleep
 
 from asgebsmanager.mds_utils import get_imds_token, get_instance_metadata
-
+from asgebsmanager.file_utils import get_fs_util_for
 
 class AsgEbsManager:
 
     def __init__(self,region,asg_name):
         self.asg_name = asg_name
         self.session = boto3.Session(region_name=region)
         self.ec2_client = self.session.client('ec2')
 
     @staticmethod
     def __get_name():
         return 'AsgEbsManager'
     
-    def latest_volume(self,az,state=None):
+    def latest_volume(self,az=None,state=None):
         status = ["available","in-use"] if state is None else [state]
-        volumes = self.ec2_client.describe_volumes(
-            Filters=[
+        filters = [
                 {
                     'Name': 'tag:BelongsTo',
                     'Values': [
                         self.asg_name,
                     ]
                 },
                 {
                     'Name': 'tag:ManagedBy',
                     'Values': [
                         self.__get_name(),
                     ]
                 },
                 {
+                    'Name': 'status',
+                    'Values': status
+                }
+            ]
+        if az is not None:
+            filters.append({
                     'Name': 'availability-zone',
                     'Values': [
                         az,
                     ]
-                },
-                {
-                    'Name': 'status',
-                    'Values': status
-                }
-            ],
+            })
+        volumes = self.ec2_client.describe_volumes(
+            Filters=filters,
             MaxResults=100
         )
 
         if len(volumes['Volumes']) > 0:
             sorted_volume = [volume['VolumeId'] for volume in sorted(volumes['Volumes'], key=lambda volume: volume['CreateTime'])]
             return sorted_volume[0]
         return None
@@ -123,100 +125,146 @@
                     'Key': 'ManagedBy',
                     'Value': self.__get_name(),
                 }
             ]
         )
 
 def manage_ebs(args):
-    asg_ebs_manager = AsgEbsManager(region=args.region,asg_name=args.asg_name)
+    try: 
+       # get fs_util
+        fs_util = get_fs_util_for(args.fs_type,args={
+            'device': args.device,
+            'mount_point': args.mount_point
+        })
+
+        asg_ebs_manager = AsgEbsManager(region=args.region,asg_name=args.asg_name)
 
-    # get the current instance az and id
-    mds_token = get_imds_token()
+        # get the current instance az and id
+        mds_token = get_imds_token()
 
-    az =  get_instance_metadata(mds_token,"placement/availability-zone")
-    instance_id =  get_instance_metadata(mds_token,"instance-id")
+        az =  get_instance_metadata(mds_token,"placement/availability-zone")
+        instance_id =  get_instance_metadata(mds_token,"instance-id")
 
-    volume_id = asg_ebs_manager.latest_volume(az)
-    # if volume_id is not None, there is chance we can get the available volume
-    if volume_id is not None:
-        # find the available volume
-        volume_id = asg_ebs_manager.latest_volume(az,'available')
-        # wait for some other volume to be available
-        max_retries = args.check_timeout
-        while volume_id is None and max_retries > 0:
-                sleep(60)
-                volume_id = asg_ebs_manager.latest_volume(az,'available')
-                max_retries -= 1
-        if max_retries == 0:
-            volume_id = None
-    
-    # check the difference in the volume configuration and if there is a diff, 
-    # create a new volume from the snapshot of the existing volume and
-    # delete the older volume
-    if volume_id:
-        volume = asg_ebs_manager.describe_volume(volume_id)
-        snapshot_id = None
-        if volume['Size'] != args.size or volume['Iops'] != args.iops or volume['Throughput'] != args.throughput:
-            snapshot_id = asg_ebs_manager.create_snapshot(volume_id)
-            snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
+        volume_id = asg_ebs_manager.latest_volume(az)
+        # if volume_id is not None, there is chance we can get the available volume
+        if volume_id is not None:
+            # find the available volume
+            volume_id = asg_ebs_manager.latest_volume(az,'available')
+            # wait for some other volume to be available
             max_retries = args.check_timeout
-            while snapshot['State'] != 'completed' and max_retries > 0:
+            while volume_id is None and max_retries > 0:
                 sleep(60)
+                volume_id = asg_ebs_manager.latest_volume(az,'available')
                 max_retries -= 1
-                snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
-            # if snapshot is not getting created, attach the same volume
             if max_retries == 0:
-                snapshot_id = None
+                volume_id = None
 
-        # if the snapshot is created, create a new volume
-        if snapshot_id:
-            old_volume_id = volume_id
-            asg_ebs_manager.tag_resource(snapshot_id)
-            volume_id = asg_ebs_manager.create_volume(az,args.size,args.iops,args.throughput,snapshot_id=snapshot_id)
+        az_diff = False
+
+        # try to find an available volume in other azs and create snapshot 
+        if volume_id is None:
+            volume_id = asg_ebs_manager.latest_volume()
+            # if volume_id is not None, there is chance we can get the available volume
+            if volume_id is not None:
+                # find the available volume
+                volume_id = asg_ebs_manager.latest_volume(state='available')
+                # wait for some other volume to be available
+                max_retries = args.check_timeout
+                while volume_id is None and max_retries > 0:
+                        sleep(60)
+                        volume_id = asg_ebs_manager.latest_volume(state='available')
+                        max_retries -= 1
+                if max_retries == 0:
+                    volume_id = None
+                if volume_id is not None:
+                    az_diff = True
+
+        # only if 'force' is enabled
+        # check the difference in the volume configuration and if there is a diff, 
+        # create a new volume from the snapshot of the existing volume and
+        # delete the older volume 
+        if volume_id and args.force:
+            volume = asg_ebs_manager.describe_volume(volume_id)
+            snapshot_id = None
+            if volume['Size'] != args.size or volume['Iops'] != args.iops or volume['Throughput'] != args.throughput or az_diff:
+                snapshot_id = asg_ebs_manager.create_snapshot(volume_id)
+                snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
+                max_retries = args.check_timeout
+                while snapshot['State'] != 'completed' and max_retries > 0:
+                    sleep(60)
+                    max_retries -= 1
+                    snapshot = asg_ebs_manager.describe_snapshot(snapshot_id)
+                # if snapshot is not getting created, attach the same volume
+                if max_retries == 0:
+                    snapshot_id = None
+
+            # if the snapshot is created, create a new volume
+            if snapshot_id:
+                old_volume_id = volume_id
+                asg_ebs_manager.tag_resource(snapshot_id)
+                volume_id = asg_ebs_manager.create_volume(az,args.size,args.iops,args.throughput,snapshot_id=snapshot_id)
+                max_retries = args.check_timeout
+                volume = asg_ebs_manager.describe_volume(volume_id)
+                while volume['State'] != 'available' and max_retries > 0:
+                    sleep(60)
+                    max_retries -= 1
+                    volume = asg_ebs_manager.describe_volume(volume_id)
+                if max_retries == 0:
+                    volume_id = None
+                if args.delete:
+                    asg_ebs_manager.delete_volume(old_volume_id)
+                    asg_ebs_manager.delete_snapshot(snapshot_id)
+                az_diff = False
+                
+        # In this case , we cannot do anything other than creating a new volume
+        if volume_id is None: 
+            volume_id = asg_ebs_manager.create_volume(az,args.size,args.iops,args.throughput)
             max_retries = args.check_timeout
             volume = asg_ebs_manager.describe_volume(volume_id)
             while volume['State'] != 'available' and max_retries > 0:
                 sleep(60)
                 max_retries -= 1
                 volume = asg_ebs_manager.describe_volume(volume_id)
             if max_retries == 0:
                 volume_id = None
-            if args.delete:
-                asg_ebs_manager.delete_volume(old_volume_id)
-                asg_ebs_manager.delete_snapshot(snapshot_id)
-            
 
 
-    # In this case , we cannot do anything other than creating a new volume
-    if volume_id is None and args.force: 
-        volume_id = asg_ebs_manager.create_volume(az,args.size,args.iops,args.throughput)
-        max_retries = args.check_timeout
-        volume = asg_ebs_manager.describe_volume(volume_id)
-        while volume['State'] != 'available' and max_retries > 0:
-            sleep(60)
-            max_retries -= 1
+        # if we are able to create/ reuse old volume in the same az, attach the volume to the instance and tag it
+        if volume_id is not None and not az_diff:
+            volume_id = asg_ebs_manager.attach_volume(volume_id,instance_id,args.device)
+            max_retries = args.check_timeout
             volume = asg_ebs_manager.describe_volume(volume_id)
-        if max_retries == 0:
-            volume_id = None
+            while volume['State'] != 'in-use' and max_retries > 0:
+                sleep(60)
+                max_retries -= 1
+                volume = asg_ebs_manager.describe_volume(volume_id)
+            if max_retries == 0:
+                volume_id = None
+            
+            # if we are able to attach volume successfully to the instance, tag the volume 
+            if volume_id is not None:
+                asg_ebs_manager.tag_resource(volume_id)
+
+            if fs_util.wait_for_device():
+                fs_util.format()
+                fs_util.mount()
+            else:
+                raise Exception(f"Unable to locate device {args.device}")
+            return
 
+    # catch all 
+    except Exception as e:
+        print(f'Some error occurred :: {e}')
 
-    # if we are able to create/ reuse old volume, attach the volume to the instance and tag it
-    if volume_id is not None:
-        volume_id = asg_ebs_manager.attach_volume(volume_id,instance_id,args.device)
-        max_retries = args.check_timeout
-        volume = asg_ebs_manager.describe_volume(volume_id)
-        while volume['State'] != 'in-use' and max_retries > 0:
-            sleep(60)
-            max_retries -= 1
-            volume = asg_ebs_manager.describe_volume(volume_id)
-        if max_retries == 0:
-            volume_id = None
-        
-        # if we are able to attach volume successfully to the instance, tag the volume 
-        if volume_id is not None:
-            asg_ebs_manager.tag_resource(volume_id)
-            return
+    # cleanup
+    try:
+        if snapshot_id:
+            asg_ebs_manager.delete_snapshot(snapshot_id)
+        if volume_id:
+            asg_ebs_manager.delete_volume(volume_id)
+    except Exception as e:
+        pass
 
     # Exiting because we were not able to create or attach volume successfully
     exit(1)
```

### Comparing `asgebsmanager-1.3/src/asgebsmanager/mds_utils.py` & `asgebsmanager-1.4/src/asgebsmanager/mds_utils.py`

 * *Files identical despite different names*

