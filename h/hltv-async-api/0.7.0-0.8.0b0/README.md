# Comparing `tmp/hltv_async_api-0.7.0.tar.gz` & `tmp/hltv_async_api-0.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.7.0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.8.0b0.tar", max compression
```

## Comparing `hltv_async_api-0.7.0.tar` & `hltv_async_api-0.8.0b0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      124 2024-04-23 19:31:20.254506 hltv_async_api-0.7.0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    42132 2024-04-23 19:29:37.150858 hltv_async_api-0.7.0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.7.0/LICENSE
--rw-r--r--   0        0        0      639 2024-04-23 19:31:20.262384 hltv_async_api-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    15333 2024-04-23 18:10:26.740670 hltv_async_api-0.7.0/README.md
--rw-r--r--   0        0        0    15834 1970-01-01 00:00:00.000000 hltv_async_api-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-30 11:24:20.003853 hltv_async_api-0.8.0b0/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    45823 2024-04-30 11:12:31.459993 hltv_async_api-0.8.0b0/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     4159 2024-04-30 11:02:43.900064 hltv_async_api-0.8.0b0/hltv_async_api/unreleased.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.8.0b0/LICENSE
+-rw-r--r--   0        0        0      640 2024-04-30 11:24:19.991583 hltv_async_api-0.8.0b0/pyproject.toml
+-rw-r--r--   0        0        0    16049 2024-04-30 11:23:03.942665 hltv_async_api-0.8.0b0/README.md
+-rw-r--r--   0        0        0    16539 1970-01-01 00:00:00.000000 hltv_async_api-0.8.0b0/PKG-INFO
```

### Comparing `hltv_async_api-0.7.0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.8.0b0/hltv_async_api/aiohltv.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                  timeout: int = 5,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
                  delete_proxy: bool = False,
-                 tz: str = 'Europe/Copenhagen',
+                 tz: str | None = None,
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "Europe/Copenhagen"
         }
         self.DEBUG = debug
@@ -32,15 +32,15 @@
         self.logger = logging.getLogger(__name__)
 
         self.MAX_DELAY = max_delay
         self.timeout = timeout
         self.max_retries = max_retries
 
         self.TIMEZONE = tz
-        self._check_tz()
+        self._init_tz(tz)
 
         self.PROXY_PATH = proxy_path
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
         self.PROXY_ONCE = delete_proxy
 
         if self.PROXY_PATH:
@@ -55,21 +55,21 @@
         else:
             self.USE_PROXY = False
 
         self.session = None
         self.loop = asyncio.get_running_loop()
 
     async def __aenter__(self):
-        await self._create_session()
+        self._create_session()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
-    async def _create_session(self):
+    def _create_session(self):
         if not self.session:
             self.logger.debug('Creating Session')
             self.session = ClientSession()
 
     async def close(self):
         if self.session:
             self.logger.debug('Closing Session')
@@ -103,28 +103,29 @@
             self.max_retries = max_retries
         if proxy_protocol:
             self.PROXY_PROTOCOL = proxy_protocol
         if delete_proxy is not None:
             self.PROXY_ONCE = delete_proxy
         if tz is not None:
             self.TIMEZONE = tz
-            self._check_tz()
+            self._init_tz()
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
-    def _check_tz(self):
-        try:
-            pytz.timezone(self.TIMEZONE)
-        except pytz.exceptions.UnknownTimeZoneError:
-            self.logger.error('UnknownTimeZoneError, using default timezone: Europe/Copenhagen')
-            self.TIMEZONE = 'Europe/Copenhagen'
+    def _init_tz(self, tz: str | None = None):
+        if tz:
+            try:
+                pytz.timezone(self.TIMEZONE)
+            except pytz.exceptions.UnknownTimeZoneError:
+                self.logger.error('UnknownTimeZoneError, Using default timezone: Europe/Copenhagen')
+                self.TIMEZONE = None
 
     def _get_proxy(self):
         proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
             proxy = self.PROXY_PROTOCOL + '://' + proxy
 
@@ -170,38 +171,35 @@
             proxy = self._get_proxy()
         else:
             # delay, only for non-proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
             async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
-                if response.status == 403 or response.status == 404:
-                    self.logger.debug("Got 403 forbitten")
-                    return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
-                    #return False, self._parse_error_handler(delay)
-
-                # checking for challenge page.
-                result = await response.text()
-                page = await self.loop.run_in_executor(None, partial(self._f, result))
-                forbitten = await self.loop.run_in_executor(None, partial(self._cloudflare_check, page))
-                #forbitten, parsed = self._cloudflare_check(result)
-                if forbitten:
-                    return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
-                    #return False, self._parse_error_handler(delay)
+                if response.status == 200:
+                    result = await response.text()
+                    page = await self.loop.run_in_executor(None, partial(self._f, result))
+                    forbitten = await self.loop.run_in_executor(None, partial(self._cloudflare_check, page))
+
+                    if forbitten:
+                        return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
+                    return True, page
+
+                self.logger.debug(f"Error, Code {response.status=}")
+                return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
 
-                return True, page
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError, ClientTimeout) as e:
             self.logger.debug(e)
             delay = self._parse_error_handler(delay)
             return False, delay
 
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
-            await self._create_session()
+            self._create_session()
         status = False
         try_ = 1
         result = None
 
         # parse until success or not max retries
         while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
@@ -236,22 +234,22 @@
         words = date_.split()
         num = ''.join(c for c in words[-2] if c.isdigit())
         date_string = words[-3] + num + words[-1]
         date = datetime.strptime(date_string, "%B%d%Y")
         return date.strftime("%d-%m-%Y")
 
     def _localize_datetime_to_timezone(self, date_: datetime = None, date_str: str = None) -> datetime:
-        if self.TIMEZONE == 'Europe/Copenhagen':
+        if not self.TIMEZONE:
             return date_
         if date_str:
             date_ = datetime.strptime(date_str, '%d-%m-%Y')
         if date_.tzinfo:
             return date_.astimezone(pytz.timezone(self.TIMEZONE))
-        else:
-            return pytz.timezone('Europe/Copenhagen').localize(date_).astimezone(pytz.timezone(self.TIMEZONE))
+
+        return pytz.timezone('Europe/Copenhagen').localize(date_).astimezone(pytz.timezone(self.TIMEZONE))
 
     async def get(self, type: str, id: int | str | None = None,
                   title: str | None = None,
                   team1: str | None = None,
                   team2: str | None = None):
         if type == 'events':
             if id:
@@ -368,27 +366,32 @@
                             })
 
         except AttributeError:
             return None
 
         return matches
 
-    async def get_match_info(self, match_id: str | int, team1: str, team2: str, event_title: str, stats: bool = True):
-        r = await self._fetch(f"https://www.hltv.org/matches/{str(match_id)}/"
+    async def get_match_info(self, id: str | int,
+                             team1: str,
+                             team2: str,
+                             event_title: str,
+                             stats: bool = True,
+                             predicts: bool = True):
+        r = await self._fetch(f"https://www.hltv.org/matches/{str(id)}/"
                               f"{team1.replace(' ', '-')}-vs-"
                               f"{team2.replace(' ', '-')}-"
                               f"{event_title.replace(' ', '-')}")
         if not r:
             return
         status_ = {'Match over': 0, 'LIVE': 1}
-
         status = r.find('div', {'class': 'countdown'}).text
-
         status_int = status_[status] if status in status_ else 2
 
+        match_info = {'id': id}
+
         if status_int == 2:
             components = status.split(" : ")
 
             days, hours, minutes, seconds = 0, 0, 0, 0
 
             for component in components:
                 if 'd' in component:
@@ -404,14 +407,16 @@
                 days=days,
                 hours=hours,
                 minutes=minutes,
                 seconds=seconds)
 
             status = self._localize_datetime_to_timezone(date_=date_).strftime('%d-%m-%Y-%H-%M')
 
+        match_info['status'] = status
+
         score1, score2 = 0, 0
 
         if status_int == 0:
             scores = r.find_all('div', class_='team')
             score1 = scores[0].get_text().replace('\n', '')[-1]
             score2 = scores[1].get_text().replace('\n', '')[-1]
 
@@ -435,16 +440,18 @@
                     elif 'pick' in map_div.find('span', class_='results-right')['class']:
                         pick = team2
                 except TypeError:
                     pick = ''
 
             maps.append({'mapname': mapname, 'r_team1': r_team1, 'r_team2': r_team2, 'pick': pick})
 
-        stats_ = []
+        match_info['maps'] = maps
+
         if stats and status_int == 0:
+            stats_ = []
             for table_div in r.find_all('table', {'class': 'table totalstats'})[:2]:
                 for player in table_div.find_all('tr')[1:]:
                     player_id = player.find('a', class_='flagAlign')['href'].split('/')[2]
                     player_name = player.find('div', class_='statsPlayerName').text.strip()
                     nickname = re.findall(r"'(.*?)'", player_name)[0]
 
                     kd = player.find('td', class_='kd').text.strip()
@@ -453,14 +460,15 @@
                     stats_.append({
                         'id': player_id,
                         'nickname': nickname,
                         'kd': kd,
                         'adr': adr,
                         'rating': rating
                     })
+            match_info['stats'] = stats_
 
         if status_int == 1:
             for map in maps:
                 try:
                     if map["r_team1"].isdigit() and map["r_team2"].isdigit():
                         len_ = len(map)
                         s1, s2 = int(map["r_team1"]), int(map["r_team2"])
@@ -473,19 +481,27 @@
 
                         elif s2 > 12 and s2 > s1:
                             if len_ != 1:
                                 score2 += 1
                             else:
                                 score2 = s2
                                 score1 = s1
-
                 except ValueError:
                     pass
 
-        return {'id': match_id, 'score1': score1, 'score2': score2, 'status': status, 'maps': maps, 'stats': stats_}
+        if predicts and status != 0:
+            try:
+                predict_div = r.find('div', class_='standard-box pick-a-winner').find_all('div', class_='percentage')
+                match_info['predict1'] = predict_div[0].text
+                match_info['predict2'] = predict_div[1].text
+            except (AttributeError, IndexError):
+                pass
+
+        match_info['score1'], match_info['score2'] = score1, score2
+        return match_info
 
     async def get_results(self, days: int = 1,
                           min_rating: int = 1,
                           max: int = 30,
                           featured: bool = True,
                           regular: bool = True) -> list[dict[str, Any]] | None:
         """returns a list of big event matches results"""
@@ -531,86 +547,90 @@
 
         if regular:
 
             n = 0
 
             for i, date_div in enumerate(r.find_all('div', class_='results-sublist')[1:], start=1):
                 if i > days: break
-
-                date_ = self.__normalize_date(date_div.find('span', class_='standard-headline').text)
-                date = self._localize_datetime_to_timezone(date_str=date_).strftime('%d-%m-%Y')
+                try:
+                    date__ = self.__normalize_date(date_div.find('span', class_='standard-headline').text)
+                    date = self._localize_datetime_to_timezone(date_str=date__).strftime('%d-%m-%Y')
+                except Exception:
+                    date = None
 
                 for res in date_div.find_all("a", {"class": "a-reset"}):
                     if res['href'] == '/forums' or n > max:
                         break
+                    result_ = {}
                     rating = len(res.find_all('i', {'class': 'fa fa-star star'}))
 
                     if rating >= min_rating:
+                        match_id = 0
+                        team1 = 'TBD'
+                        team2 = 'TBD'
                         try:
                             match_id = res['href'].split('/', 3)[2]
                         except IndexError:
-                            match_id = 0
+                            pass
+                        finally:
+                            result_['id'] = match_id
+                            if date: result_['date'] = date
                         try:
                             teams = res.find_all('td', class_='team-cell')
                             team1 = teams[0].get_text().strip()
                             team2 = teams[1].get_text().strip()
                         except (AttributeError, IndexError):
-                            team1 = 'TBD'
-                            team2 = 'TBD'
-
-                        event = res.find('span', class_='event-name').text
+                            pass
+                        finally:
+                            result_['team1'] = team1
+                            result_['team2'] = team2
 
                         scores = res.find("td", class_="result-score").text.strip().split('-')
-                        s_t1 = scores[0].strip()
-                        s_t2 = scores[1].strip()
-
-                        results.append({
-                            'id': match_id,
-                            'date': date,
-                            'team1': team1,
-                            'team2': team2,
-                            'score1': s_t1,
-                            'score2': s_t2,
-                            'rating': rating,
-                            'event': event,
-                        })
+                        result_['score1'] = scores[0].strip()
+                        result_['score2'] = scores[1].strip()
+                        result_['rating'] = rating
+                        result_['event'] = res.find('span', class_='event-name').text
 
+                        results.append(result_)
                         n += 1
 
         return results
 
-    async def get_event_results(self, event: int | str, days: int = 1, max_: int = 10) -> list[dict[str, Any]] | None:
-        r = await self._fetch("https://www.hltv.org/results?event=" + str(event))
+    async def get_event_results(self, event_id: int | str, days: int = 1, max_: int = 10) -> list[
+                                                                                                 dict[str, Any]] | None:
+        r = await self._fetch("https://www.hltv.org/results?event=" + str(event_id))
         if not r:
             return
 
         match_results = []
 
         n = 0
         for i, result in enumerate(
                 r.find("div", {'class', 'results-holder'}).find_all("div", {'class', 'results-sublist'}), start=1):
             if i > days or n > max_:
                 break
-            date_ = self.__normalize_date(result.find("span", class_="standard-headline").text.strip())
-            date = self._localize_datetime_to_timezone(date_str=date_).strftime("%d-%m-%Y")
+            try:
+                date_ = self.__normalize_date(result.find("span", class_="standard-headline").text.strip())
+                date = self._localize_datetime_to_timezone(date_str=date_).strftime("%d-%m-%Y")
+            except Exception:
+                date = None
 
             for match in result.find_all("a", class_="a-reset"):
                 if n > max_:
                     break
 
                 id_ = match['href'].split('/')[2]
                 teams = match.find_all("div", class_="team")
                 team1 = teams[0].text.strip()
                 team2 = teams[1].text.strip()
 
                 scores = match.find("td", class_="result-score").text.strip().split('-')
                 score_t1 = scores[0].strip()
                 score_t2 = scores[1].strip()
 
-                # TODO add team ids
                 match_results.append({
                     'id': id_,
                     'date': date,
                     'team1': team1,
                     'team2': team2,
                     'score1': score_t1,
                     'score2': score_t2,
@@ -623,15 +643,15 @@
         if not r:
             return
 
         live_matches: List | Any
         matches = []
         try:
             live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div",
-                                                     {'class', 'liveMatch-container'})
+                                                                                   {'class', 'liveMatch-container'})
         except AttributeError:
             live_matches = []
         for live in live_matches:
             id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
@@ -653,16 +673,15 @@
                 'team1': team1,
                 'team2': team2,
                 't1_id': t1_id,
                 't2_id': t2_id
             })
 
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
-            date_ = datetime.strptime(date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1],
-                                      "%Y-%m-%d")
+            date_ = date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1]
             for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
                 teams_ = match.find_all("div", class_="matchTeamName text-ellipsis")
                 id_ = match.find('a')['href'].split('/')[2]
                 t1_id = 0
                 t2_id = 0
                 time_ = match.find('div', {'class', 'matchTime'}).text
                 team1_ = 'TBD'
@@ -807,26 +826,27 @@
                 'start': event_start,
                 'end': event_end,
                 'prize': prize,
                 'teams': team_num,
                 'location': location,
                 'group': groups}
 
-    async def get_top_teams(self, max_teams=30):
+    async def get_top_teams(self, max_teams=30, date_str: str = ''):
         """
         returns a list of the top 1-30 teams
         :params:
         max_teams: int = 30
         :return:
         [('rank','title','points', 'change', 'id')]
         change - difference between last ranking update
         """
-        today = date.today()
-        current_weekday = today.weekday()
-        last_monday = today - timedelta(days=current_weekday)
+        day = datetime.strptime(date_str, "%Y-%m-%d") if date_str else date.today()
+
+        current_weekday = day.weekday()
+        last_monday = day - timedelta(days=current_weekday)
 
         teams = []
 
         r = await self._fetch("https://www.hltv.org/ranking/teams/" + last_monday.strftime('%Y/%B/%d').lower())
 
         if not r:
             return
@@ -872,22 +892,26 @@
     async def get_team_info(self, team_id: int | str, title: str) -> dict[str, list[str]]:
         """
         Returns Information about team
         :params:
         team_id: int | str
         title: str
         :returns:
-        (team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys) | None
+        (team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophies) | None
         weeks - weeks in top 20
         """
         r = await self._fetch("https://www.hltv.org/team/" + str(team_id) + '/' + title.replace(' ', '-'))
-        players = []
+        players = {}
         try:
-            for player in r.find_all('span', {'class': 'text-ellipsis bold'}):
-                players.append(player.text)
+            known_players = r.find('div', class_='bodyshot-team g-grid').find_all('a')
+            players = {player.find('span', {'class': 'text-ellipsis bold'}).text: int(player['href'].split('/')[2]) for
+                       player in known_players}
+
+            #unknown_players = {'unknown' + str(i): 0 for i in range(len(players) + 1, 6)}
+            #players.update(unknown_players)
 
             rank = '0'
             weeks = '0'
             age = '0'
             coach = ''
 
             for i, stat in enumerate(r.find_all('div', {'class': 'profile-team-stat'}), start=1):
@@ -919,15 +943,15 @@
                     'age': age,
                     'weekstop30': weeks,
                     'last_trophy': last_trophy,
                     'total_trophies': total_trophies}
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
-    async def get_best_players(self, top=40):
+    async def get_top_players(self, top=40):
         """
         returns a list of the top (1-40) players in top 20 at the year
         :params:
         top: int = 40
         :returns:
         ('rank', 'name', 'team', 'maps', 'rating')
         maps - maps played
@@ -959,27 +983,95 @@
                         break
                     except AttributeError:
                         pass
 
                 players.append({
                     'id': id_,
                     'rank': rank,
-                    'name': name,
+                    'nickname': name,
                     'team': team,
                     'maps': maps,
                     'rating': rating,
                 })
                 rank += 1
                 if rank > top:
                     break
         except AttributeError:
             raise AttributeError("Top players parsing error, probably page not fully loaded")
 
         return players
 
+    async def get_player_info(self, id: int | str, nickname: str):
+        r = await self._fetch(f'https://www.hltv.org/player/{str(id)}/{nickname}')
+
+        name_div = r.find('div', class_='playerRealname')
+        name = name_div.get_text().strip()
+        nationality = name_div.find('img')['title']
+
+        try:
+            team_div = r.find('div', class_='playerInfoRow playerTeam').find('a')
+            team_str = team_div.get_text().strip()
+            team_id = int(team_div['href'].split('/', 3)[2])
+        except (AttributeError, TypeError):
+            team_str = 'None'
+            team_id = 0
+
+        age = int(r.find('div', class_='playerInfoRow playerAge').find('span', class_='listRight').get_text().strip().split()[0])
+
+        rating_div = r.find('div', class_='playerpage-container').find_all('span', class_='statsVal')
+        rating = rating_div[0].get_text().strip()
+        kpr = rating_div[1].get_text().strip()
+        hs = rating_div[2].get_text().strip()
+
+        mvps = 0
+        last_trophy = ''
+        try:
+            trophies_div = r.find('div', class_='trophyRow').find_all(class_='trophy')
+            total_trophies = len(trophies_div)
+
+            # Find last trophy
+            last_trophy = ''
+            for trophy in trophies_div:
+                try:
+                    if trophy['href'] and 'events' in trophy['href']:
+                        last_trophy = trophy.find('span', class_='trophyDescription')['title']
+                        break
+                except (KeyError, TypeError):
+                    pass
+
+            # Find MVPs
+            try:
+                mvps = int(trophies_div[0].find('div', class_='mvp-count').text)
+            except (IndexError, AttributeError, ValueError):
+                mvps = 0
+
+        except Exception:
+            total_trophies = 0
+
+        matches = []
+        matches_div = r.find_all('div', class_='col-6 text-ellipsis')[1]
+        for match in matches_div.find_all('a'):
+            matches.append(int(match['href'].split('/', 4)[3]))
+
+        return {'id': int(id),
+                'nickname': nickname,
+                'team': team_str,
+                'team_id': team_id,
+                'name': name,
+                'nationality': nationality,
+                'age': age,
+                'rating': rating,
+                'kpr': kpr,
+                'hs': hs,
+                'last_matches': matches,
+                'last_trophy': last_trophy,
+                'total_trophies': total_trophies,
+                'total_mvps': mvps,
+                }
+
     async def get_last_news(self, max_reg_news=2, only_today=True, only_featured=False):
 
         r = await self._fetch('https://www.hltv.org/')
 
         today = datetime.now(tz=pytz.timezone('Europe/Copenhagen'))
         article_days = {
             1: today.strftime('%d-%m'),
@@ -1031,11 +1123,12 @@
                 break
 
         return news
 
 
 async def main():
     async with Hltv(proxy_path='proxies.txt', proxy_protocol='http', debug=True) as hltv:
-        print(await hltv.get_matches())
+        print(await hltv.get_player_info(7998, 's1mple'))
+
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `hltv_async_api-0.7.0/LICENSE` & `hltv_async_api-0.8.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.7.0/pyproject.toml` & `hltv_async_api-0.8.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.7.0"
+version = "0.8.0b"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.7.0/README.md` & `hltv_async_api-0.8.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
+# hltv-async-api an **unofficial** asynchronous HLTV API Wrapper for Python. Use only in non-commercial purposes
 
 
 **This page is not completed, not all methods and configs are written**
 
 
 # Features
 
@@ -104,15 +104,15 @@
     ```
     await hltv.get_matches(days=1)
     
     >>> [{'id': '2371201', 'date': 'LIVE', 'time': 'LIVE', 'team1': 'Imperial', 'team2': 'MIBR', 't1_id': '9455', 't2_id': '9215', 'maps': '3', 'rating': 1, 'event': 'RES Regional Series 3 LATAM'}, {'id': '2370964', 'date': '2024-04-16', 'time': '12:30', 'team1': 'SAW', 'team2': 'Sampi', 't1_id': '10567', 't2_id': '10695', 'maps': '3', 'rating': 1, 'event': 'Thunderpick World Championship 2024 EU Closed Qualifier 1'}, {'id': '2371367', 'date': '2024-04-16', 'time': '14:00', 'team1': 'Gaimin Gladiators', 'team2': 'Permitta', 't1_id': '11571', 't2_id': '12009', 'maps': '3', 'rating': 1, 'event': 'Elisa Invitational Spring 2024'}]
     
     ```
 
-* **get_match_info(match_id: int | str, team1, team2, event_title)**
+* **get_match_info(match_id: int | str, team1, team2, event_title, stats: bool = True, predicts: bool = True)**
   
     ```
     await hltv.get_match_info(2370931, 'Mouz', 'faze', 'iem-chengdu-2024')  
   
     >>>(2370931, '0', '2', 'Match over', [{'mapname': 'Overpass', 'r_team1': '10', 'r_team2': '13'}, {'mapname': 'Nuke', 'r_team1': '6', 'r_team2': '13'}, {'mapname': 'Mirage', 'r_team1': '-', 'r_team2': '-'}], [{'id': '18850', 'nickname': 'Jimpphat', 'kd': '33-29', 'adr': '80.9', 'rating': '1.08'}, 
   
     {'id': '18072', 'nickname': 'torzsi', 'kd': '26-25', 'adr': '70.5', 'rating': '1.02'}, {'id': '13666', 'nickname': 'Brollan', 'kd': '25-31', 'adr': '68.4', 'rating': '0.90'}, {'id': '20312', 'nickname': 'xertioN', 'kd': '23-31', 'adr': '62.4', 'rating': '0.82'}, {'id': '16820', 'nickname': 'siuhy', 'kd': '17-30', 'adr': '51.6', 'rating': '0.70'}, {'id': '18053', 'nickname': 'broky', 'kd': '34-22', 'adr': '79.3', 'rating': '1.33'}, {'id': '9960', 'nickname': 'frozen', 'kd': '33-23', 'adr': '85.5', 'rating': '1.31'}, {'id': '11816', 'nickname': 'ropz', 'kd': '31-26', 'adr': '73.0', 'rating': '1.20'}, {'id': '8183', 'nickname': 'rain', 'kd': '27-26', 'adr': '82.0', 'rating': '1.18'}, {'id': '429', 'nickname': 'karrigan', 'kd': '20-28', 'adr': '49.7', 'rating': '0.81'}])  
@@ -169,15 +169,15 @@
 
     ```
     await hltv.get_top_teams(2)
     
     >>>[{'id': '1111', 'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'id': '1111', 'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
     ```
 
-* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
+* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, {player:player_id}, coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
 
     ```
     await hltv.get_team_info(6667, 'faze')
     
     >>>(6667, 'faze', '1', ['karrigan', 'rain', 'frozen', 'ropz', 'broky'], 'NEO', '26.6', '258', 'IEM Chengdu 2024', 22)
     ```
 
@@ -194,14 +194,22 @@
 
     ```
     await hltv.get_best_players(2)
     
     >>>[{'id': '19230', 'rank': 1, 'name': 'm0NESY', 'team': 'G2', 'maps': '44', 'rating': '1.37'}, {'id': '18053', 'rank': 2, 'name': 'broky', 'team': 'FaZe', 'maps': '54', 'rating': '1.19'}]
     ```
 
+* **get_player_info(id: str | int, nickname: str)**
+  
+  ```
+  await hltv.get_player_info(7998, 's1mple')
+  
+  {'id': 7998, 'nickname': 's1mple', 'team': 'Natus Vincere', 'team_id': 4608, 'name': 'Oleksandr Kostyliev', 'nationality': 'Ukraine', 'age': 26, 'rating': '0.94', 'kpr': '0.60', 'hs': '57.9%', 'last_matches': [103059, 99745, 99728, 99696, 99471, 99364], 'last_trophy': 'BLAST Premier Spring Final 2022', 'total_trophies': 30, 'total_mvps': 21}
+  ```
+
 * **get(type: str, id: int | str | None = None, title: str | None = None, team1: str | None = None, team2: str | None = None):**
   (BETA) This method is not finished. Possible types 'events', 'matches', 'teams', also u can add id | title | team1 | team2, to parse more.
   
   ```
   
   await hltv.get('matches', 2371201, 'res-regional-series-3-latam', 'IMPERIAL', 'MIBR')
   
@@ -209,15 +217,15 @@
   
   ```
 ---
 # Configs
 
 * max_delay: int = 15
 
-    We automaticly increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
+    Automatically increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
 
     ```
     hltv = Hltv(max_delay=5)
     
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 4s
@@ -402,23 +410,28 @@
 
 # Tests:
 
 **<a href='https://github.com/akimerslys/hltv-async-api/blob/main/test/hard_test.py'>To test library you can use temporarily test file</a>**
 
 ```
 
-Parsed 15 matches.(17s) ERRORS: 0/15
-Parsed 13 events.(28s) ERRORS: 0/13
+Parsed 208 matches.(97s) ERRORS: 0/208
+Parsed 25 events.(23s) ERRORS: 0/25
 Parsed 31 teams.(41s) ERRORS: 0/31
+Parsed 31 players.(28s) ERRORS: 0/31
 ERRORS=0
-SUCCESS=64
-Total parsed=64
-Total time 40.8259
+SUCCESS=284
+Total parsed=284
+Total time 96.8368
 
 ```
 
+# Beta / Unreleased
+
+**That functions were made for myself, before using recommend you to check the file**
+
 # Requirements:
 
 Python 3.9+
 
 License:
 HLTV Async is licensed under the MIT License, allowing for personal and commercial use with minimal restrictions.
```

### Comparing `hltv_async_api-0.7.0/PKG-INFO` & `hltv_async_api-0.8.0b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.7.0
+Version: 0.8.0b0
 Summary: An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: lxml (==5.2.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: setuptools (>=69.1.0,<70.0.0)
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Description-Content-Type: text/markdown
 
-# hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
+# hltv-async-api an **unofficial** asynchronous HLTV API Wrapper for Python. Use only in non-commercial purposes
 
 
 **This page is not completed, not all methods and configs are written**
 
 
 # Features
 
@@ -127,15 +127,15 @@
     ```
     await hltv.get_matches(days=1)
     
     >>> [{'id': '2371201', 'date': 'LIVE', 'time': 'LIVE', 'team1': 'Imperial', 'team2': 'MIBR', 't1_id': '9455', 't2_id': '9215', 'maps': '3', 'rating': 1, 'event': 'RES Regional Series 3 LATAM'}, {'id': '2370964', 'date': '2024-04-16', 'time': '12:30', 'team1': 'SAW', 'team2': 'Sampi', 't1_id': '10567', 't2_id': '10695', 'maps': '3', 'rating': 1, 'event': 'Thunderpick World Championship 2024 EU Closed Qualifier 1'}, {'id': '2371367', 'date': '2024-04-16', 'time': '14:00', 'team1': 'Gaimin Gladiators', 'team2': 'Permitta', 't1_id': '11571', 't2_id': '12009', 'maps': '3', 'rating': 1, 'event': 'Elisa Invitational Spring 2024'}]
     
     ```
 
-* **get_match_info(match_id: int | str, team1, team2, event_title)**
+* **get_match_info(match_id: int | str, team1, team2, event_title, stats: bool = True, predicts: bool = True)**
   
     ```
     await hltv.get_match_info(2370931, 'Mouz', 'faze', 'iem-chengdu-2024')  
   
     >>>(2370931, '0', '2', 'Match over', [{'mapname': 'Overpass', 'r_team1': '10', 'r_team2': '13'}, {'mapname': 'Nuke', 'r_team1': '6', 'r_team2': '13'}, {'mapname': 'Mirage', 'r_team1': '-', 'r_team2': '-'}], [{'id': '18850', 'nickname': 'Jimpphat', 'kd': '33-29', 'adr': '80.9', 'rating': '1.08'}, 
   
     {'id': '18072', 'nickname': 'torzsi', 'kd': '26-25', 'adr': '70.5', 'rating': '1.02'}, {'id': '13666', 'nickname': 'Brollan', 'kd': '25-31', 'adr': '68.4', 'rating': '0.90'}, {'id': '20312', 'nickname': 'xertioN', 'kd': '23-31', 'adr': '62.4', 'rating': '0.82'}, {'id': '16820', 'nickname': 'siuhy', 'kd': '17-30', 'adr': '51.6', 'rating': '0.70'}, {'id': '18053', 'nickname': 'broky', 'kd': '34-22', 'adr': '79.3', 'rating': '1.33'}, {'id': '9960', 'nickname': 'frozen', 'kd': '33-23', 'adr': '85.5', 'rating': '1.31'}, {'id': '11816', 'nickname': 'ropz', 'kd': '31-26', 'adr': '73.0', 'rating': '1.20'}, {'id': '8183', 'nickname': 'rain', 'kd': '27-26', 'adr': '82.0', 'rating': '1.18'}, {'id': '429', 'nickname': 'karrigan', 'kd': '20-28', 'adr': '49.7', 'rating': '0.81'}])  
@@ -192,15 +192,15 @@
 
     ```
     await hltv.get_top_teams(2)
     
     >>>[{'id': '1111', 'rank': '1', 'title': 'FaZe', 'points': '939', 'change': '-', 'id': '6667'}, {'id': '1111', 'rank': '2', 'title': 'Natus Vincere', 'points': '757', 'change': '+4', 'id': '4608'}]
     ```
 
-* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, [players], coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
+* **get_team_info(team_id: int | str, title: str) -> (team_id, team_title, rank, {player:player_id}, coach, average_age, weeks_in_top_20, last_trophy, total_trophys)**
 
     ```
     await hltv.get_team_info(6667, 'faze')
     
     >>>(6667, 'faze', '1', ['karrigan', 'rain', 'frozen', 'ropz', 'broky'], 'NEO', '26.6', '258', 'IEM Chengdu 2024', 22)
     ```
 
@@ -217,14 +217,22 @@
 
     ```
     await hltv.get_best_players(2)
     
     >>>[{'id': '19230', 'rank': 1, 'name': 'm0NESY', 'team': 'G2', 'maps': '44', 'rating': '1.37'}, {'id': '18053', 'rank': 2, 'name': 'broky', 'team': 'FaZe', 'maps': '54', 'rating': '1.19'}]
     ```
 
+* **get_player_info(id: str | int, nickname: str)**
+  
+  ```
+  await hltv.get_player_info(7998, 's1mple')
+  
+  {'id': 7998, 'nickname': 's1mple', 'team': 'Natus Vincere', 'team_id': 4608, 'name': 'Oleksandr Kostyliev', 'nationality': 'Ukraine', 'age': 26, 'rating': '0.94', 'kpr': '0.60', 'hs': '57.9%', 'last_matches': [103059, 99745, 99728, 99696, 99471, 99364], 'last_trophy': 'BLAST Premier Spring Final 2022', 'total_trophies': 30, 'total_mvps': 21}
+  ```
+
 * **get(type: str, id: int | str | None = None, title: str | None = None, team1: str | None = None, team2: str | None = None):**
   (BETA) This method is not finished. Possible types 'events', 'matches', 'teams', also u can add id | title | team1 | team2, to parse more.
   
   ```
   
   await hltv.get('matches', 2371201, 'res-regional-series-3-latam', 'IMPERIAL', 'MIBR')
   
@@ -232,15 +240,15 @@
   
   ```
 ---
 # Configs
 
 * max_delay: int = 15
 
-    We automaticly increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
+    Automatically increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
 
     ```
     hltv = Hltv(max_delay=5)
     
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 4s
@@ -425,24 +433,29 @@
 
 # Tests:
 
 **<a href='https://github.com/akimerslys/hltv-async-api/blob/main/test/hard_test.py'>To test library you can use temporarily test file</a>**
 
 ```
 
-Parsed 15 matches.(17s) ERRORS: 0/15
-Parsed 13 events.(28s) ERRORS: 0/13
+Parsed 208 matches.(97s) ERRORS: 0/208
+Parsed 25 events.(23s) ERRORS: 0/25
 Parsed 31 teams.(41s) ERRORS: 0/31
+Parsed 31 players.(28s) ERRORS: 0/31
 ERRORS=0
-SUCCESS=64
-Total parsed=64
-Total time 40.8259
+SUCCESS=284
+Total parsed=284
+Total time 96.8368
 
 ```
 
+# Beta / Unreleased
+
+**That functions were made for myself, before using recommend you to check the file**
+
 # Requirements:
 
 Python 3.9+
 
 License:
 HLTV Async is licensed under the MIT License, allowing for personal and commercial use with minimal restrictions.
```

