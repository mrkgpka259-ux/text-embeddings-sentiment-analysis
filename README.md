This project implements an embedding-based sentiment analysis system using a Twitter dataset containing approximately 27,000 tweets. The objective is to classify tweets into three categories: Positive, Neutral, and Negative using transformer-based text representations.

Rather than relying on traditional methods such as TF-IDF or Bag-of-Words, this project utilizes Sentence-BERT (all-MiniLM-L6-v2) to generate dense semantic embeddings for each tweet. These embeddings capture contextual meaning and relationships between words, enabling more accurate sentiment classification, especially for short and informal social media text.

The workflow begins with text preprocessing, including lowercasing and removal of URLs, mentions, hashtags, and punctuation. After cleaning the data, embeddings are generated for all tweets. The dataset is then split into training and testing sets, and a Logistic Regression classifier is trained on the embedding vectors to predict sentiment labels.

Model performance is evaluated using standard metrics such as Accuracy, Precision, Recall, and F1-score. A confusion matrix is included to analyze class-wise performance and identify misclassification patterns. Additional exploratory data analysis is performed through sentiment distribution plots, text length analysis, and class-wise word clouds to understand dataset characteristics.

The model achieves strong overall performance, demonstrating that transformer-based embeddings significantly improve sentiment classification compared to traditional feature engineering approaches. Custom tweet predictions further validate the practical effectiveness of the system.

This project showcases the power of modern embedding techniques in natural language processing and highlights their applicability to real-world sentiment analysis tasks.
