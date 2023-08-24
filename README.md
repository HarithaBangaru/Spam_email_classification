# Spam_email_classification
The Dataset has two columns:
1. Label the class of data (ham or spam) and
2.Text message
Other unwanted columns are removed.
We drop the last four columns as the last three columns don’t have any values and we don’t need a length column.
# Multinomial Naïve Bayes.
from sklearn.feature_extraction.text import CountVectorizer
countvectorizer =CountVectorizer()
By using this Count-Vectorizer we’ll tokenize a collection of text documents and built a vocabulary, this vocabulary is also used to encode new documents.
# Importing package and fitting model:
from sklearn.naive_bayes import MultinomialNB
multinomialnb = MultinomialNB()
# SVM
# Importing package and fitting model:
from sklearn.svm import LinearSVC
linearsvc = LinearSVC()
linearsvc.fit(x_train,y_train)

By seeing the above results, we can say that the Naïve Bayes model and SVM are performing well on classifying spam messages with 98% accuracy but comparing the two models, SVM is performing better. These models can efficiently predict if the message is spam or not.

