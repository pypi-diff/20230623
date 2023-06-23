# Comparing `tmp/mys_goods_tool-2.0.4.tar.gz` & `tmp/mys_goods_tool-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mys_goods_tool-2.0.4.tar", max compression
+gzip compressed data, was "mys_goods_tool-2.0.5.tar", max compression
```

## Comparing `mys_goods_tool-2.0.4.tar` & `mys_goods_tool-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/LICENSE
--rw-r--r--   0        0        0     3972 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/__main__.py
--rw-r--r--   0        0        0    58103 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/api.py
--rw-r--r--   0        0        0     5536 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/custom_css.py
--rw-r--r--   0        0        0     7599 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/custom_widget.py
--rw-r--r--   0        0        0     9570 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/data_model.py
--rw-r--r--   0        0        0    17597 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/exchange_mode.py
--rw-r--r--   0        0        0    43505 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/exchange_plan_view.py
--rw-r--r--   0        0        0     6910 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3-localized.html
--rw-r--r--   0        0        0     6840 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3.html
--rw-r--r--   0        0        0     6890 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/index.html
--rw-r--r--   0        0        0    10861 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt.js
--rw-r--r--   0        0        0    14792 2023-05-26 19:18:19.810899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt4.js
--rw-r--r--   0        0        0   366500 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/jquery.js
--rw-r--r--   0        0        0     6831 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/localized.html
--rw-r--r--   0        0        0    10717 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/geetest.py
--rw-r--r--   0        0        0    22544 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/login_view.py
--rw-r--r--   0        0        0    13045 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/tui.py
--rw-r--r--   0        0        0    17824 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/user_data.py
--rw-r--r--   0        0        0    11385 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/mys_goods_tool/utils.py
--rw-r--r--   0        0        0     1639 2023-05-26 19:18:19.814899 mys_goods_tool-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/LICENSE
+-rw-r--r--   0        0        0     3734 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/__main__.py
+-rw-r--r--   0        0        0    57821 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/api.py
+-rw-r--r--   0        0        0     5536 2023-06-23 14:24:06.803754 mys_goods_tool-2.0.5/mys_goods_tool/custom_css.py
+-rw-r--r--   0        0        0     7599 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/custom_widget.py
+-rw-r--r--   0        0        0     9681 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/data_model.py
+-rw-r--r--   0        0        0    17597 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/exchange_mode.py
+-rw-r--r--   0        0        0    43495 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/exchange_plan_view.py
+-rw-r--r--   0        0        0     6910 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3-localized.html
+-rw-r--r--   0        0        0     6840 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3.html
+-rw-r--r--   0        0        0     6890 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/index.html
+-rw-r--r--   0        0        0    10861 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt.js
+-rw-r--r--   0        0        0    14792 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt4.js
+-rw-r--r--   0        0        0   366500 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/jquery.js
+-rw-r--r--   0        0        0     6831 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/localized.html
+-rw-r--r--   0        0        0    10717 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/geetest.py
+-rw-r--r--   0        0        0    22213 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/login_view.py
+-rw-r--r--   0        0        0    12814 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/tui.py
+-rw-r--r--   0        0        0    17901 2023-06-23 14:24:06.807754 mys_goods_tool-2.0.5/mys_goods_tool/user_data.py
+-rw-r--r--   0        0        0    10056 2023-06-23 14:24:06.811754 mys_goods_tool-2.0.5/mys_goods_tool/utils.py
+-rw-r--r--   0        0        0     1639 2023-06-23 14:24:06.811754 mys_goods_tool-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5119 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.5/PKG-INFO
```

### Comparing `mys_goods_tool-2.0.4/LICENSE` & `mys_goods_tool-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/README.md` & `mys_goods_tool-2.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,24 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复启动后由于商品数据相关问题而导致的崩溃
-- 修复 Linux 实际不会应用 uvloop 的问题
-- 人机验证更新至
-  GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
+- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
 - [x] 支持米游社所有分区的商品兑换
 
-### TODO
-- [ ] 更新至极验第四代适应性验证
-
 ### 预览图
 
 <details>
   <summary>短信验证登录</summary>
   <img src="https://user-images.githubusercontent.com/63289359/235790425-7c502a69-baac-4ced-ba07-d068a88a7ae9.png" alt="短信验证登录页面" />
   <img src="https://user-images.githubusercontent.com/63289359/235790979-85954be8-023f-47e0-bb69-bb16385905d4.png" alt="人机验证页面" />
 </details>
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/__main__.py` & `mys_goods_tool-2.0.5/mys_goods_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/api.py` & `mys_goods_tool-2.0.5/mys_goods_tool/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 URL_GAME_LIST = "https://bbs-api.mihoyo.com/apihub/api/getGameList"
 URL_MYB = "https://api-takumi.mihoyo.com/common/homutreasure/v1/web/user/point?app_id=1&point_sn=myb"
 URL_DEVICE_LOGIN = "https://bbs-api.mihoyo.com/apihub/api/deviceLogin"
 URL_DEVICE_SAVE = "https://bbs-api.mihoyo.com/apihub/api/saveDevice"
 URL_GOOD_LIST = "https://api-takumi.mihoyo.com/mall/v1/web/goods/list?app_id=1&point_sn=myb&page_size=20&page={" \
                 "page}&game={game} "
 URL_CHECK_GOOD = "https://api-takumi.mihoyo.com/mall/v1/web/goods/detail?app_id=1&point_sn=myb&goods_id={}"
-URL_EXCHANGE = "https://api-takumi.mihoyo.com/mall/v1/web/goods/exchange"
+URL_EXCHANGE = "https://api-takumi.miyoushe.com/mall/v1/web/goods/exchange"
 URL_ADDRESS = "https://api-takumi.mihoyo.com/account/address/list?t={}"
 URL_REGISTRABLE = "https://webapi.account.mihoyo.com/Api/is_mobile_registrable?mobile={mobile}&t={t}"
 URL_CREATE_MMT = "https://webapi.account.mihoyo.com/Api/create_mmt?scene_type=1&now={now}&reason=user.mihoyo.com%2523%252Flogin%252Fcaptcha&action_type=login_by_mobile_captcha&t={t}"
 URL_CREATE_MOBILE_CAPTCHA = "https://webapi.account.mihoyo.com/Api/create_mobile_captcha"
 URL_GET_USER_INFO = "https://bbs-api.miyoushe.com/user/api/getUserFullInfo?uid={uid}"
 
 HEADERS_WEBAPI = {
@@ -193,15 +193,17 @@
     "Accept-Language":
         "zh-CN,zh-Hans;q=0.9",
     "Connection":
         "keep-alive",
     "Content-Type":
         "application/json;charset=utf-8",
     "Host":
-        "api-takumi.mihoyo.com",
+        "api-takumi.miyoushe.com",
+    "Origin":
+        "https://webstatic.mihoyo.com",
     "User-Agent":
         conf.device_config.USER_AGENT_MOBILE,
     "x-rpc-app_version":
         conf.device_config.X_RPC_APP_VERSION,
     "x-rpc-channel":
         "appstore",
     "x-rpc-client_type":
@@ -675,28 +677,28 @@
         else:
             logger.exception(f"检查用户 {phone_number} 是否可以注册 - 请求失败")
             return BaseApiStatus(network_error=True), None, device_id, None
 
 
 async def create_mmt(client: Optional[httpx.AsyncClient] = None,
                      use_v4: bool = True,
-                     device_id: str = generate_device_id(),
+                     device_id: str = None,
                      retry: bool = True) -> Tuple[
     BaseApiStatus, Optional[MmtData], str, Optional[httpx.AsyncClient]]:
     """
     发送短信验证前所需的人机验证任务申请
 
     :param client: httpx.AsyncClient 连接
     :param use_v4: 是否使用极验第四代人机验证
-    :param device_id: 设备 ID
+    :param device_id: 设备ID
     :param retry: 是否允许重试
     :return: (API返回状态, 人机验证任务数据, 设备ID, httpx.AsyncClient连接对象)
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = device_id
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     if use_v4:
         headers.setdefault("x-rpc-source", "accountWebsite")
     async def request():
         """
         发送请求的闭包函数
         """
         time_now = round(NtpTime.time() * 1000)
@@ -728,67 +730,62 @@
 
 
 async def create_mobile_captcha(phone_number: int,
                                 mmt_data: MmtData,
                                 geetest_result: Union[GeetestResult, GeetestResultV4],
                                 client: Optional[httpx.AsyncClient] = None,
                                 use_v4: bool = True,
-                                device_id: str = generate_device_id(),
+                                device_id: str = None,
                                 retry: bool = True
                                 ) -> Tuple[CreateMobileCaptchaStatus, Optional[httpx.AsyncClient]]:
     """
     发送短信验证码
 
     :param phone_number: 手机号
     :param mmt_data: 人机验证任务数据
     :param geetest_result: 人机验证结果数据
     :param client: httpx.AsyncClient 连接
     :param use_v4: 是否使用极验第四代人机验证
-    :param device_id: 设备 ID
+    :param device_id: 设备ID
     :param retry: 是否允许重试
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = device_id
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     if use_v4 and isinstance(geetest_result, GeetestResultV4):
-        params = {
+        geetest_v4_data = geetest_result.dict(skip_defaults=True)
+        content = {
             "action_type": "login",
             "mmt_key": mmt_data.mmt_key,
-            "geetest_v4_data": geetest_result.dict(skip_defaults=True),
-            "mobile": phone_number,
-            "t": round(NtpTime.time() * 1000)
+            "geetest_v4_data": str(geetest_v4_data).replace("'", '"'),
+            "mobile": str(phone_number),
+            "t": str(round(NtpTime.time() * 1000))
         }
     else:
-        params = {
+        content = {
             "action_type": "login",
             "mmt_key": mmt_data.mmt_key,
             "geetest_challenge": mmt_data.challenge,
             "geetest_validate": geetest_result.validate,
             "geetest_seccode": geetest_result.seccode,
             "mobile": phone_number,
             "t": round(NtpTime.time() * 1000)
         }
-    encoded_params = urlencode(params)
 
     async def request():
         """
         发送请求的闭包函数
         """
         return await client.post(URL_CREATE_MOBILE_CAPTCHA,
-                                 content=encoded_params,
+                                 data=content,
                                  headers=headers,
                                  timeout=conf.preference.timeout)
 
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
-                # FIXME 2023/4/13: 似乎会导致卡在连接状态，暂时弃用
-                #   res = await client.options(URL_CREATE_MOBILE_CAPTCHA,
-                #                            headers=headers,
-                #                            timeout=conf.preference.timeout)
-                #   cookies.update(res.cookies)
                 if client and not client.is_closed:
                     res = await request()
                 else:
                     async with httpx.AsyncClient() as client:
                         res = await request()
                 api_result = ApiResultHandler(res.json())
                 if api_result.success:
@@ -806,54 +803,50 @@
             logger.exception(f"发送短信验证码 - 请求失败")
             return CreateMobileCaptchaStatus(network_error=True), None
 
 
 async def get_login_ticket_by_captcha(phone_number: str,
                                       captcha: int,
                                       client: Optional[httpx.AsyncClient] = None,
+                                      device_id: str = None,
                                       retry: bool = True) -> \
         Tuple[
             GetCookieStatus, Optional[BBSCookies]]:
     """
     通过短信验证码获取 login_ticket
 
     :param phone_number: 手机号
     :param captcha: 短信验证码
     :param client: httpx.AsyncClient 连接
+    :param device_id: 设备ID
     :param retry: 是否允许重试
 
     >>> import asyncio
     >>> coroutine = get_cookie_token_by_captcha("12345678910", 123456)
     >>> assert asyncio.new_event_loop().run_until_complete(coroutine)[0].incorrect_captcha is True
     """
 
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = generate_device_id()
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     params = {
         "mobile": phone_number,
         "mobile_captcha": captcha,
         "source": "user.mihoyo.com",
         "t": round(NtpTime.time() * 1000),
     }
     encoded_params = urlencode(params)
 
     async def request():
         """
         发送请求的闭包函数
         """
-        _cookies = {}
-        _res = await client.options(URL_LOGIN_TICKET_BY_CAPTCHA,
-                                    headers=headers,
-                                    timeout=conf.preference.timeout
-                                    )
-        _cookies.update(_res.cookies)
+        # TODO 还需要进一步简化代码
         return await client.post(URL_LOGIN_TICKET_BY_CAPTCHA,
                                  headers=headers,
                                  content=encoded_params,
-                                 cookies=_cookies,
                                  timeout=conf.preference.timeout
                                  )
 
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 if client is not None:
@@ -973,27 +966,32 @@
             logger.debug(f"网络请求返回: {res.text}")
             return GetCookieStatus(incorrect_return=True), None
         else:
             logger.exception(f"通过短信验证码获取 cookie_token: 网络请求失败")
             return GetCookieStatus(network_error=True), None
 
 
-async def get_login_ticket_by_password(account: str, password: str, mmt_data: MmtData, geetest_result: GeetestResult,
+async def get_login_ticket_by_password(account: str,
+                                       password: str,
+                                       mmt_data: MmtData,
+                                       geetest_result: GeetestResult,
+                                       device_id: str = None,
                                        retry: bool = True) -> Tuple[GetCookieStatus, Optional[BBSCookies]]:
     """
     使用密码登录获取login_ticket
 
     :param account: 账号
     :param password: 密码
     :param mmt_data: GEETEST验证任务数据
     :param geetest_result: GEETEST验证结果数据
+    :param device_id: 设备ID
     :param retry: 是否允许重试
     """
     headers = HEADERS_WEBAPI.copy()
-    headers["x-rpc-device_id"] = generate_device_id()
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     params = {
         "account": account,
         "password": password,
         "is_crypto": False,
         "mmt_key": mmt_data.mmt_key,
         "geetest_challenge": mmt_data.challenge,
         "geetest_validate": geetest_result.validate,
@@ -1025,29 +1023,29 @@
             logger.debug(f"网络请求返回: {res.text}")
             return GetCookieStatus(incorrect_return=True), None
         else:
             logger.exception(f"使用密码登录获取login_ticket - 请求失败")
             return GetCookieStatus(network_error=True), None
 
 
-async def get_cookie_token_by_stoken(cookies: BBSCookies, device_id: Optional[str] = None, retry: bool = True) -> Tuple[
+async def get_cookie_token_by_stoken(cookies: BBSCookies, device_id: str = None, retry: bool = True) -> Tuple[
     GetCookieStatus, Optional[BBSCookies]]:
     """
     通过 stoken_v2 获取 cookie_token
 
     :param cookies: 米游社Cookies，需要包含 stoken_v2 和 mid
     :param device_id: X_RPC_DEVICE_ID
     :param retry: 是否允许重试
 
     >>> import asyncio
     >>> coroutine = get_cookie_token_by_stoken(BBSCookies())
     >>> assert asyncio.new_event_loop().run_until_complete(coroutine)[0].success is False
     """
     headers = HEADERS_PASSPORT_API.copy()
-    headers["x-rpc-device_id"] = device_id if device_id else generate_device_id()
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     if not cookies.stoken_v2:
         return GetCookieStatus(missing_stoken_v2=True), None
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
                     res = await client.get(
@@ -1074,29 +1072,29 @@
             logger.debug(f"网络请求返回: {res.text}")
             return GetCookieStatus(incorrect_return=True), None
         else:
             logger.exception(f"通过 stoken 获取 cookie_token: 网络请求失败")
             return GetCookieStatus(network_error=True), None
 
 
-async def get_stoken_v2_by_v1(cookies: BBSCookies, device_id: Optional[str] = None, retry: bool = True) -> Tuple[
+async def get_stoken_v2_by_v1(cookies: BBSCookies, device_id: str = None, retry: bool = True) -> Tuple[
     GetCookieStatus, Optional[BBSCookies]]:
     """
     通过 stoken_v1 获取 stoken_v2 以及 mid
 
     :param cookies: 米游社Cookies，需要包含 stoken_v1
     :param device_id: X_RPC_DEVICE_ID
     :param retry: 是否允许重试
 
     >>> import asyncio
     >>> coroutine = get_stoken_v2_by_v1(BBSCookies())
     >>> assert asyncio.new_event_loop().run_until_complete(coroutine)[0].success is False
     """
     headers = HEADERS_PASSPORT_API.copy()
-    headers["x-rpc-device_id"] = device_id if device_id else generate_device_id()
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     headers.setdefault("x-rpc-aigis", "")
     headers.setdefault("x-rpc-app_id", "bll8iq97cem8")
 
     if not cookies.stoken_v1:
         return GetCookieStatus(missing_stoken_v1=True), None
     try:
         async for attempt in get_async_retry(retry):
@@ -1128,29 +1126,29 @@
             logger.debug(f"网络请求返回: {res.text}")
             return GetCookieStatus(incorrect_return=True), None
         else:
             logger.exception(f"通过 stoken_v1 获取 stoken_v2: 网络请求失败")
             return GetCookieStatus(network_error=True), None
 
 
-async def get_ltoken_by_stoken(cookies: BBSCookies, device_id: Optional[str] = None, retry: bool = True) -> Tuple[
+async def get_ltoken_by_stoken(cookies: BBSCookies, device_id: str = None, retry: bool = True) -> Tuple[
     GetCookieStatus, Optional[BBSCookies]]:
     """
     通过 stoken_v2 和 mid 获取 ltoken
 
     :param cookies: 米游社Cookies，需要包含 stoken_v2 和 mid
     :param device_id: X_RPC_DEVICE_ID
     :param retry: 是否允许重试
 
     >>> import asyncio
     >>> coroutine = get_ltoken_by_stoken(BBSCookies())
     >>> assert asyncio.new_event_loop().run_until_complete(coroutine)[0].success is False
     """
     headers = HEADERS_PASSPORT_API.copy()
-    headers["x-rpc-device_id"] = device_id if device_id else generate_device_id()
+    headers["x-rpc-device_id"] = device_id or generate_device_id()
     if not cookies.stoken_v2:
         return GetCookieStatus(missing_stoken_v2=True), None
     if not cookies.mid:
         return GetCookieStatus(missing_mid=True), None
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/custom_css.py` & `mys_goods_tool-2.0.5/mys_goods_tool/custom_css.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/custom_widget.py` & `mys_goods_tool-2.0.5/mys_goods_tool/custom_widget.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/data_model.py` & `mys_goods_tool-2.0.5/mys_goods_tool/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,43 +126,45 @@
     def time_text(self):
         """
         商品的兑换时间文本
 
         :return:
         如果返回`None`，说明需要进一步查询商品详细信息才能获取兑换时间
         """
-        if self.is_time_end():
+        if self.time_end:
             return "已结束"
         elif self.time == 0:
             return None
-        elif self.is_time_limited():
+        elif self.time_limited:
             return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.time))
         else:
             return "任何时间"
 
     @property
     def stoke_text(self):
         """
         商品的库存文本
         """
-        if self.is_time_end():
+        if self.time_end:
             return "无"
-        elif self.is_time_limited():
+        elif self.time_limited:
             return str(self.num)
         else:
             return "不限"
 
-    def is_time_limited(self):
+    @property
+    def time_limited(self):
         """
         是否为限时商品
         """
         # 不限量被认为是不限时商品
         return not self.unlimit
 
-    def is_time_end(self):
+    @property
+    def time_end(self):
         """
         兑换是否已经结束
         """
         return self.next_time == 0
 
     @property
     def num(self):
@@ -306,14 +308,18 @@
     """成功"""
     network_error = False
     """连接失败"""
     incorrect_return = False
     """服务器返回数据不正确"""
     login_expired = False
     """登录失效"""
+    need_verify = False
+    """需要进行人机验证"""
+    invalid_ds = False
+    """Headers DS无效"""
 
     def __bool__(self):
         if self.success:
             return True
         else:
             return False
 
@@ -384,9 +390,9 @@
 class GeetestResultV4(BaseModel):
     """
     GEETEST GT4 人机验证结果数据
     """
     captcha_id: str
     lot_number: str
     pass_token: str
-    gen_time: int
+    gen_time: str
     captcha_output: str
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/exchange_mode.py` & `mys_goods_tool-2.0.5/mys_goods_tool/exchange_mode.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/exchange_plan_view.py` & `mys_goods_tool-2.0.5/mys_goods_tool/exchange_plan_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         # 进度条、刷新按钮
         self.loading.show()
         self.button_refresh.disable()
 
         for goods_data in self.good_dict.values():
             name, abbr = goods_data.partition
             good_list_status, good_list = await get_good_list(abbr)
-            good_list = list(filter(lambda x: x.is_time_limited() and not x.is_time_end(), good_list))
+            good_list = list(filter(lambda x: x.time_limited and not x.time_end, good_list))
 
             # 一种情况是获取成功但返回的商品数据为空，一种是API请求失败
             goods_data.option_list.clear_options()
             if not good_list_status:
                 self.app.notice(f"[bold red]获取频道 [bold red]{name}[/] 的商品数据失败！[/]")
                 # TODO 待补充各种错误情况
             if good_list:
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3-localized.html` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3-localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/gt3.html` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/gt3.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/index.html` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/index.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt.js` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/gt4.js` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/gt4.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/libs/jquery.js` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/libs/jquery.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest-webui/localized.html` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest-webui/localized.html`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/geetest.py` & `mys_goods_tool-2.0.5/mys_goods_tool/geetest.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/login_view.py` & `mys_goods_tool-2.0.5/mys_goods_tool/login_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from rich.markdown import Markdown
 from textual.app import ComposeResult
 from textual.widgets import (
     Input
 )
 
 from mys_goods_tool.api import create_mobile_captcha, create_mmt, get_login_ticket_by_captcha, \
-    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken, \
-    check_registrable
+    get_multi_token_by_login_ticket, get_cookie_token_by_stoken, get_stoken_v2_by_v1, get_ltoken_by_stoken
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import RadioStatus, StaticStatus, ControllableButton, LoadingDisplay
 from mys_goods_tool.data_model import GeetestResult, MmtData, GetCookieStatus
 from mys_goods_tool.exchange_plan_view import ExchangePlanView
 from mys_goods_tool.geetest import GeetestProcessManager, SetAddressProcessManager
 from mys_goods_tool.user_data import config as conf, UserAccount, CONFIG_PATH
 from mys_goods_tool.utils import logger
@@ -141,15 +140,16 @@
 
         self.button = self.ButtonTuple(
             send=ControllableButton("发送短信验证码", variant="primary", id="create_captcha_send"),
             stop_geetest=ControllableButton("放弃人机验证", variant="warning", id="create_captcha_stop_geetest"),
             success=ControllableButton("完成", variant="success", id="create_captcha_success"),
             error=ControllableButton("返回", variant="error", id="create_captcha_error")
         )
-        [i.hide() for i in self.button[1:]]
+        for button in self.button[1:]:
+            button.hide()
 
     def compose(self) -> ComposeResult:
         yield Static("手机号", classes="label")
         yield self.input
         yield Static()
         yield from self.button
         yield Static()
@@ -276,25 +276,15 @@
             return
         self.before_create_captcha = False
 
         [i.turn_off() for i in CaptchaLoginInformation.radio_tuple]
         self.button.send.disable()
         self.loading.show()
 
-        if PhoneForm.client:
-            await PhoneForm.client.aclose()
-        check_registrable_status, registrable, PhoneForm.device_id, PhoneForm.client = await check_registrable(
-            int(self.input.value))
-        if registrable:
-            self.close_create_captcha_send()
-            self.button.error.show()
-            self.app.notice("[red]该手机号尚未注册！[/]")
-            return
-        create_mmt_status, self.mmt_data, PhoneForm.device_id, PhoneForm.client = await create_mmt(PhoneForm.client,
-                                                                                                   device_id=PhoneForm.device_id)
+        create_mmt_status, self.mmt_data, PhoneForm.device_id, PhoneForm.client = await create_mmt()
         if not create_mmt_status:
             self.close_create_captcha_send()
             self.button.error.show()
             self.app.notice("[red]获取Geetest行为验证任务数据失败！[/]")
             return
         else:
             logger.info(f"已成功获取Geetest行为验证任务数据 {self.mmt_data}")
@@ -394,15 +384,18 @@
         account: Optional[UserAccount] = None
         login_status: GetCookieStatus = GetCookieStatus(success=False)
         phone_number = PhoneForm.input.value
         captcha = int(self.input.value) if self.input.value.isdigit() else self.input.value
 
         # 1. 通过短信验证码获取 login_ticket / 使用已有 login_ticket
         if captcha:
-            login_status, cookies = await get_login_ticket_by_captcha(phone_number, captcha, PhoneForm.client)
+            login_status, cookies = await get_login_ticket_by_captcha(phone_number,
+                                                                      captcha,
+                                                                      PhoneForm.client,
+                                                                      PhoneForm.device_id)
             if login_status:
                 logger.info(f"用户 {phone_number} 成功获取 login_ticket: {cookies.login_ticket}")
                 account = conf.accounts.get(cookies.bbs_uid)
                 """当前的账户数据对象"""
                 if not account or not account.cookies:
                     conf.accounts.update({
                         cookies.bbs_uid: UserAccount(phone_number=phone_number, cookies=cookies)
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/tui.py` & `mys_goods_tool-2.0.5/mys_goods_tool/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
-from io import StringIO
 
+from io import StringIO
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.text import Text
 from textual import events
 from textual.app import App, ComposeResult, DEFAULT_COLORS
 from textual.binding import Binding
 from textual.color import Color
@@ -27,29 +27,25 @@
 from mys_goods_tool.user_data import ROOT_PATH, VERSION
 from mys_goods_tool.utils import LOG_FORMAT, logger
 
 WELCOME_MD = """
 # Mys_Goods_Tool - 米游社商品兑换工具
 
 ## 更新说明
-- 修复启动后由于商品数据相关问题而导致的崩溃
-- 修复 Linux 实际不会应用 uvloop 的问题
-- 人机验证更新至 GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
+
+- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
 
 ## 功能和特性
 
 - 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - 短信验证码登录（只需接收一次验证码）
 - 内置人机验证页面，无需前往官网验证
 - 多账号支持
 - 支持米游社所有分区的商品兑换
 
-### TODO
-- 更新至极验第四代适应性验证
-
 ## 其他
 - [**🔗完整说明文档**](https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki)
 - 仅供学习时参考
 
 - 相似项目推荐:  \
   **mysTool - 米游社辅助工具插件**  \
   简介：NoneBot2 插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒  \
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/user_data.py` & `mys_goods_tool-2.0.5/mys_goods_tool/user_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
 from json import JSONDecodeError
-from pathlib import Path
-from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
-    Mapping
 
+import os
 from httpx import Cookies
 from loguru import logger
+from pathlib import Path
 from pydantic import BaseModel, Extra, ValidationError, BaseSettings, validator
+from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
+    Mapping
 
 from mys_goods_tool.data_model import BaseModelWithSetter, Good, Address, GameRecord, BaseModelWithUpdate
 
 ROOT_PATH = Path("./")
 """程序所在目录"""
 
 CONFIG_PATH = ROOT_PATH / "user_data.json"
 """用户数据文件默认路径"""
 
-VERSION = "2.0.4"
+VERSION = "2.0.5"
 """程序当前版本"""
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     DictStrAny = Dict[str, Any]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
@@ -348,14 +348,15 @@
     '''Android 设备传入url参数生成 DS 所需的 salt'''
     SALT_PROD: str = "JwYDpKvLj6MrMqqYU6jTKF17KNO2PXoS"
 
     class Config(Preference.Config):
         pass
 
 
+# TODO 与用户数据文件中的配置有差异时询问是否使用更新
 class DeviceConfig(BaseSettings):
     """
     设备信息
     DS算法与设备信息有关联，非必要请勿修改
     """
     USER_AGENT_MOBILE: str = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) miHoYoBBS/2.42.1"
     '''移动端 User-Agent(Mozilla UA)'''
@@ -390,15 +391,15 @@
     '''安卓端 x-rpc-sys_version'''
 
     X_RPC_CHANNEL: str = "appstore"
     '''Headers所用的 x-rpc-channel'''
     X_RPC_CHANNEL_ANDROID: str = "miyousheluodi"
     '''安卓端 x-rpc-channel'''
 
-    X_RPC_APP_VERSION: str = "2.28.1"
+    X_RPC_APP_VERSION: str = "2.52.1"
     '''Headers所用的 x-rpc-app_version'''
     X_RPC_PLATFORM: str = "ios"
     '''Headers所用的 x-rpc-platform'''
     UA: str = "\".Not/A)Brand\";v=\"99\", \"Microsoft Edge\";v=\"103\", \"Chromium\";v=\"103\""
     '''Headers所用的 sec-ch-ua'''
     UA_PLATFORM: str = "\"macOS\""
     '''Headers所用的 sec-ch-ua-platform'''
```

### Comparing `mys_goods_tool-2.0.4/mys_goods_tool/utils.py` & `mys_goods_tool-2.0.5/mys_goods_tool/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+import time
+from multiprocessing import Pool, pool
+
 import hashlib
+import httpx
 import json
+import ntplib
 import os
 import random
 import string
-import time
-import traceback
+import tenacity
 import uuid
-from multiprocessing import Pool, pool
+from loguru import logger
+from pydantic import ValidationError
 from socket import socket, AF_INET, SOCK_STREAM
 from typing import Literal, Union, Dict, List, Any, Callable, Iterable, Optional
 from urllib.parse import urlencode
 
-import httpx
-import ntplib
-import tenacity
-from loguru import logger
-from pydantic import ValidationError
-
 from mys_goods_tool.user_data import config as conf
 
 LOG_FORMAT: str = (
     "<g>{time:MM-DD HH:mm:ss}</g> "
     "[<lvl>{level}</lvl>] "
     "<c><u>{name}</u></c> | "
     "{message}"
@@ -77,16 +76,15 @@
                 return False
             try:
                 for attempt in get_async_retry(True):
                     with attempt:
                         cls.time_offset = ntplib.NTPClient().request(
                             conf.preference.ntp_server).tx_time - time.time()
             except tenacity.RetryError:
-                logger.error("校对互联网时间失败，改为使用本地时间")
-                logger.debug(traceback.format_exc())
+                logger.exception("校对互联网时间失败，改为使用本地时间")
                 return False
             logger.info("互联网时间校对完成")
             return True
         else:
             logger.info("未开启互联网时间校对，跳过时间同步")
             return True
 
@@ -101,58 +99,14 @@
 def generate_device_id() -> str:
     """
     生成随机的x-rpc-device_id
     """
     return str(uuid.uuid4()).upper()
 
 
-def check_login(response: str):
-    """
-    通过网络请求返回的数据，检查是否登录失效
-
-    如果返回数据为`None`，返回`True`
-
-    :param response: 网络请求返回的数据
-    :return: 是否登录失效
-    """
-    try:
-        if response is None:
-            return True
-        res_dict = json.loads(response)
-        if "message" in res_dict:
-            response: str = res_dict["message"]
-            for message in ("Please login", "登录失效", "尚未登录"):
-                if response.find(message) != -1:
-                    return False
-            return True
-    except (json.JSONDecodeError, KeyError):
-        return True
-
-
-def check_ds(response: str):
-    """
-    通过网络请求返回的数据，检查Header中DS是否有效
-
-    如果返回数据为`None`，返回`True`
-
-    :param response: 网络请求返回的数据
-    :return: DS是否有效
-    """
-    try:
-        if response is None:
-            return True
-        res_dict = json.loads(response)
-        if res_dict["message"] == "invalid request":
-            return False
-        else:
-            return True
-    except (json.JSONDecodeError, KeyError):
-        return True
-
-
 def cookie_str_to_dict(cookie_str: str) -> Dict[str, str]:
     """
     将字符串Cookie转换为字典Cookie
     """
     cookie_str = cookie_str.replace(" ", "")
     # Cookie末尾缺少 ; 的情况
     if cookie_str[-1] != ";":
@@ -184,15 +138,16 @@
     获取Headers中所需DS
 
     :param data: 可选，网络请求中需要发送的数据
     :param params: 可选，URL参数
     :param platform: 可选，平台，ios或android
     :param salt: 可选，自定义salt
     """
-    if data is None and params is None or salt != conf.salt_config.SALT_PROD:
+    if data is None and params is None or \
+            salt is not None and salt != conf.salt_config.SALT_PROD:
         if platform == "ios":
             salt = salt or conf.salt_config.SALT_IOS
         else:
             salt = salt or conf.salt_config.SALT_ANDROID
         t = str(int(NtpTime.time()))
         a = "".join(random.sample(
             string.ascii_lowercase + string.digits, 6))
@@ -236,16 +191,15 @@
     try:
         async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
                     res = await client.get(url, timeout=conf.preference.timeout, follow_redirects=True)
                 return res.content
     except tenacity.RetryError:
-        logger.error(f"下载文件 - {url} 失败")
-        logger.debug(f"{traceback.format_exc()}")
+        logger.exception(f"下载文件 - {url} 失败")
 
 
 PORT_RANGE = (1024, 49151)
 """
 随机选择的端口所在范围
 
 端口范围说明：https://www.rfc-editor.org/rfc/rfc6335.html#section-6
@@ -318,16 +272,15 @@
             self.index = 0
         if not success:
             return False
         else:
             try:
                 conf.device_config.parse_obj(Subscribe.conf_list[self.index]["config"])
             except ValidationError:
-                logger.error(f"获取在线配置资源 - 加载配置失败")
-                logger.debug(traceback.format_exc())
+                logger.exception(f"获取在线配置资源 - 加载配置失败")
                 return False
 
             self.index += 1
             return True
 
 
 class ProcessManager:
```

### Comparing `mys_goods_tool-2.0.4/pyproject.toml` & `mys_goods_tool-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mys-goods-tool"
-version = "2.0.4"
+version = "2.0.5"
 description = "米游社商品兑换工具|短信验证登录|终端TUI界面"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.ml>"]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 repository = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 documentation = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki"
 keywords = ["mihoyo", "mihoyobbs", "genshin impact", "textual", "tui"]
@@ -19,30 +19,30 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 tenacity = "^8.2.2"
-requests = "^2.30.0"
+requests = "^2.31.0"
 ping3 = "^4.0.4"
 ntplib = "^0.4.0"
-pydantic = "^1.10.6"
+pydantic = "^1.10.9"
 loguru = "^0.7.0"
-httpx = "^0.24.0"
-rich = "^13.3.5"
-textual = "^0.24.1"
+httpx = "^0.24.1"
+rich = "^13.4.2"
+textual = "^0.27.0"
 socksio = "^1.0.0"
 apscheduler = "^3.10.1"
 
 [tool.poetry.group.uvloop.dependencies]
 uvloop = "^0.17.0"
 
 [tool.poetry.group.pyinstaller.dependencies]
-pyinstaller = "==5.10.1"
+pyinstaller = "==5.12.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-html = "^3.2.0"
 pytest-asyncio = "^0.21.0"
 flake8 = "^6.0.0"
```

### Comparing `mys_goods_tool-2.0.4/PKG-INFO` & `mys_goods_tool-2.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: mys-goods-tool
-Version: 2.0.4
+Version: 2.0.5
 Summary: 米游社商品兑换工具|短信验证登录|终端TUI界面
 Home-page: https://github.com/Ljzd-PRO/Mys_Goods_Tool
 Keywords: mihoyo,mihoyobbs,genshin impact,textual,tui
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apscheduler (>=3.10.1,<4.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
 Requires-Dist: ping3 (>=4.0.4,<5.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: socksio (>=1.0.0,<2.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
-Requires-Dist: textual (>=0.24.1,<0.25.0)
+Requires-Dist: textual (>=0.27.0,<0.28.0)
 Project-URL: Bug Tracker, https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues
 Project-URL: Documentation, https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki
 Project-URL: Repository, https://github.com/Ljzd-PRO/Mys_Goods_Tool
 Description-Content-Type: text/markdown
 
 <div>
   <img alt="Mys_Goods_Tool 预览" src="https://user-images.githubusercontent.com/63289359/235797444-21a86294-609e-4c7a-9d7d-5d3683fe6ab2.png" width="45%" />
@@ -44,30 +44,24 @@
   <img alt="代码行数" src="https://img.shields.io/tokei/lines/github/Ljzd-PRO/Mys_Goods_Tool?style=for-the-badge">
   <img alt="构建结果" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/build-v2.yml?event=pull_request&style=for-the-badge">
   <img alt="Python版本兼容性测试" src="https://img.shields.io/github/actions/workflow/status/Ljzd-PRO/Mys_Goods_Tool/python-package.yml?event=pull_request&label=Versions%20Test&style=for-the-badge">
 </div>
 
 ### 更新说明
 
-- 修复启动后由于商品数据相关问题而导致的崩溃
-- 修复 Linux 实际不会应用 uvloop 的问题
-- 人机验证更新至
-  GT4（但实际上暂时不可用 [#105](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues/105#issuecomment-1552727784)）
+- 修复短信验证码发送失败的问题 #105 #94 #104 - #126 by @Night-stars-1
 
 ## 功能和特性
 
 - [x] 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - [x] 短信验证码登录（只需接收一次验证码）
 - [x] 内置人机验证页面，无需前往官网验证
 - [x] 多账号支持
 - [x] 支持米游社所有分区的商品兑换
 
-### TODO
-- [ ] 更新至极验第四代适应性验证
-
 ### 预览图
 
 <details>
   <summary>短信验证登录</summary>
   <img src="https://user-images.githubusercontent.com/63289359/235790425-7c502a69-baac-4ced-ba07-d068a88a7ae9.png" alt="短信验证登录页面" />
   <img src="https://user-images.githubusercontent.com/63289359/235790979-85954be8-023f-47e0-bb69-bb16385905d4.png" alt="人机验证页面" />
 </details>
```

