# Comparing `tmp/aiavatar-0.1.4-py3-none-any.whl.zip` & `tmp/aiavatar-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 19644 bytes, number of entries: 20
+Zip file size: 20365 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-Jun-04 12:15 aiavatar/avatar.py
--rw-r--r--  2.0 unx     5621 b- defN 23-Jun-04 16:36 aiavatar/bot.py
+-rw-r--r--  2.0 unx     5672 b- defN 23-Jun-23 10:05 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
--rw-r--r--  2.0 unx     2535 b- defN 23-Jun-03 02:13 aiavatar/device/audio.py
+-rw-r--r--  2.0 unx     2344 b- defN 23-Jun-22 03:33 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx     1650 b- defN 23-Jun-04 16:30 aiavatar/face/__init__.py
 -rw-r--r--  2.0 unx     1556 b- defN 23-Jun-04 16:30 aiavatar/face/vrchat.py
--rw-r--r--  2.0 unx     6210 b- defN 23-Jun-03 02:23 aiavatar/listeners/__init__.py
--rw-r--r--  2.0 unx      788 b- defN 23-May-24 12:01 aiavatar/listeners/voicerequest.py
--rw-r--r--  2.0 unx     1007 b- defN 23-Jun-03 02:44 aiavatar/listeners/wakeword.py
+-rw-r--r--  2.0 unx     6081 b- defN 23-Jun-23 10:01 aiavatar/listeners/__init__.py
+-rw-r--r--  2.0 unx      815 b- defN 23-Jun-23 10:01 aiavatar/listeners/voicerequest.py
+-rw-r--r--  2.0 unx     1034 b- defN 23-Jun-23 10:01 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
--rw-r--r--  2.0 unx     2151 b- defN 23-May-27 08:42 aiavatar/processors/chatgpt.py
+-rw-r--r--  2.0 unx     5177 b- defN 23-Jun-23 10:05 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
--rw-r--r--  2.0 unx     2794 b- defN 23-Jun-02 14:22 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8081 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/RECORD
-20 files, 49974 bytes uncompressed, 16992 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     2281 b- defN 23-Jun-22 03:33 aiavatar/speech/voicevox.py
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8953 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/RECORD
+20 files, 53144 bytes uncompressed, 17713 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.1.4.dist-info/LICENSE
+Filename: aiavatar-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.1.4.dist-info/METADATA
+Filename: aiavatar-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.1.4.dist-info/WHEEL
+Filename: aiavatar-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.1.4.dist-info/top_level.txt
+Filename: aiavatar-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.1.4.dist-info/RECORD
+Filename: aiavatar-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/bot.py

```diff
@@ -19,14 +19,15 @@
         self,
         google_api_key: str,
         openai_api_key: str,
         voicevox_url: str,
         voicevox_speaker_id: int=46,
         volume_threshold: int=3000,
         start_voice: str="どうしたの",
+        functions: dict=None,
         system_message_content: str=None,
         animation_controller: AnimationController=None,
         face_controller: FaceController=None,
         avatar_request_parser: Callable=None,
         input_device: int=-1,
         output_device: int=-1
     ):
@@ -68,15 +69,15 @@
                 output_device_info = AudioDevice.get_default_output_device_info()
             output_device = output_device_info["index"]
 
         self.output_device = output_device
         self.logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
 
         # Processor
-        self.chat_processor = ChatGPTProcessor(self.openai_api_key, system_message_content=system_message_content)
+        self.chat_processor = ChatGPTProcessor(self.openai_api_key, functions=functions, system_message_content=system_message_content)
 
         # Listeners
         self.request_listener = VoiceRequestListener(self.google_api_key, volume_threshold=volume_threshold, device_index=self.input_device)
 
         # Avatar
         speech_controller = VoicevoxSpeechController(self.voicevox_url, self.voicevox_speaker_id, device_index=self.output_device)
         animation_controller = animation_controller or AnimationControllerDummy()
```

## aiavatar/device/audio.py

```diff
@@ -1,79 +1,68 @@
-from pyaudio import PyAudio
+import sounddevice
 
 class AudioDevice:
     @classmethod
     def get_default_input_device_info(cls):
-        pa = PyAudio()
-        ret = pa.get_default_input_device_info()
-        pa.terminate()
-        return ret
+        device_list = sounddevice.query_devices()
+        for idx in sounddevice.default.device:
+            if device_list[idx]["max_input_channels"] > 0:
+                return device_list[idx]
 
     @classmethod
     def get_default_output_device_info(cls):
-        pa = PyAudio()
-        ret = pa.get_default_output_device_info()
-        pa.terminate()
-        return ret
+        device_list = sounddevice.query_devices()
+        for idx in sounddevice.default.device:
+            if device_list[idx]["max_output_channels"] > 0:
+                return device_list[idx]
 
     @classmethod
     def get_device_info(cls, index: int):
-        pa = PyAudio()
-        ret = pa.get_device_info_by_index(index)
-        pa.terminate()
-        return ret
+        return sounddevice.query_devices(index)
 
     @classmethod
     def get_input_device_by_name(cls, name: str):
-        for d in AudioDevice.get_audio_devices():
-            if d["maxInputChannels"] > 0:
+        for d in sounddevice.query_devices():
+            if d["max_input_channels"] > 0:
                 if name.lower() in d["name"].lower():
                     return d
         return None
 
     @classmethod
     def get_output_device_by_name(cls, name: str):
-        for d in AudioDevice.get_audio_devices():
-            if d["maxOutputChannels"] > 0:
+        for d in sounddevice.query_devices():
+            if d["max_output_channels"] > 0:
                 if name.lower() in d["name"].lower():
                     return d
         return None
 
     @classmethod
     def get_input_device_with_prompt(cls, prompt: str=None):
         print("==== Input devices ====")
-        for d in AudioDevice.get_audio_devices():
-            if d["maxInputChannels"] > 0:
+        for d in sounddevice.query_devices():
+            if d["max_input_channels"] > 0:
                 print(f'{d["index"]}: {d["name"]}')
         idx = input(prompt or "Index of microphone device (Skip to use default): ")
         if idx == "":
             return cls.get_default_input_device_info()
         else:
             return cls.get_device_info(int(idx))
 
     @classmethod
     def get_output_device_with_prompt(cls, prompt: str=None):
         print("==== Output devices ====")
-        for d in AudioDevice.get_audio_devices():
-            if d["maxOutputChannels"] > 0:
+        for d in sounddevice.query_devices():
+            if d["max_output_channels"] > 0:
                 print(f'{d["index"]}: {d["name"]}')
         idx = input(prompt or "Index of speaker device (Skip to use default): ")
         if idx == "":
             return cls.get_default_output_device_info()
         else:
             return cls.get_device_info(int(idx))
 
     @classmethod
     def get_audio_devices(cls):
-        devices = []
-        pa = PyAudio()
-        for i in range(pa.get_device_count()):
-            devices.append(pa.get_device_info_by_index(i))
-        pa.terminate()
-        return devices
+        return sounddevice.query_devices()
 
     @classmethod
     def list_audio_devices(cls):
-        devices = cls.get_audio_devices()
-        print("Available audio devices:")
-        for d in devices:
-            print(f"{d['index']}: {d['name']}")
+        print(cls.get_audio_devices())
```

## aiavatar/listeners/__init__.py

```diff
@@ -1,61 +1,58 @@
 import base64
 from logging import getLogger, NullHandler
 import numpy
 import time
 import traceback
 from typing import Callable
 import aiohttp
-import pyaudio
+import sounddevice
 
 class SpeechListenerBase:
-    def __init__(self, api_key: str, on_speech_recognized: Callable, volume_threshold: int=3000, timeout: float=1.0, detection_timeout: float=0.0, min_duration: float=0.3, max_duration: float=20.0, lang: str="ja-JP", rate: int=44100, device_index: int=-1):
+    def __init__(self, api_key: str, on_speech_recognized: Callable, volume_threshold: int=3000, timeout: float=1.0, detection_timeout: float=0.0, min_duration: float=0.3, max_duration: float=20.0, lang: str="ja-JP", rate: int=44100, channels: int=1, device_index: int=-1):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
-        self.pa = pyaudio.PyAudio()
         self.api_key = api_key
         self.on_speech_recognized = on_speech_recognized
         self.volume_threshold = volume_threshold
         self.timeout = timeout
         self.detection_timeout = detection_timeout
         self.min_duration = min_duration
         self.max_duration = max_duration
         self.lang = lang
+        self.channels = channels
         self.rate = rate
         self.device_index = device_index
         self.is_listening = False
 
     def record_audio(self, device_index) -> bytes:
         audio_data = []
 
         def callback(in_data, frame_count, time_info, status):
-            audio_data.append(in_data)
-            return (None, pyaudio.paContinue)
+            audio_data.append(in_data.copy())
 
         try:
-            stream = self.pa.open(
-                input_device_index=device_index,
-                format=pyaudio.paInt16,
-                channels=1,
-                rate=self.rate,
-                input=True,
-                stream_callback=callback
+            stream = sounddevice.InputStream(
+                channels=self.channels,
+                samplerate=self.rate,
+                dtype=numpy.int16,
+                callback=callback
             )
 
             start_time = time.time()
             is_recording = False
             silence_start_time = time.time()
             is_silent = False
             last_detected_time = time.time()
-            stream.start_stream()
+            stream.start()
 
-            while stream.is_active():
+            while stream.active:
                 current_time = time.time()
-                volume = numpy.frombuffer(b"".join(audio_data[-10:]), dtype=numpy.int16).max() if audio_data else 0
+                volume = numpy.linalg.norm(audio_data[-10:]) / 50 if audio_data else 0
 
                 if not is_recording:
                     if volume > self.volume_threshold:
                         audio_data = audio_data[-100:]  # Use 100ms data before start recording
                         is_recording = True
                         start_time = current_time
 
@@ -96,15 +93,15 @@
                     self.logger.info(f"Voice detection timeout: {self.detection_timeout}")
                     break
 
         except Exception as ex:
             self.logger.error(f"Error at record_audio: {str(ex)}\n{traceback.format_exc()}")
 
         finally:
-            stream.stop_stream()
+            stream.stop()
             stream.close()
 
         # Return empty bytes
         return b"".join([])
 
     async def transcribe(self, audio_data: list) -> str:
         audio_b64 = base64.b64encode(audio_data).decode("utf-8")
```

## aiavatar/listeners/voicerequest.py

```diff
@@ -1,12 +1,12 @@
 from . import SpeechListenerBase
 
 class VoiceRequestListener(SpeechListenerBase):
-    def __init__(self, api_key: str, volume_threshold: int=3000, timeout: float=1.0, detection_timeout: float=10.0, min_duration: float=0.3, max_duration: float=20.0, lang: str="ja-JP", rate: int=44100, device_index: int=-1):
-        super().__init__(api_key, self.on_request, volume_threshold, timeout, detection_timeout, min_duration, max_duration, lang, rate, device_index)
+    def __init__(self, api_key: str, volume_threshold: int=3000, timeout: float=1.0, detection_timeout: float=10.0, min_duration: float=0.3, max_duration: float=20.0, lang: str="ja-JP", rate: int=44100, channels: int=1, device_index: int=-1):
+        super().__init__(api_key, self.on_request, volume_threshold, timeout, detection_timeout, min_duration, max_duration, lang, rate, channels, device_index)
         self.last_recognized_text = None
 
     async def on_request(self, text: str):
         self.last_recognized_text = text
         self.stop_listening()
 
     async def get_request(self):
```

## aiavatar/listeners/wakeword.py

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from threading import Thread
 from typing import Callable
 from . import SpeechListenerBase
 
 class WakewordListener(SpeechListenerBase):
-    def __init__(self, api_key: str, wakewords: list, on_wakeword: Callable, volume_threshold: int=3000, timeout: float=0.3, min_duration: float=0.2, max_duration: float=2, lang: str="ja-JP", rate: int=44100, device_index: int=-1, verbose: bool=False):
-        super().__init__(api_key, self.invoke_on_wakeword, volume_threshold, timeout, 0.0, min_duration, max_duration, lang, rate, device_index)
+    def __init__(self, api_key: str, wakewords: list, on_wakeword: Callable, volume_threshold: int=3000, timeout: float=0.3, min_duration: float=0.2, max_duration: float=2, lang: str="ja-JP", rate: int=44100, chennels: int=1, device_index: int=-1, verbose: bool=False):
+        super().__init__(api_key, self.invoke_on_wakeword, volume_threshold, timeout, 0.0, min_duration, max_duration, lang, rate, chennels, device_index)
         self.wakewords = wakewords
         self.on_wakeword = on_wakeword
         self.verbose = verbose
     
     async def invoke_on_wakeword(self, text: str):
         if self.verbose:
             self.logger.info(f"Recognized: {text}")
```

## aiavatar/processors/chatgpt.py

```diff
@@ -1,57 +1,134 @@
 from logging import getLogger, NullHandler
 import traceback
-from typing import Iterator
+import json
+from typing import Iterator, Callable
 from openai import ChatCompletion
 from . import ChatProcessor
 
+class ChatGPTFunction:
+    def __init__(self, name: str, description: str=None, parameters: dict=None, func: Callable=None):
+        self.name = name
+        self.description = description
+        self.parameters = parameters
+        self.func = func
+    
+    def get_spec(self):
+        return {
+            "name": self.name,
+            "description": self.description,
+            "parameters": self.parameters
+        }
+
+
+class ChatCompletionStreamResponse:
+    def __init__(self, stream: Iterator[str], function_name: str=None):
+        self.stream = stream
+        self.function_name = function_name
+
+    @property
+    def response_type(self):
+        return "function_call" if self.function_name else "content"
+
+
 class ChatGPTProcessor(ChatProcessor):
-    def __init__(self, api_key: str, model: str="gpt-3.5-turbo", temperature: float=1.0, max_tokens: int=0, system_message_content: str=None, history_count: int=10):
+    def __init__(self, api_key: str, model: str="gpt-3.5-turbo-0613", temperature: float=1.0, max_tokens: int=0, functions: dict=None, system_message_content: str=None, history_count: int=10):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
         self.api_key = api_key
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
+        self.functions = functions or {}
         self.system_message_content = system_message_content
         self.history_count = history_count
         self.histories = []
 
+    def add_function(self, name: str, description: str=None, parameters: dict=None, func: Callable=None):
+        self.functions[name] = ChatGPTFunction(name=name, description=description, parameters=parameters, func=func)
+
     def reset_histories(self):
         self.histories.clear()
 
+    async def chat_completion_stream(self, messages, call_functions: bool=True):
+        params = {
+            "api_key": self.api_key,
+            "messages": messages,
+            "model": self.model,
+            "temperature": self.temperature,
+            "stream": True,
+        }
+        if self.max_tokens:
+            params["max_tokens"] = self.max_tokens
+
+        if call_functions and self.functions:
+            params["functions"] = [v.get_spec() for _, v in self.functions.items()]
+
+        stream_resp = ChatCompletionStreamResponse(await ChatCompletion.acreate(**params))
+
+        async for chunk in stream_resp.stream:
+            if chunk:
+                delta = chunk["choices"][0]["delta"]
+                if delta.get("function_call"):
+                    stream_resp.function_name = delta["function_call"]["name"]
+                break
+        
+        return stream_resp
+
     async def chat(self, text: str) -> Iterator[str]:
         try:
             messages = []
             if self.system_message_content:
                 messages.append({"role": "system", "content": self.system_message_content})
             messages.extend(self.histories[-1 * self.history_count:])
             messages.append({"role": "user", "content": text})
 
-            params = {
-                "api_key": self.api_key,
-                "messages": messages,
-                "model": self.model,
-                "temperature": self.temperature,
-                "stream": True
-            }
-            if self.max_tokens:
-                params["max_tokens"] = self.max_tokens
-
-            completion = await ChatCompletion.acreate(**params)
-            
-            response_text = "" 
-            async for chunk in completion:
-                if chunk:
-                    content = chunk["choices"][0]["delta"].get("content")
+            response_text = ""
+            stream_resp = await self.chat_completion_stream(messages)
+
+            async for chunk in stream_resp.stream:
+                delta = chunk["choices"][0]["delta"]
+                if stream_resp.response_type == "content":
+                    content = delta.get("content")
+                    if content:
+                        response_text += delta["content"]
+                        yield content
+
+                elif stream_resp.response_type == "function_call":
+                    function_call = delta.get("function_call")
+                    if function_call:
+                        arguments = function_call["arguments"]
+                        response_text += arguments
+
+            if stream_resp.response_type == "function_call":
+                self.histories.append(messages[-1])
+                self.histories.append({
+                    "role": "assistant",
+                    "function_call": {
+                        "name": stream_resp.function_name,
+                        "arguments": response_text
+                    },
+                    "content": None
+                })
+
+                api_resp = await self.functions[stream_resp.function_name].func(**json.loads(response_text))
+
+                messages.append({"role": "function", "content": json.dumps(api_resp), "name": stream_resp.function_name})
+
+                response_text = ""
+                stream_resp = await self.chat_completion_stream(messages, False)
+
+                async for chunk in stream_resp.stream:
+                    delta = chunk["choices"][0]["delta"]
+                    content = delta.get("content")
                     if content:
                         response_text += content
                         yield content
-            
+                
             if response_text:
                 self.histories.append(messages[-1])
                 self.histories.append({"role": "assistant", "content": response_text})
 
         except Exception as ex:
             self.logger.error(f"Error at chat: {str(ex)}\n{traceback.format_exc()}")
             raise ex
```

## aiavatar/speech/voicevox.py

```diff
@@ -1,14 +1,15 @@
 import aiohttp
 import asyncio
 import io
 from logging import getLogger, NullHandler
 import traceback
 import wave
-import pyaudio
+import numpy
+import sounddevice
 from . import SpeechController
 
 class VoiceClip:
     def __init__(self, text: str):
         self.text = text
         self.download_task = None
         self.audio_clip = None
@@ -19,15 +20,14 @@
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
         self.base_url = base_url
         self.speaker_id = speaker_id
         self.device_index = device_index
         self.voice_clips = {}
-        self.pa = pyaudio.PyAudio()
         self._is_speaking = False
 
     async def download(self, voice: VoiceClip):
         params = {"speaker": self.speaker_id, "text": voice.text}
         async with aiohttp.ClientSession() as session:
             async with session.post(self.base_url + "/audio_query", params=params) as query_resp:
                 audio_query = await query_resp.json()
@@ -47,36 +47,24 @@
     async def speak(self, text: str):
         voice = self.prefetch(text)
         
         if not voice.audio_clip:
             await voice.download_task
         
         with wave.open(io.BytesIO(voice.audio_clip), "rb") as f:
-            def stream_callback(in_data, frame_count, time_info, status):
-                data = f.readframes(frame_count)
-                return (data, pyaudio.paContinue)
-
-            stream = self.pa.open(format=self.pa.get_format_from_width(width=f.getsampwidth()),
-                output_device_index=self.device_index,
-                channels=f.getnchannels(),
-                rate=f.getframerate(),
-                frames_per_buffer=1024,
-                output=True,
-                stream_callback=stream_callback,
-            )
-
             try:
                 self._is_speaking = True
-                stream.start_stream()
-                while stream.is_active():
-                    await asyncio.sleep(0.1)
+                data = numpy.frombuffer(
+                    f.readframes(f.getnframes()),
+                    dtype=numpy.int16
+                )
+                sounddevice.play(data, f.getframerate())
+                sounddevice.wait()
 
             except Exception as ex:
                 self.logger.error(f"Error at speaking: {str(ex)}\n{traceback.format_exc()}")
 
             finally:
                 self._is_speaking = False
-                stream.stop_stream()
-                stream.close()
 
     def is_speaking(self) -> bool:
         return self._is_speaking
```

## Comparing `aiavatar-0.1.4.dist-info/LICENSE` & `aiavatar-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.1.4.dist-info/METADATA` & `aiavatar-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.1.4
+Version: 0.2.0
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: numpy
 Requires-Dist: openai
-Requires-Dist: PyAudio
+Requires-Dist: sounddevice
 
 # AIAvatarKit
 
 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 
 ![AIAvatarKit Architecture Overview](documents/images/aiavatarkit_overview.png) 
 
@@ -172,14 +172,50 @@
 ```
 
 Launch VRChat as desktop mode on the machine that runs `run.py` and log in with the account for AIAvatar. Then set `VB-Cable-A` to microphone in VRChat setting window.
 
 That's all! Let's chat with the AIAvatar. Log in to VRChat on another machine (or Quest) and go to the world the AIAvatar is in.
 
 
+# ⚡️ Function Calling
+
+Use `chat_processor.add_function` to use ChatGPT function calling. In this example, `get_weather` will be called autonomously.
+
+```python
+# Add function
+async def get_weather(location: str):
+    await asyncio.sleep(1.0)
+    return {"weather": "sunny partly cloudy", "temperature": 23.4}
+
+app.chat_processor.add_function(
+    name="get_weather",
+    description="Get the current weather in a given location",
+    parameters={
+        "type": "object",
+        "properties": {
+            "location": {
+                "type": "string"
+            }
+        }
+    },
+    func=get_weather
+)
+```
+
+And, after `get_weather` called, message to get voice response will be sent to ChatGPT internally.
+
+```json
+{
+    "role": "function",
+    "content": "{\"weather\": \"sunny partly cloudy\", \"temperature\": 23.4}",
+    "name": "get_weather"
+}
+```
+
+
 # 🎤 Testing audio I/O
 
 Using the script below to test the audio I/O before configuring AIAvatar.
 
 - Step-by-Step audio device configuration.
 - Speak immediately after start if the output device is correctly configured.
 - All recognized text will be shown in console if the input device is correctly configured.
```

## Comparing `aiavatar-0.1.4.dist-info/RECORD` & `aiavatar-0.2.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 aiavatar/__init__.py,sha256=SqrO15owXtN32q55sRbSxKqRJyOZ32gao4a-SQwJTA8,351
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
-aiavatar/bot.py,sha256=jkab04ZSwhbCy8GVwa7ms58EE_LrmipTTDRFUuI1ycc,5621
+aiavatar/bot.py,sha256=HY_2mf3idOZy67msIgnJnGDXJGLnGuDhaOBeA-Jd-W8,5672
 aiavatar/animation/__init__.py,sha256=cE0zS3FgTUd0c6LcsLUnDVSTlFrCF0ZiH7-4NJxiQnU,284
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
-aiavatar/device/audio.py,sha256=oCqxsY3lB6ZULTA9EhausaTgKYMxrSBhKYytr2FQap0,2535
+aiavatar/device/audio.py,sha256=xxRzbjyabXGrhY3WDc3UYEadjCU-xS7HF_vcXtGiC88,2344
 aiavatar/face/__init__.py,sha256=FPaP8RT8UXQ_UMON7RLvg2FUotOzTFVJ1qxzVk5zBTw,1650
 aiavatar/face/vrchat.py,sha256=VOibFm5Yuof-RQGfd1Zt1tx4v-TV9Usb8aMn7rHp5HY,1556
-aiavatar/listeners/__init__.py,sha256=7EU4Ea6AdJa9soe5WtgBcJ8rsKb43M-0cmBQfUvUQXY,6210
-aiavatar/listeners/voicerequest.py,sha256=6636rbXDJ0Dw6EPD0kSsF3f46A4H0zjyY7fAMzpAvkc,788
-aiavatar/listeners/wakeword.py,sha256=UMM-1HMmEFXQpIt9C2EOuGSoxJHj1fQdrz_e9adJiGs,1007
+aiavatar/listeners/__init__.py,sha256=VGsz2XkifoMIwTqDEcfK3HB8S593CpZUPnRwpN5PoNc,6081
+aiavatar/listeners/voicerequest.py,sha256=kJM0tBTa-3PHbnSJVaSSYWJ2z4qDVkPEw0WrKQY0SpY,815
+aiavatar/listeners/wakeword.py,sha256=IX2_iNtUkjm8oSbRds6scrBYSoaywNZRhzq8GANoaIE,1034
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
-aiavatar/processors/chatgpt.py,sha256=snlUw6eYS__j_PM8ab7YZmE4CcalXKQLpdO_4JQa_h0,2151
+aiavatar/processors/chatgpt.py,sha256=gGxHcCgjewyqcTd4IZy0A-Jdzm1B9chY3rGU1Jmhh6w,5177
 aiavatar/speech/__init__.py,sha256=yiveD86ikoWYYVnpdi1r_6ou5bXr-SOkmnri6ry_qHI,275
-aiavatar/speech/voicevox.py,sha256=SsR-yFHb7fLYvA4M08wPw_eqiq9ZyISkeqHeiV2Epco,2794
-aiavatar-0.1.4.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.1.4.dist-info/METADATA,sha256=QsxGgQdCSemzPf7UmTQR23FH6QLdl3gTRjmwHj7KjMA,8081
-aiavatar-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiavatar-0.1.4.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.1.4.dist-info/RECORD,,
+aiavatar/speech/voicevox.py,sha256=8taNU-ziWhL_fR5b_caP5IiOkwzPlLvfRALRj6WbPCQ,2281
+aiavatar-0.2.0.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.2.0.dist-info/METADATA,sha256=qbs_cuhGzlDgdsqzklgnVUaZFIa_HVHA2_A01W_PyOQ,8953
+aiavatar-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiavatar-0.2.0.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.2.0.dist-info/RECORD,,
```

