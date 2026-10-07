# MachineLearning-Projects

## Spam Detection Model
The goal of this system is to classify emails as "spam" or "nospam"
Dataset is taken from Kaggle: [Here](https://www.kaggle.com/datasets/venky73/spam-mails-dataset/data).

Following steps were take for spam detection.

Data Cleaning:
1. Remove unnecessary columns
2. Rename columns for clarity
3. Remove duplicates.
4. Check for null values

Exploratory Data Analysis:
1. Total Ham vs Spam
2. Avg length of emails for spam vs ham
3. Avg words for emails of spam vs ham
4. Word Cloud for Spam vs Ham

Data Pre-processing:
1. Lower-case: the characters of the email are made lower-case
2. Regex: is used to remove special characters and white-spaces.  
3. Stopwords: stopwords for eng langage were removed.
4. Stemming using nltk.PorterStem

Machine Learning: 
1. A TF-IDF vectorizer was used to convert features (email contents) and target (0 or 1). 
2. An 80/20 split was done for Test/Train data 
3. Naive Bayes algorithm was used for the model training. 

Finally, the model's performance is evaluated using methods like:
1.  Confusion Matrix
2. Accuracy: 94% accuracy was reported
3. Classification Report: F1 score, precision and recall were noted.
