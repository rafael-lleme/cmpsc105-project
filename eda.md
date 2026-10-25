# Spotify Streaming Behavior
## Deliverable 1

The main goal of this part of the project is to analyze the characteristics of the available songs in the Spotify dataset, and investigate if there is any corelation between those characteristics and the popularity of a song. Because we are simulating a group of data scientists working for a record label, we'll need to understand if factors such as danceability, energy, tempo, and music genre can help us identify what makes a song a hit.

At first, the dataset has 114000 entries and 21 columns, including information about the artist, albums, genres and sound related characteristics of the songs. 

During the first analysis, I identified 3 missing values in the "Artists" column, album_name and track_name all were at the same entry. Because it was only a singular line between 114000, i decided to remove it, because i wouldn't be a signficant information loss. I also removed the "Unnamed: 0", since it represented a unnecessary variable.

Another finding was the presence of 42.259 repeated track IDs, when i took a closer look at it, i noticed that some song appeared in different music genres. Because of it, i decided to keep those repetitions, so we don't lose information on the songs' classifications.

After the data cleanse, the data set was at 113999 entries and 20 columns.

The average popularity of the songs was approximately 33.24 in a 0 to 100 scale, while the median was 35. The histogram showed a bigger concentration of entries with low / moderate popularity, while songs with scores above 80 were relatively rare. Besides that, approximately 14.05% of the entries had a popularity score of 0.

I also analyzed the relationship with danceability and popularity, using a scatter plot and calculating the correlation. The result was only 0.035, indicating a really weak positive-linear relation. That suggest that a song being more "danceable" doesn't necessarily mean it will be more popular.

On the other hand, when comparing 5 music genres using a box plot, I found considerable changes. Pop and Hip-Hop showed the highest popularity medians, close to 66 and 58, while rock, country, and classical showed significantly lower ones. That brings up the possibility that a music genre is more associated with popularity than the danceability by itself, even though we need more analysis to confirm that hyphothesis.

One of the biggest limitations I found was the distribuition of music genres. The data set contains 114 genres. practically all of them with 1000 entries. That suggests that the data was selected in a balanced / controlled way, instead of representing real distribuition in Spotify songs.

Besides that, the presence of repeated song in different genres can influence statistic results, because some songs can lead to more weight in the analysis.

Another important point is that the data set uses a popularity score, but doesn't present directly the numver of streams / listeners. So we can't really affirm that a song with zero popularity was never reproduced.

Finally, factors such as investment in marketing, artist recognition, and playlist presence can also influence popularity, but they're not present in the dataset.

This initial exploration showed that there isn't a strong linear relation between danceability and popularity, whereas the difference between music genres were more evident. However, we still can't conclude that the genre is the main factor responsible for the success of a song.

For the next analysis, it'd be interesting to investigate other characterists such as compare correlations within the different genres and analyze if popular hit songs share specific patterns. The objective will be understanding the factor that are associated with the musical success better, considerig the data set's limitation.
