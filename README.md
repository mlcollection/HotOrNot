# Hot or Not?
### Creating a Hit Song Predictor  

Hit songs translate to real dollars. Songs that have been vetted as hits can generate revenue long past their tenure on the musical charts by providing credibility and visibility to a song, an artist and their entire brand. This study aims to understand the profile of a hit record and create a classifier to determine if a song is likely to be "Hot" or "Not".

#### Retrieval of Billboard Hot 100 Data  
The Billboard Hot 100 is a weekly chart that showcases the top 100 tracks in the USA based on sales (physical and digital), streaming and radio airplay. It debuted on August 4th, 1958 and considered the industry standard for hit songs. The data was acquired using billboard.py, a Python API for accessing music charts from Billboard.com.

The variables of interest are:  
**Date** - Date of the chart  
**Title** – Title of the track  
**Artist** – Name of the artist, as formatted on Billboard.com  
**Rank** – Track's current position on the chart  
**Peak** – Track's peak position on the chart as of the chart date  
**Weeks** – The number of weeks the track has been or was on the chart, including future dates (up until the present time)

#### Retrieval of Spotify Data   
Spotify has made a huge mark in the digital streaming space since going live in 2008. With over songs, 113,000,00 subscribers in over countries. It is no wonder that the popularity of songs on this platform are highly related to ability to chart.
Spotify URIs were obtained using the spotipy 2.9.0. These unique identifiers were then used to retrieve features about the tracks.  

These include:  
acousticness  
danceability  
duration_ms  
dynamic_range  
energy  
explicit  
instrumentalness  
key  
loudness  
mode  
popularity  
release_date  
sections  
speechiness  
tempo  
time_signature  
valence  

#### Hot or Not Classifier 
The classifer is created using Logistic Regression, Support Vector Machine and Random Forest and the metrics are compared.
