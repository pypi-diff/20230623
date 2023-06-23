# Comparing `tmp/spotify_recommender_api-4.3.0-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 40027 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-23 03:52 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx      636 b- defN 23-Jun-23 03:35 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    14957 b- defN 23-Jun-23 03:43 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 03:41 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx   108957 b- defN 23-Jun-23 03:52 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     6305 b- defN 23-Jun-23 03:49 spotify_recommender_api/request_handler.py
+Zip file size: 40747 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jun-23 14:38 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-23 14:31 spotify_recommender_api/authentication.py
+-rw-rw-r--  2.0 unx    15037 b- defN 23-Jun-23 14:31 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 14:32 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx   111983 b- defN 23-Jun-23 14:37 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     6305 b- defN 23-Jun-23 14:31 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     6720 b- defN 23-Jun-23 03:51 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9510 b- defN 23-Jun-23 03:36 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    21409 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1193 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/RECORD
-13 files, 171965 bytes uncompressed, 37995 bytes compressed:  77.9%
+-rw-rw-r--  2.0 unx     6720 b- defN 23-Jun-23 14:32 spotify_recommender_api/server.py
+-rw-rw-r--  2.0 unx     9510 b- defN 23-Jun-23 14:32 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    21409 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-23 14:40 spotify_recommender_api-4.3.1.dist-info/RECORD
+13 files, 175698 bytes uncompressed, 38715 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.3.0.dist-info/METADATA
+Filename: spotify_recommender_api-4.3.1.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.3.0.dist-info/WHEEL
+Filename: spotify_recommender_api-4.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.3.0.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.3.0.dist-info/RECORD
+Filename: spotify_recommender_api-4.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.3.0'
+__version__ = '4.3.1'
```

## spotify_recommender_api/authentication.py

```diff
@@ -1,21 +1,39 @@
 import os
-from spotify_recommender_api.sensitive import *
+import logging
+import spotify_recommender_api.request_handler as requests
 from spotify_recommender_api.server import up_server
-from spotify_recommender_api.request_handler import post_request_with_auth
 
 
 def get_auth() -> str:
     """Function to retrieve the authentication token for the first time in the execution
 
     Returns:
         str: Auth Token
     """
-    up_server()
 
     with open('./.spotify-recommender-util/execution.txt', 'r') as f:
-        auth_token = f.readline()
+        try:
+            auth_token = f.readline()
 
-    if os.path.exists("./.spotify-recommender-util/execution-status.txt"):
-        os.remove("./.spotify-recommender-util/execution-status.txt")
+            requests.get_request(
+                headers={
+                    "Accept": "application/json",
+                    "Content-Type": "application/json",
+                    "Authorization": f'Bearer {auth_token}'
+                },
+                url='https://api.spotify.com/v1/search?q=NF&type=artist&limit=1'
+            ).json()['artists']
+
+        except Exception as e:
+            logging.debug('Error while trying the existant auth token. Executing server to retrieve a new one.', e)
+
+            up_server()
+
+            with open('./.spotify-recommender-util/execution.txt', 'r') as f:
+                auth_token = f.readline()
+
+            if os.path.exists("./.spotify-recommender-util/execution-status.txt"):
+                os.remove("./.spotify-recommender-util/execution-status.txt")
+
+        return auth_token
 
-    return auth_token
```

## spotify_recommender_api/core.py

```diff
@@ -141,15 +141,15 @@
     Raises:
         ValueError: The type argument musts be one of the valid options
 
     Returns:
         str: The playlist id
     """
     if additional_info is None:
-        return 
+        return
 
     if type == 'song':
         playlist_name = f"{additional_info!r} Related"
         description = f"Songs related to {additional_info!r}, within the playlist {base_playlist_name}"
     elif type in {'short', 'medium'}:
         playlist_name = "Recent-ish Favorites" if type == 'medium' else "Latest Favorites"
         description = f"Songs related to your {type} term top 5, within the playlist {base_playlist_name}"
@@ -196,16 +196,16 @@
             playlist_name += f' ({criteria})'
 
     elif type == 'general-recommendation':
         playlist_name = f"General Recommendation based on {additional_info[1]}"
         description = additional_info[0]
 
     elif type == 'mood':
-        playlist_name = f"{additional_info} Songs".capitalize()
-        description = f'Songs related to the mood "{additional_info}", within the playlist {base_playlist_name}'
+        playlist_name = f"{additional_info[0]} Songs".capitalize()
+        description = f'Songs related to the mood "{additional_info[0]}"{", excluding the mostly instrumental songs" if additional_info[1] else ""}, within the playlist {base_playlist_name}'
 
     else:
         raise ValueError('type not valid')
 
     if playlist_id_found := util.playlist_exists(name=playlist_name, base_playlist_name=base_playlist_name, headers=headers, _update_created_playlists=_update_created_playlists):
         new_id = playlist_id_found
```

## spotify_recommender_api/recommender.py

```diff
@@ -6,15 +6,14 @@
 import pandas as pd
 import spotify_recommender_api.util as util
 import spotify_recommender_api.core as core
 import spotify_recommender_api.authentication as auth
 import spotify_recommender_api.request_handler as requests
 from functools import reduce
 from typing import Any, Union
-from spotify_recommender_api.sensitive import CLIENT_ID, CLIENT_SECRET
 from spotify_recommender_api.error import AccessTokenExpiredError
 warnings.filterwarnings('error')
 
 
 class SpotifyAPI:
     """
     Spotify API is the Class that provides access to the playlists recommendations
@@ -454,31 +453,34 @@
 
             for offset in range(0, len(full_uris_list), 100):
 
                 uris = ','.join(full_uris_list[offset:offset + min(len(full_uris_list) - offset, 100)])
                 add_songs_req = requests.post_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
 
 
-    def __build_playlist(self, type: str, uris: str, add_info=None):
+    def __build_playlist(self, type: str, uris: str):
         """Function that builds the contents of a playlist
 
         Note:
             This function will change the user's library by filling the previously created empty playlist
 
         Args:
             type (str): the type of the playlist being created
             uris (str): string containing all song uris in the format the Spotify API expects
         """
         if not uris:
             raise ValueError('Invalid value for the song uris')
 
         additional_information_by_type = {
-            'mood': add_info,
             'song': getattr(self, '_SpotifyAPI__song_name', None),
             'artist': getattr(self, '_SpotifyAPI__artist_name', None),
+            'mood': [
+                getattr(self, '_SpotifyAPI__mood', None),
+                getattr(self, '_SpotifyAPI__exclude_mostly_instrumental', None),
+            ],
             'profile-recommendation': [
                 getattr(self, '_SpotifyAPI__profile_recommendation_criteria', None),
                 getattr(self, '_SpotifyAPI__profile_recommendation_date', None)
             ],
             'playlist-recommendation': [
                 getattr(self, '_SpotifyAPI__playlist_recommendation_criteria', None),
                 getattr(self, '_SpotifyAPI__playlist_recommendation_date', None),
@@ -544,15 +546,15 @@
                 ids = []
             uris = ','.join([f'spotify:track:{song}' for song in ids])
 
         else:
             uris = ''
             raise ValueError('Invalid type')
 
-        self.__build_playlist(type=type, uris=uris, add_info=getattr(self, '_SpotifyAPI__mood', None))
+        self.__build_playlist(type=type, uris=uris)
 
     def get_recommendations_for_song(
         self,
         K: int,
         song: str,
         generate_csv: bool = False,
         with_distance: bool = False,
@@ -1015,40 +1017,91 @@
                     'popularity': x['popularity']
                 }
                 for x in top_songs
             ],
             columns=['name', 'artists', 'genres', 'popularity']
         )
 
+    def __playlist_needs_update(self, playlist: 'tuple[str, str, str, str]', playlist_types_to_update: 'list[str]') -> bool:
+        """Function to determine if a playlist inside the user's library needs to be updated
+
+        Args:
+            playlist (tuple[str, str, str, str]): Playlist information
+            playlist_types_to_update (list[str]): Playlist types to be updated
+
+        Returns:
+            bool: The flag that indicates whether the playlist should be updated or not
+        """
+        _, name, description, _ = playlist
+
+        if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
+            return True
+
+        elif 'Profile Recommendation' in name and ' - 20' not in name and 'profile-recommendation' in playlist_types_to_update:
+            return True
+
+        elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
+            if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
+                return True
+
+            elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)) and 'artist-mix' in playlist_types_to_update:
+                return True
+
+            elif (re.match(r"This once was \'(.*?)\'", name) or re.match(r'This once was \"(.*?)\"', name)) and 'artist-full' in playlist_types_to_update:
+                return True
+
+            elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
+                return True
+
+            elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
+                return True
+
+        return False
+
     def update_all_generated_playlists(self, *, K: Union[int, None] = None, playlist_types_to_update: Union['list[str]', None] = None):
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
-
-        Keyword Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
-            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all - ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation'].
+            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all - ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation', 'mood'].
         """
         if playlist_types_to_update is None:
-            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation']
+            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation', 'mood']
 
         total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
 
         playlists = []
 
         for offset in range(0, total_playlist_count, 50):
             request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
 
             playlists += [(playlist['id'], playlist['name'], playlist['description'], playlist['tracks']['total']) for playlist in request['items']]
 
-        for _, name, description, total_tracks in playlists:
+        playlists = [
+                playlist
+                for playlist in playlists
+                if self.__playlist_needs_update(
+                        playlist=playlist,
+                        playlist_types_to_update=playlist_types_to_update
+                )
+            ]
+
+        last_printed_perc_update = 0
+
+        for index, (_, name, description, total_tracks) in enumerate(playlists):
             try:
+                logging.debug(f'Updating song {name} - {index}/{len(playlists)}')
+                if last_printed_perc_update + 10 <= (perc_update := next((perc for perc in range(100, 0, -10) if (100 * index) / len(playlists) >= perc), 100)) < 100:
+                    logging.info(f'Playlists update operation at {perc_update}%')
+                    last_printed_perc_update = perc_update
+
                 if K is not None:
                     total_tracks = K
+
                 if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
                     self.get_most_listened(time_range=name.split(" ")[0].lower(), K=total_tracks, build_playlist=True)
 
                 elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
                     if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
                         song_name = name.replace(" Related", '')[1:-1]
                         self.__song_name = song_name
@@ -1073,46 +1126,53 @@
                             build_playlist=True,
                             artist_name=artist_name,
                             complete_with_similar=False,
                             ensure_all_artist_songs=f'All {artist_name}' in description,
                             _auto=True
                         )
 
-                    # elif name == 'Recent-ish Favorites':
-                    #     self.__write_playlist(type='medium', K=total_tracks)
-
-                    # elif name == 'Latest Favorites':
-                    #     self.__write_playlist(type='short', K=total_tracks)
-
                     elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
                         criteria = name.split('(')[1].split(')')[0]
                         if ',' in criteria:
                             criteria = 'mixed'
 
-                        time_range = 'all_time' if 'for all_time' in name else name.split(
-                            'for the last')[-1].split('(')[0].strip()
+                        time_range = 'all_time' if 'for all_time' in name else name.split('for the last')[-1].split('(')[0].strip()
 
                         self.get_playlist_recommendation(
                             K=total_tracks,
                             build_playlist=True,
                             time_range=time_range,
                             main_criteria=criteria,
                         )
 
+                    elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
+                        mood = ' '.join(name.split(' ')[:-1]).lower()
+
+                        exclude_mostly_instrumental = 'excluding the mostly instrumental songs' in description
+
+                        self.get_songs_by_mood(
+                            mood=mood,
+                            K=total_tracks,
+                            build_playlist=True,
+                            exclude_mostly_instrumental=exclude_mostly_instrumental,
+                        )
+
                 elif 'Profile Recommendation' in name and ' - 20' not in name and 'profile-recommendation' in playlist_types_to_update:
                     criteria = name.split('(')[1].split(')')[0]
                     if ',' in criteria:
                         criteria = 'mixed'
 
                     self.get_profile_recommendation(
                         K=total_tracks,
                         build_playlist=True,
                         main_criteria=criteria,
                     )
 
+                logging.info('Playlists update operation at 100%')
+
             except ValueError as e:
                 logging.error(f"Unfortunately we couldn't update a playlist because\n {e}")
 
     def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
         """Calculates the amount of times each genre was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
@@ -1866,26 +1926,24 @@
 
                 elif main_criteria == 'genres':
                     url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
                 elif main_criteria == 'mixed':
                     url += f'&seed_tracks={",".join(tracks[:1])}&seed_artists={",".join(artists[:2])}&seed_genres={",".join(genres[:2])}'
                 elif main_criteria == 'tracks':
                     url += f'&seed_tracks={",".join(tracks[:2])}&seed_genres={",".join(genres[:3])}'
-                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_loudness=!s}&{max_loudness=!s}&{target_loudness=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
 
                 recommendations = requests.get_request(url=url, headers=self.__headers).json()
 
                 songs = []
 
                 for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(
-                        song=song, added_at=False), self.__get_song_genres(song)
+                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                        song=song, headers=self.__headers)
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
                     songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "danceability": danceability,
@@ -2032,16 +2090,21 @@
                     elif not artists_info and not genres_info:
                         description += 'the tracks '
 
                     if isinstance(tracks_info, dict):
                         for song, artist in tracks_info.items():
                             description += f'{song} by {artist}, '
 
-                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
-                            'tracks']['items'][0]['id'] for song, artist in tracks_info.items()]
+                        tracks = [
+                            requests.get_request(
+                                headers=self.__headers,
+                                url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1',
+                            ).json()['tracks']['items'][0]['id']
+                            for song, artist in tracks_info.items()
+                        ]
 
                     elif isinstance(tracks_info[0], tuple) or isinstance(tracks_info[0], list):
                         for song, artist in tracks_info: # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
                             description += f'{song} by {artist}, '
                         tracks = [
                             requests.get_request(
                                 headers=self.__headers,
@@ -2049,23 +2112,26 @@
                             ).json()['tracks']['items'][0]['id']
                         for song, artist in tracks_info # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
                     ]
 
                     elif isinstance(tracks_info[0], str):
                         for song in tracks_info:
                             description += f'{song}, '
-                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1', headers=self.__headers).json()[
-                            'tracks']['items'][0]['id'] for song in tracks_info]
+                        tracks = [
+                            requests.get_request(
+                                headers=self.__headers,
+                                url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1',
+                            ).json()['tracks']['items'][0]['id']
+                            for song in tracks_info
+                        ]
 
                     else:
-                        raise ValueError(
-                            'The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]')
+                        raise ValueError('The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]')
 
-                    description = ' and '.join(
-                        description[:-2].rsplit(', ', 1)) if len(artists_info) > 1 else description[:-2]
+                    description = ' and '.join(description[:-2].rsplit(', ', 1)) if len(artists_info) > 1 else description[:-2]
 
                     url += f'&seed_tracks={",".join(tracks)}'
 
                     if len(tracks_info) == 1:
                         description = description.replace('tracks', 'track')
 
                 if use_main_playlist_audio_features:
@@ -2087,27 +2153,24 @@
                     min_loudness = audio_statistics['min_loudness'] * 0.8
                     max_loudness = audio_statistics['max_loudness'] * 1.2
                     target_loudness = audio_statistics['mean_loudness']
                     min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
                     max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
                     target_instrumentalness = audio_statistics['mean_instrumentalness']
 
-                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_loudness=!s}&{max_loudness=!s}&{target_loudness=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
 
-                recommendations = requests.get_request(
-                    url=url, headers=self.__headers).json()
+                recommendations = requests.get_request(url=url, headers=self.__headers).json()
 
                 songs = []
 
                 for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(
-                        song=song, added_at=False), self.__get_song_genres(song)
+                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                        song=song, headers=self.__headers)
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
                     songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "danceability": danceability,
@@ -2216,14 +2279,15 @@
             logging.warning(f'The playlist does not contain {K} {mood} songs. Therefore there are only {len(playlist)} in the returned playlist. ')
 
         if build_playlist:
 
             for _ in range(2):
                 try:
                     self.__mood = mood
+                    self.__exclude_mostly_instrumental = exclude_mostly_instrumental
                     ids = playlist['id'].tolist()
 
                     self.__write_playlist(
                         K=K,
                         type=f'mood',
                         additional_info=ids
                     )
@@ -2237,14 +2301,15 @@
                     self.__headers['Authorization'] = f'Bearer {auth_token}'
                 else:
                     break
 
         return playlist
 
 
+
 def start_api(user_id: str, *, playlist_url: Union[str, None] = None, playlist_id: Union[str, None] = None, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
     """Function that prepares for and initializes the API
 
     Note:
         Internet Connection is required
 
     Args:
```

## Comparing `spotify_recommender_api-4.3.0.dist-info/METADATA` & `spotify_recommender_api-4.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.3.0
+Version: 4.3.1
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

