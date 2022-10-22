# Spotifraud
This utilizes the Spotify API to find various monetary and music statistics.

Version 0.1.1

BACKEND:

user.py
  - This is responsible for authorizing the user, by following the
    OAuth2 flow to fetch necessary tokens from Spotify. The refresh process
    is initiated as needed when the token expires. The token is used to
    interact with the Spotify API via spotipy client.
    
client_services.py:
  - This utilizes the Spotipy library for python3 to get many of the endpoints, and desired returns, from spotifys header library. The header library
    offers many srervices for interacting with the spotify app, such as generating playlists, getting artists and songs, and other statistics. This
    class is the main bulk of the backend.
    
endpoints.py:
  - Sends and gets requests to spotify using the headers in the client_services class.
