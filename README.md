# Analysis of Spotify: Listening Patterns In the US and Across the World

## 1) Introduction and Motivation
All around the world people are connected by music. It gives everyone a way to express themselves and brings people together. In today's society people listen to music in many different circumstances in which their music preferences may change. As a studnt between walking to class, working out at the gym, or studying in the library, you are bound to see a large number of individuals with headphones on listening to a variety of different music. Music has the ability to highten experiences, set the tone, and change the mood. Using Spotify's API to access world listening tredns, our project aimed to discover what makes music popular and if there are any differences in popular music between the United States and Globally.

## 2) Methods
Since we all regularly use spotify to listen to music, we obtained the spotify API (called Spotipy) to gain access to a wide range of data. We were able to access complex data from the Global top 50 songs and the US top 50 songs on spotify. We completed two seperate analyses on these two playlists and then compared trends found in each one.

Within the avaliable data for both playlists we found audio features of the songs, allowing us to determine characteristics that made these songs popular. This was the approach we took to determine the “qualities” of music that people find the most entertaining thus making these songs popular. We also looked at the correlation between all of the audio features to determine the likelihood of a feature being present based off of the presence of another feature.

We compared listening trends between the global top 50 and the US top 50 by looking at artist frequency in the top 50, genre frequency, and track popularity based on genre. We also were able to visulaize the songs and artists that appeared in both playlists to see how similar the top 50 globally is to the top 50 in the US.

## 3) API Acquisition
We were able to use the spotipy python module that is provided by spotify. This allowed us to access the spotipy API which is well documented and allowed us to access information about songs and certain information about personal user profiles. We had to request persmission from spotify to create a project using the spotify developers page. We were then given a client ID number as well as client secret number through the spotify app that allowed us to have access to the data.

## 4) Visualization and Analysis for Global Top 50 Playlist
In order to reach our goals for the project, we began by getting data from the Top 50 Global Songs playlist created by Spotify. The live playlist updates every week with the new top songs across the world. Using the spotipy documentation, we determined the varibles that were of our interest and put them into a data frame. The varibles that we decided to use were track name, track popularity, artist, artist popularity, genre, album name, and song uri. The song uri's were not used for any analysis, but were used for accessing song information.

#### gets the top 50 tracks globally with the artist, track popularity, artist popularity, genre, 
#### album name, and uri
<img width="1152" alt="Screenshot 2024-04-07 at 8 56 45 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/3d2886ff-2000-4edb-bbb3-1a0f85d2e474">

#### gets audio features for the top 50 songs using spotipy package audio features 
<img width="1070" alt="Screenshot 2024-04-07 at 8 57 34 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/83885e2a-75ff-4ca5-87e5-ee8901b47987">

#### spearman rank correlation between the different audio features

<img width="669" alt="Screenshot 2024-04-07 at 8 58 17 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/0572ccd5-5e62-4f4f-873b-939d940b5d3c">

#### finalized data frame with both song information and audio feature information.

<img width="1421" alt="Screenshot 2024-04-07 at 8 59 30 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/6a350d0c-0261-4f2d-86f4-57d42ab90a0d">

#### Artist that had the most songs in the top 50 
<img width="437" alt="Screenshot 2024-04-07 at 9 00 16 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/2bfe68e7-25b0-4c07-81a8-ee2028be3c93">

#### Music Popularity by Genre
<img width="480" alt="Screenshot 2024-04-07 at 9 01 00 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/fce4162f-bf4d-4bd1-b21c-db8c6bc7d84c">

#### Genre frquency in top 50 songs 
<img width="472" alt="Screenshot 2024-04-07 at 9 01 30 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/9042df1a-adb5-45a8-87ba-9286291a5ed0">

# Average audio score across top 50 songs
<img width="448" alt="Screenshot 2024-04-07 at 9 01 45 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/6e7f279f-32fb-4e85-bccb-57b01414e8aa">

## 5) Visulaization and Analysis for US Top 50 Playlist 

#### Top US Songs 
<img width="792" alt="Screenshot 2024-04-07 at 9 03 38 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/7def5b2e-3214-4dfd-8d84-cd8b2c45ac43">

#### Audio features and correlations 
<img width="1087" alt="Screenshot 2024-04-07 at 9 03 49 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/5bea5700-2c69-40a6-b3c6-99f380dd6e5b">

<img width="457" alt="Screenshot 2024-04-07 at 9 04 28 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/cb3bcb06-d419-4cc9-925b-ec1b05022f5f">

#### Top Artists in top 50 US 
<img width="499" alt="Screenshot 2024-04-07 at 9 04 41 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/3099454e-0d6c-41ac-9a4e-ba74524717eb">

#### Music Popularity by Genre
<img width="541" alt="Screenshot 2024-04-07 at 9 05 03 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/06ac20e2-38f6-4535-b6b4-51bb22ab0525">

#### Genre frquency in top 50 songs 

<img width="493" alt="Screenshot 2024-04-07 at 9 05 43 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/86e881df-424e-4e9e-a284-47b3ff03c235">

#### Average Audio Features 

<img width="473" alt="Screenshot 2024-04-07 at 9 06 06 AM" src="https://github.com/lex910/Spotify-World-Listening-Trends-/assets/101606445/3a5073de-4521-4805-b617-bda7cd93ba93">

## 7) Conclusion and Discussion
Recap of our findings/analysis:
Overall, there were only 19 songs that appeared in both the Global and US top 50 spotify playlists. Additionally, only 22 artists appeared in both the global and US top 50. Given that both of these account for less than 50% of the total songs, we can conclude that there is a difference in the current top songs globally and in the US.

When looking at audio features to determine what factors make songs popular, danceability and energy were among the top two globally and in the US. In the US, the higest audio feature was energy while globally it was danceability. On average pop and reggatone music had the highest danceability scores and since these genres were more present globally, danceability was the highest audio feature. Dancability and speachiness and energy and loudness were the audio features of songs that were the most correlated.

KAROL G currently has the most songs in the global top 50 while Morgan Wallen has the most in the United States. Globally, pop is the most popular genre amount the top 50 and also has the highest average song popularity score. In the US, country is the most frequent genre but has the lowest average popularity score most likely due to the fact of the recency of Morgan Wallen's new album. The songs have not had enough time to accumulate total listens which is factored into the determination of the track popularity score.

Limitations to our research:
While we were successful in answering our research questions, we did face some limitations that hindered our creativity that we originally were hoping to implement. For exmample, we were interested in analyzing the difference in music taste by age group or by city. For example, would their be differences in the music tastes between Davis, a college town, and Sacramento, a town with more diverse demographics? However, the spotipy package did not provide locations and age groups of listeners, which made this kind of analysis hard out of reach. We also faced limitations in our audio feature analysis. We chose to use the audio features that we measured on the same scale. However, we struggled to impliment the other audio features in our research.

Taking our research further:
One way we hope to advance our project is by running more analysis on our own top songs to compare to the global and US top 50 playlists. By looking at the personal analysis playlist, we realized how much the season and peoples day to day schedule influence their music choices. Since spotify updates the global playlist weekly and the US playlist daily, we would also be curious to re-run our analysis in different seasons to see if results change/remain consistent. For example, do more slow christmas songs enter the top 50 during winter time opposed to the summer when more upbeat songs may overtake the top 50?

## 8) References
Web API reference: Spotify for developers. Home. (n.d.). Retrieved February 25, 2023, from https://developer.spotify.com/documentation/web-api/reference/#/operations/get-track

Welcome to spotipy!¶. Welcome to Spotipy! - spotipy 2.0 documentation. (n.d.). Retrieved February 25, 2023, from https://spotipy.readthedocs.io/en/2.16.1/#module-spotipy.oauth2

