# Disaster_tweets

This project uses an introductory dataset from Kaggle.com about sentiment analysis of Tweets.
The tweets are split into two categories, either "Disaster" or "Not Disaster".
And the goal is to train an unsupervised learning algorithm to classify tweets based on text into either category.

The goals
* To perform sucessful data cleanup to provide the best overall model performance possible.
* To train a model to predict whether a tweet falls into category 1 or 0 based on the contents of the text column in either data set.

Model Selection, and hyperparameter tuning:
The model I chose was the Bidirectional LSTM.
Which stands for Long Short Term memory.
Bidirectional LSTM or BiLSTM is a term used for a sequence model which contains two
LSTM layers, one for processing input in the forward direction and the other for processing in the backward direction.
It is usually used in NLP-related tasks. The intuition behind this approach is that by processing data in both directions,
the model is able to better understand the relationship between sequences (e.g. knowing the following and preceding words in a sentence).*https://www.geeksforgeeks.org/bidirectional-lstm-in-nlp/#

Results and Discussion:
Over all my best performing model was model number 9. The worst performer was model number 16.
The increases are marginal. But this helps show what works and what does not.
And also most of the models (except for 16)

What helped improve results the most in my opinion.Was reducting learning rates.
Reducing learning rates had the greatest effect. The accuracy increased but the stability of the validation results between training sessions did also, meaning
the models fit better to the validation data. And that might mean better results on the test data.
Please see the figure below. The green line is the overall accuracy for model 7,
and it looks much smoother and less jagged than model 9. But model 9 shows better results for the validation accuracy.

![plots_for_github](https://github.com/oohtmeel1/Disaster_tweets/assets/115196648/cddefb9e-3b53-4b88-9d04-ed7719381bf9)



