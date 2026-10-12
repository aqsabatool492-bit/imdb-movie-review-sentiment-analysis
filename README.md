🎬 IMDB Movie Review Sentiment Analysis
Exploratory Data Analysis & Natural Language Processing Classification
A machine learning project that analyzes IMDB movie reviews and classifies them as positive or negative using Natural Language Processing (NLP) and the Multinomial Naive Bayes algorithm.

📌 Project Overview
Sentiment analysis is a Natural Language Processing (NLP) technique used to identify the emotional tone of text. In this project, the IMDB movie review dataset is explored, cleaned, and used to train a machine learning model that predicts whether a movie review expresses a positive or negative sentiment.

The project covers the complete workflow, from Exploratory Data Analysis (EDA) to text preprocessing, model training, and performance evaluation.

🎯 Objectives
Perform Exploratory Data Analysis on the IMDB movie review dataset.
Understand the distribution of positive and negative reviews.
Analyze review lengths and frequently occurring words.
Clean and preprocess textual data for machine learning.
Convert text into numerical features using TF-IDF vectorization.
Train a Multinomial Naive Bayes classification model.
Evaluate the model using standard classification metrics.
Predict the sentiment of new movie reviews.
🛠️ Technologies & Libraries
Python — Core programming language
Pandas — Data loading, manipulation, and analysis
NumPy — Numerical operations
Matplotlib — Data visualization
Seaborn — Statistical visualizations
Scikit-learn — Machine learning, feature extraction, and evaluation
Jupyter Notebook — Interactive development environment
Natural Language Processing (NLP) — Text analysis and preprocessing
📂 Dataset
Dataset Source: https://github.com/SK7here/Movie-Review-Sentiment-Analysis/blob/master/IMDB-Dataset.csv
The dataset contains 50,000 movie reviews labeled as positive or negative. The CSV file is not included in this repository due to its large size. 
To run the notebook, download IMDB-Dataset.csv from the source above and place it in the same directory as the notebook.
Dataset features:

Column	Description
review	Text of the movie review
sentiment	Sentiment label: positive or negative
The dataset initially contains 50,000 reviews. After data preparation, 49,582 usable reviews were retained for analysis and model development.

The dataset contains two sentiment classes, making this a binary classification problem.

🔍 Exploratory Data Analysis (EDA)
EDA was performed to understand the dataset's structure, quality, and textual characteristics.

Key analysis included:

Dataset dimensions, column names, and data types
Missing values and duplicate records
Distribution of positive and negative reviews
Review length analysis using character, word, and sentence counts
Comparison of review lengths across sentiment classes
Inspection of HTML tags, URLs, digits, and uppercase text
Identification and visualization of frequently occurring words
Analysis of sentiment distribution across review-length groups
Examination of representative positive and negative reviews
⚙️ Data Preprocessing
The following preprocessing steps were applied before model training:

Removed records with missing reviews or sentiment labels.
Standardized sentiment labels and retained positive and negative classes.
Removed empty reviews and duplicate review-label records.
Cleaned HTML tags and decoded HTML entities.
Removed URLs and unnecessary whitespace.
Converted text into numerical features using TF-IDF vectorization.
Used unigram and bigram features to capture individual words and two-word phrases.
The dataset was divided into training and testing sets using an 80:20 split, with stratified sampling to preserve the class distribution.

🤖 Machine Learning Model
Multinomial Naive Bayes
Multinomial Naive Bayes is a probabilistic classification algorithm commonly used for text classification tasks. It estimates the probability that a review belongs to a particular sentiment class based on its text features.

TF-IDF Vectorization
Term Frequency–Inverse Document Frequency (TF-IDF) transforms text into numerical features. It gives greater importance to words that are informative within a review while reducing the influence of words that occur frequently across many reviews.

Model Pipeline
The machine learning pipeline consists of:

Text cleaning and preprocessing
TF-IDF feature extraction
Multinomial Naive Bayes classification
Sentiment prediction and probability estimation
A pipeline combines feature extraction and classification into a single workflow, ensuring that the same transformation process is applied during training and prediction.

📊 Model Performance
The model is evaluated using the following metrics:

Accuracy: Overall proportion of correctly classified reviews.
Precision: Proportion of predicted reviews in a class that actually belong to that class.
Recall: Proportion of actual reviews in a class correctly identified by the model.
F1-Score: Harmonic mean of precision and recall.
ROC-AUC: Measures how well the model distinguishes between positive and negative reviews.
Confusion Matrix: Shows correct and incorrect predictions for both sentiment classes.
The notebook also visualizes the confusion matrix and ROC curve and tests the trained model on new sample reviews.

Final performance metrics will be added after the model finishes training and the evaluation results are verified.

📈 Key Learnings
Understanding the complete workflow of a text classification project
Performing EDA on a large textual dataset
Cleaning and preparing text for machine learning
Converting unstructured text into numerical features
Understanding TF-IDF vectorization and n-gram features
Applying Multinomial Naive Bayes to sentiment classification
Evaluating classification models using multiple performance metrics
Building a reusable Scikit-learn pipeline for text prediction
📂 Repository Structure
imdb-movie-review-sentiment-analysis/
│
├── README.md
├── IMDB-Dataset.csv
└── imdb-movie-review-sentiment-analysis-naive-bayes.ipynb
🚀 Getting Started
1. Clone the Repository
git clone https://github.com/YOUR-USERNAME/imdb-movie-review-sentiment-analysis.git
Replace YOUR-USERNAME with your GitHub username.

2. Navigate to the Project Directory
cd imdb-movie-review-sentiment-analysis
3. Install the Required Libraries
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
4. Launch Jupyter Notebook
jupyter notebook
Open imdb-movie-review-sentiment-analysis-naive-bayes.ipynb and run the cells in order.

🔮 Future Improvements
Experiment with alternative text vectorization techniques.
Compare Multinomial Naive Bayes with Logistic Regression and Support Vector Machines.
Optimize model parameters to improve classification performance.
Explore advanced NLP techniques and transformer-based sentiment classification.
Test the model on additional movie reviews and real-world text data.
👩‍💻 Author
Aqsa Batool

Computer Science Student | Data Science & Machine Learning Enthusiast

This project is part of my hands-on learning journey in Data Science, Natural Language Processing, and Machine Learning.
