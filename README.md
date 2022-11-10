# Spotify-ETL-Pipeline
Extracting data from Spotify and Genius APIs to analyze popularity amongst hip-hop artists.

### Overview
In this project, I sought to better understand popularity among the hip-hop artists. To do this, I accessed the APIs of Spotify and Genius. Genius gave me pageviews - which are a rough metric for popularity of a song - and Spotify gave me the song and artist data.
One of the greatest challenges in this project was reconciling differences between the artist and song names between the APIs. To solve this, I learned about
and implemented a fuzzy matching algorithm that used multiple metrics/functions and aggregated them to give a score. Based on this score, a limit was placed
on whether or not to accept the name version. It's a relevant problem that I've run into a couple of times, so it was nice to find a solution.
I took this data and exported it into a local SQL database using psycopg2 in Python, and then successfully connected this SQL database to Tableau.
My experience lies in Power BI, which is costly, therefore I haven't built out a visual in Tableau as of yet. 

Tools and Technologies used:
Python, Spotify and Genius APIs, SQL, psycopg2, fuzzy matching
