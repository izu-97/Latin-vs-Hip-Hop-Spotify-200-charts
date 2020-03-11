# Latin vs Hip Hop on Spotify 200 charts

Mateo Izureita

06-03-20

## Project description

This projects main goal is to analyse the top 200 charts on spotify over a period of 3 years. Triying to see a development olver time of different genres and songs, the characteristics of songs that are popular arounf the world categorize by genre. It also tries to answer the questions of how many people listen to music on spotify around the world, how the market is devided by aritst and which has been some of the key events over the last years that have push certain genres to the top. The data was provided by spotify official API and unofficial API (Spotipy). With help of this tool, i was able to get different songs characteristics such as valence, tempo, danceablility, etc the rank of hte sonf per week, the country were it was listened to, listeners per week and genre. The data was display with tableau, and can be found in this [presentation](https://public.tableau.com/profile/izurieta.mateo#!/vizhome/LatinvsHipHopSpotify200charts/finalpresentation), were the user will find a varaity of graphics to analyse and have a deepper understanding of how music has develope over time. This project also compares the latin and hip hop genres and tries to explain the phenomenon of why latin music has grown so much in the last years, which were the foundations that let this genre evolve and grown so much.

## Questions

- How are the countries that lsiten the most music on spotify?
- How is the distribution per country?
- Which are the top 5 genres on spotify over the last 3 years?
- How many streams do they got?
- How latin and hip hop genres have developed over time?
- How are the most important artist?
- Whichs events influced on the rise of this genres?
- Which are the characteristics of iconic songs that top the charts?

## Dataset

The dataset used for this analysis was build by myself using the help of [fycharts](https://github.com/kelvingakuo/fycharts?fbclid=IwAR3BPolR97WzwzMjjAsRAmVoU82K6nA_y3PJwsIOxj06ociWkPDmiMOPeHM) a python library for gathering date pf the top 200 spotify charts by contry over time. And the spotify [API](https://developer.spotify.com/documentation/web-api/) to gather the characteristics of the song and the genre. 


In the dataset we can find the following columns:

Artist: Name of the artist
Position: Position during the week
Streams: Number of streams during the week
Track Name: Name of the track
Acousticness: The higher the value the more acoustic the song is
Analysis_url: The link or gathering the info
Danceability: The higher the value, the easier it is to dance to this song
Date: The first day of the week
Duration_ms: Duration of the song in ms
Energy: The energy of a song, the higher the value the more energetic the song
Id_caller: Spotify id of the song
Instrumentalness: How instrumental is the song 
Liveness: The higher the value, the more likely the song is a live recording
Loudness: The higher the value, the louder the song
Region: Where the song was stream
Speechiness: The higher the value the more spoken word the song contains
Valence: The higher the value, the more positive mood for the song
Genre: The genre of the song 

## Workflow

I have always been very pasionate about music so i decided to do my final project about that. I was lookig for a date bas to used and i stumble upon the spotipy library for python which help me gathered the data of the songs it was realy complecated to make it work properlly but after sometime i manage to make it work properlly and was able to download all the csv files for each countrie where spotify is available. 

After i already got the data of the songs and its corresponding ids i started using the spotify API. I had to register as a developer and the reasons for using the API. After going to that process i got the rights to used it but connecting to it took a long time. After i figure out how to connect with the API i manage to get the characteristics of the songs and the genre. 

After getting each individual countrie csv i merge them together to create the dataset i would work with, then i join the characteristics trough the id and also the genre. 

Afterwards i did a quick analysis with python to see if there is any missing values, i clean the data, fill the missing values,slice the date to have just the first day of te week and after that i was done and ready to dive deep on the data.
















