# Natural-Language-Processing-Sentiment-Analysis
Sentiment analysis of the Movie Reviews


## Introduction: 
### Project Overview: 
The goal of the project is to complete classification tasks, where we develop features for the task and demonstrate that we can carry out experiments that show which sets of features are the best for that data.

We have chosen to work with the Kaggle competition move review phrase data, which has been labeled for sentiment. This dataset was produced for the Kaggle competition (https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews). This data uses sentiment analysis provided by Socher et al, detailed at this web site: http://nlp.stanford.edu/sentiment/. 

Additionally, the data was taken from the original Pang and Lee movie review corpus, which is based on reviews from the Rotten Tomatoes website. Socher’s group used crowdsourcing to manually annotate all the subphrases of sentences with a sentiment label ranging over: “negative”, “somewhat negative”, “neutral”, “somewhat positive”, “positive”. 

The following table shows the numbers associated with the sentiment labels in the dataset:

------------ | -------------
0 - | --Negative
1 | Somewhat Negative
2 | Neutral
3 | Somewhat positive 
4	| Positive 


### Data Review: 
We used training data “train.tsv” and testing “test.tsv” datasets for our experiments. The train.tsv dataset contained the reviews with their related sentiment labels. In addition, each phrase is given a SentenceId that corresponds to each sentence. This allows us to track which sentences belong to which reviews.  The test.tsv dataset contains only the reviews and their associated SentenceId. We will seek to assign a sentiment label to each of these reviews. 

Below, we will first review our text classification tasks. This includes the steps taken to process the text, tokenize it, and if we chose to complete some pre-processing or additional filtering steps. We will then, for Phase Two,  produced “bag of word” features in the notation of the NLTK. This function will be written in Python. For Phase Three, we will complete several experiments where we will use two different sets of features and compare their results. We have chosen to first use the Unigram feature as a baseline and see if  we can improve accuracy after pre-processing. Our second experiment will be a POS tag features. After, we will use sentiment lexicon and count the subjectivity features (positive count and  negative count).  Our fourth experiment will be representing negation of opinions. Finally, our fifth experiment will use Bigram features in addition to Unigram features. For Phase Four of our project, we will use the NLTK Naïve Bayes Classifier to train and test a classifier on each of our feature sets. We will analyze  the results by using cross-validation to compare their precision, recall, and F-measure scores. Additionally, for our advanced task, we trained the classifier on the whole training set and tested it on a separate test set. We chose to use Weka  and Sklearn to accomplish this task.

We have chosen to remove all mentions of python code from our report. For specific technical questions, please see the appendix or attached python code. 
