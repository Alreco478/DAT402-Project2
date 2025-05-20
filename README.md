# DAT402-Project2: Music Genre Classification
Alexander Coover
2024-04-16

Dataset: The dataset I selected contains 114 different genres of music, with 1000 songs per genre from Spotify. Each row contains various different metrics and information about the song. Some of the metrics include popularity from 0-100, duration of the song, danceability, energy, key, etc. For the exact features used, refer to the variable importance plot.

Project Summary: For my first project in this class, I used Naive Bayes to try my best and make predictions of what genre a song is based on the features of my dataset. I created a valid model, but I know a lot more machine learning practices now, so I decided to use a random forest to make predictions this time. In addition to cleaning up my Project 1 a bit, I also created code for hierarchical clustering from scratch so that I could combine the 114 different genres present in the dataset into a much smaller pool to select from. After narrowing the pool down to the final genre groups, I created naive bayes and random forest models, then showed how successful each one was using both overall accuracy and accuracy per genre.

Conclusion: The hierarchical clustering was incredibly effective in combining similar genres and was key to the success of the project. I have tested the entire project with 20 final genre groups and got an overall accuracy of 58.7% with naive bayes and 81.7% with random forest. I also tested with 10 final genre groups and got 77% accuracy with naive bayes and 88% accuracy with random forest. I decided to create the report with 13 final groups mainly because the graphs aren’t as cluttered as they are with 20, and 10 final groups seemed to be forcing genre combinations that didn’t make as much sense.

Possible Areas for further improvement of the project:
  - Narrowing down features to reduce dimensionality. Time signature, key, and liveness are not good predictors of genre.
  - Optimizing the number of final genre groups. I did not do this because of computing limitations and I did not want to wait for it to run.
  - Creating more intentional names for the genre groups. Every time 2 are combined, the decision of which genre takes the other’s name is decided by alphabetical order. I could probably look into the tree and come up with one of the genres that is within it, not necessarily the current name, and pick that to best suit the genres contained.

