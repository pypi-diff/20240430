# Comparing `tmp/tweepy_authlib-1.3.0.tar.gz` & `tmp/tweepy_authlib-1.3.1.tar.gz`

## Comparing `tweepy_authlib-1.3.0.tar` & `tweepy_authlib-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/.editorconfig
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/.env.example
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/example_json.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/example_pickle.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/tests/test_main.py
--rw-r--r--   0        0        0    33768 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/tweepy_authlib/CookieSessionUserHandler.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/tweepy_authlib/__about__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/tweepy_authlib/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/License.txt
--rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/Readme.md
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.editorconfig
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.env.example
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/License.txt
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/example_json.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/example_pickle.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tests/test_main.py
+-rw-r--r--   0        0        0    33475 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/CookieSessionUserHandler.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/__about__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/tweepy_authlib/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/.gitignore
+-rw-r--r--   0        0        0    12308 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/Readme.md
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 tweepy_authlib-1.3.1/PKG-INFO
```

### Comparing `tweepy_authlib-1.3.0/example_json.py` & `tweepy_authlib-1.3.1/example_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,13 @@
         json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.json')
```

### Comparing `tweepy_authlib-1.3.0/example_pickle.py` & `tweepy_authlib-1.3.1/example_pickle.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,13 @@
         pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.pickle')
```

### Comparing `tweepy_authlib-1.3.0/tests/test_main.py` & `tweepy_authlib-1.3.1/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         api = tweepy.API(auth_handler)
         user = api.verify_credentials()
         print('-' * terminal_size)
         print(user)
         print('-' * terminal_size)
         assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
         # assert api.user_timeline(screen_name='elonmusk')[0].user.screen_name == 'elonmusk'
-        api.home_timeline()
+        # api.home_timeline()
         with open('cookie.pickle', 'wb') as f:
             pickle.dump(auth_handler.get_cookies(), f)
     else:
         pytest.skip('TWITTER_SCREEN_NAME or TWITTER_PASSWORD is not set.')
 
 def test_07(tweet: bool = False):
 
@@ -71,15 +71,15 @@
         #     print('-' * terminal_size)
         #     print(api.update_status(f'Hello, Twitter! (API Test Tweet, {datetime.datetime.now().strftime("%Y/%m/%d %H:%M:%S")})'))
         print('-' * terminal_size)
         print(user)
         print('-' * terminal_size)
         assert user.screen_name == os.environ['TWITTER_SCREEN_NAME']
         # assert api.user_timeline(screen_name='elonmusk')[0].user.screen_name == 'elonmusk'
-        api.home_timeline()
+        # api.home_timeline()
         auth_handler.logout()
     else:
         pytest.skip('TWITTER_SCREEN_NAME or TWITTER_PASSWORD is not set.')
 
 
 if __name__ == '__main__':
     dotenv.load_dotenv()
```

### Comparing `tweepy_authlib-1.3.0/tweepy_authlib/CookieSessionUserHandler.py` & `tweepy_authlib-1.3.1/tweepy_authlib/CookieSessionUserHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,20 +544,19 @@
         self._auth_flow_api_headers['x-guest-token'] = self._session.cookies.get('gt')
 
         # これ以降は基本認証フロー API へのアクセスしか行わないので、セッションのヘッダーを認証フロー API 用のものに差し替える
         self._session.headers.clear()
         self._session.headers.update(self._auth_flow_api_headers)
 
         # 極力公式の Twitter Web App に偽装するためのダミーリクエスト
-        ## https://api.twitter.com/1.1/attribution/event.json に関してはもしかすると意味があるかも
-        self._session.get('https://api.twitter.com/1.1/hashflags.json',)
-        self._session.post('https://api.twitter.com/1.1/attribution/event.json', json={'event': 'open'})
+        self._session.get('https://api.twitter.com/1.1/hashflags.json')
 
         # https://api.twitter.com/1.1/onboarding/task.json?task=login に POST して認証フローを開始
         ## 認証フローを開始するには、Cookie に "ct0" と "gt" がセットされている必要がある
+        ## 2024年4月時点の Twitter Web App が送信する JSON パラメータを模倣している
         flow_01_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json?flow_name=login', json={
             'input_flow_data': {
                 'flow_context': {
                     'debug_overrides': {},
                     'start_location': {
                         'location': 'manual_link',
                     }
@@ -606,17 +605,14 @@
                 'wait_spinner': 3,
                 'web_modal': 1,
             }
         })
         if flow_01_response.status_code != 200:
             raise self._get_tweepy_exception(flow_01_response)
 
-        # 極力公式の Twitter Web App に偽装するためのダミーリクエスト
-        self._session.post('https://api.twitter.com/1.1/branch/init.json', json={})
-
         # js_inst (難読化された JavaScript で、これの実行結果を認証フローに送信する必要があるらしい) を取得
         js_inst_response = self._session.get('https://twitter.com/i/js_inst?c_name=ui_metrics', headers=self._js_headers)
         if js_inst_response.status_code != 200:
             raise tweepy.TweepyException('Failed to get js_inst')
 
         # js_inst の JavaScript を実行し、ui_metrics オブジェクトを取得
         ui_metrics = self._get_ui_metrics(js_inst_response.text)
```

### Comparing `tweepy_authlib-1.3.0/.gitignore` & `tweepy_authlib-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.3.0/License.txt` & `tweepy_authlib-1.3.1/License.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2023 tsukumi
+Copyright (c) 2023-2024 tsukumi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tweepy_authlib-1.3.0/Readme.md` & `tweepy_authlib-1.3.1/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
 # tweepy-authlib
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 
-> **Warning**  
-> **旧 TweetDeck の完全廃止にともない、09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されてしまいました。**  
-> このため、**v1.1.0 以前の TweetDeck の Bearer トークンを使い API v1.1 にアクセスする実装が動作しなくなっています。**  
-> **これに伴い、Bearer トークンに代わりに Twitter Web App の Bearer トークンを利用するように変更した、v1.2.0 をリリースしました。**  
-> statuses/update を含めた主にツイート系の API v1.1 にすでにアクセスできない状態で、今後も段階的にアクセスできなくなる API が増えていくと思われます。  
-> 09/14 時点では home_timeline や verify_credentials などの一部 API には今まで通りの方法で tweepy と tweepy-authlib を使いアクセスできますが、今後はそれらの API にもアクセスできなくなる可能性があります。
+> [!WARNING]  
+> **旧 TweetDeck の完全廃止にともない、2023/09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されています。**  
+> **2024/04/30 時点では、account/verify_credentials や upload.twitter.com 以下の API を除き大半の Twitter API v1.1 にアクセスできなくなっています。**  
+> 現在 tweepy-authlib を使いタイムライン取得 / ツイート検索 / ツイート送信機能などを実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。  
+> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、実装時の参考にしてください。
+
+> [!IMPORTANT]  
+> 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
+> [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
 **Table of Contents**
 
 - [tweepy-authlib](#tweepy-authlib)
   - [Description](#description)
@@ -26,44 +29,42 @@
 ## Description
 
 Twitter Web App (Web 版公式クライアント) の内部 API を使い、[Tweepy](https://github.com/tweepy/tweepy) でスクリーンネームとパスワードで認証するためのライブラリです。
 
 スクリーンネーム (ex: `@elonmusk`) とパスワードを指定して認証し、取得した Cookie などの認証情報で Twitter API v1.1 にアクセスできます。  
 毎回ログインしていては面倒 & 不審なアクセス扱いされそうなので、Cookie をファイルなどに保存し、次回以降はその Cookie を使ってログインする機能もあります。
 
-Tweepy を利用しているソースコードのうち、認証部分 (`tweepy.auth.OAuth1UserHandler`) を `tweepy_authlib.CookieSessionUserHandler` に置き換えるだけで、かんたんに Cookie ベースの認証に変更できます！
-
-Twitter API の有料化に伴って通常の OAuth API が利用できなくなった場合も、この `CookieSessionUserHandler` を使えば引き続き Twitter API v1.1 にアクセスできるはず…！  
+Tweepy を利用しているソースコードのうち、認証部分 (`tweepy.auth.OAuth1UserHandler`) を `tweepy_authlib.CookieSessionUserHandler` に置き換えるだけで、かんたんに Cookie ベースの認証に変更できます！  
 認証部分以外は OAuth API のときの実装がそのまま使えるので、ソースコードの変更も最小限に抑えられます。
 
-> **Note**  
+> [!NOTE]  
 > OAuth API と公式クライアント用の内部 API がほぼ共通だった v1.1 とは異なり、v2 では OAuth API と公式クライアント用の内部 API が大きく異なります。  
 > そのため、`CookieSessionUserHandler` は Twitter API v2 には対応していません。  
 > また、今のところ2段階認証にも対応していません (2段階認証に関しては技術的には実装可能だが、確認コードの送信周りの実装が面倒…) 。
 
 認証フローはブラウザ上で動作する Web 版公式クライアントの API アクセス動作や HTTP リクエストヘッダーを可能な限りエミュレートしています。  
 ブラウザから抽出した Web 版公式クライアントのログイン済み Cookie を使うことでも認証が可能です。
 
-> **Note**  
+> [!NOTE]  
 > ブラウザから Cookie を抽出する場合、(不審なアクセス扱いされないために) できればすべての Cookie を抽出することが望ましいですが、実装上は Cookie 内の `auth_token` と `ct0` の2つの値だけあれば認証できます。  
 > なお、ブラウザから取得した Cookie は事前に `requests.cookies.RequestsCookieJar` に変換してください。
 
 さらに API アクセス時は TweetDeck の HTTP リクエスト (Twitter API v1.1) をエミュレートしているため、レートリミットなどの制限は TweetDeck と同一です。  
 
-> **Note**  
+> [!NOTE]  
 > `CookieSessionUserHandler` で取得した認証情報を使うと、TweetDeck でしか利用できない search/universal などの内部 API にもアクセスできるようになります。  
 > ただし、Tweepy はそうした内部 API をサポートしていないため、アクセスするには独自に `tweepy.API.request()` で HTTP リクエストを送る必要があります。
 
-> **Warning**  
+> [!WARNING]  
 > このライブラリは、非公式かつ内部的な API をリバースエンジニアリングし、ブラウザとほぼ同じように API アクセスを行うことで、本来 Web 版公式クライアントでしか利用できない Cookie 認証での Twitter API v1.1 へのアクセスを可能にしています。  
 > 可能な限りブラウザの挙動を模倣することでできるだけ Twitter 側に怪しまれないような実装を行っていますが、非公式な方法ゆえ、**このライブラリを利用して Twitter API にアクセスすると、最悪アカウント凍結やシャドウバンなどの制限が適用される可能性もあります。**  
 > また、**Twitter API の仕様変更により、このライブラリが突然動作しなくなることも考えられます。**  
 > このライブラリを利用して API アクセスを行うことによって生じたいかなる損害についても、著者は一切の責任を負いません。利用にあたっては十分ご注意ください。
 
-> **Warning**  
+> [!WARNING]  
 > **スクリーンネームとパスワードを指定して認証する際は、できるだけログイン実績のある IP アドレスでの実行をおすすめします。**  
 > このライブラリでの認証は、Web 版公式クライアントのログインと同じように行われるため、ログイン実績のない IP アドレスから認証すると、不審なログインとして扱われてしまう可能性があります。  
 > また、実行毎に毎回認証を行うと、不審なログインとして扱われてしまう可能性が高くなります。  
 > **初回の認証以降では、以前認証した際に保存した Cookie を使って認証することを強く推奨します。**
 
 ## Installation
 
@@ -132,16 +133,14 @@
         json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.json')
 ```
@@ -199,16 +198,14 @@
         pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.pickle')
 ```
```

### Comparing `tweepy_authlib-1.3.0/pyproject.toml` & `tweepy_authlib-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.3.0/PKG-INFO` & `tweepy_authlib-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tweepy-authlib
-Version: 1.3.0
+Version: 1.3.1
 Summary: Twitter Web App (Web 版公式クライアント) の内部 API を使い、Tweepy でスクリーンネームとパスワードで認証するためのライブラリ
 Project-URL: Documentation, https://github.com/tsukumijima/tweepy-authlib
 Project-URL: Issues, https://github.com/tsukumijima/tweepy-authlib/issues
 Project-URL: Source, https://github.com/tsukumijima/tweepy-authlib
 Author: tsukumi
 License-Expression: MIT
-License-File: License.txt
 Keywords: Library,Tweepy,Twitter
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python
@@ -28,20 +27,23 @@
 
 
 # tweepy-authlib
 
 [![PyPI - Version](https://img.shields.io/pypi/v/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tweepy-authlib.svg)](https://pypi.org/project/tweepy-authlib)
 
-> **Warning**  
-> **旧 TweetDeck の完全廃止にともない、09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されてしまいました。**  
-> このため、**v1.1.0 以前の TweetDeck の Bearer トークンを使い API v1.1 にアクセスする実装が動作しなくなっています。**  
-> **これに伴い、Bearer トークンに代わりに Twitter Web App の Bearer トークンを利用するように変更した、v1.2.0 をリリースしました。**  
-> statuses/update を含めた主にツイート系の API v1.1 にすでにアクセスできない状態で、今後も段階的にアクセスできなくなる API が増えていくと思われます。  
-> 09/14 時点では home_timeline や verify_credentials などの一部 API には今まで通りの方法で tweepy と tweepy-authlib を使いアクセスできますが、今後はそれらの API にもアクセスできなくなる可能性があります。
+> [!WARNING]  
+> **旧 TweetDeck の完全廃止にともない、2023/09/14 頃から内部的に残存していた Twitter API v1.1 の段階的なシャットダウンが開始されています。**  
+> **2024/04/30 時点では、account/verify_credentials や upload.twitter.com 以下の API を除き大半の Twitter API v1.1 にアクセスできなくなっています。**  
+> 現在 tweepy-authlib を使いタイムライン取得 / ツイート検索 / ツイート送信機能などを実装するには、別途 GraphQL API (Twitter Web App の内部 API) クライアントを自作する必要があります。  
+> 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、実装時の参考にしてください。
+
+> [!IMPORTANT]  
+> 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
+> [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
 **Table of Contents**
 
 - [tweepy-authlib](#tweepy-authlib)
   - [Description](#description)
@@ -54,44 +56,42 @@
 ## Description
 
 Twitter Web App (Web 版公式クライアント) の内部 API を使い、[Tweepy](https://github.com/tweepy/tweepy) でスクリーンネームとパスワードで認証するためのライブラリです。
 
 スクリーンネーム (ex: `@elonmusk`) とパスワードを指定して認証し、取得した Cookie などの認証情報で Twitter API v1.1 にアクセスできます。  
 毎回ログインしていては面倒 & 不審なアクセス扱いされそうなので、Cookie をファイルなどに保存し、次回以降はその Cookie を使ってログインする機能もあります。
 
-Tweepy を利用しているソースコードのうち、認証部分 (`tweepy.auth.OAuth1UserHandler`) を `tweepy_authlib.CookieSessionUserHandler` に置き換えるだけで、かんたんに Cookie ベースの認証に変更できます！
-
-Twitter API の有料化に伴って通常の OAuth API が利用できなくなった場合も、この `CookieSessionUserHandler` を使えば引き続き Twitter API v1.1 にアクセスできるはず…！  
+Tweepy を利用しているソースコードのうち、認証部分 (`tweepy.auth.OAuth1UserHandler`) を `tweepy_authlib.CookieSessionUserHandler` に置き換えるだけで、かんたんに Cookie ベースの認証に変更できます！  
 認証部分以外は OAuth API のときの実装がそのまま使えるので、ソースコードの変更も最小限に抑えられます。
 
-> **Note**  
+> [!NOTE]  
 > OAuth API と公式クライアント用の内部 API がほぼ共通だった v1.1 とは異なり、v2 では OAuth API と公式クライアント用の内部 API が大きく異なります。  
 > そのため、`CookieSessionUserHandler` は Twitter API v2 には対応していません。  
 > また、今のところ2段階認証にも対応していません (2段階認証に関しては技術的には実装可能だが、確認コードの送信周りの実装が面倒…) 。
 
 認証フローはブラウザ上で動作する Web 版公式クライアントの API アクセス動作や HTTP リクエストヘッダーを可能な限りエミュレートしています。  
 ブラウザから抽出した Web 版公式クライアントのログイン済み Cookie を使うことでも認証が可能です。
 
-> **Note**  
+> [!NOTE]  
 > ブラウザから Cookie を抽出する場合、(不審なアクセス扱いされないために) できればすべての Cookie を抽出することが望ましいですが、実装上は Cookie 内の `auth_token` と `ct0` の2つの値だけあれば認証できます。  
 > なお、ブラウザから取得した Cookie は事前に `requests.cookies.RequestsCookieJar` に変換してください。
 
 さらに API アクセス時は TweetDeck の HTTP リクエスト (Twitter API v1.1) をエミュレートしているため、レートリミットなどの制限は TweetDeck と同一です。  
 
-> **Note**  
+> [!NOTE]  
 > `CookieSessionUserHandler` で取得した認証情報を使うと、TweetDeck でしか利用できない search/universal などの内部 API にもアクセスできるようになります。  
 > ただし、Tweepy はそうした内部 API をサポートしていないため、アクセスするには独自に `tweepy.API.request()` で HTTP リクエストを送る必要があります。
 
-> **Warning**  
+> [!WARNING]  
 > このライブラリは、非公式かつ内部的な API をリバースエンジニアリングし、ブラウザとほぼ同じように API アクセスを行うことで、本来 Web 版公式クライアントでしか利用できない Cookie 認証での Twitter API v1.1 へのアクセスを可能にしています。  
 > 可能な限りブラウザの挙動を模倣することでできるだけ Twitter 側に怪しまれないような実装を行っていますが、非公式な方法ゆえ、**このライブラリを利用して Twitter API にアクセスすると、最悪アカウント凍結やシャドウバンなどの制限が適用される可能性もあります。**  
 > また、**Twitter API の仕様変更により、このライブラリが突然動作しなくなることも考えられます。**  
 > このライブラリを利用して API アクセスを行うことによって生じたいかなる損害についても、著者は一切の責任を負いません。利用にあたっては十分ご注意ください。
 
-> **Warning**  
+> [!WARNING]  
 > **スクリーンネームとパスワードを指定して認証する際は、できるだけログイン実績のある IP アドレスでの実行をおすすめします。**  
 > このライブラリでの認証は、Web 版公式クライアントのログインと同じように行われるため、ログイン実績のない IP アドレスから認証すると、不審なログインとして扱われてしまう可能性があります。  
 > また、実行毎に毎回認証を行うと、不審なログインとして扱われてしまう可能性が高くなります。  
 > **初回の認証以降では、以前認証した際に保存した Cookie を使って認証することを強く推奨します。**
 
 ## Installation
 
@@ -160,16 +160,14 @@
         json.dump(cookies.get_dict(), f, ensure_ascii=False, indent=4)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.json')
 ```
@@ -227,16 +225,14 @@
         pickle.dump(cookies, f)
 
 # Tweepy で Twitter API v1.1 にアクセス
 api = tweepy.API(auth_handler)
 print('-' * terminal_size)
 print(api.verify_credentials())
 print('-' * terminal_size)
-print(api.home_timeline())
-print('-' * terminal_size)
 
 # 継続してログインしない場合は明示的にログアウト
 ## 単に Cookie を消去するだけだと Twitter にセッションが残り続けてしまう
 ## ログアウト後は、取得した Cookie では再認証できなくなる
 #auth_handler.logout()
 #os.unlink('cookie.pickle')
 ```
```

