# -Tinder-Review-Sentiment-Analysis

Project Overview

This project leverages Natural Language Processing (NLP) and Machine Learning (ML) to analyze user sentiment in Tinder reviews from Google Play. By classifying reviews into positive, negative, and neutral sentiments, we extract valuable insights into user experiences, common complaints, and feature requests. Additionally, we apply topic modeling to uncover recurring themes in user feedback, providing actionable recommendations for improving the platform.

Methodology

1: Data Preprocessing

Tokenization: Breaking text into individual words for analysis.
Part-of-Speech (POS) Tagging: Identifying adjectives, nouns, and verbs.
Lemmatization: Reducing words to their base form for consistency.
Stopword Removal: Eliminating common words that do not add meaning.
Adjective Extraction: Identifying key descriptive words used in reviews.
Word Frequency Analysis: Identifying the most frequently used adjectives to determine common themes.

2: Sentiment Classification

We used two ML models to classify user sentiment:

Naïve Bayes (TF-IDF & CountVectorizer): Achieved 84.29% accuracy with TF-IDF.

KNN with Cosine Similarity: Achieved 82.7% accuracy with k = 15.

Final Choice: Naïve Bayes (TF-IDF) due to its higher accuracy and efficiency.

3: Topic Modeling (LDA - Latent Dirichlet Allocation)

We extracted key topics from reviews by training LDA models with 5 and 6 topics. Major identified themes included:

Fake Profiles & Bots. 
Subscription & Pricing Concerns.
Account Bans & Moderation Issues.
User Engagement & Matching Algorit.hm 
Technical Glitches & Performance Problems.

Results & Insights

User dissatisfaction is primarily driven by fake profiles and pricing concerns.
Subscription complaints are frequent, suggesting a need for clearer pricing and billing policies.
Moderation and account bans frustrate users, indicating possible transparency improvements.
Positive feedback highlights good matches and user experience but is outweighed by concerns.
LDA topic modeling helped identify key problem areas for app improvement.

Tech Stack & Libraries

Programming Language: Python 
NLP & Machine Learning: NLTK, scikit-learn, spaCy
Data Visualization: matplotlib, wordcloud
Topic Modeling: gensim, LDA
