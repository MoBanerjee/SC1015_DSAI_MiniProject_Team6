# <u>What influences Song Popularity more - Lyrics or Other Statistical Features like tempo, loudness, etc?</u>
## About
While composing songs, artists need to focus on several parameters like- lyrics, tempo, duration,danceability, etc. to name a few. Often, the artists are confused about which feature of the song they should focus more on. Additionally, despite the hardwork, many songs fail to gain sufficient popularity among the audience.Keeping this problem in mind, the goal of our SC1015 Mini-project is to find out which parameters of a song influence its popularity more- its lyrics or its other statistical features like tempo, danceability, etc. Analysing this influence using data science can assist artists in focusing more on relevant features and thus, in releasing more chartbuster songs.

To achieve this goal, we followed the following steps-:

1. Extract suitable datasets- one for lyrics and other for features like tempo,key,etc
2. Clean the datasets
3. Use suitable models for predicting popularity index of song
4. Compare the accuracy of prediction done using lyrics and prediction done using the other statistical features to decide which gives a better prediction    and thus, influences popularity more.

## Presentation
Presentation Video-: [Click Here](https://youtu.be/8SpMJKR04Vw)

For detailed walkthrough, please view the source code in order from:

  1. Data Extraction and Cleaning
  2. Data Visualisation and EDA
  3. Train-Test Split
  4. Sequential Neural Network
  5. Random Forest
  6. Linear Regression (For Statistical Data)
  7. LSTM Network
  8. Linear Regression (For Lyrics Data)

## Problem Definition
What predicts Song Popularity better - Lyrics or Other Statistical Features like tempo, loudness, etc?

Features Analysed-:
 1. Numerical: tempo, danceability, loudness etc.
 2. Categorical: explicit (true/false)
 3. Lyrics: language

## Datasets Used
We extracted these two datasets from Kaggle.
  1. Dataset for statistical features like tempo, key, etc-: [Click Here](https://www.kaggle.com/datasets/lehaknarnauli/spotify-datasets/code?select=tracks.csv)
  2. Dataset for lyrics data-: [Click Here](https://www.kaggle.com/datasets/neisse/scrapped-lyrics-from-6-genres?select=lyrics-data.csv)

## Models Used
Models used for predicting popularity using features like tempo, key, loudness, etc :
  1. Sequential Neural Network
  2. Random Forest
  3. Linear Regression
  
Models used for predicting popularity using lyrics :
  1. Long Short-Term Memory (LSTM) Network
  2. Linear Regression

## Conclusion
  1. For statistical data, we obtained the best results with neural networks.It yielded a Mean Squared Error of only 0.026 which is lesser than that given      by both the baseline models(Random Forest and Linear Regression).
  
  2. Random Forest model yielded an MSE of 15.53. It fared better than regression but fell short of the accuracy given by neural networks.
  
  3. Regression model performed the worst as it yielded a large mean squared error of 261.71 and a poor R square score of 0.23 for statistical data.
  
  4. For lyrics data, we obtained the best results with LSTM.It yielded a Mean Squared Error of only 0.045 which is lesser than that given by the baseline      model(Linear Regression) used.
  
  5. Since the mean squared error of statistical data(0.026) is lesser than that of lyrics data(0.045), hence we conclude that the statistical features          like liveness, tempo, danceability, etc are better predictors of the popularity of a song than its lyrics. Thus, our inference would be that artists        should focus more on these statistical features than on lyrics in order to compose more chartbuster songs.
  
## Takeaways
* Data Pre-processing (Text Processing for Natural Language Processing)
  1. Tokenization
  2. Stemming
  3. Stopwords Removal
* Machine Learning
  1. Implementing Sequential Neural Network
  2. Implementing LSTM Network

## References
1. https://www.kaggle.com/datasets/lehaknarnauli/spotify-datasets/code?select=tracks.csv
2. https://www.kaggle.com/datasets/neisse/scrapped-lyrics-from-6-genres?select=lyrics-data.csv
3. https://towardsdatascience.com/text-preprocessing-in-natural-language-processing-using-python-6113ff5decd8
4. https://www.activestate.com/resources/quick-reads/how-to-create-a-neural-network-in-python-with-and-without-keras/
5. https://towardsdatascience.com/random-forest-in-python-24d0893d51c0

## Contributors
  1. Ananya Agarwal - Data extraction, Data cleaning and EDA 
  2. Mohor Banerjee - Models for Statistical Data
  3. Shrivardhan Goenka - Models on Lyrics Data















