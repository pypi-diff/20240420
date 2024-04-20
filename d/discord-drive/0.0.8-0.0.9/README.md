# Comparing `tmp/discord_drive-0.0.8.tar.gz` & `tmp/discord_drive-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_drive-0.0.8.tar", last modified: Tue Apr 16 17:54:49 2024, max compression
+gzip compressed data, was "discord_drive-0.0.9.tar", last modified: Tue Apr 16 21:32:29 2024, max compression
```

## Comparing `discord_drive-0.0.8.tar` & `discord_drive-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 17:54:49.389652 discord_drive-0.0.8/
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     1081 2024-01-30 22:16:40.000000 discord_drive-0.0.8/LICENSE.md
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2641 2024-04-16 17:54:49.378653 discord_drive-0.0.8/PKG-INFO
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     3169 2024-04-16 17:41:53.000000 discord_drive-0.0.8/README.md
-drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 17:54:49.252813 discord_drive-0.0.8/discord_drive/
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       44 2024-04-16 17:00:50.000000 discord_drive-0.0.8/discord_drive/__init__.py
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)    24580 2024-04-16 17:00:50.000000 discord_drive-0.0.8/discord_drive/_discord_drive.py
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)    14199 2024-04-16 17:50:09.000000 discord_drive-0.0.8/discord_drive/_drive.py
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      241 2024-04-16 17:00:50.000000 discord_drive-0.0.8/discord_drive/_utils.py
-drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 17:54:49.368538 discord_drive-0.0.8/discord_drive.egg-info/
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2641 2024-04-16 17:54:49.000000 discord_drive-0.0.8/discord_drive.egg-info/PKG-INFO
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      319 2024-04-16 17:54:49.000000 discord_drive-0.0.8/discord_drive.egg-info/SOURCES.txt
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        1 2024-04-16 17:54:49.000000 discord_drive-0.0.8/discord_drive.egg-info/dependency_links.txt
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      120 2024-04-16 17:54:49.000000 discord_drive-0.0.8/discord_drive.egg-info/requires.txt
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       14 2024-04-16 17:54:49.000000 discord_drive-0.0.8/discord_drive.egg-info/top_level.txt
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       38 2024-04-16 17:54:49.390654 discord_drive-0.0.8/setup.cfg
--rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2847 2024-04-16 17:54:41.000000 discord_drive-0.0.8/setup.py
+drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 21:32:29.087315 discord_drive-0.0.9/
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     1081 2024-01-30 22:16:40.000000 discord_drive-0.0.9/LICENSE.md
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2641 2024-04-16 21:32:29.080319 discord_drive-0.0.9/PKG-INFO
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     3169 2024-04-16 17:41:53.000000 discord_drive-0.0.9/README.md
+drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 21:32:28.919443 discord_drive-0.0.9/discord_drive/
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       44 2024-04-16 17:00:50.000000 discord_drive-0.0.9/discord_drive/__init__.py
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)    24834 2024-04-16 21:28:32.000000 discord_drive-0.0.9/discord_drive/_discord_drive.py
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)    14575 2024-04-16 21:30:26.000000 discord_drive-0.0.9/discord_drive/_drive.py
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      289 2024-04-16 21:17:08.000000 discord_drive-0.0.9/discord_drive/_utils.py
+drwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        0 2024-04-16 21:32:29.072310 discord_drive-0.0.9/discord_drive.egg-info/
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2641 2024-04-16 21:32:28.000000 discord_drive-0.0.9/discord_drive.egg-info/PKG-INFO
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      319 2024-04-16 21:32:28.000000 discord_drive-0.0.9/discord_drive.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)        1 2024-04-16 21:32:28.000000 discord_drive-0.0.9/discord_drive.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)      120 2024-04-16 21:32:28.000000 discord_drive-0.0.9/discord_drive.egg-info/requires.txt
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       14 2024-04-16 21:32:28.000000 discord_drive-0.0.9/discord_drive.egg-info/top_level.txt
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)       38 2024-04-16 21:32:29.088315 discord_drive-0.0.9/setup.cfg
+-rwxrwxrwx   0 thedomino1313  (1000) thedomino1313  (1000)     2847 2024-04-16 21:19:43.000000 discord_drive-0.0.9/setup.py
```

### Comparing `discord_drive-0.0.8/LICENSE.md` & `discord_drive-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.8/PKG-INFO` & `discord_drive-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord_drive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Use Google Drive via Discord!
 Home-page: https://github.com/thedomino1313/DiscordDrive
 Author: Ryan Karch, Dominic Beyer
 Author-email: 
 License: MIT
 Keywords: Discord,Google Drive
 Description-Content-Type: text/markdown
```

### Comparing `discord_drive-0.0.8/README.md` & `discord_drive-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.8/discord_drive/_discord_drive.py` & `discord_drive-0.0.9/discord_drive/_discord_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from discord.ext.commands import has_permissions, MissingPermissions
 from discord.ext.pages import Paginator, Page
 from mimetypes import guess_extension
 from pprint import pprint
 from typing import List
 
 from ._drive import DriveAPI
+from ._utils import empty_dir
 
 class DriveAPICommands(discord.ext.commands.Cog):
     
     _drive_state = defaultdict(lambda: defaultdict(id=None, folders=[], files=[]))
     _wd_cache = None
     
 
@@ -301,19 +302,24 @@
             if timeout != float("inf"):
                 await ctx.send_followup(embed=embed, delete_after=timeout)
                 await sleep(timeout)
                 self.API.revoke_sharing(file[file.index("file/d/")+7:-19])
             else:
                 await ctx.send_followup(embed=embed)
         else:
-            embed.add_field(name="Download the attached file!", value=f"File expires {('<t:' + str(int(time() + timeout)) + ':R>') if timeout != float('inf') else 'never'}.", inline=True)
-            if timeout != float("inf"):
-                await ctx.send_followup(embed=embed, file=file, delete_after=timeout)
-            else:
-                await ctx.send_followup(embed=embed, file=file)
+            @DriveAPI._temp_dir_async("temp")
+            async def send_file():
+                embed.add_field(name="Download the attached file!", value=f"File expires {('<t:' + str(int(time() + timeout)) + ':R>') if timeout != float('inf') else 'never'}.", inline=True)
+                if timeout != float("inf"):
+                    await ctx.send_followup(embed=embed, file=file, delete_after=timeout)
+                else:
+                    await ctx.send_followup(embed=embed, file=file)
+                file.close()
+
+            await send_file()
                 
     @discord.ext.commands.slash_command(name="share", description="Share a file from your current working directory")
     async def share(
         self, 
         ctx: discord.ApplicationContext, 
         name: discord.Option(str, "Pick a file", autocomplete=discord.utils.basic_autocomplete(_get_files)), # type: ignore
         user: discord.SlashCommandOptionType.user,
@@ -364,14 +370,16 @@
             
             embed.add_field(name="Download the attached file!", value=f"File expires {('<t:' + str(int(time() + timeout)) + ':R>') if timeout != float('inf') else 'never'}.", inline=True)
             if timeout != float("inf"):
                 # await user.send(embed=embed, ephemeral=True)
                 await user.send(embed=embed, file=file, delete_after=timeout)
             else:
                 await user.send(embed=embed, file=file)
+            file.close()
+            empty_dir("temp")
         
     
     @discord.ext.commands.slash_command(name="mkdir", description="Make a new folder in your current working directory")
     @has_permissions(administrator=True)
     async def mkdir(self, ctx: discord.ApplicationContext, folder_name: discord.SlashCommandOptionType.string):
 
         if not await self._API_ready(ctx):
```

### Comparing `discord_drive-0.0.8/discord_drive/_drive.py` & `discord_drive-0.0.9/discord_drive/_drive.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,42 +43,54 @@
                 if arg in annotations:
                     assert isinstance(kwargs[arg], annotations[arg]), f"Argument '{arg}' is not of the type '{str(annotations[arg])[8:-2]}'."
             return func(self, *args, **kwargs)    
         return _validate
     
     def _temp_dir_async(path):
         def _temp_decorator(func):
-            async def _temp_manager(self, *args, **kwargs):
+            async def _temp_manager(*args, **kwargs):
                 """Wraps an asynchronous functon. Creates an empty temporary directory before the function,
                 calls the function, and then clears and removes the temporary directory.
                 """
                 if not os.path.exists(path):
                     os.mkdir(path)
                 else:
+                    try:
+                        empty_dir(path)
+                    except Exception as e:
+                        pass
+                ret = await func(*args, **kwargs)
+                try:
                     empty_dir(path)
-                ret = await func(self, *args, **kwargs)
-                empty_dir(path)
-                os.rmdir(path)
+                    os.rmdir(path)
+                except Exception as e:
+                    pass
                 return ret
             return _temp_manager
         return _temp_decorator
     
     def _temp_dir(path):
         def _temp_decorator(func):
-            def _temp_manager(self, *args, **kwargs):
+            def _temp_manager(*args, **kwargs):
                 """Wraps a synchronous functon. Creates an empty temporary directory before the function,
                 calls the function, and then clears and removes the temporary directory.
                 """
                 if not os.path.exists(path):
                     os.mkdir(path)
                 else:
+                    try:
+                        empty_dir(path)
+                    except Exception as e:
+                        pass
+                ret = func(*args, **kwargs)
+                try:
                     empty_dir(path)
-                ret = func(self, *args, **kwargs)
-                empty_dir(path)
-                os.rmdir(path)
+                    os.rmdir(path)
+                except Exception as e:
+                    pass
                 return ret
             return _temp_manager
         return _temp_decorator
 
 
     @_input_validator
     def __init__(self, root:str):
```

### Comparing `discord_drive-0.0.8/discord_drive.egg-info/PKG-INFO` & `discord_drive-0.0.9/discord_drive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord_drive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Use Google Drive via Discord!
 Home-page: https://github.com/thedomino1313/DiscordDrive
 Author: Ryan Karch, Dominic Beyer
 Author-email: 
 License: MIT
 Keywords: Discord,Google Drive
 Description-Content-Type: text/markdown
```

### Comparing `discord_drive-0.0.8/setup.py` & `discord_drive-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 `/pwd`: Shows the caller the file path of their current directory.\\
 `/share <file> <user> <timeout (optional)>`: Sends a specified server member a dm with a file from the caller's current directory. Files and users have autocomplete. Timeout defaults to 60 seconds, where the file will then no longer be allowed to be downloaded.\\
 `/upload <attachment>`: Uploads a file or zip file to the caller's current directory. Zip files must contain just the files, and no folders, as they will not be read.
 """
 
 setup(
     name='discord_drive',
-    version='0.0.8',
+    version='0.0.9',
     description='Use Google Drive via Discord!',
     license='MIT',
     packages=['discord_drive'],
     author='Ryan Karch, Dominic Beyer',
     author_email='',
     keywords=['Discord', 'Google Drive'],
     url='https://github.com/thedomino1313/DiscordDrive',
```

