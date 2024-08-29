Problem Statement

Social media platforms like Twitter generate massive amounts of user-generated content every day, with tweets reflecting a wide range of sentiments. Businesses, researchers, and analysts often seek to understand public opinion by analyzing these sentiments, but manually categorizing large volumes of tweets is impractical.

Objective: 

The primary goal of this project was to analyze sentiment in tweets, classifying them into positive or negative sentiments using machine learning techniques. The project involved preprocessing raw tweet data, applying unsupervised learning for clustering, and using supervised learning models for classification.

Steps and Methodology:

Data Preparation:

Dataset: The dataset contained tweets with labeled sentiment (target) values of 0 (Negative) and 4 (Positive).
Data Balancing: The dataset was balanced by selecting an equal number of positive and negative tweets, resulting in 20,000 total samples (10,000 positive and 10,000 negative).
Visualization: The distribution of targets was visualized, and word clouds were generated to visualize the most common words associated with each sentiment.
Unsupervised Learning:

Text Preprocessing: Applied text preprocessing techniques, including tokenization and removal of unnecessary characters (e.g., URLs, special characters).
Vectorization and Dimensionality Reduction: Used TF-IDF vectorization to convert text data into numerical form, followed by PCA for dimensionality reduction.
Clustering: Applied K-Means clustering to identify natural groupings within the tweets, visualizing the clusters to gain insights into the data structure.
Supervised Learning:

1. Feature and Label Definition: 

Defined features as TF-IDF vectors and labels as sentiment targets.

2. Model Training and Evaluation: 

Trained and evaluated several supervised learning models, including Logistic Regression, SVM, Random Forest, Gradient Boosting, and Naive Bayes.

3. Metrics: 

Used accuracy, precision, recall, F1 score, and ROC AUC to assess model performance. Confusion matrices were generated to visualize classification results.

4. Model Testing:

Prediction on New Inputs: Created a function to predict sentiment on new tweet inputs, testing the models on manually crafted sentences to evaluate their performance.
Model Comparisons: Compared the predictions across different models to determine the most reliable for sentiment analysis.

Results:

The models achieved strong performance, with Logistic Regression and Random Forest showing the best balance of precision and recall.
The testing phase confirmed that the models could effectively classify new, unseen tweets into positive and negative sentiments.

Conclusion: 

This project successfully demonstrated the use of both unsupervised and supervised learning techniques for sentiment analysis on tweets. The models developed are capable of accurately predicting sentiment, making them valuable tools for social media analysis, customer feedback monitoring, and other applications involving large volumes of text data.

Future Work:

1. Further Feature Engineering:

Incorporating additional features such as word embeddings (e.g., Word2Vec, GloVe) or leveraging pre-trained transformers like BERT could improve model accuracy.

2. Real-Time Analysis: 

Implementing the model in a real-time system to analyze sentiment on live tweets as they are posted.

3. Broader Sentiment Categories: 

Expanding the model to classify tweets into more nuanced sentiment categories (e.g., very positive, neutral, very negative).
