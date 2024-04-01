# Wrapped_Project

***Added 04/01/2024: This project was completed in April 2022 as the final project of the course CMSE 202: Computational Modeling and Data Analysis II at the Michigan State University. My contributions are data slicing, all algorithms, and cross-validation.***

***Below is the original description:***

This project is a model of Spotify Wrapped. Our project uses packages like numpy and pandas to take data and reduce it down into readable and easy to manupilate dataframes. The data used in this project was taken from our own spotify history (as Spotify allows for you to download your streaming history for the last year); the data files were the streaming histories from groupmates Raksha Sridharan, Jack Haggerty, Jacob Kaspar, Hannah Sullivan, Hande Huang, and an extra dataset by an associate of Jacob's, delivered from Spotify. Our project also uses a csv named tracks.csv by Yamac Eren Ay that is an accumulation of many songs from 1921 to 2020; specifically on Spotify. It doesn't have all of the songs currently on Spotify that have been released during these years, but it has many of them, and is extremely useful for our project. It has nine features that we will use to help find similar songs via knn to the songs on our streaming histories. 

Our project also uses a package called spotipy, created by Paul Lamere (plamere on Github) and other contributors. Spotipy allows for ease of access into spotipy's data on artists, genres, albums, playlists, and more, which were instrumental to helping us understand how we were going to create the recommendation feature for our project. 

The project is a file of code that can be ran straight from the start that has methods of recommendation based on a playlist, a dataframe, passed through as an input. The dataframe is cleaned up and we start finding a recommendation based on the 100 top artists and top 10 genres. Next is a function to get the tracks, artist, and msPlayed of the streaming history that are unique values with no duplicates. We read in tracks.csv, clean up the dataframe, and sort by popularity. We use our personalized data and the nine features from tracks.csv via a 9D coordinate function and a distance function to output the nearest neighbors with a knn function. At the end you get your recommended songs, your top listened to genres, artists, and songs, as well as a visualization of your top listened to songs in the form of a frequency bar graph.

In an attempt to make the code as user friendly as possible, an explanation of how to run the code follows. Firstly, one must obtain their Spotify history from the past year. This can be acquired through the Privacy Settings tab under User Account. Once this has been sent (and how many 'Streaming History' files are has been determined), simply running each cell of the code will ask the user how many files, ask them to select each file, then at the end, spit out their Spotify Wrapped.

A bulk of our work was done between Han, Jacob, Hannah, and Raksha. Hannah and Jacob worked on figuring out how to intially look at, clean up, and analyze our personal spotify data and how to work Spotipy. Han helped with a bulk of the actual knn code and functions, as well as finding tracks.csv to help cross-reference our data. Raksha and Hannah helped to keep the slides and README.md cleaned, up to date, and organized, and Jacob worked to make sure the final notebook was documented, clean, and functioning. Our groupmate Jack helped in the initial two brainstorming sessions and sent in his streaming data but was unable to actually contribute much code in the making of the project. 


# Resources:

Lamere, P. et al. (2014). Spotipy. https://github.com/plamere/spotipy. https://spotipy.readthedocs.io/en/2.19.0/. 

Ay, Y. (2021). "Spotify Dataset 1921-2020, 600k+ Tracks". https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks?select=tracks.csv. 

Spotify 


# Packages Used:

Numpy

Pandas 

Math 

json

tkinter

Matplotlib.pyplot 

Seaborn

Functools

Random
