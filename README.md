# Spotifraud
This utilizes the Spotify API to find various monetary and music statistics.

The initial goal of this project was to create a python application using Spotify's API to pull the number of streams on an artists song, and find out
how much the artist made versus spotify. The user would be able to search for a song, and get this result.

Initially I was successful in setting up a class to utilize various endpoints in spotify's API.
I created various functions to allow the user to request artists data, song links, album cover images, and more. However, I was struggling to find an efficient way to get the exact stream count for a song, but I continued on.

Next, I made a system for the user to enter a string of a song name and have it return all the information it could on that song from a request to Spotify's API, but there was a problem.
The huge string returned contained a lot of interesting and useful information, but not the number
of streams on the song. Frustrated, I did what I told myself I would not do at the start of this
project - I googled " Python project to get Spotify Streams". What I found was dissapointing.

Spotify does not allow for API access to their stream count data, as they believe such access 
could be used nefariously to artificially inflate streams. The only way people were to achieve
what I wanted was to user a Web Scraper, which is pretty far outside of the scope of what I was 
planning on building.

To alter course, I did make a function to calculate how much money the artist made off of a song
by allowing the user to manually enter the integer amount. This is less than ideal, but to 
try and salvage this I hope to make this a more abstract implmentation of spotifys API in python.
