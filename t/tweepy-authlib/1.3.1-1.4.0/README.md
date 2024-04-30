# Comparing `tmp/tweepy_authlib-1.3.1.tar.gz` & `tmp/tweepy_authlib-1.4.0.tar.gz`

## Comparing `tweepy_authlib-1.3.1.tar` & `tweepy_authlib-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.editorconfig
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.env.example
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/License.txt
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/example_json.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/example_pickle.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tests/test_main.py
--rw-r--r--   0        0        0    33475 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/CookieSessionUserHandler.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/__about__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.gitignore
--rw-r--r--   0        0        0    12308 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/Readme.md
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/.editorconfig
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/.env.example
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/License.txt
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/example_json.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/example_pickle.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/tests/test_main.py
+-rw-r--r--   0        0        0    33755 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/tweepy_authlib/CookieSessionUserHandler.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/tweepy_authlib/__about__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/tweepy_authlib/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/.gitignore
+-rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/Readme.md
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    17378 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.0/PKG-INFO
```

### Comparing `tweepy_authlib-1.3.1/License.txt` & `tweepy_authlib-1.4.0/License.txt`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.3.1/tweepy_authlib/CookieSessionUserHandler.py` & `tweepy_authlib-1.4.0/tweepy_authlib/CookieSessionUserHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,23 @@
     認証フローは2023年2月現在の Twitter Web App (Chrome Desktop) の挙動に極力合わせたもの
     requests.auth.AuthBase を継承しているので、tweepy.API の auth パラメーターに渡すことができる
 
     ref: https://github.com/mikf/gallery-dl/blob/master/gallery_dl/extractor/twitter.py
     ref: https://github.com/fa0311/TwitterFrontendFlow/blob/master/TwitterFrontendFlow/TwitterFrontendFlow.py
     """
 
-    user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36'
-    sec_ch_ua = '"Chromium";v="116", "Not)A;Brand";v="24", "Google Chrome";v="116"'
+    # User-Agent と Sec-CH-UA を Chrome 124 に偽装
+    USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36'
+    SEC_CH_UA = '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"'
+
+    # Twitter Web App (GraphQL API) の Bearer トークン
+    TWITTER_WEB_APP_BEARER_TOKEN = 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA'
+
+    # 旧 TweetDeck (Twitter API v1.1) の Bearer トークン
+    TWEETDECK_BEARER_TOKEN = 'Bearer AAAAAAAAAAAAAAAAAAAAAFQODgEAAAAAVHTp76lzh3rFzcHbmHVvQxYYpTw%3DckAlMINMjmCwxUcaXbAN4XqJVdgMJaHqNOFgPMK0zN1qLqLQCF'
 
 
     def __init__(self, cookies: Optional[RequestsCookieJar] = None, screen_name: Optional[str] = None, password: Optional[str] = None) -> None:
         """
         CookieSessionUserHandler を初期化する
         cookies と screen_name, password のどちらかを指定する必要がある
 
@@ -63,28 +70,26 @@
 
         # パスワードが空文字列
         if self.password == '':
             raise ValueError('password must not be empty string.')
 
         # HTML 取得時の HTTP リクエストヘッダー
         self._html_headers = {
-            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
+            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'ja',
-            'cache-control': 'no-cache',
-            'pragma': 'no-cache',
-            'sec-ch-ua': self.sec_ch_ua,
+            'sec-ch-ua': self.SEC_CH_UA,
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
             'sec-fetch-mode': 'navigate',
             'sec-fetch-site': 'same-origin',
             'sec-fetch-user': '?1',
             'upgrade-insecure-requests': '1',
-            'user-agent': self.user_agent,
+            'user-agent': self.USER_AGENT,
         }
 
         # JavaScript 取得時の HTTP リクエストヘッダー
         self._js_headers = self._html_headers.copy()
         self._js_headers['accept'] = '*/*'
         self._js_headers['referer'] = 'https://twitter.com/'
         self._js_headers['sec-fetch-dest'] = 'script'
@@ -92,74 +97,46 @@
         del self._js_headers['sec-fetch-user']
 
         # 認証フロー API アクセス時の HTTP リクエストヘッダー
         self._auth_flow_api_headers = {
             'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'ja',
-            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-            'cache-control': 'no-cache',
+            'authorization': self.TWITTER_WEB_APP_BEARER_TOKEN,
+            'content-type': 'application/json',
             'origin': 'https://twitter.com',
-            'pragma': 'no-cache',
             'referer': 'https://twitter.com/',
-            'sec-ch-ua': self.sec_ch_ua,
+            'sec-ch-ua': self.SEC_CH_UA,
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-site',
-            'user-agent': self.user_agent,
+            'user-agent': self.USER_AGENT,
             'x-csrf-token': None,  # ここは後でセットする
             'x-guest-token': None,  # ここは後でセットする
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'ja',
         }
 
-        # 旧 TweetDeck API (Twitter API v1.1) アクセス時の HTTP リクエストヘッダー
-        self._tweetdeck_api_headers = {
-            'accept': 'text/plain, */*; q=0.01',
-            'accept-encoding': 'gzip, deflate, br',
-            'accept-language': 'ja',
-            # 旧 TweetDeck の Bearer トークンが無効化されたため、代わりに Twitter Web App の Bearer トークンを使う
-            # 'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAAF7aAAAAAAAASCiRjWvh7R5wxaKkFp7MM%2BhYBqM%3DbQ0JPmjU9F6ZoMhDfI4uTNAaQuTDm2uO9x3WFVr2xBZ2nhjdP0',
-            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-            'cache-control': 'no-cache',
-            # 旧 TweetDeck 自体は廃止されているので、origin と referer は Twitter Web App からのアクセスという体にしている
-            'origin': 'https:/twitter.com',
-            'pragma': 'no-cache',
-            'referer': 'https://twitter.com/',
-            'sec-ch-ua': self.sec_ch_ua,
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"Windows"',
-            'sec-fetch-dest': 'empty',
-            'sec-fetch-mode': 'cors',
-            'sec-fetch-site': 'same-site',
-            'user-agent': self.user_agent,
-            'x-csrf-token': None,  # ここは後でセットする
-            'x-twitter-auth-type': 'OAuth2Session',
-            'x-twitter-client-version': 'Twitter-TweetDeck-blackbird-chrome/4.0.220811153004 web/',
-        }
-
         # GraphQL API (Twitter Web App API) アクセス時の HTTP リクエストヘッダー
-        ## tweepy-authlib 内部では使われておらず、ユーザーの便宜のために用意しているもの
-        ## GraphQL API は https://twitter.com/i/api/graphql/ 配下にあり同一ドメインのため、origin と referer は意図的に省略している
+        ## GraphQL API は https://twitter.com/i/api/graphql/ 配下にあり同一ドメインのため、referer は意図的に省略している
         self._graphql_api_headers = {
-            'accept': 'text/plain, */*; q=0.01',
+            'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'ja',
-            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-            'cache-control': 'no-cache',
-            'pragma': 'no-cache',
-            'sec-ch-ua': self.sec_ch_ua,
+            'authorization': self.TWITTER_WEB_APP_BEARER_TOKEN,
+            'content-type': 'application/json',
+            'sec-ch-ua': self.SEC_CH_UA,
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-site',
-            'user-agent': self.user_agent,
+            'user-agent': self.USER_AGENT,
             'x-csrf-token': None,  # ここは後でセットする
             'x-twitter-active-user': 'yes',
             'x-twitter-auth-type': 'OAuth2Session',
             'x-twitter-client-language': 'ja',
         }
 
         # Cookie ログイン用のセッションを作成
@@ -185,24 +162,26 @@
             raise tweepy.TweepyException('Failed to get auth_token or ct0 from Cookie')
 
         # Cookie の "gt" 値 (ゲストトークン) を認証フロー API 用ヘッダーにセット
         guest_token = self._session.cookies.get('gt')
         if guest_token:
             self._auth_flow_api_headers['x-guest-token'] = guest_token
 
-        # Cookie の "ct0" 値 (CSRF トークン) を TweetDeck API 用ヘッダーにセット
+        # Cookie の "ct0" 値 (CSRF トークン) を GraphQL API 用ヘッダーにセット
         csrf_token = self._session.cookies.get('ct0')
         if csrf_token:
             self._auth_flow_api_headers['x-csrf-token'] = csrf_token
-            self._tweetdeck_api_headers['x-csrf-token'] = csrf_token
             self._graphql_api_headers['x-csrf-token'] = csrf_token
 
-        # これ以降は基本 TweetDeck API へのアクセスしか行わないので、セッションのヘッダーを TweetDeck API 用のものに差し替える
+        # セッションのヘッダーを GraphQL API 用のものに差し替える
+        ## 以前は旧 TweetDeck API 用ヘッダーに差し替えていたが、旧 TweetDeck が完全廃止されたことで
+        ## 逆に怪しまれる可能性があるため GraphQL API 用ヘッダーに変更した
+        ## cross_origin=True を指定して、twitter.com から api.twitter.com にクロスオリジンリクエストを送信した際のヘッダーを模倣する
         self._session.headers.clear()
-        self._session.headers.update(self._tweetdeck_api_headers)
+        self._session.headers.update(self.get_graphql_api_headers(cross_origin=True))
 
 
     def __call__(self, request: PreparedRequest) -> PreparedRequest:
         """
         requests ライブラリからリクエスト開始時に呼び出されるフック
 
         Args:
@@ -211,20 +190,43 @@
         Returns:
             PreparedRequest: 認証情報を追加した PreparedRequest オブジェクト
         """
 
         # リクエストヘッダーを認証用セッションのものに差し替える
         request.headers.update(self._session.headers)  # type: ignore
 
+        # Twitter API v1.1 の一部 API には旧 TweetDeck 用の Bearer トークンでないとアクセスできないため、
+        # 該当の API のみ旧 TweetDeck 用の Bearer トークンに差し替える
+        # それ以外の API ではそのまま Twitter Web App の Bearer トークンを使い続けることで、不審判定される可能性を下げる
+        ## OldTweetDeck の interception.js に記載の API のうち、明示的に PUBLIC_TOKEN[1] が設定されている API が対象
+        ## ref: https://raw.githubusercontent.com/dimdenGD/OldTweetDeck/main/src/interception.js
+        TWEETDECK_BEARER_TOKEN_REQUIRED_APIS = [
+            '/1.1/statuses/home_timeline.json',
+            '/1.1/lists/statuses.json',
+            '/1.1/activity/about_me.json',
+            '/1.1/statuses/mentions_timeline.json',
+            '/1.1/favorites/',
+            '/1.1/collections/',
+        ]
+        assert request.url is not None
+        if any(api_url in request.url for api_url in TWEETDECK_BEARER_TOKEN_REQUIRED_APIS):
+            request.headers['authorization'] = self.TWEETDECK_BEARER_TOKEN
+
+        # upload.twitter.com 以下の API のみ、Twitter Web App の挙動に合わせいくつかのヘッダーを削除する
+        if 'upload.twitter.com' in request.url:
+            request.headers.pop('x-client-transaction-id', None)  # 未実装だが将来的に実装した時のため
+            request.headers.pop('x-twitter-active-user', None)
+            request.headers.pop('x-twitter-client-language', None)
+
         # Cookie を認証用セッションのものに差し替える
         request._cookies.update(self._session.cookies)  # type: ignore
         cookie_header = ''
         for key, value in self._session.cookies.get_dict().items():
             cookie_header += f'{key}={value}; '
-        request.headers['cookie'] = cookie_header
+        request.headers['cookie'] = cookie_header.rstrip('; ')
 
         # API からレスポンスが返ってきた際に自動で CSRF トークンを更新する
         ## やらなくても大丈夫かもしれないけど、念のため
         request.hooks['response'].append(self._on_response_received)
 
         # 認証情報を追加した PreparedRequest オブジェクトを返す
         return request
@@ -247,15 +249,15 @@
 
     def get_cookies(self) -> RequestsCookieJar:
         """
         現在のログインセッションの Cookie を取得する
         返される RequestsCookieJar を pickle などで保存しておくことで、再ログインせずにセッションを継続できる
 
         Returns:
-            str: RequestsCookieJar
+            RequestsCookieJar: Cookie
         """
 
         return self._session.cookies
 
 
     def get_cookies_as_dict(self) -> Dict[str, str]:
         """
@@ -265,59 +267,55 @@
         Returns:
             Dict[str, str]: Cookie
         """
 
         return self._session.cookies.get_dict()
 
 
-    def get_tweetdeck_api_headers(self) -> Dict[str, str]:
-        """
-        旧 TweetDeck API (Twitter API v1.1) アクセス用の HTTP リクエストヘッダーを取得する
-        このリクエストヘッダーを使い独自に API リクエストを行う際は、
-        必ず x-csrf-token ヘッダーの値を常に Cookie 内の "ct0" と一致させるように実装しなければならない
-
-        Returns:
-            Dict[str, str]: 旧 TweetDeck API (Twitter API v1.1) アクセス用の HTTP リクエストヘッダー
-        """
-
-        return self._tweetdeck_api_headers
-
-
-    def get_graphql_api_headers(self) -> Dict[str, str]:
+    def get_graphql_api_headers(self, cross_origin: bool = False) -> Dict[str, str]:
         """
         GraphQL API (Twitter Web App API) アクセス用の HTTP リクエストヘッダーを取得する
         このリクエストヘッダーを使い独自に API リクエストを行う際は、
         必ず x-csrf-token ヘッダーの値を常に Cookie 内の "ct0" と一致させるように実装しなければならない
+        Twitter API v1.1 に使う場合は cross_origin=True を指定すること (api.twitter.com が twitter.com から見て cross-origin になるため)
+        逆に GraphQL API に使う場合は cross_origin=False でなければならない (GraphQL API は twitter.com から見て same-origin になるため)
+
+        Args:
+            cross_origin (bool, optional): 返すヘッダーを twitter.com 以外のオリジンに送信するかどうか. Defaults to False.
 
         Returns:
             Dict[str, str]: GraphQL API (Twitter Web App API) アクセス用の HTTP リクエストヘッダー
         """
 
-        return self._graphql_api_headers
+        headers = self._graphql_api_headers.copy()
+
+        # クロスオリジン用に origin と referer を追加
+        # Twitter Web App から api.twitter.com にクロスオリジンリクエストを送信する際のヘッダーを模倣する
+        if cross_origin is True:
+            headers['origin'] = 'https://twitter.com'
+            headers['referer'] = 'https://twitter.com/'
+
+        return headers
 
 
     def logout(self) -> None:
         """
         ログアウト処理を行い、Twitter からセッションを切断する
         単に Cookie を削除するだけだと Twitter にセッションが残り続けてしまうため、今後ログインしない場合は明示的にこのメソッドを呼び出すこと
         このメソッドを呼び出した後は、取得した Cookie では再認証できなくなる
 
         Raises:
             tweepy.HTTPException: サーバーエラーなどの問題でログアウトに失敗した
             tweepy.TweepyException: ログアウト処理中にエラーが発生した
         """
 
         # ログアウト API 専用ヘッダー
-        ## self._auth_flow_api_headers と基本的には共通なため、コピーして変更箇所のみ変更する
-        logout_headers = self._auth_flow_api_headers.copy()
+        ## self._graphql_api_headers と基本共通で、content-type だけ application/x-www-form-urlencoded に変更
+        logout_headers = self._graphql_api_headers.copy()
         logout_headers['content-type'] = 'application/x-www-form-urlencoded'
-        del logout_headers['x-guest-token']
-        logout_headers['x-twitter-auth-type'] = 'OAuth2Session'
-        ## ヘッダーの dict をアルファベット順にソート
-        logout_headers = dict(sorted(logout_headers.items(), key=lambda x: x[0]))
 
         # ログアウト API にログアウトすることを伝える
         ## この API を実行すると、サーバー側でセッションが切断され、今まで持っていたほとんどの Cookie が消去される
         logout_api_response = self._session.post('https://api.twitter.com/1.1/account/logout.json', headers=logout_headers, data={
             'redirectAfterLogout': 'https://twitter.com/account/switch',
         })
         if logout_api_response.status_code != 200:
@@ -341,15 +339,14 @@
         """
 
         csrf_token = response.cookies.get('ct0')
         if csrf_token:
             if self._session.cookies.get('ct0') != csrf_token:
                 self._session.cookies.set('ct0', csrf_token, domain='.twitter.com')
             self._auth_flow_api_headers['x-csrf-token'] = csrf_token
-            self._tweetdeck_api_headers['x-csrf-token'] = csrf_token
             self._graphql_api_headers['x-csrf-token'] = csrf_token
             self._session.headers['x-csrf-token'] = csrf_token
 
 
     def _get_tweepy_exception(self, response: requests.Response) -> tweepy.TweepyException:
         """
         TweepyException を継承した、ステータスコードと一致する例外クラスを取得する
```

### Comparing `tweepy_authlib-1.3.1/.gitignore` & `tweepy_authlib-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.3.1/Readme.md` & `tweepy_authlib-1.4.0/Readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,33 @@
 # tweepy-authlib
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 
 > [!WARNING]  
 > **旧 TweetDeck の完全廃止にともない、2023/09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されています。**  
-> **2024/04/30 時点では、account/verify_credentials や upload.twitter.com 以下の API を除き大半の Twitter API v1.1 にアクセスできなくなっています。**  
-> 現在 tweepy-authlib を使いタイムライン取得 / ツイート検索 / ツイート送信機能などを実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。  
-> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、実装時の参考にしてください。
+> **2024/04/30 時点では、下記 API が既に廃止されています ([参考](https://github.com/dimdenGD/OldTweetDeck/blob/main/src/interception.js)) 。**  
+> 現時点では 2023/09 にサーバー負荷が高い API が一括廃止されて以降の動きはありません。ただし、リストにない API も既に廃止されている可能性があります。
+> - `search/tweets` : ツイート検索
+> - `search/universal` : ツイート検索 (旧 TweetDeck 独自 API)
+> - `statuses/update` : ツイート投稿
+> - `statuses/retweet/:id` : リツイート
+> - `statuses/unretweet/:id` : リツイート取り消し
+> - `statuses/show/:id` : ツイート詳細
+> - `statuses/destroy/:id` : ツイート削除
+> - `statuses/user_timeline` : ユーザータイムライン
+> - `users/search` : ユーザー検索
+>
+> **現在 tweepy-authlib を利用して上記機能を実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。**  
+> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、参考になれば幸いです。  
+> また現時点で廃止されていない API を利用したサンプルコードが [example_json.py](example_json.py) と [example_pickle.py](example_pickle.py) にありますので、そちらもご一読ください。
+
+> [!NOTE]  
+> **tweepy-authlib v1.4.0 以降では、より厳密に Twitter Web App からの HTTP リクエストに偽装したり、一部の Twitter API v1.1 に再びアクセスできるようになるなど、様々な改善が行われています！**  
+> 凍結やアカウントロックのリスクを下げるためにも、最新版の tweepy-authlib の利用をおすすめします。
 
 > [!IMPORTANT]  
 > 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
 > [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
@@ -72,27 +88,36 @@
 pip install tweepy-authlib
 ```
 
 ## Usage
 
 ### With JSON
 
+[example_json.py](example_json.py)
+
 ```python
-import json
+import dotenv
 import os
+import json
 import tweepy
 from pathlib import Path
+from pprint import pprint
 from requests.cookies import RequestsCookieJar
 from tweepy_authlib import CookieSessionUserHandler
 
 try:
     terminal_size = os.get_terminal_size().columns
 except OSError:
     terminal_size = 80
 
+# ユーザー名とパスワードを環境変数から取得
+dotenv.load_dotenv()
+screen_name = os.environ.get('TWITTER_SCREEN_NAME', 'your_screen_name')
+password = os.environ.get('TWITTER_PASSWORD', 'your_password')
+
 # 保存した Cookie を使って認証
 ## 毎回ログインすると不審なログインとして扱われる可能性が高くなるため、
 ## できるだけ以前認証した際に保存した Cookie を使って認証することを推奨
 if Path('cookie.json').exists():
 
     # 保存した Cookie を読み込む
     with open('cookie.json', 'r') as f:
@@ -108,61 +133,110 @@
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
     ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
     try:
-        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+        auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
     except tweepy.HTTPException as ex:
         # パスワードが間違っているなどの理由で認証に失敗した場合
         if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
             error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
         else:
             error_message = 'Unknown Error'
         raise Exception(f'Failed to authenticate with password ({error_message})')
     except tweepy.TweepyException as ex:
         # 認証フローの途中で予期せぬエラーが発生し、ログインに失敗した
         error_message = f'Message: {ex}'
         raise Exception(f'Unexpected error occurred while authenticate with password ({error_message})')
 
     # 現在のログインセッションの Cookie を取得
-    cookies = auth_handler.get_cookies()
+    cookies_dict = auth_handler.get_cookies_as_dict()
 
-    # Cookie を pickle 化して保存
+    # Cookie を JSON ファイルに保存
     with open('cookie.json', 'w') as f:
-        json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
+        json.dump(cookies_dict, f, ensure_ascii=False, indent=4)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
+
+print('=' * terminal_size)
+print('Logged in user:')
+print('-' * terminal_size)
+user = api.verify_credentials()
+assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
+pprint(user._json)
+print('=' * terminal_size)
+
+print('Followers (3 users):')
+print('-' * terminal_size)
+followers = user.followers(count=3)
+for follower in followers:
+    pprint(follower._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Following (3 users):')
+print('-' * terminal_size)
+friends = user.friends(count=3)
+for friend in friends:
+    pprint(friend._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Home timeline (3 tweets):')
 print('-' * terminal_size)
-print(api.verify_credentials())
+home_timeline = api.home_timeline(count=3)
+for status in home_timeline:
+    pprint(status._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+tweet_id = home_timeline[0].id
+print('Like tweet:')
+print('-' * terminal_size)
+pprint(api.create_favorite(tweet_id)._json)
+print('=' * terminal_size)
+
+print('Unlike tweet:')
 print('-' * terminal_size)
+pprint(api.destroy_favorite(tweet_id)._json)
+print('=' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
-## ログアウト後は、取得した Cookie では再認証できなくなる
-#auth_handler.logout()
-#os.unlink('cookie.json')
+## ログアウト後は、取得した Cookie は再利用できなくなる
+auth_handler.logout()
+os.unlink('cookie.json')
 ```
 
 ### With Pickle
 
+[example_pickle.py](example_pickle.py)
+
 ```python
+import dotenv
 import os
 import pickle
 import tweepy
 from pathlib import Path
+from pprint import pprint
 from tweepy_authlib import CookieSessionUserHandler
 
 try:
     terminal_size = os.get_terminal_size().columns
 except OSError:
     terminal_size = 80
 
+# ユーザー名とパスワードを環境変数から取得
+dotenv.load_dotenv()
+screen_name = os.environ.get('TWITTER_SCREEN_NAME', 'your_screen_name')
+password = os.environ.get('TWITTER_PASSWORD', 'your_password')
+
 # 保存した Cookie を使って認証
 ## 毎回ログインすると不審なログインとして扱われる可能性が高くなるため、
 ## できるだけ以前認証した際に保存した Cookie を使って認証することを推奨
 if Path('cookie.pickle').exists():
 
     # 保存した Cookie を読み込む
     with open('cookie.pickle', 'rb') as f:
@@ -173,15 +247,15 @@
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
     ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
     try:
-        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+        auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
     except tweepy.HTTPException as ex:
         # パスワードが間違っているなどの理由で認証に失敗した場合
         if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
             error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
         else:
             error_message = 'Unknown Error'
         raise Exception(f'Failed to authenticate with password ({error_message})')
@@ -195,21 +269,61 @@
 
     # Cookie を pickle 化して保存
     with open('cookie.pickle', 'wb') as f:
         pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
+
+print('=' * terminal_size)
+print('Logged in user:')
+print('-' * terminal_size)
+user = api.verify_credentials()
+assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
+pprint(user._json)
+print('=' * terminal_size)
+
+print('Followers (3 users):')
 print('-' * terminal_size)
-print(api.verify_credentials())
+followers = user.followers(count=3)
+for follower in followers:
+    pprint(follower._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Following (3 users):')
+print('-' * terminal_size)
+friends = user.friends(count=3)
+for friend in friends:
+    pprint(friend._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Home timeline (3 tweets):')
+print('-' * terminal_size)
+home_timeline = api.home_timeline(count=3)
+for status in home_timeline:
+    pprint(status._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+tweet_id = home_timeline[0].id
+print('Like tweet:')
+print('-' * terminal_size)
+pprint(api.create_favorite(tweet_id)._json)
+print('=' * terminal_size)
+
+print('Unlike tweet:')
 print('-' * terminal_size)
+pprint(api.destroy_favorite(tweet_id)._json)
+print('=' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
-## ログアウト後は、取得した Cookie では再認証できなくなる
-#auth_handler.logout()
-#os.unlink('cookie.pickle')
+## ログアウト後は、取得した Cookie は再利用できなくなる
+auth_handler.logout()
+os.unlink('cookie.pickle')
 ```
 
 ## License
 
 [MIT License](License.txt)
```

### Comparing `tweepy_authlib-1.3.1/pyproject.toml` & `tweepy_authlib-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.3.1/PKG-INFO` & `tweepy_authlib-1.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tweepy-authlib
-Version: 1.3.1
+Version: 1.4.0
 Summary: Twitter Web App (Web 版公式クライアント) の内部 API を使い、Tweepy でスクリーンネームとパスワードで認証するためのライブラリ
 Project-URL: Documentation, https://github.com/tsukumijima/tweepy-authlib
 Project-URL: Issues, https://github.com/tsukumijima/tweepy-authlib/issues
 Project-URL: Source, https://github.com/tsukumijima/tweepy-authlib
 Author: tsukumi
 License-Expression: MIT
 Keywords: Library,Tweepy,Twitter
@@ -29,17 +29,33 @@
 # tweepy-authlib
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 
 > [!WARNING]  
 > **旧 TweetDeck の完全廃止にともない、2023/09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されています。**  
-> **2024/04/30 時点では、account/verify_credentials や upload.twitter.com 以下の API を除き大半の Twitter API v1.1 にアクセスできなくなっています。**  
-> 現在 tweepy-authlib を使いタイムライン取得 / ツイート検索 / ツイート送信機能などを実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。  
-> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、実装時の参考にしてください。
+> **2024/04/30 時点では、下記 API が既に廃止されています ([参考](https://github.com/dimdenGD/OldTweetDeck/blob/main/src/interception.js)) 。**  
+> 現時点では 2023/09 にサーバー負荷が高い API が一括廃止されて以降の動きはありません。ただし、リストにない API も既に廃止されている可能性があります。
+> - `search/tweets` : ツイート検索
+> - `search/universal` : ツイート検索 (旧 TweetDeck 独自 API)
+> - `statuses/update` : ツイート投稿
+> - `statuses/retweet/:id` : リツイート
+> - `statuses/unretweet/:id` : リツイート取り消し
+> - `statuses/show/:id` : ツイート詳細
+> - `statuses/destroy/:id` : ツイート削除
+> - `statuses/user_timeline` : ユーザータイムライン
+> - `users/search` : ユーザー検索
+>
+> **現在 tweepy-authlib を利用して上記機能を実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。**  
+> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、参考になれば幸いです。  
+> また現時点で廃止されていない API を利用したサンプルコードが [example_json.py](example_json.py) と [example_pickle.py](example_pickle.py) にありますので、そちらもご一読ください。
+
+> [!NOTE]  
+> **tweepy-authlib v1.4.0 以降では、より厳密に Twitter Web App からの HTTP リクエストに偽装したり、一部の Twitter API v1.1 に再びアクセスできるようになるなど、様々な改善が行われています！**  
+> 凍結やアカウントロックのリスクを下げるためにも、最新版の tweepy-authlib の利用をおすすめします。
 
 > [!IMPORTANT]  
 > 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
 > [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
@@ -99,27 +115,36 @@
 pip install tweepy-authlib
 ```
 
 ## Usage
 
 ### With JSON
 
+[example_json.py](example_json.py)
+
 ```python
-import json
+import dotenv
 import os
+import json
 import tweepy
 from pathlib import Path
+from pprint import pprint
 from requests.cookies import RequestsCookieJar
 from tweepy_authlib import CookieSessionUserHandler
 
 try:
     terminal_size = os.get_terminal_size().columns
 except OSError:
     terminal_size = 80
 
+# ユーザー名とパスワードを環境変数から取得
+dotenv.load_dotenv()
+screen_name = os.environ.get('TWITTER_SCREEN_NAME', 'your_screen_name')
+password = os.environ.get('TWITTER_PASSWORD', 'your_password')
+
 # 保存した Cookie を使って認証
 ## 毎回ログインすると不審なログインとして扱われる可能性が高くなるため、
 ## できるだけ以前認証した際に保存した Cookie を使って認証することを推奨
 if Path('cookie.json').exists():
 
     # 保存した Cookie を読み込む
     with open('cookie.json', 'r') as f:
@@ -135,61 +160,110 @@
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
     ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
     try:
-        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+        auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
     except tweepy.HTTPException as ex:
         # パスワードが間違っているなどの理由で認証に失敗した場合
         if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
             error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
         else:
             error_message = 'Unknown Error'
         raise Exception(f'Failed to authenticate with password ({error_message})')
     except tweepy.TweepyException as ex:
         # 認証フローの途中で予期せぬエラーが発生し、ログインに失敗した
         error_message = f'Message: {ex}'
         raise Exception(f'Unexpected error occurred while authenticate with password ({error_message})')
 
     # 現在のログインセッションの Cookie を取得
-    cookies = auth_handler.get_cookies()
+    cookies_dict = auth_handler.get_cookies_as_dict()
 
-    # Cookie を pickle 化して保存
+    # Cookie を JSON ファイルに保存
     with open('cookie.json', 'w') as f:
-        json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
+        json.dump(cookies_dict, f, ensure_ascii=False, indent=4)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
+
+print('=' * terminal_size)
+print('Logged in user:')
+print('-' * terminal_size)
+user = api.verify_credentials()
+assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
+pprint(user._json)
+print('=' * terminal_size)
+
+print('Followers (3 users):')
+print('-' * terminal_size)
+followers = user.followers(count=3)
+for follower in followers:
+    pprint(follower._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Following (3 users):')
+print('-' * terminal_size)
+friends = user.friends(count=3)
+for friend in friends:
+    pprint(friend._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Home timeline (3 tweets):')
 print('-' * terminal_size)
-print(api.verify_credentials())
+home_timeline = api.home_timeline(count=3)
+for status in home_timeline:
+    pprint(status._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+tweet_id = home_timeline[0].id
+print('Like tweet:')
+print('-' * terminal_size)
+pprint(api.create_favorite(tweet_id)._json)
+print('=' * terminal_size)
+
+print('Unlike tweet:')
 print('-' * terminal_size)
+pprint(api.destroy_favorite(tweet_id)._json)
+print('=' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
-## ログアウト後は、取得した Cookie では再認証できなくなる
-#auth_handler.logout()
-#os.unlink('cookie.json')
+## ログアウト後は、取得した Cookie は再利用できなくなる
+auth_handler.logout()
+os.unlink('cookie.json')
 ```
 
 ### With Pickle
 
+[example_pickle.py](example_pickle.py)
+
 ```python
+import dotenv
 import os
 import pickle
 import tweepy
 from pathlib import Path
+from pprint import pprint
 from tweepy_authlib import CookieSessionUserHandler
 
 try:
     terminal_size = os.get_terminal_size().columns
 except OSError:
     terminal_size = 80
 
+# ユーザー名とパスワードを環境変数から取得
+dotenv.load_dotenv()
+screen_name = os.environ.get('TWITTER_SCREEN_NAME', 'your_screen_name')
+password = os.environ.get('TWITTER_PASSWORD', 'your_password')
+
 # 保存した Cookie を使って認証
 ## 毎回ログインすると不審なログインとして扱われる可能性が高くなるため、
 ## できるだけ以前認証した際に保存した Cookie を使って認証することを推奨
 if Path('cookie.pickle').exists():
 
     # 保存した Cookie を読み込む
     with open('cookie.pickle', 'rb') as f:
@@ -200,15 +274,15 @@
 
 # スクリーンネームとパスワードを指定して認証
 else:
 
     # スクリーンネームとパスワードを渡す
     ## スクリーンネームとパスワードを指定する場合は初期化時に認証のための API リクエストが多数行われるため、完了まで数秒かかる
     try:
-        auth_handler = CookieSessionUserHandler(screen_name='your_screen_name', password='your_password')
+        auth_handler = CookieSessionUserHandler(screen_name=screen_name, password=password)
     except tweepy.HTTPException as ex:
         # パスワードが間違っているなどの理由で認証に失敗した場合
         if len(ex.api_codes) > 0 and len(ex.api_messages) > 0:
             error_message = f'Code: {ex.api_codes[0]}, Message: {ex.api_messages[0]}'
         else:
             error_message = 'Unknown Error'
         raise Exception(f'Failed to authenticate with password ({error_message})')
@@ -222,21 +296,61 @@
 
     # Cookie を pickle 化して保存
     with open('cookie.pickle', 'wb') as f:
         pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
+
+print('=' * terminal_size)
+print('Logged in user:')
+print('-' * terminal_size)
+user = api.verify_credentials()
+assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
+pprint(user._json)
+print('=' * terminal_size)
+
+print('Followers (3 users):')
 print('-' * terminal_size)
-print(api.verify_credentials())
+followers = user.followers(count=3)
+for follower in followers:
+    pprint(follower._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Following (3 users):')
+print('-' * terminal_size)
+friends = user.friends(count=3)
+for friend in friends:
+    pprint(friend._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+print('Home timeline (3 tweets):')
+print('-' * terminal_size)
+home_timeline = api.home_timeline(count=3)
+for status in home_timeline:
+    pprint(status._json)
+    print('-' * terminal_size)
+print('=' * terminal_size)
+
+tweet_id = home_timeline[0].id
+print('Like tweet:')
+print('-' * terminal_size)
+pprint(api.create_favorite(tweet_id)._json)
+print('=' * terminal_size)
+
+print('Unlike tweet:')
 print('-' * terminal_size)
+pprint(api.destroy_favorite(tweet_id)._json)
+print('=' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
-## ログアウト後は、取得した Cookie では再認証できなくなる
-#auth_handler.logout()
-#os.unlink('cookie.pickle')
+## ログアウト後は、取得した Cookie は再利用できなくなる
+auth_handler.logout()
+os.unlink('cookie.pickle')
 ```
 
 ## License
 
 [MIT License](License.txt)
```

