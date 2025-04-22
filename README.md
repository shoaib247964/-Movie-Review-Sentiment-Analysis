# -Movie-Review-Sentiment-Analysis
# 🎬 Movie Reviews Sentiment Analysis

This project analyzes movie reviews using Natural Language Processing (NLP) techniques and classifies them as **positive** or **negative** sentiments using three types of Naive Bayes classifiers.

## 📌 Description

Sentiment Analysis is a popular application of NLP, especially in social media and review platforms. In this project:

- Reviews are preprocessed (cleaned and normalized)
- A Bag of Words model is created using `CountVectorizer`
- Three Naive Bayes classifiers are trained:
  - GaussianNB
  - MultinomialNB
  - BernoulliNB
- Accuracy of each classifier is calculated on test data

## 🧠 Algorithms Used

- **Gaussian Naive Bayes**
- **Multinomial Naive Bayes**
- **Bernoulli Naive Bayes**

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- NLTK
- joblib

## 🧹 Preprocessing Steps

1. Remove HTML tags
2. Remove special characters
3. Convert text to lowercase
4. Remove stopwords
5. Apply stemming

## 🧪 Accuracy

Accuracy scores on the test dataset:

- **GaussianNB**: ~`98`
- **MultinomialNB**: ~`99`
- **BernoulliNB**: ~`99`

*(Replace XX% with actual values after running the script)*

## 📁 Dataset

IMDB reviews dataset in `Dataset/IMDB.csv` containing:
- `review` (text)
- `sentiment` (positive/negative)

## 💾 Output

The trained models are saved in the `Models/` directory:
- `MRSA_gnb.pkl`
- `MRSA_mnb.pkl`
- `MRSA_bnb.pkl`

## 📊 How to Run

```bash
# Install requirements
pip install -r requirements.txt

# Run the script
python movie_reviews_sentiment_analysis.py
