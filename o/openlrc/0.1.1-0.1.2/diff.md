# Comparing `tmp/openlrc-0.1.1.tar.gz` & `tmp/openlrc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlrc-0.1.1.tar", max compression
+gzip compressed data, was "openlrc-0.1.2.tar", max compression
```

## Comparing `openlrc-0.1.1.tar` & `openlrc-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,15 @@
--rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.1/LICENSE
--rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.1/openlrc/__init__.py
--rw-r--r--   0        0        0      257 2023-06-09 13:43:55.157439 openlrc-0.1.1/openlrc/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5400 2023-06-15 19:13:45.417991 openlrc-0.1.1/openlrc/__pycache__/chatbot.cpython-310.pyc
--rw-r--r--   0        0        0     1031 2023-06-09 20:00:35.708506 openlrc-0.1.1/openlrc/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      656 2023-06-15 20:08:26.472755 openlrc-0.1.1/openlrc/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0     5882 2023-06-15 19:59:15.690355 openlrc-0.1.1/openlrc/__pycache__/openlrc.cpython-310.pyc
--rw-r--r--   0        0        0     4804 2023-06-15 17:09:26.804252 openlrc-0.1.1/openlrc/__pycache__/opt.cpython-310.pyc
--rw-r--r--   0        0        0     6798 2023-06-15 19:59:20.343415 openlrc-0.1.1/openlrc/__pycache__/prompter.cpython-310.pyc
--rw-r--r--   0        0        0     3340 2023-06-15 08:09:06.043276 openlrc-0.1.1/openlrc/__pycache__/subtitle.cpython-310.pyc
--rw-r--r--   0        0        0     4057 2023-06-15 18:20:42.834750 openlrc-0.1.1/openlrc/__pycache__/transcribe.cpython-310.pyc
--rw-r--r--   0        0        0     4657 2023-06-15 15:42:00.472565 openlrc-0.1.1/openlrc/__pycache__/translate.cpython-310.pyc
--rw-r--r--   0        0        0     3558 2023-06-15 08:09:06.045276 openlrc-0.1.1/openlrc/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     6066 2023-06-16 02:10:14.597437 openlrc-0.1.1/openlrc/chatbot.py
--rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.1.1/openlrc/exceptions.py
--rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.1/openlrc/logger.py
--rw-r--r--   0        0        0     7588 2023-06-16 02:39:22.869319 openlrc-0.1.1/openlrc/openlrc.py
--rw-r--r--   0        0        0     5498 2023-06-15 17:09:22.318005 openlrc-0.1.1/openlrc/opt.py
--rw-r--r--   0        0        0     6900 2023-06-15 19:57:21.308031 openlrc-0.1.1/openlrc/prompter.py
--rw-r--r--   0        0        0     2523 2023-06-15 08:09:05.047514 openlrc-0.1.1/openlrc/subtitle.py
--rw-r--r--   0        0        0     5675 2023-06-15 18:20:06.625488 openlrc-0.1.1/openlrc/transcribe.py
--rw-r--r--   0        0        0     5562 2023-06-15 15:41:13.481695 openlrc-0.1.1/openlrc/translate.py
--rw-r--r--   0        0        0     2488 2023-06-15 08:08:08.742912 openlrc-0.1.1/openlrc/utils.py
--rw-r--r--   0        0        0     1113 2023-06-16 02:40:25.990250 openlrc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2176 2023-06-16 02:40:04.456156 openlrc-0.1.1/README.md
--rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 openlrc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 10:20:06.659160 openlrc-0.1.2/LICENSE
+-rw-r--r--   0        0        0      106 2023-06-09 13:01:57.605311 openlrc-0.1.2/openlrc/__init__.py
+-rw-r--r--   0        0        0     6534 2023-06-22 22:44:31.210888 openlrc-0.1.2/openlrc/chatbot.py
+-rw-r--r--   0        0        0      532 2023-06-09 19:56:29.876606 openlrc-0.1.2/openlrc/exceptions.py
+-rw-r--r--   0        0        0      597 2023-06-15 20:08:22.292558 openlrc-0.1.2/openlrc/logger.py
+-rw-r--r--   0        0        0     8777 2023-06-22 16:23:55.581748 openlrc-0.1.2/openlrc/openlrc.py
+-rw-r--r--   0        0        0     5104 2023-06-20 09:23:36.095683 openlrc-0.1.2/openlrc/opt.py
+-rw-r--r--   0        0        0     6782 2023-06-22 22:23:54.135290 openlrc-0.1.2/openlrc/prompter.py
+-rw-r--r--   0        0        0     3071 2023-06-21 09:39:23.768067 openlrc-0.1.2/openlrc/subtitle.py
+-rw-r--r--   0        0        0     5688 2023-06-21 02:12:44.479638 openlrc-0.1.2/openlrc/transcribe.py
+-rw-r--r--   0        0        0     5592 2023-06-22 20:09:21.182541 openlrc-0.1.2/openlrc/translate.py
+-rw-r--r--   0        0        0     3201 2023-06-20 08:37:49.043106 openlrc-0.1.2/openlrc/utils.py
+-rw-r--r--   0        0        0     1158 2023-06-22 22:51:49.212478 openlrc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2436 2023-06-22 22:53:57.118364 openlrc-0.1.2/README.md
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 openlrc-0.1.2/PKG-INFO
```

### Comparing `openlrc-0.1.1/LICENSE` & `openlrc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.1/openlrc/chatbot.py` & `openlrc-0.1.2/openlrc/chatbot.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,86 +8,95 @@
 
 from openlrc.exceptions import ChatBotException
 from openlrc.logger import logger
 from openlrc.utils import get_messages_token_number, get_text_token_number
 
 
 class GPTBot:
-    def __init__(self, model='gpt-3.5-turbo-16k', retry=8, max_async=16, fee_limit=0.05):
+    def __init__(self, model='gpt-3.5-turbo-16k', temperature=1, top_p=1, retry=8, max_async=16, fee_limit=0.05):
         openai.api_key = os.getenv("OPENAI_API_KEY")
 
         self.model = model
+        self.temperature = temperature
+        self.top_p = top_p
         self.retry = retry
         self.max_async = max_async
         self.fee_limit = fee_limit
 
         # Pricing for 1k tokens, info from https://openai.com/pricing
         self.pricing = {
             'gpt-3.5-turbo': (0.0015, 0.002),
             'gpt-3.5-turbo-16k': (0.003, 0.004),
             'gpt-4': (0.03, 0.06),
             'gpt-4-32k': (0.06, 0.12)
         }
-        self.fee = []
+        self.api_fees = []  # OpenAI API fee for each call
+
+    def update(self, temperature=None, top_p=None):
+        if temperature:
+            self.temperature = temperature
+
+        if top_p:
+            self.top_p = top_p
 
     def estimate_fee(self, messages: List[Dict]):
         """
         Estimate the total fee for the given messages.
         """
         token_map = {'system': 0, 'user': 0, 'assistant': 0}
         for message in messages:
             token_map[message['role']] += get_text_token_number(message['content'])
 
         prompt_price, completion_price = self.pricing[self.model]
 
-        total_price = (sum(token_map.values()) * prompt_price + token_map['user'] * completion_price) / 1000
+        total_price = (sum(token_map.values()) * prompt_price + token_map['user'] * completion_price * 2) / 1000
 
         return total_price
 
     def update_fee(self, response):
         prompt_price, completion_price = self.pricing[self.model]
 
         prompt_tokens = response.usage['prompt_tokens']
         completion_tokens = response.usage['completion_tokens']
 
-        self.fee[-1] += (prompt_tokens * prompt_price + completion_tokens * completion_price) / 1000
+        self.api_fees[-1] += (prompt_tokens * prompt_price + completion_tokens * completion_price) / 1000
 
     async def _create_achat(self, messages: List[Dict], output_checker: Callable = lambda x: True):
-        # TODO: accumulate the actual fee for each thread.
-
         logger.debug(f'Raw content: {messages}')
 
         response = None
         for i in range(self.retry):
             try:
                 response = openai.ChatCompletion.create(
                     model=self.model,
-                    messages=messages
+                    messages=messages,
+                    temperature=self.temperature,
+                    top_p=self.top_p
                 )
                 self.update_fee(response)
                 if response.choices[0].finish_reason == 'length':
                     raise ChatBotException(
-                        f'Failed to get completion. Exceed max token length.'
-                        f'prompt tokens: {response.usage["prompt_tokens"]}, '
-                        f'completion tokens: {response.usage["completion_tokens"]}, '
-                        f'total tokens: {response.usage["total_tokens"]}'
+                        f'Failed to get completion. Exceed max token length. '
+                        f'Prompt tokens: {response.usage["prompt_tokens"]}, '
+                        f'Completion tokens: {response.usage["completion_tokens"]}, '
+                        f'Total tokens: {response.usage["total_tokens"]}'
                         f'Reduce chunk_size may help.'
                     )
                 if not output_checker(messages, response.choices[0].message.content):
                     logger.warning(f'Invalid response format. Retry num: {i + 1}.')
                     continue
 
                 break
             except openai.error.RateLimitError:
                 logger.warning(f'Rate limit exceeded. Wait 10s before retry. Retry num: {i + 1}.')
                 time.sleep(10)
             except openai.error.Timeout:
                 logger.warning(f'Timeout. Wait 3 before retry. Retry num: {i + 1}.')
                 time.sleep(3)
-            except openai.error.APIConnectionError:
+            except (openai.error.APIConnectionError, openai.error.ServiceUnavailableError):
                 logger.warning(f'API connection error. Wait 30s before retry. Retry num: {i + 1}.')
                 time.sleep(30)
             except openai.error.APIError:
                 logger.warning(f'API error. Wait 30s before retry. Retry num: {i + 1}.')
                 time.sleep(30)
 
         if not response:
@@ -122,21 +131,22 @@
         token_numbers = [get_messages_token_number(message) for message in messages_list]
         logger.info(f'Max token num: {max(token_numbers):.0f}, '
                     f'Avg token num: {sum(token_numbers) / len(token_numbers):.0f}')
 
         # if the approximated billing fee exceeds the limit, raise an exception.
         approximated_fee = sum([self.estimate_fee(messages) for messages in messages_list])
         logger.info(f'Approximated billing fee: {approximated_fee:.4f} USD')
-        self.fee += [0]  # Actual fee for this translation call.
+        self.api_fees += [0]  # Actual fee for this translation call.
         if approximated_fee > self.fee_limit:
             raise ChatBotException(f'Approximated billing fee {approximated_fee} '
                                    f'exceeds the limit: {self.fee_limit}$.')
 
         try:
             results = asyncio.run(self._amessage(messages_list, output_checker=output_checker))
         except ChatBotException as e:
+            logger.error(f'Failed to message with GPT. Error: {e}')
             raise e
         finally:
-            logger.info(f'Translation fee for this call: {self.fee[-1]:.4f} USD')
-            logger.info(f'Total bot translation fee: {sum(self.fee):.4f} USD')
+            logger.info(f'Translation fee for this call: {self.api_fees[-1]:.4f} USD')
+            logger.info(f'Total bot translation fee: {sum(self.api_fees):.4f} USD')
 
         return results
```

### Comparing `openlrc-0.1.1/openlrc/exceptions.py` & `openlrc-0.1.2/openlrc/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.1/openlrc/logger.py` & `openlrc-0.1.2/openlrc/logger.py`

 * *Files identical despite different names*

### Comparing `openlrc-0.1.1/openlrc/openlrc.py` & `openlrc-0.1.2/openlrc/openlrc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import json
 import os
+import traceback
 from multiprocessing.pool import ThreadPool
 from pprint import pformat
 from queue import Queue
-from threading import Thread
+from threading import Thread, Lock
 
 from openlrc.logger import logger
 from openlrc.opt import SubtitleOptimizer
 from openlrc.subtitle import Subtitle
 from openlrc.transcribe import Transcriber
-from openlrc.translate import Translator
+from openlrc.translate import GPTTranslator
 from openlrc.utils import Timer, change_ext, extend_filename, get_audio_duration
 
 
 class LRCer:
-    """
-    :param model_name: Name of whisper model (tiny, tiny.en, base, base.en, small, small.en, medium,
-                    medium.en, large-v1, or large-v2) When a size is configured, the converted model is downloaded
-                    from the Hugging Face Hub.
-                    Default: ``large-v2``
-    :param fee_limit: The maximum fee you are willing to pay for translation. Default: ``0.1``
-    """
+    def __init__(self, model_name='large-v2', compute_type='float16', fee_limit=0.1, consumer_thread=11):
+        """
+        :param model_name: Name of whisper model (tiny, tiny.en, base, base.en, small, small.en, medium,
+                        medium.en, large-v1, or large-v2) When a size is configured, the converted model is downloaded
+                        from the Hugging Face Hub.
+                        Default: ``large-v2``
+        :param compute_type: The type of computation to use. Can be ``int8``, ``int8_float16``, ``int16``,
+                        ``float16`` or ``float32``.
+                        Default: ``float16``
+        :param fee_limit: The maximum fee you are willing to pay for one translation call. Default: ``0.1``
+        :param consumer_thread: To prevent exceeding the RPM and TPM limits set by OpenAI, the default is TPM/MAX_TOKEN.
+        """
 
-    def __init__(self, model_name='large-v2', fee_limit=0.1):
-        self.transcriber = Transcriber(model_name=model_name)
+        self.transcriber = Transcriber(model_name=model_name, compute_type=compute_type)
         self.fee_limit = fee_limit
+        self.api_fee = 0  # Can be updated in different thread, operation should be thread-safe
+
+        self._lock = Lock()
+        self.exception = None
+        self.consumer_thread = consumer_thread
 
     def transcription_producer(self, transcription_queue, audio_paths):
         """
         Sequential Producer.
         """
         for audio_path in audio_paths:
             transcribed_path = change_ext(extend_filename(audio_path, '_transcribed'), 'json')
@@ -55,64 +65,73 @@
     def transcription_consumer(self, transcription_queue, target_lang, prompter, audio_type):
         """
         Parallel Consumer.
         """
         with ThreadPool() as pool:
             _ = [pool.apply_async(self.translation_worker,
                                   args=(transcription_queue, target_lang, prompter, audio_type))
-                 for _ in range(os.cpu_count())]
+                 for _ in range(self.consumer_thread)]
             pool.close()
             pool.join()
         logger.info('Transcription consumer finished.')
 
     def translation_worker(self, transcription_queue, target_lang, prompter, audio_type):
         """
         Parallel translation.
         """
         while True:
-            logger.info(f'Translation worker waiting transcription...')
+            logger.debug(f'Translation worker waiting transcription...')
             transcribed_path = transcription_queue.get()
 
             if transcribed_path is None:
                 transcription_queue.put(None)
-                logger.info('Translation worker finished.')
+                logger.debug('Translation worker finished.')
                 return
 
             logger.info(f'Got transcription: {transcribed_path}')
             transcribed_sub = Subtitle(transcribed_path)
             transcribed_opt_sub = self.post_process(transcribed_sub, update_name=True)
 
             # xxx_transcribed_optimized_translated.json
             translated_path = extend_filename(transcribed_opt_sub.filename, '_translated')
             if not os.path.exists(translated_path):
                 # Translate the transcribed json
-                translator = Translator(prompter=prompter, fee_limit=self.fee_limit)
+                translator = GPTTranslator(prompter=prompter, fee_limit=self.fee_limit)
 
                 with Timer('Translation process'):
-                    target_texts = translator.translate(transcribed_opt_sub.get_texts(),
-                                                        src_lang=transcribed_opt_sub.lang,
-                                                        target_lang=target_lang,
-                                                        audio_type=audio_type)
+                    try:
+                        target_texts = translator.translate(
+                            transcribed_opt_sub.get_texts(),
+                            src_lang=transcribed_opt_sub.lang,
+                            target_lang=target_lang,
+                            title=transcribed_path.replace('_transcribed.json', ''),
+                            audio_type=audio_type,
+                            compare_path=transcribed_path.replace('_transcribed.json', '_compare.json')
+                        )
+                    except Exception as e:
+                        self.exception = e
+
+                with self._lock:
+                    self.api_fee += translator.api_fee  # Ensure thread-safe
 
                 transcribed_opt_sub.set_texts(target_texts)
 
                 # xxx_transcribed_optimized_translated.json
                 transcribed_opt_sub.save(translated_path, update_name=True)
             else:
-                logger.info(f'Found transcribed json file: {translated_path}')
+                logger.info(f'Found translated json file: {translated_path}')
 
             translated_sub = Subtitle(translated_path)
             output_filename = transcribed_path.replace('_transcribed.json', '.json')
 
             final_subtitle = self.post_process(translated_sub, output_name=output_filename, t2m=target_lang == 'zh-cn',
-                                               remove_files=[
-                                                   transcribed_opt_sub.filename,  # xxx_transcribed_optimized.json
-                                               ], update_name=True)  # xxx.json
+                                               update_name=True)  # xxx.json
 
             final_subtitle.to_lrc()
+            logger.info(f'Translation fee til now: {self.api_fee:.4f} USD')
 
     def run(self, audio_paths, target_lang='zh-cn', prompter='base_trans', audio_type='Anime'):
         """
         Split the translation into 2 phases: transcription and translation. They're running in parallel.
         Firstly, transcribe the audios one-by-one. At the same time, translation threads are created and waiting for
         the transcription results. After all the transcriptions are done, the translation threads will start to
         translate the transcribed texts.
@@ -132,14 +151,19 @@
 
             consumer.start()
             producer.start()
 
             producer.join()
             consumer.join()
 
+            if self.exception:
+                traceback.print_exception(type(self.exception), self.exception, self.exception.__traceback__)
+
+        logger.info(f'Totally used API fee: {self.api_fee:.4f} USD')
+
     @staticmethod
     def to_json(segments, name, lang):
         result = {
             'generator': 'LRC generated by https://github.com/zh-plus/Open-Lyrics',
             'language': lang,
             'segments': []
         }
```

### Comparing `openlrc-0.1.1/openlrc/opt.py` & `openlrc-0.1.2/openlrc/opt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import math
+import re
 from typing import Union
 
 import opencc
 
 from openlrc.logger import logger
 from openlrc.subtitle import Subtitle
 from openlrc.utils import extend_filename
@@ -75,29 +75,19 @@
     def merge_repeat(self):
         """
         Merge the same pattern in one lyric.
         :return:
         """
         new_elements = self.subtitle.segments
 
-        def get_repeat(text):
-            """
-            Check if the text is repeated for [1-4] words.
-            """
-            for j in range(1, 5):
-                repeating_num = math.floor(len(text) / float(j))
-                if text[:j] * repeating_num == text[:j * repeating_num]:
-                    return text[:j]
-            return None
-
-        for i in range(len(new_elements)):
-            repeat_text = get_repeat(new_elements[i].text)
-            if repeat_text:
-                new_elements[i].text = repeat_text + '...(Repeat)'
-                logger.debug(f'Merge same words: {repeat_text}')
+        for i, element in enumerate(new_elements):
+            text = element.text
+            text = re.sub(r'(.)\1{4,}', r'\1\1...', text)
+            text = re.sub(r'(.+)\1{4,}', r'\1\1...', text)
+            new_elements[i].text = text
 
         logger.debug('Merge same words done.')
 
         self.subtitle.segments = new_elements
 
     def cut_long(self, threshold=125, keep=20):
         new_elements = self.subtitle.segments
@@ -137,15 +127,15 @@
 
         logger.debug('Remove empty done.')
 
     def perform_all(self, t2m=False):
         for _ in range(2):
             self.merge_same()
             self.merge_short()
-            # self.merge_same_words()
+            self.merge_repeat()
             self.cut_long()
             self.remove_unk()
             self.remove_empty()
 
             if t2m or self.subtitle.lang.lower() == 'zh-cn':
                 self.traditional2mandarin()
```

### Comparing `openlrc-0.1.1/openlrc/subtitle.py` & `openlrc-0.1.2/openlrc/subtitle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import sys
 from dataclasses import dataclass
+from functools import partial
 from typing import List, Union
 
 from openlrc.logger import logger
 from openlrc.utils import format_timestamp, change_ext
 
 
 @dataclass
@@ -29,14 +30,18 @@
 
 class Subtitle:
     """
     Save a sequence of Element, and meta data.
     """
 
     def __init__(self, filename):
+        """
+        :param filename: json file.
+        """
+
         self.filename = filename
         with open(filename, encoding='utf-8') as f:
             content = json.loads(f.read())
 
         self.lang = content['language']
         self.generator = content['generator']
         self.segments: List[Element] = [Element(**seg) for seg in content['segments']]
@@ -63,23 +68,32 @@
 
         if update_name:
             self.filename = filename
 
         return filename
 
     def to_lrc(self):
-        """
-        Save lrc file.
-        """
         lrc_name = change_ext(self.filename, 'lrc')
+        fmt = partial(format_timestamp, fmt='lrc')
         with open(lrc_name, 'w', encoding='utf-8') as f:
             print(f'LRC generated by https://github.com/zh-plus/Open-Lyrics, lang={self.lang}', file=f, flush=True)
             for i, segment in enumerate(self.segments):
                 print(
-                    f'[{format_timestamp(segment.start)}] {segment.text}',
+                    f'[{fmt(segment.start)}] {segment.text}',
                     file=f,
                     flush=True,
                 )
                 if i == len(self.segments) - 1 or segment.end != self.segments[i + 1].start:
-                    print(f'[{format_timestamp(segment.end)}]', file=f, flush=True)
+                    print(f'[{fmt(segment.end)}]', file=f, flush=True)
 
         logger.info(f'File saved to {lrc_name}')
+
+    def to_srt(self):
+        srt_name = change_ext(self.filename, 'srt')
+        fmt = partial(format_timestamp, fmt='srt')
+        with open(srt_name, 'w', encoding='utf-8') as f:
+            for i, segment in enumerate(self.segments, start=1):
+                print(f'{i}\n'
+                      f'{fmt(segment.start)} --> {fmt(segment.end)}\n'
+                      f'{segment.text}\n\n', file=f, flush=True)
+
+        logger.info(f'File saved to {srt_name}')
```

### Comparing `openlrc-0.1.1/openlrc/transcribe.py` & `openlrc-0.1.2/openlrc/transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Transcriber:
     def __init__(self, model_name='large-v2', compute_type='float16', device='cuda'):
         self.model_name = model_name
         self.compute_type = compute_type
         self.device = device
 
     def transcribe(self, audio_path, batch_size=8):
-        whisper_model = whisperx.load_model('large-v2', compute_type='float16', device=self.device)
+        whisper_model = whisperx.load_model(self.model_name, compute_type=self.compute_type, device=self.device)
         audio = whisperx.load_audio(audio_path)
 
         with Timer('Base Whisper Transcription'):
             result = whisper_model.transcribe(audio, batch_size=batch_size)
 
         release_memory(whisper_model)
```

### Comparing `openlrc-0.1.1/openlrc/translate.py` & `openlrc-0.1.2/openlrc/translate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,116 +1,140 @@
 import json
-from typing import Callable
+import os
+import re
+import uuid
+
+import requests
 
 from openlrc.chatbot import GPTBot
 from openlrc.logger import logger
-from openlrc.prompter import prompter_map
+from openlrc.prompter import prompter_map, BaseTranslatePrompter
 
 
-class Translator:
-    def __init__(self, prompter: str = 'base_trans', chunk_size=160,
-                 fee_limit=0.1, intercept_line=None, force_translate=False):
+class GPTTranslator:
+    def __init__(self, prompter: str = 'base_trans', fee_limit=0.1, chunk_size=30, intercept_line=None,
+                 force_translate=False):
         """
         :param prompter: Translate prompter, choices can be found in `prompter_map` from prompter.py.
-        :param chunk_size: Use smaller chunk size to avoid exceeding the token limit & output complete message.
-                Larger chunk size may improve the translation result. However, large chunk size make the response
-                of OpenAI API slower and more unstable.
         :param fee_limit: Fee limit (USD) for OpenAI API.
+        :param chunk_size: Use small (<20) chunk size for speed (more async call), and enhance translation
+                    stability (keep audio timeline consistency).
         :param intercept_line: Intercepted text line number.
         :param force_translate: Force translation even if the source language is the same as the target language.
         """
         if prompter not in prompter_map:
             raise ValueError(f'Prompter {prompter} not found.')
 
         self.prompter = prompter
-        self.chunk_size = chunk_size
         self.fee_limit = fee_limit
+        self.chunk_size = chunk_size
+        self.api_fee = 0
         self.intercept_line = intercept_line
         self.force_translate = force_translate
 
-    def _make_chunks(self, texts):
-        chunks = [texts[i:i + self.chunk_size] for i in range(0, len(texts), self.chunk_size)]
+    @staticmethod
+    def make_chunks(texts, chunk_size=30):
+        """
+        Split the subtitle into chunks, each chunk has a line number of chunk_size.
+        :return: List of chunks, each chunk is a list of (line_number, text) tuples
+        """
 
-        if len(chunks) > 1 and len(chunks[-1]) <= self.chunk_size / 2:
-            # Merge the last two chunks if the last chunk is too small
-            last_two = chunks[-2] + chunks[-1]
-
-            # Split the merged into 2 equally sized chunks
-            chunks[-2] = last_two[:len(last_two) // 2]
-            chunks[-1] = last_two[len(last_two) // 2:]
+        chunks = []
+        start = 1
+        for i in range(0, len(texts), chunk_size):
+            chunk = [(start + j, text) for j, text in enumerate(texts[i:i + chunk_size])]
+            start += len(chunk)
+            chunks.append(chunk)
+
+        # if the last chunk is too small, merge it to the previous chunk
+        if len(chunks) >= 2 and len(chunks[-1]) < chunk_size / 2:
+            chunks[-2].extend(chunks[-1])
+            chunks.pop()
 
         return chunks
 
-    def parse_responses(self, chunks, responses, post_process_fn: Callable = lambda x: x):
-        results = []
+    def parse_responses(self, response):
+        content = response.choices[0].message.content
 
-        for i, response in enumerate(responses):
-            content = response.choices[0].message.content
-            logger.debug(f'Target content - chunk{i}: {content}')
-
-            chunk_json_content = json.loads(content)
-            logger.debug(f'Length of the translated chunk: {len(chunk_json_content["list"])}')
-
-            chunk_size = len(chunks[i])
-            # Helping OpenAI clean up their mess.
-            if len(chunk_json_content['list']) < chunk_size:
-                logger.warning(f'The number of translated sentences is less than that of the original list. '
-                               f'Add {chunk_size - len(chunk_json_content["list"])} <MANUALLY-ADDED> label')
-                chunk_json_content['list'] += [' '] * (chunk_size - len(chunk_json_content['list']))
-            elif len(chunk_json_content['list']) > chunk_size:
-                logger.warning('The number of translated sentences is more than that of the original list. Truncated')
-                chunk_json_content['list'] = chunk_json_content['list'][:chunk_size]
+        try:
+            # Extract summary tag
+            summary = re.search(r'<summary>(.*)</summary>', content)
+            scene = re.search(r'<scene>(.*)</scene>', content)
 
-            results += chunk_json_content['list']
+            summary = summary.group(1) if summary else ''
+            scene = scene.group(1) if scene else ''
 
-        results = post_process_fn(results)
+            translation = re.findall(r'Translation>\n*(.*?)(?:#\d+|<summary>|\n*$)', content, re.DOTALL)
 
-        return results
+            return summary.strip(), scene.strip(), [t.strip() for t in translation]
 
-    def translate(self, texts, src_lang, target_lang, audio_type='Anime'):
-        prompter = prompter_map[self.prompter](src_lang, target_lang, audio_type)
-        translate_bot = GPTBot(fee_limit=self.fee_limit)
+        except Exception as e:
+            logger.error(f'Failed to extract contents from response: {content}')
+            raise e
 
-        chunks = self._make_chunks(texts)
+    def translate(self, texts, src_lang, target_lang, audio_type='Anime', title='', synopsis='',
+                  compare_path='test_intermediate.json'):
+        prompter: BaseTranslatePrompter = prompter_map[self.prompter](
+            src_lang, target_lang, audio_type, title=title, synopsis=synopsis)
+        translate_bot = GPTBot(fee_limit=self.fee_limit)
+        translate_bot.update(temperature=0.7)
 
-        # Step 1: Revision step in source language
-        step1_user_inputs = [prompter.format_texts(chunk) for chunk in chunks]
+        chunks = self.make_chunks(texts, chunk_size=self.chunk_size)
 
-        logger.info(f'Translating {len(step1_user_inputs)} user_prompts of source texts with async call.')
+        # Start chunk-by-chunk translation
+        translations = []
+        summaries = []
+        summary, scene = '', ''
+        for i, chunk in enumerate(chunks, start=1):
+            user_input = prompter.format_texts(chunk)
+            messages_list = [
+                {'role': 'system', 'content': prompter.system()},
+                {'role': 'user', 'content': prompter.user(i, user_input, summaries, scene)}
+            ]
+            response = translate_bot.message(messages_list, output_checker=prompter.check_format)[0]
+            summary, scene, translated = self.parse_responses(response)
+            translations.extend(translated)
+            summaries.append(summary)
+            logger.info(f'Translating {title}: {i}/{len(chunks)}')
+            logger.info(f'summary: {summary}')
+            logger.info(f'scene: {scene}')
+
+        self.api_fee += sum(translate_bot.api_fees)
+        compare_results = {
+            'compare': [{'idx': i, 'input': user_input, 'output': translation} for
+                        i, (user_input, translation) in
+                        enumerate(zip(texts, translations), start=1)]}
+
+        with open(compare_path, 'w', encoding='utf-8') as f:
+            json.dump(compare_results, f, indent=4, ensure_ascii=False)
+
+        return translations
+
+
+class MSTranslator:
+    def __init__(self):
+        self.key = os.environ['MS_TRANSLATOR_KEY']
+        self.endpoint = 'https://api.cognitive.microsofttranslator.com'
+        self.location = 'eastasia'
+        self.path = '/translate'
+        self.constructed_url = self.endpoint + self.path
+
+        self.headers = {
+            'Ocp-Apim-Subscription-Key': self.key,
+            'Ocp-Apim-Subscription-Region': self.location,
+            'Content-type': 'application/json',
+            'X-ClientTraceId': str(uuid.uuid4())
+        }
+
+    def translate(self, texts, src_lang, target_lang):
+        params = {
+            'api-version': '3.0',
+            'from': src_lang,
+            'to': target_lang
+        }
 
-        # Chunked messages
-        step1_messages_list = [
-            [{'role': 'system', 'content': prompter.system()},
-             {'role': 'user', 'content': prompter.step1(user_input)}]
-            for user_input in step1_user_inputs
-        ]
-        responses = translate_bot.message(step1_messages_list, output_checker=prompter.check_format)
-        step1_results = self.parse_responses(chunks, responses, post_process_fn=prompter.post_process)
-
-        logger.debug(f'After {src_lang} revision: {step1_results}')
-
-        # Step 2: Translation step from source language to target language (Keep chat history)
-        step2_messages_list = [
-            messages + [
-                {'role': 'assistant', 'content': responses[i].choices[0].message.content},
-                {'role': 'user', 'content': prompter.step2()}
-            ] for i, messages in enumerate(step1_messages_list)
-        ]
-        responses = translate_bot.message(step2_messages_list, output_checker=prompter.check_format)
-        step2_results = self.parse_responses(chunks, responses, post_process_fn=prompter.post_process)
-
-        logger.debug(f'After translation: {step2_results}')
-
-        # Step 3: Revision step in target language
-        chunks = self._make_chunks(step2_results)
-        step3_user_inputs = [prompter.format_texts(chunk) for chunk in chunks]
-        step3_messages_list = [
-            [{'role': 'system', 'content': prompter.system()},
-             {'role': 'user', 'content': prompter.step3(user_input)}]
-            for user_input in step3_user_inputs
-        ]
-        responses = translate_bot.message(step3_messages_list, output_checker=prompter.check_format)
-        step3_results = self.parse_responses(chunks, responses, post_process_fn=prompter.post_process)
+        body = [{'text': text} for text in texts]
 
-        logger.debug(f'After {target_lang} revision: {step3_results}')
+        request = requests.post(self.constructed_url, params=params, headers=self.headers, json=body)
+        response = request.json()
 
-        return step3_results
+        return json.dumps(response, sort_keys=True, ensure_ascii=False, indent=4, separators=(',', ': '))
```

### Comparing `openlrc-0.1.1/openlrc/utils.py` & `openlrc-0.1.2/openlrc/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,25 +78,41 @@
         self.start()
         return self
 
     def __exit__(self, *args):
         self.stop()
 
 
-def parse_timestamp(time_stamp):
-    minutes, seconds = time_stamp.split(':')
-    seconds, hundredths_of_sec = seconds.split('.')
-    return int(minutes) * 60 + int(seconds) + int(hundredths_of_sec) / 100.0
+def parse_timestamp(time_stamp, fmt='lrc'):
+    if fmt == 'lrc':
+        minutes, seconds = time_stamp.split(':')
+        seconds, hundredths_of_sec = seconds.split('.')
+        return int(minutes) * 60 + int(seconds) + int(hundredths_of_sec) / 100.0
+    elif fmt == 'srt':
+        hours, minutes, seconds = time_stamp.split(':')
+        seconds, milliseconds = seconds.split(',')
+        return int(hours) * 3600 + int(minutes) * 60 + int(seconds) + int(milliseconds) / 1000.0
+    else:
+        raise ValueError(f"Unsupported timestamp format: {fmt}")
 
 
-def format_timestamp(seconds: float):
+def format_timestamp(seconds: float, fmt='lrc'):
     assert seconds >= 0, "non-negative timestamp expected"
     milliseconds = round(seconds * 1000.0)
 
+    hours = milliseconds // 3600000
+    milliseconds %= 3600000
+
     minutes = milliseconds // 60000
     milliseconds %= 60000
 
     seconds = milliseconds // 1000
     milliseconds %= 1000
 
-    # [<minutes>:<seconds>.<hundredths of a second>]
-    return f"{minutes:02d}:{seconds:02d}.{milliseconds // 10:02d}"
+    if fmt == 'lrc':
+        # [<minutes>:<seconds>.<hundredths of a second>] for lrc
+        return f"{minutes:02d}:{seconds:02d}.{milliseconds // 10:02d}"
+    elif fmt == 'srt':
+        # [<hours>:<minutes>:<seconds>,<milliseconds>] for srt
+        return f"{hours:02d}:{minutes:02d}:{seconds:02d},{milliseconds:03d}"
+    else:
+        raise ValueError(f"Unsupported timestamp format: {fmt}")
```

### Comparing `openlrc-0.1.1/pyproject.toml` & `openlrc-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "openlrc"
-version = "0.1.1"
+version = "0.1.2"
 description = "Transcribe (whisper) and translate (gpt) voice into LRC file."
 license = "MIT"
 authors = [
     "Hao Zheng <zhenghaosustc@gmail.com>"
 ]
 readme = "README.md"
 homepage = "https://github.com/zh-plus/Open-Lyrics"
@@ -40,10 +40,12 @@
 tiktoken = "^0.3.1"
 langcodes = "^3.3.0"
 language-data = "^1.1"
 rich = "^12.6.0"
 tqdm = "^4.65.0"
 audioread = "^3.0.0"
 opencc = "^1.1.1"
+punctuators = "^0.0.5"
+colorlog = "^6.7.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zh-plus/Open-Lyrics/issues"
```

### Comparing `openlrc-0.1.1/README.md` & `openlrc-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Open-Lyrics
 
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using [OpenAI-GPT](https://github.com/openai/openai-python).
 
-**This new project is rapidly underway, and we welcome any issues or pull requests.**
-
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
    enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
@@ -33,25 +31,33 @@
 
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
+
+# Single file
 lrcer.run('./data/test.mp3', target_lang='zh-cn')  # Generate translated ./data/test.lrc with default translate prompt.
+
+# Multiple files
+lrcer.run(['./data/test1.mp3', './data/test2.mp3'], target_lang='zh-cn')
+# Note we run the transcription sequentially, but run the translation concurrently for each file.
 ```
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
 - [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
 - [x] [Usability] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
+- [x] [Quality] Improve batched translation/polish prompt according
+  to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
 - [ ] [Usability] Multiple output format support.
 - [ ] [Efficiency] Add Azure OpenAI Service support.
 - [ ] [Usability] Add local LLM support.
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
```

### Comparing `openlrc-0.1.1/PKG-INFO` & `openlrc-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transcribe (whisper) and translate (gpt) voice into LRC file.
 Home-page: https://github.com/zh-plus/Open-Lyrics
 License: MIT
 Keywords: openai-gpt3,whisper,voice transcribe,lrc
 Author: Hao Zheng
 Author-email: zhenghaosustc@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,33 +14,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: audioread (>=3.0.0,<4.0.0)
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: faster-whisper (>=0.6.0,<0.7.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: opencc (>=1.1.1,<2.0.0)
+Requires-Dist: punctuators (>=0.0.5,<0.0.6)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
 
 Open-Lyrics is a Python library that transcribes voice files using
 [faster-whisper](https://github.com/guillaumekln/faster-whisper), and translates/polishes the resulting text
 into `.lrc` files in the desired language using [OpenAI-GPT](https://github.com/openai/openai-python).
 
-**This new project is rapidly underway, and we welcome any issues or pull requests.**
-
 ## Installation
 
 1. Please install CUDA and cuDNN first according to https://opennmt.net/CTranslate2/installation.html to
    enable `faster-whisper`.
 
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
@@ -64,25 +64,33 @@
 
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
+
+# Single file
 lrcer.run('./data/test.mp3', target_lang='zh-cn')  # Generate translated ./data/test.lrc with default translate prompt.
+
+# Multiple files
+lrcer.run(['./data/test1.mp3', './data/test2.mp3'], target_lang='zh-cn')
+# Note we run the transcription sequentially, but run the translation concurrently for each file.
 ```
 
 ## Todo
 
 - [x] [Efficiency] Batched translate/polish for GPT request (enable contextual ability).
 - [x] [Efficiency] Concurrent support for GPT request.
 - [x] [Efficiency & Transcription Quality] Use [whisperx](https://github.com/m-bain/whisperX) for transcription.
 - [x] [Translation Quality] Make translate prompt more robust according to https://github.com/openai/openai-cookbook.
 - [x] [Usability] Automatically fix json encoder error using GPT.
 - [x] [Efficiency] Asynchronously perform transcription and translation for multiple audio inputs.
+- [x] [Quality] Improve batched translation/polish prompt according
+  to [gpt-subtrans](https://github.com/machinewrapped/gpt-subtrans).
 - [ ] [Usability] Multiple output format support.
 - [ ] [Efficiency] Add Azure OpenAI Service support.
 - [ ] [Usability] Add local LLM support.
 - [ ] [Others] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
```

