This file provides high level overview of the project.

**Data**
1. The tweets data is about Tesla and downloaded from Kaggle, containing 80,793 tweets from 2021-09-30 to 2022-09-29.
2. The stock data is Tesla daily stock price downloaded from Yahoo Finance, from 2021-09-30 to 2022-09-29.

**Sentiment Generation**
1. Stock_Sentiment_Generation.ipynb
2. The pre-trained model, FinBert, is downloaded from HugginFace.
3. It take around 6 hours to run the model on the Tweets dataset, using Google Colab.
4. The result is saved under the same directory of notebooks, preventing rework due to Google Colab disconnection.

**Stock Prediction**
1. Stock_Sentiment_Prediction.ipynb
2. Process flows
Data Processing
    Step 1: read sentiment generation result saved under the same directory
    Step 2: data processing
    Step 3: install yfinance
    Step 4: download stock data

Using Categorical Features
    Create categorical features
    Analyze relationship between sentiment and stock price movement.
    Feature Engineering
        Step 1: creating training datasets
        Step 2: feature importance analysis, using RandomForestClassifier
        Conclusion

Using Numeric features
    Create numeric features
    Feature Engineering
        Step 1: creating training datasets
        Step 2: feature importance analysis, using RandomForestClassifier
        Conclusion

Train with Other Models
    Creating training datasets
    Decision Tree
    Adaboost
    KNN
    Conclusion

Future improvements
