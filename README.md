# Twitter Sentiment Analysis using Neural Networks
The repo includes code to process text, engineer features and perform sentiment analysis using Neural Networks. The project uses **LSTM** to train on the data and achieves a **testing accuracy of 79%**. LSTM is good at capturing the long-distance semantics between the words in a sentence.


Twitter sentiment analysis allows you to keep track of what's being said about your product or service on social media, and can help you detect angry customers or negative mentions before they they escalate. At the same time, Twitter sentiment analysis can provide valuable insights that drive decisions.

## Setup to use this code.

### Download the dataset
The dataset has been taken from [Kaggle](https://www.kaggle.com/kazanova/sentiment140)
1. Download the file from kaggle.
2. Extract the zip and rename the `csv` to `dataset.csv`
3. Create a folder `data` inside `Twitter-Sentiment-Analysis-using-Neural-Networks` folder
3. Copy the file dataset.csv to inside the `data` folder

## Working the code

### Understanding the data
The Jupyter notebook **Dataset analysis.ipynb** includes analysis for the various columns in the dataset and a basic overview of the dataset.
1. Run Jupyter
```
jupyter notebook
```
2. Select the file **Dataset analysis.ipynb** from the list to see dataset analysis.

### Twitter Sentiment Analysis
The whole project is broken into different Python files from splitting the dataset to actually doing sentiment analysis. The steps to carry out Twitter Sentiment Analysis are:
1. Run the file `train-test-split.py` to split the Twitter dataset into training and testing data.
```
python train-test-split.py
```
2. Run the file `preprocessing.py` to process the tweets.
- Remove @user mentions
- Remove non-alphabetic characters + spaces + apostrophe
- Remove links
- Remove single characters
- Remove stopwords
- Lemmatize words
- Stem words

Feel free to contribute and use this repo.



