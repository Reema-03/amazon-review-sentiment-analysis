# Amazon Review Sentiment Analysis using NLP and Machine Learning

## Project Overview

This project performs sentiment analysis on Amazon product reviews using Natural Language Processing and Machine Learning. The goal is to classify customer reviews into positive, neutral, or negative sentiment categories.

The project compares traditional machine learning models with a rule-based NLP model called VADER.

## Objective

The main objective of this project is to analyze Amazon customer reviews and build a sentiment classification system that can predict whether a review is positive, neutral, or negative.

## Dataset

The dataset used in this project is the Amazon Fine Food Reviews dataset.

Dataset source: Kaggle Amazon Fine Food Reviews dataset

The original dataset contains Amazon product reviews along with ratings, review text, summary, user information, and product information.

For this project, a subset of 50,000 reviews was used for efficient experimentation in Google Colab.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn
- TF-IDF Vectorizer
- VADER Sentiment Analyzer

## Project Workflow

1. Loaded Amazon review dataset
2. Selected useful columns: review text, rating, and summary
3. Removed missing values and duplicate reviews
4. Created sentiment labels from ratings
5. Performed exploratory data analysis
6. Analyzed rating distribution and sentiment distribution
7. Performed review length analysis
8. Cleaned text data using NLP preprocessing
9. Converted text into numerical features using TF-IDF
10. Trained multiple machine learning models
11. Applied VADER rule-based sentiment analysis
12. Compared all models using evaluation metrics
13. Built a custom sentiment prediction function
14. Saved the trained model and vectorizer

## Sentiment Labeling

The review ratings were converted into sentiment labels as follows:

| Rating | Sentiment |
|---|---|
| 1-2 | Negative |
| 3 | Neutral |
| 4-5 | Positive |

## Models Used

The following models were used in this project:

- Logistic Regression
- Naive Bayes
- Linear SVM
- VADER Sentiment Analyzer

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

## Results

The final models were compared using weighted F1-score. The best performing model was selected based on the evaluation results.

Machine learning models using TF-IDF performed well because they learned patterns from the review text. VADER was added as a rule-based NLP approach and compared with the supervised machine learning models.

## Business Insights

- Most reviews in the dataset are positive, showing that satisfied customers are more likely to leave reviews.
- Negative reviews can help businesses identify issues related to product quality, delivery, packaging, or customer expectations.
- Neutral reviews are harder to classify because they often contain mixed opinions.
- Sentiment analysis can help e-commerce businesses monitor customer feedback at scale.

## Files in This Repository

| File | Description |
|---|---|
| `Amazon_Review_Sentiment_Analysis.ipynb` | Main Google Colab notebook |
| `requirements.txt` | Required Python libraries |
| `best_sentiment_model.pkl` | Saved best machine learning model |
| `tfidf_vectorizer.pkl` | Saved TF-IDF vectorizer |
| `model_comparison_results.csv` | ML model comparison results |
| `final_model_comparison_with_vader.csv` | Final comparison including VADER |
| `sample_reviews_with_vader.csv` | Sample reviews with VADER predictions |

## How to Run This Project

1. Open the notebook in Google Colab.
2. Upload or mount the Amazon reviews dataset from Google Drive.
3. Install/import the required libraries.
4. Run all notebook cells from top to bottom.
5. Check the model comparison table and final evaluation results.

## Future Improvements

- Train the models on the full dataset
- Add deep learning models such as LSTM or BERT
- Deploy the model using Streamlit
- Build a dashboard for business users
- Perform product-category level sentiment analysis

## Conclusion

This project demonstrates an end-to-end NLP pipeline for sentiment analysis using Amazon product reviews. It includes data cleaning, EDA, text preprocessing, model training, VADER analysis, model evaluation, and business insights.
