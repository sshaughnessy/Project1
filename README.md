# Project1
Impact of COVID-19 on Music

Contents: 
1.	Why did we choose this project?
2.	What is our Data Source?
3.	What is our Hypothesis?
4.	What are specific questions we addressed?
5.	How did we clean the data?
6.	What is the analysis?
7.	What are additional questions we'd want to address / next steps to accomplish that?
8.	.png's of our key charts / outputs and the code
9.	Link to the GitHub repository
______________________________________________________________________________

1.	Why did we choose this project?
The COVID-19 Pandemic had an impact on everybody’s lives. We were interested in understanding how music trends were impacted during this time. Did music help people get through the hard times? Were people listening to more or less music? How did music change to fit the climate of the world around us during the pandemic?

2.	What is our Data Source?
Data Source: (Sample dataset of a 160,000 songs)
Spotify U.S. Dataset 1922-2021 (Audio features of ~600k songs released in between 1922 and 2021)
https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks?select=data_by_genres_o.csv

3.	What is our Hypothesis?
Alternate Hypothesis: Music released in January 2020 through April 2021 was statistically different than music released in 2015-2019 according to *various metrics, likely a result of the COVID-19 pandemic.

Null Hypothesis: Music released in January 2020 through April 2021 was not statistically different than music released in 2015-2019 according to *various metrics, likely a result of the COVID-19 pandemic.

Various Metrics include: (Metrics are scored in scale of 0 (low confidence) to 1 (high confidence) except for tempo and explicitness)

- Danceability: How suitable a track is for dancing based on a combination of musical elements.
- Speechiness: Speechiness detects the presence of spoken words in a track.
- Acousticness: A confidence measure of whether the track is acoustic (i.e. the track was performed acoustically, without electronic instruments).
- Energy: A perceptual measure of intensity and activity (Fast, loud, noisy).
- Instrumentalness: A measure that predicts whether a track contains no vocals, not counting mouth sounds like "ooh" and "aah."
- Liveness: Detects the presence of an audience in the recording.
- Valence: The musical positiveness conveyed by a track. 
- Tempo: The overall estimated beats per minute (BPM).
- Explicitness: Whether a song contains explicit content.

4.	What are specific questions we addressed?
- Did the various metrics of music change over the last 5 years? 
- Did the various metrics of music change during the COVID-19 Pandemic?
- Did the metrics of tracks streamed change in the last 5 years?
- Did the metrics of tracks streamed change during COVID-19?

5.	How did we clean the data?
Raw Data: Random tracks released from 1922 to 2021 (> 600k tracks)
Basic Clean-Up
- Narrowed Date Range: 2015-2021
- Dropped duplicate rows, removed all “Remastered” songs, converted tempo column to 0-1 scale
- Determined 7 Metrics for Analysis
Dropped extraneous metrics not useful to our analysis (ID, ID_Artist, key, mode, time_signature)
- Dropped Spoken Word Tracks
Dropped tracks with “speechiness” scores over 0.66, since tracks over 0.66 are not considered music.
- Created variables for Month, Quarter, and Year, from release dates for analysis

6.	What is the analysis?
Main Analysis: Music released in January 2020 through April 2021 was statistically different than music released in 2015-2019, possibly a result of the COVID-19 pandemic.

Question 1: 
Most metrics stayed the same over the last 5 years. 
- Explicitness increased the most significantly. 
- Metrics decreased for Q3 to Q4 for most years. 
The increase in explicitness could mean that more artists were comfortable releasing songs that had more explicit language. Metrics decreased at the end of each year could mean that most producers/label companies attempt to release music only at the beginning of the year. 

Question 2: 
Danceability and Energy metric scores most significantly changed
- Danceability scores increased
- Energy scores decreased
The change in scores could mean that songs released during Covid were more danceable, possibly to combat the mood of the pandemic.

Question 3 & 4:
Danceability and Explicit metric scores changed most significantly 
- Both scores increased
The change in scores indicate that songs streamed during Covid were more danceable and explicit  

7.	What are additional questions we'd want to address / next steps to accomplish that?
- Was there a change in music consumption (Spotify subscription trends) during the pandemic?
- How did music trends change by genre?
- Was there a change in user demographics and differences in music that they listen to?
- How many new artists came in Spotify?
- Change in existing artist popularity?
- What are songs in playlists with COVID title?
In order to answer these questions, we would need additional data about Spotify subscriptions, genres released/streamed, user demographics, artist information, and user playlist data. 

8.	Analysis and Data Images (found in images folder)

Prepping the data: 
Question 1 graphs by Year: 
Question 1 graphs by Quarter: 
Question 2: Graph
Question 3: Graphs
Question 4: Graphs
 
9.	Link to GitHub repository: 
https://github.com/sshaughnessy/Project1


![image](https://user-images.githubusercontent.com/83885856/129448395-96af5f17-22d2-408d-a50b-4e1bb87284cc.png)


