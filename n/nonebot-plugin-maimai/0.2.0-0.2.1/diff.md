# Comparing `tmp/nonebot_plugin_maimai-0.2.0.tar.gz` & `tmp/nonebot_plugin_maimai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.2.0.tar` & `nonebot_plugin_maimai-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1089 2023-02-08 00:46:07.674998 nonebot_plugin_maimai-0.2.0/LICENSE
--rw-r--r--   0        0        0    13245 2023-06-12 14:56:52.704104 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 03:30:51.719115 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1605 2023-02-08 01:36:17.843087 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17837 2023-06-12 14:49:23.491131 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17928 2023-06-12 14:49:22.832470 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5522 2023-06-12 14:49:03.118975 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      397 2023-03-02 02:30:46.242798 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     7497 2023-05-20 16:28:12.333709 nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1062 2023-06-12 14:55:04.696808 nonebot_plugin_maimai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3478 2023-06-12 14:54:59.661881 nonebot_plugin_maimai-0.2.0/README.md
--rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3492 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/README.md
+-rw-r--r--   0        0        0    15433 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1556 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17432 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17520 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5353 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      385 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     7312 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1059 2023-06-23 15:41:59.856062 nonebot_plugin_maimai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.2.0/LICENSE` & `nonebot_plugin_maimai-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Diving-Fish
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Diving-Fish
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/image.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import base64
-from io import BytesIO
-from .tool import STATIC
-from PIL import ImageFont, ImageDraw, Image
-
-
-path = STATIC + '/high_eq_image.png'
-fontpath = STATIC + "/msyh.ttc"
-
-
-def draw_text(img_pil, text, offset_x):
-    draw = ImageDraw.Draw(img_pil)
-    font = ImageFont.truetype(fontpath, 48)
-    width, height = draw.textsize(text, font)
-    x = 5
-    if width > 390:
-        font = ImageFont.truetype(fontpath, int(390 * 48 / width))
-        width, height = draw.textsize(text, font)
-    else:
-        x = int((400 - width) / 2)
-    draw.rectangle((x + offset_x - 2, 360, x + 2 + width + offset_x, 360 + height * 1.2), fill=(0, 0, 0, 255))
-    draw.text((x + offset_x, 360), text, font=font, fill=(255, 255, 255, 255))
-
-
-def text_to_image(text):
-    font = ImageFont.truetype(fontpath, 24)
-    padding = 10
-    margin = 4
-    text_list = text.split('\n')
-    max_width = 0
-    for text in text_list:
-        w, h = font.getsize(text)
-        max_width = max(max_width, w)
-    wa = max_width + padding * 2
-    ha = h * len(text_list) + margin * (len(text_list) - 1) + padding * 2
-    i = Image.new('RGB', (wa, ha), color=(255, 255, 255))
-    draw = ImageDraw.Draw(i)
-    for j in range(len(text_list)):
-        text = text_list[j]
-        draw.text((padding, padding + j * (margin + h)), text, font=font, fill=(0, 0, 0))
-    return i
-
-
-def image_to_base64(img, format='PNG'):
-    output_buffer = BytesIO()
-    img.save(output_buffer, format)
-    byte_data = output_buffer.getvalue()
-    base64_str = base64.b64encode(byte_data)
-    return base64_str
+import base64
+from io import BytesIO
+from .tool import STATIC
+from PIL import ImageFont, ImageDraw, Image
+
+
+path = STATIC + '/high_eq_image.png'
+fontpath = STATIC + "/msyh.ttc"
+
+
+def draw_text(img_pil, text, offset_x):
+    draw = ImageDraw.Draw(img_pil)
+    font = ImageFont.truetype(fontpath, 48)
+    width, height = draw.textsize(text, font)
+    x = 5
+    if width > 390:
+        font = ImageFont.truetype(fontpath, int(390 * 48 / width))
+        width, height = draw.textsize(text, font)
+    else:
+        x = int((400 - width) / 2)
+    draw.rectangle((x + offset_x - 2, 360, x + 2 + width + offset_x, 360 + height * 1.2), fill=(0, 0, 0, 255))
+    draw.text((x + offset_x, 360), text, font=font, fill=(255, 255, 255, 255))
+
+
+def text_to_image(text):
+    font = ImageFont.truetype(fontpath, 24)
+    padding = 10
+    margin = 4
+    text_list = text.split('\n')
+    max_width = 0
+    for text in text_list:
+        w, h = font.getsize(text)
+        max_width = max(max_width, w)
+    wa = max_width + padding * 2
+    ha = h * len(text_list) + margin * (len(text_list) - 1) + padding * 2
+    i = Image.new('RGB', (wa, ha), color=(255, 255, 255))
+    draw = ImageDraw.Draw(i)
+    for j in range(len(text_list)):
+        text = text_list[j]
+        draw.text((padding, padding + j * (margin + h)), text, font=font, fill=(0, 0, 0))
+    return i
+
+
+def image_to_base64(img, format='PNG'):
+    output_buffer = BytesIO()
+    img.save(output_buffer, format)
+    byte_data = output_buffer.getvalue()
+    base64_str = base64.b64encode(byte_data)
+    return base64_str
```

### Comparing `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,405 +1,408 @@
-# Author: xyb, Diving_Fish
-
-import os
-import math
-from typing import Optional, Dict, List,Tuple
-from .tool import STATIC
-import aiohttp
-from PIL import Image, ImageDraw, ImageFont, ImageFilter
-from .maimaidx_music import get_cover_len5_id, total_list
-
-
-scoreRank = 'D C B BB BBB A AA AAA S S+ SS SS+ SSS SSS+'.split(' ')
-combo = ' FC FC+ AP AP+'.split(' ')
-diffs = 'Basic Advanced Expert Master Re:Master'.split(' ')
-
-
-class ChartInfo(object):
-    def __init__(self, idNum:str, diff:int, tp:str, achievement:float, ra:int, comboId:int, scoreId:int,
-                 title:str, ds:float, lv:str):
-        self.idNum = idNum
-        self.diff = diff
-        self.tp = tp
-        self.achievement = achievement
-        self.ra = ra
-        self.comboId = comboId
-        self.scoreId = scoreId
-        self.title = title
-        self.ds = ds
-        self.lv = lv
-
-    def __str__(self):
-        return '%-50s' % f'{self.title} [{self.tp}]' + f'{self.ds}\t{diffs[self.diff]}\t{self.ra}'
-
-    def __eq__(self, other):
-        return self.ra == other.ra
-
-    def __lt__(self, other):
-        return self.ra < other.ra
-
-    @classmethod
-    def from_json(cls, data):
-        rate = ['d', 'c', 'b', 'bb', 'bbb', 'a', 'aa', 'aaa', 's', 'sp', 'ss', 'ssp', 'sss', 'sssp']
-        ri = rate.index(data["rate"])
-        fc = ['', 'fc', 'fcp', 'ap', 'app']
-        fi = fc.index(data["fc"])
-        return cls(
-            idNum=total_list.by_title(data["title"]).id,
-            title=data["title"],
-            diff=data["level_index"],
-            ra=data["ra"],
-            ds=data["ds"],
-            comboId=fi,
-            scoreId=ri,
-            lv=data["level"],
-            achievement=data["achievements"],
-            tp=data["type"]
-        )
-
-
-
-class BestList(object):
-
-    def __init__(self, size:int):
-        self.data = []
-        self.size = size
-
-    def push(self, elem:ChartInfo):
-        if len(self.data) >= self.size and elem < self.data[-1]:
-            return
-        self.data.append(elem)
-        self.data.sort()
-        self.data.reverse()
-        while(len(self.data) > self.size):
-            del self.data[-1]
-
-    def pop(self):
-        del self.data[-1]
-
-    def __str__(self):
-        return '[\n\t' + ', \n\t'.join([str(ci) for ci in self.data]) + '\n]'
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        return self.data[index]
-
-
-class DrawBest(object):
-
-    def __init__(self, sdBest:BestList, dxBest:BestList, userName:str, playerRating:int, musicRating:int):
-        self.sdBest = sdBest
-        self.dxBest = dxBest
-        self.userName = self._stringQ2B(userName)
-        self.playerRating = playerRating
-        self.musicRating = musicRating
-        self.rankRating = self.playerRating - self.musicRating
-        self.pic_dir = STATIC + '/mai/pic/'
-        self.cover_dir = STATIC + '/mai/cover/'
-        self.img = Image.open(self.pic_dir + 'UI_TTR_BG_Base_Plus.png').convert('RGBA')
-        self.ROWS_IMG = [2]
-        for i in range(6):
-            self.ROWS_IMG.append(116 + 96 * i)
-        self.COLOUMS_IMG = []
-        for i in range(6):
-            self.COLOUMS_IMG.append(2 + 172 * i)
-        for i in range(4):
-            self.COLOUMS_IMG.append(888 + 172 * i)
-        self.draw()
-
-    def _Q2B(self, uchar):
-        """单个字符 全角转半角"""
-        inside_code = ord(uchar)
-        if inside_code == 0x3000:
-            inside_code = 0x0020
-        else:
-            inside_code -= 0xfee0
-        if inside_code < 0x0020 or inside_code > 0x7e: #转完之后不是半角字符返回原来的字符
-            return uchar
-        return chr(inside_code)
-
-    def _stringQ2B(self, ustring):
-        """把字符串全角转半角"""
-        return "".join([self._Q2B(uchar) for uchar in ustring])
-
-    def _getCharWidth(self, o) -> int:
-        widths = [
-            (126, 1), (159, 0), (687, 1), (710, 0), (711, 1), (727, 0), (733, 1), (879, 0), (1154, 1), (1161, 0),
-            (4347, 1), (4447, 2), (7467, 1), (7521, 0), (8369, 1), (8426, 0), (9000, 1), (9002, 2), (11021, 1),
-            (12350, 2), (12351, 1), (12438, 2), (12442, 0), (19893, 2), (19967, 1), (55203, 2), (63743, 1),
-            (64106, 2), (65039, 1), (65059, 0), (65131, 2), (65279, 1), (65376, 2), (65500, 1), (65510, 2),
-            (120831, 1), (262141, 2), (1114109, 1),
-        ]
-        if o == 0xe or o == 0xf:
-            return 0
-        for num, wid in widths:
-            if o <= num:
-                return wid
-        return 1
-
-    def _coloumWidth(self, s:str):
-        res = 0
-        for ch in s:
-            res += self._getCharWidth(ord(ch))
-        return res
-
-    def _changeColumnWidth(self, s:str, len:int) -> str:
-        res = 0
-        sList = []
-        for ch in s:
-            res += self._getCharWidth(ord(ch))
-            if res <= len:
-                sList.append(ch)
-        return ''.join(sList)
-
-    def _resizePic(self, img:Image.Image, time:float):
-        return img.resize((int(img.size[0] * time), int(img.size[1] * time)))
-
-    def _findRaPic(self) -> str:
-        num = '10'
-        if self.playerRating < 1000:
-            num = '01'
-        elif self.playerRating < 2000:
-            num = '02'
-        elif self.playerRating < 3000:
-            num = '03'
-        elif self.playerRating < 4000:
-            num = '04'
-        elif self.playerRating < 5000:
-            num = '05'
-        elif self.playerRating < 6000:
-            num = '06'
-        elif self.playerRating < 7000:
-            num = '07'
-        elif self.playerRating < 8000:
-            num = '08'
-        elif self.playerRating < 8500:
-            num = '09'
-        return f'UI_CMN_DXRating_S_{num}.png'
-
-    def _drawRating(self, ratingBaseImg:Image.Image):
-        COLOUMS_RATING = [86, 100, 115, 130, 145]
-        theRa = self.playerRating
-        i = 4
-        while theRa:
-            digit = theRa % 10
-            theRa = theRa // 10
-            digitImg = Image.open(self.pic_dir + f'UI_NUM_Drating_{digit}.png').convert('RGBA')
-            digitImg = self._resizePic(digitImg, 0.6)
-            ratingBaseImg.paste(digitImg, (COLOUMS_RATING[i] - 2, 9), mask=digitImg.split()[3])
-            i = i - 1
-        return ratingBaseImg
-
-    def _drawBestList(self, img:Image.Image, sdBest:BestList, dxBest:BestList):
-        itemW = 164
-        itemH = 88
-        Color = [(69, 193, 36), (255, 186, 1), (255, 90, 102), (134, 49, 200), (217, 197, 233)]
-        levelTriagle = [(itemW, 0), (itemW - 27, 0), (itemW, 27)]
-        rankPic = 'D C B BB BBB A AA AAA S Sp SS SSp SSS SSSp'.split(' ')
-        comboPic = ' FC FCp AP APp'.split(' ')
-        imgDraw = ImageDraw.Draw(img)
-        titleFontName = STATIC + '/adobe_simhei.otf'
-        for num in range(0, len(sdBest)):
-            i = num // 5
-            j = num % 5
-            chartInfo = sdBest[num]
-            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
-            if not os.path.exists(pngPath):
-                pngPath = self.cover_dir + '01000.png'
-            temp = Image.open(pngPath).convert('RGB')
-            temp = self._resizePic(temp, itemW / temp.size[0])
-            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
-            temp = temp.filter(ImageFilter.GaussianBlur(3))
-            temp = temp.point(lambda p: int(p * 0.72))
-
-            tempDraw = ImageDraw.Draw(temp)
-            tempDraw.polygon(levelTriagle, Color[chartInfo.diff])
-            font = ImageFont.truetype(titleFontName, 16, encoding='utf-8')
-            title = chartInfo.title
-            if self._coloumWidth(title) > 15:
-                title = self._changeColumnWidth(title, 14) + '...'
-            tempDraw.text((8, 8), title, 'white', font)
-            font = ImageFont.truetype(titleFontName, 14, encoding='utf-8')
-
-            tempDraw.text((7, 28), f'{"%.4f" % chartInfo.achievement}%', 'white', font)
-            rankImg = Image.open(self.pic_dir + f'UI_GAM_Rank_{rankPic[chartInfo.scoreId]}.png').convert('RGBA')
-            rankImg = self._resizePic(rankImg, 0.3)
-            temp.paste(rankImg, (88, 28), rankImg.split()[3])
-            if chartInfo.comboId:
-                comboImg = Image.open(self.pic_dir + f'UI_MSS_MBase_Icon_{comboPic[chartInfo.comboId]}_S.png').convert('RGBA')
-                comboImg = self._resizePic(comboImg, 0.45)
-                temp.paste(comboImg, (119, 27), comboImg.split()[3])
-            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 12, encoding='utf-8')
-            tempDraw.text((8, 44), f'Base: {chartInfo.ds} -> {chartInfo.ra}', 'white', font)
-            font = ImageFont.truetype(STATIC +'/adobe_simhei.otf', 18, encoding='utf-8')
-            tempDraw.text((8, 60), f'#{num + 1}', 'white', font)
-
-            recBase = Image.new('RGBA', (itemW, itemH), 'black')
-            recBase = recBase.point(lambda p: int(p * 0.8))
-            img.paste(recBase, (self.COLOUMS_IMG[j] + 5, self.ROWS_IMG[i + 1] + 5))
-            img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
-        for num in range(len(sdBest), sdBest.size):
-            i = num // 5
-            j = num % 5
-            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
-            temp = self._resizePic(temp, itemW / temp.size[0])
-            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
-            temp = temp.filter(ImageFilter.GaussianBlur(1))
-            img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
-        for num in range(0, len(dxBest)):
-            i = num // 3
-            j = num % 3
-            chartInfo = dxBest[num]
-            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
-            if not os.path.exists(pngPath):
-                pngPath = self.cover_dir + '01000.png'
-            temp = Image.open(pngPath).convert('RGB')
-            temp = self._resizePic(temp, itemW / temp.size[0])
-            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
-            temp = temp.filter(ImageFilter.GaussianBlur(3))
-            temp = temp.point(lambda p: int(p * 0.72))
-
-            tempDraw = ImageDraw.Draw(temp)
-            tempDraw.polygon(levelTriagle, Color[chartInfo.diff])
-            font = ImageFont.truetype(titleFontName, 16, encoding='utf-8')
-            title = chartInfo.title
-            if self._coloumWidth(title) > 15:
-                title = self._changeColumnWidth(title, 14) + '...'
-            tempDraw.text((8, 8), title, 'white', font)
-            font = ImageFont.truetype(titleFontName, 14, encoding='utf-8')
-
-            tempDraw.text((7, 28), f'{"%.4f" % chartInfo.achievement}%', 'white', font)
-            rankImg = Image.open(self.pic_dir + f'UI_GAM_Rank_{rankPic[chartInfo.scoreId]}.png').convert('RGBA')
-            rankImg = self._resizePic(rankImg, 0.3)
-            temp.paste(rankImg, (88, 28), rankImg.split()[3])
-            if chartInfo.comboId:
-                comboImg = Image.open(self.pic_dir + f'UI_MSS_MBase_Icon_{comboPic[chartInfo.comboId]}_S.png').convert(
-                    'RGBA')
-                comboImg = self._resizePic(comboImg, 0.45)
-                temp.paste(comboImg, (119, 27), comboImg.split()[3])
-            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 12, encoding='utf-8')
-            tempDraw.text((8, 44), f'Base: {chartInfo.ds} -> {chartInfo.ra}', 'white', font)
-            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 18, encoding='utf-8')
-            tempDraw.text((8, 60), f'#{num + 1}', 'white', font)
-
-            recBase = Image.new('RGBA', (itemW, itemH), 'black')
-            recBase = recBase.point(lambda p: int(p * 0.8))
-            img.paste(recBase, (self.COLOUMS_IMG[j + 6] + 5, self.ROWS_IMG[i + 1] + 5))
-            img.paste(temp, (self.COLOUMS_IMG[j + 6] + 4, self.ROWS_IMG[i + 1] + 4))
-        for num in range(len(dxBest), dxBest.size):
-            i = num // 3
-            j = num % 3
-            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
-            temp = self._resizePic(temp, itemW / temp.size[0])
-            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
-            temp = temp.filter(ImageFilter.GaussianBlur(1))
-            img.paste(temp, (self.COLOUMS_IMG[j + 6] + 4, self.ROWS_IMG[i + 1] + 4))
-
-    def draw(self):
-        splashLogo = Image.open(self.pic_dir + 'UI_CMN_TabTitle_MaimaiTitle_Ver214.png').convert('RGBA')
-        splashLogo = self._resizePic(splashLogo, 0.65)
-        self.img.paste(splashLogo, (10, 10), mask=splashLogo.split()[3])
-
-        ratingBaseImg = Image.open(self.pic_dir + self._findRaPic()).convert('RGBA')
-        ratingBaseImg = self._drawRating(ratingBaseImg)
-        ratingBaseImg = self._resizePic(ratingBaseImg, 0.85)
-        self.img.paste(ratingBaseImg, (240, 8), mask=ratingBaseImg.split()[3])
-
-        namePlateImg = Image.open(self.pic_dir + 'UI_TST_PlateMask.png').convert('RGBA')
-        namePlateImg = namePlateImg.resize((285, 40))
-        namePlateDraw = ImageDraw.Draw(namePlateImg)
-        font1 = ImageFont.truetype(STATIC + '/msyh.ttc', 28, encoding='unic')
-        namePlateDraw.text((12, 4), ' '.join(list(self.userName)), 'black', font1)
-        nameDxImg = Image.open(self.pic_dir + 'UI_CMN_Name_DX.png').convert('RGBA')
-        nameDxImg = self._resizePic(nameDxImg, 0.9)
-        namePlateImg.paste(nameDxImg, (230, 4), mask=nameDxImg.split()[3])
-        self.img.paste(namePlateImg, (240, 40), mask=namePlateImg.split()[3])
-
-        shougouImg = Image.open(self.pic_dir + 'UI_CMN_Shougou_Rainbow.png').convert('RGBA')
-        shougouDraw = ImageDraw.Draw(shougouImg)
-        font2 = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 14, encoding='utf-8')
-        playCountInfo = f'底分: {self.musicRating} + 段位分: {self.rankRating}'
-        shougouImgW, shougouImgH = shougouImg.size
-        playCountInfoW, playCountInfoH = shougouDraw.textsize(playCountInfo, font2)
-        textPos = ((shougouImgW - playCountInfoW - font2.getoffset(playCountInfo)[0]) / 2, 5)
-        shougouDraw.text((textPos[0] - 1, textPos[1]), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0] + 1, textPos[1]), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0], textPos[1] - 1), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0], textPos[1] + 1), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0] - 1, textPos[1] - 1), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0] + 1, textPos[1] - 1), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0] - 1, textPos[1] + 1), playCountInfo, 'black', font2)
-        shougouDraw.text((textPos[0] + 1, textPos[1] + 1), playCountInfo, 'black', font2)
-        shougouDraw.text(textPos, playCountInfo, 'white', font2)
-        shougouImg = self._resizePic(shougouImg, 1.05)
-        self.img.paste(shougouImg, (240, 83), mask=shougouImg.split()[3])
-
-        self._drawBestList(self.img, self.sdBest, self.dxBest)
-
-        authorBoardImg = Image.open(self.pic_dir + 'UI_CMN_MiniDialog_01.png').convert('RGBA')
-        authorBoardImg = self._resizePic(authorBoardImg, 0.35)
-        authorBoardDraw = ImageDraw.Draw(authorBoardImg)
-        authorBoardDraw.text((31, 28), '   Generated By\nXybBot & Chiyuki', 'black', font2)
-        self.img.paste(authorBoardImg, (1224, 19), mask=authorBoardImg.split()[3])
-
-        dxImg = Image.open(self.pic_dir + 'UI_RSL_MBase_Parts_01.png').convert('RGBA')
-        self.img.paste(dxImg, (890, 65), mask=dxImg.split()[3])
-        sdImg = Image.open(self.pic_dir + 'UI_RSL_MBase_Parts_02.png').convert('RGBA')
-        self.img.paste(sdImg, (758, 65), mask=sdImg.split()[3])
-
-        # self.img.show()
-
-    def getDir(self):
-        return self.img
-
-
-def computeRa(ds: float, achievement:float) -> int:
-    baseRa = 15.0
-    if achievement >= 50 and achievement < 60:
-        baseRa = 5.0
-    elif achievement < 70:
-        baseRa = 6.0
-    elif achievement < 75:
-        baseRa = 7.0
-    elif achievement < 80:
-        baseRa = 7.5
-    elif achievement < 90:
-        baseRa = 8.0
-    elif achievement < 94:
-        baseRa = 9.0
-    elif achievement < 97:
-        baseRa = 9.4
-    elif achievement < 98:
-        baseRa = 10.0
-    elif achievement < 99:
-        baseRa = 11.0
-    elif achievement < 99.5:
-        baseRa = 12.0
-    elif achievement < 99.99:
-        baseRa = 13.0
-    elif achievement < 100:
-        baseRa = 13.5
-    elif achievement < 100.5:
-        baseRa = 14.0
-
-    return math.floor(ds * (min(100.5, achievement) / 100) * baseRa)
-
-
-async def generate(payload: Dict) -> Tuple[Optional[Image.Image], bool]:
-    async with aiohttp.request("POST", "https://www.diving-fish.com/api/maimaidxprober/query/player", json=payload) as resp:
-        if resp.status == 400:
-            return None, 400
-        if resp.status == 403:
-            return None, 403
-        sd_best = BestList(25)
-        dx_best = BestList(15)
-        obj = await resp.json()
-        dx: List[Dict] = obj["charts"]["dx"]
-        sd: List[Dict] = obj["charts"]["sd"]
-        for c in sd:
-            sd_best.push(ChartInfo.from_json(c))
-        for c in dx:
-            dx_best.push(ChartInfo.from_json(c))
-        pic = DrawBest(sd_best, dx_best, obj["nickname"], obj["rating"] + obj["additional_rating"], obj["rating"]).getDir()
-        return pic, 0
+
+import os
+import math
+from typing import Optional, Dict, List, Tuple
+from .tool import STATIC
+import aiohttp
+from PIL import Image, ImageDraw, ImageFont, ImageFilter
+from .maimaidx_music import total_list, get_cover_len5_id
+
+
+scoreRank = 'D C B BB BBB A AA AAA S S+ SS SS+ SSS SSS+'.split(' ')
+combo = ' FC FC+ AP AP+'.split(' ')
+diffs = 'Basic Advanced Expert Master Re:Master'.split(' ')
+
+
+class ChartInfo(object):
+    def __init__(self, idNum:str, diff:int, tp:str, achievement:float, ra:int, comboId:int, scoreId:int,
+                 title:str, ds:float, lv:str):
+        self.idNum = idNum
+        self.diff = diff
+        self.tp = tp
+        self.achievement = achievement
+        self.ra = computeRa(ds,achievement)
+        self.comboId = comboId
+        self.scoreId = scoreId
+        self.title = title
+        self.ds = ds
+        self.lv = lv
+
+    def __str__(self):
+        return '%-50s' % f'{self.title} [{self.tp}]' + f'{self.ds}\t{diffs[self.diff]}\t{self.ra}'
+
+    def __eq__(self, other):
+        return self.ra == other.ra
+
+    def __lt__(self, other):
+        return self.ra < other.ra
+
+    @classmethod
+    def from_json(cls, data):
+        rate = ['d', 'c', 'b', 'bb', 'bbb', 'a', 'aa', 'aaa', 's', 'sp', 'ss', 'ssp', 'sss', 'sssp']
+        ri = rate.index(data["rate"])
+        fc = ['', 'fc', 'fcp', 'ap', 'app']
+        fi = fc.index(data["fc"])
+        return cls(
+            idNum=total_list.by_title(data["title"]).id,
+            title=data["title"],
+            diff=data["level_index"],
+            ra=data["ra"],
+            ds=data["ds"],
+            comboId=fi,
+            scoreId=ri,
+            lv=data["level"],
+            achievement=data["achievements"],
+            tp=data["type"]
+        )
+
+
+
+class BestList(object):
+
+    def __init__(self, size:int):
+        self.data = []
+        self.size = size
+
+    def push(self, elem:ChartInfo):
+        if len(self.data) >= self.size and elem < self.data[-1]:
+            return
+        self.data.append(elem)
+        self.data.sort()
+        self.data.reverse()
+        while(len(self.data) > self.size):
+            del self.data[-1]
+
+    def pop(self):
+        del self.data[-1]
+
+    def __str__(self):
+        return '[\n\t' + ', \n\t'.join([str(ci) for ci in self.data]) + '\n]'
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        return self.data[index]
+
+
+class DrawBest(object):
+
+    def __init__(self, sdBest:BestList, dxBest:BestList, userName:str):
+        self.sdBest = sdBest
+        self.dxBest = dxBest
+        self.userName = self._stringQ2B(userName)
+        self.sdRating = 0
+        self.dxRating = 0
+        for sd in sdBest:
+            self.sdRating += computeRa(sd.ds, sd.achievement)
+        for dx in dxBest:
+            self.dxRating += computeRa(dx.ds, dx.achievement)
+        self.playerRating = self.sdRating + self.dxRating
+        self.pic_dir = STATIC + '/mai/pic/'
+        self.cover_dir = STATIC + '/mai/cover/'
+        self.img = Image.open(self.pic_dir + 'UI_TTR_BG_Base_Plus.png').convert('RGBA')
+        self.ROWS_IMG = [2]
+        for i in range(6):
+            self.ROWS_IMG.append(116 + 96 * i)
+        self.COLOUMS_IMG = []
+        for i in range(8):
+            self.COLOUMS_IMG.append(2 + 138 * i)
+        for i in range(4):
+            self.COLOUMS_IMG.append(988 + 138 * i)
+        self.draw()
+
+    def _Q2B(self, uchar):
+        """单个字符 全角转半角"""
+        inside_code = ord(uchar)
+        if inside_code == 0x3000:
+            inside_code = 0x0020
+        else:
+            inside_code -= 0xfee0
+        if inside_code < 0x0020 or inside_code > 0x7e: #转完之后不是半角字符返回原来的字符
+            return uchar
+        return chr(inside_code)
+
+    def _stringQ2B(self, ustring):
+        """把字符串全角转半角"""
+        return "".join([self._Q2B(uchar) for uchar in ustring])
+
+    def _getCharWidth(self, o) -> int:
+        widths = [
+            (126, 1), (159, 0), (687, 1), (710, 0), (711, 1), (727, 0), (733, 1), (879, 0), (1154, 1), (1161, 0),
+            (4347, 1), (4447, 2), (7467, 1), (7521, 0), (8369, 1), (8426, 0), (9000, 1), (9002, 2), (11021, 1),
+            (12350, 2), (12351, 1), (12438, 2), (12442, 0), (19893, 2), (19967, 1), (55203, 2), (63743, 1),
+            (64106, 2), (65039, 1), (65059, 0), (65131, 2), (65279, 1), (65376, 2), (65500, 1), (65510, 2),
+            (120831, 1), (262141, 2), (1114109, 1),
+        ]
+        if o == 0xe or o == 0xf:
+            return 0
+        for num, wid in widths:
+            if o <= num:
+                return wid
+        return 1
+
+    def _coloumWidth(self, s:str):
+        res = 0
+        for ch in s:
+            res += self._getCharWidth(ord(ch))
+        return res
+
+    def _changeColumnWidth(self, s:str, len:int) -> str:
+        res = 0
+        sList = []
+        for ch in s:
+            res += self._getCharWidth(ord(ch))
+            if res <= len:
+                sList.append(ch)
+        return ''.join(sList)
+
+    def _resizePic(self, img:Image.Image, time:float):
+        return img.resize((int(img.size[0] * time), int(img.size[1] * time)))
+
+    def _findRaPic(self) -> str:
+        num = '10'
+        if self.playerRating < 1000:
+            num = '01'
+        elif self.playerRating < 2000:
+            num = '02'
+        elif self.playerRating < 4000:
+            num = '03'
+        elif self.playerRating < 7000:
+            num = '04'
+        elif self.playerRating < 10000:
+            num = '05'
+        elif self.playerRating < 12000:
+            num = '06'
+        elif self.playerRating < 13000:
+            num = '07'
+        elif self.playerRating < 14500:
+            num = '08'
+        elif self.playerRating < 15000:
+            num = '09'
+        return f'UI_CMN_DXRating_S_{num}.png'
+
+    def _drawRating(self, ratingBaseImg:Image.Image):
+        COLOUMS_RATING = [86, 100, 115, 130, 145]
+        theRa = self.playerRating
+        i = 4
+        while theRa:
+            digit = theRa % 10
+            theRa = theRa // 10
+            digitImg = Image.open(self.pic_dir + f'UI_NUM_Drating_{digit}.png').convert('RGBA')
+            digitImg = self._resizePic(digitImg, 0.6)
+            ratingBaseImg.paste(digitImg, (COLOUMS_RATING[i] - 2, 9), mask=digitImg.split()[3])
+            i = i - 1
+        return ratingBaseImg
+
+    def _drawBestList(self, img:Image.Image, sdBest:BestList, dxBest:BestList):
+        itemW = 131
+        itemH = 88
+        Color = [(69, 193, 36), (255, 186, 1), (255, 90, 102), (134, 49, 200), (217, 197, 233)]
+        levelTriagle = [(itemW, 0), (itemW - 27, 0), (itemW, 27)]
+        rankPic = 'D C B BB BBB A AA AAA S Sp SS SSp SSS SSSp'.split(' ')
+        comboPic = ' FC FCp AP APp'.split(' ')
+        imgDraw = ImageDraw.Draw(img)
+        titleFontName = STATIC + '/adobe_simhei.otf'
+        for num in range(0, len(sdBest)):
+            i = num // 7
+            j = num % 7
+            chartInfo = sdBest[num]
+            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
+            if not os.path.exists(pngPath):
+                pngPath = self.cover_dir + '01000.png'
+            temp = Image.open(pngPath).convert('RGB')
+            temp = self._resizePic(temp, itemW / temp.size[0])
+            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
+            temp = temp.filter(ImageFilter.GaussianBlur(3))
+            temp = temp.point(lambda p: int(p * 0.72))
+
+            tempDraw = ImageDraw.Draw(temp)
+            tempDraw.polygon(levelTriagle, Color[chartInfo.diff])
+            font = ImageFont.truetype(titleFontName, 16, encoding='utf-8')
+            title = chartInfo.title
+            if self._coloumWidth(title) > 15:
+                title = self._changeColumnWidth(title, 12) + '...'
+            tempDraw.text((8, 8), title, 'white', font)
+            font = ImageFont.truetype(titleFontName, 12, encoding='utf-8')
+
+            tempDraw.text((7, 28), f'{"%.4f" % chartInfo.achievement}%', 'white', font)
+            rankImg = Image.open(self.pic_dir + f'UI_GAM_Rank_{rankPic[chartInfo.scoreId]}.png').convert('RGBA')
+            rankImg = self._resizePic(rankImg, 0.3)
+            temp.paste(rankImg, (72, 28), rankImg.split()[3])
+            if chartInfo.comboId:
+                comboImg = Image.open(self.pic_dir + f'UI_MSS_MBase_Icon_{comboPic[chartInfo.comboId]}_S.png').convert('RGBA')
+                comboImg = self._resizePic(comboImg, 0.45)
+                temp.paste(comboImg, (103, 27), comboImg.split()[3])
+            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 12, encoding='utf-8')
+            tempDraw.text((8, 44), f'Base: {chartInfo.ds} -> {computeRa(chartInfo.ds, chartInfo.achievement)}', 'white', font)
+            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 18, encoding='utf-8')
+            tempDraw.text((8, 60), f'#{num + 1}', 'white', font)
+
+            recBase = Image.new('RGBA', (itemW, itemH), 'black')
+            recBase = recBase.point(lambda p: int(p * 0.8))
+            img.paste(recBase, (self.COLOUMS_IMG[j] + 5, self.ROWS_IMG[i + 1] + 5))
+            img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
+        for num in range(len(sdBest), sdBest.size):
+            i = num // 7
+            j = num % 7
+            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
+            temp = self._resizePic(temp, itemW / temp.size[0])
+            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
+            temp = temp.filter(ImageFilter.GaussianBlur(1))
+            img.paste(temp, (self.COLOUMS_IMG[j] + 4, self.ROWS_IMG[i + 1] + 4))
+        for num in range(0, len(dxBest)):
+            i = num // 3
+            j = num % 3
+            chartInfo = dxBest[num]
+            pngPath = self.cover_dir + f'{get_cover_len5_id(chartInfo.idNum)}.png'
+            if not os.path.exists(pngPath):
+                pngPath = self.cover_dir + '01000.png'
+            temp = Image.open(pngPath).convert('RGB')
+            temp = self._resizePic(temp, itemW / temp.size[0])
+            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
+            temp = temp.filter(ImageFilter.GaussianBlur(3))
+            temp = temp.point(lambda p: int(p * 0.72))
+
+            tempDraw = ImageDraw.Draw(temp)
+            tempDraw.polygon(levelTriagle, Color[chartInfo.diff])
+            font = ImageFont.truetype(titleFontName, 14, encoding='utf-8')
+            title = chartInfo.title
+            if self._coloumWidth(title) > 13:
+                title = self._changeColumnWidth(title, 12) + '...'
+            tempDraw.text((8, 8), title, 'white', font)
+            font = ImageFont.truetype(titleFontName, 12, encoding='utf-8')
+
+            tempDraw.text((7, 28), f'{"%.4f" % chartInfo.achievement}%', 'white', font)
+            rankImg = Image.open(self.pic_dir + f'UI_GAM_Rank_{rankPic[chartInfo.scoreId]}.png').convert('RGBA')
+            rankImg = self._resizePic(rankImg, 0.3)
+            temp.paste(rankImg, (72, 28), rankImg.split()[3])
+            if chartInfo.comboId:
+                comboImg = Image.open(self.pic_dir + f'UI_MSS_MBase_Icon_{comboPic[chartInfo.comboId]}_S.png').convert(
+                    'RGBA')
+                comboImg = self._resizePic(comboImg, 0.45)
+                temp.paste(comboImg, (103, 27), comboImg.split()[3])
+            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 12, encoding='utf-8')
+            tempDraw.text((8, 44), f'Base: {chartInfo.ds} -> {chartInfo.ra}', 'white', font)
+            font = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 18, encoding='utf-8')
+            tempDraw.text((8, 60), f'#{num + 1}', 'white', font)
+
+            recBase = Image.new('RGBA', (itemW, itemH), 'black')
+            recBase = recBase.point(lambda p: int(p * 0.8))
+            img.paste(recBase, (self.COLOUMS_IMG[j + 8] + 5, self.ROWS_IMG[i + 1] + 5))
+            img.paste(temp, (self.COLOUMS_IMG[j + 8] + 4, self.ROWS_IMG[i + 1] + 4))
+        for num in range(len(dxBest), dxBest.size):
+            i = num // 3
+            j = num % 3
+            temp = Image.open(self.cover_dir + f'01000.png').convert('RGB')
+            temp = self._resizePic(temp, itemW / temp.size[0])
+            temp = temp.crop((0, (temp.size[1] - itemH) / 2, itemW, (temp.size[1] + itemH) / 2))
+            temp = temp.filter(ImageFilter.GaussianBlur(1))
+            img.paste(temp, (self.COLOUMS_IMG[j + 8] + 4, self.ROWS_IMG[i + 1] + 4))
+
+    def draw(self):
+        splashLogo = Image.open(self.pic_dir + 'UI_CMN_TabTitle_MaimaiTitle_Ver214.png').convert('RGBA')
+        splashLogo = self._resizePic(splashLogo, 0.65)
+        self.img.paste(splashLogo, (10, 10), mask=splashLogo.split()[3])
+
+        ratingBaseImg = Image.open(self.pic_dir + self._findRaPic()).convert('RGBA')
+        ratingBaseImg = self._drawRating(ratingBaseImg)
+        ratingBaseImg = self._resizePic(ratingBaseImg, 0.85)
+        self.img.paste(ratingBaseImg, (240, 8), mask=ratingBaseImg.split()[3])
+
+        namePlateImg = Image.open(self.pic_dir + 'UI_TST_PlateMask.png').convert('RGBA')
+        namePlateImg = namePlateImg.resize((285, 40))
+        namePlateDraw = ImageDraw.Draw(namePlateImg)
+        font1 = ImageFont.truetype(STATIC + '/msyh.ttc', 28, encoding='unic')
+        namePlateDraw.text((12, 4), ' '.join(list(self.userName)), 'black', font1)
+        nameDxImg = Image.open(self.pic_dir + 'UI_CMN_Name_DX.png').convert('RGBA')
+        nameDxImg = self._resizePic(nameDxImg, 0.9)
+        namePlateImg.paste(nameDxImg, (230, 4), mask=nameDxImg.split()[3])
+        self.img.paste(namePlateImg, (240, 40), mask=namePlateImg.split()[3])
+
+        shougouImg = Image.open(self.pic_dir + 'UI_CMN_Shougou_Rainbow.png').convert('RGBA')
+        shougouDraw = ImageDraw.Draw(shougouImg)
+        font2 = ImageFont.truetype(STATIC + '/adobe_simhei.otf', 14, encoding='utf-8')
+        playCountInfo = f'SD: {self.sdRating} + DX: {self.dxRating} = {self.playerRating}'
+        shougouImgW, shougouImgH = shougouImg.size
+        playCountInfoW, playCountInfoH = shougouDraw.textsize(playCountInfo, font2)
+        textPos = ((shougouImgW - playCountInfoW - font2.getoffset(playCountInfo)[0]) / 2, 5)
+        shougouDraw.text((textPos[0] - 1, textPos[1]), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0] + 1, textPos[1]), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0], textPos[1] - 1), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0], textPos[1] + 1), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0] - 1, textPos[1] - 1), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0] + 1, textPos[1] - 1), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0] - 1, textPos[1] + 1), playCountInfo, 'black', font2)
+        shougouDraw.text((textPos[0] + 1, textPos[1] + 1), playCountInfo, 'black', font2)
+        shougouDraw.text(textPos, playCountInfo, 'white', font2)
+        shougouImg = self._resizePic(shougouImg, 1.05)
+        self.img.paste(shougouImg, (240, 83), mask=shougouImg.split()[3])
+
+        self._drawBestList(self.img, self.sdBest, self.dxBest)
+
+        authorBoardImg = Image.open(self.pic_dir + 'UI_CMN_MiniDialog_01.png').convert('RGBA')
+        authorBoardImg = self._resizePic(authorBoardImg, 0.35)
+        authorBoardDraw = ImageDraw.Draw(authorBoardImg)
+        authorBoardDraw.text((31, 28), '   Generated By\nXybBot & Chiyuki', 'black', font2)
+        self.img.paste(authorBoardImg, (1224, 19), mask=authorBoardImg.split()[3])
+
+        dxImg = Image.open(self.pic_dir + 'UI_RSL_MBase_Parts_01.png').convert('RGBA')
+        self.img.paste(dxImg, (988, 65), mask=dxImg.split()[3])
+        sdImg = Image.open(self.pic_dir + 'UI_RSL_MBase_Parts_02.png').convert('RGBA')
+        self.img.paste(sdImg, (865, 65), mask=sdImg.split()[3])
+
+        # self.img.show()
+
+    def getDir(self):
+        return self.img
+
+
+def computeRa(ds: float, achievement: float) -> int:
+    baseRa = 22.4 
+    if achievement < 50:
+        baseRa = 7.0
+    elif achievement < 60:
+        baseRa = 8.0 
+    elif achievement < 70:
+        baseRa = 9.6 
+    elif achievement < 75:
+        baseRa = 11.2 
+    elif achievement < 80:
+        baseRa = 12.0 
+    elif achievement < 90:
+        baseRa = 13.6 
+    elif achievement < 94:
+        baseRa = 15.2 
+    elif achievement < 97:
+        baseRa = 16.8 
+    elif achievement < 98:
+        baseRa = 20.0 
+    elif achievement < 99:
+        baseRa = 20.3
+    elif achievement < 99.5:
+        baseRa = 20.8 
+    elif achievement < 100:
+        baseRa = 21.1 
+    elif achievement < 100.5:
+        baseRa = 21.6 
+
+    return math.floor(ds * (min(100.5, achievement) / 100) * baseRa)
+
+
+async def generate50(payload: Dict) -> Tuple[Optional[Image.Image], bool]:
+    async with aiohttp.request("POST", "https://www.diving-fish.com/api/maimaidxprober/query/player", json=payload) as resp:
+        if resp.status == 400:
+            return None, 400
+        if resp.status == 403:
+            return None, 403
+        sd_best = BestList(35)
+        dx_best = BestList(15)
+        obj = await resp.json()
+        dx: List[Dict] = obj["charts"]["dx"]
+        sd: List[Dict] = obj["charts"]["sd"]
+        for c in sd:
+            sd_best.push(ChartInfo.from_json(c))
+        for c in dx:
+            dx_best.push(ChartInfo.from_json(c))
+        pic = DrawBest(sd_best, dx_best, obj["nickname"]).getDir()
+        return pic, 0
```

### Comparing `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1121 +1,1090 @@
-00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
-00000010: 6f72 7420 6d61 7468 0d0a 6672 6f6d 2074  ort math..from t
-00000020: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
-00000030: 696f 6e61 6c2c 2044 6963 742c 204c 6973  ional, Dict, Lis
-00000040: 742c 2054 7570 6c65 0d0a 6672 6f6d 202e  t, Tuple..from .
-00000050: 746f 6f6c 2069 6d70 6f72 7420 5354 4154  tool import STAT
-00000060: 4943 0d0a 696d 706f 7274 2061 696f 6874  IC..import aioht
-00000070: 7470 0d0a 6672 6f6d 2050 494c 2069 6d70  tp..from PIL imp
-00000080: 6f72 7420 496d 6167 652c 2049 6d61 6765  ort Image, Image
-00000090: 4472 6177 2c20 496d 6167 6546 6f6e 742c  Draw, ImageFont,
-000000a0: 2049 6d61 6765 4669 6c74 6572 0d0a 6672   ImageFilter..fr
-000000b0: 6f6d 202e 6d61 696d 6169 6478 5f6d 7573  om .maimaidx_mus
-000000c0: 6963 2069 6d70 6f72 7420 746f 7461 6c5f  ic import total_
-000000d0: 6c69 7374 2c20 6765 745f 636f 7665 725f  list, get_cover_
-000000e0: 6c65 6e35 5f69 640d 0a0d 0a0d 0a73 636f  len5_id......sco
-000000f0: 7265 5261 6e6b 203d 2027 4420 4320 4220  reRank = 'D C B 
-00000100: 4242 2042 4242 2041 2041 4120 4141 4120  BB BBB A AA AAA 
-00000110: 5320 532b 2053 5320 5353 2b20 5353 5320  S S+ SS SS+ SSS 
-00000120: 5353 532b 272e 7370 6c69 7428 2720 2729  SSS+'.split(' ')
-00000130: 0d0a 636f 6d62 6f20 3d20 2720 4643 2046  ..combo = ' FC F
-00000140: 432b 2041 5020 4150 2b27 2e73 706c 6974  C+ AP AP+'.split
-00000150: 2827 2027 290d 0a64 6966 6673 203d 2027  (' ')..diffs = '
-00000160: 4261 7369 6320 4164 7661 6e63 6564 2045  Basic Advanced E
-00000170: 7870 6572 7420 4d61 7374 6572 2052 653a  xpert Master Re:
-00000180: 4d61 7374 6572 272e 7370 6c69 7428 2720  Master'.split(' 
-00000190: 2729 0d0a 0d0a 0d0a 636c 6173 7320 4368  ')......class Ch
-000001a0: 6172 7449 6e66 6f28 6f62 6a65 6374 293a  artInfo(object):
-000001b0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000001c0: 5f5f 2873 656c 662c 2069 644e 756d 3a73  __(self, idNum:s
-000001d0: 7472 2c20 6469 6666 3a69 6e74 2c20 7470  tr, diff:int, tp
-000001e0: 3a73 7472 2c20 6163 6869 6576 656d 656e  :str, achievemen
-000001f0: 743a 666c 6f61 742c 2072 613a 696e 742c  t:float, ra:int,
-00000200: 2063 6f6d 626f 4964 3a69 6e74 2c20 7363   comboId:int, sc
-00000210: 6f72 6549 643a 696e 742c 0d0a 2020 2020  oreId:int,..    
-00000220: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-00000230: 6c65 3a73 7472 2c20 6473 3a66 6c6f 6174  le:str, ds:float
-00000240: 2c20 6c76 3a73 7472 293a 0d0a 2020 2020  , lv:str):..    
-00000250: 2020 2020 7365 6c66 2e69 644e 756d 203d      self.idNum =
-00000260: 2069 644e 756d 0d0a 2020 2020 2020 2020   idNum..        
-00000270: 7365 6c66 2e64 6966 6620 3d20 6469 6666  self.diff = diff
-00000280: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00000290: 7020 3d20 7470 0d0a 2020 2020 2020 2020  p = tp..        
-000002a0: 7365 6c66 2e61 6368 6965 7665 6d65 6e74  self.achievement
-000002b0: 203d 2061 6368 6965 7665 6d65 6e74 0d0a   = achievement..
-000002c0: 2020 2020 2020 2020 7365 6c66 2e72 6120          self.ra 
-000002d0: 3d20 636f 6d70 7574 6552 6128 6473 2c61  = computeRa(ds,a
-000002e0: 6368 6965 7665 6d65 6e74 290d 0a20 2020  chievement)..   
-000002f0: 2020 2020 2073 656c 662e 636f 6d62 6f49       self.comboI
-00000300: 6420 3d20 636f 6d62 6f49 640d 0a20 2020  d = comboId..   
-00000310: 2020 2020 2073 656c 662e 7363 6f72 6549       self.scoreI
-00000320: 6420 3d20 7363 6f72 6549 640d 0a20 2020  d = scoreId..   
-00000330: 2020 2020 2073 656c 662e 7469 746c 6520       self.title 
-00000340: 3d20 7469 746c 650d 0a20 2020 2020 2020  = title..       
-00000350: 2073 656c 662e 6473 203d 2064 730d 0a20   self.ds = ds.. 
-00000360: 2020 2020 2020 2073 656c 662e 6c76 203d         self.lv =
-00000370: 206c 760d 0a0d 0a20 2020 2064 6566 205f   lv....    def _
-00000380: 5f73 7472 5f5f 2873 656c 6629 3a0d 0a20  _str__(self):.. 
-00000390: 2020 2020 2020 2072 6574 7572 6e20 2725         return '%
-000003a0: 2d35 3073 2720 2520 6627 7b73 656c 662e  -50s' % f'{self.
-000003b0: 7469 746c 657d 205b 7b73 656c 662e 7470  title} [{self.tp
-000003c0: 7d5d 2720 2b20 6627 7b73 656c 662e 6473  }]' + f'{self.ds
-000003d0: 7d5c 747b 6469 6666 735b 7365 6c66 2e64  }\t{diffs[self.d
-000003e0: 6966 665d 7d5c 747b 7365 6c66 2e72 617d  iff]}\t{self.ra}
-000003f0: 270d 0a0d 0a20 2020 2064 6566 205f 5f65  '....    def __e
-00000400: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
-00000410: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00000420: 6e20 7365 6c66 2e72 6120 3d3d 206f 7468  n self.ra == oth
-00000430: 6572 2e72 610d 0a0d 0a20 2020 2064 6566  er.ra....    def
-00000440: 205f 5f6c 745f 5f28 7365 6c66 2c20 6f74   __lt__(self, ot
-00000450: 6865 7229 3a0d 0a20 2020 2020 2020 2072  her):..        r
-00000460: 6574 7572 6e20 7365 6c66 2e72 6120 3c20  eturn self.ra < 
-00000470: 6f74 6865 722e 7261 0d0a 0d0a 2020 2020  other.ra....    
-00000480: 4063 6c61 7373 6d65 7468 6f64 0d0a 2020  @classmethod..  
-00000490: 2020 6465 6620 6672 6f6d 5f6a 736f 6e28    def from_json(
-000004a0: 636c 732c 2064 6174 6129 3a0d 0a20 2020  cls, data):..   
-000004b0: 2020 2020 2072 6174 6520 3d20 5b27 6427       rate = ['d'
-000004c0: 2c20 2763 272c 2027 6227 2c20 2762 6227  , 'c', 'b', 'bb'
-000004d0: 2c20 2762 6262 272c 2027 6127 2c20 2761  , 'bbb', 'a', 'a
-000004e0: 6127 2c20 2761 6161 272c 2027 7327 2c20  a', 'aaa', 's', 
-000004f0: 2773 7027 2c20 2773 7327 2c20 2773 7370  'sp', 'ss', 'ssp
-00000500: 272c 2027 7373 7327 2c20 2773 7373 7027  ', 'sss', 'sssp'
-00000510: 5d0d 0a20 2020 2020 2020 2072 6920 3d20  ]..        ri = 
-00000520: 7261 7465 2e69 6e64 6578 2864 6174 615b  rate.index(data[
-00000530: 2272 6174 6522 5d29 0d0a 2020 2020 2020  "rate"])..      
-00000540: 2020 6663 203d 205b 2727 2c20 2766 6327    fc = ['', 'fc'
-00000550: 2c20 2766 6370 272c 2027 6170 272c 2027  , 'fcp', 'ap', '
-00000560: 6170 7027 5d0d 0a20 2020 2020 2020 2066  app']..        f
-00000570: 6920 3d20 6663 2e69 6e64 6578 2864 6174  i = fc.index(dat
-00000580: 615b 2266 6322 5d29 0d0a 2020 2020 2020  a["fc"])..      
-00000590: 2020 7265 7475 726e 2063 6c73 280d 0a20    return cls(.. 
-000005a0: 2020 2020 2020 2020 2020 2069 644e 756d             idNum
-000005b0: 3d74 6f74 616c 5f6c 6973 742e 6279 5f74  =total_list.by_t
-000005c0: 6974 6c65 2864 6174 615b 2274 6974 6c65  itle(data["title
-000005d0: 225d 292e 6964 2c0d 0a20 2020 2020 2020  "]).id,..       
-000005e0: 2020 2020 2074 6974 6c65 3d64 6174 615b       title=data[
-000005f0: 2274 6974 6c65 225d 2c0d 0a20 2020 2020  "title"],..     
-00000600: 2020 2020 2020 2064 6966 663d 6461 7461         diff=data
-00000610: 5b22 6c65 7665 6c5f 696e 6465 7822 5d2c  ["level_index"],
-00000620: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00000630: 3d64 6174 615b 2272 6122 5d2c 0d0a 2020  =data["ra"],..  
-00000640: 2020 2020 2020 2020 2020 6473 3d64 6174            ds=dat
-00000650: 615b 2264 7322 5d2c 0d0a 2020 2020 2020  a["ds"],..      
-00000660: 2020 2020 2020 636f 6d62 6f49 643d 6669        comboId=fi
-00000670: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00000680: 636f 7265 4964 3d72 692c 0d0a 2020 2020  coreId=ri,..    
-00000690: 2020 2020 2020 2020 6c76 3d64 6174 615b          lv=data[
-000006a0: 226c 6576 656c 225d 2c0d 0a20 2020 2020  "level"],..     
-000006b0: 2020 2020 2020 2061 6368 6965 7665 6d65         achieveme
-000006c0: 6e74 3d64 6174 615b 2261 6368 6965 7665  nt=data["achieve
-000006d0: 6d65 6e74 7322 5d2c 0d0a 2020 2020 2020  ments"],..      
-000006e0: 2020 2020 2020 7470 3d64 6174 615b 2274        tp=data["t
-000006f0: 7970 6522 5d0d 0a20 2020 2020 2020 2029  ype"]..        )
-00000700: 0d0a 0d0a 0d0a 0d0a 636c 6173 7320 4265  ........class Be
-00000710: 7374 4c69 7374 286f 626a 6563 7429 3a0d  stList(object):.
-00000720: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00000730: 745f 5f28 7365 6c66 2c20 7369 7a65 3a69  t__(self, size:i
-00000740: 6e74 293a 0d0a 2020 2020 2020 2020 7365  nt):..        se
-00000750: 6c66 2e64 6174 6120 3d20 5b5d 0d0a 2020  lf.data = []..  
-00000760: 2020 2020 2020 7365 6c66 2e73 697a 6520        self.size 
-00000770: 3d20 7369 7a65 0d0a 0d0a 2020 2020 6465  = size....    de
-00000780: 6620 7075 7368 2873 656c 662c 2065 6c65  f push(self, ele
-00000790: 6d3a 4368 6172 7449 6e66 6f29 3a0d 0a20  m:ChartInfo):.. 
-000007a0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-000007b0: 6c66 2e64 6174 6129 203e 3d20 7365 6c66  lf.data) >= self
-000007c0: 2e73 697a 6520 616e 6420 656c 656d 203c  .size and elem <
-000007d0: 2073 656c 662e 6461 7461 5b2d 315d 3a0d   self.data[-1]:.
-000007e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000007f0: 7572 6e0d 0a20 2020 2020 2020 2073 656c  urn..        sel
-00000800: 662e 6461 7461 2e61 7070 656e 6428 656c  f.data.append(el
-00000810: 656d 290d 0a20 2020 2020 2020 2073 656c  em)..        sel
-00000820: 662e 6461 7461 2e73 6f72 7428 290d 0a20  f.data.sort().. 
-00000830: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00000840: 2e72 6576 6572 7365 2829 0d0a 2020 2020  .reverse()..    
-00000850: 2020 2020 7768 696c 6528 6c65 6e28 7365      while(len(se
-00000860: 6c66 2e64 6174 6129 203e 2073 656c 662e  lf.data) > self.
-00000870: 7369 7a65 293a 0d0a 2020 2020 2020 2020  size):..        
-00000880: 2020 2020 6465 6c20 7365 6c66 2e64 6174      del self.dat
-00000890: 615b 2d31 5d0d 0a0d 0a20 2020 2064 6566  a[-1]....    def
-000008a0: 2070 6f70 2873 656c 6629 3a0d 0a20 2020   pop(self):..   
-000008b0: 2020 2020 2064 656c 2073 656c 662e 6461       del self.da
-000008c0: 7461 5b2d 315d 0d0a 0d0a 2020 2020 6465  ta[-1]....    de
-000008d0: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
-000008e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000008f0: 2027 5b5c 6e5c 7427 202b 2027 2c20 5c6e   '[\n\t' + ', \n
-00000900: 5c74 272e 6a6f 696e 285b 7374 7228 6369  \t'.join([str(ci
-00000910: 2920 666f 7220 6369 2069 6e20 7365 6c66  ) for ci in self
-00000920: 2e64 6174 615d 2920 2b20 275c 6e5d 270d  .data]) + '\n]'.
-00000930: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
-00000940: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
-00000950: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
-00000960: 6c66 2e64 6174 6129 0d0a 0d0a 2020 2020  lf.data)....    
-00000970: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
-00000980: 7365 6c66 2c20 696e 6465 7829 3a0d 0a20  self, index):.. 
-00000990: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000009a0: 6c66 2e64 6174 615b 696e 6465 785d 0d0a  lf.data[index]..
-000009b0: 0d0a 0d0a 636c 6173 7320 4472 6177 4265  ....class DrawBe
-000009c0: 7374 286f 626a 6563 7429 3a0d 0a0d 0a20  st(object):.... 
-000009d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000009e0: 7365 6c66 2c20 7364 4265 7374 3a42 6573  self, sdBest:Bes
-000009f0: 744c 6973 742c 2064 7842 6573 743a 4265  tList, dxBest:Be
-00000a00: 7374 4c69 7374 2c20 7573 6572 4e61 6d65  stList, userName
-00000a10: 3a73 7472 293a 0d0a 2020 2020 2020 2020  :str):..        
-00000a20: 7365 6c66 2e73 6442 6573 7420 3d20 7364  self.sdBest = sd
-00000a30: 4265 7374 0d0a 2020 2020 2020 2020 7365  Best..        se
-00000a40: 6c66 2e64 7842 6573 7420 3d20 6478 4265  lf.dxBest = dxBe
-00000a50: 7374 0d0a 2020 2020 2020 2020 7365 6c66  st..        self
-00000a60: 2e75 7365 724e 616d 6520 3d20 7365 6c66  .userName = self
-00000a70: 2e5f 7374 7269 6e67 5132 4228 7573 6572  ._stringQ2B(user
-00000a80: 4e61 6d65 290d 0a20 2020 2020 2020 2073  Name)..        s
-00000a90: 656c 662e 7364 5261 7469 6e67 203d 2030  elf.sdRating = 0
-00000aa0: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-00000ab0: 7852 6174 696e 6720 3d20 300d 0a20 2020  xRating = 0..   
-00000ac0: 2020 2020 2066 6f72 2073 6420 696e 2073       for sd in s
-00000ad0: 6442 6573 743a 0d0a 2020 2020 2020 2020  dBest:..        
-00000ae0: 2020 2020 7365 6c66 2e73 6452 6174 696e      self.sdRatin
-00000af0: 6720 2b3d 2063 6f6d 7075 7465 5261 2873  g += computeRa(s
-00000b00: 642e 6473 2c20 7364 2e61 6368 6965 7665  d.ds, sd.achieve
-00000b10: 6d65 6e74 290d 0a20 2020 2020 2020 2066  ment)..        f
-00000b20: 6f72 2064 7820 696e 2064 7842 6573 743a  or dx in dxBest:
-00000b30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000b40: 6c66 2e64 7852 6174 696e 6720 2b3d 2063  lf.dxRating += c
-00000b50: 6f6d 7075 7465 5261 2864 782e 6473 2c20  omputeRa(dx.ds, 
-00000b60: 6478 2e61 6368 6965 7665 6d65 6e74 290d  dx.achievement).
-00000b70: 0a20 2020 2020 2020 2073 656c 662e 706c  .        self.pl
-00000b80: 6179 6572 5261 7469 6e67 203d 2073 656c  ayerRating = sel
-00000b90: 662e 7364 5261 7469 6e67 202b 2073 656c  f.sdRating + sel
-00000ba0: 662e 6478 5261 7469 6e67 0d0a 2020 2020  f.dxRating..    
-00000bb0: 2020 2020 7365 6c66 2e70 6963 5f64 6972      self.pic_dir
-00000bc0: 203d 2053 5441 5449 4320 2b20 272f 6d61   = STATIC + '/ma
-00000bd0: 692f 7069 632f 270d 0a20 2020 2020 2020  i/pic/'..       
-00000be0: 2073 656c 662e 636f 7665 725f 6469 7220   self.cover_dir 
-00000bf0: 3d20 5354 4154 4943 202b 2027 2f6d 6169  = STATIC + '/mai
-00000c00: 2f63 6f76 6572 2f27 0d0a 2020 2020 2020  /cover/'..      
-00000c10: 2020 7365 6c66 2e69 6d67 203d 2049 6d61    self.img = Ima
-00000c20: 6765 2e6f 7065 6e28 7365 6c66 2e70 6963  ge.open(self.pic
-00000c30: 5f64 6972 202b 2027 5549 5f54 5452 5f42  _dir + 'UI_TTR_B
-00000c40: 475f 4261 7365 5f50 6c75 732e 706e 6727  G_Base_Plus.png'
-00000c50: 292e 636f 6e76 6572 7428 2752 4742 4127  ).convert('RGBA'
-00000c60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000c70: 524f 5753 5f49 4d47 203d 205b 325d 0d0a  ROWS_IMG = [2]..
-00000c80: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00000c90: 2072 616e 6765 2836 293a 0d0a 2020 2020   range(6):..    
-00000ca0: 2020 2020 2020 2020 7365 6c66 2e52 4f57          self.ROW
-00000cb0: 535f 494d 472e 6170 7065 6e64 2831 3136  S_IMG.append(116
-00000cc0: 202b 2039 3620 2a20 6929 0d0a 2020 2020   + 96 * i)..    
-00000cd0: 2020 2020 7365 6c66 2e43 4f4c 4f55 4d53      self.COLOUMS
-00000ce0: 5f49 4d47 203d 205b 5d0d 0a20 2020 2020  _IMG = []..     
-00000cf0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00000d00: 6528 3829 3a0d 0a20 2020 2020 2020 2020  e(8):..         
-00000d10: 2020 2073 656c 662e 434f 4c4f 554d 535f     self.COLOUMS_
-00000d20: 494d 472e 6170 7065 6e64 2832 202b 2031  IMG.append(2 + 1
-00000d30: 3338 202a 2069 290d 0a20 2020 2020 2020  38 * i)..       
-00000d40: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000d50: 3429 3a0d 0a20 2020 2020 2020 2020 2020  4):..           
-00000d60: 2073 656c 662e 434f 4c4f 554d 535f 494d   self.COLOUMS_IM
-00000d70: 472e 6170 7065 6e64 2839 3838 202b 2031  G.append(988 + 1
-00000d80: 3338 202a 2069 290d 0a20 2020 2020 2020  38 * i)..       
-00000d90: 2073 656c 662e 6472 6177 2829 0d0a 0d0a   self.draw()....
-00000da0: 2020 2020 6465 6620 5f51 3242 2873 656c      def _Q2B(sel
-00000db0: 662c 2075 6368 6172 293a 0d0a 2020 2020  f, uchar):..    
-00000dc0: 2020 2020 2222 22e5 8d95 e4b8 aae5 ad97      """.........
-00000dd0: e7ac a620 e585 a8e8 a792 e8bd ace5 8d8a  ... ............
-00000de0: e8a7 9222 2222 0d0a 2020 2020 2020 2020  ..."""..        
-00000df0: 696e 7369 6465 5f63 6f64 6520 3d20 6f72  inside_code = or
-00000e00: 6428 7563 6861 7229 0d0a 2020 2020 2020  d(uchar)..      
-00000e10: 2020 6966 2069 6e73 6964 655f 636f 6465    if inside_code
-00000e20: 203d 3d20 3078 3330 3030 3a0d 0a20 2020   == 0x3000:..   
-00000e30: 2020 2020 2020 2020 2069 6e73 6964 655f           inside_
-00000e40: 636f 6465 203d 2030 7830 3032 300d 0a20  code = 0x0020.. 
-00000e50: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00000e60: 2020 2020 2020 2020 2020 696e 7369 6465            inside
-00000e70: 5f63 6f64 6520 2d3d 2030 7866 6565 300d  _code -= 0xfee0.
-00000e80: 0a20 2020 2020 2020 2069 6620 696e 7369  .        if insi
-00000e90: 6465 5f63 6f64 6520 3c20 3078 3030 3230  de_code < 0x0020
-00000ea0: 206f 7220 696e 7369 6465 5f63 6f64 6520   or inside_code 
-00000eb0: 3e20 3078 3765 3a20 23e8 bdac e5ae 8ce4  > 0x7e: #.......
-00000ec0: b98b e590 8ee4 b88d e698 afe5 8d8a e8a7  ................
-00000ed0: 92e5 ad97 e7ac a6e8 bf94 e59b 9ee5 8e9f  ................
-00000ee0: e69d a5e7 9a84 e5ad 97e7 aca6 0d0a 2020  ..............  
-00000ef0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000f00: 2075 6368 6172 0d0a 2020 2020 2020 2020   uchar..        
-00000f10: 7265 7475 726e 2063 6872 2869 6e73 6964  return chr(insid
-00000f20: 655f 636f 6465 290d 0a0d 0a20 2020 2064  e_code)....    d
-00000f30: 6566 205f 7374 7269 6e67 5132 4228 7365  ef _stringQ2B(se
-00000f40: 6c66 2c20 7573 7472 696e 6729 3a0d 0a20  lf, ustring):.. 
-00000f50: 2020 2020 2020 2022 2222 e68a 8ae5 ad97         """......
-00000f60: e7ac a6e4 b8b2 e585 a8e8 a792 e8bd ace5  ................
-00000f70: 8d8a e8a7 9222 2222 0d0a 2020 2020 2020  ....."""..      
-00000f80: 2020 7265 7475 726e 2022 222e 6a6f 696e    return "".join
-00000f90: 285b 7365 6c66 2e5f 5132 4228 7563 6861  ([self._Q2B(ucha
-00000fa0: 7229 2066 6f72 2075 6368 6172 2069 6e20  r) for uchar in 
-00000fb0: 7573 7472 696e 675d 290d 0a0d 0a20 2020  ustring])....   
-00000fc0: 2064 6566 205f 6765 7443 6861 7257 6964   def _getCharWid
-00000fd0: 7468 2873 656c 662c 206f 2920 2d3e 2069  th(self, o) -> i
-00000fe0: 6e74 3a0d 0a20 2020 2020 2020 2077 6964  nt:..        wid
-00000ff0: 7468 7320 3d20 5b0d 0a20 2020 2020 2020  ths = [..       
-00001000: 2020 2020 2028 3132 362c 2031 292c 2028       (126, 1), (
-00001010: 3135 392c 2030 292c 2028 3638 372c 2031  159, 0), (687, 1
-00001020: 292c 2028 3731 302c 2030 292c 2028 3731  ), (710, 0), (71
-00001030: 312c 2031 292c 2028 3732 372c 2030 292c  1, 1), (727, 0),
-00001040: 2028 3733 332c 2031 292c 2028 3837 392c   (733, 1), (879,
-00001050: 2030 292c 2028 3131 3534 2c20 3129 2c20   0), (1154, 1), 
-00001060: 2831 3136 312c 2030 292c 0d0a 2020 2020  (1161, 0),..    
-00001070: 2020 2020 2020 2020 2834 3334 372c 2031          (4347, 1
-00001080: 292c 2028 3434 3437 2c20 3229 2c20 2837  ), (4447, 2), (7
-00001090: 3436 372c 2031 292c 2028 3735 3231 2c20  467, 1), (7521, 
-000010a0: 3029 2c20 2838 3336 392c 2031 292c 2028  0), (8369, 1), (
-000010b0: 3834 3236 2c20 3029 2c20 2839 3030 302c  8426, 0), (9000,
-000010c0: 2031 292c 2028 3930 3032 2c20 3229 2c20   1), (9002, 2), 
-000010d0: 2831 3130 3231 2c20 3129 2c0d 0a20 2020  (11021, 1),..   
-000010e0: 2020 2020 2020 2020 2028 3132 3335 302c           (12350,
-000010f0: 2032 292c 2028 3132 3335 312c 2031 292c   2), (12351, 1),
-00001100: 2028 3132 3433 382c 2032 292c 2028 3132   (12438, 2), (12
-00001110: 3434 322c 2030 292c 2028 3139 3839 332c  442, 0), (19893,
-00001120: 2032 292c 2028 3139 3936 372c 2031 292c   2), (19967, 1),
-00001130: 2028 3535 3230 332c 2032 292c 2028 3633   (55203, 2), (63
-00001140: 3734 332c 2031 292c 0d0a 2020 2020 2020  743, 1),..      
-00001150: 2020 2020 2020 2836 3431 3036 2c20 3229        (64106, 2)
-00001160: 2c20 2836 3530 3339 2c20 3129 2c20 2836  , (65039, 1), (6
-00001170: 3530 3539 2c20 3029 2c20 2836 3531 3331  5059, 0), (65131
-00001180: 2c20 3229 2c20 2836 3532 3739 2c20 3129  , 2), (65279, 1)
-00001190: 2c20 2836 3533 3736 2c20 3229 2c20 2836  , (65376, 2), (6
-000011a0: 3535 3030 2c20 3129 2c20 2836 3535 3130  5500, 1), (65510
-000011b0: 2c20 3229 2c0d 0a20 2020 2020 2020 2020  , 2),..         
-000011c0: 2020 2028 3132 3038 3331 2c20 3129 2c20     (120831, 1), 
-000011d0: 2832 3632 3134 312c 2032 292c 2028 3131  (262141, 2), (11
-000011e0: 3134 3130 392c 2031 292c 0d0a 2020 2020  14109, 1),..    
-000011f0: 2020 2020 5d0d 0a20 2020 2020 2020 2069      ]..        i
-00001200: 6620 6f20 3d3d 2030 7865 206f 7220 6f20  f o == 0xe or o 
-00001210: 3d3d 2030 7866 3a0d 0a20 2020 2020 2020  == 0xf:..       
-00001220: 2020 2020 2072 6574 7572 6e20 300d 0a20       return 0.. 
-00001230: 2020 2020 2020 2066 6f72 206e 756d 2c20         for num, 
-00001240: 7769 6420 696e 2077 6964 7468 733a 0d0a  wid in widths:..
-00001250: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00001260: 203c 3d20 6e75 6d3a 0d0a 2020 2020 2020   <= num:..      
-00001270: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001280: 2077 6964 0d0a 2020 2020 2020 2020 7265   wid..        re
-00001290: 7475 726e 2031 0d0a 0d0a 2020 2020 6465  turn 1....    de
-000012a0: 6620 5f63 6f6c 6f75 6d57 6964 7468 2873  f _coloumWidth(s
-000012b0: 656c 662c 2073 3a73 7472 293a 0d0a 2020  elf, s:str):..  
-000012c0: 2020 2020 2020 7265 7320 3d20 300d 0a20        res = 0.. 
-000012d0: 2020 2020 2020 2066 6f72 2063 6820 696e         for ch in
-000012e0: 2073 3a0d 0a20 2020 2020 2020 2020 2020   s:..           
-000012f0: 2072 6573 202b 3d20 7365 6c66 2e5f 6765   res += self._ge
-00001300: 7443 6861 7257 6964 7468 286f 7264 2863  tCharWidth(ord(c
-00001310: 6829 290d 0a20 2020 2020 2020 2072 6574  h))..        ret
-00001320: 7572 6e20 7265 730d 0a0d 0a20 2020 2064  urn res....    d
-00001330: 6566 205f 6368 616e 6765 436f 6c75 6d6e  ef _changeColumn
-00001340: 5769 6474 6828 7365 6c66 2c20 733a 7374  Width(self, s:st
-00001350: 722c 206c 656e 3a69 6e74 2920 2d3e 2073  r, len:int) -> s
-00001360: 7472 3a0d 0a20 2020 2020 2020 2072 6573  tr:..        res
-00001370: 203d 2030 0d0a 2020 2020 2020 2020 734c   = 0..        sL
-00001380: 6973 7420 3d20 5b5d 0d0a 2020 2020 2020  ist = []..      
-00001390: 2020 666f 7220 6368 2069 6e20 733a 0d0a    for ch in s:..
-000013a0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-000013b0: 2b3d 2073 656c 662e 5f67 6574 4368 6172  += self._getChar
-000013c0: 5769 6474 6828 6f72 6428 6368 2929 0d0a  Width(ord(ch))..
-000013d0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-000013e0: 6573 203c 3d20 6c65 6e3a 0d0a 2020 2020  es <= len:..    
-000013f0: 2020 2020 2020 2020 2020 2020 734c 6973              sLis
-00001400: 742e 6170 7065 6e64 2863 6829 0d0a 2020  t.append(ch)..  
-00001410: 2020 2020 2020 7265 7475 726e 2027 272e        return ''.
-00001420: 6a6f 696e 2873 4c69 7374 290d 0a0d 0a20  join(sList).... 
-00001430: 2020 2064 6566 205f 7265 7369 7a65 5069     def _resizePi
-00001440: 6328 7365 6c66 2c20 696d 673a 496d 6167  c(self, img:Imag
-00001450: 652e 496d 6167 652c 2074 696d 653a 666c  e.Image, time:fl
-00001460: 6f61 7429 3a0d 0a20 2020 2020 2020 2072  oat):..        r
-00001470: 6574 7572 6e20 696d 672e 7265 7369 7a65  eturn img.resize
-00001480: 2828 696e 7428 696d 672e 7369 7a65 5b30  ((int(img.size[0
-00001490: 5d20 2a20 7469 6d65 292c 2069 6e74 2869  ] * time), int(i
-000014a0: 6d67 2e73 697a 655b 315d 202a 2074 696d  mg.size[1] * tim
-000014b0: 6529 2929 0d0a 0d0a 2020 2020 6465 6620  e)))....    def 
-000014c0: 5f66 696e 6452 6150 6963 2873 656c 6629  _findRaPic(self)
-000014d0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-000014e0: 2020 6e75 6d20 3d20 2731 3027 0d0a 2020    num = '10'..  
-000014f0: 2020 2020 2020 6966 2073 656c 662e 706c        if self.pl
-00001500: 6179 6572 5261 7469 6e67 203c 2031 3030  ayerRating < 100
-00001510: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00001520: 6e75 6d20 3d20 2730 3127 0d0a 2020 2020  num = '01'..    
-00001530: 2020 2020 656c 6966 2073 656c 662e 706c      elif self.pl
-00001540: 6179 6572 5261 7469 6e67 203c 2032 3030  ayerRating < 200
-00001550: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00001560: 6e75 6d20 3d20 2730 3227 0d0a 2020 2020  num = '02'..    
-00001570: 2020 2020 656c 6966 2073 656c 662e 706c      elif self.pl
-00001580: 6179 6572 5261 7469 6e67 203c 2034 3030  ayerRating < 400
-00001590: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000015a0: 6e75 6d20 3d20 2730 3327 0d0a 2020 2020  num = '03'..    
-000015b0: 2020 2020 656c 6966 2073 656c 662e 706c      elif self.pl
-000015c0: 6179 6572 5261 7469 6e67 203c 2037 3030  ayerRating < 700
-000015d0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000015e0: 6e75 6d20 3d20 2730 3427 0d0a 2020 2020  num = '04'..    
-000015f0: 2020 2020 656c 6966 2073 656c 662e 706c      elif self.pl
-00001600: 6179 6572 5261 7469 6e67 203c 2031 3030  ayerRating < 100
-00001610: 3030 3a0d 0a20 2020 2020 2020 2020 2020  00:..           
-00001620: 206e 756d 203d 2027 3035 270d 0a20 2020   num = '05'..   
-00001630: 2020 2020 2065 6c69 6620 7365 6c66 2e70       elif self.p
-00001640: 6c61 7965 7252 6174 696e 6720 3c20 3132  layerRating < 12
-00001650: 3030 303a 0d0a 2020 2020 2020 2020 2020  000:..          
-00001660: 2020 6e75 6d20 3d20 2730 3627 0d0a 2020    num = '06'..  
-00001670: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00001680: 706c 6179 6572 5261 7469 6e67 203c 2031  playerRating < 1
-00001690: 3330 3030 3a0d 0a20 2020 2020 2020 2020  3000:..         
-000016a0: 2020 206e 756d 203d 2027 3037 270d 0a20     num = '07'.. 
-000016b0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-000016c0: 2e70 6c61 7965 7252 6174 696e 6720 3c20  .playerRating < 
-000016d0: 3134 3530 303a 0d0a 2020 2020 2020 2020  14500:..        
-000016e0: 2020 2020 6e75 6d20 3d20 2730 3827 0d0a      num = '08'..
-000016f0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00001700: 662e 706c 6179 6572 5261 7469 6e67 203c  f.playerRating <
-00001710: 2031 3530 3030 3a0d 0a20 2020 2020 2020   15000:..       
-00001720: 2020 2020 206e 756d 203d 2027 3039 270d       num = '09'.
-00001730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001740: 6627 5549 5f43 4d4e 5f44 5852 6174 696e  f'UI_CMN_DXRatin
-00001750: 675f 535f 7b6e 756d 7d2e 706e 6727 0d0a  g_S_{num}.png'..
-00001760: 0d0a 2020 2020 6465 6620 5f64 7261 7752  ..    def _drawR
-00001770: 6174 696e 6728 7365 6c66 2c20 7261 7469  ating(self, rati
-00001780: 6e67 4261 7365 496d 673a 496d 6167 652e  ngBaseImg:Image.
-00001790: 496d 6167 6529 3a0d 0a20 2020 2020 2020  Image):..       
-000017a0: 2043 4f4c 4f55 4d53 5f52 4154 494e 4720   COLOUMS_RATING 
-000017b0: 3d20 5b38 362c 2031 3030 2c20 3131 352c  = [86, 100, 115,
-000017c0: 2031 3330 2c20 3134 355d 0d0a 2020 2020   130, 145]..    
-000017d0: 2020 2020 7468 6552 6120 3d20 7365 6c66      theRa = self
-000017e0: 2e70 6c61 7965 7252 6174 696e 670d 0a20  .playerRating.. 
-000017f0: 2020 2020 2020 2069 203d 2034 0d0a 2020         i = 4..  
-00001800: 2020 2020 2020 7768 696c 6520 7468 6552        while theR
-00001810: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
-00001820: 6469 6769 7420 3d20 7468 6552 6120 2520  digit = theRa % 
-00001830: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
-00001840: 7468 6552 6120 3d20 7468 6552 6120 2f2f  theRa = theRa //
-00001850: 2031 300d 0a20 2020 2020 2020 2020 2020   10..           
-00001860: 2064 6967 6974 496d 6720 3d20 496d 6167   digitImg = Imag
-00001870: 652e 6f70 656e 2873 656c 662e 7069 635f  e.open(self.pic_
-00001880: 6469 7220 2b20 6627 5549 5f4e 554d 5f44  dir + f'UI_NUM_D
-00001890: 7261 7469 6e67 5f7b 6469 6769 747d 2e70  rating_{digit}.p
-000018a0: 6e67 2729 2e63 6f6e 7665 7274 2827 5247  ng').convert('RG
-000018b0: 4241 2729 0d0a 2020 2020 2020 2020 2020  BA')..          
-000018c0: 2020 6469 6769 7449 6d67 203d 2073 656c    digitImg = sel
-000018d0: 662e 5f72 6573 697a 6550 6963 2864 6967  f._resizePic(dig
-000018e0: 6974 496d 672c 2030 2e36 290d 0a20 2020  itImg, 0.6)..   
-000018f0: 2020 2020 2020 2020 2072 6174 696e 6742           ratingB
-00001900: 6173 6549 6d67 2e70 6173 7465 2864 6967  aseImg.paste(dig
-00001910: 6974 496d 672c 2028 434f 4c4f 554d 535f  itImg, (COLOUMS_
-00001920: 5241 5449 4e47 5b69 5d20 2d20 322c 2039  RATING[i] - 2, 9
-00001930: 292c 206d 6173 6b3d 6469 6769 7449 6d67  ), mask=digitImg
-00001940: 2e73 706c 6974 2829 5b33 5d29 0d0a 2020  .split()[3])..  
-00001950: 2020 2020 2020 2020 2020 6920 3d20 6920            i = i 
-00001960: 2d20 310d 0a20 2020 2020 2020 2072 6574  - 1..        ret
-00001970: 7572 6e20 7261 7469 6e67 4261 7365 496d  urn ratingBaseIm
-00001980: 670d 0a0d 0a20 2020 2064 6566 205f 6472  g....    def _dr
-00001990: 6177 4265 7374 4c69 7374 2873 656c 662c  awBestList(self,
-000019a0: 2069 6d67 3a49 6d61 6765 2e49 6d61 6765   img:Image.Image
-000019b0: 2c20 7364 4265 7374 3a42 6573 744c 6973  , sdBest:BestLis
-000019c0: 742c 2064 7842 6573 743a 4265 7374 4c69  t, dxBest:BestLi
-000019d0: 7374 293a 0d0a 2020 2020 2020 2020 6974  st):..        it
-000019e0: 656d 5720 3d20 3133 310d 0a20 2020 2020  emW = 131..     
-000019f0: 2020 2069 7465 6d48 203d 2038 380d 0a20     itemH = 88.. 
-00001a00: 2020 2020 2020 2043 6f6c 6f72 203d 205b         Color = [
-00001a10: 2836 392c 2031 3933 2c20 3336 292c 2028  (69, 193, 36), (
-00001a20: 3235 352c 2031 3836 2c20 3129 2c20 2832  255, 186, 1), (2
-00001a30: 3535 2c20 3930 2c20 3130 3229 2c20 2831  55, 90, 102), (1
-00001a40: 3334 2c20 3439 2c20 3230 3029 2c20 2832  34, 49, 200), (2
-00001a50: 3137 2c20 3139 372c 2032 3333 295d 0d0a  17, 197, 233)]..
-00001a60: 2020 2020 2020 2020 6c65 7665 6c54 7269          levelTri
-00001a70: 6167 6c65 203d 205b 2869 7465 6d57 2c20  agle = [(itemW, 
-00001a80: 3029 2c20 2869 7465 6d57 202d 2032 372c  0), (itemW - 27,
-00001a90: 2030 292c 2028 6974 656d 572c 2032 3729   0), (itemW, 27)
-00001aa0: 5d0d 0a20 2020 2020 2020 2072 616e 6b50  ]..        rankP
-00001ab0: 6963 203d 2027 4420 4320 4220 4242 2042  ic = 'D C B BB B
-00001ac0: 4242 2041 2041 4120 4141 4120 5320 5370  BB A AA AAA S Sp
-00001ad0: 2053 5320 5353 7020 5353 5320 5353 5370   SS SSp SSS SSSp
-00001ae0: 272e 7370 6c69 7428 2720 2729 0d0a 2020  '.split(' ')..  
-00001af0: 2020 2020 2020 636f 6d62 6f50 6963 203d        comboPic =
-00001b00: 2027 2046 4320 4643 7020 4150 2041 5070   ' FC FCp AP APp
-00001b10: 272e 7370 6c69 7428 2720 2729 0d0a 2020  '.split(' ')..  
-00001b20: 2020 2020 2020 696d 6744 7261 7720 3d20        imgDraw = 
-00001b30: 496d 6167 6544 7261 772e 4472 6177 2869  ImageDraw.Draw(i
-00001b40: 6d67 290d 0a20 2020 2020 2020 2074 6974  mg)..        tit
-00001b50: 6c65 466f 6e74 4e61 6d65 203d 2053 5441  leFontName = STA
-00001b60: 5449 4320 2b20 272f 6164 6f62 655f 7369  TIC + '/adobe_si
-00001b70: 6d68 6569 2e6f 7466 270d 0a20 2020 2020  mhei.otf'..     
-00001b80: 2020 2066 6f72 206e 756d 2069 6e20 7261     for num in ra
-00001b90: 6e67 6528 302c 206c 656e 2873 6442 6573  nge(0, len(sdBes
-00001ba0: 7429 293a 0d0a 2020 2020 2020 2020 2020  t)):..          
-00001bb0: 2020 6920 3d20 6e75 6d20 2f2f 2037 0d0a    i = num // 7..
-00001bc0: 2020 2020 2020 2020 2020 2020 6a20 3d20              j = 
-00001bd0: 6e75 6d20 2520 370d 0a20 2020 2020 2020  num % 7..       
-00001be0: 2020 2020 2063 6861 7274 496e 666f 203d       chartInfo =
-00001bf0: 2073 6442 6573 745b 6e75 6d5d 0d0a 2020   sdBest[num]..  
-00001c00: 2020 2020 2020 2020 2020 706e 6750 6174            pngPat
-00001c10: 6820 3d20 7365 6c66 2e63 6f76 6572 5f64  h = self.cover_d
-00001c20: 6972 202b 2066 277b 6765 745f 636f 7665  ir + f'{get_cove
-00001c30: 725f 6c65 6e35 5f69 6428 6368 6172 7449  r_len5_id(chartI
-00001c40: 6e66 6f2e 6964 4e75 6d29 7d2e 706e 6727  nfo.idNum)}.png'
-00001c50: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001c60: 206e 6f74 206f 732e 7061 7468 2e65 7869   not os.path.exi
-00001c70: 7374 7328 706e 6750 6174 6829 3a0d 0a20  sts(pngPath):.. 
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001c90: 6e67 5061 7468 203d 2073 656c 662e 636f  ngPath = self.co
-00001ca0: 7665 725f 6469 7220 2b20 2730 3130 3030  ver_dir + '01000
-00001cb0: 2e70 6e67 270d 0a20 2020 2020 2020 2020  .png'..         
-00001cc0: 2020 2074 656d 7020 3d20 496d 6167 652e     temp = Image.
-00001cd0: 6f70 656e 2870 6e67 5061 7468 292e 636f  open(pngPath).co
-00001ce0: 6e76 6572 7428 2752 4742 2729 0d0a 2020  nvert('RGB')..  
-00001cf0: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-00001d00: 2073 656c 662e 5f72 6573 697a 6550 6963   self._resizePic
-00001d10: 2874 656d 702c 2069 7465 6d57 202f 2074  (temp, itemW / t
-00001d20: 656d 702e 7369 7a65 5b30 5d29 0d0a 2020  emp.size[0])..  
-00001d30: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-00001d40: 2074 656d 702e 6372 6f70 2828 302c 2028   temp.crop((0, (
-00001d50: 7465 6d70 2e73 697a 655b 315d 202d 2069  temp.size[1] - i
-00001d60: 7465 6d48 2920 2f20 322c 2069 7465 6d57  temH) / 2, itemW
-00001d70: 2c20 2874 656d 702e 7369 7a65 5b31 5d20  , (temp.size[1] 
-00001d80: 2b20 6974 656d 4829 202f 2032 2929 0d0a  + itemH) / 2))..
-00001d90: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00001da0: 203d 2074 656d 702e 6669 6c74 6572 2849   = temp.filter(I
-00001db0: 6d61 6765 4669 6c74 6572 2e47 6175 7373  mageFilter.Gauss
-00001dc0: 6961 6e42 6c75 7228 3329 290d 0a20 2020  ianBlur(3))..   
-00001dd0: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
-00001de0: 7465 6d70 2e70 6f69 6e74 286c 616d 6264  temp.point(lambd
-00001df0: 6120 703a 2069 6e74 2870 202a 2030 2e37  a p: int(p * 0.7
-00001e00: 3229 290d 0a0d 0a20 2020 2020 2020 2020  2))....         
-00001e10: 2020 2074 656d 7044 7261 7720 3d20 496d     tempDraw = Im
-00001e20: 6167 6544 7261 772e 4472 6177 2874 656d  ageDraw.Draw(tem
-00001e30: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
-00001e40: 7465 6d70 4472 6177 2e70 6f6c 7967 6f6e  tempDraw.polygon
-00001e50: 286c 6576 656c 5472 6961 676c 652c 2043  (levelTriagle, C
-00001e60: 6f6c 6f72 5b63 6861 7274 496e 666f 2e64  olor[chartInfo.d
-00001e70: 6966 665d 290d 0a20 2020 2020 2020 2020  iff])..         
-00001e80: 2020 2066 6f6e 7420 3d20 496d 6167 6546     font = ImageF
-00001e90: 6f6e 742e 7472 7565 7479 7065 2874 6974  ont.truetype(tit
-00001ea0: 6c65 466f 6e74 4e61 6d65 2c20 3136 2c20  leFontName, 16, 
-00001eb0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-00001ec0: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00001ed0: 6974 6c65 203d 2063 6861 7274 496e 666f  itle = chartInfo
-00001ee0: 2e74 6974 6c65 0d0a 2020 2020 2020 2020  .title..        
-00001ef0: 2020 2020 6966 2073 656c 662e 5f63 6f6c      if self._col
-00001f00: 6f75 6d57 6964 7468 2874 6974 6c65 2920  oumWidth(title) 
-00001f10: 3e20 3135 3a0d 0a20 2020 2020 2020 2020  > 15:..         
-00001f20: 2020 2020 2020 2074 6974 6c65 203d 2073         title = s
-00001f30: 656c 662e 5f63 6861 6e67 6543 6f6c 756d  elf._changeColum
-00001f40: 6e57 6964 7468 2874 6974 6c65 2c20 3132  nWidth(title, 12
-00001f50: 2920 2b20 272e 2e2e 270d 0a20 2020 2020  ) + '...'..     
-00001f60: 2020 2020 2020 2074 656d 7044 7261 772e         tempDraw.
-00001f70: 7465 7874 2828 382c 2038 292c 2074 6974  text((8, 8), tit
-00001f80: 6c65 2c20 2777 6869 7465 272c 2066 6f6e  le, 'white', fon
-00001f90: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00001fa0: 666f 6e74 203d 2049 6d61 6765 466f 6e74  font = ImageFont
-00001fb0: 2e74 7275 6574 7970 6528 7469 746c 6546  .truetype(titleF
-00001fc0: 6f6e 744e 616d 652c 2031 322c 2065 6e63  ontName, 12, enc
-00001fd0: 6f64 696e 673d 2775 7466 2d38 2729 0d0a  oding='utf-8')..
-00001fe0: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00001ff0: 6d70 4472 6177 2e74 6578 7428 2837 2c20  mpDraw.text((7, 
-00002000: 3238 292c 2066 277b 2225 2e34 6622 2025  28), f'{"%.4f" %
-00002010: 2063 6861 7274 496e 666f 2e61 6368 6965   chartInfo.achie
-00002020: 7665 6d65 6e74 7d25 272c 2027 7768 6974  vement}%', 'whit
-00002030: 6527 2c20 666f 6e74 290d 0a20 2020 2020  e', font)..     
-00002040: 2020 2020 2020 2072 616e 6b49 6d67 203d         rankImg =
-00002050: 2049 6d61 6765 2e6f 7065 6e28 7365 6c66   Image.open(self
-00002060: 2e70 6963 5f64 6972 202b 2066 2755 495f  .pic_dir + f'UI_
-00002070: 4741 4d5f 5261 6e6b 5f7b 7261 6e6b 5069  GAM_Rank_{rankPi
-00002080: 635b 6368 6172 7449 6e66 6f2e 7363 6f72  c[chartInfo.scor
-00002090: 6549 645d 7d2e 706e 6727 292e 636f 6e76  eId]}.png').conv
-000020a0: 6572 7428 2752 4742 4127 290d 0a20 2020  ert('RGBA')..   
-000020b0: 2020 2020 2020 2020 2072 616e 6b49 6d67           rankImg
-000020c0: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
-000020d0: 6963 2872 616e 6b49 6d67 2c20 302e 3329  ic(rankImg, 0.3)
-000020e0: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-000020f0: 6d70 2e70 6173 7465 2872 616e 6b49 6d67  mp.paste(rankImg
-00002100: 2c20 2837 322c 2032 3829 2c20 7261 6e6b  , (72, 28), rank
-00002110: 496d 672e 7370 6c69 7428 295b 335d 290d  Img.split()[3]).
-00002120: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002130: 6368 6172 7449 6e66 6f2e 636f 6d62 6f49  chartInfo.comboI
-00002140: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00002150: 2020 2020 636f 6d62 6f49 6d67 203d 2049      comboImg = I
-00002160: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
-00002170: 6963 5f64 6972 202b 2066 2755 495f 4d53  ic_dir + f'UI_MS
-00002180: 535f 4d42 6173 655f 4963 6f6e 5f7b 636f  S_MBase_Icon_{co
-00002190: 6d62 6f50 6963 5b63 6861 7274 496e 666f  mboPic[chartInfo
-000021a0: 2e63 6f6d 626f 4964 5d7d 5f53 2e70 6e67  .comboId]}_S.png
-000021b0: 2729 2e63 6f6e 7665 7274 2827 5247 4241  ').convert('RGBA
-000021c0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-000021d0: 2020 2020 636f 6d62 6f49 6d67 203d 2073      comboImg = s
-000021e0: 656c 662e 5f72 6573 697a 6550 6963 2863  elf._resizePic(c
-000021f0: 6f6d 626f 496d 672c 2030 2e34 3529 0d0a  omboImg, 0.45)..
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 7465 6d70 2e70 6173 7465 2863 6f6d 626f  temp.paste(combo
-00002220: 496d 672c 2028 3130 332c 2032 3729 2c20  Img, (103, 27), 
-00002230: 636f 6d62 6f49 6d67 2e73 706c 6974 2829  comboImg.split()
-00002240: 5b33 5d29 0d0a 2020 2020 2020 2020 2020  [3])..          
-00002250: 2020 666f 6e74 203d 2049 6d61 6765 466f    font = ImageFo
-00002260: 6e74 2e74 7275 6574 7970 6528 5354 4154  nt.truetype(STAT
-00002270: 4943 202b 2027 2f61 646f 6265 5f73 696d  IC + '/adobe_sim
-00002280: 6865 692e 6f74 6627 2c20 3132 2c20 656e  hei.otf', 12, en
-00002290: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
-000022a0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-000022b0: 7044 7261 772e 7465 7874 2828 382c 2034  pDraw.text((8, 4
-000022c0: 3429 2c20 6627 4261 7365 3a20 7b63 6861  4), f'Base: {cha
-000022d0: 7274 496e 666f 2e64 737d 202d 3e20 7b63  rtInfo.ds} -> {c
-000022e0: 6f6d 7075 7465 5261 2863 6861 7274 496e  omputeRa(chartIn
-000022f0: 666f 2e64 732c 2063 6861 7274 496e 666f  fo.ds, chartInfo
-00002300: 2e61 6368 6965 7665 6d65 6e74 297d 272c  .achievement)}',
-00002310: 2027 7768 6974 6527 2c20 666f 6e74 290d   'white', font).
-00002320: 0a20 2020 2020 2020 2020 2020 2066 6f6e  .            fon
-00002330: 7420 3d20 496d 6167 6546 6f6e 742e 7472  t = ImageFont.tr
-00002340: 7565 7479 7065 2853 5441 5449 4320 2b20  uetype(STATIC + 
-00002350: 272f 6164 6f62 655f 7369 6d68 6569 2e6f  '/adobe_simhei.o
-00002360: 7466 272c 2031 382c 2065 6e63 6f64 696e  tf', 18, encodin
-00002370: 673d 2775 7466 2d38 2729 0d0a 2020 2020  g='utf-8')..    
-00002380: 2020 2020 2020 2020 7465 6d70 4472 6177          tempDraw
-00002390: 2e74 6578 7428 2838 2c20 3630 292c 2066  .text((8, 60), f
-000023a0: 2723 7b6e 756d 202b 2031 7d27 2c20 2777  '#{num + 1}', 'w
-000023b0: 6869 7465 272c 2066 6f6e 7429 0d0a 0d0a  hite', font)....
-000023c0: 2020 2020 2020 2020 2020 2020 7265 6342              recB
-000023d0: 6173 6520 3d20 496d 6167 652e 6e65 7728  ase = Image.new(
-000023e0: 2752 4742 4127 2c20 2869 7465 6d57 2c20  'RGBA', (itemW, 
-000023f0: 6974 656d 4829 2c20 2762 6c61 636b 2729  itemH), 'black')
-00002400: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002410: 6342 6173 6520 3d20 7265 6342 6173 652e  cBase = recBase.
-00002420: 706f 696e 7428 6c61 6d62 6461 2070 3a20  point(lambda p: 
-00002430: 696e 7428 7020 2a20 302e 3829 290d 0a20  int(p * 0.8)).. 
-00002440: 2020 2020 2020 2020 2020 2069 6d67 2e70             img.p
-00002450: 6173 7465 2872 6563 4261 7365 2c20 2873  aste(recBase, (s
-00002460: 656c 662e 434f 4c4f 554d 535f 494d 475b  elf.COLOUMS_IMG[
-00002470: 6a5d 202b 2035 2c20 7365 6c66 2e52 4f57  j] + 5, self.ROW
-00002480: 535f 494d 475b 6920 2b20 315d 202b 2035  S_IMG[i + 1] + 5
-00002490: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000024a0: 696d 672e 7061 7374 6528 7465 6d70 2c20  img.paste(temp, 
-000024b0: 2873 656c 662e 434f 4c4f 554d 535f 494d  (self.COLOUMS_IM
-000024c0: 475b 6a5d 202b 2034 2c20 7365 6c66 2e52  G[j] + 4, self.R
-000024d0: 4f57 535f 494d 475b 6920 2b20 315d 202b  OWS_IMG[i + 1] +
-000024e0: 2034 2929 0d0a 2020 2020 2020 2020 666f   4))..        fo
-000024f0: 7220 6e75 6d20 696e 2072 616e 6765 286c  r num in range(l
-00002500: 656e 2873 6442 6573 7429 2c20 7364 4265  en(sdBest), sdBe
-00002510: 7374 2e73 697a 6529 3a0d 0a20 2020 2020  st.size):..     
-00002520: 2020 2020 2020 2069 203d 206e 756d 202f         i = num /
-00002530: 2f20 370d 0a20 2020 2020 2020 2020 2020  / 7..           
-00002540: 206a 203d 206e 756d 2025 2037 0d0a 2020   j = num % 7..  
-00002550: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-00002560: 2049 6d61 6765 2e6f 7065 6e28 7365 6c66   Image.open(self
-00002570: 2e63 6f76 6572 5f64 6972 202b 2066 2730  .cover_dir + f'0
-00002580: 3130 3030 2e70 6e67 2729 2e63 6f6e 7665  1000.png').conve
-00002590: 7274 2827 5247 4227 290d 0a20 2020 2020  rt('RGB')..     
-000025a0: 2020 2020 2020 2074 656d 7020 3d20 7365         temp = se
-000025b0: 6c66 2e5f 7265 7369 7a65 5069 6328 7465  lf._resizePic(te
-000025c0: 6d70 2c20 6974 656d 5720 2f20 7465 6d70  mp, itemW / temp
-000025d0: 2e73 697a 655b 305d 290d 0a20 2020 2020  .size[0])..     
-000025e0: 2020 2020 2020 2074 656d 7020 3d20 7465         temp = te
-000025f0: 6d70 2e63 726f 7028 2830 2c20 2874 656d  mp.crop((0, (tem
-00002600: 702e 7369 7a65 5b31 5d20 2d20 6974 656d  p.size[1] - item
-00002610: 4829 202f 2032 2c20 6974 656d 572c 2028  H) / 2, itemW, (
-00002620: 7465 6d70 2e73 697a 655b 315d 202b 2069  temp.size[1] + i
-00002630: 7465 6d48 2920 2f20 3229 290d 0a20 2020  temH) / 2))..   
-00002640: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
-00002650: 7465 6d70 2e66 696c 7465 7228 496d 6167  temp.filter(Imag
-00002660: 6546 696c 7465 722e 4761 7573 7369 616e  eFilter.Gaussian
-00002670: 426c 7572 2831 2929 0d0a 2020 2020 2020  Blur(1))..      
-00002680: 2020 2020 2020 696d 672e 7061 7374 6528        img.paste(
-00002690: 7465 6d70 2c20 2873 656c 662e 434f 4c4f  temp, (self.COLO
-000026a0: 554d 535f 494d 475b 6a5d 202b 2034 2c20  UMS_IMG[j] + 4, 
-000026b0: 7365 6c66 2e52 4f57 535f 494d 475b 6920  self.ROWS_IMG[i 
-000026c0: 2b20 315d 202b 2034 2929 0d0a 2020 2020  + 1] + 4))..    
-000026d0: 2020 2020 666f 7220 6e75 6d20 696e 2072      for num in r
-000026e0: 616e 6765 2830 2c20 6c65 6e28 6478 4265  ange(0, len(dxBe
-000026f0: 7374 2929 3a0d 0a20 2020 2020 2020 2020  st)):..         
-00002700: 2020 2069 203d 206e 756d 202f 2f20 330d     i = num // 3.
-00002710: 0a20 2020 2020 2020 2020 2020 206a 203d  .            j =
-00002720: 206e 756d 2025 2033 0d0a 2020 2020 2020   num % 3..      
-00002730: 2020 2020 2020 6368 6172 7449 6e66 6f20        chartInfo 
-00002740: 3d20 6478 4265 7374 5b6e 756d 5d0d 0a20  = dxBest[num].. 
-00002750: 2020 2020 2020 2020 2020 2070 6e67 5061             pngPa
-00002760: 7468 203d 2073 656c 662e 636f 7665 725f  th = self.cover_
-00002770: 6469 7220 2b20 6627 7b67 6574 5f63 6f76  dir + f'{get_cov
-00002780: 6572 5f6c 656e 355f 6964 2863 6861 7274  er_len5_id(chart
-00002790: 496e 666f 2e69 644e 756d 297d 2e70 6e67  Info.idNum)}.png
-000027a0: 270d 0a20 2020 2020 2020 2020 2020 2069  '..            i
-000027b0: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
-000027c0: 6973 7473 2870 6e67 5061 7468 293a 0d0a  ists(pngPath):..
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 706e 6750 6174 6820 3d20 7365 6c66 2e63  pngPath = self.c
-000027f0: 6f76 6572 5f64 6972 202b 2027 3031 3030  over_dir + '0100
-00002800: 302e 706e 6727 0d0a 2020 2020 2020 2020  0.png'..        
-00002810: 2020 2020 7465 6d70 203d 2049 6d61 6765      temp = Image
-00002820: 2e6f 7065 6e28 706e 6750 6174 6829 2e63  .open(pngPath).c
-00002830: 6f6e 7665 7274 2827 5247 4227 290d 0a20  onvert('RGB').. 
-00002840: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
-00002850: 3d20 7365 6c66 2e5f 7265 7369 7a65 5069  = self._resizePi
-00002860: 6328 7465 6d70 2c20 6974 656d 5720 2f20  c(temp, itemW / 
-00002870: 7465 6d70 2e73 697a 655b 305d 290d 0a20  temp.size[0]).. 
-00002880: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
-00002890: 3d20 7465 6d70 2e63 726f 7028 2830 2c20  = temp.crop((0, 
-000028a0: 2874 656d 702e 7369 7a65 5b31 5d20 2d20  (temp.size[1] - 
-000028b0: 6974 656d 4829 202f 2032 2c20 6974 656d  itemH) / 2, item
-000028c0: 572c 2028 7465 6d70 2e73 697a 655b 315d  W, (temp.size[1]
-000028d0: 202b 2069 7465 6d48 2920 2f20 3229 290d   + itemH) / 2)).
-000028e0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-000028f0: 7020 3d20 7465 6d70 2e66 696c 7465 7228  p = temp.filter(
-00002900: 496d 6167 6546 696c 7465 722e 4761 7573  ImageFilter.Gaus
-00002910: 7369 616e 426c 7572 2833 2929 0d0a 2020  sianBlur(3))..  
-00002920: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-00002930: 2074 656d 702e 706f 696e 7428 6c61 6d62   temp.point(lamb
-00002940: 6461 2070 3a20 696e 7428 7020 2a20 302e  da p: int(p * 0.
-00002950: 3732 2929 0d0a 0d0a 2020 2020 2020 2020  72))....        
-00002960: 2020 2020 7465 6d70 4472 6177 203d 2049      tempDraw = I
-00002970: 6d61 6765 4472 6177 2e44 7261 7728 7465  mageDraw.Draw(te
-00002980: 6d70 290d 0a20 2020 2020 2020 2020 2020  mp)..           
-00002990: 2074 656d 7044 7261 772e 706f 6c79 676f   tempDraw.polygo
-000029a0: 6e28 6c65 7665 6c54 7269 6167 6c65 2c20  n(levelTriagle, 
-000029b0: 436f 6c6f 725b 6368 6172 7449 6e66 6f2e  Color[chartInfo.
-000029c0: 6469 6666 5d29 0d0a 2020 2020 2020 2020  diff])..        
-000029d0: 2020 2020 666f 6e74 203d 2049 6d61 6765      font = Image
-000029e0: 466f 6e74 2e74 7275 6574 7970 6528 7469  Font.truetype(ti
-000029f0: 746c 6546 6f6e 744e 616d 652c 2031 342c  tleFontName, 14,
-00002a00: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
-00002a10: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00002a20: 7469 746c 6520 3d20 6368 6172 7449 6e66  title = chartInf
-00002a30: 6f2e 7469 746c 650d 0a20 2020 2020 2020  o.title..       
-00002a40: 2020 2020 2069 6620 7365 6c66 2e5f 636f       if self._co
-00002a50: 6c6f 756d 5769 6474 6828 7469 746c 6529  loumWidth(title)
-00002a60: 203e 2031 333a 0d0a 2020 2020 2020 2020   > 13:..        
-00002a70: 2020 2020 2020 2020 7469 746c 6520 3d20          title = 
-00002a80: 7365 6c66 2e5f 6368 616e 6765 436f 6c75  self._changeColu
-00002a90: 6d6e 5769 6474 6828 7469 746c 652c 2031  mnWidth(title, 1
-00002aa0: 3229 202b 2027 2e2e 2e27 0d0a 2020 2020  2) + '...'..    
-00002ab0: 2020 2020 2020 2020 7465 6d70 4472 6177          tempDraw
-00002ac0: 2e74 6578 7428 2838 2c20 3829 2c20 7469  .text((8, 8), ti
-00002ad0: 746c 652c 2027 7768 6974 6527 2c20 666f  tle, 'white', fo
-00002ae0: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00002af0: 2066 6f6e 7420 3d20 496d 6167 6546 6f6e   font = ImageFon
-00002b00: 742e 7472 7565 7479 7065 2874 6974 6c65  t.truetype(title
-00002b10: 466f 6e74 4e61 6d65 2c20 3132 2c20 656e  FontName, 12, en
-00002b20: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
-00002b30: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
-00002b40: 656d 7044 7261 772e 7465 7874 2828 372c  empDraw.text((7,
-00002b50: 2032 3829 2c20 6627 7b22 252e 3466 2220   28), f'{"%.4f" 
-00002b60: 2520 6368 6172 7449 6e66 6f2e 6163 6869  % chartInfo.achi
-00002b70: 6576 656d 656e 747d 2527 2c20 2777 6869  evement}%', 'whi
-00002b80: 7465 272c 2066 6f6e 7429 0d0a 2020 2020  te', font)..    
-00002b90: 2020 2020 2020 2020 7261 6e6b 496d 6720          rankImg 
-00002ba0: 3d20 496d 6167 652e 6f70 656e 2873 656c  = Image.open(sel
-00002bb0: 662e 7069 635f 6469 7220 2b20 6627 5549  f.pic_dir + f'UI
-00002bc0: 5f47 414d 5f52 616e 6b5f 7b72 616e 6b50  _GAM_Rank_{rankP
-00002bd0: 6963 5b63 6861 7274 496e 666f 2e73 636f  ic[chartInfo.sco
-00002be0: 7265 4964 5d7d 2e70 6e67 2729 2e63 6f6e  reId]}.png').con
-00002bf0: 7665 7274 2827 5247 4241 2729 0d0a 2020  vert('RGBA')..  
-00002c00: 2020 2020 2020 2020 2020 7261 6e6b 496d            rankIm
-00002c10: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
-00002c20: 5069 6328 7261 6e6b 496d 672c 2030 2e33  Pic(rankImg, 0.3
-00002c30: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00002c40: 656d 702e 7061 7374 6528 7261 6e6b 496d  emp.paste(rankIm
-00002c50: 672c 2028 3732 2c20 3238 292c 2072 616e  g, (72, 28), ran
-00002c60: 6b49 6d67 2e73 706c 6974 2829 5b33 5d29  kImg.split()[3])
-00002c70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00002c80: 2063 6861 7274 496e 666f 2e63 6f6d 626f   chartInfo.combo
-00002c90: 4964 3a0d 0a20 2020 2020 2020 2020 2020  Id:..           
-00002ca0: 2020 2020 2063 6f6d 626f 496d 6720 3d20       comboImg = 
-00002cb0: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
-00002cc0: 7069 635f 6469 7220 2b20 6627 5549 5f4d  pic_dir + f'UI_M
-00002cd0: 5353 5f4d 4261 7365 5f49 636f 6e5f 7b63  SS_MBase_Icon_{c
-00002ce0: 6f6d 626f 5069 635b 6368 6172 7449 6e66  omboPic[chartInf
-00002cf0: 6f2e 636f 6d62 6f49 645d 7d5f 532e 706e  o.comboId]}_S.pn
-00002d00: 6727 292e 636f 6e76 6572 7428 0d0a 2020  g').convert(..  
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2752 4742 4127 290d 0a20 2020 2020    'RGBA')..     
-00002d30: 2020 2020 2020 2020 2020 2063 6f6d 626f             combo
-00002d40: 496d 6720 3d20 7365 6c66 2e5f 7265 7369  Img = self._resi
-00002d50: 7a65 5069 6328 636f 6d62 6f49 6d67 2c20  zePic(comboImg, 
-00002d60: 302e 3435 290d 0a20 2020 2020 2020 2020  0.45)..         
-00002d70: 2020 2020 2020 2074 656d 702e 7061 7374         temp.past
-00002d80: 6528 636f 6d62 6f49 6d67 2c20 2831 3033  e(comboImg, (103
-00002d90: 2c20 3237 292c 2063 6f6d 626f 496d 672e  , 27), comboImg.
-00002da0: 7370 6c69 7428 295b 335d 290d 0a20 2020  split()[3])..   
-00002db0: 2020 2020 2020 2020 2066 6f6e 7420 3d20           font = 
-00002dc0: 496d 6167 6546 6f6e 742e 7472 7565 7479  ImageFont.truety
-00002dd0: 7065 2853 5441 5449 4320 2b20 272f 6164  pe(STATIC + '/ad
-00002de0: 6f62 655f 7369 6d68 6569 2e6f 7466 272c  obe_simhei.otf',
-00002df0: 2031 322c 2065 6e63 6f64 696e 673d 2775   12, encoding='u
-00002e00: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
-00002e10: 2020 2020 7465 6d70 4472 6177 2e74 6578      tempDraw.tex
-00002e20: 7428 2838 2c20 3434 292c 2066 2742 6173  t((8, 44), f'Bas
-00002e30: 653a 207b 6368 6172 7449 6e66 6f2e 6473  e: {chartInfo.ds
-00002e40: 7d20 2d3e 207b 6368 6172 7449 6e66 6f2e  } -> {chartInfo.
-00002e50: 7261 7d27 2c20 2777 6869 7465 272c 2066  ra}', 'white', f
-00002e60: 6f6e 7429 0d0a 2020 2020 2020 2020 2020  ont)..          
-00002e70: 2020 666f 6e74 203d 2049 6d61 6765 466f    font = ImageFo
-00002e80: 6e74 2e74 7275 6574 7970 6528 5354 4154  nt.truetype(STAT
-00002e90: 4943 202b 2027 2f61 646f 6265 5f73 696d  IC + '/adobe_sim
-00002ea0: 6865 692e 6f74 6627 2c20 3138 2c20 656e  hei.otf', 18, en
-00002eb0: 636f 6469 6e67 3d27 7574 662d 3827 290d  coding='utf-8').
-00002ec0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00002ed0: 7044 7261 772e 7465 7874 2828 382c 2036  pDraw.text((8, 6
-00002ee0: 3029 2c20 6627 237b 6e75 6d20 2b20 317d  0), f'#{num + 1}
-00002ef0: 272c 2027 7768 6974 6527 2c20 666f 6e74  ', 'white', font
-00002f00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002f10: 2072 6563 4261 7365 203d 2049 6d61 6765   recBase = Image
-00002f20: 2e6e 6577 2827 5247 4241 272c 2028 6974  .new('RGBA', (it
-00002f30: 656d 572c 2069 7465 6d48 292c 2027 626c  emW, itemH), 'bl
-00002f40: 6163 6b27 290d 0a20 2020 2020 2020 2020  ack')..         
-00002f50: 2020 2072 6563 4261 7365 203d 2072 6563     recBase = rec
-00002f60: 4261 7365 2e70 6f69 6e74 286c 616d 6264  Base.point(lambd
-00002f70: 6120 703a 2069 6e74 2870 202a 2030 2e38  a p: int(p * 0.8
-00002f80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00002f90: 696d 672e 7061 7374 6528 7265 6342 6173  img.paste(recBas
-00002fa0: 652c 2028 7365 6c66 2e43 4f4c 4f55 4d53  e, (self.COLOUMS
-00002fb0: 5f49 4d47 5b6a 202b 2038 5d20 2b20 352c  _IMG[j + 8] + 5,
-00002fc0: 2073 656c 662e 524f 5753 5f49 4d47 5b69   self.ROWS_IMG[i
-00002fd0: 202b 2031 5d20 2b20 3529 290d 0a20 2020   + 1] + 5))..   
-00002fe0: 2020 2020 2020 2020 2069 6d67 2e70 6173           img.pas
-00002ff0: 7465 2874 656d 702c 2028 7365 6c66 2e43  te(temp, (self.C
-00003000: 4f4c 4f55 4d53 5f49 4d47 5b6a 202b 2038  OLOUMS_IMG[j + 8
-00003010: 5d20 2b20 342c 2073 656c 662e 524f 5753  ] + 4, self.ROWS
-00003020: 5f49 4d47 5b69 202b 2031 5d20 2b20 3429  _IMG[i + 1] + 4)
-00003030: 290d 0a20 2020 2020 2020 2066 6f72 206e  )..        for n
-00003040: 756d 2069 6e20 7261 6e67 6528 6c65 6e28  um in range(len(
-00003050: 6478 4265 7374 292c 2064 7842 6573 742e  dxBest), dxBest.
-00003060: 7369 7a65 293a 0d0a 2020 2020 2020 2020  size):..        
-00003070: 2020 2020 6920 3d20 6e75 6d20 2f2f 2033      i = num // 3
-00003080: 0d0a 2020 2020 2020 2020 2020 2020 6a20  ..            j 
-00003090: 3d20 6e75 6d20 2520 330d 0a20 2020 2020  = num % 3..     
-000030a0: 2020 2020 2020 2074 656d 7020 3d20 496d         temp = Im
-000030b0: 6167 652e 6f70 656e 2873 656c 662e 636f  age.open(self.co
-000030c0: 7665 725f 6469 7220 2b20 6627 3031 3030  ver_dir + f'0100
-000030d0: 302e 706e 6727 292e 636f 6e76 6572 7428  0.png').convert(
-000030e0: 2752 4742 2729 0d0a 2020 2020 2020 2020  'RGB')..        
-000030f0: 2020 2020 7465 6d70 203d 2073 656c 662e      temp = self.
-00003100: 5f72 6573 697a 6550 6963 2874 656d 702c  _resizePic(temp,
-00003110: 2069 7465 6d57 202f 2074 656d 702e 7369   itemW / temp.si
-00003120: 7a65 5b30 5d29 0d0a 2020 2020 2020 2020  ze[0])..        
-00003130: 2020 2020 7465 6d70 203d 2074 656d 702e      temp = temp.
-00003140: 6372 6f70 2828 302c 2028 7465 6d70 2e73  crop((0, (temp.s
-00003150: 697a 655b 315d 202d 2069 7465 6d48 2920  ize[1] - itemH) 
-00003160: 2f20 322c 2069 7465 6d57 2c20 2874 656d  / 2, itemW, (tem
-00003170: 702e 7369 7a65 5b31 5d20 2b20 6974 656d  p.size[1] + item
-00003180: 4829 202f 2032 2929 0d0a 2020 2020 2020  H) / 2))..      
-00003190: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
-000031a0: 702e 6669 6c74 6572 2849 6d61 6765 4669  p.filter(ImageFi
-000031b0: 6c74 6572 2e47 6175 7373 6961 6e42 6c75  lter.GaussianBlu
-000031c0: 7228 3129 290d 0a20 2020 2020 2020 2020  r(1))..         
-000031d0: 2020 2069 6d67 2e70 6173 7465 2874 656d     img.paste(tem
-000031e0: 702c 2028 7365 6c66 2e43 4f4c 4f55 4d53  p, (self.COLOUMS
-000031f0: 5f49 4d47 5b6a 202b 2038 5d20 2b20 342c  _IMG[j + 8] + 4,
-00003200: 2073 656c 662e 524f 5753 5f49 4d47 5b69   self.ROWS_IMG[i
-00003210: 202b 2031 5d20 2b20 3429 290d 0a0d 0a20   + 1] + 4)).... 
-00003220: 2020 2064 6566 2064 7261 7728 7365 6c66     def draw(self
-00003230: 293a 0d0a 2020 2020 2020 2020 7370 6c61  ):..        spla
-00003240: 7368 4c6f 676f 203d 2049 6d61 6765 2e6f  shLogo = Image.o
-00003250: 7065 6e28 7365 6c66 2e70 6963 5f64 6972  pen(self.pic_dir
-00003260: 202b 2027 5549 5f43 4d4e 5f54 6162 5469   + 'UI_CMN_TabTi
-00003270: 746c 655f 4d61 696d 6169 5469 746c 655f  tle_MaimaiTitle_
-00003280: 5665 7232 3134 2e70 6e67 2729 2e63 6f6e  Ver214.png').con
-00003290: 7665 7274 2827 5247 4241 2729 0d0a 2020  vert('RGBA')..  
-000032a0: 2020 2020 2020 7370 6c61 7368 4c6f 676f        splashLogo
-000032b0: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
-000032c0: 6963 2873 706c 6173 684c 6f67 6f2c 2030  ic(splashLogo, 0
-000032d0: 2e36 3529 0d0a 2020 2020 2020 2020 7365  .65)..        se
-000032e0: 6c66 2e69 6d67 2e70 6173 7465 2873 706c  lf.img.paste(spl
-000032f0: 6173 684c 6f67 6f2c 2028 3130 2c20 3130  ashLogo, (10, 10
-00003300: 292c 206d 6173 6b3d 7370 6c61 7368 4c6f  ), mask=splashLo
-00003310: 676f 2e73 706c 6974 2829 5b33 5d29 0d0a  go.split()[3])..
-00003320: 0d0a 2020 2020 2020 2020 7261 7469 6e67  ..        rating
-00003330: 4261 7365 496d 6720 3d20 496d 6167 652e  BaseImg = Image.
-00003340: 6f70 656e 2873 656c 662e 7069 635f 6469  open(self.pic_di
-00003350: 7220 2b20 7365 6c66 2e5f 6669 6e64 5261  r + self._findRa
-00003360: 5069 6328 2929 2e63 6f6e 7665 7274 2827  Pic()).convert('
-00003370: 5247 4241 2729 0d0a 2020 2020 2020 2020  RGBA')..        
-00003380: 7261 7469 6e67 4261 7365 496d 6720 3d20  ratingBaseImg = 
-00003390: 7365 6c66 2e5f 6472 6177 5261 7469 6e67  self._drawRating
-000033a0: 2872 6174 696e 6742 6173 6549 6d67 290d  (ratingBaseImg).
-000033b0: 0a20 2020 2020 2020 2072 6174 696e 6742  .        ratingB
-000033c0: 6173 6549 6d67 203d 2073 656c 662e 5f72  aseImg = self._r
-000033d0: 6573 697a 6550 6963 2872 6174 696e 6742  esizePic(ratingB
-000033e0: 6173 6549 6d67 2c20 302e 3835 290d 0a20  aseImg, 0.85).. 
-000033f0: 2020 2020 2020 2073 656c 662e 696d 672e         self.img.
-00003400: 7061 7374 6528 7261 7469 6e67 4261 7365  paste(ratingBase
-00003410: 496d 672c 2028 3234 302c 2038 292c 206d  Img, (240, 8), m
-00003420: 6173 6b3d 7261 7469 6e67 4261 7365 496d  ask=ratingBaseIm
-00003430: 672e 7370 6c69 7428 295b 335d 290d 0a0d  g.split()[3])...
-00003440: 0a20 2020 2020 2020 206e 616d 6550 6c61  .        namePla
-00003450: 7465 496d 6720 3d20 496d 6167 652e 6f70  teImg = Image.op
-00003460: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
-00003470: 2b20 2755 495f 5453 545f 506c 6174 654d  + 'UI_TST_PlateM
-00003480: 6173 6b2e 706e 6727 292e 636f 6e76 6572  ask.png').conver
-00003490: 7428 2752 4742 4127 290d 0a20 2020 2020  t('RGBA')..     
-000034a0: 2020 206e 616d 6550 6c61 7465 496d 6720     namePlateImg 
-000034b0: 3d20 6e61 6d65 506c 6174 6549 6d67 2e72  = namePlateImg.r
-000034c0: 6573 697a 6528 2832 3835 2c20 3430 2929  esize((285, 40))
-000034d0: 0d0a 2020 2020 2020 2020 6e61 6d65 506c  ..        namePl
-000034e0: 6174 6544 7261 7720 3d20 496d 6167 6544  ateDraw = ImageD
-000034f0: 7261 772e 4472 6177 286e 616d 6550 6c61  raw.Draw(namePla
-00003500: 7465 496d 6729 0d0a 2020 2020 2020 2020  teImg)..        
-00003510: 666f 6e74 3120 3d20 496d 6167 6546 6f6e  font1 = ImageFon
-00003520: 742e 7472 7565 7479 7065 2853 5441 5449  t.truetype(STATI
-00003530: 4320 2b20 272f 6d73 7968 2e74 7463 272c  C + '/msyh.ttc',
-00003540: 2032 382c 2065 6e63 6f64 696e 673d 2775   28, encoding='u
-00003550: 6e69 6327 290d 0a20 2020 2020 2020 206e  nic')..        n
-00003560: 616d 6550 6c61 7465 4472 6177 2e74 6578  amePlateDraw.tex
-00003570: 7428 2831 322c 2034 292c 2027 2027 2e6a  t((12, 4), ' '.j
-00003580: 6f69 6e28 6c69 7374 2873 656c 662e 7573  oin(list(self.us
-00003590: 6572 4e61 6d65 2929 2c20 2762 6c61 636b  erName)), 'black
-000035a0: 272c 2066 6f6e 7431 290d 0a20 2020 2020  ', font1)..     
-000035b0: 2020 206e 616d 6544 7849 6d67 203d 2049     nameDxImg = I
-000035c0: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
-000035d0: 6963 5f64 6972 202b 2027 5549 5f43 4d4e  ic_dir + 'UI_CMN
-000035e0: 5f4e 616d 655f 4458 2e70 6e67 2729 2e63  _Name_DX.png').c
-000035f0: 6f6e 7665 7274 2827 5247 4241 2729 0d0a  onvert('RGBA')..
-00003600: 2020 2020 2020 2020 6e61 6d65 4478 496d          nameDxIm
-00003610: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
-00003620: 5069 6328 6e61 6d65 4478 496d 672c 2030  Pic(nameDxImg, 0
-00003630: 2e39 290d 0a20 2020 2020 2020 206e 616d  .9)..        nam
-00003640: 6550 6c61 7465 496d 672e 7061 7374 6528  ePlateImg.paste(
-00003650: 6e61 6d65 4478 496d 672c 2028 3233 302c  nameDxImg, (230,
-00003660: 2034 292c 206d 6173 6b3d 6e61 6d65 4478   4), mask=nameDx
-00003670: 496d 672e 7370 6c69 7428 295b 335d 290d  Img.split()[3]).
-00003680: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
-00003690: 672e 7061 7374 6528 6e61 6d65 506c 6174  g.paste(namePlat
-000036a0: 6549 6d67 2c20 2832 3430 2c20 3430 292c  eImg, (240, 40),
-000036b0: 206d 6173 6b3d 6e61 6d65 506c 6174 6549   mask=namePlateI
-000036c0: 6d67 2e73 706c 6974 2829 5b33 5d29 0d0a  mg.split()[3])..
-000036d0: 0d0a 2020 2020 2020 2020 7368 6f75 676f  ..        shougo
-000036e0: 7549 6d67 203d 2049 6d61 6765 2e6f 7065  uImg = Image.ope
-000036f0: 6e28 7365 6c66 2e70 6963 5f64 6972 202b  n(self.pic_dir +
-00003700: 2027 5549 5f43 4d4e 5f53 686f 7567 6f75   'UI_CMN_Shougou
-00003710: 5f52 6169 6e62 6f77 2e70 6e67 2729 2e63  _Rainbow.png').c
-00003720: 6f6e 7665 7274 2827 5247 4241 2729 0d0a  onvert('RGBA')..
-00003730: 2020 2020 2020 2020 7368 6f75 676f 7544          shougouD
-00003740: 7261 7720 3d20 496d 6167 6544 7261 772e  raw = ImageDraw.
-00003750: 4472 6177 2873 686f 7567 6f75 496d 6729  Draw(shougouImg)
-00003760: 0d0a 2020 2020 2020 2020 666f 6e74 3220  ..        font2 
-00003770: 3d20 496d 6167 6546 6f6e 742e 7472 7565  = ImageFont.true
-00003780: 7479 7065 2853 5441 5449 4320 2b20 272f  type(STATIC + '/
-00003790: 6164 6f62 655f 7369 6d68 6569 2e6f 7466  adobe_simhei.otf
-000037a0: 272c 2031 342c 2065 6e63 6f64 696e 673d  ', 14, encoding=
-000037b0: 2775 7466 2d38 2729 0d0a 2020 2020 2020  'utf-8')..      
-000037c0: 2020 706c 6179 436f 756e 7449 6e66 6f20    playCountInfo 
-000037d0: 3d20 6627 5344 3a20 7b73 656c 662e 7364  = f'SD: {self.sd
-000037e0: 5261 7469 6e67 7d20 2b20 4458 3a20 7b73  Rating} + DX: {s
-000037f0: 656c 662e 6478 5261 7469 6e67 7d20 3d20  elf.dxRating} = 
-00003800: 7b73 656c 662e 706c 6179 6572 5261 7469  {self.playerRati
-00003810: 6e67 7d27 0d0a 2020 2020 2020 2020 7368  ng}'..        sh
-00003820: 6f75 676f 7549 6d67 572c 2073 686f 7567  ougouImgW, shoug
-00003830: 6f75 496d 6748 203d 2073 686f 7567 6f75  ouImgH = shougou
-00003840: 496d 672e 7369 7a65 0d0a 2020 2020 2020  Img.size..      
-00003850: 2020 706c 6179 436f 756e 7449 6e66 6f57    playCountInfoW
-00003860: 2c20 706c 6179 436f 756e 7449 6e66 6f48  , playCountInfoH
-00003870: 203d 2073 686f 7567 6f75 4472 6177 2e74   = shougouDraw.t
-00003880: 6578 7473 697a 6528 706c 6179 436f 756e  extsize(playCoun
-00003890: 7449 6e66 6f2c 2066 6f6e 7432 290d 0a20  tInfo, font2).. 
-000038a0: 2020 2020 2020 2074 6578 7450 6f73 203d         textPos =
-000038b0: 2028 2873 686f 7567 6f75 496d 6757 202d   ((shougouImgW -
-000038c0: 2070 6c61 7943 6f75 6e74 496e 666f 5720   playCountInfoW 
-000038d0: 2d20 666f 6e74 322e 6765 746f 6666 7365  - font2.getoffse
-000038e0: 7428 706c 6179 436f 756e 7449 6e66 6f29  t(playCountInfo)
-000038f0: 5b30 5d29 202f 2032 2c20 3529 0d0a 2020  [0]) / 2, 5)..  
-00003900: 2020 2020 2020 7368 6f75 676f 7544 7261        shougouDra
-00003910: 772e 7465 7874 2828 7465 7874 506f 735b  w.text((textPos[
-00003920: 305d 202d 2031 2c20 7465 7874 506f 735b  0] - 1, textPos[
-00003930: 315d 292c 2070 6c61 7943 6f75 6e74 496e  1]), playCountIn
-00003940: 666f 2c20 2762 6c61 636b 272c 2066 6f6e  fo, 'black', fon
-00003950: 7432 290d 0a20 2020 2020 2020 2073 686f  t2)..        sho
-00003960: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
-00003970: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
-00003980: 6578 7450 6f73 5b31 5d29 2c20 706c 6179  extPos[1]), play
-00003990: 436f 756e 7449 6e66 6f2c 2027 626c 6163  CountInfo, 'blac
-000039a0: 6b27 2c20 666f 6e74 3229 0d0a 2020 2020  k', font2)..    
-000039b0: 2020 2020 7368 6f75 676f 7544 7261 772e      shougouDraw.
-000039c0: 7465 7874 2828 7465 7874 506f 735b 305d  text((textPos[0]
-000039d0: 2c20 7465 7874 506f 735b 315d 202d 2031  , textPos[1] - 1
-000039e0: 292c 2070 6c61 7943 6f75 6e74 496e 666f  ), playCountInfo
-000039f0: 2c20 2762 6c61 636b 272c 2066 6f6e 7432  , 'black', font2
-00003a00: 290d 0a20 2020 2020 2020 2073 686f 7567  )..        shoug
-00003a10: 6f75 4472 6177 2e74 6578 7428 2874 6578  ouDraw.text((tex
-00003a20: 7450 6f73 5b30 5d2c 2074 6578 7450 6f73  tPos[0], textPos
-00003a30: 5b31 5d20 2b20 3129 2c20 706c 6179 436f  [1] + 1), playCo
-00003a40: 756e 7449 6e66 6f2c 2027 626c 6163 6b27  untInfo, 'black'
-00003a50: 2c20 666f 6e74 3229 0d0a 2020 2020 2020  , font2)..      
-00003a60: 2020 7368 6f75 676f 7544 7261 772e 7465    shougouDraw.te
-00003a70: 7874 2828 7465 7874 506f 735b 305d 202d  xt((textPos[0] -
-00003a80: 2031 2c20 7465 7874 506f 735b 315d 202d   1, textPos[1] -
-00003a90: 2031 292c 2070 6c61 7943 6f75 6e74 496e   1), playCountIn
-00003aa0: 666f 2c20 2762 6c61 636b 272c 2066 6f6e  fo, 'black', fon
-00003ab0: 7432 290d 0a20 2020 2020 2020 2073 686f  t2)..        sho
-00003ac0: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
-00003ad0: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
-00003ae0: 6578 7450 6f73 5b31 5d20 2d20 3129 2c20  extPos[1] - 1), 
-00003af0: 706c 6179 436f 756e 7449 6e66 6f2c 2027  playCountInfo, '
-00003b00: 626c 6163 6b27 2c20 666f 6e74 3229 0d0a  black', font2)..
-00003b10: 2020 2020 2020 2020 7368 6f75 676f 7544          shougouD
-00003b20: 7261 772e 7465 7874 2828 7465 7874 506f  raw.text((textPo
-00003b30: 735b 305d 202d 2031 2c20 7465 7874 506f  s[0] - 1, textPo
-00003b40: 735b 315d 202b 2031 292c 2070 6c61 7943  s[1] + 1), playC
-00003b50: 6f75 6e74 496e 666f 2c20 2762 6c61 636b  ountInfo, 'black
-00003b60: 272c 2066 6f6e 7432 290d 0a20 2020 2020  ', font2)..     
-00003b70: 2020 2073 686f 7567 6f75 4472 6177 2e74     shougouDraw.t
-00003b80: 6578 7428 2874 6578 7450 6f73 5b30 5d20  ext((textPos[0] 
-00003b90: 2b20 312c 2074 6578 7450 6f73 5b31 5d20  + 1, textPos[1] 
-00003ba0: 2b20 3129 2c20 706c 6179 436f 756e 7449  + 1), playCountI
-00003bb0: 6e66 6f2c 2027 626c 6163 6b27 2c20 666f  nfo, 'black', fo
-00003bc0: 6e74 3229 0d0a 2020 2020 2020 2020 7368  nt2)..        sh
-00003bd0: 6f75 676f 7544 7261 772e 7465 7874 2874  ougouDraw.text(t
-00003be0: 6578 7450 6f73 2c20 706c 6179 436f 756e  extPos, playCoun
-00003bf0: 7449 6e66 6f2c 2027 7768 6974 6527 2c20  tInfo, 'white', 
-00003c00: 666f 6e74 3229 0d0a 2020 2020 2020 2020  font2)..        
-00003c10: 7368 6f75 676f 7549 6d67 203d 2073 656c  shougouImg = sel
-00003c20: 662e 5f72 6573 697a 6550 6963 2873 686f  f._resizePic(sho
-00003c30: 7567 6f75 496d 672c 2031 2e30 3529 0d0a  ugouImg, 1.05)..
-00003c40: 2020 2020 2020 2020 7365 6c66 2e69 6d67          self.img
-00003c50: 2e70 6173 7465 2873 686f 7567 6f75 496d  .paste(shougouIm
-00003c60: 672c 2028 3234 302c 2038 3329 2c20 6d61  g, (240, 83), ma
-00003c70: 736b 3d73 686f 7567 6f75 496d 672e 7370  sk=shougouImg.sp
-00003c80: 6c69 7428 295b 335d 290d 0a0d 0a20 2020  lit()[3])....   
-00003c90: 2020 2020 2073 656c 662e 5f64 7261 7742       self._drawB
-00003ca0: 6573 744c 6973 7428 7365 6c66 2e69 6d67  estList(self.img
-00003cb0: 2c20 7365 6c66 2e73 6442 6573 742c 2073  , self.sdBest, s
-00003cc0: 656c 662e 6478 4265 7374 290d 0a0d 0a20  elf.dxBest).... 
-00003cd0: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
-00003ce0: 7264 496d 6720 3d20 496d 6167 652e 6f70  rdImg = Image.op
-00003cf0: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
-00003d00: 2b20 2755 495f 434d 4e5f 4d69 6e69 4469  + 'UI_CMN_MiniDi
-00003d10: 616c 6f67 5f30 312e 706e 6727 292e 636f  alog_01.png').co
-00003d20: 6e76 6572 7428 2752 4742 4127 290d 0a20  nvert('RGBA').. 
-00003d30: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
-00003d40: 7264 496d 6720 3d20 7365 6c66 2e5f 7265  rdImg = self._re
-00003d50: 7369 7a65 5069 6328 6175 7468 6f72 426f  sizePic(authorBo
-00003d60: 6172 6449 6d67 2c20 302e 3335 290d 0a20  ardImg, 0.35).. 
-00003d70: 2020 2020 2020 2061 7574 686f 7242 6f61         authorBoa
-00003d80: 7264 4472 6177 203d 2049 6d61 6765 4472  rdDraw = ImageDr
-00003d90: 6177 2e44 7261 7728 6175 7468 6f72 426f  aw.Draw(authorBo
-00003da0: 6172 6449 6d67 290d 0a20 2020 2020 2020  ardImg)..       
-00003db0: 2061 7574 686f 7242 6f61 7264 4472 6177   authorBoardDraw
-00003dc0: 2e74 6578 7428 2833 312c 2032 3829 2c20  .text((31, 28), 
-00003dd0: 2720 2020 4765 6e65 7261 7465 6420 4279  '   Generated By
-00003de0: 5c6e 5879 6242 6f74 2026 2043 6869 7975  \nXybBot & Chiyu
-00003df0: 6b69 272c 2027 626c 6163 6b27 2c20 666f  ki', 'black', fo
-00003e00: 6e74 3229 0d0a 2020 2020 2020 2020 7365  nt2)..        se
-00003e10: 6c66 2e69 6d67 2e70 6173 7465 2861 7574  lf.img.paste(aut
-00003e20: 686f 7242 6f61 7264 496d 672c 2028 3132  horBoardImg, (12
-00003e30: 3234 2c20 3139 292c 206d 6173 6b3d 6175  24, 19), mask=au
-00003e40: 7468 6f72 426f 6172 6449 6d67 2e73 706c  thorBoardImg.spl
-00003e50: 6974 2829 5b33 5d29 0d0a 0d0a 2020 2020  it()[3])....    
-00003e60: 2020 2020 6478 496d 6720 3d20 496d 6167      dxImg = Imag
-00003e70: 652e 6f70 656e 2873 656c 662e 7069 635f  e.open(self.pic_
-00003e80: 6469 7220 2b20 2755 495f 5253 4c5f 4d42  dir + 'UI_RSL_MB
-00003e90: 6173 655f 5061 7274 735f 3031 2e70 6e67  ase_Parts_01.png
-00003ea0: 2729 2e63 6f6e 7665 7274 2827 5247 4241  ').convert('RGBA
-00003eb0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
-00003ec0: 2e69 6d67 2e70 6173 7465 2864 7849 6d67  .img.paste(dxImg
-00003ed0: 2c20 2839 3838 2c20 3635 292c 206d 6173  , (988, 65), mas
-00003ee0: 6b3d 6478 496d 672e 7370 6c69 7428 295b  k=dxImg.split()[
-00003ef0: 335d 290d 0a20 2020 2020 2020 2073 6449  3])..        sdI
-00003f00: 6d67 203d 2049 6d61 6765 2e6f 7065 6e28  mg = Image.open(
-00003f10: 7365 6c66 2e70 6963 5f64 6972 202b 2027  self.pic_dir + '
-00003f20: 5549 5f52 534c 5f4d 4261 7365 5f50 6172  UI_RSL_MBase_Par
-00003f30: 7473 5f30 322e 706e 6727 292e 636f 6e76  ts_02.png').conv
-00003f40: 6572 7428 2752 4742 4127 290d 0a20 2020  ert('RGBA')..   
-00003f50: 2020 2020 2073 656c 662e 696d 672e 7061       self.img.pa
-00003f60: 7374 6528 7364 496d 672c 2028 3836 352c  ste(sdImg, (865,
-00003f70: 2036 3529 2c20 6d61 736b 3d73 6449 6d67   65), mask=sdImg
-00003f80: 2e73 706c 6974 2829 5b33 5d29 0d0a 0d0a  .split()[3])....
-00003f90: 2020 2020 2020 2020 2320 7365 6c66 2e69          # self.i
-00003fa0: 6d67 2e73 686f 7728 290d 0a0d 0a20 2020  mg.show()....   
-00003fb0: 2064 6566 2067 6574 4469 7228 7365 6c66   def getDir(self
-00003fc0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00003fd0: 726e 2073 656c 662e 696d 670d 0a0d 0a0d  rn self.img.....
-00003fe0: 0a64 6566 2063 6f6d 7075 7465 5261 2864  .def computeRa(d
-00003ff0: 733a 2066 6c6f 6174 2c20 6163 6869 6576  s: float, achiev
-00004000: 656d 656e 743a 2066 6c6f 6174 2920 2d3e  ement: float) ->
-00004010: 2069 6e74 3a0d 0a20 2020 2062 6173 6552   int:..    baseR
-00004020: 6120 3d20 3232 2e34 200d 0a20 2020 2069  a = 22.4 ..    i
-00004030: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
-00004040: 3530 3a0d 0a20 2020 2020 2020 2062 6173  50:..        bas
-00004050: 6552 6120 3d20 372e 300d 0a20 2020 2065  eRa = 7.0..    e
-00004060: 6c69 6620 6163 6869 6576 656d 656e 7420  lif achievement 
-00004070: 3c20 3630 3a0d 0a20 2020 2020 2020 2062  < 60:..        b
-00004080: 6173 6552 6120 3d20 382e 3020 0d0a 2020  aseRa = 8.0 ..  
-00004090: 2020 656c 6966 2061 6368 6965 7665 6d65    elif achieveme
-000040a0: 6e74 203c 2037 303a 0d0a 2020 2020 2020  nt < 70:..      
-000040b0: 2020 6261 7365 5261 203d 2039 2e36 200d    baseRa = 9.6 .
-000040c0: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
-000040d0: 656d 656e 7420 3c20 3735 3a0d 0a20 2020  ement < 75:..   
-000040e0: 2020 2020 2062 6173 6552 6120 3d20 3131       baseRa = 11
-000040f0: 2e32 200d 0a20 2020 2065 6c69 6620 6163  .2 ..    elif ac
-00004100: 6869 6576 656d 656e 7420 3c20 3830 3a0d  hievement < 80:.
-00004110: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
-00004120: 3d20 3132 2e30 200d 0a20 2020 2065 6c69  = 12.0 ..    eli
-00004130: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
-00004140: 3930 3a0d 0a20 2020 2020 2020 2062 6173  90:..        bas
-00004150: 6552 6120 3d20 3133 2e36 200d 0a20 2020  eRa = 13.6 ..   
-00004160: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
-00004170: 7420 3c20 3934 3a0d 0a20 2020 2020 2020  t < 94:..       
-00004180: 2062 6173 6552 6120 3d20 3135 2e32 200d   baseRa = 15.2 .
-00004190: 0a20 2020 2065 6c69 6620 6163 6869 6576  .    elif achiev
-000041a0: 656d 656e 7420 3c20 3937 3a0d 0a20 2020  ement < 97:..   
-000041b0: 2020 2020 2062 6173 6552 6120 3d20 3136       baseRa = 16
-000041c0: 2e38 200d 0a20 2020 2065 6c69 6620 6163  .8 ..    elif ac
-000041d0: 6869 6576 656d 656e 7420 3c20 3938 3a0d  hievement < 98:.
-000041e0: 0a20 2020 2020 2020 2062 6173 6552 6120  .        baseRa 
-000041f0: 3d20 3230 2e30 200d 0a20 2020 2065 6c69  = 20.0 ..    eli
-00004200: 6620 6163 6869 6576 656d 656e 7420 3c20  f achievement < 
-00004210: 3939 3a0d 0a20 2020 2020 2020 2062 6173  99:..        bas
-00004220: 6552 6120 3d20 3230 2e33 0d0a 2020 2020  eRa = 20.3..    
-00004230: 656c 6966 2061 6368 6965 7665 6d65 6e74  elif achievement
-00004240: 203c 2039 392e 353a 0d0a 2020 2020 2020   < 99.5:..      
-00004250: 2020 6261 7365 5261 203d 2032 302e 3820    baseRa = 20.8 
-00004260: 0d0a 2020 2020 656c 6966 2061 6368 6965  ..    elif achie
-00004270: 7665 6d65 6e74 203c 2031 3030 3a0d 0a20  vement < 100:.. 
-00004280: 2020 2020 2020 2062 6173 6552 6120 3d20         baseRa = 
-00004290: 3231 2e31 200d 0a20 2020 2065 6c69 6620  21.1 ..    elif 
-000042a0: 6163 6869 6576 656d 656e 7420 3c20 3130  achievement < 10
-000042b0: 302e 353a 0d0a 2020 2020 2020 2020 6261  0.5:..        ba
-000042c0: 7365 5261 203d 2032 312e 3620 0d0a 0d0a  seRa = 21.6 ....
-000042d0: 2020 2020 7265 7475 726e 206d 6174 682e      return math.
-000042e0: 666c 6f6f 7228 6473 202a 2028 6d69 6e28  floor(ds * (min(
-000042f0: 3130 302e 352c 2061 6368 6965 7665 6d65  100.5, achieveme
-00004300: 6e74 2920 2f20 3130 3029 202a 2062 6173  nt) / 100) * bas
-00004310: 6552 6129 0d0a 0d0a 0d0a 6173 796e 6320  eRa)......async 
-00004320: 6465 6620 6765 6e65 7261 7465 3530 2870  def generate50(p
-00004330: 6179 6c6f 6164 3a20 4469 6374 2920 2d3e  ayload: Dict) ->
-00004340: 2054 7570 6c65 5b4f 7074 696f 6e61 6c5b   Tuple[Optional[
-00004350: 496d 6167 652e 496d 6167 655d 2c20 626f  Image.Image], bo
-00004360: 6f6c 5d3a 0d0a 2020 2020 6173 796e 6320  ol]:..    async 
-00004370: 7769 7468 2061 696f 6874 7470 2e72 6571  with aiohttp.req
-00004380: 7565 7374 2822 504f 5354 222c 2022 6874  uest("POST", "ht
-00004390: 7470 733a 2f2f 7777 772e 6469 7669 6e67  tps://www.diving
-000043a0: 2d66 6973 682e 636f 6d2f 6170 692f 6d61  -fish.com/api/ma
-000043b0: 696d 6169 6478 7072 6f62 6572 2f71 7565  imaidxprober/que
-000043c0: 7279 2f70 6c61 7965 7222 2c20 6a73 6f6e  ry/player", json
-000043d0: 3d70 6179 6c6f 6164 2920 6173 2072 6573  =payload) as res
-000043e0: 703a 0d0a 2020 2020 2020 2020 6966 2072  p:..        if r
-000043f0: 6573 702e 7374 6174 7573 203d 3d20 3430  esp.status == 40
-00004400: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00004410: 7265 7475 726e 204e 6f6e 652c 2034 3030  return None, 400
-00004420: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
-00004430: 702e 7374 6174 7573 203d 3d20 3430 333a  p.status == 403:
-00004440: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00004450: 7475 726e 204e 6f6e 652c 2034 3033 0d0a  turn None, 403..
-00004460: 2020 2020 2020 2020 7364 5f62 6573 7420          sd_best 
-00004470: 3d20 4265 7374 4c69 7374 2833 3529 0d0a  = BestList(35)..
-00004480: 2020 2020 2020 2020 6478 5f62 6573 7420          dx_best 
-00004490: 3d20 4265 7374 4c69 7374 2831 3529 0d0a  = BestList(15)..
-000044a0: 2020 2020 2020 2020 6f62 6a20 3d20 6177          obj = aw
-000044b0: 6169 7420 7265 7370 2e6a 736f 6e28 290d  ait resp.json().
-000044c0: 0a20 2020 2020 2020 2064 783a 204c 6973  .        dx: Lis
-000044d0: 745b 4469 6374 5d20 3d20 6f62 6a5b 2263  t[Dict] = obj["c
-000044e0: 6861 7274 7322 5d5b 2264 7822 5d0d 0a20  harts"]["dx"].. 
-000044f0: 2020 2020 2020 2073 643a 204c 6973 745b         sd: List[
-00004500: 4469 6374 5d20 3d20 6f62 6a5b 2263 6861  Dict] = obj["cha
-00004510: 7274 7322 5d5b 2273 6422 5d0d 0a20 2020  rts"]["sd"]..   
-00004520: 2020 2020 2066 6f72 2063 2069 6e20 7364       for c in sd
-00004530: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00004540: 645f 6265 7374 2e70 7573 6828 4368 6172  d_best.push(Char
-00004550: 7449 6e66 6f2e 6672 6f6d 5f6a 736f 6e28  tInfo.from_json(
-00004560: 6329 290d 0a20 2020 2020 2020 2066 6f72  c))..        for
-00004570: 2063 2069 6e20 6478 3a0d 0a20 2020 2020   c in dx:..     
-00004580: 2020 2020 2020 2064 785f 6265 7374 2e70         dx_best.p
-00004590: 7573 6828 4368 6172 7449 6e66 6f2e 6672  ush(ChartInfo.fr
-000045a0: 6f6d 5f6a 736f 6e28 6329 290d 0a20 2020  om_json(c))..   
-000045b0: 2020 2020 2070 6963 203d 2044 7261 7742       pic = DrawB
-000045c0: 6573 7428 7364 5f62 6573 742c 2064 785f  est(sd_best, dx_
-000045d0: 6265 7374 2c20 6f62 6a5b 226e 6963 6b6e  best, obj["nickn
-000045e0: 616d 6522 5d29 2e67 6574 4469 7228 290d  ame"]).getDir().
-000045f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004600: 7069 632c 2030 0d0a                      pic, 0..
+00000000: 2320 4175 7468 6f72 3a20 7879 622c 2044  # Author: xyb, D
+00000010: 6976 696e 675f 4669 7368 0a0a 696d 706f  iving_Fish..impo
+00000020: 7274 206f 730a 696d 706f 7274 206d 6174  rt os.import mat
+00000030: 680a 6672 6f6d 2074 7970 696e 6720 696d  h.from typing im
+00000040: 706f 7274 204f 7074 696f 6e61 6c2c 2044  port Optional, D
+00000050: 6963 742c 204c 6973 742c 5475 706c 650a  ict, List,Tuple.
+00000060: 6672 6f6d 202e 746f 6f6c 2069 6d70 6f72  from .tool impor
+00000070: 7420 5354 4154 4943 0a69 6d70 6f72 7420  t STATIC.import 
+00000080: 6169 6f68 7474 700a 6672 6f6d 2050 494c  aiohttp.from PIL
+00000090: 2069 6d70 6f72 7420 496d 6167 652c 2049   import Image, I
+000000a0: 6d61 6765 4472 6177 2c20 496d 6167 6546  mageDraw, ImageF
+000000b0: 6f6e 742c 2049 6d61 6765 4669 6c74 6572  ont, ImageFilter
+000000c0: 0a66 726f 6d20 2e6d 6169 6d61 6964 785f  .from .maimaidx_
+000000d0: 6d75 7369 6320 696d 706f 7274 2067 6574  music import get
+000000e0: 5f63 6f76 6572 5f6c 656e 355f 6964 2c20  _cover_len5_id, 
+000000f0: 746f 7461 6c5f 6c69 7374 0a0a 0a73 636f  total_list...sco
+00000100: 7265 5261 6e6b 203d 2027 4420 4320 4220  reRank = 'D C B 
+00000110: 4242 2042 4242 2041 2041 4120 4141 4120  BB BBB A AA AAA 
+00000120: 5320 532b 2053 5320 5353 2b20 5353 5320  S S+ SS SS+ SSS 
+00000130: 5353 532b 272e 7370 6c69 7428 2720 2729  SSS+'.split(' ')
+00000140: 0a63 6f6d 626f 203d 2027 2046 4320 4643  .combo = ' FC FC
+00000150: 2b20 4150 2041 502b 272e 7370 6c69 7428  + AP AP+'.split(
+00000160: 2720 2729 0a64 6966 6673 203d 2027 4261  ' ').diffs = 'Ba
+00000170: 7369 6320 4164 7661 6e63 6564 2045 7870  sic Advanced Exp
+00000180: 6572 7420 4d61 7374 6572 2052 653a 4d61  ert Master Re:Ma
+00000190: 7374 6572 272e 7370 6c69 7428 2720 2729  ster'.split(' ')
+000001a0: 0a0a 0a63 6c61 7373 2043 6861 7274 496e  ...class ChartIn
+000001b0: 666f 286f 626a 6563 7429 3a0a 2020 2020  fo(object):.    
+000001c0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000001d0: 662c 2069 644e 756d 3a73 7472 2c20 6469  f, idNum:str, di
+000001e0: 6666 3a69 6e74 2c20 7470 3a73 7472 2c20  ff:int, tp:str, 
+000001f0: 6163 6869 6576 656d 656e 743a 666c 6f61  achievement:floa
+00000200: 742c 2072 613a 696e 742c 2063 6f6d 626f  t, ra:int, combo
+00000210: 4964 3a69 6e74 2c20 7363 6f72 6549 643a  Id:int, scoreId:
+00000220: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
+00000230: 2020 2020 2020 7469 746c 653a 7374 722c        title:str,
+00000240: 2064 733a 666c 6f61 742c 206c 763a 7374   ds:float, lv:st
+00000250: 7229 3a0a 2020 2020 2020 2020 7365 6c66  r):.        self
+00000260: 2e69 644e 756d 203d 2069 644e 756d 0a20  .idNum = idNum. 
+00000270: 2020 2020 2020 2073 656c 662e 6469 6666         self.diff
+00000280: 203d 2064 6966 660a 2020 2020 2020 2020   = diff.        
+00000290: 7365 6c66 2e74 7020 3d20 7470 0a20 2020  self.tp = tp.   
+000002a0: 2020 2020 2073 656c 662e 6163 6869 6576       self.achiev
+000002b0: 656d 656e 7420 3d20 6163 6869 6576 656d  ement = achievem
+000002c0: 656e 740a 2020 2020 2020 2020 7365 6c66  ent.        self
+000002d0: 2e72 6120 3d20 7261 0a20 2020 2020 2020  .ra = ra.       
+000002e0: 2073 656c 662e 636f 6d62 6f49 6420 3d20   self.comboId = 
+000002f0: 636f 6d62 6f49 640a 2020 2020 2020 2020  comboId.        
+00000300: 7365 6c66 2e73 636f 7265 4964 203d 2073  self.scoreId = s
+00000310: 636f 7265 4964 0a20 2020 2020 2020 2073  coreId.        s
+00000320: 656c 662e 7469 746c 6520 3d20 7469 746c  elf.title = titl
+00000330: 650a 2020 2020 2020 2020 7365 6c66 2e64  e.        self.d
+00000340: 7320 3d20 6473 0a20 2020 2020 2020 2073  s = ds.        s
+00000350: 656c 662e 6c76 203d 206c 760a 0a20 2020  elf.lv = lv..   
+00000360: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
+00000370: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00000380: 726e 2027 252d 3530 7327 2025 2066 277b  rn '%-50s' % f'{
+00000390: 7365 6c66 2e74 6974 6c65 7d20 5b7b 7365  self.title} [{se
+000003a0: 6c66 2e74 707d 5d27 202b 2066 277b 7365  lf.tp}]' + f'{se
+000003b0: 6c66 2e64 737d 5c74 7b64 6966 6673 5b73  lf.ds}\t{diffs[s
+000003c0: 656c 662e 6469 6666 5d7d 5c74 7b73 656c  elf.diff]}\t{sel
+000003d0: 662e 7261 7d27 0a0a 2020 2020 6465 6620  f.ra}'..    def 
+000003e0: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
+000003f0: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
+00000400: 7572 6e20 7365 6c66 2e72 6120 3d3d 206f  urn self.ra == o
+00000410: 7468 6572 2e72 610a 0a20 2020 2064 6566  ther.ra..    def
+00000420: 205f 5f6c 745f 5f28 7365 6c66 2c20 6f74   __lt__(self, ot
+00000430: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
+00000440: 7475 726e 2073 656c 662e 7261 203c 206f  turn self.ra < o
+00000450: 7468 6572 2e72 610a 0a20 2020 2040 636c  ther.ra..    @cl
+00000460: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00000470: 6620 6672 6f6d 5f6a 736f 6e28 636c 732c  f from_json(cls,
+00000480: 2064 6174 6129 3a0a 2020 2020 2020 2020   data):.        
+00000490: 7261 7465 203d 205b 2764 272c 2027 6327  rate = ['d', 'c'
+000004a0: 2c20 2762 272c 2027 6262 272c 2027 6262  , 'b', 'bb', 'bb
+000004b0: 6227 2c20 2761 272c 2027 6161 272c 2027  b', 'a', 'aa', '
+000004c0: 6161 6127 2c20 2773 272c 2027 7370 272c  aaa', 's', 'sp',
+000004d0: 2027 7373 272c 2027 7373 7027 2c20 2773   'ss', 'ssp', 's
+000004e0: 7373 272c 2027 7373 7370 275d 0a20 2020  ss', 'sssp'].   
+000004f0: 2020 2020 2072 6920 3d20 7261 7465 2e69       ri = rate.i
+00000500: 6e64 6578 2864 6174 615b 2272 6174 6522  ndex(data["rate"
+00000510: 5d29 0a20 2020 2020 2020 2066 6320 3d20  ]).        fc = 
+00000520: 5b27 272c 2027 6663 272c 2027 6663 7027  ['', 'fc', 'fcp'
+00000530: 2c20 2761 7027 2c20 2761 7070 275d 0a20  , 'ap', 'app']. 
+00000540: 2020 2020 2020 2066 6920 3d20 6663 2e69         fi = fc.i
+00000550: 6e64 6578 2864 6174 615b 2266 6322 5d29  ndex(data["fc"])
+00000560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000570: 636c 7328 0a20 2020 2020 2020 2020 2020  cls(.           
+00000580: 2069 644e 756d 3d74 6f74 616c 5f6c 6973   idNum=total_lis
+00000590: 742e 6279 5f74 6974 6c65 2864 6174 615b  t.by_title(data[
+000005a0: 2274 6974 6c65 225d 292e 6964 2c0a 2020  "title"]).id,.  
+000005b0: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+000005c0: 6461 7461 5b22 7469 746c 6522 5d2c 0a20  data["title"],. 
+000005d0: 2020 2020 2020 2020 2020 2064 6966 663d             diff=
+000005e0: 6461 7461 5b22 6c65 7665 6c5f 696e 6465  data["level_inde
+000005f0: 7822 5d2c 0a20 2020 2020 2020 2020 2020  x"],.           
+00000600: 2072 613d 6461 7461 5b22 7261 225d 2c0a   ra=data["ra"],.
+00000610: 2020 2020 2020 2020 2020 2020 6473 3d64              ds=d
+00000620: 6174 615b 2264 7322 5d2c 0a20 2020 2020  ata["ds"],.     
+00000630: 2020 2020 2020 2063 6f6d 626f 4964 3d66         comboId=f
+00000640: 692c 0a20 2020 2020 2020 2020 2020 2073  i,.            s
+00000650: 636f 7265 4964 3d72 692c 0a20 2020 2020  coreId=ri,.     
+00000660: 2020 2020 2020 206c 763d 6461 7461 5b22         lv=data["
+00000670: 6c65 7665 6c22 5d2c 0a20 2020 2020 2020  level"],.       
+00000680: 2020 2020 2061 6368 6965 7665 6d65 6e74       achievement
+00000690: 3d64 6174 615b 2261 6368 6965 7665 6d65  =data["achieveme
+000006a0: 6e74 7322 5d2c 0a20 2020 2020 2020 2020  nts"],.         
+000006b0: 2020 2074 703d 6461 7461 5b22 7479 7065     tp=data["type
+000006c0: 225d 0a20 2020 2020 2020 2029 0a0a 0a0a  "].        )....
+000006d0: 636c 6173 7320 4265 7374 4c69 7374 286f  class BestList(o
+000006e0: 626a 6563 7429 3a0a 0a20 2020 2064 6566  bject):..    def
+000006f0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00000700: 7369 7a65 3a69 6e74 293a 0a20 2020 2020  size:int):.     
+00000710: 2020 2073 656c 662e 6461 7461 203d 205b     self.data = [
+00000720: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+00000730: 697a 6520 3d20 7369 7a65 0a0a 2020 2020  ize = size..    
+00000740: 6465 6620 7075 7368 2873 656c 662c 2065  def push(self, e
+00000750: 6c65 6d3a 4368 6172 7449 6e66 6f29 3a0a  lem:ChartInfo):.
+00000760: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+00000770: 656c 662e 6461 7461 2920 3e3d 2073 656c  elf.data) >= sel
+00000780: 662e 7369 7a65 2061 6e64 2065 6c65 6d20  f.size and elem 
+00000790: 3c20 7365 6c66 2e64 6174 615b 2d31 5d3a  < self.data[-1]:
+000007a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000007b0: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
+000007c0: 2e64 6174 612e 6170 7065 6e64 2865 6c65  .data.append(ele
+000007d0: 6d29 0a20 2020 2020 2020 2073 656c 662e  m).        self.
+000007e0: 6461 7461 2e73 6f72 7428 290a 2020 2020  data.sort().    
+000007f0: 2020 2020 7365 6c66 2e64 6174 612e 7265      self.data.re
+00000800: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
+00000810: 7768 696c 6528 6c65 6e28 7365 6c66 2e64  while(len(self.d
+00000820: 6174 6129 203e 2073 656c 662e 7369 7a65  ata) > self.size
+00000830: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00000840: 656c 2073 656c 662e 6461 7461 5b2d 315d  el self.data[-1]
+00000850: 0a0a 2020 2020 6465 6620 706f 7028 7365  ..    def pop(se
+00000860: 6c66 293a 0a20 2020 2020 2020 2064 656c  lf):.        del
+00000870: 2073 656c 662e 6461 7461 5b2d 315d 0a0a   self.data[-1]..
+00000880: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
+00000890: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+000008a0: 6574 7572 6e20 275b 5c6e 5c74 2720 2b20  eturn '[\n\t' + 
+000008b0: 272c 205c 6e5c 7427 2e6a 6f69 6e28 5b73  ', \n\t'.join([s
+000008c0: 7472 2863 6929 2066 6f72 2063 6920 696e  tr(ci) for ci in
+000008d0: 2073 656c 662e 6461 7461 5d29 202b 2027   self.data]) + '
+000008e0: 5c6e 5d27 0a0a 2020 2020 6465 6620 5f5f  \n]'..    def __
+000008f0: 6c65 6e5f 5f28 7365 6c66 293a 0a20 2020  len__(self):.   
+00000900: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
+00000910: 7365 6c66 2e64 6174 6129 0a0a 2020 2020  self.data)..    
+00000920: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
+00000930: 7365 6c66 2c20 696e 6465 7829 3a0a 2020  self, index):.  
+00000940: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000950: 662e 6461 7461 5b69 6e64 6578 5d0a 0a0a  f.data[index]...
+00000960: 636c 6173 7320 4472 6177 4265 7374 286f  class DrawBest(o
+00000970: 626a 6563 7429 3a0a 0a20 2020 2064 6566  bject):..    def
+00000980: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00000990: 7364 4265 7374 3a42 6573 744c 6973 742c  sdBest:BestList,
+000009a0: 2064 7842 6573 743a 4265 7374 4c69 7374   dxBest:BestList
+000009b0: 2c20 7573 6572 4e61 6d65 3a73 7472 2c20  , userName:str, 
+000009c0: 706c 6179 6572 5261 7469 6e67 3a69 6e74  playerRating:int
+000009d0: 2c20 6d75 7369 6352 6174 696e 673a 696e  , musicRating:in
+000009e0: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
+000009f0: 2e73 6442 6573 7420 3d20 7364 4265 7374  .sdBest = sdBest
+00000a00: 0a20 2020 2020 2020 2073 656c 662e 6478  .        self.dx
+00000a10: 4265 7374 203d 2064 7842 6573 740a 2020  Best = dxBest.  
+00000a20: 2020 2020 2020 7365 6c66 2e75 7365 724e        self.userN
+00000a30: 616d 6520 3d20 7365 6c66 2e5f 7374 7269  ame = self._stri
+00000a40: 6e67 5132 4228 7573 6572 4e61 6d65 290a  ngQ2B(userName).
+00000a50: 2020 2020 2020 2020 7365 6c66 2e70 6c61          self.pla
+00000a60: 7965 7252 6174 696e 6720 3d20 706c 6179  yerRating = play
+00000a70: 6572 5261 7469 6e67 0a20 2020 2020 2020  erRating.       
+00000a80: 2073 656c 662e 6d75 7369 6352 6174 696e   self.musicRatin
+00000a90: 6720 3d20 6d75 7369 6352 6174 696e 670a  g = musicRating.
+00000aa0: 2020 2020 2020 2020 7365 6c66 2e72 616e          self.ran
+00000ab0: 6b52 6174 696e 6720 3d20 7365 6c66 2e70  kRating = self.p
+00000ac0: 6c61 7965 7252 6174 696e 6720 2d20 7365  layerRating - se
+00000ad0: 6c66 2e6d 7573 6963 5261 7469 6e67 0a20  lf.musicRating. 
+00000ae0: 2020 2020 2020 2073 656c 662e 7069 635f         self.pic_
+00000af0: 6469 7220 3d20 5354 4154 4943 202b 2027  dir = STATIC + '
+00000b00: 2f6d 6169 2f70 6963 2f27 0a20 2020 2020  /mai/pic/'.     
+00000b10: 2020 2073 656c 662e 636f 7665 725f 6469     self.cover_di
+00000b20: 7220 3d20 5354 4154 4943 202b 2027 2f6d  r = STATIC + '/m
+00000b30: 6169 2f63 6f76 6572 2f27 0a20 2020 2020  ai/cover/'.     
+00000b40: 2020 2073 656c 662e 696d 6720 3d20 496d     self.img = Im
+00000b50: 6167 652e 6f70 656e 2873 656c 662e 7069  age.open(self.pi
+00000b60: 635f 6469 7220 2b20 2755 495f 5454 525f  c_dir + 'UI_TTR_
+00000b70: 4247 5f42 6173 655f 506c 7573 2e70 6e67  BG_Base_Plus.png
+00000b80: 2729 2e63 6f6e 7665 7274 2827 5247 4241  ').convert('RGBA
+00000b90: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00000ba0: 524f 5753 5f49 4d47 203d 205b 325d 0a20  ROWS_IMG = [2]. 
+00000bb0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00000bc0: 7261 6e67 6528 3629 3a0a 2020 2020 2020  range(6):.      
+00000bd0: 2020 2020 2020 7365 6c66 2e52 4f57 535f        self.ROWS_
+00000be0: 494d 472e 6170 7065 6e64 2831 3136 202b  IMG.append(116 +
+00000bf0: 2039 3620 2a20 6929 0a20 2020 2020 2020   96 * i).       
+00000c00: 2073 656c 662e 434f 4c4f 554d 535f 494d   self.COLOUMS_IM
+00000c10: 4720 3d20 5b5d 0a20 2020 2020 2020 2066  G = [].        f
+00000c20: 6f72 2069 2069 6e20 7261 6e67 6528 3629  or i in range(6)
+00000c30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00000c40: 6c66 2e43 4f4c 4f55 4d53 5f49 4d47 2e61  lf.COLOUMS_IMG.a
+00000c50: 7070 656e 6428 3220 2b20 3137 3220 2a20  ppend(2 + 172 * 
+00000c60: 6929 0a20 2020 2020 2020 2066 6f72 2069  i).        for i
+00000c70: 2069 6e20 7261 6e67 6528 3429 3a0a 2020   in range(4):.  
+00000c80: 2020 2020 2020 2020 2020 7365 6c66 2e43            self.C
+00000c90: 4f4c 4f55 4d53 5f49 4d47 2e61 7070 656e  OLOUMS_IMG.appen
+00000ca0: 6428 3838 3820 2b20 3137 3220 2a20 6929  d(888 + 172 * i)
+00000cb0: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+00000cc0: 6177 2829 0a0a 2020 2020 6465 6620 5f51  aw()..    def _Q
+00000cd0: 3242 2873 656c 662c 2075 6368 6172 293a  2B(self, uchar):
+00000ce0: 0a20 2020 2020 2020 2022 2222 e58d 95e4  .        """....
+00000cf0: b8aa e5ad 97e7 aca6 20e5 85a8 e8a7 92e8  ........ .......
+00000d00: bdac e58d 8ae8 a792 2222 220a 2020 2020  ........""".    
+00000d10: 2020 2020 696e 7369 6465 5f63 6f64 6520      inside_code 
+00000d20: 3d20 6f72 6428 7563 6861 7229 0a20 2020  = ord(uchar).   
+00000d30: 2020 2020 2069 6620 696e 7369 6465 5f63       if inside_c
+00000d40: 6f64 6520 3d3d 2030 7833 3030 303a 0a20  ode == 0x3000:. 
+00000d50: 2020 2020 2020 2020 2020 2069 6e73 6964             insid
+00000d60: 655f 636f 6465 203d 2030 7830 3032 300a  e_code = 0x0020.
+00000d70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000d80: 2020 2020 2020 2020 2020 696e 7369 6465            inside
+00000d90: 5f63 6f64 6520 2d3d 2030 7866 6565 300a  _code -= 0xfee0.
+00000da0: 2020 2020 2020 2020 6966 2069 6e73 6964          if insid
+00000db0: 655f 636f 6465 203c 2030 7830 3032 3020  e_code < 0x0020 
+00000dc0: 6f72 2069 6e73 6964 655f 636f 6465 203e  or inside_code >
+00000dd0: 2030 7837 653a 2023 e8bd ace5 ae8c e4b9   0x7e: #........
+00000de0: 8be5 908e e4b8 8de6 98af e58d 8ae8 a792  ................
+00000df0: e5ad 97e7 aca6 e8bf 94e5 9b9e e58e 9fe6  ................
+00000e00: 9da5 e79a 84e5 ad97 e7ac a60a 2020 2020  ............    
+00000e10: 2020 2020 2020 2020 7265 7475 726e 2075          return u
+00000e20: 6368 6172 0a20 2020 2020 2020 2072 6574  char.        ret
+00000e30: 7572 6e20 6368 7228 696e 7369 6465 5f63  urn chr(inside_c
+00000e40: 6f64 6529 0a0a 2020 2020 6465 6620 5f73  ode)..    def _s
+00000e50: 7472 696e 6751 3242 2873 656c 662c 2075  tringQ2B(self, u
+00000e60: 7374 7269 6e67 293a 0a20 2020 2020 2020  string):.       
+00000e70: 2022 2222 e68a 8ae5 ad97 e7ac a6e4 b8b2   """............
+00000e80: e585 a8e8 a792 e8bd ace5 8d8a e8a7 9222  ..............."
+00000e90: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00000ea0: 6e20 2222 2e6a 6f69 6e28 5b73 656c 662e  n "".join([self.
+00000eb0: 5f51 3242 2875 6368 6172 2920 666f 7220  _Q2B(uchar) for 
+00000ec0: 7563 6861 7220 696e 2075 7374 7269 6e67  uchar in ustring
+00000ed0: 5d29 0a0a 2020 2020 6465 6620 5f67 6574  ])..    def _get
+00000ee0: 4368 6172 5769 6474 6828 7365 6c66 2c20  CharWidth(self, 
+00000ef0: 6f29 202d 3e20 696e 743a 0a20 2020 2020  o) -> int:.     
+00000f00: 2020 2077 6964 7468 7320 3d20 5b0a 2020     widths = [.  
+00000f10: 2020 2020 2020 2020 2020 2831 3236 2c20            (126, 
+00000f20: 3129 2c20 2831 3539 2c20 3029 2c20 2836  1), (159, 0), (6
+00000f30: 3837 2c20 3129 2c20 2837 3130 2c20 3029  87, 1), (710, 0)
+00000f40: 2c20 2837 3131 2c20 3129 2c20 2837 3237  , (711, 1), (727
+00000f50: 2c20 3029 2c20 2837 3333 2c20 3129 2c20  , 0), (733, 1), 
+00000f60: 2838 3739 2c20 3029 2c20 2831 3135 342c  (879, 0), (1154,
+00000f70: 2031 292c 2028 3131 3631 2c20 3029 2c0a   1), (1161, 0),.
+00000f80: 2020 2020 2020 2020 2020 2020 2834 3334              (434
+00000f90: 372c 2031 292c 2028 3434 3437 2c20 3229  7, 1), (4447, 2)
+00000fa0: 2c20 2837 3436 372c 2031 292c 2028 3735  , (7467, 1), (75
+00000fb0: 3231 2c20 3029 2c20 2838 3336 392c 2031  21, 0), (8369, 1
+00000fc0: 292c 2028 3834 3236 2c20 3029 2c20 2839  ), (8426, 0), (9
+00000fd0: 3030 302c 2031 292c 2028 3930 3032 2c20  000, 1), (9002, 
+00000fe0: 3229 2c20 2831 3130 3231 2c20 3129 2c0a  2), (11021, 1),.
+00000ff0: 2020 2020 2020 2020 2020 2020 2831 3233              (123
+00001000: 3530 2c20 3229 2c20 2831 3233 3531 2c20  50, 2), (12351, 
+00001010: 3129 2c20 2831 3234 3338 2c20 3229 2c20  1), (12438, 2), 
+00001020: 2831 3234 3432 2c20 3029 2c20 2831 3938  (12442, 0), (198
+00001030: 3933 2c20 3229 2c20 2831 3939 3637 2c20  93, 2), (19967, 
+00001040: 3129 2c20 2835 3532 3033 2c20 3229 2c20  1), (55203, 2), 
+00001050: 2836 3337 3433 2c20 3129 2c0a 2020 2020  (63743, 1),.    
+00001060: 2020 2020 2020 2020 2836 3431 3036 2c20          (64106, 
+00001070: 3229 2c20 2836 3530 3339 2c20 3129 2c20  2), (65039, 1), 
+00001080: 2836 3530 3539 2c20 3029 2c20 2836 3531  (65059, 0), (651
+00001090: 3331 2c20 3229 2c20 2836 3532 3739 2c20  31, 2), (65279, 
+000010a0: 3129 2c20 2836 3533 3736 2c20 3229 2c20  1), (65376, 2), 
+000010b0: 2836 3535 3030 2c20 3129 2c20 2836 3535  (65500, 1), (655
+000010c0: 3130 2c20 3229 2c0a 2020 2020 2020 2020  10, 2),.        
+000010d0: 2020 2020 2831 3230 3833 312c 2031 292c      (120831, 1),
+000010e0: 2028 3236 3231 3431 2c20 3229 2c20 2831   (262141, 2), (1
+000010f0: 3131 3431 3039 2c20 3129 2c0a 2020 2020  114109, 1),.    
+00001100: 2020 2020 5d0a 2020 2020 2020 2020 6966      ].        if
+00001110: 206f 203d 3d20 3078 6520 6f72 206f 203d   o == 0xe or o =
+00001120: 3d20 3078 663a 0a20 2020 2020 2020 2020  = 0xf:.         
+00001130: 2020 2072 6574 7572 6e20 300a 2020 2020     return 0.    
+00001140: 2020 2020 666f 7220 6e75 6d2c 2077 6964      for num, wid
+00001150: 2069 6e20 7769 6474 6873 3a0a 2020 2020   in widths:.    
+00001160: 2020 2020 2020 2020 6966 206f 203c 3d20          if o <= 
+00001170: 6e75 6d3a 0a20 2020 2020 2020 2020 2020  num:.           
+00001180: 2020 2020 2072 6574 7572 6e20 7769 640a       return wid.
+00001190: 2020 2020 2020 2020 7265 7475 726e 2031          return 1
+000011a0: 0a0a 2020 2020 6465 6620 5f63 6f6c 6f75  ..    def _colou
+000011b0: 6d57 6964 7468 2873 656c 662c 2073 3a73  mWidth(self, s:s
+000011c0: 7472 293a 0a20 2020 2020 2020 2072 6573  tr):.        res
+000011d0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
+000011e0: 2063 6820 696e 2073 3a0a 2020 2020 2020   ch in s:.      
+000011f0: 2020 2020 2020 7265 7320 2b3d 2073 656c        res += sel
+00001200: 662e 5f67 6574 4368 6172 5769 6474 6828  f._getCharWidth(
+00001210: 6f72 6428 6368 2929 0a20 2020 2020 2020  ord(ch)).       
+00001220: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
+00001230: 2064 6566 205f 6368 616e 6765 436f 6c75   def _changeColu
+00001240: 6d6e 5769 6474 6828 7365 6c66 2c20 733a  mnWidth(self, s:
+00001250: 7374 722c 206c 656e 3a69 6e74 2920 2d3e  str, len:int) ->
+00001260: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
+00001270: 7320 3d20 300a 2020 2020 2020 2020 734c  s = 0.        sL
+00001280: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
+00001290: 2066 6f72 2063 6820 696e 2073 3a0a 2020   for ch in s:.  
+000012a0: 2020 2020 2020 2020 2020 7265 7320 2b3d            res +=
+000012b0: 2073 656c 662e 5f67 6574 4368 6172 5769   self._getCharWi
+000012c0: 6474 6828 6f72 6428 6368 2929 0a20 2020  dth(ord(ch)).   
+000012d0: 2020 2020 2020 2020 2069 6620 7265 7320           if res 
+000012e0: 3c3d 206c 656e 3a0a 2020 2020 2020 2020  <= len:.        
+000012f0: 2020 2020 2020 2020 734c 6973 742e 6170          sList.ap
+00001300: 7065 6e64 2863 6829 0a20 2020 2020 2020  pend(ch).       
+00001310: 2072 6574 7572 6e20 2727 2e6a 6f69 6e28   return ''.join(
+00001320: 734c 6973 7429 0a0a 2020 2020 6465 6620  sList)..    def 
+00001330: 5f72 6573 697a 6550 6963 2873 656c 662c  _resizePic(self,
+00001340: 2069 6d67 3a49 6d61 6765 2e49 6d61 6765   img:Image.Image
+00001350: 2c20 7469 6d65 3a66 6c6f 6174 293a 0a20  , time:float):. 
+00001360: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
+00001370: 672e 7265 7369 7a65 2828 696e 7428 696d  g.resize((int(im
+00001380: 672e 7369 7a65 5b30 5d20 2a20 7469 6d65  g.size[0] * time
+00001390: 292c 2069 6e74 2869 6d67 2e73 697a 655b  ), int(img.size[
+000013a0: 315d 202a 2074 696d 6529 2929 0a0a 2020  1] * time)))..  
+000013b0: 2020 6465 6620 5f66 696e 6452 6150 6963    def _findRaPic
+000013c0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+000013d0: 2020 2020 2020 206e 756d 203d 2027 3130         num = '10
+000013e0: 270a 2020 2020 2020 2020 6966 2073 656c  '.        if sel
+000013f0: 662e 706c 6179 6572 5261 7469 6e67 203c  f.playerRating <
+00001400: 2031 3030 303a 0a20 2020 2020 2020 2020   1000:.         
+00001410: 2020 206e 756d 203d 2027 3031 270a 2020     num = '01'.  
+00001420: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00001430: 706c 6179 6572 5261 7469 6e67 203c 2032  playerRating < 2
+00001440: 3030 303a 0a20 2020 2020 2020 2020 2020  000:.           
+00001450: 206e 756d 203d 2027 3032 270a 2020 2020   num = '02'.    
+00001460: 2020 2020 656c 6966 2073 656c 662e 706c      elif self.pl
+00001470: 6179 6572 5261 7469 6e67 203c 2033 3030  ayerRating < 300
+00001480: 303a 0a20 2020 2020 2020 2020 2020 206e  0:.            n
+00001490: 756d 203d 2027 3033 270a 2020 2020 2020  um = '03'.      
+000014a0: 2020 656c 6966 2073 656c 662e 706c 6179    elif self.play
+000014b0: 6572 5261 7469 6e67 203c 2034 3030 303a  erRating < 4000:
+000014c0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+000014d0: 203d 2027 3034 270a 2020 2020 2020 2020   = '04'.        
+000014e0: 656c 6966 2073 656c 662e 706c 6179 6572  elif self.player
+000014f0: 5261 7469 6e67 203c 2035 3030 303a 0a20  Rating < 5000:. 
+00001500: 2020 2020 2020 2020 2020 206e 756d 203d             num =
+00001510: 2027 3035 270a 2020 2020 2020 2020 656c   '05'.        el
+00001520: 6966 2073 656c 662e 706c 6179 6572 5261  if self.playerRa
+00001530: 7469 6e67 203c 2036 3030 303a 0a20 2020  ting < 6000:.   
+00001540: 2020 2020 2020 2020 206e 756d 203d 2027           num = '
+00001550: 3036 270a 2020 2020 2020 2020 656c 6966  06'.        elif
+00001560: 2073 656c 662e 706c 6179 6572 5261 7469   self.playerRati
+00001570: 6e67 203c 2037 3030 303a 0a20 2020 2020  ng < 7000:.     
+00001580: 2020 2020 2020 206e 756d 203d 2027 3037         num = '07
+00001590: 270a 2020 2020 2020 2020 656c 6966 2073  '.        elif s
+000015a0: 656c 662e 706c 6179 6572 5261 7469 6e67  elf.playerRating
+000015b0: 203c 2038 3030 303a 0a20 2020 2020 2020   < 8000:.       
+000015c0: 2020 2020 206e 756d 203d 2027 3038 270a       num = '08'.
+000015d0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+000015e0: 662e 706c 6179 6572 5261 7469 6e67 203c  f.playerRating <
+000015f0: 2038 3530 303a 0a20 2020 2020 2020 2020   8500:.         
+00001600: 2020 206e 756d 203d 2027 3039 270a 2020     num = '09'.  
+00001610: 2020 2020 2020 7265 7475 726e 2066 2755        return f'U
+00001620: 495f 434d 4e5f 4458 5261 7469 6e67 5f53  I_CMN_DXRating_S
+00001630: 5f7b 6e75 6d7d 2e70 6e67 270a 0a20 2020  _{num}.png'..   
+00001640: 2064 6566 205f 6472 6177 5261 7469 6e67   def _drawRating
+00001650: 2873 656c 662c 2072 6174 696e 6742 6173  (self, ratingBas
+00001660: 6549 6d67 3a49 6d61 6765 2e49 6d61 6765  eImg:Image.Image
+00001670: 293a 0a20 2020 2020 2020 2043 4f4c 4f55  ):.        COLOU
+00001680: 4d53 5f52 4154 494e 4720 3d20 5b38 362c  MS_RATING = [86,
+00001690: 2031 3030 2c20 3131 352c 2031 3330 2c20   100, 115, 130, 
+000016a0: 3134 355d 0a20 2020 2020 2020 2074 6865  145].        the
+000016b0: 5261 203d 2073 656c 662e 706c 6179 6572  Ra = self.player
+000016c0: 5261 7469 6e67 0a20 2020 2020 2020 2069  Rating.        i
+000016d0: 203d 2034 0a20 2020 2020 2020 2077 6869   = 4.        whi
+000016e0: 6c65 2074 6865 5261 3a0a 2020 2020 2020  le theRa:.      
+000016f0: 2020 2020 2020 6469 6769 7420 3d20 7468        digit = th
+00001700: 6552 6120 2520 3130 0a20 2020 2020 2020  eRa % 10.       
+00001710: 2020 2020 2074 6865 5261 203d 2074 6865       theRa = the
+00001720: 5261 202f 2f20 3130 0a20 2020 2020 2020  Ra // 10.       
+00001730: 2020 2020 2064 6967 6974 496d 6720 3d20       digitImg = 
+00001740: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
+00001750: 7069 635f 6469 7220 2b20 6627 5549 5f4e  pic_dir + f'UI_N
+00001760: 554d 5f44 7261 7469 6e67 5f7b 6469 6769  UM_Drating_{digi
+00001770: 747d 2e70 6e67 2729 2e63 6f6e 7665 7274  t}.png').convert
+00001780: 2827 5247 4241 2729 0a20 2020 2020 2020  ('RGBA').       
+00001790: 2020 2020 2064 6967 6974 496d 6720 3d20       digitImg = 
+000017a0: 7365 6c66 2e5f 7265 7369 7a65 5069 6328  self._resizePic(
+000017b0: 6469 6769 7449 6d67 2c20 302e 3629 0a20  digitImg, 0.6). 
+000017c0: 2020 2020 2020 2020 2020 2072 6174 696e             ratin
+000017d0: 6742 6173 6549 6d67 2e70 6173 7465 2864  gBaseImg.paste(d
+000017e0: 6967 6974 496d 672c 2028 434f 4c4f 554d  igitImg, (COLOUM
+000017f0: 535f 5241 5449 4e47 5b69 5d20 2d20 322c  S_RATING[i] - 2,
+00001800: 2039 292c 206d 6173 6b3d 6469 6769 7449   9), mask=digitI
+00001810: 6d67 2e73 706c 6974 2829 5b33 5d29 0a20  mg.split()[3]). 
+00001820: 2020 2020 2020 2020 2020 2069 203d 2069             i = i
+00001830: 202d 2031 0a20 2020 2020 2020 2072 6574   - 1.        ret
+00001840: 7572 6e20 7261 7469 6e67 4261 7365 496d  urn ratingBaseIm
+00001850: 670a 0a20 2020 2064 6566 205f 6472 6177  g..    def _draw
+00001860: 4265 7374 4c69 7374 2873 656c 662c 2069  BestList(self, i
+00001870: 6d67 3a49 6d61 6765 2e49 6d61 6765 2c20  mg:Image.Image, 
+00001880: 7364 4265 7374 3a42 6573 744c 6973 742c  sdBest:BestList,
+00001890: 2064 7842 6573 743a 4265 7374 4c69 7374   dxBest:BestList
+000018a0: 293a 0a20 2020 2020 2020 2069 7465 6d57  ):.        itemW
+000018b0: 203d 2031 3634 0a20 2020 2020 2020 2069   = 164.        i
+000018c0: 7465 6d48 203d 2038 380a 2020 2020 2020  temH = 88.      
+000018d0: 2020 436f 6c6f 7220 3d20 5b28 3639 2c20    Color = [(69, 
+000018e0: 3139 332c 2033 3629 2c20 2832 3535 2c20  193, 36), (255, 
+000018f0: 3138 362c 2031 292c 2028 3235 352c 2039  186, 1), (255, 9
+00001900: 302c 2031 3032 292c 2028 3133 342c 2034  0, 102), (134, 4
+00001910: 392c 2032 3030 292c 2028 3231 372c 2031  9, 200), (217, 1
+00001920: 3937 2c20 3233 3329 5d0a 2020 2020 2020  97, 233)].      
+00001930: 2020 6c65 7665 6c54 7269 6167 6c65 203d    levelTriagle =
+00001940: 205b 2869 7465 6d57 2c20 3029 2c20 2869   [(itemW, 0), (i
+00001950: 7465 6d57 202d 2032 372c 2030 292c 2028  temW - 27, 0), (
+00001960: 6974 656d 572c 2032 3729 5d0a 2020 2020  itemW, 27)].    
+00001970: 2020 2020 7261 6e6b 5069 6320 3d20 2744      rankPic = 'D
+00001980: 2043 2042 2042 4220 4242 4220 4120 4141   C B BB BBB A AA
+00001990: 2041 4141 2053 2053 7020 5353 2053 5370   AAA S Sp SS SSp
+000019a0: 2053 5353 2053 5353 7027 2e73 706c 6974   SSS SSSp'.split
+000019b0: 2827 2027 290a 2020 2020 2020 2020 636f  (' ').        co
+000019c0: 6d62 6f50 6963 203d 2027 2046 4320 4643  mboPic = ' FC FC
+000019d0: 7020 4150 2041 5070 272e 7370 6c69 7428  p AP APp'.split(
+000019e0: 2720 2729 0a20 2020 2020 2020 2069 6d67  ' ').        img
+000019f0: 4472 6177 203d 2049 6d61 6765 4472 6177  Draw = ImageDraw
+00001a00: 2e44 7261 7728 696d 6729 0a20 2020 2020  .Draw(img).     
+00001a10: 2020 2074 6974 6c65 466f 6e74 4e61 6d65     titleFontName
+00001a20: 203d 2053 5441 5449 4320 2b20 272f 6164   = STATIC + '/ad
+00001a30: 6f62 655f 7369 6d68 6569 2e6f 7466 270a  obe_simhei.otf'.
+00001a40: 2020 2020 2020 2020 666f 7220 6e75 6d20          for num 
+00001a50: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
+00001a60: 7364 4265 7374 2929 3a0a 2020 2020 2020  sdBest)):.      
+00001a70: 2020 2020 2020 6920 3d20 6e75 6d20 2f2f        i = num //
+00001a80: 2035 0a20 2020 2020 2020 2020 2020 206a   5.            j
+00001a90: 203d 206e 756d 2025 2035 0a20 2020 2020   = num % 5.     
+00001aa0: 2020 2020 2020 2063 6861 7274 496e 666f         chartInfo
+00001ab0: 203d 2073 6442 6573 745b 6e75 6d5d 0a20   = sdBest[num]. 
+00001ac0: 2020 2020 2020 2020 2020 2070 6e67 5061             pngPa
+00001ad0: 7468 203d 2073 656c 662e 636f 7665 725f  th = self.cover_
+00001ae0: 6469 7220 2b20 6627 7b67 6574 5f63 6f76  dir + f'{get_cov
+00001af0: 6572 5f6c 656e 355f 6964 2863 6861 7274  er_len5_id(chart
+00001b00: 496e 666f 2e69 644e 756d 297d 2e70 6e67  Info.idNum)}.png
+00001b10: 270a 2020 2020 2020 2020 2020 2020 6966  '.            if
+00001b20: 206e 6f74 206f 732e 7061 7468 2e65 7869   not os.path.exi
+00001b30: 7374 7328 706e 6750 6174 6829 3a0a 2020  sts(pngPath):.  
+00001b40: 2020 2020 2020 2020 2020 2020 2020 706e                pn
+00001b50: 6750 6174 6820 3d20 7365 6c66 2e63 6f76  gPath = self.cov
+00001b60: 6572 5f64 6972 202b 2027 3031 3030 302e  er_dir + '01000.
+00001b70: 706e 6727 0a20 2020 2020 2020 2020 2020  png'.           
+00001b80: 2074 656d 7020 3d20 496d 6167 652e 6f70   temp = Image.op
+00001b90: 656e 2870 6e67 5061 7468 292e 636f 6e76  en(pngPath).conv
+00001ba0: 6572 7428 2752 4742 2729 0a20 2020 2020  ert('RGB').     
+00001bb0: 2020 2020 2020 2074 656d 7020 3d20 7365         temp = se
+00001bc0: 6c66 2e5f 7265 7369 7a65 5069 6328 7465  lf._resizePic(te
+00001bd0: 6d70 2c20 6974 656d 5720 2f20 7465 6d70  mp, itemW / temp
+00001be0: 2e73 697a 655b 305d 290a 2020 2020 2020  .size[0]).      
+00001bf0: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
+00001c00: 702e 6372 6f70 2828 302c 2028 7465 6d70  p.crop((0, (temp
+00001c10: 2e73 697a 655b 315d 202d 2069 7465 6d48  .size[1] - itemH
+00001c20: 2920 2f20 322c 2069 7465 6d57 2c20 2874  ) / 2, itemW, (t
+00001c30: 656d 702e 7369 7a65 5b31 5d20 2b20 6974  emp.size[1] + it
+00001c40: 656d 4829 202f 2032 2929 0a20 2020 2020  emH) / 2)).     
+00001c50: 2020 2020 2020 2074 656d 7020 3d20 7465         temp = te
+00001c60: 6d70 2e66 696c 7465 7228 496d 6167 6546  mp.filter(ImageF
+00001c70: 696c 7465 722e 4761 7573 7369 616e 426c  ilter.GaussianBl
+00001c80: 7572 2833 2929 0a20 2020 2020 2020 2020  ur(3)).         
+00001c90: 2020 2074 656d 7020 3d20 7465 6d70 2e70     temp = temp.p
+00001ca0: 6f69 6e74 286c 616d 6264 6120 703a 2069  oint(lambda p: i
+00001cb0: 6e74 2870 202a 2030 2e37 3229 290a 0a20  nt(p * 0.72)).. 
+00001cc0: 2020 2020 2020 2020 2020 2074 656d 7044             tempD
+00001cd0: 7261 7720 3d20 496d 6167 6544 7261 772e  raw = ImageDraw.
+00001ce0: 4472 6177 2874 656d 7029 0a20 2020 2020  Draw(temp).     
+00001cf0: 2020 2020 2020 2074 656d 7044 7261 772e         tempDraw.
+00001d00: 706f 6c79 676f 6e28 6c65 7665 6c54 7269  polygon(levelTri
+00001d10: 6167 6c65 2c20 436f 6c6f 725b 6368 6172  agle, Color[char
+00001d20: 7449 6e66 6f2e 6469 6666 5d29 0a20 2020  tInfo.diff]).   
+00001d30: 2020 2020 2020 2020 2066 6f6e 7420 3d20           font = 
+00001d40: 496d 6167 6546 6f6e 742e 7472 7565 7479  ImageFont.truety
+00001d50: 7065 2874 6974 6c65 466f 6e74 4e61 6d65  pe(titleFontName
+00001d60: 2c20 3136 2c20 656e 636f 6469 6e67 3d27  , 16, encoding='
+00001d70: 7574 662d 3827 290a 2020 2020 2020 2020  utf-8').        
+00001d80: 2020 2020 7469 746c 6520 3d20 6368 6172      title = char
+00001d90: 7449 6e66 6f2e 7469 746c 650a 2020 2020  tInfo.title.    
+00001da0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00001db0: 5f63 6f6c 6f75 6d57 6964 7468 2874 6974  _coloumWidth(tit
+00001dc0: 6c65 2920 3e20 3135 3a0a 2020 2020 2020  le) > 15:.      
+00001dd0: 2020 2020 2020 2020 2020 7469 746c 6520            title 
+00001de0: 3d20 7365 6c66 2e5f 6368 616e 6765 436f  = self._changeCo
+00001df0: 6c75 6d6e 5769 6474 6828 7469 746c 652c  lumnWidth(title,
+00001e00: 2031 3429 202b 2027 2e2e 2e27 0a20 2020   14) + '...'.   
+00001e10: 2020 2020 2020 2020 2074 656d 7044 7261           tempDra
+00001e20: 772e 7465 7874 2828 382c 2038 292c 2074  w.text((8, 8), t
+00001e30: 6974 6c65 2c20 2777 6869 7465 272c 2066  itle, 'white', f
+00001e40: 6f6e 7429 0a20 2020 2020 2020 2020 2020  ont).           
+00001e50: 2066 6f6e 7420 3d20 496d 6167 6546 6f6e   font = ImageFon
+00001e60: 742e 7472 7565 7479 7065 2874 6974 6c65  t.truetype(title
+00001e70: 466f 6e74 4e61 6d65 2c20 3134 2c20 656e  FontName, 14, en
+00001e80: 636f 6469 6e67 3d27 7574 662d 3827 290a  coding='utf-8').
+00001e90: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00001ea0: 7044 7261 772e 7465 7874 2828 372c 2032  pDraw.text((7, 2
+00001eb0: 3829 2c20 6627 7b22 252e 3466 2220 2520  8), f'{"%.4f" % 
+00001ec0: 6368 6172 7449 6e66 6f2e 6163 6869 6576  chartInfo.achiev
+00001ed0: 656d 656e 747d 2527 2c20 2777 6869 7465  ement}%', 'white
+00001ee0: 272c 2066 6f6e 7429 0a20 2020 2020 2020  ', font).       
+00001ef0: 2020 2020 2072 616e 6b49 6d67 203d 2049       rankImg = I
+00001f00: 6d61 6765 2e6f 7065 6e28 7365 6c66 2e70  mage.open(self.p
+00001f10: 6963 5f64 6972 202b 2066 2755 495f 4741  ic_dir + f'UI_GA
+00001f20: 4d5f 5261 6e6b 5f7b 7261 6e6b 5069 635b  M_Rank_{rankPic[
+00001f30: 6368 6172 7449 6e66 6f2e 7363 6f72 6549  chartInfo.scoreI
+00001f40: 645d 7d2e 706e 6727 292e 636f 6e76 6572  d]}.png').conver
+00001f50: 7428 2752 4742 4127 290a 2020 2020 2020  t('RGBA').      
+00001f60: 2020 2020 2020 7261 6e6b 496d 6720 3d20        rankImg = 
+00001f70: 7365 6c66 2e5f 7265 7369 7a65 5069 6328  self._resizePic(
+00001f80: 7261 6e6b 496d 672c 2030 2e33 290a 2020  rankImg, 0.3).  
+00001f90: 2020 2020 2020 2020 2020 7465 6d70 2e70            temp.p
+00001fa0: 6173 7465 2872 616e 6b49 6d67 2c20 2838  aste(rankImg, (8
+00001fb0: 382c 2032 3829 2c20 7261 6e6b 496d 672e  8, 28), rankImg.
+00001fc0: 7370 6c69 7428 295b 335d 290a 2020 2020  split()[3]).    
+00001fd0: 2020 2020 2020 2020 6966 2063 6861 7274          if chart
+00001fe0: 496e 666f 2e63 6f6d 626f 4964 3a0a 2020  Info.comboId:.  
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002000: 6d62 6f49 6d67 203d 2049 6d61 6765 2e6f  mboImg = Image.o
+00002010: 7065 6e28 7365 6c66 2e70 6963 5f64 6972  pen(self.pic_dir
+00002020: 202b 2066 2755 495f 4d53 535f 4d42 6173   + f'UI_MSS_MBas
+00002030: 655f 4963 6f6e 5f7b 636f 6d62 6f50 6963  e_Icon_{comboPic
+00002040: 5b63 6861 7274 496e 666f 2e63 6f6d 626f  [chartInfo.combo
+00002050: 4964 5d7d 5f53 2e70 6e67 2729 2e63 6f6e  Id]}_S.png').con
+00002060: 7665 7274 2827 5247 4241 2729 0a20 2020  vert('RGBA').   
+00002070: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00002080: 626f 496d 6720 3d20 7365 6c66 2e5f 7265  boImg = self._re
+00002090: 7369 7a65 5069 6328 636f 6d62 6f49 6d67  sizePic(comboImg
+000020a0: 2c20 302e 3435 290a 2020 2020 2020 2020  , 0.45).        
+000020b0: 2020 2020 2020 2020 7465 6d70 2e70 6173          temp.pas
+000020c0: 7465 2863 6f6d 626f 496d 672c 2028 3131  te(comboImg, (11
+000020d0: 392c 2032 3729 2c20 636f 6d62 6f49 6d67  9, 27), comboImg
+000020e0: 2e73 706c 6974 2829 5b33 5d29 0a20 2020  .split()[3]).   
+000020f0: 2020 2020 2020 2020 2066 6f6e 7420 3d20           font = 
+00002100: 496d 6167 6546 6f6e 742e 7472 7565 7479  ImageFont.truety
+00002110: 7065 2853 5441 5449 4320 2b20 272f 6164  pe(STATIC + '/ad
+00002120: 6f62 655f 7369 6d68 6569 2e6f 7466 272c  obe_simhei.otf',
+00002130: 2031 322c 2065 6e63 6f64 696e 673d 2775   12, encoding='u
+00002140: 7466 2d38 2729 0a20 2020 2020 2020 2020  tf-8').         
+00002150: 2020 2074 656d 7044 7261 772e 7465 7874     tempDraw.text
+00002160: 2828 382c 2034 3429 2c20 6627 4261 7365  ((8, 44), f'Base
+00002170: 3a20 7b63 6861 7274 496e 666f 2e64 737d  : {chartInfo.ds}
+00002180: 202d 3e20 7b63 6861 7274 496e 666f 2e72   -> {chartInfo.r
+00002190: 617d 272c 2027 7768 6974 6527 2c20 666f  a}', 'white', fo
+000021a0: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+000021b0: 666f 6e74 203d 2049 6d61 6765 466f 6e74  font = ImageFont
+000021c0: 2e74 7275 6574 7970 6528 5354 4154 4943  .truetype(STATIC
+000021d0: 202b 272f 6164 6f62 655f 7369 6d68 6569   +'/adobe_simhei
+000021e0: 2e6f 7466 272c 2031 382c 2065 6e63 6f64  .otf', 18, encod
+000021f0: 696e 673d 2775 7466 2d38 2729 0a20 2020  ing='utf-8').   
+00002200: 2020 2020 2020 2020 2074 656d 7044 7261           tempDra
+00002210: 772e 7465 7874 2828 382c 2036 3029 2c20  w.text((8, 60), 
+00002220: 6627 237b 6e75 6d20 2b20 317d 272c 2027  f'#{num + 1}', '
+00002230: 7768 6974 6527 2c20 666f 6e74 290a 0a20  white', font).. 
+00002240: 2020 2020 2020 2020 2020 2072 6563 4261             recBa
+00002250: 7365 203d 2049 6d61 6765 2e6e 6577 2827  se = Image.new('
+00002260: 5247 4241 272c 2028 6974 656d 572c 2069  RGBA', (itemW, i
+00002270: 7465 6d48 292c 2027 626c 6163 6b27 290a  temH), 'black').
+00002280: 2020 2020 2020 2020 2020 2020 7265 6342              recB
+00002290: 6173 6520 3d20 7265 6342 6173 652e 706f  ase = recBase.po
+000022a0: 696e 7428 6c61 6d62 6461 2070 3a20 696e  int(lambda p: in
+000022b0: 7428 7020 2a20 302e 3829 290a 2020 2020  t(p * 0.8)).    
+000022c0: 2020 2020 2020 2020 696d 672e 7061 7374          img.past
+000022d0: 6528 7265 6342 6173 652c 2028 7365 6c66  e(recBase, (self
+000022e0: 2e43 4f4c 4f55 4d53 5f49 4d47 5b6a 5d20  .COLOUMS_IMG[j] 
+000022f0: 2b20 352c 2073 656c 662e 524f 5753 5f49  + 5, self.ROWS_I
+00002300: 4d47 5b69 202b 2031 5d20 2b20 3529 290a  MG[i + 1] + 5)).
+00002310: 2020 2020 2020 2020 2020 2020 696d 672e              img.
+00002320: 7061 7374 6528 7465 6d70 2c20 2873 656c  paste(temp, (sel
+00002330: 662e 434f 4c4f 554d 535f 494d 475b 6a5d  f.COLOUMS_IMG[j]
+00002340: 202b 2034 2c20 7365 6c66 2e52 4f57 535f   + 4, self.ROWS_
+00002350: 494d 475b 6920 2b20 315d 202b 2034 2929  IMG[i + 1] + 4))
+00002360: 0a20 2020 2020 2020 2066 6f72 206e 756d  .        for num
+00002370: 2069 6e20 7261 6e67 6528 6c65 6e28 7364   in range(len(sd
+00002380: 4265 7374 292c 2073 6442 6573 742e 7369  Best), sdBest.si
+00002390: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
+000023a0: 2069 203d 206e 756d 202f 2f20 350a 2020   i = num // 5.  
+000023b0: 2020 2020 2020 2020 2020 6a20 3d20 6e75            j = nu
+000023c0: 6d20 2520 350a 2020 2020 2020 2020 2020  m % 5.          
+000023d0: 2020 7465 6d70 203d 2049 6d61 6765 2e6f    temp = Image.o
+000023e0: 7065 6e28 7365 6c66 2e63 6f76 6572 5f64  pen(self.cover_d
+000023f0: 6972 202b 2066 2730 3130 3030 2e70 6e67  ir + f'01000.png
+00002400: 2729 2e63 6f6e 7665 7274 2827 5247 4227  ').convert('RGB'
+00002410: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+00002420: 6d70 203d 2073 656c 662e 5f72 6573 697a  mp = self._resiz
+00002430: 6550 6963 2874 656d 702c 2069 7465 6d57  ePic(temp, itemW
+00002440: 202f 2074 656d 702e 7369 7a65 5b30 5d29   / temp.size[0])
+00002450: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00002460: 7020 3d20 7465 6d70 2e63 726f 7028 2830  p = temp.crop((0
+00002470: 2c20 2874 656d 702e 7369 7a65 5b31 5d20  , (temp.size[1] 
+00002480: 2d20 6974 656d 4829 202f 2032 2c20 6974  - itemH) / 2, it
+00002490: 656d 572c 2028 7465 6d70 2e73 697a 655b  emW, (temp.size[
+000024a0: 315d 202b 2069 7465 6d48 2920 2f20 3229  1] + itemH) / 2)
+000024b0: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+000024c0: 6d70 203d 2074 656d 702e 6669 6c74 6572  mp = temp.filter
+000024d0: 2849 6d61 6765 4669 6c74 6572 2e47 6175  (ImageFilter.Gau
+000024e0: 7373 6961 6e42 6c75 7228 3129 290a 2020  ssianBlur(1)).  
+000024f0: 2020 2020 2020 2020 2020 696d 672e 7061            img.pa
+00002500: 7374 6528 7465 6d70 2c20 2873 656c 662e  ste(temp, (self.
+00002510: 434f 4c4f 554d 535f 494d 475b 6a5d 202b  COLOUMS_IMG[j] +
+00002520: 2034 2c20 7365 6c66 2e52 4f57 535f 494d   4, self.ROWS_IM
+00002530: 475b 6920 2b20 315d 202b 2034 2929 0a20  G[i + 1] + 4)). 
+00002540: 2020 2020 2020 2066 6f72 206e 756d 2069         for num i
+00002550: 6e20 7261 6e67 6528 302c 206c 656e 2864  n range(0, len(d
+00002560: 7842 6573 7429 293a 0a20 2020 2020 2020  xBest)):.       
+00002570: 2020 2020 2069 203d 206e 756d 202f 2f20       i = num // 
+00002580: 330a 2020 2020 2020 2020 2020 2020 6a20  3.            j 
+00002590: 3d20 6e75 6d20 2520 330a 2020 2020 2020  = num % 3.      
+000025a0: 2020 2020 2020 6368 6172 7449 6e66 6f20        chartInfo 
+000025b0: 3d20 6478 4265 7374 5b6e 756d 5d0a 2020  = dxBest[num].  
+000025c0: 2020 2020 2020 2020 2020 706e 6750 6174            pngPat
+000025d0: 6820 3d20 7365 6c66 2e63 6f76 6572 5f64  h = self.cover_d
+000025e0: 6972 202b 2066 277b 6765 745f 636f 7665  ir + f'{get_cove
+000025f0: 725f 6c65 6e35 5f69 6428 6368 6172 7449  r_len5_id(chartI
+00002600: 6e66 6f2e 6964 4e75 6d29 7d2e 706e 6727  nfo.idNum)}.png'
+00002610: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002620: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
+00002630: 7473 2870 6e67 5061 7468 293a 0a20 2020  ts(pngPath):.   
+00002640: 2020 2020 2020 2020 2020 2020 2070 6e67               png
+00002650: 5061 7468 203d 2073 656c 662e 636f 7665  Path = self.cove
+00002660: 725f 6469 7220 2b20 2730 3130 3030 2e70  r_dir + '01000.p
+00002670: 6e67 270a 2020 2020 2020 2020 2020 2020  ng'.            
+00002680: 7465 6d70 203d 2049 6d61 6765 2e6f 7065  temp = Image.ope
+00002690: 6e28 706e 6750 6174 6829 2e63 6f6e 7665  n(pngPath).conve
+000026a0: 7274 2827 5247 4227 290a 2020 2020 2020  rt('RGB').      
+000026b0: 2020 2020 2020 7465 6d70 203d 2073 656c        temp = sel
+000026c0: 662e 5f72 6573 697a 6550 6963 2874 656d  f._resizePic(tem
+000026d0: 702c 2069 7465 6d57 202f 2074 656d 702e  p, itemW / temp.
+000026e0: 7369 7a65 5b30 5d29 0a20 2020 2020 2020  size[0]).       
+000026f0: 2020 2020 2074 656d 7020 3d20 7465 6d70       temp = temp
+00002700: 2e63 726f 7028 2830 2c20 2874 656d 702e  .crop((0, (temp.
+00002710: 7369 7a65 5b31 5d20 2d20 6974 656d 4829  size[1] - itemH)
+00002720: 202f 2032 2c20 6974 656d 572c 2028 7465   / 2, itemW, (te
+00002730: 6d70 2e73 697a 655b 315d 202b 2069 7465  mp.size[1] + ite
+00002740: 6d48 2920 2f20 3229 290a 2020 2020 2020  mH) / 2)).      
+00002750: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
+00002760: 702e 6669 6c74 6572 2849 6d61 6765 4669  p.filter(ImageFi
+00002770: 6c74 6572 2e47 6175 7373 6961 6e42 6c75  lter.GaussianBlu
+00002780: 7228 3329 290a 2020 2020 2020 2020 2020  r(3)).          
+00002790: 2020 7465 6d70 203d 2074 656d 702e 706f    temp = temp.po
+000027a0: 696e 7428 6c61 6d62 6461 2070 3a20 696e  int(lambda p: in
+000027b0: 7428 7020 2a20 302e 3732 2929 0a0a 2020  t(p * 0.72))..  
+000027c0: 2020 2020 2020 2020 2020 7465 6d70 4472            tempDr
+000027d0: 6177 203d 2049 6d61 6765 4472 6177 2e44  aw = ImageDraw.D
+000027e0: 7261 7728 7465 6d70 290a 2020 2020 2020  raw(temp).      
+000027f0: 2020 2020 2020 7465 6d70 4472 6177 2e70        tempDraw.p
+00002800: 6f6c 7967 6f6e 286c 6576 656c 5472 6961  olygon(levelTria
+00002810: 676c 652c 2043 6f6c 6f72 5b63 6861 7274  gle, Color[chart
+00002820: 496e 666f 2e64 6966 665d 290a 2020 2020  Info.diff]).    
+00002830: 2020 2020 2020 2020 666f 6e74 203d 2049          font = I
+00002840: 6d61 6765 466f 6e74 2e74 7275 6574 7970  mageFont.truetyp
+00002850: 6528 7469 746c 6546 6f6e 744e 616d 652c  e(titleFontName,
+00002860: 2031 362c 2065 6e63 6f64 696e 673d 2775   16, encoding='u
+00002870: 7466 2d38 2729 0a20 2020 2020 2020 2020  tf-8').         
+00002880: 2020 2074 6974 6c65 203d 2063 6861 7274     title = chart
+00002890: 496e 666f 2e74 6974 6c65 0a20 2020 2020  Info.title.     
+000028a0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+000028b0: 636f 6c6f 756d 5769 6474 6828 7469 746c  coloumWidth(titl
+000028c0: 6529 203e 2031 353a 0a20 2020 2020 2020  e) > 15:.       
+000028d0: 2020 2020 2020 2020 2074 6974 6c65 203d           title =
+000028e0: 2073 656c 662e 5f63 6861 6e67 6543 6f6c   self._changeCol
+000028f0: 756d 6e57 6964 7468 2874 6974 6c65 2c20  umnWidth(title, 
+00002900: 3134 2920 2b20 272e 2e2e 270a 2020 2020  14) + '...'.    
+00002910: 2020 2020 2020 2020 7465 6d70 4472 6177          tempDraw
+00002920: 2e74 6578 7428 2838 2c20 3829 2c20 7469  .text((8, 8), ti
+00002930: 746c 652c 2027 7768 6974 6527 2c20 666f  tle, 'white', fo
+00002940: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+00002950: 666f 6e74 203d 2049 6d61 6765 466f 6e74  font = ImageFont
+00002960: 2e74 7275 6574 7970 6528 7469 746c 6546  .truetype(titleF
+00002970: 6f6e 744e 616d 652c 2031 342c 2065 6e63  ontName, 14, enc
+00002980: 6f64 696e 673d 2775 7466 2d38 2729 0a0a  oding='utf-8')..
+00002990: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+000029a0: 4472 6177 2e74 6578 7428 2837 2c20 3238  Draw.text((7, 28
+000029b0: 292c 2066 277b 2225 2e34 6622 2025 2063  ), f'{"%.4f" % c
+000029c0: 6861 7274 496e 666f 2e61 6368 6965 7665  hartInfo.achieve
+000029d0: 6d65 6e74 7d25 272c 2027 7768 6974 6527  ment}%', 'white'
+000029e0: 2c20 666f 6e74 290a 2020 2020 2020 2020  , font).        
+000029f0: 2020 2020 7261 6e6b 496d 6720 3d20 496d      rankImg = Im
+00002a00: 6167 652e 6f70 656e 2873 656c 662e 7069  age.open(self.pi
+00002a10: 635f 6469 7220 2b20 6627 5549 5f47 414d  c_dir + f'UI_GAM
+00002a20: 5f52 616e 6b5f 7b72 616e 6b50 6963 5b63  _Rank_{rankPic[c
+00002a30: 6861 7274 496e 666f 2e73 636f 7265 4964  hartInfo.scoreId
+00002a40: 5d7d 2e70 6e67 2729 2e63 6f6e 7665 7274  ]}.png').convert
+00002a50: 2827 5247 4241 2729 0a20 2020 2020 2020  ('RGBA').       
+00002a60: 2020 2020 2072 616e 6b49 6d67 203d 2073       rankImg = s
+00002a70: 656c 662e 5f72 6573 697a 6550 6963 2872  elf._resizePic(r
+00002a80: 616e 6b49 6d67 2c20 302e 3329 0a20 2020  ankImg, 0.3).   
+00002a90: 2020 2020 2020 2020 2074 656d 702e 7061           temp.pa
+00002aa0: 7374 6528 7261 6e6b 496d 672c 2028 3838  ste(rankImg, (88
+00002ab0: 2c20 3238 292c 2072 616e 6b49 6d67 2e73  , 28), rankImg.s
+00002ac0: 706c 6974 2829 5b33 5d29 0a20 2020 2020  plit()[3]).     
+00002ad0: 2020 2020 2020 2069 6620 6368 6172 7449         if chartI
+00002ae0: 6e66 6f2e 636f 6d62 6f49 643a 0a20 2020  nfo.comboId:.   
+00002af0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00002b00: 626f 496d 6720 3d20 496d 6167 652e 6f70  boImg = Image.op
+00002b10: 656e 2873 656c 662e 7069 635f 6469 7220  en(self.pic_dir 
+00002b20: 2b20 6627 5549 5f4d 5353 5f4d 4261 7365  + f'UI_MSS_MBase
+00002b30: 5f49 636f 6e5f 7b63 6f6d 626f 5069 635b  _Icon_{comboPic[
+00002b40: 6368 6172 7449 6e66 6f2e 636f 6d62 6f49  chartInfo.comboI
+00002b50: 645d 7d5f 532e 706e 6727 292e 636f 6e76  d]}_S.png').conv
+00002b60: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00002b70: 2020 2020 2020 2020 2027 5247 4241 2729           'RGBA')
+00002b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b90: 2063 6f6d 626f 496d 6720 3d20 7365 6c66   comboImg = self
+00002ba0: 2e5f 7265 7369 7a65 5069 6328 636f 6d62  ._resizePic(comb
+00002bb0: 6f49 6d67 2c20 302e 3435 290a 2020 2020  oImg, 0.45).    
+00002bc0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00002bd0: 2e70 6173 7465 2863 6f6d 626f 496d 672c  .paste(comboImg,
+00002be0: 2028 3131 392c 2032 3729 2c20 636f 6d62   (119, 27), comb
+00002bf0: 6f49 6d67 2e73 706c 6974 2829 5b33 5d29  oImg.split()[3])
+00002c00: 0a20 2020 2020 2020 2020 2020 2066 6f6e  .            fon
+00002c10: 7420 3d20 496d 6167 6546 6f6e 742e 7472  t = ImageFont.tr
+00002c20: 7565 7479 7065 2853 5441 5449 4320 2b20  uetype(STATIC + 
+00002c30: 272f 6164 6f62 655f 7369 6d68 6569 2e6f  '/adobe_simhei.o
+00002c40: 7466 272c 2031 322c 2065 6e63 6f64 696e  tf', 12, encodin
+00002c50: 673d 2775 7466 2d38 2729 0a20 2020 2020  g='utf-8').     
+00002c60: 2020 2020 2020 2074 656d 7044 7261 772e         tempDraw.
+00002c70: 7465 7874 2828 382c 2034 3429 2c20 6627  text((8, 44), f'
+00002c80: 4261 7365 3a20 7b63 6861 7274 496e 666f  Base: {chartInfo
+00002c90: 2e64 737d 202d 3e20 7b63 6861 7274 496e  .ds} -> {chartIn
+00002ca0: 666f 2e72 617d 272c 2027 7768 6974 6527  fo.ra}', 'white'
+00002cb0: 2c20 666f 6e74 290a 2020 2020 2020 2020  , font).        
+00002cc0: 2020 2020 666f 6e74 203d 2049 6d61 6765      font = Image
+00002cd0: 466f 6e74 2e74 7275 6574 7970 6528 5354  Font.truetype(ST
+00002ce0: 4154 4943 202b 2027 2f61 646f 6265 5f73  ATIC + '/adobe_s
+00002cf0: 696d 6865 692e 6f74 6627 2c20 3138 2c20  imhei.otf', 18, 
+00002d00: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
+00002d10: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+00002d20: 6d70 4472 6177 2e74 6578 7428 2838 2c20  mpDraw.text((8, 
+00002d30: 3630 292c 2066 2723 7b6e 756d 202b 2031  60), f'#{num + 1
+00002d40: 7d27 2c20 2777 6869 7465 272c 2066 6f6e  }', 'white', fon
+00002d50: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+00002d60: 7265 6342 6173 6520 3d20 496d 6167 652e  recBase = Image.
+00002d70: 6e65 7728 2752 4742 4127 2c20 2869 7465  new('RGBA', (ite
+00002d80: 6d57 2c20 6974 656d 4829 2c20 2762 6c61  mW, itemH), 'bla
+00002d90: 636b 2729 0a20 2020 2020 2020 2020 2020  ck').           
+00002da0: 2072 6563 4261 7365 203d 2072 6563 4261   recBase = recBa
+00002db0: 7365 2e70 6f69 6e74 286c 616d 6264 6120  se.point(lambda 
+00002dc0: 703a 2069 6e74 2870 202a 2030 2e38 2929  p: int(p * 0.8))
+00002dd0: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
+00002de0: 2e70 6173 7465 2872 6563 4261 7365 2c20  .paste(recBase, 
+00002df0: 2873 656c 662e 434f 4c4f 554d 535f 494d  (self.COLOUMS_IM
+00002e00: 475b 6a20 2b20 365d 202b 2035 2c20 7365  G[j + 6] + 5, se
+00002e10: 6c66 2e52 4f57 535f 494d 475b 6920 2b20  lf.ROWS_IMG[i + 
+00002e20: 315d 202b 2035 2929 0a20 2020 2020 2020  1] + 5)).       
+00002e30: 2020 2020 2069 6d67 2e70 6173 7465 2874       img.paste(t
+00002e40: 656d 702c 2028 7365 6c66 2e43 4f4c 4f55  emp, (self.COLOU
+00002e50: 4d53 5f49 4d47 5b6a 202b 2036 5d20 2b20  MS_IMG[j + 6] + 
+00002e60: 342c 2073 656c 662e 524f 5753 5f49 4d47  4, self.ROWS_IMG
+00002e70: 5b69 202b 2031 5d20 2b20 3429 290a 2020  [i + 1] + 4)).  
+00002e80: 2020 2020 2020 666f 7220 6e75 6d20 696e        for num in
+00002e90: 2072 616e 6765 286c 656e 2864 7842 6573   range(len(dxBes
+00002ea0: 7429 2c20 6478 4265 7374 2e73 697a 6529  t), dxBest.size)
+00002eb0: 3a0a 2020 2020 2020 2020 2020 2020 6920  :.            i 
+00002ec0: 3d20 6e75 6d20 2f2f 2033 0a20 2020 2020  = num // 3.     
+00002ed0: 2020 2020 2020 206a 203d 206e 756d 2025         j = num %
+00002ee0: 2033 0a20 2020 2020 2020 2020 2020 2074   3.            t
+00002ef0: 656d 7020 3d20 496d 6167 652e 6f70 656e  emp = Image.open
+00002f00: 2873 656c 662e 636f 7665 725f 6469 7220  (self.cover_dir 
+00002f10: 2b20 6627 3031 3030 302e 706e 6727 292e  + f'01000.png').
+00002f20: 636f 6e76 6572 7428 2752 4742 2729 0a20  convert('RGB'). 
+00002f30: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
+00002f40: 3d20 7365 6c66 2e5f 7265 7369 7a65 5069  = self._resizePi
+00002f50: 6328 7465 6d70 2c20 6974 656d 5720 2f20  c(temp, itemW / 
+00002f60: 7465 6d70 2e73 697a 655b 305d 290a 2020  temp.size[0]).  
+00002f70: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
+00002f80: 2074 656d 702e 6372 6f70 2828 302c 2028   temp.crop((0, (
+00002f90: 7465 6d70 2e73 697a 655b 315d 202d 2069  temp.size[1] - i
+00002fa0: 7465 6d48 2920 2f20 322c 2069 7465 6d57  temH) / 2, itemW
+00002fb0: 2c20 2874 656d 702e 7369 7a65 5b31 5d20  , (temp.size[1] 
+00002fc0: 2b20 6974 656d 4829 202f 2032 2929 0a20  + itemH) / 2)). 
+00002fd0: 2020 2020 2020 2020 2020 2074 656d 7020             temp 
+00002fe0: 3d20 7465 6d70 2e66 696c 7465 7228 496d  = temp.filter(Im
+00002ff0: 6167 6546 696c 7465 722e 4761 7573 7369  ageFilter.Gaussi
+00003000: 616e 426c 7572 2831 2929 0a20 2020 2020  anBlur(1)).     
+00003010: 2020 2020 2020 2069 6d67 2e70 6173 7465         img.paste
+00003020: 2874 656d 702c 2028 7365 6c66 2e43 4f4c  (temp, (self.COL
+00003030: 4f55 4d53 5f49 4d47 5b6a 202b 2036 5d20  OUMS_IMG[j + 6] 
+00003040: 2b20 342c 2073 656c 662e 524f 5753 5f49  + 4, self.ROWS_I
+00003050: 4d47 5b69 202b 2031 5d20 2b20 3429 290a  MG[i + 1] + 4)).
+00003060: 0a20 2020 2064 6566 2064 7261 7728 7365  .    def draw(se
+00003070: 6c66 293a 0a20 2020 2020 2020 2073 706c  lf):.        spl
+00003080: 6173 684c 6f67 6f20 3d20 496d 6167 652e  ashLogo = Image.
+00003090: 6f70 656e 2873 656c 662e 7069 635f 6469  open(self.pic_di
+000030a0: 7220 2b20 2755 495f 434d 4e5f 5461 6254  r + 'UI_CMN_TabT
+000030b0: 6974 6c65 5f4d 6169 6d61 6954 6974 6c65  itle_MaimaiTitle
+000030c0: 5f56 6572 3231 342e 706e 6727 292e 636f  _Ver214.png').co
+000030d0: 6e76 6572 7428 2752 4742 4127 290a 2020  nvert('RGBA').  
+000030e0: 2020 2020 2020 7370 6c61 7368 4c6f 676f        splashLogo
+000030f0: 203d 2073 656c 662e 5f72 6573 697a 6550   = self._resizeP
+00003100: 6963 2873 706c 6173 684c 6f67 6f2c 2030  ic(splashLogo, 0
+00003110: 2e36 3529 0a20 2020 2020 2020 2073 656c  .65).        sel
+00003120: 662e 696d 672e 7061 7374 6528 7370 6c61  f.img.paste(spla
+00003130: 7368 4c6f 676f 2c20 2831 302c 2031 3029  shLogo, (10, 10)
+00003140: 2c20 6d61 736b 3d73 706c 6173 684c 6f67  , mask=splashLog
+00003150: 6f2e 7370 6c69 7428 295b 335d 290a 0a20  o.split()[3]).. 
+00003160: 2020 2020 2020 2072 6174 696e 6742 6173         ratingBas
+00003170: 6549 6d67 203d 2049 6d61 6765 2e6f 7065  eImg = Image.ope
+00003180: 6e28 7365 6c66 2e70 6963 5f64 6972 202b  n(self.pic_dir +
+00003190: 2073 656c 662e 5f66 696e 6452 6150 6963   self._findRaPic
+000031a0: 2829 292e 636f 6e76 6572 7428 2752 4742  ()).convert('RGB
+000031b0: 4127 290a 2020 2020 2020 2020 7261 7469  A').        rati
+000031c0: 6e67 4261 7365 496d 6720 3d20 7365 6c66  ngBaseImg = self
+000031d0: 2e5f 6472 6177 5261 7469 6e67 2872 6174  ._drawRating(rat
+000031e0: 696e 6742 6173 6549 6d67 290a 2020 2020  ingBaseImg).    
+000031f0: 2020 2020 7261 7469 6e67 4261 7365 496d      ratingBaseIm
+00003200: 6720 3d20 7365 6c66 2e5f 7265 7369 7a65  g = self._resize
+00003210: 5069 6328 7261 7469 6e67 4261 7365 496d  Pic(ratingBaseIm
+00003220: 672c 2030 2e38 3529 0a20 2020 2020 2020  g, 0.85).       
+00003230: 2073 656c 662e 696d 672e 7061 7374 6528   self.img.paste(
+00003240: 7261 7469 6e67 4261 7365 496d 672c 2028  ratingBaseImg, (
+00003250: 3234 302c 2038 292c 206d 6173 6b3d 7261  240, 8), mask=ra
+00003260: 7469 6e67 4261 7365 496d 672e 7370 6c69  tingBaseImg.spli
+00003270: 7428 295b 335d 290a 0a20 2020 2020 2020  t()[3])..       
+00003280: 206e 616d 6550 6c61 7465 496d 6720 3d20   namePlateImg = 
+00003290: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
+000032a0: 7069 635f 6469 7220 2b20 2755 495f 5453  pic_dir + 'UI_TS
+000032b0: 545f 506c 6174 654d 6173 6b2e 706e 6727  T_PlateMask.png'
+000032c0: 292e 636f 6e76 6572 7428 2752 4742 4127  ).convert('RGBA'
+000032d0: 290a 2020 2020 2020 2020 6e61 6d65 506c  ).        namePl
+000032e0: 6174 6549 6d67 203d 206e 616d 6550 6c61  ateImg = namePla
+000032f0: 7465 496d 672e 7265 7369 7a65 2828 3238  teImg.resize((28
+00003300: 352c 2034 3029 290a 2020 2020 2020 2020  5, 40)).        
+00003310: 6e61 6d65 506c 6174 6544 7261 7720 3d20  namePlateDraw = 
+00003320: 496d 6167 6544 7261 772e 4472 6177 286e  ImageDraw.Draw(n
+00003330: 616d 6550 6c61 7465 496d 6729 0a20 2020  amePlateImg).   
+00003340: 2020 2020 2066 6f6e 7431 203d 2049 6d61       font1 = Ima
+00003350: 6765 466f 6e74 2e74 7275 6574 7970 6528  geFont.truetype(
+00003360: 5354 4154 4943 202b 2027 2f6d 7379 682e  STATIC + '/msyh.
+00003370: 7474 6327 2c20 3238 2c20 656e 636f 6469  ttc', 28, encodi
+00003380: 6e67 3d27 756e 6963 2729 0a20 2020 2020  ng='unic').     
+00003390: 2020 206e 616d 6550 6c61 7465 4472 6177     namePlateDraw
+000033a0: 2e74 6578 7428 2831 322c 2034 292c 2027  .text((12, 4), '
+000033b0: 2027 2e6a 6f69 6e28 6c69 7374 2873 656c   '.join(list(sel
+000033c0: 662e 7573 6572 4e61 6d65 2929 2c20 2762  f.userName)), 'b
+000033d0: 6c61 636b 272c 2066 6f6e 7431 290a 2020  lack', font1).  
+000033e0: 2020 2020 2020 6e61 6d65 4478 496d 6720        nameDxImg 
+000033f0: 3d20 496d 6167 652e 6f70 656e 2873 656c  = Image.open(sel
+00003400: 662e 7069 635f 6469 7220 2b20 2755 495f  f.pic_dir + 'UI_
+00003410: 434d 4e5f 4e61 6d65 5f44 582e 706e 6727  CMN_Name_DX.png'
+00003420: 292e 636f 6e76 6572 7428 2752 4742 4127  ).convert('RGBA'
+00003430: 290a 2020 2020 2020 2020 6e61 6d65 4478  ).        nameDx
+00003440: 496d 6720 3d20 7365 6c66 2e5f 7265 7369  Img = self._resi
+00003450: 7a65 5069 6328 6e61 6d65 4478 496d 672c  zePic(nameDxImg,
+00003460: 2030 2e39 290a 2020 2020 2020 2020 6e61   0.9).        na
+00003470: 6d65 506c 6174 6549 6d67 2e70 6173 7465  mePlateImg.paste
+00003480: 286e 616d 6544 7849 6d67 2c20 2832 3330  (nameDxImg, (230
+00003490: 2c20 3429 2c20 6d61 736b 3d6e 616d 6544  , 4), mask=nameD
+000034a0: 7849 6d67 2e73 706c 6974 2829 5b33 5d29  xImg.split()[3])
+000034b0: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
+000034c0: 672e 7061 7374 6528 6e61 6d65 506c 6174  g.paste(namePlat
+000034d0: 6549 6d67 2c20 2832 3430 2c20 3430 292c  eImg, (240, 40),
+000034e0: 206d 6173 6b3d 6e61 6d65 506c 6174 6549   mask=namePlateI
+000034f0: 6d67 2e73 706c 6974 2829 5b33 5d29 0a0a  mg.split()[3])..
+00003500: 2020 2020 2020 2020 7368 6f75 676f 7549          shougouI
+00003510: 6d67 203d 2049 6d61 6765 2e6f 7065 6e28  mg = Image.open(
+00003520: 7365 6c66 2e70 6963 5f64 6972 202b 2027  self.pic_dir + '
+00003530: 5549 5f43 4d4e 5f53 686f 7567 6f75 5f52  UI_CMN_Shougou_R
+00003540: 6169 6e62 6f77 2e70 6e67 2729 2e63 6f6e  ainbow.png').con
+00003550: 7665 7274 2827 5247 4241 2729 0a20 2020  vert('RGBA').   
+00003560: 2020 2020 2073 686f 7567 6f75 4472 6177       shougouDraw
+00003570: 203d 2049 6d61 6765 4472 6177 2e44 7261   = ImageDraw.Dra
+00003580: 7728 7368 6f75 676f 7549 6d67 290a 2020  w(shougouImg).  
+00003590: 2020 2020 2020 666f 6e74 3220 3d20 496d        font2 = Im
+000035a0: 6167 6546 6f6e 742e 7472 7565 7479 7065  ageFont.truetype
+000035b0: 2853 5441 5449 4320 2b20 272f 6164 6f62  (STATIC + '/adob
+000035c0: 655f 7369 6d68 6569 2e6f 7466 272c 2031  e_simhei.otf', 1
+000035d0: 342c 2065 6e63 6f64 696e 673d 2775 7466  4, encoding='utf
+000035e0: 2d38 2729 0a20 2020 2020 2020 2070 6c61  -8').        pla
+000035f0: 7943 6f75 6e74 496e 666f 203d 2066 27e5  yCountInfo = f'.
+00003600: ba95 e588 863a 207b 7365 6c66 2e6d 7573  .....: {self.mus
+00003610: 6963 5261 7469 6e67 7d20 2b20 e6ae b5e4  icRating} + ....
+00003620: bd8d e588 863a 207b 7365 6c66 2e72 616e  .....: {self.ran
+00003630: 6b52 6174 696e 677d 270a 2020 2020 2020  kRating}'.      
+00003640: 2020 7368 6f75 676f 7549 6d67 572c 2073    shougouImgW, s
+00003650: 686f 7567 6f75 496d 6748 203d 2073 686f  hougouImgH = sho
+00003660: 7567 6f75 496d 672e 7369 7a65 0a20 2020  ugouImg.size.   
+00003670: 2020 2020 2070 6c61 7943 6f75 6e74 496e       playCountIn
+00003680: 666f 572c 2070 6c61 7943 6f75 6e74 496e  foW, playCountIn
+00003690: 666f 4820 3d20 7368 6f75 676f 7544 7261  foH = shougouDra
+000036a0: 772e 7465 7874 7369 7a65 2870 6c61 7943  w.textsize(playC
+000036b0: 6f75 6e74 496e 666f 2c20 666f 6e74 3229  ountInfo, font2)
+000036c0: 0a20 2020 2020 2020 2074 6578 7450 6f73  .        textPos
+000036d0: 203d 2028 2873 686f 7567 6f75 496d 6757   = ((shougouImgW
+000036e0: 202d 2070 6c61 7943 6f75 6e74 496e 666f   - playCountInfo
+000036f0: 5720 2d20 666f 6e74 322e 6765 746f 6666  W - font2.getoff
+00003700: 7365 7428 706c 6179 436f 756e 7449 6e66  set(playCountInf
+00003710: 6f29 5b30 5d29 202f 2032 2c20 3529 0a20  o)[0]) / 2, 5). 
+00003720: 2020 2020 2020 2073 686f 7567 6f75 4472         shougouDr
+00003730: 6177 2e74 6578 7428 2874 6578 7450 6f73  aw.text((textPos
+00003740: 5b30 5d20 2d20 312c 2074 6578 7450 6f73  [0] - 1, textPos
+00003750: 5b31 5d29 2c20 706c 6179 436f 756e 7449  [1]), playCountI
+00003760: 6e66 6f2c 2027 626c 6163 6b27 2c20 666f  nfo, 'black', fo
+00003770: 6e74 3229 0a20 2020 2020 2020 2073 686f  nt2).        sho
+00003780: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
+00003790: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
+000037a0: 6578 7450 6f73 5b31 5d29 2c20 706c 6179  extPos[1]), play
+000037b0: 436f 756e 7449 6e66 6f2c 2027 626c 6163  CountInfo, 'blac
+000037c0: 6b27 2c20 666f 6e74 3229 0a20 2020 2020  k', font2).     
+000037d0: 2020 2073 686f 7567 6f75 4472 6177 2e74     shougouDraw.t
+000037e0: 6578 7428 2874 6578 7450 6f73 5b30 5d2c  ext((textPos[0],
+000037f0: 2074 6578 7450 6f73 5b31 5d20 2d20 3129   textPos[1] - 1)
+00003800: 2c20 706c 6179 436f 756e 7449 6e66 6f2c  , playCountInfo,
+00003810: 2027 626c 6163 6b27 2c20 666f 6e74 3229   'black', font2)
+00003820: 0a20 2020 2020 2020 2073 686f 7567 6f75  .        shougou
+00003830: 4472 6177 2e74 6578 7428 2874 6578 7450  Draw.text((textP
+00003840: 6f73 5b30 5d2c 2074 6578 7450 6f73 5b31  os[0], textPos[1
+00003850: 5d20 2b20 3129 2c20 706c 6179 436f 756e  ] + 1), playCoun
+00003860: 7449 6e66 6f2c 2027 626c 6163 6b27 2c20  tInfo, 'black', 
+00003870: 666f 6e74 3229 0a20 2020 2020 2020 2073  font2).        s
+00003880: 686f 7567 6f75 4472 6177 2e74 6578 7428  hougouDraw.text(
+00003890: 2874 6578 7450 6f73 5b30 5d20 2d20 312c  (textPos[0] - 1,
+000038a0: 2074 6578 7450 6f73 5b31 5d20 2d20 3129   textPos[1] - 1)
+000038b0: 2c20 706c 6179 436f 756e 7449 6e66 6f2c  , playCountInfo,
+000038c0: 2027 626c 6163 6b27 2c20 666f 6e74 3229   'black', font2)
+000038d0: 0a20 2020 2020 2020 2073 686f 7567 6f75  .        shougou
+000038e0: 4472 6177 2e74 6578 7428 2874 6578 7450  Draw.text((textP
+000038f0: 6f73 5b30 5d20 2b20 312c 2074 6578 7450  os[0] + 1, textP
+00003900: 6f73 5b31 5d20 2d20 3129 2c20 706c 6179  os[1] - 1), play
+00003910: 436f 756e 7449 6e66 6f2c 2027 626c 6163  CountInfo, 'blac
+00003920: 6b27 2c20 666f 6e74 3229 0a20 2020 2020  k', font2).     
+00003930: 2020 2073 686f 7567 6f75 4472 6177 2e74     shougouDraw.t
+00003940: 6578 7428 2874 6578 7450 6f73 5b30 5d20  ext((textPos[0] 
+00003950: 2d20 312c 2074 6578 7450 6f73 5b31 5d20  - 1, textPos[1] 
+00003960: 2b20 3129 2c20 706c 6179 436f 756e 7449  + 1), playCountI
+00003970: 6e66 6f2c 2027 626c 6163 6b27 2c20 666f  nfo, 'black', fo
+00003980: 6e74 3229 0a20 2020 2020 2020 2073 686f  nt2).        sho
+00003990: 7567 6f75 4472 6177 2e74 6578 7428 2874  ugouDraw.text((t
+000039a0: 6578 7450 6f73 5b30 5d20 2b20 312c 2074  extPos[0] + 1, t
+000039b0: 6578 7450 6f73 5b31 5d20 2b20 3129 2c20  extPos[1] + 1), 
+000039c0: 706c 6179 436f 756e 7449 6e66 6f2c 2027  playCountInfo, '
+000039d0: 626c 6163 6b27 2c20 666f 6e74 3229 0a20  black', font2). 
+000039e0: 2020 2020 2020 2073 686f 7567 6f75 4472         shougouDr
+000039f0: 6177 2e74 6578 7428 7465 7874 506f 732c  aw.text(textPos,
+00003a00: 2070 6c61 7943 6f75 6e74 496e 666f 2c20   playCountInfo, 
+00003a10: 2777 6869 7465 272c 2066 6f6e 7432 290a  'white', font2).
+00003a20: 2020 2020 2020 2020 7368 6f75 676f 7549          shougouI
+00003a30: 6d67 203d 2073 656c 662e 5f72 6573 697a  mg = self._resiz
+00003a40: 6550 6963 2873 686f 7567 6f75 496d 672c  ePic(shougouImg,
+00003a50: 2031 2e30 3529 0a20 2020 2020 2020 2073   1.05).        s
+00003a60: 656c 662e 696d 672e 7061 7374 6528 7368  elf.img.paste(sh
+00003a70: 6f75 676f 7549 6d67 2c20 2832 3430 2c20  ougouImg, (240, 
+00003a80: 3833 292c 206d 6173 6b3d 7368 6f75 676f  83), mask=shougo
+00003a90: 7549 6d67 2e73 706c 6974 2829 5b33 5d29  uImg.split()[3])
+00003aa0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00003ab0: 6472 6177 4265 7374 4c69 7374 2873 656c  drawBestList(sel
+00003ac0: 662e 696d 672c 2073 656c 662e 7364 4265  f.img, self.sdBe
+00003ad0: 7374 2c20 7365 6c66 2e64 7842 6573 7429  st, self.dxBest)
+00003ae0: 0a0a 2020 2020 2020 2020 6175 7468 6f72  ..        author
+00003af0: 426f 6172 6449 6d67 203d 2049 6d61 6765  BoardImg = Image
+00003b00: 2e6f 7065 6e28 7365 6c66 2e70 6963 5f64  .open(self.pic_d
+00003b10: 6972 202b 2027 5549 5f43 4d4e 5f4d 696e  ir + 'UI_CMN_Min
+00003b20: 6944 6961 6c6f 675f 3031 2e70 6e67 2729  iDialog_01.png')
+00003b30: 2e63 6f6e 7665 7274 2827 5247 4241 2729  .convert('RGBA')
+00003b40: 0a20 2020 2020 2020 2061 7574 686f 7242  .        authorB
+00003b50: 6f61 7264 496d 6720 3d20 7365 6c66 2e5f  oardImg = self._
+00003b60: 7265 7369 7a65 5069 6328 6175 7468 6f72  resizePic(author
+00003b70: 426f 6172 6449 6d67 2c20 302e 3335 290a  BoardImg, 0.35).
+00003b80: 2020 2020 2020 2020 6175 7468 6f72 426f          authorBo
+00003b90: 6172 6444 7261 7720 3d20 496d 6167 6544  ardDraw = ImageD
+00003ba0: 7261 772e 4472 6177 2861 7574 686f 7242  raw.Draw(authorB
+00003bb0: 6f61 7264 496d 6729 0a20 2020 2020 2020  oardImg).       
+00003bc0: 2061 7574 686f 7242 6f61 7264 4472 6177   authorBoardDraw
+00003bd0: 2e74 6578 7428 2833 312c 2032 3829 2c20  .text((31, 28), 
+00003be0: 2720 2020 4765 6e65 7261 7465 6420 4279  '   Generated By
+00003bf0: 5c6e 5879 6242 6f74 2026 2043 6869 7975  \nXybBot & Chiyu
+00003c00: 6b69 272c 2027 626c 6163 6b27 2c20 666f  ki', 'black', fo
+00003c10: 6e74 3229 0a20 2020 2020 2020 2073 656c  nt2).        sel
+00003c20: 662e 696d 672e 7061 7374 6528 6175 7468  f.img.paste(auth
+00003c30: 6f72 426f 6172 6449 6d67 2c20 2831 3232  orBoardImg, (122
+00003c40: 342c 2031 3929 2c20 6d61 736b 3d61 7574  4, 19), mask=aut
+00003c50: 686f 7242 6f61 7264 496d 672e 7370 6c69  horBoardImg.spli
+00003c60: 7428 295b 335d 290a 0a20 2020 2020 2020  t()[3])..       
+00003c70: 2064 7849 6d67 203d 2049 6d61 6765 2e6f   dxImg = Image.o
+00003c80: 7065 6e28 7365 6c66 2e70 6963 5f64 6972  pen(self.pic_dir
+00003c90: 202b 2027 5549 5f52 534c 5f4d 4261 7365   + 'UI_RSL_MBase
+00003ca0: 5f50 6172 7473 5f30 312e 706e 6727 292e  _Parts_01.png').
+00003cb0: 636f 6e76 6572 7428 2752 4742 4127 290a  convert('RGBA').
+00003cc0: 2020 2020 2020 2020 7365 6c66 2e69 6d67          self.img
+00003cd0: 2e70 6173 7465 2864 7849 6d67 2c20 2838  .paste(dxImg, (8
+00003ce0: 3930 2c20 3635 292c 206d 6173 6b3d 6478  90, 65), mask=dx
+00003cf0: 496d 672e 7370 6c69 7428 295b 335d 290a  Img.split()[3]).
+00003d00: 2020 2020 2020 2020 7364 496d 6720 3d20          sdImg = 
+00003d10: 496d 6167 652e 6f70 656e 2873 656c 662e  Image.open(self.
+00003d20: 7069 635f 6469 7220 2b20 2755 495f 5253  pic_dir + 'UI_RS
+00003d30: 4c5f 4d42 6173 655f 5061 7274 735f 3032  L_MBase_Parts_02
+00003d40: 2e70 6e67 2729 2e63 6f6e 7665 7274 2827  .png').convert('
+00003d50: 5247 4241 2729 0a20 2020 2020 2020 2073  RGBA').        s
+00003d60: 656c 662e 696d 672e 7061 7374 6528 7364  elf.img.paste(sd
+00003d70: 496d 672c 2028 3735 382c 2036 3529 2c20  Img, (758, 65), 
+00003d80: 6d61 736b 3d73 6449 6d67 2e73 706c 6974  mask=sdImg.split
+00003d90: 2829 5b33 5d29 0a0a 2020 2020 2020 2020  ()[3])..        
+00003da0: 2320 7365 6c66 2e69 6d67 2e73 686f 7728  # self.img.show(
+00003db0: 290a 0a20 2020 2064 6566 2067 6574 4469  )..    def getDi
+00003dc0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00003dd0: 2072 6574 7572 6e20 7365 6c66 2e69 6d67   return self.img
+00003de0: 0a0a 0a64 6566 2063 6f6d 7075 7465 5261  ...def computeRa
+00003df0: 2864 733a 2066 6c6f 6174 2c20 6163 6869  (ds: float, achi
+00003e00: 6576 656d 656e 743a 666c 6f61 7429 202d  evement:float) -
+00003e10: 3e20 696e 743a 0a20 2020 2062 6173 6552  > int:.    baseR
+00003e20: 6120 3d20 3135 2e30 0a20 2020 2069 6620  a = 15.0.    if 
+00003e30: 6163 6869 6576 656d 656e 7420 3e3d 2035  achievement >= 5
+00003e40: 3020 616e 6420 6163 6869 6576 656d 656e  0 and achievemen
+00003e50: 7420 3c20 3630 3a0a 2020 2020 2020 2020  t < 60:.        
+00003e60: 6261 7365 5261 203d 2035 2e30 0a20 2020  baseRa = 5.0.   
+00003e70: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003e80: 7420 3c20 3730 3a0a 2020 2020 2020 2020  t < 70:.        
+00003e90: 6261 7365 5261 203d 2036 2e30 0a20 2020  baseRa = 6.0.   
+00003ea0: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003eb0: 7420 3c20 3735 3a0a 2020 2020 2020 2020  t < 75:.        
+00003ec0: 6261 7365 5261 203d 2037 2e30 0a20 2020  baseRa = 7.0.   
+00003ed0: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003ee0: 7420 3c20 3830 3a0a 2020 2020 2020 2020  t < 80:.        
+00003ef0: 6261 7365 5261 203d 2037 2e35 0a20 2020  baseRa = 7.5.   
+00003f00: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003f10: 7420 3c20 3930 3a0a 2020 2020 2020 2020  t < 90:.        
+00003f20: 6261 7365 5261 203d 2038 2e30 0a20 2020  baseRa = 8.0.   
+00003f30: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003f40: 7420 3c20 3934 3a0a 2020 2020 2020 2020  t < 94:.        
+00003f50: 6261 7365 5261 203d 2039 2e30 0a20 2020  baseRa = 9.0.   
+00003f60: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003f70: 7420 3c20 3937 3a0a 2020 2020 2020 2020  t < 97:.        
+00003f80: 6261 7365 5261 203d 2039 2e34 0a20 2020  baseRa = 9.4.   
+00003f90: 2065 6c69 6620 6163 6869 6576 656d 656e   elif achievemen
+00003fa0: 7420 3c20 3938 3a0a 2020 2020 2020 2020  t < 98:.        
+00003fb0: 6261 7365 5261 203d 2031 302e 300a 2020  baseRa = 10.0.  
+00003fc0: 2020 656c 6966 2061 6368 6965 7665 6d65    elif achieveme
+00003fd0: 6e74 203c 2039 393a 0a20 2020 2020 2020  nt < 99:.       
+00003fe0: 2062 6173 6552 6120 3d20 3131 2e30 0a20   baseRa = 11.0. 
+00003ff0: 2020 2065 6c69 6620 6163 6869 6576 656d     elif achievem
+00004000: 656e 7420 3c20 3939 2e35 3a0a 2020 2020  ent < 99.5:.    
+00004010: 2020 2020 6261 7365 5261 203d 2031 322e      baseRa = 12.
+00004020: 300a 2020 2020 656c 6966 2061 6368 6965  0.    elif achie
+00004030: 7665 6d65 6e74 203c 2039 392e 3939 3a0a  vement < 99.99:.
+00004040: 2020 2020 2020 2020 6261 7365 5261 203d          baseRa =
+00004050: 2031 332e 300a 2020 2020 656c 6966 2061   13.0.    elif a
+00004060: 6368 6965 7665 6d65 6e74 203c 2031 3030  chievement < 100
+00004070: 3a0a 2020 2020 2020 2020 6261 7365 5261  :.        baseRa
+00004080: 203d 2031 332e 350a 2020 2020 656c 6966   = 13.5.    elif
+00004090: 2061 6368 6965 7665 6d65 6e74 203c 2031   achievement < 1
+000040a0: 3030 2e35 3a0a 2020 2020 2020 2020 6261  00.5:.        ba
+000040b0: 7365 5261 203d 2031 342e 300a 0a20 2020  seRa = 14.0..   
+000040c0: 2072 6574 7572 6e20 6d61 7468 2e66 6c6f   return math.flo
+000040d0: 6f72 2864 7320 2a20 286d 696e 2831 3030  or(ds * (min(100
+000040e0: 2e35 2c20 6163 6869 6576 656d 656e 7429  .5, achievement)
+000040f0: 202f 2031 3030 2920 2a20 6261 7365 5261   / 100) * baseRa
+00004100: 290a 0a0a 6173 796e 6320 6465 6620 6765  )...async def ge
+00004110: 6e65 7261 7465 2870 6179 6c6f 6164 3a20  nerate(payload: 
+00004120: 4469 6374 2920 2d3e 2054 7570 6c65 5b4f  Dict) -> Tuple[O
+00004130: 7074 696f 6e61 6c5b 496d 6167 652e 496d  ptional[Image.Im
+00004140: 6167 655d 2c20 626f 6f6c 5d3a 0a20 2020  age], bool]:.   
+00004150: 2061 7379 6e63 2077 6974 6820 6169 6f68   async with aioh
+00004160: 7474 702e 7265 7175 6573 7428 2250 4f53  ttp.request("POS
+00004170: 5422 2c20 2268 7474 7073 3a2f 2f77 7777  T", "https://www
+00004180: 2e64 6976 696e 672d 6669 7368 2e63 6f6d  .diving-fish.com
+00004190: 2f61 7069 2f6d 6169 6d61 6964 7870 726f  /api/maimaidxpro
+000041a0: 6265 722f 7175 6572 792f 706c 6179 6572  ber/query/player
+000041b0: 222c 206a 736f 6e3d 7061 796c 6f61 6429  ", json=payload)
+000041c0: 2061 7320 7265 7370 3a0a 2020 2020 2020   as resp:.      
+000041d0: 2020 6966 2072 6573 702e 7374 6174 7573    if resp.status
+000041e0: 203d 3d20 3430 303a 0a20 2020 2020 2020   == 400:.       
+000041f0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00004200: 2c20 3430 300a 2020 2020 2020 2020 6966  , 400.        if
+00004210: 2072 6573 702e 7374 6174 7573 203d 3d20   resp.status == 
+00004220: 3430 333a 0a20 2020 2020 2020 2020 2020  403:.           
+00004230: 2072 6574 7572 6e20 4e6f 6e65 2c20 3430   return None, 40
+00004240: 330a 2020 2020 2020 2020 7364 5f62 6573  3.        sd_bes
+00004250: 7420 3d20 4265 7374 4c69 7374 2832 3529  t = BestList(25)
+00004260: 0a20 2020 2020 2020 2064 785f 6265 7374  .        dx_best
+00004270: 203d 2042 6573 744c 6973 7428 3135 290a   = BestList(15).
+00004280: 2020 2020 2020 2020 6f62 6a20 3d20 6177          obj = aw
+00004290: 6169 7420 7265 7370 2e6a 736f 6e28 290a  ait resp.json().
+000042a0: 2020 2020 2020 2020 6478 3a20 4c69 7374          dx: List
+000042b0: 5b44 6963 745d 203d 206f 626a 5b22 6368  [Dict] = obj["ch
+000042c0: 6172 7473 225d 5b22 6478 225d 0a20 2020  arts"]["dx"].   
+000042d0: 2020 2020 2073 643a 204c 6973 745b 4469       sd: List[Di
+000042e0: 6374 5d20 3d20 6f62 6a5b 2263 6861 7274  ct] = obj["chart
+000042f0: 7322 5d5b 2273 6422 5d0a 2020 2020 2020  s"]["sd"].      
+00004300: 2020 666f 7220 6320 696e 2073 643a 0a20    for c in sd:. 
+00004310: 2020 2020 2020 2020 2020 2073 645f 6265             sd_be
+00004320: 7374 2e70 7573 6828 4368 6172 7449 6e66  st.push(ChartInf
+00004330: 6f2e 6672 6f6d 5f6a 736f 6e28 6329 290a  o.from_json(c)).
+00004340: 2020 2020 2020 2020 666f 7220 6320 696e          for c in
+00004350: 2064 783a 0a20 2020 2020 2020 2020 2020   dx:.           
+00004360: 2064 785f 6265 7374 2e70 7573 6828 4368   dx_best.push(Ch
+00004370: 6172 7449 6e66 6f2e 6672 6f6d 5f6a 736f  artInfo.from_jso
+00004380: 6e28 6329 290a 2020 2020 2020 2020 7069  n(c)).        pi
+00004390: 6320 3d20 4472 6177 4265 7374 2873 645f  c = DrawBest(sd_
+000043a0: 6265 7374 2c20 6478 5f62 6573 742c 206f  best, dx_best, o
+000043b0: 626a 5b22 6e69 636b 6e61 6d65 225d 2c20  bj["nickname"], 
+000043c0: 6f62 6a5b 2272 6174 696e 6722 5d20 2b20  obj["rating"] + 
+000043d0: 6f62 6a5b 2261 6464 6974 696f 6e61 6c5f  obj["additional_
+000043e0: 7261 7469 6e67 225d 2c20 6f62 6a5b 2272  rating"], obj["r
+000043f0: 6174 696e 6722 5d29 2e67 6574 4469 7228  ating"]).getDir(
+00004400: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004410: 2070 6963 2c20 300a                       pic, 0.
```

### Comparing `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-
-import random
-from typing import Dict, List, Optional, Union, Tuple, Any
-from copy import deepcopy
-
-import aiohttp,asyncio
-
-def get_cover_len5_id(mid) -> str:
-    mid = int(mid)
-    if mid > 10000 and mid <= 11000:
-        mid -= 10000
-    return f'{mid:05d}'
-
-def cross(checker: List[Any], elem: Optional[Union[Any, List[Any]]], diff):
-    ret = False
-    diff_ret = []
-    if not elem or elem is Ellipsis:
-        return True, diff
-    if isinstance(elem, List):
-        for _j in (range(len(checker)) if diff is Ellipsis else diff):
-            if _j >= len(checker):
-                continue
-            __e = checker[_j]
-            if __e in elem:
-                diff_ret.append(_j)
-                ret = True
-    elif isinstance(elem, Tuple):
-        for _j in (range(len(checker)) if diff is Ellipsis else diff):
-            if _j >= len(checker):
-                continue
-            __e = checker[_j]
-            if elem[0] <= __e <= elem[1]:
-                diff_ret.append(_j)
-                ret = True
-    else:
-        for _j in (range(len(checker)) if diff is Ellipsis else diff):
-            if _j >= len(checker):
-                continue
-            __e = checker[_j]
-            if elem == __e:
-                return True, [_j]
-    return ret, diff_ret
-
-
-def in_or_equal(checker: Any, elem: Optional[Union[Any, List[Any]]]):
-    if elem is Ellipsis:
-        return True
-    if isinstance(elem, List):
-        return checker in elem
-    elif isinstance(elem, Tuple):
-        return elem[0] <= checker <= elem[1]
-    else:
-        return checker == elem
-
-
-class Chart(Dict):
-    tap: Optional[int] = None
-    slide: Optional[int] = None
-    hold: Optional[int] = None
-    touch: Optional[int] = None
-    brk: Optional[int] = None
-    charter: Optional[int] = None
-
-    def __getattribute__(self, item):
-        if item == 'tap':
-            return self['notes'][0]
-        elif item == 'hold':
-            return self['notes'][1]
-        elif item == 'slide':
-            return self['notes'][2]
-        elif item == 'touch':
-            return self['notes'][3] if len(self['notes']) == 5 else 0
-        elif item == 'brk':
-            return self['notes'][-1]
-        elif item == 'charter':
-            return self['charter']
-        return super().__getattribute__(item)
-
-
-class Music(Dict):
-    id: Optional[str] = None
-    title: Optional[str] = None
-    ds: Optional[List[float]] = None
-    level: Optional[List[str]] = None
-    genre: Optional[str] = None
-    type: Optional[str] = None
-    bpm: Optional[float] = None
-    version: Optional[str] = None
-    charts: Optional[Chart] = None
-    release_date: Optional[str] = None
-    artist: Optional[str] = None
-
-    diff: List[int] = []
-
-    def __getattribute__(self, item):
-        if item in {'genre', 'artist', 'release_date', 'bpm', 'version'}:
-            if item == 'version':
-                return self['basic_info']['from']
-            return self['basic_info'][item]
-        elif item in self:
-            return self[item]
-        return super().__getattribute__(item)
-
-
-class MusicList(List[Music]):
-    def by_id(self, music_id: str) -> Optional[Music]:
-        for music in self:
-            if music.id == music_id:
-                return music
-        return None
-
-    def by_title(self, music_title: str) -> Optional[Music]:
-        for music in self:
-            if music.title == music_title:
-                return music
-        return None
-
-    def random(self):
-        return random.choice(self)
-
-    def filter(self,
-               *,
-               level: Optional[Union[str, List[str]]] = ...,
-               ds: Optional[Union[float, List[float], Tuple[float, float]]] = ...,
-               title_search: Optional[str] = ...,
-               genre: Optional[Union[str, List[str]]] = ...,
-               bpm: Optional[Union[float, List[float], Tuple[float, float]]] = ...,
-               type: Optional[Union[str, List[str]]] = ...,
-               diff: List[int] = ...,
-               ):
-        new_list = MusicList()
-        for music in self:
-            diff2 = diff
-            music = deepcopy(music)
-            ret, diff2 = cross(music.level, level, diff2)
-            if not ret:
-                continue
-            ret, diff2 = cross(music.ds, ds, diff2)
-            if not ret:
-                continue
-            if not in_or_equal(music.genre, genre):
-                continue
-            if not in_or_equal(music.type, type):
-                continue
-            if not in_or_equal(music.bpm, bpm):
-                continue
-            if title_search is not Ellipsis and title_search.lower() not in music.title.lower():
-                continue
-            music.diff = diff2
-            new_list.append(music)
-        return new_list
-
-
-async def main():
-    global obj,total_list
-    async def fetch_json(url):
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                return await response.json()
-
-    obj = await fetch_json('https://www.diving-fish.com/api/maimaidxprober/music_data')
-    total_list = MusicList(obj)
-    for __i in range(len(total_list)):
-        total_list[__i] = Music(total_list[__i])
-        for __j in range(len(total_list[__i].charts)):
-            total_list[__i].charts[__j] = Chart(total_list[__i].charts[__j])
-    
-asyncio.run(main())
-
+
+import random
+from typing import Dict, List, Optional, Union, Tuple, Any
+from copy import deepcopy
+
+import aiohttp,asyncio
+
+def get_cover_len5_id(mid) -> str:
+    mid = int(mid)
+    if mid > 10000 and mid <= 11000:
+        mid -= 10000
+    return f'{mid:05d}'
+
+def cross(checker: List[Any], elem: Optional[Union[Any, List[Any]]], diff):
+    ret = False
+    diff_ret = []
+    if not elem or elem is Ellipsis:
+        return True, diff
+    if isinstance(elem, List):
+        for _j in (range(len(checker)) if diff is Ellipsis else diff):
+            if _j >= len(checker):
+                continue
+            __e = checker[_j]
+            if __e in elem:
+                diff_ret.append(_j)
+                ret = True
+    elif isinstance(elem, Tuple):
+        for _j in (range(len(checker)) if diff is Ellipsis else diff):
+            if _j >= len(checker):
+                continue
+            __e = checker[_j]
+            if elem[0] <= __e <= elem[1]:
+                diff_ret.append(_j)
+                ret = True
+    else:
+        for _j in (range(len(checker)) if diff is Ellipsis else diff):
+            if _j >= len(checker):
+                continue
+            __e = checker[_j]
+            if elem == __e:
+                return True, [_j]
+    return ret, diff_ret
+
+
+def in_or_equal(checker: Any, elem: Optional[Union[Any, List[Any]]]):
+    if elem is Ellipsis:
+        return True
+    if isinstance(elem, List):
+        return checker in elem
+    elif isinstance(elem, Tuple):
+        return elem[0] <= checker <= elem[1]
+    else:
+        return checker == elem
+
+
+class Chart(Dict):
+    tap: Optional[int] = None
+    slide: Optional[int] = None
+    hold: Optional[int] = None
+    touch: Optional[int] = None
+    brk: Optional[int] = None
+    charter: Optional[int] = None
+
+    def __getattribute__(self, item):
+        if item == 'tap':
+            return self['notes'][0]
+        elif item == 'hold':
+            return self['notes'][1]
+        elif item == 'slide':
+            return self['notes'][2]
+        elif item == 'touch':
+            return self['notes'][3] if len(self['notes']) == 5 else 0
+        elif item == 'brk':
+            return self['notes'][-1]
+        elif item == 'charter':
+            return self['charter']
+        return super().__getattribute__(item)
+
+
+class Music(Dict):
+    id: Optional[str] = None
+    title: Optional[str] = None
+    ds: Optional[List[float]] = None
+    level: Optional[List[str]] = None
+    genre: Optional[str] = None
+    type: Optional[str] = None
+    bpm: Optional[float] = None
+    version: Optional[str] = None
+    charts: Optional[Chart] = None
+    release_date: Optional[str] = None
+    artist: Optional[str] = None
+
+    diff: List[int] = []
+
+    def __getattribute__(self, item):
+        if item in {'genre', 'artist', 'release_date', 'bpm', 'version'}:
+            if item == 'version':
+                return self['basic_info']['from']
+            return self['basic_info'][item]
+        elif item in self:
+            return self[item]
+        return super().__getattribute__(item)
+
+
+class MusicList(List[Music]):
+    def by_id(self, music_id: str) -> Optional[Music]:
+        for music in self:
+            if music.id == music_id:
+                return music
+        return None
+
+    def by_title(self, music_title: str) -> Optional[Music]:
+        for music in self:
+            if music.title == music_title:
+                return music
+        return None
+
+    def random(self):
+        return random.choice(self)
+
+    def filter(self,
+               *,
+               level: Optional[Union[str, List[str]]] = ...,
+               ds: Optional[Union[float, List[float], Tuple[float, float]]] = ...,
+               title_search: Optional[str] = ...,
+               genre: Optional[Union[str, List[str]]] = ...,
+               bpm: Optional[Union[float, List[float], Tuple[float, float]]] = ...,
+               type: Optional[Union[str, List[str]]] = ...,
+               diff: List[int] = ...,
+               ):
+        new_list = MusicList()
+        for music in self:
+            diff2 = diff
+            music = deepcopy(music)
+            ret, diff2 = cross(music.level, level, diff2)
+            if not ret:
+                continue
+            ret, diff2 = cross(music.ds, ds, diff2)
+            if not ret:
+                continue
+            if not in_or_equal(music.genre, genre):
+                continue
+            if not in_or_equal(music.type, type):
+                continue
+            if not in_or_equal(music.bpm, bpm):
+                continue
+            if title_search is not Ellipsis and title_search.lower() not in music.title.lower():
+                continue
+            music.diff = diff2
+            new_list.append(music)
+        return new_list
+
+
+async def main():
+    global obj,total_list
+    async def fetch_json(url):
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                return await response.json()
+
+    obj = await fetch_json('https://www.diving-fish.com/api/maimaidxprober/music_data')
+    total_list = MusicList(obj)
+    for __i in range(len(total_list)):
+        total_list[__i] = Music(total_list[__i])
+        for __j in range(len(total_list[__i].charts)):
+            total_list[__i].charts[__j] = Chart(total_list[__i].charts[__j])
+    
+asyncio.run(main())
+
```

### Comparing `nonebot_plugin_maimai-0.2.0/nonebot_plugin_maimai/public.py` & `nonebot_plugin_maimai-0.2.1/nonebot_plugin_maimai/public.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from nonebot import on_command, on_notice
-from nonebot.typing import T_State
-from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageSegment
-from nonebot.exception import IgnoredException
-from nonebot.message import event_preprocessor
-from nonebot_plugin_txt2img import Txt2Img
-from nonebot import get_driver
-from nonebot.params import CommandArg
-from nonebot.matcher import Matcher
-from .libraries.image import *
-
-from bs4 import BeautifulSoup
-from typing import Dict,List
-import aiohttp
-from io import BytesIO
-import json
-
-try:
-    maimai_font: str = get_driver().config.maimai_font
-except:
-    maimai_font: str = 'simsun.ttc'
-try:
-    b_cookie: str = get_driver().config.b_cookie
-except:
-    b_cookie: str = ''
-
-@event_preprocessor
-async def preprocessor(bot, event, state):
-    if hasattr(event, 'message_type') and event.message_type == "private" and event.sub_type != "friend":
-        raise IgnoredException("not reply group temp message")
-
-        
-help = on_command('help',aliases={'舞萌帮助','mai帮助'})
-
-
-@help.handle()
-async def _():
-    help_str = '''可用命令如下：
-今日舞萌 查看今天的舞萌运势
-XXXmaimaiXXX什么 随机一首歌
-随个[dx/标准][绿黄红紫白]<难度> 随机一首指定条件的乐曲
-查歌<乐曲标题的一部分> 查询符合条件的乐曲
-[绿黄红紫白]id<歌曲编号> 查询乐曲信息或谱面信息
-<歌曲别名>是什么歌 查询乐曲别名对应的乐曲
-定数查歌 <定数>  查询定数对应的乐曲
-定数查歌 <定数下限> <定数上限>
-分数线 <难度+歌曲id> <分数线> 详情请输入“分数线 帮助”查看'''
-    # await help.send(Message([
-    #     MessageSegment("image", {
-    #         "file": f"base64://{str(image_to_base64(text_to_image(help_str)), encoding='utf-8')}"
-    #     })
-    # ]))
-    title = '可用命令如下：'
-    txt2img = Txt2Img()
-    txt2img.set_font_size(font_size = 32)
-    pic = txt2img.draw(title, help_str)
-    try:
-        await help.send(MessageSegment.image(pic))
-    except:
-        await help.send(help_str)
-
-
-
-search = on_command('search',aliases={'b站搜索','mai搜索'})
-@search.handle()
-async def _(state: T_State,matcher:Matcher ,arg:Message = CommandArg()):
-    msg = arg.extract_plain_text()
-    data_list:List[Dict[str,Dict[str,str]]] = await get_target(msg)
-    state['msg'] = data_list
-    result_img = await data_to_img(data_list)
-    img = BytesIO()
-    result_img.save(img,format="png")
-    img_bytes = img.getvalue()
-    await matcher.send(MessageSegment.image(img_bytes))
-
-@search.got("tap",prompt="请输入需要的序号")
-async def _(state: T_State,matcher:Matcher ):
-    tag:Message = state['tap']
-    tag = tag.extract_plain_text()
-    if tag.isdigit() and int(tag) in range(1, 10):
-        msg:List[Dict[str,Dict[str,str]]] = state['msg']
-        Url = msg[int(tag)-1]['url']['视频链接:']
-        print(msg[int(tag)-1])
-        await matcher.finish(Url)
-    
-async def fetch_page(url, headers):
-    async with aiohttp.ClientSession(headers=headers) as session:
-        async with session.get(url) as response:
-            return await response.text()    
-    
-async def get_target(keyword:str):
-    headers = {
-    'User-Agent':
-        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
-    'cookie': b_cookie
-    }
-
-    mainUrl='https://search.bilibili.com/all?keyword='+keyword
-    content = await fetch_page(mainUrl, headers)
-    mainSoup = BeautifulSoup(content, "html.parser")
-    viedoNum = 1
-    msg_list = []
-    for item in mainSoup.find_all('div',class_="bili-video-card"):
-        item:BeautifulSoup
-        msg = {'data':{},'url':{}}
-        # try:
-        msg['data']['序号:'] = '第'+ viedoNum.__str__() + '个视频:'
-        val=item.find('div',class_="bili-video-card__info--right")
-        msg['data']['视频标题:'] =  val.find('h3',class_="bili-video-card__info--tit")['title']
-        msg['url']['视频链接:'] = 'https:'+ val.find('a')['href'] + '\n'
-        try:
-            msg['data']['up主:'] = item.find('span',class_="bili-video-card__info--author").text.strip()
-            msg['data']['视频观看量:'] = item.select('span.bili-video-card__stats--item span')[0].text.strip()
-        except (AttributeError,IndexError):
-            continue
-        
-        msg['data']['弹幕量:'] =  item.select('span.bili-video-card__stats--item span')[1].text.strip()
-        msg['data']['上传时间:'] = item.find('span',class_='bili-video-card__info--date').text.strip()
-        msg['data']['视频时长:'] = item.find('span',class_='bili-video-card__stats__duration').text.strip()
-        msg['url']['封面:'] = 'https:'+ item.find('img').get('src')
-        # except:
-        #     continue
-        print(json.dumps(msg,indent=4,ensure_ascii=False) )
-        msg_list.append(msg)
-        if viedoNum == 9:
-            break
-        viedoNum += 1
-    return msg_list
-
-
-async def make_dict_img(data: Dict[str, str], cell_width: int, cell_height: int, font_size: int) -> Image:
-    img = Image.new('RGBA', (cell_width, cell_height), color=(255, 255, 255, 255))
-    draw = ImageDraw.Draw(img)
-    font = ImageFont.truetype(maimai_font, font_size)
-
-    i = 0
-    for k, v in data.items():
-        lentext = f"{k}{v}"
-        while len(lentext) > 0:
-            draw.text((10, i * (font_size + 5)), lentext[:25], font=font, fill=(0, 0, 0, 255))
-            lentext = lentext[25:]
-            i += 1
-
-    return img
-
-
-async def data_to_img(msg_list: List[Dict[str, Dict[str, str]]], cell_width=1080//3, cell_height=1920//3, font_size=20) -> Image:
-    cols = 3
-    rows = 3
-
-    # 创建一张1080*1920的空白图
-    result_img = Image.new('RGBA', (cell_width * cols, cell_height * rows), color=(255, 255, 255, 255))
-
-    # 将每个dict对象转换成包含两个dict对象的列表
-    data_list = []
-    for msg in msg_list:
-        data = msg['data']
-        url = msg['url']
-        data_list.append((url, data))
-
-    for i, (url, data) in enumerate(data_list):
-        # 将图片缩放并插入到格子中
-        image_content = await fetch_page(url['封面:'], headers={
-            'User-Agent':
-                'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
-        })
-        image = Image.open(BytesIO(image_content))
-        img_width, img_height = image.size
-        ratio = min(cell_width/img_width, cell_height/img_height)
-        new_width = int(img_width*ratio)
-        new_height = int(img_height*ratio)
-        image = image.resize((new_width, new_height), Image.ANTIALIAS)
-        img_x = ((i % cols) * cell_width) + ((cell_width - new_width) // 2)
-        img_y = ((i // cols) * cell_height) + ((cell_height - new_height-200) // 2)
-        result_img.paste(image, (img_x, img_y))
- 
-
-        # 添加文字信息到下方
-        dict_img = await make_dict_img(data, cell_width, cell_height, font_size)
-        dict_x = ((i % cols) * cell_width) + ((cell_width - dict_img.size[0]) // 2)
-        dict_y = ((i // cols) * cell_height) + new_height + ((cell_height - new_height - font_size - dict_img.size[1]) // 2) + new_height*1
-        result_img.paste(dict_img, (dict_x, dict_y))
-
-    return result_img
-
+from nonebot import on_command, on_notice
+from nonebot.typing import T_State
+from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageSegment
+from nonebot.exception import IgnoredException
+from nonebot.message import event_preprocessor
+from nonebot_plugin_txt2img import Txt2Img
+from nonebot import get_driver
+from nonebot.params import CommandArg
+from nonebot.matcher import Matcher
+from .libraries.image import *
+
+from bs4 import BeautifulSoup
+from typing import Dict,List
+import aiohttp
+from io import BytesIO
+import json
+
+try:
+    maimai_font: str = get_driver().config.maimai_font
+except:
+    maimai_font: str = 'simsun.ttc'
+try:
+    b_cookie: str = get_driver().config.b_cookie
+except:
+    b_cookie: str = ''
+
+@event_preprocessor
+async def preprocessor(bot, event, state):
+    if hasattr(event, 'message_type') and event.message_type == "private" and event.sub_type != "friend":
+        raise IgnoredException("not reply group temp message")
+
+        
+help = on_command('help',aliases={'舞萌帮助','mai帮助'})
+
+
+@help.handle()
+async def _():
+    help_str = '''可用命令如下：
+今日舞萌 查看今天的舞萌运势
+XXXmaimaiXXX什么 随机一首歌
+随个[dx/标准][绿黄红紫白]<难度> 随机一首指定条件的乐曲
+查歌<乐曲标题的一部分> 查询符合条件的乐曲
+[绿黄红紫白]id<歌曲编号> 查询乐曲信息或谱面信息
+<歌曲别名>是什么歌 查询乐曲别名对应的乐曲
+定数查歌 <定数>  查询定数对应的乐曲
+定数查歌 <定数下限> <定数上限>
+分数线 <难度+歌曲id> <分数线> 详情请输入“分数线 帮助”查看'''
+    # await help.send(Message([
+    #     MessageSegment("image", {
+    #         "file": f"base64://{str(image_to_base64(text_to_image(help_str)), encoding='utf-8')}"
+    #     })
+    # ]))
+    title = '可用命令如下：'
+    txt2img = Txt2Img()
+    txt2img.set_font_size(font_size = 32)
+    pic = txt2img.draw(title, help_str)
+    try:
+        await help.send(MessageSegment.image(pic))
+    except:
+        await help.send(help_str)
+
+
+
+search = on_command('search',aliases={'b站搜索','mai搜索'})
+@search.handle()
+async def _(state: T_State,matcher:Matcher ,arg:Message = CommandArg()):
+    msg = arg.extract_plain_text()
+    data_list:List[Dict[str,Dict[str,str]]] = await get_target(msg)
+    state['msg'] = data_list
+    result_img = await data_to_img(data_list)
+    img = BytesIO()
+    result_img.save(img,format="png")
+    img_bytes = img.getvalue()
+    await matcher.send(MessageSegment.image(img_bytes))
+
+@search.got("tap",prompt="请输入需要的序号")
+async def _(state: T_State,matcher:Matcher ):
+    tag:Message = state['tap']
+    tag = tag.extract_plain_text()
+    if tag.isdigit() and int(tag) in range(1, 10):
+        msg:List[Dict[str,Dict[str,str]]] = state['msg']
+        Url = msg[int(tag)-1]['url']['视频链接:']
+        print(msg[int(tag)-1])
+        await matcher.finish(Url)
+    
+async def fetch_page(url, headers):
+    async with aiohttp.ClientSession(headers=headers) as session:
+        async with session.get(url) as response:
+            return await response.text()    
+    
+async def get_target(keyword:str):
+    headers = {
+    'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
+    'cookie': b_cookie
+    }
+
+    mainUrl='https://search.bilibili.com/all?keyword='+keyword
+    content = await fetch_page(mainUrl, headers)
+    mainSoup = BeautifulSoup(content, "html.parser")
+    viedoNum = 1
+    msg_list = []
+    for item in mainSoup.find_all('div',class_="bili-video-card"):
+        item:BeautifulSoup
+        msg = {'data':{},'url':{}}
+        # try:
+        msg['data']['序号:'] = '第'+ viedoNum.__str__() + '个视频:'
+        val=item.find('div',class_="bili-video-card__info--right")
+        msg['data']['视频标题:'] =  val.find('h3',class_="bili-video-card__info--tit")['title']
+        msg['url']['视频链接:'] = 'https:'+ val.find('a')['href'] + '\n'
+        try:
+            msg['data']['up主:'] = item.find('span',class_="bili-video-card__info--author").text.strip()
+            msg['data']['视频观看量:'] = item.select('span.bili-video-card__stats--item span')[0].text.strip()
+        except (AttributeError,IndexError):
+            continue
+        
+        msg['data']['弹幕量:'] =  item.select('span.bili-video-card__stats--item span')[1].text.strip()
+        msg['data']['上传时间:'] = item.find('span',class_='bili-video-card__info--date').text.strip()
+        msg['data']['视频时长:'] = item.find('span',class_='bili-video-card__stats__duration').text.strip()
+        msg['url']['封面:'] = 'https:'+ item.find('img').get('src')
+        # except:
+        #     continue
+        print(json.dumps(msg,indent=4,ensure_ascii=False) )
+        msg_list.append(msg)
+        if viedoNum == 9:
+            break
+        viedoNum += 1
+    return msg_list
+
+
+async def make_dict_img(data: Dict[str, str], cell_width: int, cell_height: int, font_size: int) -> Image:
+    img = Image.new('RGBA', (cell_width, cell_height), color=(255, 255, 255, 255))
+    draw = ImageDraw.Draw(img)
+    font = ImageFont.truetype(maimai_font, font_size)
+
+    i = 0
+    for k, v in data.items():
+        lentext = f"{k}{v}"
+        while len(lentext) > 0:
+            draw.text((10, i * (font_size + 5)), lentext[:25], font=font, fill=(0, 0, 0, 255))
+            lentext = lentext[25:]
+            i += 1
+
+    return img
+
+
+async def data_to_img(msg_list: List[Dict[str, Dict[str, str]]], cell_width=1080//3, cell_height=1920//3, font_size=20) -> Image:
+    cols = 3
+    rows = 3
+
+    # 创建一张1080*1920的空白图
+    result_img = Image.new('RGBA', (cell_width * cols, cell_height * rows), color=(255, 255, 255, 255))
+
+    # 将每个dict对象转换成包含两个dict对象的列表
+    data_list = []
+    for msg in msg_list:
+        data = msg['data']
+        url = msg['url']
+        data_list.append((url, data))
+
+    for i, (url, data) in enumerate(data_list):
+        # 将图片缩放并插入到格子中
+        image_content = await fetch_page(url['封面:'], headers={
+            'User-Agent':
+                'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62',
+        })
+        image = Image.open(BytesIO(image_content))
+        img_width, img_height = image.size
+        ratio = min(cell_width/img_width, cell_height/img_height)
+        new_width = int(img_width*ratio)
+        new_height = int(img_height*ratio)
+        image = image.resize((new_width, new_height), Image.ANTIALIAS)
+        img_x = ((i % cols) * cell_width) + ((cell_width - new_width) // 2)
+        img_y = ((i // cols) * cell_height) + ((cell_height - new_height-200) // 2)
+        result_img.paste(image, (img_x, img_y))
+ 
+
+        # 添加文字信息到下方
+        dict_img = await make_dict_img(data, cell_width, cell_height, font_size)
+        dict_x = ((i % cols) * cell_width) + ((cell_width - dict_img.size[0]) // 2)
+        dict_y = ((i // cols) * cell_height) + new_height + ((cell_height - new_height - font_size - dict_img.size[1]) // 2) + new_height*1
+        result_img.paste(dict_img, (dict_x, dict_y))
+
+    return result_img
+
```

### Comparing `nonebot_plugin_maimai-0.2.0/pyproject.toml` & `nonebot_plugin_maimai-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-[tool.poetry]
-name = "nonebot_plugin_maimai"
-version = "0.2.0"
-description= "Maimai DX plugin for NoneBot"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
-repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai"
-keywords = ["maimai", "nonebot2", "plugin"]
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-
-]
-include = [
-    "LICENSE","README.md"
-]
- 
-[tool.poetry.dependencies]
-python = "^3.9"
-aiohttp = "^3.8.3"
-nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = ">=2.1.3"
-pillow = ">=9.3.0"
-nonebot-plugin-txt2img = "^0.3.0"
-bs4 = "^0.0.1"
- 
-[tool.poetry.dev-dependencies]
- 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
+[tool.poetry]
+name = "nonebot_plugin_maimai"
+version = "0.2.1"
+description= "Maimai DX plugin for NoneBot"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_maimai"
+repository = "https://github.com/Agnes4m/nonebot_plugin_maimai"
+keywords = ["maimai", "nonebot2", "plugin"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+
+]
+include = [
+    "LICENSE","README.md"
+]
+ 
+[tool.poetry.dependencies]
+python = "^3.9"
+aiohttp = "^3.8.3"
+nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = ">=2.1.3"
+pillow = ">=9.3.0"
+httpx = ">=0.22.0"
+nonebot-plugin-txt2img = "^0.3.0"
+bs4 = "^0.0.1"
+ 
+[tool.poetry.dev-dependencies]
+ 
+[build-system]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_maimai-0.2.0/README.md` & `nonebot_plugin_maimai-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-<div align="center">
-  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_maimai
-_✨maimaiDX，nonebot2插件版本✨_
-
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="stars">
-</a>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
-</div>
-
-## 说明
-
-从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
-
-修改部分：
- - b40/b50可以艾特人查询
- - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
- - env设置 `maimai_font`和`b_cookie`,分别是str对象的`字体`和`cookie`
- - 新增指令`b站搜索[text]`
-
-我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
-
-## 前置步骤（和原项目一样）
-
-安装:
-
-    pip3 install nonebot_plugin_maimai
-    nb plugin install nonebot_plugin_maimai
-    # git clone 那我建议你还是用原作者的罢
-
-您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)
-
- - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static
- - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置
-
-> 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。
-
-## FAQ
-
-配置 nonebot 或 cq-http 过程中出错？
-> 请查阅 https://github.com/nonebot/nonebot2 以及 https://github.com/Mrs4s/go-cqhttp 中的文档。
-
-部分消息发不出来？
-> 被风控了。解决方式：换号或者让这个号保持登陆状态和一定的聊天频率，持续一段时间。
-
-## 说明
-
-本 bot 提供了如下功能：
-
-命令 | 功能
---- | ---
-help | 查看帮助文档
-今日舞萌 | 查看今天的舞萌运势
-XXXmaimaiXXX什么 | 随机一首歌
-随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲
-查歌<乐曲标题的一部分> | 查询符合条件的乐曲
-[绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息
-定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲
-分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线
-
-## 原作者
-
-[Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献
-
-## License
-
-MIT
-
-您可以自由使用本项目的代码用于商业或非商业的用途，但必须附带 MIT 授权协议。
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_maimai
+_✨maimaiDX，nonebot2插件版本✨_
+
+<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="stars">
+</a>
+<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
+</div>
+
+## 说明（已更新舞萌国服2023，重新下载资源）
+
+从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
+
+修改部分：
+ - b40/b50可以艾特人查询
+ - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
+ - （可循）env设置 `maimai_font`,是str对象的`字体`
+ - 新增指令`b站搜索[text]`
+
+我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
+
+## 前置步骤（和原项目一样）
+
+安装（仍选其一）:
+
+    pip3 install nonebot_plugin_maimai
+    nb plugin install nonebot_plugin_maimai
+    git clone https://github.com/Agnes4m/nonebot_plugin_maimai.git
+
+您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)
+
+ - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static
+ - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置
+
+> 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。
+
+## FAQ
+
+配置 nonebot 或 cq-http 过程中出错？
+> 请查阅 https://github.com/nonebot/nonebot2 以及 https://github.com/Mrs4s/go-cqhttp 中的文档。
+
+部分消息发不出来？
+> 被风控了。解决方式：换号或者让这个号保持登陆状态和一定的聊天频率，持续一段时间。
+
+## 说明
+
+本 bot 提供了如下功能：
+
+命令 | 功能
+--- | ---
+help | 查看帮助文档
+今日舞萌 | 查看今天的舞萌运势
+XXXmaimaiXXX什么 | 随机一首歌
+随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲
+查歌<乐曲标题的一部分> | 查询符合条件的乐曲
+[绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息
+定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲
+分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线
+
+## 原作者
+
+[Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献
+
+## License
+
+MIT
+
+您可以自由使用本项目的代码用于商业或非商业的用途，但必须附带 MIT 授权协议。
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
-## è¯´æ ä»[mai-bot](https://github.com/Diving-Fish/mai-
+## è¯´æï¼å·²æ´æ°èèå½æ2023ï¼éæ°ä¸è½½èµæºï¼ ä»[mai-bot]
+(https://github.com/Diving-Fish/mai-
 bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
 b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
-maimai/static - envè®¾ç½®
-`maimai_font`å`b_cookie`,åå«æ¯strå¯¹è±¡ç`å­ä½`å`cookie` -
+maimai/static - ï¼å¯å¾ªï¼envè®¾ç½® `maimai_font`,æ¯strå¯¹è±¡ç`å­ä½` -
 æ°å¢æä»¤`bç«æç´¢[text]`
 æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
 [å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
-åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£: pip3 install nonebot_plugin_maimai
-nb plugin install nonebot_plugin_maimai # git clone
-é£æå»ºè®®ä½ è¿æ¯ç¨åä½èçç½¢ æ¨éè¦ä»[æ­¤é¾æ¥](https://
+åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£ï¼ä»éå¶ä¸ï¼: pip3 install
+nonebot_plugin_maimai nb plugin install nonebot_plugin_maimai git clone https:/
+/github.com/Agnes4m/nonebot_plugin_maimai.git æ¨éè¦ä»[æ­¤é¾æ¥](https://
 www.diving-fish.com/maibot/
 static.zip)ä¸è½½èµæºæä»¶å¹¶ï¼å¹¶å°å¶staticæä»¶è§£åå°:
 (ä»¥ä¸æ¹æ³2é1) - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
 æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static - æºå¨äººç®å½ä¸
 - æç»è·¯å¾ç±»ä¼¼æ¯/path/to/data/maimai/staticä¸­ãå¶ä¸­bot.pyæä»¶å¨/
 path/toä½ç½® > èµæºæä»¶ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·èªè§å¨ä¸è½½ 24
 å°æ¶åå é¤èµæºæä»¶ã ## FAQ éç½® nonebot æ cq-http
```

### Comparing `nonebot_plugin_maimai-0.2.0/PKG-INFO` & `nonebot_plugin_maimai-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Maimai DX plugin for NoneBot
-Home-page: https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai
+Home-page: https://github.com/Agnes4m/nonebot_plugin_maimai
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3)
 Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: pillow (>=9.3.0)
-Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_maimai
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <img src="https://s2.loli.net/2022/06/16/opBDE8Swad5rU3n.png" width="180" height="180" alt="NoneBotPluginLogo">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_maimai
@@ -40,37 +41,37 @@
 </a>
 <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
 </a>
-    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
-## 说明
+## 说明（已更新舞萌国服2023，重新下载资源）
 
 从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
 
 修改部分：
  - b40/b50可以艾特人查询
  - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
- - env设置 `maimai_font`和`b_cookie`,分别是str对象的`字体`和`cookie`
+ - （可循）env设置 `maimai_font`,是str对象的`字体`
  - 新增指令`b站搜索[text]`
 
 我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
 
 ## 前置步骤（和原项目一样）
 
-安装:
+安装（仍选其一）:
 
     pip3 install nonebot_plugin_maimai
     nb plugin install nonebot_plugin_maimai
-    # git clone 那我建议你还是用原作者的罢
+    git clone https://github.com/Agnes4m/nonebot_plugin_maimai.git
 
 您需要从[此链接](https://www.diving-fish.com/maibot/static.zip)下载资源文件并，并将其static文件解压到:(以下方法2选1)
 
  - pypi`nonebot_plugin_maimai`文件夹中 - 最终路径类似是/path/to/nonebot_plugin_maimai/static
  - 机器人目录下 - 最终路径类似是/path/to/data/maimai/static中。其中bot.py文件在/path/to位置
 
 > 资源文件仅供学习交流使用，请自觉在下载 24 小时内删除资源文件。
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.0 Summary:
-Maimai DX plugin for NoneBot Home-page: https://github.com/Umamusume-Agnes-
-Digital/nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin
-Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
->=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
-(>=3.8.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: nonebot-
-adapter-onebot (>=2.1.3) Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow (>=9.3.0)
-Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.1 Summary:
+Maimai DX plugin for NoneBot Home-page: https://github.com/Agnes4m/
+nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin Author:
+Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: httpx (>=0.22.0) Requires-
+Dist: nonebot-adapter-onebot (>=2.1.3) Requires-Dist: nonebot-plugin-txt2img
+(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow
+(>=9.3.0) Project-URL: Repository, https://github.com/Agnes4m/
 nonebot_plugin_maimai Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
-## è¯´æ ä»[mai-bot](https://github.com/Diving-Fish/mai-
+## è¯´æï¼å·²æ´æ°èèå½æ2023ï¼éæ°ä¸è½½èµæºï¼ ä»[mai-bot]
+(https://github.com/Diving-Fish/mai-
 bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
 b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
-maimai/static - envè®¾ç½®
-`maimai_font`å`b_cookie`,åå«æ¯strå¯¹è±¡ç`å­ä½`å`cookie` -
+maimai/static - ï¼å¯å¾ªï¼envè®¾ç½® `maimai_font`,æ¯strå¯¹è±¡ç`å­ä½` -
 æ°å¢æä»¤`bç«æç´¢[text]`
 æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
 [å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
-åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£: pip3 install nonebot_plugin_maimai
-nb plugin install nonebot_plugin_maimai # git clone
-é£æå»ºè®®ä½ è¿æ¯ç¨åä½èçç½¢ æ¨éè¦ä»[æ­¤é¾æ¥](https://
+åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£ï¼ä»éå¶ä¸ï¼: pip3 install
+nonebot_plugin_maimai nb plugin install nonebot_plugin_maimai git clone https:/
+/github.com/Agnes4m/nonebot_plugin_maimai.git æ¨éè¦ä»[æ­¤é¾æ¥](https://
 www.diving-fish.com/maibot/
 static.zip)ä¸è½½èµæºæä»¶å¹¶ï¼å¹¶å°å¶staticæä»¶è§£åå°:
 (ä»¥ä¸æ¹æ³2é1) - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
 æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static - æºå¨äººç®å½ä¸
 - æç»è·¯å¾ç±»ä¼¼æ¯/path/to/data/maimai/staticä¸­ãå¶ä¸­bot.pyæä»¶å¨/
 path/toä½ç½® > èµæºæä»¶ä»ä¾å­¦ä¹ äº¤æµä½¿ç¨ï¼è¯·èªè§å¨ä¸è½½ 24
 å°æ¶åå é¤èµæºæä»¶ã ## FAQ éç½® nonebot æ cq-http
```

