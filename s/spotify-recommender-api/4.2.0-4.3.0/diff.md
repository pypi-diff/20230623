# Comparing `tmp/spotify_recommender_api-4.2.0-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 37935 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-May-28 16:03 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx      636 b- defN 23-May-28 16:02 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    14264 b- defN 23-May-28 16:03 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     1966 b- defN 23-May-28 16:02 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx    98800 b- defN 23-May-28 16:02 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     5933 b- defN 23-May-28 16:02 spotify_recommender_api/request_handler.py
+Zip file size: 40027 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jun-23 03:52 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx      636 b- defN 23-Jun-23 03:35 spotify_recommender_api/authentication.py
+-rw-rw-r--  2.0 unx    14957 b- defN 23-Jun-23 03:43 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 03:41 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx   108957 b- defN 23-Jun-23 03:52 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     6305 b- defN 23-Jun-23 03:49 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     6661 b- defN 23-May-28 16:03 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9304 b- defN 23-May-28 16:02 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    21022 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1192 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/RECORD
-13 files, 160014 bytes uncompressed, 35903 bytes compressed:  77.6%
+-rw-rw-r--  2.0 unx     6720 b- defN 23-Jun-23 03:51 spotify_recommender_api/server.py
+-rw-rw-r--  2.0 unx     9510 b- defN 23-Jun-23 03:36 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    21409 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1193 b- defN 23-Jun-23 04:00 spotify_recommender_api-4.3.0.dist-info/RECORD
+13 files, 171965 bytes uncompressed, 37995 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.2.0.dist-info/METADATA
+Filename: spotify_recommender_api-4.3.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.2.0.dist-info/WHEEL
+Filename: spotify_recommender_api-4.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.2.0.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.2.0.dist-info/RECORD
+Filename: spotify_recommender_api-4.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.2.0'
+__version__ = '4.3.0'
```

## spotify_recommender_api/core.py

```diff
@@ -2,18 +2,19 @@
 import logging
 import datetime
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import spotify_recommender_api.util as util
 import spotify_recommender_api.request_handler as requests
+from typing import Union, Any
 sns.set()
 
 
-def list_distance(indexed_genre_list_a: 'list[int]', indexed_genre_list_b: 'list[int]') -> int:
+def list_distance(indexed_genre_list_a: 'list[int]', indexed_genre_list_b: 'list[int]') -> float:
     """The weighted algorithm that calculates the distance between two songs according to either the distance between each song list of genres or the distance between each song list of artists
 
     Note:
         The "distance" is a mathematical value that represents how different two songs are, considering some parameter such as their genres or artists
 
     Note:
         For obvious reasons although both the parameters have two value options (genres, artists), when one of the parameters is specified as one of those, the other follows
@@ -31,28 +32,40 @@
             distance += 0.4 if int(item_a) == 1 else 0.2
         elif int(item_a) == 1:
             distance -= 0.4
 
     return distance
 
 
-def calculate_total_distance(genres_distance: float, energy_distance: float, valence_distance: float, artists_distance: float, tempo_distance: float, danceability_distance: float, instrumentalness_distance: float, popularity_distance: float, artist_recommendation: bool) -> float:
+def calculate_total_distance(
+        tempo_distance: float,
+        genres_distance: float,
+        energy_distance: float,
+        valence_distance: float,
+        artists_distance: float,
+        loudness_distance: float,
+        popularity_distance: float,
+        artist_recommendation: bool,
+        danceability_distance: float,
+        instrumentalness_distance: float
+    ) -> float:
     return (
         genres_distance * 0.8 +
         energy_distance * 0.6 +
         valence_distance * 0.9 +
         artists_distance * 0.38 +
         tempo_distance * 0.0025 +
+        loudness_distance * 0.25 +
         danceability_distance * 0.25 +
         instrumentalness_distance * 0.4 +
         popularity_distance * (0.003 if artist_recommendation else 0.015)
     )
 
 
-def compute_distance(song_a: 'dict[str,]', song_b: 'dict[str,]', artist_recommendation: bool = False) -> float:
+def compute_distance(song_a: 'dict[str, Any]', song_b: 'dict[str, Any]', artist_recommendation: bool = False) -> float:
     """The portion of the algorithm that calculates the overall distance between two songs regarding the following:
     - genres: the difference between the two song's genres, using the list_distance function above
     - artists: the difference between the two song's artists, using the list_distance function above
     - popularity: the difference between the two song's popularity, considering it a basic absolute value from the actual difference between the values
     - danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
     - energy: Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
     - instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content
@@ -68,41 +81,46 @@
         a (dict[str,]): the song a, having all it's caracteristics
         b (dict[str,]): the song b, having all it's caracteristics
 
     Returns:
         float: the distance between the two songs
     # """
 
-    genres_distance = list_distance(
-        song_a['genres_indexed'], song_b['genres_indexed'])
-    artists_distance = list_distance(
-        song_a['artists_indexed'], song_b['artists_indexed'])
-    popularity_distance = abs(song_a['popularity'] - song_b['popularity'])
-    danceability_distance = abs(
-        song_a['danceability'] - song_b['danceability'])
-    energy_distance = abs(song_a['energy'] - song_b['energy'])
-    instrumentalness_distance = abs(
-        round(song_a['instrumentalness'], 2) - round(song_b['instrumentalness'], 2))
     tempo_distance = abs(song_a['tempo'] - song_b['tempo'])
+    energy_distance = abs(song_a['energy'] - song_b['energy'])
     valence_distance = abs(song_a['valence'] - song_b['valence'])
+    popularity_distance = abs(song_a['popularity'] - song_b['popularity'])
+    danceability_distance = abs(song_a['danceability'] - song_b['danceability'])
+    loudness_distance = abs(song_a['loudness'] - song_b['loudness'])
+    genres_distance = list_distance(song_a['genres_indexed'], song_b['genres_indexed'])
+    artists_distance = list_distance(song_a['artists_indexed'], song_b['artists_indexed'])
+    instrumentalness_distance = abs(round(song_a['instrumentalness'], 2) - round(song_b['instrumentalness'], 2))
 
     return calculate_total_distance(
         tempo_distance=tempo_distance,
         genres_distance=genres_distance,
         energy_distance=energy_distance,
         valence_distance=valence_distance,
         artists_distance=artists_distance,
         popularity_distance=popularity_distance,
+        loudness_distance=loudness_distance,
         danceability_distance=danceability_distance,
         artist_recommendation=artist_recommendation,
         instrumentalness_distance=instrumentalness_distance,
     )
 
 
-def create_playlist(type: str, headers: dict, user_id: str, base_playlist_name: str, additional_info: str = None, _update_created_playlists: bool = False) -> str:
+def create_playlist(
+        type: str,
+        user_id: str,
+        headers: dict,
+        base_playlist_name: str,
+        additional_info: Union[str, 'list[Any]', None] = None,
+        _update_created_playlists: bool = False
+    ) -> Union[str, bool, None]:
     """Function that will return the empty playlist id, to be filled in later by the recommender songs
     This playlist may be a new one just created or a playlist that was previously created and now had all its songs removed
 
     Note:
         This function will change the user's library either making a new playlist or making an existing one empty
 
     Args:
@@ -122,14 +140,16 @@
 
     Raises:
         ValueError: The type argument musts be one of the valid options
 
     Returns:
         str: The playlist id
     """
+    if additional_info is None:
+        return 
 
     if type == 'song':
         playlist_name = f"{additional_info!r} Related"
         description = f"Songs related to {additional_info!r}, within the playlist {base_playlist_name}"
     elif type in {'short', 'medium'}:
         playlist_name = "Recent-ish Favorites" if type == 'medium' else "Latest Favorites"
         description = f"Songs related to your {type} term top 5, within the playlist {base_playlist_name}"
@@ -175,14 +195,18 @@
         else:
             playlist_name += f' ({criteria})'
 
     elif type == 'general-recommendation':
         playlist_name = f"General Recommendation based on {additional_info[1]}"
         description = additional_info[0]
 
+    elif type == 'mood':
+        playlist_name = f"{additional_info} Songs".capitalize()
+        description = f'Songs related to the mood "{additional_info}", within the playlist {base_playlist_name}'
+
     else:
         raise ValueError('type not valid')
 
     if playlist_id_found := util.playlist_exists(name=playlist_name, base_playlist_name=base_playlist_name, headers=headers, _update_created_playlists=_update_created_playlists):
         new_id = playlist_id_found
 
         playlist_tracks = list(map(lambda track: {'uri': track['track']['uri']}, requests.get_request(
@@ -227,24 +251,25 @@
         'id': row['id'],
         'name': row['name'],
         'genres': row['genres'],
         'artists': row['artists'],
         'popularity': row['popularity'],
         'added_at': row['added_at'],
         'danceability': row['danceability'],
+        'loudness': row['loudness'],
         'energy': row['energy'],
         'instrumentalness': row['instrumentalness'],
         'tempo': row['tempo'],
         'valence': row['valence'],
         'genres_indexed': row['genres_indexed'],
         'artists_indexed': row['artists_indexed']
     }
 
 
-def knn_prepared_data(playlist: pd.DataFrame) -> 'list[dict[str,]]':
+def knn_prepared_data(playlist: pd.DataFrame) -> 'list[dict[str, Any]]':
     """Function to prepare the data for the algorithm which calculates the distances between the songs
 
     Note:
         It will make a copy of the playlist to a list, to avoid changing the original DataFrame playlist.
         And also leave it in an easier to 'iterate over' format
 
     Args:
@@ -258,29 +283,30 @@
             'id',
             'name',
             'genres',
             'artists',
             'popularity',
             'added_at',
             'danceability',
+            'loudness',
             'energy',
             'instrumentalness',
             'tempo',
             'valence',
             'genres_indexed',
             'artists_indexed'
         ]
     ].copy()
 
     data['track_dict'] = data.apply(create_playlist_data_dict, axis=1)
 
     return data['track_dict'].tolist()
 
 
-def plot_bar_chart(df: pd.DataFrame, chart_title: str = None, top: int = 10, plot_max: bool = True):
+def plot_bar_chart(df: pd.DataFrame, chart_title: Union[str, None] = None, top: int = 10, plot_max: bool = True):
     """Plot a bar Chart with the top values from the dictionary
 
     Args:
         df (pd.DataFrame): DataFrame to plotthat contains the data
         chart_title (str, optional): label of the chart. Defaults to None
         top (int, optional): numbers of values to be in the chart. Defaults to 10
     """
```

## spotify_recommender_api/error.py

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Union, Any
 
 class HTTPRequestError(Exception):
     """Generic exception for HTTP Request Exceptions
         It can receive the error code and function name, and the function arguments, besides the message, to better help debugging the error
     """
     def __init__(
         self,
@@ -34,16 +34,16 @@
     def __init__(self, func_name=None, message=None, *args, **kwargs):
         super().__init__(*args, err_code='429 Too Many Requests', func_name=func_name, message=message, **kwargs)
 
 class AccessTokenExpiredError(HTTPRequestError):
     """Exception raised when the SpofifyAPI access token has expired
         It can receive the function name and the function arguments, besides the message, to better help debugging the error
     """
-    func: Callable
-    args: list
-    kwargs: 'dict[str,]'
+    func: Union[Callable, None]
+    args: 'tuple[Any]'
+    kwargs: 'dict[str, Any]'
 
-    def __init__(self, func_name: str = None, func: Callable = None, message: str = None, *args, **kwargs):
+    def __init__(self, func_name: Union[str, None] = None, func: Union[Callable, None] = None, message: Union[str, None] = None, *args, **kwargs):
         super().__init__(*args, err_code='401 Access Token Expired', func_name=func_name, message=message, **kwargs)
         self.func = func
         self.args = args
         self.kwargs = kwargs
```

## spotify_recommender_api/recommender.py

```diff
@@ -1,22 +1,22 @@
 import os
 import re
 import logging
 import operator
+import warnings
 import pandas as pd
 import spotify_recommender_api.util as util
 import spotify_recommender_api.core as core
 import spotify_recommender_api.authentication as auth
 import spotify_recommender_api.request_handler as requests
 from functools import reduce
-from spotify_recommender_api.sensitive import *
+from typing import Any, Union
+from spotify_recommender_api.sensitive import CLIENT_ID, CLIENT_SECRET
 from spotify_recommender_api.error import AccessTokenExpiredError
-
-
-pd.options.mode.chained_assignment = None
+warnings.filterwarnings('error')
 
 
 class SpotifyAPI:
     """
     Spotify API is the Class that provides access to the playlists recommendations
     """
 
@@ -43,16 +43,15 @@
                 else:
                     self.__update_created_files = True
 
             except FileNotFoundError as exc:
                 raise FileNotFoundError(
                     'The playlist with the specified ID does not exist in the CSV format, try again but selecting the "web" option, as the source for the playlist') from exc
 
-        self.__artists, self.__songs, self.__all_genres = list(map(lambda arr: arr if type(
-            arr) != 'str' else eval(arr), [df['artists'][0], df['songs'][0], df['all_genres'][0]]))
+        self.__artists, self.__songs, self.__all_genres = [eval(arr) if isinstance(arr, str) else arr for arr in [df['artists'][0], df['songs'][0], df['all_genres'][0]]]
 
         if self.__update_created_files:
             self.__playlist = pd.read_csv('playlist.csv')
         else:
             self.__playlist = pd.read_csv(f'{self.__base_playlist_name}.csv')
 
     def __get_playlist(self):
@@ -67,15 +66,15 @@
         self.__update_created_files = False
         if answer.lower() == 'csv':
             self.__get_playlist_from_csv()
             return False
 
         return True
 
-    def __get_song_genres(self, song: 'dict[str,]') -> 'list[str]':
+    def __get_song_genres(self, song: 'dict[str, Any]') -> 'list[str]':
         """
         Function that gets all the genres for a given song
 
         Args:
           song(dict[str,]): the song dictionary
 
         Returns:
@@ -117,24 +116,24 @@
                     headers=self.__headers,
                     url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=!s}'
                 )
                 for song in all_genres_res.json()["items"]:
                     (id, name, popularity, artist, added_at), song_genres = util.song_data(
                         song=song), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                        song=song, headers=self.__headers)
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
                     self.__songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "added_at": added_at,
                         "danceability": danceability,
+                        "loudness": loudness,
                         "energy": energy,
                         "instrumentalness": instrumentalness,
                         "tempo": tempo,
                         "valence": valence
                     })
                     self.__all_genres += song_genres
 
@@ -164,34 +163,35 @@
                         headers=self.__headers,
                         url=f'https://api.spotify.com/v1/me/tracks?limit=50&{offset=!s}'
                     )
                     for song in all_genres_res.json()["items"]:
                         (id, name, popularity, artist, added_at), song_genres = util.song_data(
                             song=song), self.__get_song_genres(song)
                         song['id'] = id
-                        danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                        danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
                             song=song, headers=self.__headers)
                         self.__songs.append({
                             "id": id,
                             "name": name,
                             "artists": artist,
                             "popularity": popularity,
                             "genres": song_genres,
                             "added_at": added_at,
                             "danceability": danceability,
+                            "loudness": loudness,
                             "energy": energy,
                             "instrumentalness": instrumentalness,
                             "tempo": tempo,
                             "valence": valence
                         })
                         self.__all_genres += song_genres
 
                 logging.info(f'Songs mapping complete: {total_song_count}/{total_song_count}')
 
-                self.__all_genres = list(set(self.__all_genres))
+                self.__all_genres: 'list[str]' = list(set(self.__all_genres))
 
             except AccessTokenExpiredError as e:
                 logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
@@ -211,33 +211,37 @@
 
         self.__all_artists = list(self.__artists.keys())
         playlist = pd.DataFrame(data=list(songs))
 
         playlist["genres_indexed"] = [
             util.item_list_indexed(
                 all_items=self.__all_genres,
-                items=eval(genre) if type(genre) == 'str' else genre,
+                items=eval(genre) if isinstance(genre, str) else genre,
             ) for genre in playlist["genres"]
         ]
         playlist["artists_indexed"] = [
             util.item_list_indexed(
                 all_items=self.__all_artists,
-                items=eval(artist) if type(
-                    artist) == 'str' else artist,
+                items=eval(artist) if isinstance(artist, str) else artist,
             ) for artist in playlist["artists"]
         ]
         playlist['id'] = playlist["id"].astype(str)
         playlist['name'] = playlist["name"].astype(str)
         playlist['popularity'] = playlist["popularity"].astype(int)
         playlist['added_at'] = pd.to_datetime(playlist["added_at"])
         playlist['danceability'] = playlist["danceability"].astype(float)
         playlist['energy'] = playlist["energy"].astype(float)
         playlist['instrumentalness'] = playlist["instrumentalness"].astype(float)
         playlist['tempo'] = playlist["tempo"].astype(float)
         playlist['valence'] = playlist["valence"].astype(float)
+        if 'loudness' not in playlist.columns:
+            playlist['loudness'] = 0
+            logging.warning('Since version 4.3.0, there is a new column "loudness" and in order to get it you will need to get the playlist from web and not csv, after that everything will work just as before')
+
+        playlist['loudness'] = playlist["loudness"].astype(float)
         self.__playlist = playlist
 
     def playlist_to_csv(self):
         """
         Function to convert playlist to CSV format
         Really useful if the package is being used in a .py file since it is not worth it to use it directly through web requests everytime even more when the playlist has not changed since last package usage
         """
@@ -263,28 +267,29 @@
                 'id',
                 'name',
                 'artists',
                 'genres',
                 'popularity',
                 'added_at',
                 'danceability',
+                'loudness',
                 'energy',
                 'instrumentalness',
                 'tempo',
                 'valence'
             ]
         ]
 
         playlist.to_csv(f'{self.__base_playlist_name}.csv')
 
     def select_playlist(
             self,
             user_id: str,
-            playlist_id: str = None,
-            playlist_url: str = None,
+            playlist_id: Union[str, None] = None,
+            playlist_url: Union[str, None] = None,
             liked_songs: bool = False,
             prepare_favorites: bool = False
         ) -> None:
         """Function to select a playlist to be mapped and be available on all the playlist related recommendation functions
 
         Args:
             user_id (str): Spotify User ID
@@ -348,15 +353,15 @@
         if self.__update_created_files:
             self.playlist_to_csv()
 
         self.__top_genres = self.__top_artists = self.__top_tracks = None
 
 
 
-    def __init__(self, auth_token: str, user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False, prepare_favorites: bool = False):
+    def __init__(self, auth_token: str, user_id: str, playlist_id: Union[str, None] = None, playlist_url: Union[str, None] = None, liked_songs: bool = False, prepare_favorites: bool = False):
         """Spotify API is the Class that provides access to the playlists recommendations
 
         Note:
             It will trigger most of the API functions and can take a good while to complete
 
 
         Args:
@@ -383,125 +388,125 @@
             user_id=user_id,
             liked_songs=liked_songs,
             playlist_id=playlist_id,
             playlist_url=playlist_url,
             prepare_favorites=prepare_favorites
         )
 
-    def __get_neighbors(self, song: str, K: int, song_dict: list, type: str = None) -> list:
+    def __get_neighbors(self, song: int, K: int, song_dict: list, type: Union[str, None] = None) -> list:
         """Function thats using the distance calculated above, returns the K nearest neighbors for a given song
 
         Args:
             song (str): song's index in the songs list
             K (int): desired number K of neighbors to be returned
             song_dict (list): the list of songs
             type (str, optional): Neighbor playlist type. Defaults to None.
 
         Returns:
             list: list neighbors
         """
+        if type is None:
+            return []
+
         distances = []
 
         for song_index, song_value in enumerate(song_dict):
             if song_index != song:
-                dist = core.compute_distance(
-                    song_a=song_dict[song], song_b=song_value, artist_recommendation='artist' in type)
+                dist = core.compute_distance(song_a=song_dict[song], song_b=song_value, artist_recommendation='artist' in type)
                 distances.append((song_index, dist))
 
         distances.sort(key=operator.itemgetter(1))
         return [[*distances[x]] for x in range(K)]
 
-    def __get_index_for_song(self, song: str) -> int:
+    def __get_index_for_song(self, song: Union[str, 'list[str]', None]) -> int:
         """Function that returns the index of a given song in the list of songs
 
         Args:
             song (str): song name
 
         Raises:
             ValueError: Playlist does not contain the song
 
         Returns:
             int: the index for the song
         """
         if song not in list(self.__playlist['name']):
             raise ValueError(f'Playlist does not contain the song {song!r}')
 
-        item = self.__playlist[[self.__playlist['name'][x] ==
-                                song for x in range(len(self.__playlist['name']))]]
-        index = item.index[0]
-        return index
+        item = self.__playlist.index[self.__playlist['name'] == song].tolist()
+
+        return item[0]
 
-    def __push_songs_to_playlist(self, full_uris: str, playlist_id: str):
+
+    def __push_songs_to_playlist(self, full_uris: str, playlist_id: Union[str, bool, None]):
         """Function to push soongs to a specified playlist
 
         Args:
             full_uris (str): list of song uri's
             playlist_id (str): playlist id
         """
-        full_uris = full_uris.split(',')
+        full_uris_list = full_uris.split(',')
 
-        if len(full_uris) <= 100:
-            uris = ','.join(full_uris)
-            add_songs_req = requests.post_request(
-                url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
+        if len(full_uris_list) <= 100:
+            uris = ','.join(full_uris_list)
+            add_songs_req = requests.post_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
 
         else:
 
-            for offset in range(0, len(full_uris), 100):
+            for offset in range(0, len(full_uris_list), 100):
+
+                uris = ','.join(full_uris_list[offset:offset + min(len(full_uris_list) - offset, 100)])
+                add_songs_req = requests.post_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
 
-                uris = ','.join(
-                    full_uris[offset:offset + min(len(full_uris) - offset, 100)])
-                add_songs_req = requests.post_request(
-                    url=f'https://api.spotify.com/v1/playlists/{playlist_id}/tracks?{uris=!s}', headers=self.__headers)
 
-    def __build_playlist(self, type: str, uris: str):
+    def __build_playlist(self, type: str, uris: str, add_info=None):
         """Function that builds the contents of a playlist
 
         Note:
             This function will change the user's library by filling the previously created empty playlist
 
         Args:
             type (str): the type of the playlist being created
             uris (str): string containing all song uris in the format the Spotify API expects
         """
         if not uris:
             raise ValueError('Invalid value for the song uris')
 
+        additional_information_by_type = {
+            'mood': add_info,
+            'song': getattr(self, '_SpotifyAPI__song_name', None),
+            'artist': getattr(self, '_SpotifyAPI__artist_name', None),
+            'profile-recommendation': [
+                getattr(self, '_SpotifyAPI__profile_recommendation_criteria', None),
+                getattr(self, '_SpotifyAPI__profile_recommendation_date', None)
+            ],
+            'playlist-recommendation': [
+                getattr(self, '_SpotifyAPI__playlist_recommendation_criteria', None),
+                getattr(self, '_SpotifyAPI__playlist_recommendation_date', None),
+                getattr(self, '_SpotifyAPI__playlist_recommendation_time_range', None)
+            ],
+            'general-recommendation': [
+                getattr(self, '_SpotifyAPI__general_recommendation_description', None),
+                getattr(self, '_SpotifyAPI__general_recommendation_description_types', None)
+            ],
+        }
+
+
         playlist_id = core.create_playlist(
             type=type,
             headers=self.__headers,
             user_id=self.__user_id,
             base_playlist_name=self.__base_playlist_name,
             _update_created_playlists=self.__update_created_files,
-            additional_info=self.__song_name
-            if type == "song"
-            else self.__artist_name
-            if "artist" in type
-            else [
-                self.__profile_recommendation_criteria,
-                self.__profile_recommendation_date
-            ]
-            if type == 'profile-recommendation'
-            else [
-                self.__playlist_recommendation_criteria,
-                self.__playlist_recommendation_date,
-                self.__playlist_recommendation_time_range
-            ]
-            if type == 'playlist-recommendation'
-            else [
-                self.__general_recommendation_description,
-                self.__general_recommendation_description_types
-            ]
-            if type == 'general-recommendation'
-            else None,
+            additional_info=additional_information_by_type['artist'] if "artist" in type else additional_information_by_type.get(type)
         )
 
         self.__push_songs_to_playlist(full_uris=uris, playlist_id=playlist_id)
 
-    def __write_playlist(self, type: str, K: int, additional_info=None):
+    def __write_playlist(self, type: str, K: int, additional_info: Union[str, 'list[str]', None] = None):
         """Function that writes a new playlist with the recommendations for the given type
         type: the type of the playlist being created ('song', 'short', 'medium'):
          - 'song': a playlist related to a song
          - 'short': a playlist related to the short term favorites for that given user
          - 'medium': a playlist related to the medium term favorites for that given user
 
         Note:
@@ -516,52 +521,49 @@
             ValueError: Value for K must be between 1 and 1500
             ValueError: Invalid type
         """
         if K > 1500:
             logging.warning('K limit exceded. Maximum value for K is 1500')
             K = 1500
         elif K < 1:
-            raise ValueError(
-                f'Value for K must be between 1 and 1500 on creation of {type} playlist. {additional_info=!r}')
-        uris = ''
+            raise ValueError(f'Value for K must be between 1 and 1500 on creation of {type} playlist. {additional_info=!r}')
+
         if type == 'song':
             index = self.__get_index_for_song(additional_info)
-            uris = f'spotify:track:{self.__song_dict[index]["id"]}'
-            for neighbor in self.__get_recommendations('song', additional_info, K)['id']:
-                uris += f',spotify:track:{neighbor}'
+            uris = f'spotify:track:{self.__song_dict[index]["id"]},'
+
+            uris += ','.join([f'spotify:track:{neighbor}' for neighbor in self.__get_recommendations('song', additional_info, K)['id']])
 
         elif type in {'medium', 'short'}:
             ids = self.__medium_fav['id'] if type == 'medium' else self.__short_fav['id']
-            for neighbor in ids:
-                uris += f',spotify:track:{neighbor}'
 
-            uris = uris[1:]
+            uris = ','.join([f'spotify:track:{song}' for song in ids])
 
-        elif any(x in type for x in ['most-listened', 'artist', '-recommendation']):
+        elif any(x in type for x in ['most-listened', 'artist', '-recommendation', 'mood']):
             ids = additional_info
-            for song in ids:
-                uris += f',spotify:track:{song}'
-
-            uris = uris[1:]
+            if ids is None: # only because of strict type checking enforncing that if it can be None it souldnt be part of an iteration
+                ids = []
+            uris = ','.join([f'spotify:track:{song}' for song in ids])
 
         else:
+            uris = ''
             raise ValueError('Invalid type')
 
-        self.__build_playlist(type=type, uris=uris)
+        self.__build_playlist(type=type, uris=uris, add_info=getattr(self, '_SpotifyAPI__mood', None))
 
     def get_recommendations_for_song(
         self,
         K: int,
         song: str,
         generate_csv: bool = False,
         with_distance: bool = False,
         build_playlist: bool = False,
         generate_parquet: bool = False,
         print_base_caracteristics: bool = False
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, None]:
         """Playlist which centralises the actions for a recommendation made for a given song
 
         Note
             The build_playlist option when set to True will change the user's library
 
 
         Args:
@@ -588,18 +590,16 @@
 
             df = self.__get_recommendations('song', song, K)
             playlist_name = f'{song} Related'
 
             if print_base_caracteristics:
                 index = self.__get_index_for_song(song)
                 caracteristics = self.__song_dict[index]
-                name, genres, artists, popularity, _, danceability, energy, instrumentalness, tempo, valence = list(
-                    caracteristics.values())[1:11]
-                util.print_base_caracteristics(
-                    name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+                name, genres, artists, popularity, _, danceability, loudness, energy, instrumentalness, tempo, valence = list(caracteristics.values())[1:11]
+                util.print_base_caracteristics(name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence)
 
             if generate_csv:
                 df.to_csv(f'{playlist_name}.csv')
 
             if generate_parquet:
                 df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
 
@@ -620,58 +620,58 @@
                     break
 
             return df if with_distance else df.drop(columns=['distance'])
 
         except ValueError as e:
             logging.error(e)
 
-    def __get_desired_dict_fields(self, index: int, song_dict: list = None) -> 'list[str]':
+    def __get_desired_dict_fields(self, index: int, song_dict: Union['list[dict[str, Any]]', None] = None) -> 'list[str]':
         """Function that returns the usual fields for a given song
 
         Args:
             index (int): The index of the song inside the song list
             song_dict (list, optional): song dictionary. Defaults to None.
 
         Returns:
             list[str]: list of fields of the desired song
         """
 
         if song_dict is None:
             song_dict = self.__song_dict
 
-        song_dict = song_dict[index]
+        desired_song_dict = song_dict[index]
 
         return [
-            song_dict['id'],
-            song_dict['name'],
-            song_dict['artists'],
-            song_dict['genres'],
-            song_dict['popularity'],
-            song_dict['added_at'],
-            song_dict['danceability'],
-            song_dict['energy'],
-            song_dict['instrumentalness'],
-            song_dict['tempo'],
-            song_dict['valence']
+            desired_song_dict['id'],
+            desired_song_dict['name'],
+            desired_song_dict['artists'],
+            desired_song_dict['genres'],
+            desired_song_dict['popularity'],
+            desired_song_dict['added_at'],
+            desired_song_dict['danceability'],
+            desired_song_dict['loudness'],
+            desired_song_dict['energy'],
+            desired_song_dict['instrumentalness'],
+            desired_song_dict['tempo'],
+            desired_song_dict['valence']
         ]
 
-    def __song_list_to_df(self, neighbors: list, song_dict: list = None) -> pd.DataFrame:
+    def __song_list_to_df(self, neighbors: list, song_dict: Union['list[dict[str, Any]]', None] = None) -> pd.DataFrame:
         """Function that returns DataFrame representation of the list of neighbor songs
 
         Args:
             neighbors (list): list of a given song's neighbors
             song_dict (list, optional): song dictionary. Defaults to None.
 
         Returns:
             pd.DataFrame: Song DataFrame
         """
-        data = list(map(lambda x: list(self.__get_desired_dict_fields(
-            x[0], song_dict=song_dict) + [x[1]]), neighbors))
+        data = [list(self.__get_desired_dict_fields(neighbor[0], song_dict=song_dict) + [neighbor[1]]) for neighbor in neighbors]
 
-        return pd.DataFrame(data=data, columns=['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'energy', 'instrumentalness', 'tempo', 'valence', 'distance'])
+        return pd.DataFrame(data=data, columns=['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence', 'distance'])
 
     def __get_recommendations(self, type: str, info, K: int = 51) -> pd.DataFrame:
         """General purpose function to get recommendations for any type supported by the package
 
         Args:
             info (Any): the changed song_dict list if the type is short or medium or else it is the name of the song to get recommendations from
             K (int, optional): desired number K of neighbors to be returned. Defaults to 51.
@@ -696,16 +696,15 @@
         if type == 'song':
             index = self.__get_index_for_song(info)
         elif type in {'medium', 'short', 'artist-related'}:
             index = len(info) - 1
         else:
             raise ValueError('Type does not correspond to a valid option')
         song_dict = self.__song_dict if type == 'song' else info
-        neighbors = self.__get_neighbors(
-            song=index, K=K, song_dict=song_dict, type=type)
+        neighbors = self.__get_neighbors(song=index, K=K, song_dict=song_dict, type=type)
         return self.__song_list_to_df(neighbors, song_dict=song_dict)
 
     def __get_genres(self, genres: 'list[list[str]]') -> 'list[str]':
         """Function to unite all the genres from different songs into one list of genres
 
         Args:
             genres (list[list[str]]): the list of lists of genres from the different songs
@@ -749,15 +748,15 @@
 
         for index in range(1, len(artists)):
             for i in range(len(all_artists)):
                 all_artists[i] = all_artists[i] or artists[index][i]
 
         return all_artists
 
-    def __get_top_5(self, time_range='medium') -> 'list[dict[str,]]':
+    def __get_top_5(self, time_range='medium') -> 'list[dict[str, Any]]':
         """Function that gets and initially formats the top 5 songs in a given time_range
 
         Args:
             time_range (str, optional): The time range to get the top 5 songs from ('medium', 'short'). Defaults to 'medium'.
 
         Raises:
             ValueError: time_range must be either medium_term or short_term
@@ -776,72 +775,66 @@
                 'name': song['name'],
                 'genres': self.__get_song_genres(song),
                 'artists': list(
                     map(lambda artist: artist['name'], song['artists'])
                 ),
                 'popularity': song['popularity'],
                 'danceability': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'danceability'],
-                'energy': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'danceability'],
+                'loudness': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'loudness'],
+                'energy': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'energy'],
                 'instrumentalness': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'instrumentalness'],
                 'tempo': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'tempo'],
                 'valence': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'valence']
             }, list(
                 filter(lambda song: song['name'] in list(
                     self.__playlist['name']), top_5['items'])
             ))
         )
 
-    def __find_recommendations_to_songs(self, base_songs: 'list[dict[str, ]]', subset_name: str) -> 'dict[str,]':
+    def __find_recommendations_to_songs(self, base_songs: 'list[dict[str, Any]]', subset_name: str) -> 'dict[str, Any]':
         """Generates a song format record from a list of songs, with all the information the "song-based" recommendation needs
 
         Args:
             base_songs (list[dict[str, Any]]): List of base songs
             subset_name (str): Name of thihs subset of songs (barely seen, unless the dataframe is printed with this record in it)
 
         Returns:
             dict[str, Any]: New song fomat record with the information gathered from the list of base songs
         """
-        temp_genres = list(reduce(lambda acc, x: acc +
-                           list(set(x['genres']) - set(acc)), base_songs, []))
+        temp_genres = list(reduce(lambda acc, x: acc + list(set(x['genres']) - set(acc)), base_songs, []))
 
-        temp_artists = list(
-            reduce(lambda acc, x: acc + list(set(x['artists']) - set(acc)), base_songs, []))
+        temp_artists = list(reduce(lambda acc, x: acc + list(set(x['artists']) - set(acc)), base_songs, []))
 
         latest_fav = {
             'id': "",
             'name': subset_name,
             'genres': temp_genres,
             'artists': temp_artists,
-            'genres_indexed': self.__get_genres(list(map(lambda song: util.item_list_indexed(song['genres'], all_items=self.__all_genres), base_songs)))
+            'genres_indexed': self.__get_genres([util.item_list_indexed(song['genres'], all_items=self.__all_genres) for song in base_songs])
         }
 
-        latest_fav['artists_indexed'] = self.__get_artists(list(map(
-            lambda song: util.item_list_indexed(song['artists'], all_items=self.__all_artists), base_songs)))
+        latest_fav['artists_indexed'] = self.__get_artists([util.item_list_indexed(song['artists'], all_items=self.__all_artists) for song in base_songs])
+
+        latest_fav['popularity'] = int(round(reduce(lambda acc, song: acc + int(song['popularity']), base_songs, 0) / len(base_songs)))
 
-        latest_fav['popularity'] = int(round(reduce(
-            lambda acc, song: acc + int(song['popularity']), base_songs, 0) / len(base_songs)))
+        latest_fav['danceability'] = float(reduce(lambda acc, song: acc + float(song['danceability']), base_songs, 0) / len(base_songs))
 
-        latest_fav['danceability'] = float(reduce(
-            lambda acc, song: acc + float(song['danceability']), base_songs, 0) / len(base_songs))
+        latest_fav['loudness'] = float(reduce(lambda acc, song: acc + float(song['loudness']), base_songs, 0) / len(base_songs))
 
-        latest_fav['energy'] = float(reduce(
-            lambda acc, song: acc + float(song['energy']), base_songs, 0) / len(base_songs))
+        latest_fav['energy'] = float(reduce(lambda acc, song: acc + float(song['energy']), base_songs, 0) / len(base_songs))
 
-        latest_fav['instrumentalness'] = float(reduce(
-            lambda acc, song: acc + float(song['instrumentalness']), base_songs, 0) / len(base_songs))
+        latest_fav['instrumentalness'] = float(reduce(lambda acc, song: acc + float(song['instrumentalness']), base_songs, 0) / len(base_songs))
 
-        latest_fav['tempo'] = float(reduce(
-            lambda acc, song: acc + float(song['tempo']), base_songs, 0) / len(base_songs))
+        latest_fav['tempo'] = float(reduce(lambda acc, song: acc + float(song['tempo']), base_songs, 0) / len(base_songs))
 
-        latest_fav['valence'] = float(reduce(
-            lambda acc, song: acc + float(song['valence']), base_songs, 0) / len(base_songs))
+        latest_fav['valence'] = float(reduce(lambda acc, song: acc + float(song['valence']), base_songs, 0) / len(base_songs))
 
         return latest_fav
 
-    def __prepare_fav_data(self, term: str) -> 'dict[str,]':
+    def __prepare_fav_data(self, term: str) -> 'dict[str, Any]':
         """Function that expands on the formatting of the top_5 some time_range favorites
 
         Args:
             term (str): The time range to get the top 5 songs from ('medium', 'short')
 
         Returns:
             dict[str,]: recommendations for the favorite songs
@@ -849,15 +842,15 @@
         top_5_songs = self.__get_top_5(term)
 
         return self.__find_recommendations_to_songs(
             base_songs=top_5_songs,
             subset_name="Recent-ish Favorites" if term == 'medium' else "Latest Favorites"
         )
 
-    def __end_prepared_fav_data(self, type: str) -> 'list[dict[str,]]':
+    def __end_prepared_fav_data(self, type: str) -> 'list[dict[str, Any]]':
         """Final preparation for favorite data before getting visible
 
         Args:
             type (str): Playlist creation type
 
         Returns:
             list[dict[str,]]: song dictionary
@@ -869,24 +862,24 @@
 
     def get_playlist(self) -> pd.DataFrame:
         """Function that returns the playlist as pandas DataFrame with the needed, human readable, columns
 
         Returns:
             pd.DataFrame: Playlist DataFrame
         """
-        return self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']]
+        return self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
 
     @util.deprecated
     def get_short_term_favorites_playlist(
         self,
         generate_csv: bool = False,
         with_distance: bool = False,
         build_playlist: bool = False,
         generate_parquet: bool = False,
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, None]:
         """###DEPRECATED METHOD###\n
         Playlist which centralises the actions for a recommendation made for top 5 songs short term
 
         Note
             The build_playlist option when set to True will change the user's library
 
         Args:
@@ -910,15 +903,21 @@
 
         if build_playlist:
             self.__write_playlist('short', 51)
 
         return df if with_distance else df.drop(columns=['distance'])
 
     @util.deprecated
-    def get_medium_term_favorites_playlist(self, with_distance: bool = False, generate_csv: bool = False, generate_parquet: bool = False, build_playlist: bool = False) -> pd.DataFrame:
+    def get_medium_term_favorites_playlist(
+            self,
+            with_distance: bool = False,
+            generate_csv: bool = False,
+            generate_parquet: bool = False,
+            build_playlist: bool = False
+        ) -> Union[pd.DataFrame, None]:
         """###DEPRECATED METHOD###\n
         Playlist which centralises the actions for a recommendation made for top 5 songs medium term
 
         Note
             The build_playlist option when set to True will change the user's library
 
         Args:
@@ -948,18 +947,16 @@
     def __prepare_favorites_playlist(self):
         """###DEPRECATED METHOD###\n
         Note: Although this method and the whole medium and short term favorite category is deprecated, this method will stil run, since somebody may want to use it. Having that said, I do not recommend it
 
         Automatic creation of both the favorites related recommendations
         """
         try:
-            self.__short_fav = self.__get_recommendations(
-                'short',  self.__end_prepared_fav_data('short'))
-            self.__medium_fav = self.__get_recommendations(
-                'medium',  self.__end_prepared_fav_data('medium'))
+            self.__short_fav = self.__get_recommendations('short',  self.__end_prepared_fav_data('short'))
+            self.__medium_fav = self.__get_recommendations('medium',  self.__end_prepared_fav_data('medium'))
         except ValueError:
             return
 
     def get_most_listened(self, time_range: str = 'long', K: int = 50, build_playlist: bool = False) -> pd.DataFrame:
         """Function that creates the most-listened songs playlist for a given period of time in the users profile
 
         Args:
@@ -971,47 +968,62 @@
             ValueError: Value for K must be between 1 and 1500
 
 
         Returns:
             pd.DataFrame: pandas DataFrame containing the top K songs in the time range
         """
         if time_range not in ['long', 'medium', 'short']:
-            raise ValueError(
-                'time_range must be long, medium or short')
+            raise ValueError('time_range must be long, medium or short')
 
         if not (1 < K <= 1500):
-            raise ValueError(
-                f'Value for K must be between 1 and 1500: {time_range} term most listened')
+            raise ValueError(f'Value for K must be between 1 and 1500: {time_range} term most listened')
 
-        top = requests.get_request(
-            url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
+        top = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
 
-        top_songs = list(map(lambda song: {'id': song['id'], 'name': song['name'], 'genres': self.__get_song_genres(song), 'artists': list(map(
-            lambda artist: artist['name'], song['artists'])), 'popularity': song['popularity']}, top['items']))
+        top_songs = [
+            {
+                'id': song['id'],
+                'name': song['name'],
+                'popularity': song['popularity'],
+                'genres': self.__get_song_genres(song),
+                'artists': [artist['name'] for artist in song['artists']]
+            }
+            for song in top['items']
+        ]
 
         for _ in range(2):
             try:
 
                 if build_playlist:
-                    self.__write_playlist(
-                        f'most-listened-{time_range}', K, additional_info=list(map(lambda x: x['id'], top_songs)))
+                    self.__write_playlist(f'most-listened-{time_range}', K, additional_info=[x['id'] for x in top_songs])
 
             except AccessTokenExpiredError as e:
                 logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
-        return pd.DataFrame(data=list(map(lambda x: {'name': x['name'], 'genres': x['genres'], 'artists': x['artists'], 'popularity': x['popularity']}, top_songs)), columns=['name', 'artists', 'genres', 'popularity'])
+        return pd.DataFrame(
+            data=[
+                {
+                    'name': x['name'],
+                    'genres': x['genres'],
+                    'artists': x['artists'],
+                    'popularity': x['popularity']
+                }
+                for x in top_songs
+            ],
+            columns=['name', 'artists', 'genres', 'popularity']
+        )
 
-    def update_all_generated_playlists(self, *, K: int = None, playlist_types_to_update: 'list[str]' = None):
+    def update_all_generated_playlists(self, *, K: Union[int, None] = None, playlist_types_to_update: Union['list[str]', None] = None):
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
 
         Keyword Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
@@ -1023,15 +1035,15 @@
         total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
 
         playlists = []
 
         for offset in range(0, total_playlist_count, 50):
             request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
 
-            playlists += list(map(lambda playlist: (playlist['id'], playlist['name'], playlist['description'], playlist['tracks']['total']), request['items']))
+            playlists += [(playlist['id'], playlist['name'], playlist['description'], playlist['tracks']['total']) for playlist in request['items']]
 
         for _, name, description, total_tracks in playlists:
             try:
                 if K is not None:
                     total_tracks = K
                 if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
                     self.get_most_listened(time_range=name.split(" ")[0].lower(), K=total_tracks, build_playlist=True)
@@ -1096,15 +1108,15 @@
                         build_playlist=True,
                         main_criteria=criteria,
                     )
 
             except ValueError as e:
                 logging.error(f"Unfortunately we couldn't update a playlist because\n {e}")
 
-    def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> pd.DataFrame:
+    def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
         """Calculates the amount of times each genre was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. Must be 5, 10, 15 or False. No chart will be plotted if set to False. Defaults to False.
 
         Raises:
@@ -1155,15 +1167,15 @@
 
         if plot_top:
             core.plot_bar_chart(df=df, top=plot_top, plot_max=reduce(
                 lambda x, y: x + y, df['rate'][1:4], 0) >= 0.50)
 
         return df
 
-    def get_playlist_trending_artists(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> pd.DataFrame:
+    def get_playlist_trending_artists(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
         """Calculates the amount of times each artist was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. No chart will be plotted if set to False. Defaults to False.
 
         Raises:
@@ -1255,63 +1267,70 @@
 
         if not len(artist_songs):
             raise ValueError(
                 f'{artist_name = } does not exist in the playlist')
 
         self.__artist_name = artist_name
 
-        columns = ['id', 'name', 'artists', 'genres', 'popularity', 'added_at',
-                   'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']
+        columns = ['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']
 
         if complete_with_similar:
-            artist_songs_record_song_dict = list(map(
-                lambda x: {
+            artist_songs_record_song_dict = [{
                     'id': '',
-                    'name': x['name'],
-                    'artists': x['artists'],
-                    'genres': x['genres'],
-                    'artists_indexed': x['artists_indexed'],
-                    'genres_indexed': x['genres_indexed'],
-                    'popularity': x['popularity'],
-                    'added_at': x['added_at'],
-                    'danceability': x['danceability'],
-                    'energy': x['energy'],
-                    'instrumentalness': x['instrumentalness'],
-                    'tempo': x['tempo'],
-                    'valence': x['valence']
-                },
-                list(filter(lambda x: artist_name in x['artists'], self.__song_dict))
-            ))
+                    'name': song['name'],
+                    'artists': song['artists'],
+                    'genres': song['genres'],
+                    'artists_indexed': song['artists_indexed'],
+                    'genres_indexed': song['genres_indexed'],
+                    'popularity': song['popularity'],
+                    'added_at': song['added_at'],
+                    'danceability': song['danceability'],
+                    'loudness': song['loudness'],
+                    'energy': song['energy'],
+                    'instrumentalness': song['instrumentalness'],
+                    'tempo': song['tempo'],
+                    'valence': song['valence']
+                }
+                for song in [
+                    song
+                    for song in self.__song_dict
+                    if artist_name in song['artists']
+                ]
+            ]
 
             artist_songs_record = self.__find_recommendations_to_songs(base_songs=artist_songs_record_song_dict, subset_name=f"{artist_name} Mix")
 
-            song_dict = list(map(
-                lambda x: {
-                    'id': x['id'],
-                    'name': x['name'],
-                    'artists': x['artists'],
-                    'genres': x['genres'],
-                    'artists_indexed': x['artists_indexed'],
-                    'genres_indexed': x['genres_indexed'],
-                    'popularity': x['popularity'],
-                    'added_at': x['added_at'],
-                    'danceability': x['danceability'],
-                    'energy': x['energy'],
-                    'instrumentalness': x['instrumentalness'],
-                    'tempo': x['tempo'],
-                    'valence': x['valence']
-                },
-                list(filter(lambda x: artist_name not in x['artists'], self.__song_dict))
-            ))
+            song_dict = [{
+                    'id': song['id'],
+                    'name': song['name'],
+                    'artists': song['artists'],
+                    'genres': song['genres'],
+                    'artists_indexed': song['artists_indexed'],
+                    'genres_indexed': song['genres_indexed'],
+                    'popularity': song['popularity'],
+                    'added_at': song['added_at'],
+                    'danceability': song['danceability'],
+                    'loudness': song['loudness'],
+                    'energy': song['energy'],
+                    'instrumentalness': song['instrumentalness'],
+                    'tempo': song['tempo'],
+                    'valence': song['valence']
+                }
+                for song in [
+                    song
+                    for song in self.__song_dict
+                    if artist_name in song['artists']
+                ]
+            ]
 
             song_dict.append(artist_songs_record)
 
             mix_songs = self.__get_recommendations('artist-related', song_dict, K=K-len(artist_songs) if len(artist_songs) < K else len(artist_songs) // 3)
 
-            ids = pd.concat([artist_songs['id'], mix_songs['id']])
+            ids = pd.concat([artist_songs['id'], mix_songs['id']]).tolist()
 
             if with_distance:
                 df = artist_songs[columns]
 
                 columns.append('distance')
 
                 df['distance'] = pd.to_numeric(0)
@@ -1323,32 +1342,33 @@
 
             if print_base_caracteristics and not _auto:
                 name = artist_songs_record['name']
                 genres = artist_songs_record['genres']
                 artists = artist_songs_record['artists']
                 popularity = artist_songs_record['popularity']
                 danceability = artist_songs_record['danceability']
+                loudness = artist_songs_record['loudness']
                 energy = artist_songs_record['energy']
                 instrumentalness = artist_songs_record['instrumentalness']
                 tempo = artist_songs_record['tempo']
                 valence = artist_songs_record['valence']
-                util.print_base_caracteristics(name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+                util.print_base_caracteristics(name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence)
 
         elif not _auto and len(artist_songs) < K:
             logging.info(f'Playlist has only {len(artist_songs)} songs')
             logging.info(f'To fill the {K = } number of songs, consider using the flag complete_with_similar')
-            ids = artist_songs['id']
+            ids = artist_songs['id'].tolist()
             df = artist_songs[columns]
 
         elif ensure_all_artist_songs:
-            ids = artist_songs['id']
+            ids = artist_songs['id'].tolist()
             df = artist_songs[columns]
 
         else:
-            ids = artist_songs['id'][:K]
+            ids = artist_songs['id'][:K].tolist()
             df = artist_songs[columns][:K]
 
         if build_playlist:
             self.__write_playlist(
                 K=K,
                 type=f'artist{"-related" if complete_with_similar else "-full" if ensure_all_artist_songs else ""}',
                 additional_info=ids
@@ -1369,160 +1389,199 @@
             - instrumentalness: Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content
             - tempo: The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
             - valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
 
         Returns:
             dict[str, dict]: The dictionary with the maximum and minimum values for each audio feature used in the package
         """
-        df = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity',
-                              'added_at', 'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']]
+        df = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity','added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
 
         df_danceability = df.sort_values('danceability', ascending=True)
+        df_loudness = df.sort_values('loudness', ascending=True)
         df_energy = df.sort_values('energy', ascending=True)
-        df_instrumentalness = df.sort_values(
-            'instrumentalness', ascending=True)
+        df_instrumentalness = df.sort_values('instrumentalness', ascending=True)
         df_tempo = df.sort_values('tempo', ascending=True)
         df_valence = df.sort_values('valence', ascending=True)
         max_danceability = df_danceability.tail(n=1).reset_index(drop=True)
         min_danceability = df_danceability.head(n=1).reset_index(drop=True)
+        max_loudness = df_loudness.tail(n=1).reset_index(drop=True)
+        min_loudness = df_loudness.head(n=1).reset_index(drop=True)
         max_energy = df_energy.tail(n=1).reset_index(drop=True)
         min_energy = df_energy.head(n=1).reset_index(drop=True)
         max_instrumentalness = df_instrumentalness.tail(n=1).reset_index(drop=True)
         min_instrumentalness = df_instrumentalness.head(n=1).reset_index(drop=True)
         max_tempo = df_tempo.tail(n=1).reset_index(drop=True)
         min_tempo = df_tempo.head(n=1).reset_index(drop=True)
         max_valence = df_valence.tail(n=1).reset_index(drop=True)
         min_valence = df_valence.head(n=1).reset_index(drop=True)
 
         return {
+            'max_loudness': {
+                'id': max_loudness['id'][0],
+                'name': max_loudness['name'][0],
+                'genres': max_loudness['genres'][0],
+                'artists': max_loudness['artists'][0],
+                'popularity': max_loudness['popularity'][0],
+                'added_at': max_loudness['added_at'][0],
+                'danceability': max_loudness['danceability'][0],
+                'loudness': max_loudness['loudness'][0],
+                'energy': max_loudness['energy'][0],
+                'instrumentalness': max_loudness['instrumentalness'][0],
+                'tempo': max_loudness['tempo'][0],
+                'valence': max_loudness['valence'][0]
+            },
+            'min_loudness': {
+                'id': min_loudness['id'][0],
+                'name': min_loudness['name'][0],
+                'genres': min_loudness['genres'][0],
+                'artists': min_loudness['artists'][0],
+                'popularity': min_loudness['popularity'][0],
+                'added_at': min_loudness['added_at'][0],
+                'danceability': min_loudness['danceability'][0],
+                'loudness': min_loudness['loudness'][0],
+                'energy': min_loudness['energy'][0],
+                'instrumentalness': min_loudness['instrumentalness'][0],
+                'tempo': min_loudness['tempo'][0],
+                'valence': min_loudness['valence'][0]
+            },
             'max_danceability': {
                 'id': max_danceability['id'][0],
                 'name': max_danceability['name'][0],
                 'genres': max_danceability['genres'][0],
                 'artists': max_danceability['artists'][0],
                 'popularity': max_danceability['popularity'][0],
                 'added_at': max_danceability['added_at'][0],
                 'danceability': max_danceability['danceability'][0],
+                'loudness': max_danceability['loudness'][0],
                 'energy': max_danceability['energy'][0],
                 'instrumentalness': max_danceability['instrumentalness'][0],
                 'tempo': max_danceability['tempo'][0],
                 'valence': max_danceability['valence'][0]
             },
             'min_danceability': {
                 'id': min_danceability['id'][0],
                 'name': min_danceability['name'][0],
                 'genres': min_danceability['genres'][0],
                 'artists': min_danceability['artists'][0],
                 'popularity': min_danceability['popularity'][0],
                 'added_at': min_danceability['added_at'][0],
                 'danceability': min_danceability['danceability'][0],
+                'loudness': min_danceability['loudness'][0],
                 'energy': min_danceability['energy'][0],
                 'instrumentalness': min_danceability['instrumentalness'][0],
                 'tempo': min_danceability['tempo'][0],
                 'valence': min_danceability['valence'][0]
             },
             'max_energy': {
                 'id': max_energy['id'][0],
                 'name': max_energy['name'][0],
                 'genres': max_energy['genres'][0],
                 'artists': max_energy['artists'][0],
                 'popularity': max_energy['popularity'][0],
                 'added_at': max_energy['added_at'][0],
                 'danceability': max_energy['danceability'][0],
+                'loudness': max_energy['loudness'][0],
                 'energy': max_energy['energy'][0],
                 'instrumentalness': max_energy['instrumentalness'][0],
                 'tempo': max_energy['tempo'][0],
                 'valence': max_energy['valence'][0]
             },
             'min_energy': {
                 'id': min_energy['id'][0],
                 'name': min_energy['name'][0],
                 'genres': min_energy['genres'][0],
                 'artists': min_energy['artists'][0],
                 'popularity': min_energy['popularity'][0],
                 'added_at': min_energy['added_at'][0],
                 'danceability': min_energy['danceability'][0],
+                'loudness': min_energy['loudness'][0],
                 'energy': min_energy['energy'][0],
                 'instrumentalness': min_energy['instrumentalness'][0],
                 'tempo': min_energy['tempo'][0],
                 'valence': min_energy['valence'][0]
             },
             'max_instrumentalness': {
                 'id': max_instrumentalness['id'][0],
                 'name': max_instrumentalness['name'][0],
                 'genres': max_instrumentalness['genres'][0],
                 'artists': max_instrumentalness['artists'][0],
                 'popularity': max_instrumentalness['popularity'][0],
                 'added_at': max_instrumentalness['added_at'][0],
                 'danceability': max_instrumentalness['danceability'][0],
+                'loudness': max_instrumentalness['loudness'][0],
                 'energy': max_instrumentalness['energy'][0],
                 'instrumentalness': max_instrumentalness['instrumentalness'][0],
                 'tempo': max_instrumentalness['tempo'][0],
                 'valence': max_instrumentalness['valence'][0]
             },
             'min_instrumentalness': {
                 'id': min_instrumentalness['id'][0],
                 'name': min_instrumentalness['name'][0],
                 'genres': min_instrumentalness['genres'][0],
                 'artists': min_instrumentalness['artists'][0],
                 'popularity': min_instrumentalness['popularity'][0],
                 'added_at': min_instrumentalness['added_at'][0],
                 'danceability': min_instrumentalness['danceability'][0],
+                'loudness': min_instrumentalness['loudness'][0],
                 'energy': min_instrumentalness['energy'][0],
                 'instrumentalness': min_instrumentalness['instrumentalness'][0],
                 'tempo': min_instrumentalness['tempo'][0],
                 'valence': min_instrumentalness['valence'][0]
             },
             'max_tempo': {
                 'id': max_tempo['id'][0],
                 'name': max_tempo['name'][0],
                 'genres': max_tempo['genres'][0],
                 'artists': max_tempo['artists'][0],
                 'popularity': max_tempo['popularity'][0],
                 'added_at': max_tempo['added_at'][0],
                 'danceability': max_tempo['danceability'][0],
+                'loudness': max_tempo['loudness'][0],
                 'energy': max_tempo['energy'][0],
                 'instrumentalness': max_tempo['instrumentalness'][0],
                 'tempo': max_tempo['tempo'][0],
                 'valence': max_tempo['valence'][0]
             },
             'min_tempo': {
                 'id': min_tempo['id'][0],
                 'name': min_tempo['name'][0],
                 'genres': min_tempo['genres'][0],
                 'artists': min_tempo['artists'][0],
                 'popularity': min_tempo['popularity'][0],
                 'added_at': min_tempo['added_at'][0],
                 'danceability': min_tempo['danceability'][0],
+                'loudness': min_tempo['loudness'][0],
                 'energy': min_tempo['energy'][0],
                 'instrumentalness': min_tempo['instrumentalness'][0],
                 'tempo': min_tempo['tempo'][0],
                 'valence': min_tempo['valence'][0]
             },
             'max_valence': {
                 'id': max_valence['id'][0],
                 'name': max_valence['name'][0],
                 'genres': max_valence['genres'][0],
                 'artists': max_valence['artists'][0],
                 'popularity': max_valence['popularity'][0],
                 'added_at': max_valence['added_at'][0],
                 'danceability': max_valence['danceability'][0],
+                'loudness': max_valence['loudness'][0],
                 'energy': max_valence['energy'][0],
                 'instrumentalness': max_valence['instrumentalness'][0],
                 'tempo': max_valence['tempo'][0],
                 'valence': max_valence['valence'][0]
             },
             'min_valence': {
                 'id': min_valence['id'][0],
                 'name': min_valence['name'][0],
                 'genres': min_valence['genres'][0],
                 'artists': min_valence['artists'][0],
                 'popularity': min_valence['popularity'][0],
                 'added_at': min_valence['added_at'][0],
                 'danceability': min_valence['danceability'][0],
+                'loudness': min_valence['loudness'][0],
                 'energy': min_valence['energy'][0],
                 'instrumentalness': min_valence['instrumentalness'][0],
                 'tempo': min_valence['tempo'][0],
                 'valence': min_valence['valence'][0]
             },
         }
 
@@ -1550,42 +1609,44 @@
 
     def audio_features_statistics(self) -> 'dict[str, float]':
         """FUnctions that returns the statistics (max, min and mean) for the audio features within the playlist
 
         Returns:
             dict[str, float]: The dictionary with the statistics
         """
-        df: pd.DataFrame = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity',
-                                            'added_at', 'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']]
+        df: pd.DataFrame = self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']]
 
         return {
             'min_tempo': df['tempo'].min(),
             'max_tempo': df['tempo'].max(),
             'mean_tempo': df['tempo'].mean(),
             'min_energy': df['energy'].min(),
             'max_energy': df['energy'].max(),
             'mean_energy': df['energy'].mean(),
             'min_valence': df['valence'].min(),
             'max_valence': df['valence'].max(),
             'mean_valence': df['valence'].mean(),
             'min_danceability': df['danceability'].min(),
             'max_danceability': df['danceability'].max(),
             'mean_danceability': df['danceability'].mean(),
+            'min_loudness': df['loudness'].min(),
+            'max_loudness': df['loudness'].max(),
+            'mean_loudness': df['loudness'].mean(),
             'min_instrumentalness': df['instrumentalness'].min(),
             'max_instrumentalness': df['instrumentalness'].max(),
             'mean_instrumentalness': df['instrumentalness'].mean(),
         }
 
     def get_profile_recommendation(
         self,
         K: int = 50,
         main_criteria: str = 'mixed',
         save_with_date: bool = False,
         build_playlist: bool = False,
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, None]:
         """Builds a Profile based recommendation
 
         Args:
             K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
             main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
             save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
             build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
@@ -1600,43 +1661,47 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
-        tracks = None
-        genres = None
-        artists = None
+        tracks = []
+        genres = []
+        artists = []
 
         for _ in range(2):
             try:
 
                 if main_criteria != 'tracks':
                     if self.__top_genres or self.__top_artists:
                         genres = self.__top_genres
                         artists = self.__top_artists
 
                     else:
                         top_artists_req = requests.get_request(
                             url='https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=5', headers=self.__headers).json()['items']
 
-                        artists = list(map(lambda x: x['id'], top_artists_req))
-                        genres = list(set(reduce(
-                            lambda x, y: x + y, list(map(lambda x: x['genres'], top_artists_req)), [])))[:5]
+                        artists = [artist['id'] for artist in top_artists_req]
+                        genres = list(set(reduce(lambda x, y: x + y, [artist['genres'] for artist in top_artists_req], [])))[:5]
                         self.__top_genres = genres
                         self.__top_artists = artists
 
                 if main_criteria not in ['artists']:
                     if self.__top_tracks:
                         tracks = self.__top_tracks
 
                     else:
-                        tracks = list(map(lambda x: x['id'], requests.get_request(
-                            url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+                        tracks = [
+                            track['id']
+                            for track in requests.get_request(
+                                headers=self.__headers,
+                                url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5'
+                            ).json()['items']
+                        ]
 
                         self.__top_tracks = tracks
 
                 url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
                 if main_criteria == 'artists':
                     url += f'&seed_artists={",".join(artists)}'
@@ -1652,26 +1717,25 @@
                 if not recommendations.get("tracks"):
                     logging.error(f'There was a problem creating the profile recommendations based on {main_criteria}')
                     return
 
                 songs = []
 
                 for song in recommendations["tracks"]:
-                    (id, name, popularity, artist), song_genres = util.song_data(
-                        song=song, added_at=False), self.__get_song_genres(song)
+                    (id, name, popularity, artist), song_genres = util.song_data(song=song, added_at=False), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                        song=song, headers=self.__headers)
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
                     songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "danceability": danceability,
+                        "loudness": loudness,
                         "energy": energy,
                         "instrumentalness": instrumentalness,
                         "tempo": tempo,
                         "valence": valence
                     })
 
                 recommendations_playlist = pd.DataFrame(data=songs)
@@ -1703,15 +1767,15 @@
     def get_playlist_recommendation(
         self,
         K: int = 50,
         time_range: str = 'all_time',
         main_criteria: str = 'mixed',
         save_with_date: bool = False,
         build_playlist: bool = False,
-    ) -> pd.DataFrame:
+    ) -> Union[pd.DataFrame, None]:
         """Builds a playlist based recommendation
 
         Args:
             K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             main_criteria (str, optional): Main criteria for the recommendations playlist. Can be one of the following: 'mixed', 'artists', 'tracks', 'genres'. Defaults to 'mixed'.
             save_with_date (bool, optional): Flag to save the recommendations playlist as a Point in Time Snapshot. Defaults to False.
@@ -1728,52 +1792,73 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
-        tracks = None
-        genres = None
-        artists = None
+        tracks = []
+        genres = []
+        artists = []
 
 
         for _ in range(2):
             try:
                 audio_statistics = self.audio_features_statistics()
 
                 if main_criteria not in ['genres', 'tracks']:
-                    top_artists_names = self.get_playlist_trending_artists(time_range=time_range)[
-                        'name'][1:6].tolist()
-                    artists = list(map(lambda x: requests.get_request(
-                        url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], top_artists_names))
+
+                    if (top_artists := self.get_playlist_trending_artists(time_range=time_range)) is None:
+                        return None
+
+                    top_artists_names = top_artists['name'][1:6].tolist()
+
+                    artists = [
+                        requests.get_request(
+                            headers=self.__headers,
+                            url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1'
+                        ).json()['artists']['items'][0]['id']
+                        for x in top_artists_names
+                    ]
 
                 if main_criteria not in ['artists']:
                     if self.__top_tracks:
                         tracks = self.__top_tracks
 
                     else:
-                        tracks = list(map(lambda x: x['id'], requests.get_request(url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+                        tracks = [
+                            track['id']
+                            for track in requests.get_request(
+                                headers=self.__headers,
+                                url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5',
+                            ).json()['items']
+                        ]
 
                         self.__top_tracks = tracks
                 if main_criteria != 'artists':
-                    genres = self.get_playlist_trending_genres(time_range=time_range)['name'][1:6].tolist()[:5]
+                    if (genres := self.get_playlist_trending_genres(time_range=time_range)) is None:
+                        return None
+
+                    genres = genres['name'][1:6].tolist()[:5]
 
                 min_tempo = audio_statistics['min_tempo'] * 0.8
                 max_tempo = audio_statistics['max_tempo'] * 1.2
                 target_tempo = audio_statistics['mean_tempo']
                 min_energy = audio_statistics['min_energy'] * 0.8
                 max_energy = audio_statistics['max_energy'] * 1.2
                 target_energy = audio_statistics['mean_energy']
                 min_valence = audio_statistics['min_valence'] * 0.8
                 max_valence = audio_statistics['max_valence'] * 1.2
                 target_valence = audio_statistics['mean_valence']
                 min_danceability = audio_statistics['min_danceability'] * 0.8
                 max_danceability = audio_statistics['max_danceability'] * 1.2
                 target_danceability = audio_statistics['mean_danceability']
+                min_loudness = audio_statistics['min_loudness'] * 0.8
+                max_loudness = audio_statistics['max_loudness'] * 1.2
+                target_loudness = audio_statistics['mean_loudness']
                 min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
                 max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
                 target_instrumentalness = audio_statistics['mean_instrumentalness']
 
                 url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
                 if main_criteria == 'artists':
@@ -1781,34 +1866,34 @@
 
                 elif main_criteria == 'genres':
                     url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
                 elif main_criteria == 'mixed':
                     url += f'&seed_tracks={",".join(tracks[:1])}&seed_artists={",".join(artists[:2])}&seed_genres={",".join(genres[:2])}'
                 elif main_criteria == 'tracks':
                     url += f'&seed_tracks={",".join(tracks[:2])}&seed_genres={",".join(genres[:3])}'
-                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_loudness=!s}&{max_loudness=!s}&{target_loudness=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
 
-                recommendations = requests.get_request(
-                    url=url, headers=self.__headers).json()
+                recommendations = requests.get_request(url=url, headers=self.__headers).json()
 
                 songs = []
 
                 for song in recommendations["tracks"]:
                     (id, name, popularity, artist), song_genres = util.song_data(
                         song=song, added_at=False), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
                         song=song, headers=self.__headers)
                     songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "danceability": danceability,
+                        "loudness": loudness,
                         "energy": energy,
                         "instrumentalness": instrumentalness,
                         "tempo": tempo,
                         "valence": valence
                     })
 
                 recommendations_playlist = pd.DataFrame(data=songs)
@@ -1837,21 +1922,20 @@
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
     def get_general_recommendation(
         self,
         K: int = 50,
-        genres_info: 'list[str]' = [],
-        artists_info: 'list[str]' = [],
+        genres_info: Union['list[str]', None] = None,
+        artists_info: Union['list[str]', None] = None,
         build_playlist: bool = False,
         use_main_playlist_audio_features: bool = False,
-        tracks_info: 'list[str]|list[tuple[str]]|list[list[str]]|dict[str, str]' = [
-        ],
-    ) -> pd.DataFrame:
+        tracks_info: Union['list[str]', 'list[tuple[str]]', 'list[list[str]]', 'dict[str, str]', None] = None,
+    ) -> Union[pd.DataFrame, None]:
         """Builds a general recommendation based on up to 5 items spread across artists, genres, and tracks.
 
         Args:
             K (int, optional): Number of songs in the recommendations playlist. Defaults to 50.
             genres_info (list[str], optional): list of the genre names to be used in the recommendation. Defaults to [].
             artists_info (list[str], optional): list of the artist names to be used in the recommendation. Defaults to [].
             build_playlist (bool, optional): Flag to build the recommendations playlist in the users library. Defaults to False.
@@ -1868,40 +1952,53 @@
             pd.DataFrame: Recommendations playlist
         """
 
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if not (genres_info or artists_info or tracks_info):
-            raise ValueError(
-                'At least one of the three args must be provided: genres_info, artists_info, tracks_info')
+            raise ValueError('At least one of the three args must be provided: genres_info, artists_info, tracks_info')
+
+        if genres_info is None:
+            genres_info = []
+
+        if artists_info is None:
+            artists_info = []
+
+        if tracks_info is None:
+            tracks_info = []
 
         if len(genres_info) + len(artists_info) + len(tracks_info) > 5:
-            raise ValueError(
-                'The sum of the number of items in each of the three args mustn\'t exceed 5')
+            raise ValueError('The sum of the number of items in each of the three args mustn\'t exceed 5')
 
         url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
         description = 'General Recommendation based on '
 
-        types = []
-
         for _ in range(2):
             try:
 
+                types = []
+
                 if artists_info:
                     types.append('artists')
                     description += 'the artists '
                     for artist in artists_info:
                         description += f'{artist}, '
 
                     description = ' and '.join(description[:-2].rsplit(', ', 1))
 
-                    artists = list(map(lambda x: requests.get_request(
-                        url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], artists_info))
+                    artists = [
+                        requests.get_request(
+                            headers=self.__headers,
+                            url=f'https://api.spotify.com/v1/search?q={artist}&type=artist&limit=1',
+                        ).json()['artists']['items'][0]['id']
+                        for artist in artists_info
+                    ]
+
                     url += f'&seed_artists={",".join(artists)}'
 
                     if len(artists_info) == 1:
                         description = description.replace('artists', 'artist')
 
                 if genres_info:
                     types.append('genres')
@@ -1939,18 +2036,23 @@
                         for song, artist in tracks_info.items():
                             description += f'{song} by {artist}, '
 
                         tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
                             'tracks']['items'][0]['id'] for song, artist in tracks_info.items()]
 
                     elif isinstance(tracks_info[0], tuple) or isinstance(tracks_info[0], list):
-                        for song, artist in tracks_info:
+                        for song, artist in tracks_info: # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
                             description += f'{song} by {artist}, '
-                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
-                            'tracks']['items'][0]['id'] for song, artist in tracks_info]
+                        tracks = [
+                            requests.get_request(
+                                headers=self.__headers,
+                                url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1',
+                            ).json()['tracks']['items'][0]['id']
+                        for song, artist in tracks_info # type: ignore because of the strict typing not recognizing that the condition above makes this a safe operation
+                    ]
 
                     elif isinstance(tracks_info[0], str):
                         for song in tracks_info:
                             description += f'{song}, '
                         tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1', headers=self.__headers).json()[
                             'tracks']['items'][0]['id'] for song in tracks_info]
 
@@ -1978,38 +2080,42 @@
                     target_energy = audio_statistics['mean_energy']
                     min_valence = audio_statistics['min_valence'] * 0.8
                     max_valence = audio_statistics['max_valence'] * 1.2
                     target_valence = audio_statistics['mean_valence']
                     min_danceability = audio_statistics['min_danceability'] * 0.8
                     max_danceability = audio_statistics['max_danceability'] * 1.2
                     target_danceability = audio_statistics['mean_danceability']
+                    min_loudness = audio_statistics['min_loudness'] * 0.8
+                    max_loudness = audio_statistics['max_loudness'] * 1.2
+                    target_loudness = audio_statistics['mean_loudness']
                     min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
                     max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
                     target_instrumentalness = audio_statistics['mean_instrumentalness']
 
-                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_loudness=!s}&{max_loudness=!s}&{target_loudness=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
 
                 recommendations = requests.get_request(
                     url=url, headers=self.__headers).json()
 
                 songs = []
 
                 for song in recommendations["tracks"]:
                     (id, name, popularity, artist), song_genres = util.song_data(
                         song=song, added_at=False), self.__get_song_genres(song)
                     song['id'] = id
-                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(
                         song=song, headers=self.__headers)
                     songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
                         "genres": song_genres,
                         "danceability": danceability,
+                        "loudness": loudness,
                         "energy": energy,
                         "instrumentalness": instrumentalness,
                         "tempo": tempo,
                         "valence": valence
                     })
 
                 recommendations_playlist = pd.DataFrame(data=songs)
@@ -2035,16 +2141,111 @@
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
+    def get_songs_by_mood(
+            self,
+            mood: str,
+            K: int = 50,
+            build_playlist: bool = False,
+            exclude_mostly_instrumental: bool = False
+        ) -> pd.DataFrame:
+        """Function to create playlists based on the general mood of a song
+
+        Args:
+            mood (str): The mood of the song. Can be 'happy', 'sad' or 'calm'
+            K (int, optional): Number of songs. Defaults to 50.
+            build_playlist (bool, optional): Flag to create the playlist in the user's library. Defaults to False.
+            exclude_mostly_instrumental (bool, optional): Flag to exclude the songs which are 80% or more instrumental. Defaults to False.
+
+        Raises:
+            ValueError: If the mood is not one of the valid options the error is raised
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the new playlist
+        """
+        if mood not in ['happy', 'sad', 'calm']: # energetic still needs work to be ready
+            raise ValueError("The mood parameter must be one of the following: 'happy', 'sad', 'calm'")
+
+        energy_threshold = 0.7
+        valence_threshold = 0.5
+        instrumentalness_threshold = 0.8
+
+        mood_queries = {
+            'sad': {
+                'ascending': True,
+                'sorting': 'energy&valence',
+                'query': 'valence < @valence_threshold and energy < @energy_threshold'
+            },
+            'calm': {
+                'ascending': True,
+                'sorting': 'energy&loudness',
+                'query': 'valence >= @valence_threshold and energy < @energy_threshold'
+            },
+            'angry': {
+                'ascending': False,
+                'sorting': 'energy&loudness',
+                'query': 'valence < @valence_threshold and energy >= @energy_threshold'
+            },
+            'happy': {
+                'ascending': False,
+                'sorting': 'energy&valence',
+                'query': 'valence >= @valence_threshold and energy >= @energy_threshold'
+            }
+        }
+
+        playlist = self.__playlist.query(mood_queries[mood]['query']).copy()
+
+        if mood_queries[mood]['sorting'] == 'energy&valence':
+            playlist['mood_index'] = playlist['energy'] + 3 * playlist['valence']
+        else:
+            playlist['mood_index'] = playlist['energy'] + 3 * playlist['loudness']
+        # this is necessary because of the moods that are not consistent in terms of the conditions applied to energy and valence, for example, happy and sad which have the same condition applied to both thresholds can use both in the sorting whereas the others can't.
+
+        if exclude_mostly_instrumental:
+            playlist = playlist.query('instrumentalness <= @instrumentalness_threshold')
+
+        playlist = playlist.sort_values(by='mood_index', ascending=mood_queries[mood]['ascending'])
+
+        if len(playlist) >= K:
+            playlist = playlist[:K]
+        else:
+            K = len(playlist)
+            logging.warning(f'The playlist does not contain {K} {mood} songs. Therefore there are only {len(playlist)} in the returned playlist. ')
+
+        if build_playlist:
+
+            for _ in range(2):
+                try:
+                    self.__mood = mood
+                    ids = playlist['id'].tolist()
+
+                    self.__write_playlist(
+                        K=K,
+                        type=f'mood',
+                        additional_info=ids
+                    )
+
+                except AccessTokenExpiredError as e:
+                    logging.warning('Error due to the access token expiration')
+                    auth_token = auth.get_auth()
+
+                    self.__auth_token = auth_token
+
+                    self.__headers['Authorization'] = f'Bearer {auth_token}'
+                else:
+                    break
+
+        return playlist
+
 
-def start_api(user_id: str, *, playlist_url: str = False, playlist_id: str = False, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
+def start_api(user_id: str, *, playlist_url: Union[str, None] = None, playlist_id: Union[str, None] = None, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
     """Function that prepares for and initializes the API
 
     Note:
         Internet Connection is required
 
     Args:
         user_id(str): the id of user, present in the user account profile
@@ -2071,19 +2272,17 @@
 
     logging.basicConfig(
         level=log_level.upper(),
         datefmt='%Y-%m-%d %H:%M:%S',
         format='%(asctime)s.%(msecs)03d - %(levelname)s: %(message)s',
     )
 
-    if not playlist_url and not playlist_id and not liked_songs:
-        raise ValueError(
-            'It is necessary to specify a playlist either with playlist id or playlist url or flag the liked_songs as True')
-    if (playlist_url or playlist_id) and liked_songs:
-        raise ValueError(
-            'It is necessary to specify only one of the following parameters: playlist_id or playlist_url or liked_songs')
+    if playlist_url is None and playlist_id is None and not liked_songs:
+        raise ValueError('It is necessary to specify a playlist either with playlist id or playlist url or flag the liked_songs as True')
+    if (playlist_url is not None or playlist_id is not None) and liked_songs:
+        raise ValueError('It is necessary to specify only one of the following parameters: playlist_id or playlist_url or liked_songs')
 
     logging.info('Retrieving Authentication token')
 
     auth_token = f'Bearer {auth.get_auth()}'
 
     return SpotifyAPI(auth_token=auth_token, playlist_id=playlist_id, user_id=user_id, playlist_url=playlist_url, liked_songs=liked_songs, prepare_favorites=prepare_favorites)
```

## spotify_recommender_api/request_handler.py

```diff
@@ -1,15 +1,16 @@
 import json
 import time
 import logging
-from requests import get, post, delete, put
+import requests
+from typing import Union
 from spotify_recommender_api.error import HTTPRequestError, TooManyRequestsError, AccessTokenExpiredError
 
 
-def exponential_backoff(func, retries: int = 5, *args, **kwargs):
+def exponential_backoff(func, retries: int = 5, *args, **kwargs) -> requests.Response:
     """Exponential backoff strategy (https://en.wikipedia.org/wiki/Exponential_backoff)
     in order to retry certain function after exponetially increasing delay, to overcome "429: Too Many Requests" error
 
     Args:
         func (function): function to be executed with exponential backoff
         retries (int, optional): Number of maximum retries before raising an exception. Defaults to 5.
 
@@ -17,17 +18,17 @@
         Exception: Error raised in the function after {retries} attempts
 
     Returns:
         Any: specified function return
     """
     x = 0
     while x <= retries:
-        response = None
+        response = requests.Response()
         try:
-            response = func(*args, **kwargs)
+            response: requests.Response = func(*args, **kwargs)
             try:
                 response.json()
             except Exception as e: # this error happens when there is a 204 response and the response.json() cannot be decoded properly regardless of the request being successful
                 pass
             else:
                 if response.status_code != 204 and 'error' in response.json():
                     raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs)
@@ -51,90 +52,92 @@
             if x >= retries:
                 raise TooManyRequestsError(func_name=func.__name__, message=f'After {retries} attempts, the execution of the function failed with the 429 exception', *args, **kwargs) from e
 
             sleep = 2 ** x
             logging.warning(f'\tError raised: sleeping {sleep} seconds')
             time.sleep(sleep)
 
+    return requests.Response()
 
-def get_request(url: str, headers: dict = None, retries: int = 10) -> dict:
+
+def get_request(url: str, headers: Union[dict, None] = None, retries: int = 10) -> requests.Response:
     """GET request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=get, url=url, headers=headers, retries=retries)
+    return exponential_backoff(func=requests.get, url=url, headers=headers, retries=retries)
 
-def post_request(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
+def post_request(url: str, headers: Union[dict, None] = None, data: Union[dict, None] = None, retries: int = 10) -> requests.Response:
     """POST request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=post, url=url, headers=headers, data=json.dumps(data), retries=retries)
+    return exponential_backoff(func=requests.post, url=url, headers=headers, data=json.dumps(data), retries=retries)
 
-def post_request_dict(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
+def post_request_dict(url: str, headers: Union[dict, None] = None, data: Union[dict, None] = None, retries: int = 10) -> requests.Response:
     """POST request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=post, url=url, headers=headers, data=data, retries=retries)
+    return exponential_backoff(func=requests.post, url=url, headers=headers, data=data, retries=retries)
 
-def post_request_with_auth(url: str, headers: dict = None, data: dict = None, auth: 'tuple[str]' = None, retries: int = 10) -> dict:
+def post_request_with_auth(url: str, headers: Union[dict, None] = None, data: Union[dict, None] = None, auth: Union['tuple[str]', None] = None, retries: int = 10) -> requests.Response:
     """POST request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=post, url=url, headers=headers, data=data, auth=auth, retries=retries)
+    return exponential_backoff(func=requests.post, url=url, headers=headers, data=data, auth=auth, retries=retries)
 
-def put_request(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
+def put_request(url: str, headers: Union[dict, None] = None, data: Union[dict, None] = None, retries: int = 10) -> requests.Response:
     """PUT request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=put, url=url, headers=headers, data=json.dumps(data), retries=retries)
+    return exponential_backoff(func=requests.put, url=url, headers=headers, data=json.dumps(data), retries=retries)
 
-def delete_request(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
+def delete_request(url: str, headers: Union[dict, None] = None, data: Union[dict, None] = None, retries: int = 10) -> requests.Response:
     """DELETE request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
-    return exponential_backoff(func=delete, url=url, headers=headers, data=json.dumps(data), retries=retries)
+    return exponential_backoff(func=requests.delete, url=url, headers=headers, data=json.dumps(data), retries=retries)
```

## spotify_recommender_api/server.py

```diff
@@ -2,16 +2,16 @@
 import time
 import uvicorn
 import threading
 import webbrowser
 import contextlib
 from fastapi import FastAPI, status
 from fastapi.responses import HTMLResponse
-from spotify_recommender_api.sensitive import *
-from spotify_recommender_api.request_handler import *
+from spotify_recommender_api.sensitive import CLIENT_ID, CLIENT_SECRET
+from spotify_recommender_api.request_handler import post_request_with_auth
 app = FastAPI()
 
 redirect_uri = 'http://localhost:8000/callback'
 scope = ["playlist-modify-private", "playlist-read-private", "user-library-read", "user-library-modify", "user-top-read"]
 
 class Server(uvicorn.Server):
     """Subclass of uvicorn.Server so that the run and shutdown methods can be done while running in a separate thread
@@ -59,15 +59,15 @@
         auth_code (str): Temporary code to have access to the access token
 
     Returns:
         str: Access token
     """
     response = post_request_with_auth(
         "https://accounts.spotify.com/api/token",
-        auth=(CLIENT_ID, CLIENT_SECRET),
+        auth=(CLIENT_ID, CLIENT_SECRET), # type: ignore
         data={
             "grant_type": "authorization_code",
             "code": auth_code,
             "redirect_uri": redirect_uri,
         },
     )
```

## spotify_recommender_api/util.py

```diff
@@ -1,14 +1,15 @@
 import logging
 import warnings
 import datetime
 import functools
 import pandas as pd
 import spotify_recommender_api.request_handler as requests
 from dateutil import tz
+from typing import Union, Any
 
 
 def playlist_url_to_id(url: str) -> str:
     """Extracts the playlist id from it's URL
 
     Args:
         url (str): The playlist public url
@@ -37,47 +38,47 @@
 
 
     playlist_res = requests.get_request(url=f'https://api.spotify.com/v1/playlists/{playlist_id}', headers=headers)
 
     return playlist_res.json()["tracks"]["total"]
 
 
-def song_data(song: dict, added_at: bool = True) -> 'tuple[str, str, float, list[str], datetime.datetime]':
+def song_data(song: 'dict[str, Any]', added_at: bool = True) -> 'list[Union[str, float, list[str], datetime.datetime]]':
     """Function that gets additional information about the song, like its name, artists, id, popularity, date when it was added to the playlist, etc.
 
     Args:
-        song (dict): The song dictionary fetched from the Spotify API
+        song (dict[str, dict[str, str]]): The song dictionary fetched from the Spotify API
 
     Returns:
-        tuple[str, str, float, list[str], datetime.datetime]: A tuple containing the song's information
+        list[str, str, float, list[str], datetime.datetime]: A list containing the song's information
     """
     try:
         data = [song["track"]['id'], song["track"]['name'], song["track"]['popularity'], [artist["name"] for artist in song["track"]["artists"]]]
     except KeyError:
         data = [song['id'], song['name'], song['popularity'], [artist["name"] for artist in song["artists"]]]
 
     if added_at:
         data.append(song['added_at'])
 
     return data
 
 
-def item_list_indexed(items: 'list[str]', all_items: 'list[str]') -> 'list[int]':
+def item_list_indexed(items: 'list[str]', all_items: 'list[str]') -> 'list[str]':
     """Function that returns the list of items, mapped to the overall list of items, in a binary format
     Useful for the overall execution of the algorithm which determines the distance between each song
 
     Args:
         items (list[str]): list of items for a given song
         all_items (list[str]): all the items inside the entire playlist
 
     Returns:
         list[int]: indexed list of items in binary format in comparison to all the items inside the playlist
     """
 
-    return [int(all_genres_x in items) for all_genres_x in all_items]
+    return [str(int(all_genres_x in items)) for all_genres_x in all_items]
 
 
 def playlist_exists(name: str, base_playlist_name: str, headers: dict, _update_created_playlists: bool = False) -> 'str|bool':
     """Function used to check if a playlist exists inside the user's library
     Used before the creation of a new playlist
 
     Args:
@@ -127,15 +128,15 @@
     song_id = song['id']
 
     audio_features = requests.get_request(
         url=f'https://api.spotify.com/v1/audio-features/{song_id}',
         headers=headers
     ).json()
 
-    return [audio_features['danceability'], audio_features['energy'], audio_features['instrumentalness'], audio_features['tempo'], audio_features['valence']]
+    return [audio_features['danceability'], audio_features['loudness'] / -60, audio_features['energy'], audio_features['instrumentalness'], audio_features['tempo'], audio_features['valence']]
 
 
 def get_datetime_by_time_range(time_range: str = 'all_time') -> datetime.datetime:
     """Calculates the datetime that corresponds to the given time range before the current date
 
     Args:
         time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
@@ -186,43 +187,48 @@
 
     Args:
         dictionary (dict): dictionary with only the values for each
 
     Returns:
         dict[str, dict[str, float]]: new dictionary with values and total percentages
     """
-    dictionary = {key: {'value': value, 'percentage': round(
-        value / dictionary['total'], 5)} for key, value in dictionary.items()}
-
-    return dictionary
+    return {
+        key: {
+            'value': value,
+            'percentage': round(value / dictionary['total'], 5)
+        }
+        for key, value in dictionary.items()
+    }
 
 
 def print_base_caracteristics(*args):
     """
     Function that receives a list of values and print them
 
     Args:
         name (str): name of the song
         artists (list[str]): song's artists
         genres (list[str]): song's genres
         popularity (int): song's popularity
         danceability (float): song's danceability
+        loudness (float): song's loudness
         energy (float): song's energy
         instrumentalness (float): song's instrumentalness
         tempo (float): song's tempo
         valence (float): song's valence
 
     """
-    name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence = args
+    name, genres, artists, popularity, danceability, loudness, energy, instrumentalness, tempo, valence = args
 
     logging.info(f'{name = }')
     logging.info(f'{artists = }')
     logging.info(f'{genres = }')
     logging.info(f'{popularity = }')
     logging.info(f'{danceability = }')
+    logging.info(f'{loudness = }')
     logging.info(f'{energy = }')
     logging.info(f'{instrumentalness = }')
     logging.info(f'{tempo = }')
     logging.info(f'{valence = }')
 
 
 def get_base_playlist_name(playlist_id: str, headers: dict) -> str:
```

## Comparing `spotify_recommender_api-4.2.0.dist-info/METADATA` & `spotify_recommender_api-4.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.2.0
+Version: 4.3.0
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -35,37 +35,37 @@
 - [Packages used](#packages-used)
 - [OG Scripts](#og-scripts)
 - [Contribution Rules](#contributing)
 
 
 ## Use Case
  - This is the first section of this readme, because, you will see, this package can help, but nothing is perfect, so it will, as long as you fit in this particular use case ;(
- - The perfect use case for this is that one playlist (or more) that you put a bunch of songs in different times and mood styles, and when you listen to it, you feel like only listening to a part of it, some days later, that part is useless, but some other part is awesome. The big issue here is that those "parts" are shuffled, all across the playlist. Then how would one find those songs they crave, today, tomorrow, and later? Speaking from experience, it is not worth it to map manually a 1000 song playlist and filter out 50, or 100 of them.
+ - The perfect use case for this is that in one playlist (or more) you put a bunch of songs in different times and mood styles, and when you listen to it, you feel like only listening to a part of it, some days later, that part is useless, but some other part is awesome. The big issue here is that those "parts" are shuffled, all across the playlist. Then how would one find those songs they crave, today, tomorrow, and later? Speaking from experience, it is not worth it to map manually a 1000-song playlist and filter out 50, or 100 of them.
  - This package comes to solve this issue, roughly, because it tries to find the K (number) nearest songs taking into consideration genres, artists, popularity, and some audio features, such as danceability, energy, instrumentalness, tempo, and valence, using the KNN supervised machine learning technique to find the closest songs to some threshold.
  - One issue with this is that Spotify API is not the best, E.g. A LOT of artists do not have any genre associated with them, which, as justified in the next topic, is the main source of genre information used
- - Another issue is that Spotify API does not provide, at the time of publication of version 3.5.2, neither song nor album genres, which compromises a portion of the accuracy of the recommendations.  Still, I recommend you give it a try
+ - Another issue is that Spotify API does not provide, at the time of publication of version 3.5.2, either song or album genres, which compromises a portion of the accuracy of the recommendations.  Still, I recommend you give it a try
 
 
 
 
 ## Setup
 
 ### Requirements:
   - Python installed<br>
  The ideal version, to run the package is 3.8.x, the version on top of which the package was built, older versions may have some issues, as the package uses a handful of other packages and their versions may conflict.
   - Network Connection<br>
  So that a wide range of songs can be analyzed, it is imperative to have a network connection, at least for the first time executing a script using this package.
   - <strong>A fitting playlist</strong><br>
- The perfect use case for this package is that of one big playlist (200+ songs), which you feel like listening to some of them, then others but never, or rarely, all of them, since they belong to different genres/styles.
+ The perfect use case for this package is that of one big playlist (200+ songs), which you feel like listening to some of them, then others, but never, or rarely, all of them, since they belong to different genres/styles.
   - ## <strong>Patience</strong>
     It may seem funny or a joke, but the first mapping process of the playlist to a local pandas DataFrame... it will take a good while, up to 2.5 to 3 seconds per song, at 20-40Mbps Internet connection, being in Latam. All these factors play a part in the time for it to the first load.
     Just to make it clear, CPU, ram, sdd, etc., will not help much, the issue is to have up to 7 different HTTP requests per song, which make this take so long.
     Besides, as of July/2022, Spotify implemented a possible API Response: ["429: Too Many Requests"](https://http.cat/429) which forced this package to implement [Exponential Backoff](https://en.wikipedia.org/wiki/Exponential_backoff) to complete its requests, therefore what already took a while, now takes a little bit more
   - Jupyter Notebook<br>
- Not exactly a requirement but it is advised that a jupyter notebook is used (even more recommended to use the vscode extension for jupyter notebooks) because it is important, or at least more comfortable, to have the variable still in memory and then decide how to use it, without having to run a script multiple times, having to reconnect to Spotify, redownload the playlist, redo some computations, etc.
+ Not exactly a requirement but it is advised that a Jupyter notebook is used (even more recommended to use the vscode extension for Jupyter notebooks) because it is important, or at least more comfortable, to have the variable still in memory and then decide how to use it, without having to run a script multiple times, having to reconnect to Spotify, redownload the playlist, redo some computations, etc.
   - Spotify access<br>
  I mean, you knew that already, right?
 
   - ### Installing the package<br>
 ~~~ps1
 pip install spotify-recommender-api
 ~~~
@@ -77,16 +77,16 @@
  ~~~ python
  from spotify_recommender_api.recommender import start_api
  ~~~
 
 ### Starting the api
   - Gathering the initial information: (playlist_url, user_id)<br>
 
-  --- Playlist URL: The playlist url is available when right clicking the playlist name / or going to the three dots that represent the playlist options <br>
-  --- Playlist ID: The playlist id is available the hash string between the last '/' in and the '?' in the playlist url<br>
+  --- Playlist URL: The playlist URL is available when right-clicking the playlist name / or going to the three dots that represent the playlist options <br>
+  --- Playlist ID: The playlist id is available as the hash string between the last '/' in and the '?' in the playlist url<br>
   <img src='./readme-pictures/Playlist Configs.png' width='25%'><br>
   --- User ID: The user id is available when clicking the account, and accessing its information, on Spotify's website<br>
   <img src='./readme-pictures/Account.png' width='25%'><br>
   --- Liked Songs: A flag to pass in case the playlist you want to use is your profile Liked Songs <br>
   --- Log level: the logging package log level. Defaults to INFO, but can be DEBUG, INFO, WARNING and ERROR
 
   - Calling the function:
@@ -100,58 +100,58 @@
 Or
 ~~~python
 api = start_api(liked_songs=True, user_id='<USER_ID>', log_level='DEBUG')
 ~~~
 Though, to be honest, it is easier and more convenient to use the playlist URL or the liked_songs flag
 
   - Getting the Auth Token:
-  It is a hash token that expires 60 minutes after it is generated, and after April 22nd 2023 it has been fully refactored, due to a change in the Spotify API Authentication methods, which invalidated the previous way. Now As soon as you call the start_api function a fastapi server will be lauched in port 8000.<br>
-  The also there will be a web browser opened so that the user can click on the button Authorize, the log in with their spotify account, and then, the authentication is completed for that usage of the package.
+  It is a hash token that expires 60 minutes after it is generated, and after April 22nd, 2023 it has been fully refactored, due to a change in the Spotify API Authentication methods, which invalidated the previous way. Now As soon as you call the start_api to function a fast API server will be launched in port 8000.<br>
+  Also there will be a web browser opened so that the user can click on the button Authorize, log in with their Spotify account, and then, the authentication is completed for that usage of the package.
 
 
 ## Methods
  - get_playlist
 ~~~python
 # Method Use Example
 api.get_playlist()
 # Function that returns the pandas DataFrame representing the base playlist
 ~~~
  - playlist_to_csv
 ~~~python
 # Method Use Example
 api.playlist_to_csv()
-# Function that creates a csv format file containing the items in the playlist
-# Especially useful when re running the script without having changed the playlist
+# Function that creates a CSV format file containing the items in the playlist
+# Especially useful when re-running the script without having changed the playlist
 ~~~
  - get_recommendations_for_song
 ~~~python
 # Parameters
 get_recommendations_for_song(song: str, K: int, with_distance: bool, generate_csv: bool,
                         generate_parquet: bool, build_playlist: bool, print_base_caracteristics: bool)
 # Method Use Example
 api.get_recommendations_for_song(song='<SONG_NAME>', K=50)
 # Function that returns the pandas DataFrame representing the
 # given song recommendation playlist
-# the 'song' and 'K' parameters are mandatory and the rest is
+# The 'song' and 'K' parameters are mandatory and the rest is
 # defaulted to False
 # The "distance" is a mathematical value with no explicit units, that is
-# used by te algorithm to find the closest songs
+# used by the algorithm to find the closest songs
 # print_base_caracteristics will display the parameter song information
 # Note that it can be used to update a playlist if the given song already
-# has its playlist generated by this package
+# Has its playlist generated by this package
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - get_most_listened
 ~~~python
 # Parameters
 get_most_listened(time_range: str = 'long', K: int = 50, build_playlist: bool = False)
 # Method Use Example
 api.get_most_listened(time_range='short', K=53)
 # Function that returns the pandas DataFrame representing the
-# given time range most listened tracks playlist
+# given the time range most listened to tracks playlist
 # No parameters are mandatory but the default values should be noted
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - update_all_generated_playlists
 ### WILL CHANGE THE USER'S LIBRARY DRASTICALLY
 ~~~python
 # Parameters
@@ -170,43 +170,43 @@
 get_playlist_trending_genres(time_range: str = 'all_time', plot_top: int|bool = False)
 # Method Use Example
 api.get_playlist_trending_genres()
 # Function that returns a pandas DataFrame with all genres within the playlist and both their
 # overall appearance and the percentage of their appearance over the entire playlist
 # in the given time_range
 # Setting the plot_top parameter to one of the following [5, 10, 15] will plot a barplot
-# with this number of the most listened genres in the playlist
+# With this number of the most listened genres in the playlist
 ~~~
  - get_playlist_trending_artists
 ~~~python
 # Parameters
 get_playlist_trending_artists(time_range: str = 'all_time', plot_top: int|bool = False)
 # Method Use Example
 api.get_playlist_trending_artists()
 # Function that returns a pandas DataFrame with all artists within the playlist and both their
 # overall appearance and the percentage of their appearance over the entire playlist
 # in the given time_range
 # Setting the plot_top parameter to one of the following [5, 10, 15] will plot a barplot
-# with this number of the most listened artists in the playlist
+# With this number of the most listened artists in the playlist
 ~~~
  - artist_specific_playlist
 ~~~python
 # Parameters
 artist_specific_playlist(artist_name: str, K: int = 50, complete_with_similar: bool = False, build_playlist: bool = False, ensure_all_artist_songs: bool = True, print_base_caracteristics: bool = False, with_distance: bool = False)
 # Method Use Example
 api.artist_specific_playlist(artist_name='Joyner Lucas', K=50, complete_with_similar=True, print_base_caracteristics=True, build_playlist=True)
 # Function that returns a pandas DataFrame with all songs from a specific artist within the playlist
-# and can complete that new playlist with the closest songs to that artist, and create it in the users account
+# and can complete that new playlist with the closest songs to that artist, and create it in the user account
 # complete_with_similar is a Flag that indicates if the playlist will be completed with the closet songs related to the artist or only their songs
 # The ensure_all_artist_songs Flag serves the purpose of making sure all the artist's songs are present in a "This is" type playlist, regardless of the K value.
-# This behaviour is turned off by setting the Flag as False
+# This behavior is turned off by setting the Flag as False
 # print_base_caracteristics will display the parameter song information
 # The "distance" is a mathematical value with no explicit units, that is
-# used by te algorithm to find the closest songs
-# If complete_with_similar is True and K is more than all the songs with that artist, a Artist Mix is created,
+# used by the algorithm to find the closest songs
+# If complete_with_similar is True and K is more than all the songs with that artist, an Artist Mix is created,
 # otherwise, a "This once was" Playlist is created
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - audio_features_extraordinary_songs
 ~~~python
 # Parameters
 audio_features_extraordinary_songs()
@@ -218,52 +218,61 @@
  - get_profile_recommendation
 ~~~python
 # Parameters
 get_profile_recommendation(K: int = 50, main_criteria: str = 'mixed', save_with_date: bool = False,
 build_playlist: bool = False)
 # Method Use Example
 api.get_profile_recommendation(build_playlist=True)
-# Function that returns a pandas DataFrame with profile based recommendations, and create it in the users account
+# Function that returns a pandas DataFrame with profile-based recommendations, and creates it in the user account
 # main_criteria is the base info to get the recommendations
-# save_with_date is a flag to save the recommendations as a playlist as a point in time Snapshot
+# save_with_date is a flag to save the recommendations as a playlist at a point in time Snapshot
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - get_playlist_recommendation
 ~~~python
 # Parameters
 get_playlist_recommendation(K: int = 50, time_range: str = 'all_time', main_criteria: str = 'mixed', save_with_date: bool = False,
 build_playlist: bool = False)
 # Method Use Example
 api.get_playlist_recommendation(build_playlist=True)
-# Function that returns a pandas DataFrame with playlist based recommendations, and create it in the users account
+# Function that returns a pandas DataFrame with playlist-based recommendations, and creates it in the user account
 # main_criteria is the base info to get the recommendations
 # time_range is the time range to be looked at for the recommendations baseline
 # save_with_date is a flag to save the recommendations as a playlist as a point in time Snapshot
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - get_general_recommendation
 ~~~python
 # Parameters
 get_general_recommendation(K: int = 50, genres_info: 'list[str]' = [], artists_info: 'list[str]' = [], build_playlist: bool = False, use_main_playlist_audio_features: bool = False, tracks_info: Union['list[str]', 'list[tuple[str]]', 'list[list[str]]', 'dict[str, str]'] = [])
 # Method Use Example
 api.get_general_recommendation(build_playlist=True, artists_info=['NF', 'Logic'], use_main_playlist_audio_features=True)
-# Function that returns a pandas DataFrame with artists, genres, and/or tracks based recommendations, and create it in the users account
-# genres_info, artists_info and tracks_info are the lists of information that the recommendation would be based on
-# use_main_playlist_audio_features is the flag to indicate if the playlist provided audio features will be used as target for a better recommendation
+# Function that returns a pandas DataFrame with artists, genres, and/or tracks-based recommendations, and creates it in the user account
+# genres_info, artists_info, and tracks_info are the lists of information that the recommendation would be based on
+# use_main_playlist_audio_features is the flag to indicate if the playlist-provided audio features will be used as the target for a better recommendation
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~~~~
  - select_playlist
 ~~~python
 # Parameters
 select_playlist(user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False)
 # Method Use Example
 api.select_playlist(user_id='USER_ID', liked_songs=True)
-# Function to select a playlist to be mapped and be available on all the playlist related recommendation
+# Function to select a playlist to be mapped and be available on all the playlist-related recommendation
 # functions on an already existing authorization context
 ~~~~~~
+ - select_playlist
+~~~python
+# Parameters
+get_songs_by_mood(mood: str, K: int = 50, build_playlist: bool = False, exclude_mostly_instrumental: bool = False)
+# Method Use Example
+api.get_songs_by_mood(mood='happy', build_playlist=True)
+# Function to create a playlist based on the general mood of its songs
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~~~~
  - get_medium_term_favorites_playlist - DEPRECATED
 ~~~python
 # Parameters
 get_medium_term_favorites_playlist(with_distance: bool, generate_csv: bool,
                         generate_parquet: bool, build_playlist: bool)
 # Method Use Example
 api.get_medium_term_favorites_playlist(generate_csv=True, build_playlist=True)
```

## Comparing `spotify_recommender_api-4.2.0.dist-info/RECORD` & `spotify_recommender_api-4.3.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-spotify_recommender_api/__init__.py,sha256=gTh6GZub1Gxz539cnDJUpjnkqBuxLByN9jyLxdgyuVM,21
+spotify_recommender_api/__init__.py,sha256=y8JoTeT_XJHBkLPDHkagOZ5tayUYIaWASs4owPHVmPo,21
 spotify_recommender_api/authentication.py,sha256=qe48egeqnyZMD00mz2DULGaPFK-XECQOXc_zbeNsbHE,636
-spotify_recommender_api/core.py,sha256=JoZR9LFQbiy5ZrZGoB2G4kFMNMa0fVdR-hkNivTPMXk,14264
-spotify_recommender_api/error.py,sha256=DRzFWUZLI0QQ5HaKhOtEEXkDtC1-1wdfTxnmMPcjThg,1966
-spotify_recommender_api/recommender.py,sha256=MvMBSqdfgjzfz88dKXCVcG51Y_mxrgVOcrqzw7SwIzI,98800
-spotify_recommender_api/request_handler.py,sha256=nq5ITOayozz-gZwpokGwIhSp8ovIzuOuzNln2oJA9zk,5933
+spotify_recommender_api/core.py,sha256=VbanTkyXDUOIghRE3Su2Fx39ySwpto4ebR4ewYobhgQ,14957
+spotify_recommender_api/error.py,sha256=BBG5MUYuoAGElBAV058H6o13R-bYR_sGGgjAT1r7lCg,2042
+spotify_recommender_api/recommender.py,sha256=0dTegGIfuK373pQ6_EfR9QHX4FhfrpHAe5LWdlCKt8o,108957
+spotify_recommender_api/request_handler.py,sha256=iBKnJCky25FqTpOmcK89JSp4DFltElI0sTHZudMBWik,6305
 spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
-spotify_recommender_api/server.py,sha256=kG-4CoPvzpZHQzeOnKRa7vCGa5C_4NT7-b8j4jsBwHI,6661
-spotify_recommender_api/util.py,sha256=pxBFcRnwAbkDUKyzcA8YXX4zI4jVosjRHC0_EvFdHr0,9304
-spotify_recommender_api-4.2.0.dist-info/METADATA,sha256=cFaWD9uIdvOte7SATIy-8scrCLTIUs1id4Z3wEXYRJE,21022
-spotify_recommender_api-4.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-4.2.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-4.2.0.dist-info/RECORD,,
+spotify_recommender_api/server.py,sha256=GpQ1gQ-q00RN-mqPj969TCn831VgGFVirqjCzx8NJVs,6720
+spotify_recommender_api/util.py,sha256=fGw8QMrCoy_7FW8xD_2BdJ0bUHE4mj8rm0gqa1dxNwU,9510
+spotify_recommender_api-4.3.0.dist-info/METADATA,sha256=J7-FaHnEJImgT9Bip9qeKAMVL1sU-f1nmcoPUrTEpDo,21409
+spotify_recommender_api-4.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-4.3.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-4.3.0.dist-info/RECORD,,
```

