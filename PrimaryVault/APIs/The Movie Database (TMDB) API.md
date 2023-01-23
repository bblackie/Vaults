
# Functions

[Movie Discover](https://developers.themoviedb.org/3/discover/movie-discover)
[TV Discover](https://developers.themoviedb.org/3/discover/tv-discover)


# How to

Search for Movies with a date range

Use **discover**
eg.
https://api.themoviedb.org/3/discover/movie?api_key=<<api_key>>&language=en-US&sort_by=popularity.desc&page=1&primary_release_date.lte=1920-03-11&with_genres=27
e.g. 2 (official)
[Examples](https://www.themoviedb.org/documentation/api/discover)


# Processes

NB: 
- Movie/TV discover is best for finding selections of movies based on year, genre, popularity

Scenario #1:
- I have a movie name and want to see what matches come back before deciding to pull back some other fields
- Use the keyword search
- 
