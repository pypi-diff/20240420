# Comparing `tmp/aiotieba-4.4.3.tar.gz` & `tmp/aiotieba-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-4.4.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "aiotieba-4.4.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `aiotieba-4.4.3.tar` & `aiotieba-4.4.4.tar`

### file list

```diff
@@ -1,343 +1,343 @@
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 aiotieba-4.4.3/CMakeLists.txt
--rw-r--r--   0        0        0     1211 2022-11-09 12:37:21.000000 aiotieba-4.4.3/LICENSE
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/__init__.py
--rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/__version__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/__init__.py
--rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/__init__.py
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/common.py
--rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/container.py
--rw-r--r--   0        0        0     6380 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/contents.py
--rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/user.py
--rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/vimage.py
--rw-r--r--   0        0        0     1443 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_classdef/vote.py
--rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Agree_pb2.py
--rw-r--r--   0        0        0     2460 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/CommonReq_pb2.py
--rw-r--r--   0        0        0      840 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Error_pb2.py
--rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/ForumList_pb2.py
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/FrsTabInfo_pb2.py
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Media_pb2.py
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Page_pb2.py
--rw-r--r--   0        0        0     2225 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/PbContent_pb2.py
--rw-r--r--   0        0        0     1199 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/PollInfo_pb2.py
--rw-r--r--   0        0        0     2916 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/PostInfoList_pb2.py
--rw-r--r--   0        0        0     2934 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Post_pb2.py
--rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/SimpleForum_pb2.py
--rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/SubPostList_pb2.py
--rw-r--r--   0        0        0     3759 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/ThreadInfo_pb2.py
--rw-r--r--   0        0        0     4321 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/User_pb2.py
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/VideoInfo_pb2.py
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/Voice_pb2.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/_protobuf/__init__.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_bawu/__init__.py
--rw-r--r--   0        0        0      897 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_bawu/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_bawu_blacklist/__init__.py
--rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_bawu_blacklist/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_blacklist_old/__init__.py
--rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_blacklist_old/_api.py
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_post/__init__.py
--rw-r--r--   0        0        0     4719 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_post/_api.py
--rw-r--r--   0        0        0     2008 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_post/protobuf/AddPostReqIdl_pb2.py
--rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/add_post/protobuf/AddPostResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/agree/__init__.py
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/agree/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/agree_vimage/__init__.py
--rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/agree_vimage/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/block/__init__.py
--rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/block/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_bawu/__init__.py
--rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_bawu/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_bawu_blacklist/__init__.py
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_bawu_blacklist/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_blacklist_old/__init__.py
--rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_blacklist_old/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_post/__init__.py
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_post/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_posts/__init__.py
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_posts/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_thread/__init__.py
--rw-r--r--   0        0        0      916 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_thread/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_threads/__init__.py
--rw-r--r--   0        0        0      984 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/del_threads/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/dislike_forum/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/dislike_forum/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/follow_forum/__init__.py
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/follow_forum/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/follow_user/__init__.py
--rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/follow_user/_api.py
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_ats/__init__.py
--rw-r--r--   0        0        0      877 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_ats/_api.py
--rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_ats/_classdef.py
--rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_blacklist/__init__.py
--rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_blacklist/_api.py
--rw-r--r--   0        0        0     3254 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_blacklist/_classdef.py
--rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_info/__init__.py
--rw-r--r--   0        0        0     1445 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_info/_api.py
--rw-r--r--   0        0        0     4532 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_info/_classdef.py
--rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoReqIdl_pb2.py
--rw-r--r--   0        0        0     2371 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoResIdl_pb2.py
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_perm/__init__.py
--rw-r--r--   0        0        0      859 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_perm/_api.py
--rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_perm/_classdef.py
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_postlogs/__init__.py
--rw-r--r--   0        0        0     1438 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_postlogs/_api.py
--rw-r--r--   0        0        0     5348 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_postlogs/_classdef.py
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_userlogs/__init__.py
--rw-r--r--   0        0        0     1438 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_userlogs/_api.py
--rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_bawu_userlogs/_classdef.py
--rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist/__init__.py
--rw-r--r--   0        0        0      930 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist/_api.py
--rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist/_classdef.py
--rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist_old/__init__.py
--rw-r--r--   0        0        0     1679 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist_old/_api.py
--rw-r--r--   0        0        0     3175 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist_old/_classdef.py
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryReqIdl_pb2.py
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryResIdl_pb2.py
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blocks/__init__.py
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blocks/_api.py
--rw-r--r--   0        0        0     2412 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_blocks/_classdef.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_cid/__init__.py
--rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_cid/_api.py
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_comments/__init__.py
--rw-r--r--   0        0        0     1706 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_comments/_api.py
--rw-r--r--   0        0        0    24511 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_comments/_classdef.py
--rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_comments/protobuf/PbFloorReqIdl_pb2.py
--rw-r--r--   0        0        0     1808 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_comments/protobuf/PbFloorResIdl_pb2.py
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_dislike_forums/__init__.py
--rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_dislike_forums/_api.py
--rw-r--r--   0        0        0     2339 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_dislike_forums/_classdef.py
--rw-r--r--   0        0        0     1282 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListReqIdl_pb2.py
--rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListResIdl_pb2.py
--rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_fans/__init__.py
--rw-r--r--   0        0        0      928 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_fans/_api.py
--rw-r--r--   0        0        0     3300 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_fans/_classdef.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_fid/__init__.py
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_fid/_api.py
--rw-r--r--   0        0        0       87 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follow_forums/__init__.py
--rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follow_forums/_api.py
--rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follow_forums/_classdef.py
--rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follows/__init__.py
--rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follows/_api.py
--rw-r--r--   0        0        0     3088 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_follows/_classdef.py
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum/__init__.py
--rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum/_api.py
--rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum/_classdef.py
--rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum_detail/__init__.py
--rw-r--r--   0        0        0     1483 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum_detail/_api.py
--rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum_detail/_classdef.py
--rw-r--r--   0        0        0     1254 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum_detail/protobuf/GetForumDetailReqIdl_pb2.py
--rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_forum_detail/protobuf/GetForumDetailResIdl_pb2.py
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_god_threads/__init__.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_god_threads/_api.py
--rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_god_threads/_classdef.py
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_group_msg/__init__.py
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_group_msg/_api.py
--rw-r--r--   0        0        0     3033 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_group_msg/_classdef.py
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_group_msg/protobuf/GetGroupMsgReqIdl_pb2.py
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_group_msg/protobuf/GetGroupMsgResIdl_pb2.py
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_images/__init__.py
--rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_images/_api.py
--rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_images/_classdef.py
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_member_users/__init__.py
--rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_member_users/_api.py
--rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_member_users/_classdef.py
--rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_posts/__init__.py
--rw-r--r--   0        0        0     2646 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_posts/_api.py
--rw-r--r--   0        0        0    34635 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_posts/_classdef.py
--rw-r--r--   0        0        0     1480 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_posts/protobuf/PbPageReqIdl_pb2.py
--rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_posts/protobuf/PbPageResIdl_pb2.py
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_forums/__init__.py
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_forums/_api.py
--rw-r--r--   0        0        0     2893 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_forums/_classdef.py
--rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_users/__init__.py
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_users/_api.py
--rw-r--r--   0        0        0     2547 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_rank_users/_classdef.py
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recom_status/__init__.py
--rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recom_status/_api.py
--rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recom_status/_classdef.py
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recovers/__init__.py
--rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recovers/_api.py
--rw-r--r--   0        0        0     4426 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_recovers/_classdef.py
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_replys/__init__.py
--rw-r--r--   0        0        0     1508 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_replys/_api.py
--rw-r--r--   0        0        0     7906 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_replys/_classdef.py
--rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_replys/protobuf/ReplyMeReqIdl_pb2.py
--rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_replys/protobuf/ReplyMeResIdl_pb2.py
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_self_follow_forums/__init__.py
--rw-r--r--   0        0        0      904 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_self_follow_forums/_api.py
--rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_self_follow_forums/_classdef.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_initNickname/__init__.py
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_initNickname/_api.py
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_initNickname/_classdef.py
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_moindex/__init__.py
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_moindex/_api.py
--rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_selfinfo_moindex/_classdef.py
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_square_forums/__init__.py
--rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_square_forums/_api.py
--rw-r--r--   0        0        0     2670 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_square_forums/_classdef.py
--rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_square_forums/protobuf/GetForumSquareReqIdl_pb2.py
--rw-r--r--   0        0        0     1822 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_square_forums/protobuf/GetForumSquareResIdl_pb2.py
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_statistics/__init__.py
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_statistics/_api.py
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_statistics/_classdef.py
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_tab_map/__init__.py
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_tab_map/_api.py
--rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_tab_map/_classdef.py
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_tab_map/protobuf/SearchPostForumReqIdl_pb2.py
--rw-r--r--   0        0        0     1715 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_tab_map/protobuf/SearchPostForumResIdl_pb2.py
--rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_threads/__init__.py
--rw-r--r--   0        0        0     1792 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_threads/_api.py
--rw-r--r--   0        0        0    23124 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_threads/_classdef.py
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_threads/protobuf/FrsPageReqIdl_pb2.py
--rw-r--r--   0        0        0     2988 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_threads/protobuf/FrsPageResIdl_pb2.py
--rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getUserInfo_web/__init__.py
--rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getUserInfo_web/_api.py
--rw-r--r--   0        0        0     1792 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getUserInfo_web/_classdef.py
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/__init__.py
--rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/_api.py
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/_classdef.py
--rw-r--r--   0        0        0     1087 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoReqIdl_pb2.py
--rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoResIdl_pb2.py
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_panel/__init__.py
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_panel/_api.py
--rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_panel/_classdef.py
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_user_json/__init__.py
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_user_json/_api.py
--rw-r--r--   0        0        0     1095 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_uinfo_user_json/_classdef.py
--rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_unblock_appeals/__init__.py
--rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_unblock_appeals/_api.py
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_unblock_appeals/_classdef.py
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/__init__.py
--rw-r--r--   0        0        0    14869 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/_classdef.py
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/_const.py
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/get_posts/__init__.py
--rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/get_posts/_api.py
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/get_threads/__init__.py
--rw-r--r--   0        0        0     1860 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/get_threads/_api.py
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/protobuf/UserPostReqIdl_pb2.py
--rw-r--r--   0        0        0     1289 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/get_user_contents/protobuf/UserPostResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/good/__init__.py
--rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/good/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/handle_unblock_appeals/__init__.py
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/handle_unblock_appeals/_api.py
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_websocket/__init__.py
--rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_websocket/_api.py
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_websocket/_classdef.py
--rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_websocket/protobuf/UpdateClientInfoReqIdl_pb2.py
--rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_websocket/protobuf/UpdateClientInfoResIdl_pb2.py
--rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_z_id/__init__.py
--rw-r--r--   0        0        0     3167 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/init_z_id/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/login/__init__.py
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/login/_api.py
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/login/_classdef.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/move/__init__.py
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/move/_api.py
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/__init__.py
--rw-r--r--   0        0        0    13166 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/_classdef.py
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/_const.py
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/get_homepage/__init__.py
--rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/get_homepage/_api.py
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/get_uinfo_profile/__init__.py
--rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/get_uinfo_profile/_api.py
--rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/protobuf/ProfileReqIdl_pb2.py
--rw-r--r--   0        0        0     2066 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/profile/protobuf/ProfileResIdl_pb2.py
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/push_notify/__init__.py
--rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/push_notify/_api.py
--rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/push_notify/_classdef.py
--rw-r--r--   0        0        0     1504 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/push_notify/protobuf/PushNotifyResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/recommend/__init__.py
--rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/recommend/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/recover/__init__.py
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/recover/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/remove_fan/__init__.py
--rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/remove_fan/_api.py
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/search_exact/__init__.py
--rw-r--r--   0        0        0     1147 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/search_exact/_api.py
--rw-r--r--   0        0        0     2981 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/search_exact/_classdef.py
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/send_msg/__init__.py
--rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/send_msg/_api.py
--rw-r--r--   0        0        0     1258 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/send_msg/protobuf/CommitPersonalMsgReqIdl_pb2.py
--rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/send_msg/protobuf/CommitPersonalMsgResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_bawu_perm/__init__.py
--rw-r--r--   0        0        0     1355 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_bawu_perm/_api.py
--rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_blacklist/__init__.py
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_blacklist/_api.py
--rw-r--r--   0        0        0     1640 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_blacklist/protobuf/SetUserBlackReqIdl_pb2.py
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_blacklist/protobuf/SetUserBlackResIdl_pb2.py
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_msg_readed/__init__.py
--rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_msg_readed/_api.py
--rw-r--r--   0        0        0     1260 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgReqIdl_pb2.py
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_nickname_old/__init__.py
--rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_nickname_old/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_profile/__init__.py
--rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_profile/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_thread_privacy/__init__.py
--rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/set_thread_privacy/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sign_forum/__init__.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sign_forum/_api.py
--rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sign_growth/__init__.py
--rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sign_growth/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sync/__init__.py
--rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/sync/_api.py
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/__init__.py
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/_api.py
--rw-r--r--   0        0        0     2184 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/_classdef.py
--rw-r--r--   0        0        0     1276 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidReqIdl_pb2.py
--rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidResIdl_pb2.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/top/__init__.py
--rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/top/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unblock/__init__.py
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unblock/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/undislike_forum/__init__.py
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/undislike_forum/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unfollow_forum/__init__.py
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unfollow_forum/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unfollow_user/__init__.py
--rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/unfollow_user/_api.py
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/ungood/__init__.py
--rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/api/ungood/_api.py
--rw-r--r--   0        0        0    82413 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/client.py
--rw-r--r--   0        0        0     3179 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/config.py
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/const.py
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/core/__init__.py
--rw-r--r--   0        0        0    11505 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/core/account.py
--rw-r--r--   0        0        0     6347 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/core/http.py
--rw-r--r--   0        0        0     3710 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/core/net.py
--rw-r--r--   0        0        0    12163 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/core/websocket.py
--rw-r--r--   0        0        0     4114 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/enums.py
--rw-r--r--   0        0        0     2272 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/exception.py
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/__init__.py
--rw-r--r--   0        0        0     1148 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/cache.py
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/CMakeLists.txt
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/__init__.py
--rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/crypto.pyi
--rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/base32/base32.h
--rw-r--r--   0        0        0      632 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/crc/crc32.h
--rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/LICENSE
--rw-r--r--   0        0        0    21717 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/alignment.h
--rw-r--r--   0        0        0     5280 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/common.h
--rw-r--r--   0        0        0     4182 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/md5.h
--rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/private_access.h
--rw-r--r--   0        0        0     5612 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/sha1.h
--rw-r--r--   0        0        0     7216 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/rapidjson/itoa.h
--rw-r--r--   0        0        0      949 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/const.h
--rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/cuid.h
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/error.h
--rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/pywrap.h
--rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/rc442.h
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/sign.h
--rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/xxHash/LICENSE
--rw-r--r--   0        0        0   253096 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/include/xxHash/xxhash.h
--rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/base32/base32.c
--rw-r--r--   0        0        0     4291 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/crc/crc32.c
--rw-r--r--   0        0        0     9665 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/mbedtls/md5.c
--rw-r--r--   0        0        0    11123 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/mbedtls/sha1.c
--rw-r--r--   0        0        0     5790 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/cuid.c
--rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/lib.c
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/rc442.c
--rw-r--r--   0        0        0     3239 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/sign.c
--rw-r--r--   0        0        0     4348 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/helper/utils.py
--rw-r--r--   0        0        0     2645 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/logging.py
--rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 aiotieba-4.4.3/aiotieba/typing.py
--rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 aiotieba-4.4.3/pyproject.toml
--rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 aiotieba-4.4.3/PKG-INFO
+-rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 aiotieba-4.4.4/CMakeLists.txt
+-rw-r--r--   0        0        0     1211 2022-11-09 12:37:21.000000 aiotieba-4.4.4/LICENSE
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/__init__.py
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/__version__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/__init__.py
+-rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/__init__.py
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/common.py
+-rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/container.py
+-rw-r--r--   0        0        0     6380 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/contents.py
+-rw-r--r--   0        0        0     2975 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/user.py
+-rw-r--r--   0        0        0      653 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/vimage.py
+-rw-r--r--   0        0        0     1443 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_classdef/vote.py
+-rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Agree_pb2.py
+-rw-r--r--   0        0        0     2460 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/CommonReq_pb2.py
+-rw-r--r--   0        0        0      840 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Error_pb2.py
+-rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/ForumList_pb2.py
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/FrsTabInfo_pb2.py
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Media_pb2.py
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Page_pb2.py
+-rw-r--r--   0        0        0     2225 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/PbContent_pb2.py
+-rw-r--r--   0        0        0     1199 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/PollInfo_pb2.py
+-rw-r--r--   0        0        0     2916 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/PostInfoList_pb2.py
+-rw-r--r--   0        0        0     2934 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Post_pb2.py
+-rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/SimpleForum_pb2.py
+-rw-r--r--   0        0        0     1518 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/SubPostList_pb2.py
+-rw-r--r--   0        0        0     3759 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/ThreadInfo_pb2.py
+-rw-r--r--   0        0        0     4321 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/User_pb2.py
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/VideoInfo_pb2.py
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/Voice_pb2.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/_protobuf/__init__.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_bawu/__init__.py
+-rw-r--r--   0        0        0      897 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_bawu/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_bawu_blacklist/__init__.py
+-rw-r--r--   0        0        0      832 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_bawu_blacklist/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_blacklist_old/__init__.py
+-rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_blacklist_old/_api.py
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_post/__init__.py
+-rw-r--r--   0        0        0     4719 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_post/_api.py
+-rw-r--r--   0        0        0     2008 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_post/protobuf/AddPostReqIdl_pb2.py
+-rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/add_post/protobuf/AddPostResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/agree/__init__.py
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/agree/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/agree_vimage/__init__.py
+-rw-r--r--   0        0        0      908 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/agree_vimage/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/block/__init__.py
+-rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/block/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_bawu/__init__.py
+-rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_bawu/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_bawu_blacklist/__init__.py
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_bawu_blacklist/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_blacklist_old/__init__.py
+-rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_blacklist_old/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_post/__init__.py
+-rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_post/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_posts/__init__.py
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_posts/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_thread/__init__.py
+-rw-r--r--   0        0        0      916 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_thread/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_threads/__init__.py
+-rw-r--r--   0        0        0      984 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/del_threads/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/dislike_forum/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/dislike_forum/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/follow_forum/__init__.py
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/follow_forum/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/follow_user/__init__.py
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/follow_user/_api.py
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_ats/__init__.py
+-rw-r--r--   0        0        0      877 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_ats/_api.py
+-rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_ats/_classdef.py
+-rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_blacklist/__init__.py
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_blacklist/_api.py
+-rw-r--r--   0        0        0     3254 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_blacklist/_classdef.py
+-rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_info/__init__.py
+-rw-r--r--   0        0        0     1445 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_info/_api.py
+-rw-r--r--   0        0        0     4532 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_info/_classdef.py
+-rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoReqIdl_pb2.py
+-rw-r--r--   0        0        0     2371 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoResIdl_pb2.py
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_perm/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_perm/_api.py
+-rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_perm/_classdef.py
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_postlogs/__init__.py
+-rw-r--r--   0        0        0     1512 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_postlogs/_api.py
+-rw-r--r--   0        0        0     5310 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_postlogs/_classdef.py
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_userlogs/__init__.py
+-rw-r--r--   0        0        0     1512 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_userlogs/_api.py
+-rw-r--r--   0        0        0     3519 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_bawu_userlogs/_classdef.py
+-rw-r--r--   0        0        0       91 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist/__init__.py
+-rw-r--r--   0        0        0      930 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist/_api.py
+-rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist/_classdef.py
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist_old/__init__.py
+-rw-r--r--   0        0        0     1679 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist_old/_api.py
+-rw-r--r--   0        0        0     3175 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist_old/_classdef.py
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryReqIdl_pb2.py
+-rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryResIdl_pb2.py
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blocks/__init__.py
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blocks/_api.py
+-rw-r--r--   0        0        0     2412 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_blocks/_classdef.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_cid/__init__.py
+-rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_cid/_api.py
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_comments/__init__.py
+-rw-r--r--   0        0        0     1706 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_comments/_api.py
+-rw-r--r--   0        0        0    24511 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_comments/_classdef.py
+-rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_comments/protobuf/PbFloorReqIdl_pb2.py
+-rw-r--r--   0        0        0     1808 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_comments/protobuf/PbFloorResIdl_pb2.py
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_dislike_forums/__init__.py
+-rw-r--r--   0        0        0     1662 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_dislike_forums/_api.py
+-rw-r--r--   0        0        0     2339 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_dislike_forums/_classdef.py
+-rw-r--r--   0        0        0     1282 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListReqIdl_pb2.py
+-rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListResIdl_pb2.py
+-rw-r--r--   0        0        0       71 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_fans/__init__.py
+-rw-r--r--   0        0        0      928 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_fans/_api.py
+-rw-r--r--   0        0        0     3300 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_fans/_classdef.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_fid/__init__.py
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_fid/_api.py
+-rw-r--r--   0        0        0       87 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follow_forums/__init__.py
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follow_forums/_api.py
+-rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follow_forums/_classdef.py
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follows/__init__.py
+-rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follows/_api.py
+-rw-r--r--   0        0        0     3088 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_follows/_classdef.py
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum/__init__.py
+-rw-r--r--   0        0        0      824 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum/_api.py
+-rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum/_classdef.py
+-rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum_detail/__init__.py
+-rw-r--r--   0        0        0     1483 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum_detail/_api.py
+-rw-r--r--   0        0        0     1452 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum_detail/_classdef.py
+-rw-r--r--   0        0        0     1254 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum_detail/protobuf/GetForumDetailReqIdl_pb2.py
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_forum_detail/protobuf/GetForumDetailResIdl_pb2.py
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_god_threads/__init__.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_god_threads/_api.py
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_god_threads/_classdef.py
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_group_msg/__init__.py
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_group_msg/_api.py
+-rw-r--r--   0        0        0     3033 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_group_msg/_classdef.py
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_group_msg/protobuf/GetGroupMsgReqIdl_pb2.py
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_group_msg/protobuf/GetGroupMsgResIdl_pb2.py
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_images/__init__.py
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_images/_api.py
+-rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_images/_classdef.py
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_member_users/__init__.py
+-rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_member_users/_api.py
+-rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_member_users/_classdef.py
+-rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_posts/__init__.py
+-rw-r--r--   0        0        0     2646 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_posts/_api.py
+-rw-r--r--   0        0        0    34651 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_posts/_classdef.py
+-rw-r--r--   0        0        0     1480 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_posts/protobuf/PbPageReqIdl_pb2.py
+-rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_posts/protobuf/PbPageResIdl_pb2.py
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_forums/__init__.py
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_forums/_api.py
+-rw-r--r--   0        0        0     2893 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_forums/_classdef.py
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_users/__init__.py
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_users/_api.py
+-rw-r--r--   0        0        0     2547 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_rank_users/_classdef.py
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recom_status/__init__.py
+-rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recom_status/_api.py
+-rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recom_status/_classdef.py
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recovers/__init__.py
+-rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recovers/_api.py
+-rw-r--r--   0        0        0     4426 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_recovers/_classdef.py
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_replys/__init__.py
+-rw-r--r--   0        0        0     1508 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_replys/_api.py
+-rw-r--r--   0        0        0     7906 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_replys/_classdef.py
+-rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_replys/protobuf/ReplyMeReqIdl_pb2.py
+-rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_replys/protobuf/ReplyMeResIdl_pb2.py
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_self_follow_forums/__init__.py
+-rw-r--r--   0        0        0      904 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_self_follow_forums/_api.py
+-rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_self_follow_forums/_classdef.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_initNickname/__init__.py
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_initNickname/_api.py
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_initNickname/_classdef.py
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_moindex/__init__.py
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_moindex/_api.py
+-rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_selfinfo_moindex/_classdef.py
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_square_forums/__init__.py
+-rw-r--r--   0        0        0     1745 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_square_forums/_api.py
+-rw-r--r--   0        0        0     2670 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_square_forums/_classdef.py
+-rw-r--r--   0        0        0     1362 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_square_forums/protobuf/GetForumSquareReqIdl_pb2.py
+-rw-r--r--   0        0        0     1822 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_square_forums/protobuf/GetForumSquareResIdl_pb2.py
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_statistics/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_statistics/_api.py
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_statistics/_classdef.py
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_tab_map/__init__.py
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_tab_map/_api.py
+-rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_tab_map/_classdef.py
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_tab_map/protobuf/SearchPostForumReqIdl_pb2.py
+-rw-r--r--   0        0        0     1715 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_tab_map/protobuf/SearchPostForumResIdl_pb2.py
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_threads/__init__.py
+-rw-r--r--   0        0        0     1792 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_threads/_api.py
+-rw-r--r--   0        0        0    23124 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_threads/_classdef.py
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_threads/protobuf/FrsPageReqIdl_pb2.py
+-rw-r--r--   0        0        0     2988 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_threads/protobuf/FrsPageResIdl_pb2.py
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getUserInfo_web/__init__.py
+-rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getUserInfo_web/_api.py
+-rw-r--r--   0        0        0     1792 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getUserInfo_web/_classdef.py
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/__init__.py
+-rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/_api.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/_classdef.py
+-rw-r--r--   0        0        0     1087 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoReqIdl_pb2.py
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoResIdl_pb2.py
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_panel/__init__.py
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_panel/_api.py
+-rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_panel/_classdef.py
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_user_json/__init__.py
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_user_json/_api.py
+-rw-r--r--   0        0        0     1095 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_uinfo_user_json/_classdef.py
+-rw-r--r--   0        0        0       77 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_unblock_appeals/__init__.py
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_unblock_appeals/_api.py
+-rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_unblock_appeals/_classdef.py
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/__init__.py
+-rw-r--r--   0        0        0    14869 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/_classdef.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/_const.py
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/get_posts/__init__.py
+-rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/get_posts/_api.py
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/get_threads/__init__.py
+-rw-r--r--   0        0        0     1860 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/get_threads/_api.py
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/protobuf/UserPostReqIdl_pb2.py
+-rw-r--r--   0        0        0     1289 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/get_user_contents/protobuf/UserPostResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/good/__init__.py
+-rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/good/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/handle_unblock_appeals/__init__.py
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/handle_unblock_appeals/_api.py
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_websocket/__init__.py
+-rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_websocket/_api.py
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_websocket/_classdef.py
+-rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_websocket/protobuf/UpdateClientInfoReqIdl_pb2.py
+-rw-r--r--   0        0        0     1608 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_websocket/protobuf/UpdateClientInfoResIdl_pb2.py
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_z_id/__init__.py
+-rw-r--r--   0        0        0     3167 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/init_z_id/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/login/__init__.py
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/login/_api.py
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/login/_classdef.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/move/__init__.py
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/move/_api.py
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/__init__.py
+-rw-r--r--   0        0        0    13166 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/_classdef.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/_const.py
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/get_homepage/__init__.py
+-rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/get_homepage/_api.py
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/get_uinfo_profile/__init__.py
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/get_uinfo_profile/_api.py
+-rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/protobuf/ProfileReqIdl_pb2.py
+-rw-r--r--   0        0        0     2066 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/profile/protobuf/ProfileResIdl_pb2.py
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/push_notify/__init__.py
+-rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/push_notify/_api.py
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/push_notify/_classdef.py
+-rw-r--r--   0        0        0     1504 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/push_notify/protobuf/PushNotifyResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/recommend/__init__.py
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/recommend/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/recover/__init__.py
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/recover/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/remove_fan/__init__.py
+-rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/remove_fan/_api.py
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/search_exact/__init__.py
+-rw-r--r--   0        0        0     1147 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/search_exact/_api.py
+-rw-r--r--   0        0        0     2981 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/search_exact/_classdef.py
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/send_msg/__init__.py
+-rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/send_msg/_api.py
+-rw-r--r--   0        0        0     1258 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/send_msg/protobuf/CommitPersonalMsgReqIdl_pb2.py
+-rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/send_msg/protobuf/CommitPersonalMsgResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_bawu_perm/__init__.py
+-rw-r--r--   0        0        0     1355 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_bawu_perm/_api.py
+-rw-r--r--   0        0        0       72 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_blacklist/__init__.py
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_blacklist/_api.py
+-rw-r--r--   0        0        0     1640 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_blacklist/protobuf/SetUserBlackReqIdl_pb2.py
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_blacklist/protobuf/SetUserBlackResIdl_pb2.py
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_msg_readed/__init__.py
+-rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_msg_readed/_api.py
+-rw-r--r--   0        0        0     1260 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgReqIdl_pb2.py
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_nickname_old/__init__.py
+-rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_nickname_old/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_profile/__init__.py
+-rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_profile/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_thread_privacy/__init__.py
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/set_thread_privacy/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sign_forum/__init__.py
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sign_forum/_api.py
+-rw-r--r--   0        0        0       59 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sign_growth/__init__.py
+-rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sign_growth/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sync/__init__.py
+-rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/sync/_api.py
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/__init__.py
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/_api.py
+-rw-r--r--   0        0        0     2184 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/_classdef.py
+-rw-r--r--   0        0        0     1276 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidReqIdl_pb2.py
+-rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidResIdl_pb2.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/top/__init__.py
+-rw-r--r--   0        0        0     1009 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/top/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unblock/__init__.py
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unblock/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/undislike_forum/__init__.py
+-rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/undislike_forum/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unfollow_forum/__init__.py
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unfollow_forum/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unfollow_user/__init__.py
+-rw-r--r--   0        0        0      846 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/unfollow_user/_api.py
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/ungood/__init__.py
+-rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/api/ungood/_api.py
+-rw-r--r--   0        0        0    82615 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/client.py
+-rw-r--r--   0        0        0     3179 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/config.py
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/const.py
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/core/__init__.py
+-rw-r--r--   0        0        0    11505 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/core/account.py
+-rw-r--r--   0        0        0     6461 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/core/http.py
+-rw-r--r--   0        0        0     3710 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/core/net.py
+-rw-r--r--   0        0        0    12259 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/core/websocket.py
+-rw-r--r--   0        0        0     4114 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/enums.py
+-rw-r--r--   0        0        0     2272 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/exception.py
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/__init__.py
+-rw-r--r--   0        0        0     1148 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/cache.py
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/CMakeLists.txt
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/__init__.py
+-rw-r--r--   0        0        0     1426 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/crypto.pyi
+-rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/base32/base32.h
+-rw-r--r--   0        0        0      632 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/crc/crc32.h
+-rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/LICENSE
+-rw-r--r--   0        0        0    21717 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/alignment.h
+-rw-r--r--   0        0        0     5280 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/common.h
+-rw-r--r--   0        0        0     4182 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/md5.h
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/private_access.h
+-rw-r--r--   0        0        0     5612 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/sha1.h
+-rw-r--r--   0        0        0     7216 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/rapidjson/itoa.h
+-rw-r--r--   0        0        0      949 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/const.h
+-rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/cuid.h
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/error.h
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/pywrap.h
+-rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/rc442.h
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/sign.h
+-rw-r--r--   0        0        0     1389 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/xxHash/LICENSE
+-rw-r--r--   0        0        0   253096 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/include/xxHash/xxhash.h
+-rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/base32/base32.c
+-rw-r--r--   0        0        0     4291 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/crc/crc32.c
+-rw-r--r--   0        0        0     9665 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/mbedtls/md5.c
+-rw-r--r--   0        0        0    11123 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/mbedtls/sha1.c
+-rw-r--r--   0        0        0     5790 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/cuid.c
+-rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/lib.c
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/rc442.c
+-rw-r--r--   0        0        0     3239 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/sign.c
+-rw-r--r--   0        0        0     4348 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/helper/utils.py
+-rw-r--r--   0        0        0     2645 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/logging.py
+-rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 aiotieba-4.4.4/aiotieba/typing.py
+-rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 aiotieba-4.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 aiotieba-4.4.4/PKG-INFO
```

### Comparing `aiotieba-4.4.3/LICENSE` & `aiotieba-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/__init__.py` & `aiotieba-4.4.4/aiotieba/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_classdef/container.py` & `aiotieba-4.4.4/aiotieba/api/_classdef/container.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_classdef/contents.py` & `aiotieba-4.4.4/aiotieba/api/_classdef/contents.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_classdef/user.py` & `aiotieba-4.4.4/aiotieba/api/_classdef/user.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_classdef/vimage.py` & `aiotieba-4.4.4/aiotieba/api/_classdef/vimage.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_classdef/vote.py` & `aiotieba-4.4.4/aiotieba/api/_classdef/vote.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Agree_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Agree_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/CommonReq_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/CommonReq_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Error_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Error_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/ForumList_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/ForumList_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/FrsTabInfo_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/FrsTabInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Media_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Media_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Page_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Page_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/PbContent_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/PbContent_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/PollInfo_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/PollInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/PostInfoList_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/PostInfoList_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Post_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Post_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/SimpleForum_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/SimpleForum_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/SubPostList_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/SubPostList_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/ThreadInfo_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/ThreadInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/User_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/User_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/VideoInfo_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/VideoInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/_protobuf/Voice_pb2.py` & `aiotieba-4.4.4/aiotieba/api/_protobuf/Voice_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_bawu/_api.py` & `aiotieba-4.4.4/aiotieba/api/add_bawu/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_bawu_blacklist/_api.py` & `aiotieba-4.4.4/aiotieba/api/add_bawu_blacklist/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_blacklist_old/_api.py` & `aiotieba-4.4.4/aiotieba/api/add_blacklist_old/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_post/_api.py` & `aiotieba-4.4.4/aiotieba/api/add_post/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_post/protobuf/AddPostReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/add_post/protobuf/AddPostReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/add_post/protobuf/AddPostResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/add_post/protobuf/AddPostResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/agree/_api.py` & `aiotieba-4.4.4/aiotieba/api/agree/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/agree_vimage/_api.py` & `aiotieba-4.4.4/aiotieba/api/agree_vimage/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/block/_api.py` & `aiotieba-4.4.4/aiotieba/api/block/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_bawu/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_bawu/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_bawu_blacklist/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_bawu_blacklist/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_blacklist_old/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_blacklist_old/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_post/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_post/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_posts/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_posts/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_thread/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_thread/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/del_threads/_api.py` & `aiotieba-4.4.4/aiotieba/api/del_threads/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/dislike_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/dislike_forum/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/follow_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/follow_forum/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/follow_user/_api.py` & `aiotieba-4.4.4/aiotieba/api/follow_user/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_ats/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_ats/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_ats/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_ats/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_blacklist/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_blacklist/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_blacklist/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_blacklist/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_info/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_info/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_info/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_info/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_info/protobuf/GetBawuInfoResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_perm/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_perm/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_perm/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_perm/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_postlogs/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_postlogs/_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from typing import Optional
+from urllib.parse import quote
 
 import bs4
 import yarl
 
 from ...const import WEB_BASE_HOST
 from ...core import HttpCore
 from ...enums import BawuSearchType
@@ -33,14 +34,15 @@
         ('ie', 'utf-8'),
     ]
 
     if op_type:
         params.append(('op_type', op_type))
 
     if search_value:
+        search_value = quote(search_value)
         extend_params = [
             ('svalue', search_value),
             ('stype', 'post_uname' if search_type == BawuSearchType.USER else 'op_uname'),
         ]
         params += extend_params
 
     if start_dt or end_dt:
```

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_postlogs/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_postlogs/_classdef.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import dataclasses as dcs
 from datetime import datetime
-from functools import cached_property
 from typing import List
 
 import bs4
 
 from ...exception import TbErrorExt
 from ...helper import default_datetime, removeprefix
 from .._classdef import Containers
```

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_userlogs/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_userlogs/_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from typing import Optional
+from urllib.parse import quote
 
 import bs4
 import yarl
 
 from ...const import WEB_BASE_HOST
 from ...core import HttpCore
 from ...enums import BawuSearchType
@@ -33,14 +34,15 @@
         ('ie', 'utf-8'),
     ]
 
     if op_type:
         params.append(('op_type', op_type))
 
     if search_value:
+        search_value = quote(search_value)
         extend_params = [
             ('svalue', search_value),
             ('stype', 'post_uname' if search_type == BawuSearchType.USER else 'op_uname'),
         ]
         params += extend_params
 
     if start_dt or end_dt:
```

### Comparing `aiotieba-4.4.3/aiotieba/api/get_bawu_userlogs/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_bawu_userlogs/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist_old/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist_old/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist_old/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist_old/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_blacklist_old/protobuf/UserMuteQueryResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blocks/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_blocks/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_blocks/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_blocks/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_cid/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_cid/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_comments/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_comments/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_comments/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_comments/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_comments/protobuf/PbFloorReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_comments/protobuf/PbFloorReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_comments/protobuf/PbFloorResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_comments/protobuf/PbFloorResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_dislike_forums/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_dislike_forums/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_dislike_forums/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_dislike_forums/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_dislike_forums/protobuf/GetDislikeListResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_fans/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_fans/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_fans/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_fans/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_fid/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_fid/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_follow_forums/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_follow_forums/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_follow_forums/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_follow_forums/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_follows/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_follows/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_follows/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_follows/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_forum/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_forum/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum_detail/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_forum_detail/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum_detail/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_forum_detail/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum_detail/protobuf/GetForumDetailReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_forum_detail/protobuf/GetForumDetailReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_forum_detail/protobuf/GetForumDetailResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_forum_detail/protobuf/GetForumDetailResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_god_threads/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_god_threads/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_god_threads/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_god_threads/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_group_msg/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_group_msg/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_group_msg/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_group_msg/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_group_msg/protobuf/GetGroupMsgReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_group_msg/protobuf/GetGroupMsgReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_group_msg/protobuf/GetGroupMsgResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_group_msg/protobuf/GetGroupMsgResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_images/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_images/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_images/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_images/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_member_users/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_member_users/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_member_users/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_member_users/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_posts/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_posts/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_posts/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_posts/_classdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,16 +145,16 @@
         tiebapluses = []
         video = FragVideo_p()
         voice = FragVoice_p()
 
         def _frags():
             for proto in content_protos:
                 _type = proto.type
-                # 0纯文本 9电话号 18话题 27百科词条
-                if _type in [0, 9, 18, 27]:
+                # 0纯文本 9电话号 18话题 27百科词条 40梗百科
+                if _type in [0, 9, 18, 27, 40]:
                     frag = FragText_p.from_tbdata(proto)
                     texts.append(frag)
                     yield frag
                 # 11:tid=5047676428
                 elif _type in [2, 11]:
                     frag = FragEmoji_p.from_tbdata(proto)
                     emojis.append(frag)
```

### Comparing `aiotieba-4.4.3/aiotieba/api/get_posts/protobuf/PbPageReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_posts/protobuf/PbPageReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_posts/protobuf/PbPageResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_posts/protobuf/PbPageResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_rank_forums/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_rank_forums/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_rank_forums/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_rank_forums/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_rank_users/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_rank_users/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_rank_users/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_rank_users/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_recom_status/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_recom_status/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_recom_status/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_recom_status/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_recovers/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_recovers/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_recovers/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_recovers/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_replys/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_replys/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_replys/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_replys/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_replys/protobuf/ReplyMeReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_replys/protobuf/ReplyMeReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_replys/protobuf/ReplyMeResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_replys/protobuf/ReplyMeResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_self_follow_forums/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_self_follow_forums/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_self_follow_forums/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_self_follow_forums/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_selfinfo_initNickname/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_selfinfo_initNickname/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_selfinfo_initNickname/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_selfinfo_initNickname/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_selfinfo_moindex/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_selfinfo_moindex/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_selfinfo_moindex/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_selfinfo_moindex/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_square_forums/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_square_forums/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_square_forums/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_square_forums/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_square_forums/protobuf/GetForumSquareReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_square_forums/protobuf/GetForumSquareReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_square_forums/protobuf/GetForumSquareResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_square_forums/protobuf/GetForumSquareResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_statistics/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_statistics/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_statistics/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_statistics/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_tab_map/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_tab_map/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_tab_map/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_tab_map/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_tab_map/protobuf/SearchPostForumReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_tab_map/protobuf/SearchPostForumReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_tab_map/protobuf/SearchPostForumResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_tab_map/protobuf/SearchPostForumResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_threads/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_threads/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_threads/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_threads/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_threads/protobuf/FrsPageReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_threads/protobuf/FrsPageReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_threads/protobuf/FrsPageResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_threads/protobuf/FrsPageResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getUserInfo_web/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getUserInfo_web/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getUserInfo_web/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getUserInfo_web/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_getuserinfo_app/protobuf/GetUserInfoResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_panel/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_panel/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_panel/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_panel/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_user_json/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_user_json/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_uinfo_user_json/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_uinfo_user_json/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_unblock_appeals/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_unblock_appeals/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_unblock_appeals/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_unblock_appeals/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_user_contents/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/get_user_contents/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_user_contents/get_posts/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_user_contents/get_posts/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_user_contents/get_threads/_api.py` & `aiotieba-4.4.4/aiotieba/api/get_user_contents/get_threads/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_user_contents/protobuf/UserPostReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_user_contents/protobuf/UserPostReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/get_user_contents/protobuf/UserPostResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/get_user_contents/protobuf/UserPostResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/good/_api.py` & `aiotieba-4.4.4/aiotieba/api/good/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/handle_unblock_appeals/_api.py` & `aiotieba-4.4.4/aiotieba/api/handle_unblock_appeals/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/init_websocket/_api.py` & `aiotieba-4.4.4/aiotieba/api/init_websocket/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/init_websocket/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/init_websocket/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/init_websocket/protobuf/UpdateClientInfoReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/init_websocket/protobuf/UpdateClientInfoReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/init_websocket/protobuf/UpdateClientInfoResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/init_websocket/protobuf/UpdateClientInfoResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/init_z_id/_api.py` & `aiotieba-4.4.4/aiotieba/api/init_z_id/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/login/_api.py` & `aiotieba-4.4.4/aiotieba/api/login/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/login/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/login/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/move/_api.py` & `aiotieba-4.4.4/aiotieba/api/move/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/profile/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/profile/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/profile/get_homepage/_api.py` & `aiotieba-4.4.4/aiotieba/api/profile/get_homepage/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/profile/get_uinfo_profile/_api.py` & `aiotieba-4.4.4/aiotieba/api/profile/get_uinfo_profile/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/profile/protobuf/ProfileReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/profile/protobuf/ProfileReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/profile/protobuf/ProfileResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/profile/protobuf/ProfileResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/push_notify/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/push_notify/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/push_notify/protobuf/PushNotifyResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/push_notify/protobuf/PushNotifyResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/recommend/_api.py` & `aiotieba-4.4.4/aiotieba/api/recommend/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/recover/_api.py` & `aiotieba-4.4.4/aiotieba/api/recover/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/remove_fan/_api.py` & `aiotieba-4.4.4/aiotieba/api/remove_fan/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/search_exact/_api.py` & `aiotieba-4.4.4/aiotieba/api/search_exact/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/search_exact/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/search_exact/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/send_msg/_api.py` & `aiotieba-4.4.4/aiotieba/api/send_msg/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/send_msg/protobuf/CommitPersonalMsgReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/send_msg/protobuf/CommitPersonalMsgReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/send_msg/protobuf/CommitPersonalMsgResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/send_msg/protobuf/CommitPersonalMsgResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_bawu_perm/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_bawu_perm/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_blacklist/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_blacklist/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_blacklist/protobuf/SetUserBlackReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/set_blacklist/protobuf/SetUserBlackReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_blacklist/protobuf/SetUserBlackResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/set_blacklist/protobuf/SetUserBlackResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_msg_readed/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_msg_readed/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/set_msg_readed/protobuf/CommitReceivedPmsgResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_nickname_old/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_nickname_old/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_profile/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_profile/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/set_thread_privacy/_api.py` & `aiotieba-4.4.4/aiotieba/api/set_thread_privacy/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/sign_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/sign_forum/_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     request = http_core.pack_form_request(
         yarl.URL.build(scheme=APP_SECURE_SCHEME, host=APP_BASE_HOST, path="/c/c/forum/sign"), data
     )
 
     body = await http_core.net_core.send_request(request, read_bufsize=2 * 1024)
     parse_body(body)
 
-    return BoolResponse
+    return BoolResponse()
```

### Comparing `aiotieba-4.4.3/aiotieba/api/sign_growth/_api.py` & `aiotieba-4.4.4/aiotieba/api/sign_growth/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/sync/_api.py` & `aiotieba-4.4.4/aiotieba/api/sync/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/_api.py` & `aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/_classdef.py` & `aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/_classdef.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidReqIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidReqIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidResIdl_pb2.py` & `aiotieba-4.4.4/aiotieba/api/tieba_uid2user_info/protobuf/GetUserByTiebaUidResIdl_pb2.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/top/_api.py` & `aiotieba-4.4.4/aiotieba/api/top/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/unblock/_api.py` & `aiotieba-4.4.4/aiotieba/api/unblock/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/undislike_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/undislike_forum/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/unfollow_forum/_api.py` & `aiotieba-4.4.4/aiotieba/api/unfollow_forum/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/unfollow_user/_api.py` & `aiotieba-4.4.4/aiotieba/api/unfollow_user/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/api/ungood/_api.py` & `aiotieba-4.4.4/aiotieba/api/ungood/_api.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/client.py` & `aiotieba-4.4.4/aiotieba/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,16 @@
 
     @property
     def account(self) -> Account:
         return self._http_core.account
 
     @account.setter
     def account(self, new_account: Account) -> None:
-        self._http_core.account = new_account
-        self._ws_core.account = new_account
+        self._http_core.set_account(new_account)
+        self._ws_core.set_account(new_account)
 
     @handle_exception(BoolResponse)
     async def init_websocket(self) -> BoolResponse:
         """
         初始化websocket
 
         Returns:
@@ -1265,14 +1265,17 @@
 
         Args:
             fname_or_fid (str | int): 目标贴吧名或fid 优先贴吧名
             pn (int, optional): 页码. Defaults to 1.
 
         Returns:
             MemberUsers: 最新关注用户列表
+
+        Note:
+            本接口需要STOKEN
         """
 
         fname = fname_or_fid if isinstance(fname_or_fid, str) else await self.__get_fname(fname_or_fid)
 
         return await get_member_users.request(self._http_core, fname, pn)
 
     @handle_exception(get_rank_forums.RankForums)
@@ -1363,14 +1366,17 @@
             search_type (BawuSearchType, optional): 搜索类型. Defaults to BawuSearchType.USER.
             start_dt (datetime.datetime, optional): 搜索的起始时间(含). Defaults to None.
             end_dt (datetime.datetime, optional): 搜索的结束时间(含). Defaults to None.
             op_type (int, optional): 搜索操作类型. Defaults to 0.
 
         Returns:
             Userlogs: 吧务用户管理日志表
+
+        Note:
+            本接口需要STOKEN
         """
 
         fname = fname_or_fid if isinstance(fname_or_fid, str) else await self.__get_fname(fname_or_fid)
 
         return await get_bawu_userlogs.request(
             self._http_core, fname, pn, search_value, search_type, start_dt, end_dt, op_type
         )
@@ -1398,14 +1404,17 @@
             search_type (BawuSearchType, optional): 搜索类型. Defaults to BawuSearchType.USER.
             start_dt (datetime.datetime, optional): 搜索的起始时间(含). Defaults to None.
             end_dt (datetime.datetime, optional): 搜索的结束时间(含). Defaults to None.
             op_type (int, optional): 搜索操作类型. Defaults to 0.
 
         Returns:
             Postlogs: 吧务帖子管理日志表
+
+        Note:
+            本接口需要STOKEN
         """
 
         fname = fname_or_fid if isinstance(fname_or_fid, str) else await self.__get_fname(fname_or_fid)
 
         return await get_bawu_postlogs.request(
             self._http_core, fname, pn, search_value, search_type, start_dt, end_dt, op_type
         )
@@ -1440,14 +1449,17 @@
 
         Args:
             fname_or_fid (str | int): 目标贴吧的贴吧名或fid 优先贴吧名
             pn (int, optional): 页码. Defaults to 1.
 
         Returns:
             BlacklistUsers: 吧务黑名单列表
+
+        Note:
+            本接口需要STOKEN
         """
 
         fname = fname_or_fid if isinstance(fname_or_fid, str) else await self.__get_fname(fname_or_fid)
 
         return await get_bawu_blacklist.request(self._http_core, fname, pn)
 
     @handle_exception(get_statistics.Statistics)
```

### Comparing `aiotieba-4.4.3/aiotieba/config.py` & `aiotieba-4.4.4/aiotieba/config.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/core/account.py` & `aiotieba-4.4.4/aiotieba/core/account.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/core/http.py` & `aiotieba-4.4.4/aiotieba/core/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     net_core: NetCore
     app: HttpContainer
     app_proto: HttpContainer
     web: HttpContainer
     loop: asyncio.AbstractEventLoop
 
     def __init__(self, account: Account, net_core: NetCore, loop: Optional[asyncio.AbstractEventLoop] = None) -> None:
-        self.account = account
         self.net_core = net_core
         self.loop = loop
 
         from aiohttp import hdrs
 
         app_headers = {
             hdrs.USER_AGENT: f"aiotieba/{__version__}",
@@ -68,20 +67,26 @@
         web_headers = {
             hdrs.USER_AGENT: f"aiotieba/{__version__}",
             hdrs.ACCEPT_ENCODING: "gzip, deflate",
             hdrs.CACHE_CONTROL: "no-cache",
             hdrs.CONNECTION: "keep-alive",
         }
         self.web = HttpContainer(web_headers, aiohttp.CookieJar(loop=loop))
+
+        self.set_account(account)
+
+    def set_account(self, new_account: Account) -> None:
+        self.account = new_account
+
         BDUSS_morsel = aiohttp.cookiejar.Morsel()
-        BDUSS_morsel.set('BDUSS', account.BDUSS, account.BDUSS)
+        BDUSS_morsel.set('BDUSS', new_account.BDUSS, new_account.BDUSS)
         BDUSS_morsel['domain'] = "baidu.com"
         self.web.cookie_jar._cookies[("baidu.com", "/")]['BDUSS'] = BDUSS_morsel
         STOKEN_morsel = aiohttp.cookiejar.Morsel()
-        STOKEN_morsel.set('STOKEN', account.STOKEN, account.STOKEN)
+        STOKEN_morsel.set('STOKEN', new_account.STOKEN, new_account.STOKEN)
         STOKEN_morsel['domain'] = "tieba.baidu.com"
         self.web.cookie_jar._cookies[("tieba.baidu.com", "/")]['STOKEN'] = STOKEN_morsel
 
     def pack_form_request(self, url: yarl.URL, data: List[Tuple[str, str]]) -> aiohttp.ClientRequest:
         """
         自动签名参数元组列表
         并将其打包为移动端表单请求
```

### Comparing `aiotieba-4.4.3/aiotieba/core/net.py` & `aiotieba-4.4.4/aiotieba/core/net.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/core/websocket.py` & `aiotieba-4.4.4/aiotieba/core/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,24 +273,27 @@
     websocket: aiohttp.ClientWebSocketResponse
     ws_dispatcher: asyncio.Task
     mid_manager: MsgIDManager
     _status: WsStatus
     loop: asyncio.AbstractEventLoop
 
     def __init__(self, account: Account, net_core: NetCore, loop: asyncio.AbstractEventLoop) -> None:
-        self.account = account
+        self.set_account(account)
         self.net_core = net_core
         self.loop = loop
 
         self.callbacks: Dict[int, TypeWebsocketCallback] = {}
         self.websocket: aiohttp.ClientWebSocketResponse = None
         self.ws_dispatcher: asyncio.Task = None
 
         self._status = WsStatus.CLOSED
 
+    def set_account(self, new_account: Account) -> None:
+        self.account = new_account
+
     async def connect(self) -> None:
         """
         建立weboscket连接
 
         Raises:
             aiohttp.WSServerHandshakeError: websocket握手失败
         """
```

### Comparing `aiotieba-4.4.3/aiotieba/enums.py` & `aiotieba-4.4.4/aiotieba/enums.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/exception.py` & `aiotieba-4.4.4/aiotieba/exception.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/cache.py` & `aiotieba-4.4.4/aiotieba/helper/cache.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/crypto.pyi` & `aiotieba-4.4.4/aiotieba/helper/crypto/crypto.pyi`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/base32/base32.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/base32/base32.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/crc/crc32.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/crc/crc32.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/LICENSE` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/alignment.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/alignment.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/common.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/common.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/md5.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/md5.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/private_access.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/private_access.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/mbedtls/sha1.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/mbedtls/sha1.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/rapidjson/itoa.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/rapidjson/itoa.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/const.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/const.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/tbcrypto/cuid.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/tbcrypto/cuid.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/xxHash/LICENSE` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/xxHash/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/include/xxHash/xxhash.h` & `aiotieba-4.4.4/aiotieba/helper/crypto/include/xxHash/xxhash.h`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/base32/base32.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/base32/base32.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/crc/crc32.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/crc/crc32.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/mbedtls/md5.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/mbedtls/md5.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/mbedtls/sha1.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/mbedtls/sha1.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/cuid.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/cuid.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/lib.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/lib.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/rc442.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/rc442.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/crypto/src/tbcrypto/sign.c` & `aiotieba-4.4.4/aiotieba/helper/crypto/src/tbcrypto/sign.c`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/helper/utils.py` & `aiotieba-4.4.4/aiotieba/helper/utils.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/aiotieba/logging.py` & `aiotieba-4.4.4/aiotieba/logging.py`

 * *Files identical despite different names*

### Comparing `aiotieba-4.4.3/pyproject.toml` & `aiotieba-4.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aiotieba"
-version = "4.4.3"
+version = "4.4.4"
 description = "Asynchronous I/O Client for Baidu Tieba"
 authors = [{ name = "Starry-OvO", email = "starry.qvq@gmail.com" }]
 urls = { Repository = "https://github.com/Starry-OvO/aiotieba/", Documentation = "https://aiotieba.cc/" }
 readme = "README.md"
 keywords = ["baidu", "tieba"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -54,15 +54,15 @@
   "uvloop>=0.15.0,<1.0;python_version=='3.9' and sys_platform!='win32'",
   "uvloop>=0.16.0,<1.0;python_version=='3.10' and sys_platform!='win32'",
   "uvloop>=0.17.0,<1.0;python_version=='3.11' and sys_platform!='win32'",
   "uvloop>=0.18.0,<1.0;python_version>='3.12' and sys_platform!='win32'",
 ]
 
 [build-system]
-requires = ["scikit-build-core<0.9,>=0.8"]
+requires = ["scikit-build-core<0.10,>=0.8"]
 build-backend = "scikit_build_core.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
   "aiotieba[speedup]",
   "pytest==8.1.1",
```

### Comparing `aiotieba-4.4.3/PKG-INFO` & `aiotieba-4.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aiotieba
-Version: 4.4.3
+Version: 4.4.4
 Summary: Asynchronous I/O Client for Baidu Tieba
-Keywords: baidu tieba
+Keywords: baidu,tieba
 Author-Email: Starry-OvO <starry.qvq@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: aiotieba Version: 4.4.3 Summary: Asynchronous I/
-O Client for Baidu Tieba Keywords: baidu tieba Author-Email: Starry-OvO
+Metadata-Version: 2.1 Name: aiotieba Version: 4.4.4 Summary: Asynchronous I/
+O Client for Baidu Tieba Keywords: baidu,tieba Author-Email: Starry-OvO
 gmail.com> Classifier: Development Status :: 4 - Beta Classifier: Framework ::
 AsyncIO Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: The Unlicense (Unlicense) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
```

