# Latin vs Hip Hop on Spotify 200 charts

Mateo Izurieta

06-03-20

## Project description

This projects main goal is to analyse the top 200 charts on spotify over a period of 3 years. Triying to see a development over time of different genres and songs, the characteristics of songs that are popular around the world categorize by genre. It also tries to answer the questions of how many people listen to music on spotify around the world, how the market is devided by aritst and which has been some of the key events over the last years that have push certain genres to the top. The data was provided by spotify official API and unofficial API (Spotipy). With help of this tool, i was able to get different songs characteristics such as valence, tempo, danceablility, etc the rank of hte sonf per week, the country were it was listened to, listeners per week and genre. The data was display with tableau, and can be found in this [presentation](https://public.tableau.com/profile/izurieta.mateo#!/vizhome/LatinvsHipHopSpotify200charts/finalpresentation), were the user will find a varaity of graphics to analyse and have a deepper understanding of how music has develope over time. This project also compares the latin and hip hop genres and tries to explain the phenomenon of why latin music has grown so much in the last years, which were the foundations that let this genre evolve and grown so much.

## Questions

- Who are the countries that listen the most music on spotify?
- How is the distribution per country?
- Which are the top 5 genres on spotify over the last 3 years?
- How latin and hip hop genres have developed over time?
- How are the most important artist?
- Whichs events influced on the rise of this genres?
- Which are the characteristics of iconic songs that top the charts?

## Dataset

The dataset used for this analysis was build by myself using the help of [fycharts](https://github.com/kelvingakuo/fycharts?fbclid=IwAR3BPolR97WzwzMjjAsRAmVoU82K6nA_y3PJwsIOxj06ociWkPDmiMOPeHM) a python library for gathering date of the top 200 spotify charts by contry over time. And the spotify [API](https://developer.spotify.com/documentation/web-api/) to gather the characteristics of the song and the genre. 


In the dataset we can find the following columns:

- Artist: Name of the artist
- Position: Position during the week
- Streams: Number of streams during the week
- Track Name: Name of the track
- Acousticness: The higher the value the more acoustic the song is
- Analysis_url: The link or gathering the info
- Danceability: The higher the value, the easier it is to dance to this song
- Date: The first day of the week
- Duration_ms: Duration of the song in ms
- Energy: The energy of a song, the higher the value the more energetic the song
- Id_caller: Spotify id of the song
- Instrumentalness: How instrumental is the song 
- Liveness: The higher the value, the more likely the song is a live recording
- Loudness: The higher the value, the louder the song
- Region: Where the song was stream
- Speechiness: The higher the value the more spoken word the song contains
- Valence: The higher the value, the more positive mood for the song
- Genre: The genre of the song 

## Workflow

I have always been very passionate about music so i decided to do my final project about that. I was lookig for a data base to used and i stumble upon the spotipy library for python which help me gathered the data of the songs it was realy complicated to make it work properlly but after sometime i manage to make it work and was able to download all the csv files for each countrie where spotify is available. 

After i already got the data of the songs and its corresponding ids i started using the spotify API. I had to register as a developer and the reasons for using the API. After going to that process i got the rights to used it but connecting to it took a long time. After i figure out how to connect with the API i manage to get the characteristics of the songs and the genre. 

After getting each individual countrie csv i merge them together to create the dataset i would work with, then i join the characteristics trough the id and also the genre. 

Afterwards i did a quick analysis with python to see if there is any missing values, i cleaned the data, fill the missing values,slice the date to have just the first day of te week and after that i was done and ready to dive deep on the data.


**Who are the countries that listen the most music on spotify?**

As we can clearly see on the graph, the countries with the most streams are the US, Mexico, Brazil, Germany, and the UK. This can be atributted to their population since this countries have a really big population. in total arounf the world the total sum of streams is around 361 billion which means the number of streams has double over the past 3 years.

**How is the distribution per country?**

As we can expect, the number of streams per countrie is correlated with the population, we can clearly see that countries with smaller populations dont stream as uch music as countries with really populations.

**Which are the top 5 genres on spotify over the last 3 years?**

If we break down the sum of streams into differetn genres we an clearly see the top 5 genres in spotify. These being dance pop, hip hop, latin, pop, atl hip hop. Dance pop has around 59 billions, hip hop has around 34 billions and latin has 33 billions. if we sum the top three genres they take around 35% of the total streams. In this graph we can clearly see that latin music has rise over the last 3 years while dance pop has been more or less regular and hip hop having this crazy peaks whichs we will analize later.

**How latin and hip hop genres have developed over time?** 

If we look deeper into both this genres we can analyses teh causes of them being so popular and which are the factors that influence on then to became one of the most important genres at te moment.

If we take a look at the latin genre we can clearly see that on the early 2017 it went up fast and this can be atribbuted to the super hit despacito which top the charts all arount the world giving this genre the boost it needed to climb to the top. Another interesting peak can be clearly see at mid 2019 with the realease of oasis, a collaborative projet between J Balvin and Bad Bunny which was really popular in south america.

Breaking down the genre into artist we can see that there is quite a variety of artist holding this gerne on top some of them are: Luis Fonsi, Ozuna, Bad Bunny, etc. 




Looking deeper into hip hop we can see that if we dont count the peaks hip hop has being really consistent over time. But since we have a lot of peaks we have to take a deeper look into them. The firts signifcant peaks was on early 2017 with drake realisig more than life. This disc quickly became an anthem to a generation. It was stream all around te world but mostly in the US. The next one is Post Malones debut album Beerbongs and Bentleys. But the most significant peak in this genre is when th super star drake drop one of th most waited albums of all times, Scorpion. The songs in this album top the charts everywhere with around 800 millions streams in just one week.

Taking a look into each hip hop artist we can clearly s that there are only 4 big artist that have most of the streams. This Artista are Drake, Post Malone, Kendrik Lamar.

Looking into the distribution of each genre we can see that latin is much more evenly distibuted that hip hop with hip hop having just a few superstarts that let it hold its top position.

**Which are the characteristics of iconic songs that top the charts?**

Each hit song has differetn characteristics but of we group them by genre we can see that there are some key characteritics that most ht songs in each genre has.

For this presentation we just focus on energy and danceability as key metrics.

Energy is a perceptua measure of intensity and acticity, songs that feel fast, loud and noisy are categorize with a higher value.

Danceability is describe as how suitable a track for dancing.

If we look inro the bin diagram we will see taht latn music tends to be more close to the right side meaning thats is really energetic and danceable, while hip hop stays kind of center.



















