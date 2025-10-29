📰 News Article Topic Modeling using LDA & BERT
📘 Project Overview

This project focuses on unsupervised topic modeling of a large collection of news articles to identify key themes and insights. Two models were applied — Latent Dirichlet Allocation (LDA) and BERTopic (based on BERT embeddings) — to explore and extract dominant topics, visualize trends, and evaluate model quality.

🎯 Objective

The main goal is to uncover hidden topics within a massive news dataset and understand how certain words or themes dominate public discussions.
This helps in understanding media trends, public interest, and emerging issues.

🧠 Models Used
1️⃣ Latent Dirichlet Allocation (LDA)

Used bag-of-words representation.

Extracted top topics from 20,000 news articles.

Visualized topic-word relationships using pyLDAvis.

Identified dominant words such as: said, people, year, time, government, new, day, life, woman, story.

Evaluation:

Coherence Score: 0.4765

Indicates moderate topic interpretability — topics make logical sense and contain meaningful word clusters.

2️⃣ BERTopic

Built using BERT embeddings + UMAP for dimensionality reduction.

Captures semantic relationships between words better than LDA.

Automatically assigned topics to articles and visualized clusters.

Model saved for future use and new data prediction.

🔍 Workflow

Data Preprocessing

Cleaned, tokenized, and normalized text data.

Removed stopwords, punctuation, and special symbols.

Model Training

LDA and BERTopic trained on preprocessed data.

Models and vectorizers saved using joblib.

Visualization

pyLDAvis for LDA topic visualization.

BERTopic visualization for topic clusters and word importance.

Evaluation

LDA Coherence Score.

Topic quality and interpretability compared between LDA and BERT.

Insights Extraction

Analyzed which topics correspond to business, politics, sports, or lifestyle.

Created Category vs Topic Mapping for better understanding.

📊 Key Findings & Insights

Frequent words: said, people, year, time, government, new, life, story — show heavy coverage of politics, social issues, and events.

LDA revealed interpretable but broad topics.

BERTopic provided more refined and context-aware clusters.

Business applications:

Detect trending topics.

Monitor brand/media presence.

Support content categorization and recommendation.

🧩 Evaluation Metrics
Model	Metric	Score	Interpretation
LDA	Coherence Score	0.4765	Moderate topic clarity
BERTopic	Qualitative Topic Quality	High	Contextual and semantically rich topics
