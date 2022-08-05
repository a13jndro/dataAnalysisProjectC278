<h1>Data Analysis Final Project C278 <br/><a href="https://github.com/a13jndro"> </a>

<h2>Data Analysis Techniques</h2>

<p align="justify"> The goal of data analysis is to take a large pool of raw data and transform it into a meaningful dataset that allows users to make business decisions based on the data. However, even after the transformation process, raw data can be difficult to read and interpret on its own, especially when there may be millions of records to evaluate in a single dataset.
As a result, data analysis processes often include the use of visualizations, typically in the form of charts or other diagrams that present aggregated data in a format that is easier for humans to read and interpret. 
</p>

<h2>Project Goal</h2>

1. Creating Database:
- Select the top 200 songs of Spotify charts for each genre.
- Use Spotify API to get audio features.
- Use Genius API to get lyrics.
- Use package Spacy to identify language.
- Narrow dataset to only english songs.
  - Songs that did not have non english complete phrases.
- Unidecode to replace accents:
  - replaced undefined symbols with spaces.
  
2. Prediction Models (RandomForest, DescisionTree, SVC, Logistic Regression, Neural Network).
- Split the audio features data into training set (2/3 of the songs) and testing set (remaining 1/3).
- Trained the models on the training set by calling model.fit with the training data.
<p align="justify">- Scored the models on the testing set by calling model.score with the testing data.
<p align="justify">- SVC and Logistic Regression had low scores (15% and 11%) but RandomForest and DescisionTree were a bit better (27% and 42%), and Neural Network was by far the best at 81%
- Use plot-confusion-matrix module to create confusion matrices with the results from the models for the testing data for RandomForest and DescisionTree, which showed that a lot of the misclassifications were understandable (i.e. Hip Hop classified as R&B or Pop).</p>
- The results of the neural network had to be converted from vectors of scores to a single predicted genre in order to make a confusion matrix- again, the misclassifications were understandable and the results are better understood as a set of possible genres.</p>


<h2>Languages and Utilities Used</h2>

- <b>Python 3.8.2</b> 
- <b>Jupyter Notebooks</b>
- <b>PyCharm 2022.1.1 (Edu)</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
