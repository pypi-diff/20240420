# Comparing `tmp/aiavatar-0.4.5-py3-none-any.whl.zip` & `tmp/aiavatar-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,28 @@
-Zip file size: 28640 bytes, number of entries: 26
--rw-r--r--  2.0 unx      438 b- defN 24-Apr-14 09:42 aiavatar/__init__.py
+Zip file size: 30135 bytes, number of entries: 26
+-rw-r--r--  2.0 unx      712 b- defN 24-Apr-20 03:57 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 24-Apr-14 09:42 aiavatar/avatar.py
--rw-r--r--  2.0 unx     6841 b- defN 24-Apr-16 23:38 aiavatar/bot.py
+-rw-r--r--  2.0 unx     6840 b- defN 24-Apr-20 03:57 aiavatar/bot.py
 -rw-r--r--  2.0 unx     1771 b- defN 24-Apr-14 09:42 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx     1448 b- defN 24-Apr-14 09:42 aiavatar/animation/vrchat.py
 -rw-r--r--  2.0 unx       31 b- defN 24-Apr-14 09:42 aiavatar/device/__init__.py
--rw-r--r--  2.0 unx     2344 b- defN 24-Apr-14 09:42 aiavatar/device/audio.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-Apr-20 03:57 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx     1650 b- defN 24-Apr-14 09:42 aiavatar/face/__init__.py
 -rw-r--r--  2.0 unx     1556 b- defN 24-Apr-14 09:42 aiavatar/face/vrchat.py
--rw-r--r--  2.0 unx     6342 b- defN 24-Apr-14 09:42 aiavatar/listeners/__init__.py
+-rw-r--r--  2.0 unx     6342 b- defN 24-Apr-17 11:44 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx     2522 b- defN 24-Apr-14 09:42 aiavatar/listeners/azurevoicerequest.py
 -rw-r--r--  2.0 unx     2849 b- defN 24-Apr-14 09:42 aiavatar/listeners/azurewakeword.py
 -rw-r--r--  2.0 unx      977 b- defN 24-Apr-14 09:42 aiavatar/listeners/voicerequest.py
 -rw-r--r--  2.0 unx     1078 b- defN 24-Apr-14 09:42 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 24-Apr-14 09:42 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     6162 b- defN 24-Apr-14 09:42 aiavatar/processors/chatgpt.py
--rw-r--r--  2.0 unx     2550 b- defN 24-Apr-16 15:07 aiavatar/speech/__init__.py
+-rw-r--r--  2.0 unx     2550 b- defN 24-Apr-20 04:12 aiavatar/speech/__init__.py
 -rw-r--r--  2.0 unx     1887 b- defN 24-Apr-16 15:34 aiavatar/speech/azurespeech.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-16 15:07 aiavatar/speech/voicevox.py
+-rw-r--r--  2.0 unx     1202 b- defN 24-Apr-20 04:35 aiavatar/speech/voicevox.py
 -rw-r--r--  2.0 unx      220 b- defN 24-Apr-16 15:07 aiavatar/speech/soundplayers/__init__.py
--rw-r--r--  2.0 unx     2319 b- defN 24-Apr-16 15:07 aiavatar/speech/soundplayers/sounddevice_player.py
--rw-r--r--  2.0 unx    11324 b- defN 24-Apr-16 23:41 aiavatar-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    12620 b- defN 24-Apr-16 23:41 aiavatar-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 23:41 aiavatar-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-16 23:41 aiavatar-0.4.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2196 b- defN 24-Apr-16 23:41 aiavatar-0.4.5.dist-info/RECORD
-26 files, 76467 bytes uncompressed, 25088 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx     2145 b- defN 24-Apr-20 04:04 aiavatar/speech/soundplayers/sounddevice_player.py
+-rw-r--r--  2.0 unx    11324 b- defN 24-Apr-20 04:36 aiavatar-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18757 b- defN 24-Apr-20 04:36 aiavatar-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 04:36 aiavatar-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-20 04:36 aiavatar-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2196 b- defN 24-Apr-20 04:36 aiavatar-0.5.0.dist-info/RECORD
+26 files, 81695 bytes uncompressed, 26583 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -57,23 +57,23 @@
 
 Filename: aiavatar/speech/soundplayers/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/soundplayers/sounddevice_player.py
 Comment: 
 
-Filename: aiavatar-0.4.5.dist-info/LICENSE
+Filename: aiavatar-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.4.5.dist-info/METADATA
+Filename: aiavatar-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.4.5.dist-info/WHEEL
+Filename: aiavatar-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.4.5.dist-info/top_level.txt
+Filename: aiavatar-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.4.5.dist-info/RECORD
+Filename: aiavatar-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/__init__.py

```diff
@@ -1,7 +1,16 @@
+import logging
+
+logger = logging.getLogger("aiavatar")
+logger.setLevel(logging.INFO)
+log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
+streamHandler = logging.StreamHandler()
+streamHandler.setFormatter(log_format)
+logger.addHandler(streamHandler)
+
 # Device
 from .device import AudioDevice
 # Processor
 from .processors.chatgpt import ChatGPTProcessor
 # Listener
 from .listeners import WakewordListenerBase
 from .listeners import RequestListenerBase
```

## aiavatar/bot.py

```diff
@@ -1,136 +1,140 @@
 import asyncio
 from logging import getLogger, NullHandler
 import traceback
-from typing import Callable
 # Device
 from .device import AudioDevice
 # Processor
+from .processors import ChatProcessor
 from .processors.chatgpt import ChatGPTProcessor
 # Listener
-from .listeners import RequestListenerBase
-from .listeners.voicerequest import VoiceRequestListener
+from .listeners.voicerequest import VoiceRequestListener, RequestListenerBase
+from .listeners.wakeword import WakewordListener, WakewordListenerBase
 # Avatar
+from .speech import SpeechController
 from .speech.voicevox import VoicevoxSpeechController
 from .animation import AnimationController, AnimationControllerDummy
 from .face import FaceController, FaceControllerDummy
 from .avatar import AvatarController
 
+logger = getLogger(__name__)
+logger.addHandler(NullHandler())
+
+
 class AIAvatar:
     def __init__(
         self,
         *,
-        # AI
-        openai_api_key: str,
-        model: str="gpt-3.5-turbo",
-        functions: dict=None,
-        system_message_content: str=None,
-        # Speech-to-Text
+        openai_api_key: str=None,
         google_api_key: str=None,
-        volume_threshold: int=3000,
-        request_listener: RequestListenerBase=None,
-        # Text-to-Speech
-        voicevox_url: str,
+        model: str=None,
+        system_message_content: str=None,
         voicevox_speaker_id: int=46,
-        # Audio device
         input_device: int=-1,
         output_device: int=-1,
-        # Avatar
+        audio_devices: AudioDevice=None,
+        chat_processor: ChatProcessor=None,
+        request_listener: RequestListenerBase=None,
+        wakeword_listener: WakewordListenerBase=None,
+        speech_controller: SpeechController=None,
         animation_controller: AnimationController=None,
         face_controller: FaceController=None,
-        avatar_request_parser: Callable=None,
-        # Chat
-        start_voice: str="どうしたの",
-        split_chars: list=None
+        wakewords: list=None,
+        start_voice: str=None,
+        split_chars: list=None,
+        language: str="ja-JP",
+        verbose: bool=False
     ):
-
-        self.logger = getLogger(__name__)
-        self.logger.addHandler(NullHandler())
-
         # Audio Devices
-        if isinstance(input_device, int):
-            if input_device < 0:
-                input_device_info = AudioDevice.get_default_input_device_info()
-                input_device = input_device_info["index"]
-            else:
-                input_device_info = AudioDevice.get_device_info(input_device)
-        elif isinstance(input_device, str):
-            input_device_info = AudioDevice.get_input_device_by_name(input_device)
-            if input_device_info is None:
-                input_device_info = AudioDevice.get_default_input_device_info()
-            input_device = input_device_info["index"]
-
-        self.input_device = input_device
-        self.logger.info(f"Input device: [{input_device}] {input_device_info['name']}")
-
-        if isinstance(output_device, int):
-            if output_device < 0:
-                output_device_info = AudioDevice.get_default_output_device_info()
-                output_device = output_device_info["index"]
-            else:
-                output_device_info = AudioDevice.get_device_info(output_device)
-        elif isinstance(output_device, str):
-            output_device_info = AudioDevice.get_output_device_by_name(output_device)
-            if output_device_info is None:
-                output_device_info = AudioDevice.get_default_output_device_info()
-            output_device = output_device_info["index"]
-
-        self.output_device = output_device
-        self.logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
-
-        # Processor
-        self.openai_api_key = openai_api_key
-        self.chat_processor = ChatGPTProcessor(api_key=self.openai_api_key, model=model, functions=functions, system_message_content=system_message_content)
-
-        # Listeners
-        self.google_api_key = google_api_key
-        self.volume_threshold = volume_threshold
-        self.request_listener = request_listener or VoiceRequestListener(self.google_api_key, volume_threshold=volume_threshold, device_index=self.input_device)
-
-        # Speech
-        self.voicevox_url = voicevox_url
-        self.voicevox_speaker_id = voicevox_speaker_id
-        speech_controller = VoicevoxSpeechController(self.voicevox_url, self.voicevox_speaker_id, device_index=self.output_device)
-
-        # Avatar
-        animation_controller = animation_controller or AnimationControllerDummy()
-        face_controller = face_controller or FaceControllerDummy()
-        self.avatar_controller = AvatarController(speech_controller, animation_controller, face_controller, avatar_request_parser)
+        if audio_devices:
+            self.audio_devices = audio_devices
+        else:
+            self.audio_devices = AudioDevice(input_device, output_device)
+        logger.info(f"Input device: [{self.audio_devices.input_device}] {self.audio_devices.input_device_info['name']}")
+        logger.info(f"Output device: [{self.audio_devices.output_device}] {self.audio_devices.output_device_info['name']}")
+
+        # Chat Processor
+        if chat_processor:
+            self.chat_processor = chat_processor
+        else:
+            self.chat_processor = ChatGPTProcessor(
+                api_key=openai_api_key,
+                model=model or "gpt-3.5-turbo",
+                system_message_content=system_message_content
+            )
+
+        # Request Listener
+        if request_listener:
+            self.request_listener = request_listener
+        else:
+            self.request_listener = VoiceRequestListener(
+                google_api_key,
+                volume_threshold=2000,
+                device_index=self.audio_devices.input_device,
+                lang=language
+            )
+        
+        # Wakeword Listener
+        if wakeword_listener:
+            self.wakeword_listener = wakeword_listener
+        else:
+            async def _on_wakeword(text):
+                await self.start_chat(request_on_start=text, skip_start_voice=start_voice is None)
+
+            self.wakeword_listener = WakewordListener(
+                api_key=google_api_key,
+                wakewords=wakewords or ["こんにちは" if language == "ja-JP" else "Hello"],
+                on_wakeword=_on_wakeword,
+                volume_threshold=2000,
+                device_index=self.audio_devices.input_device,
+                lang=language,
+                verbose=verbose
+            )
+        
+        # Avatar Controller with Speech, Animation and Face
+        self.avatar_controller = AvatarController(
+            speech_controller or VoicevoxSpeechController(
+                base_url="http://127.0.0.1:50021",
+                speaker_id=voicevox_speaker_id,
+                device_index=self.audio_devices.output_device
+            ),
+            animation_controller or AnimationControllerDummy(verbose=verbose),
+            face_controller or FaceControllerDummy(verbose=verbose)
+        )
 
         # Chat
-        self.chat_task = None
         self.start_voice = start_voice
         self.split_chars = split_chars or ["。", "、", "？", "！", ".", ",", "?", "!"]
-
         self.on_turn_end = self.on_turn_end_default
+        self.chat_task = None
 
     async def on_turn_end_default(self, request_text: str, response_text: str) -> bool:
         return False
 
     async def chat(self, request_on_start: str=None, skip_start_voice: bool=False):
         if not skip_start_voice:
             try:
                 await self.avatar_controller.speech_controller.speak(self.start_voice)
             except Exception as ex:
-                self.logger.error(f"Error at starting chat: {str(ex)}\n{traceback.format_exc()}")
+                logger.error(f"Error at starting chat: {str(ex)}\n{traceback.format_exc()}")
 
         while True:
             request_text = ""
             response_text = ""
             try:
                 if request_on_start:
                     request_text = request_on_start
                     request_on_start = None
                 else:
                     request_text = await self.request_listener.get_request()
                     if not request_text:
                         break
 
-                self.logger.info(f"User: {request_text}")
-                self.logger.info("AI:")
+                logger.info(f"User: {request_text}")
+                logger.info("AI:")
 
                 avatar_task = asyncio.create_task(self.avatar_controller.start())
 
                 stream_buffer = ""
                 async for t in self.chat_processor.chat(request_text):
                     stream_buffer += t
                     for spc in self.split_chars:
@@ -147,21 +151,28 @@
                     self.avatar_controller.set_text(stream_buffer)
                     response_text += stream_buffer
 
                 self.avatar_controller.set_stop()
                 await avatar_task
             
             except Exception as ex:
-                self.logger.error(f"Error at chatting loop: {str(ex)}\n{traceback.format_exc()}")
+                logger.error(f"Error at chatting loop: {str(ex)}\n{traceback.format_exc()}")
 
             finally:
                 if await self.on_turn_end(request_text, response_text):
                     break
 
     async def start_chat(self, request_on_start: str=None, skip_start_voice: bool=False):
         self.stop_chat()
         self.chat_task = asyncio.create_task(self.chat(request_on_start, skip_start_voice))
         await self.chat_task
 
     def stop_chat(self):
         if self.chat_task is not None:
             self.chat_task.cancel()
+
+    def start_listening_wakeword(self, wait: bool=True):
+        ww_thread = self.wakeword_listener.start()
+        if wait:
+            ww_thread.join()
+        else:
+            return ww_thread
```

## aiavatar/device/audio.py

```diff
@@ -1,10 +1,41 @@
 import sounddevice
 
 class AudioDevice:
+    def __init__(self, input_device: int=-1, output_device: int=-1):
+        if isinstance(input_device, int):
+            if input_device < 0:
+                input_device_info = self.get_default_input_device_info()
+                input_device = input_device_info["index"]
+            else:
+                input_device_info = self.get_device_info(input_device)
+        elif isinstance(input_device, str):
+            input_device_info = self.get_input_device_by_name(input_device)
+            if input_device_info is None:
+                input_device_info = self.get_default_input_device_info()
+            input_device = input_device_info["index"]
+
+        self.input_device = input_device
+        self.input_device_info = input_device_info
+
+        if isinstance(output_device, int):
+            if output_device < 0:
+                output_device_info = self.get_default_output_device_info()
+                output_device = output_device_info["index"]
+            else:
+                output_device_info = self.get_device_info(output_device)
+        elif isinstance(output_device, str):
+            output_device_info = self.get_output_device_by_name(output_device)
+            if output_device_info is None:
+                output_device_info = self.get_default_output_device_info()
+            output_device = output_device_info["index"]
+
+        self.output_device = output_device
+        self.output_device_info = output_device_info
+
     @classmethod
     def get_default_input_device_info(cls):
         device_list = sounddevice.query_devices()
         for idx in sounddevice.default.device:
             if device_list[idx]["max_input_channels"] > 0:
                 return device_list[idx]
```

## aiavatar/speech/voicevox.py

```diff
@@ -1,85 +1,14 @@
 import aiohttp
-import asyncio
-import io
-from logging import getLogger, NullHandler
-import traceback
-import wave
-import numpy
-import sounddevice
-from . import SpeechController, SpeechControllerBase
+from . import SpeechControllerBase, VoiceClip
 from .soundplayers import SoundPlayerBase
 
 
-class VoiceClip:
-    def __init__(self, text: str):
-        self.text = text
-        self.download_task = None
-        self.audio_clip = None
-
-
-class VoicevoxSpeechController(SpeechController):
-    def __init__(self, base_url: str, speaker_id: int, device_index: int=-1, playback_margin: float=0.1):
-        self.logger = getLogger(__name__)
-        self.logger.addHandler(NullHandler())
-
-        self.base_url = base_url
-        self.speaker_id = speaker_id
-        self.device_index = device_index
-        self.playback_margin = playback_margin
-        self.voice_clips = {}
-        self._is_speaking = False
-
-    async def download(self, voice: VoiceClip):
-        params = {"speaker": self.speaker_id, "text": voice.text}
-        async with aiohttp.ClientSession() as session:
-            async with session.post(self.base_url + "/audio_query", params=params) as query_resp:
-                audio_query = await query_resp.json()
-                async with session.post(self.base_url + "/synthesis", params={"speaker": self.speaker_id}, json=audio_query) as audio_resp:
-                    voice.audio_clip = await audio_resp.read()
-
-    def prefetch(self, text: str):
-        v = self.voice_clips.get(text)
-        if v:
-            return v
-
-        v = VoiceClip(text)
-        v.download_task = asyncio.create_task(self.download(v))
-        self.voice_clips[text] = v
-        return v
-
-    async def speak(self, text: str):
-        voice = self.prefetch(text)
-        
-        if not voice.audio_clip:
-            await voice.download_task
-        
-        with wave.open(io.BytesIO(voice.audio_clip), "rb") as f:
-            try:
-                self._is_speaking = True
-                data = numpy.frombuffer(
-                    f.readframes(f.getnframes()),
-                    dtype=numpy.int16
-                )
-                framerate = f.getframerate()
-                sounddevice.play(data, framerate, device=self.device_index, blocking=False)
-                await asyncio.sleep(len(data) / framerate + self.playback_margin)
-
-            except Exception as ex:
-                self.logger.error(f"Error at speaking: {str(ex)}\n{traceback.format_exc()}")
-
-            finally:
-                self._is_speaking = False
-
-    def is_speaking(self) -> bool:
-        return self._is_speaking
-
-
-class VoicevoxSpeechControllerSubProcess(SpeechControllerBase):
-    def __init__(self, *, base_url: str, speaker_id: int, device_index: int=-1, playback_margin: float=0.1, use_subprocess=True, subprocess_timeout: float=5.0, sound_player: SoundPlayerBase=None):
+class VoicevoxSpeechController(SpeechControllerBase):
+    def __init__(self, *, base_url: str, speaker_id: int, device_index: int=-1, playback_margin: float=0.1, use_subprocess=False, subprocess_timeout: float=5.0, sound_player: SoundPlayerBase=None):
         super().__init__(
             base_url=base_url,
             device_index=device_index,
             playback_margin=playback_margin,
             use_subprocess=use_subprocess,
             subprocess_timeout=subprocess_timeout,
             sound_player=sound_player
```

## aiavatar/speech/soundplayers/sounddevice_player.py

```diff
@@ -1,27 +1,20 @@
 import asyncio
 import io
 import os
-import select
 import sys
 import wave
 import numpy
 import sounddevice
 
 
 if __name__ == "__main__":
-    device_index = int(sys.argv[1]) if len(sys.argv) > 2 else 0
-    timeout = float(sys.argv[2]) if len(sys.argv) > 3 else 5.0
+    device_index = int(sys.argv[1]) if len(sys.argv) > 1 else 0
 
     try:
-        ready, _, _ = select.select([sys.stdin], [], [], timeout)
-
-        if not ready:
-            raise Exception(f"Sound timeout ({timeout}sec)")
-
         data = sys.stdin.buffer.read()
 
         if not data:
             raise Exception("No sound data")
 
         with wave.open(io.BytesIO(data), "rb") as f:
             data = numpy.frombuffer(
@@ -52,20 +45,22 @@
                     dtype=numpy.int16
                 )
                 framerate = f.getframerate()
                 sounddevice.play(data, framerate, device=self.device_index, blocking=False)
                 await asyncio.sleep(len(data) / framerate + self.playback_margin)
 
         async def play_wave_on_subprocess(self, data):
-            process = await asyncio.create_subprocess_exec(
-                "python", os.path.abspath(__file__), str(self.device_index), str(self.subprocess_timeout),
+            proc_task = asyncio.create_subprocess_exec(
+                sys.executable, os.path.abspath(__file__), str(self.device_index),
                 stdin=asyncio.subprocess.PIPE,
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.PIPE
             )
 
+            process = await asyncio.wait_for(proc_task, self.subprocess_timeout)
+
             stdout, stderr = await process.communicate(input=data)
 
             if process.returncode != 0:
                 raise Exception(stderr.decode())
 
             return stdout
```

## Comparing `aiavatar-0.4.5.dist-info/LICENSE` & `aiavatar-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.4.5.dist-info/RECORD` & `aiavatar-0.5.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-aiavatar/__init__.py,sha256=Q7dfZ9PWg6btZmfXMbOYHfo7pUy2c6ja9c84t5HJECA,438
+aiavatar/__init__.py,sha256=o_MsrBgCxbfFE8FeUCeDJpAtWcUmd0iopx9yPbQkUMg,712
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
-aiavatar/bot.py,sha256=F1lE5UAbfnv_IAqs7_-KgnVkgtKpu1Qjun8xKt0ChrY,6841
+aiavatar/bot.py,sha256=a7WRx5pVBSXgY8HyhL1FRvMlXrMWx2TTBjBpRXbYeKE,6840
 aiavatar/animation/__init__.py,sha256=aaYbs5I7vnXPEq39sJ2h7v-sG1WqfyocH4iepDSqz08,1771
 aiavatar/animation/vrchat.py,sha256=8aD3o9_NHJCiINiI-tjxF6cGevmJtvZ9IWTsixDj1Vc,1448
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
-aiavatar/device/audio.py,sha256=xxRzbjyabXGrhY3WDc3UYEadjCU-xS7HF_vcXtGiC88,2344
+aiavatar/device/audio.py,sha256=Y_91icGtl0X6mVuder1t_PGAauBryKBhFl9goiKS6KM,3790
 aiavatar/face/__init__.py,sha256=FPaP8RT8UXQ_UMON7RLvg2FUotOzTFVJ1qxzVk5zBTw,1650
 aiavatar/face/vrchat.py,sha256=VOibFm5Yuof-RQGfd1Zt1tx4v-TV9Usb8aMn7rHp5HY,1556
 aiavatar/listeners/__init__.py,sha256=-dLrr-HV2xdRaVgxv6tkohKSmHe9REKw4sriReRbv1Y,6342
 aiavatar/listeners/azurevoicerequest.py,sha256=7m7xRmkWfTgL8JjFbFOPqZvzydTllAnFipTcM1Ru7nE,2522
 aiavatar/listeners/azurewakeword.py,sha256=Z6cjUUoeXDwVaodg4I5NUNQMY1qVRpJ7Y8_ibQKx_7E,2849
 aiavatar/listeners/voicerequest.py,sha256=cvq9IN_VA0idRzC4UFwkQZ-92IYjll94-ZaijVlLTco,977
 aiavatar/listeners/wakeword.py,sha256=EyG99lS9TKblRs4gni5UwbrfBvrVRfJSOa8QtVHHcO0,1078
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=CyMpH_Nq-HtM50eFMFmOF7cJezk5x6VOHq9OxeTYFBU,6162
 aiavatar/speech/__init__.py,sha256=u013ElPBHqQ1wrh6UUxV80QyNz57BDai7IuXwU1CKcU,2550
 aiavatar/speech/azurespeech.py,sha256=P8lnUMj4j8BRnasxCxCb-xkkFA13BvHUG03aZ04RXNU,1887
-aiavatar/speech/voicevox.py,sha256=5_TIqJyymEyqG8awR5I_Tg0iq0eWwVqYW4FsFM2f75M,3656
+aiavatar/speech/voicevox.py,sha256=CsmfvvN3F7Sb_aONRsWkR4ECy_hlCE2paeDMBg-syLY,1202
 aiavatar/speech/soundplayers/__init__.py,sha256=71xYi-8qaInz_Um8wV5zDaHpAB5sTJG9osn17aQAUKQ,220
-aiavatar/speech/soundplayers/sounddevice_player.py,sha256=sppGR11l7ENsDE3qQ_spo7RnVj6D3tLEK350dt8JhVs,2319
-aiavatar-0.4.5.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.4.5.dist-info/METADATA,sha256=4RPq83eYzVkfcwefj9bCj6ggWNwLT2122I8sHfNs_tk,12620
-aiavatar-0.4.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aiavatar-0.4.5.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.4.5.dist-info/RECORD,,
+aiavatar/speech/soundplayers/sounddevice_player.py,sha256=tBHMJ5eOiM_rKkvCWlBPE0254Ro4lcNkq8XWLB2tHP8,2145
+aiavatar-0.5.0.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.5.0.dist-info/METADATA,sha256=Sd4jk9dhdZH7a3lQDfuJvNkNBSaHguunrp6c1xjvW4c,18757
+aiavatar-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aiavatar-0.5.0.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.5.0.dist-info/RECORD,,
```

