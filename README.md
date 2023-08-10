
# Spam-Assassin-NLP-Fully-Deployed

A supervised deep learning project using Natural Language Processing(NLP) that classifies a given SMS as a spam/ ham message.
The dataset is so versatile that it can be used to train a model to detect spam e-mails also.

### Link for deployed website: 
https://spam-assassin-nlp-1l2xdjbo0gj.streamlit.app/
![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/a05d31ab-3be1-45ff-b1b3-0c38bb267354)

Steps followed are:

    1. Data Cleaning
    2. Exploratory Data Analysis(EDA)
    3. Text Processing
    4. Model Building
    5. Evaluation
    6. Improvement
    7. Website
    8. Deployement using streamlit

### Input
https://www.kaggle.com/datasets/bagavathypriya/spam-ham-dataset (Originally taken from UCI machine learning repository) . Note that although the dataset says SMS, it has a significant resemblance to the E-Mail spam dataset also.

Used NLP techniques such as tokeniztion , lemmatization , stop words removal , punctuation removal using NLTK and regex. Also performed feature engineering and handcrafted features such as number of digits, email length, number of punctuations etc which further helped in predictions . Implemented models such as Multinomial Naive Bayes, Gaussian Naive Bayes, Bernouli Nave Bayes and many other classification models to check the best performing model through accuracy and precision. Combined some best performing models to make an ensemble model to tweak the accuracy score from 97.87 to 98.16. 

Lastly, designed a basic UI to accept new input to be classified as spam/ ham. The model was saved using Pickle(a Python tool) and hosted using streamlit.

### Dependency/ Library Used
Pandas

Numpy

Sklearn

NLTK

Seaborn

Pickle

Streamlit

### Model Building
* ##### Imbalanced Data

![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/13ec0cb8-f49b-4564-b3d1-757a9cfc66b0)

* Visualizing the trend of number of characters, number of words and number of sentences in a spam/ ham SMS

![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/9e4d774f-389e-461b-8d2a-d0b5d7cdf812)

* Plotting the trend as a Heatmap

![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/04513436-f54a-44c7-986e-da3aa30dc6dd)

* Most common words in a Spam Corpus
  
![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/089dbb97-cdbd-4e41-91a2-4492aba02f6c)

* Most common words in a Ham Corpus
  
![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/1e3892f2-201d-4058-a6cb-8daa8daa91c6)

* Performance of Various Models
  
![image](https://github.com/AkGu2002/Spam-Assassin-NLP/assets/74046369/177d75ff-32ca-4065-bbd9-5e64ee30d14a)


### Top Performing Model
Combined Support Vector Classifier, Multinomial Naive Bayes and Extra Trees Classifier to build an Voting Classifier Model( Ensemble Model) whose:

*accuracy:* 0.9816247582205029

*precision:* 0.983739837398374










