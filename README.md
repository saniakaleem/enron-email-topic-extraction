#  Topic Modeling on Enron Emails using BERTopic

This project applies **BERTopic**, a modern NLP topic modeling approach, on the **Enron Email Dataset** to uncover latent themes and patterns in corporate communication. It uses state-of-the-art transformer embeddings and unsupervised learning to cluster emails into meaningful topics.

---

## Project Overview

- **Objective**: Automatically extract and visualize key topics from Enron’s public email dataset.
- **Technique**: BERTopic (using transformer embeddings + UMAP + HDBSCAN)
- **Dataset**: 10,000 emails from the Enron dataset (via HuggingFace)

---

## Methodology

1. **Text Embedding**: SentenceTransformers (`all-MiniLM-L6-v2`)
2. **Dimensionality Reduction**: UMAP
3. **Clustering**: HDBSCAN
4. **Topic Modeling**: BERTopic
5. **Visualization**: Plotly & Matplotlib via BERTopic’s built-in tools

---

##  Key Visualizations

- Inter-topic Distance Map (2D topic separation)
- Topic Hierarchy Tree (Parent → Subtopics)
- Top Topics Bar Chart
- Word Count & Email Length Distributions
- Scatter Plot: Email Length vs Word Count
- Sentiment Distribution & Correlation with Email Length

---

##  Key Insights

- Identified topics include **energy trading, legal disclaimers, internal coordination, media references, and more.**
- Emails showed strong **neutral to slightly positive sentiment**, with spikes in negative tones for legal or complaint-related messages.
- Topic hierarchy helped discover **broad themes and sub-categories** in business conversations.

---

##  Project Structure

##  Requirements

- Python 3.7+
- `bertopic`
- `sentence-transformers`
- `umap-learn`
- `hdbscan`
- `matplotlib`, `plotly`
- `pandas`, `numpy`

Install dependencies:

```bash
pip install bertopic sentence-transformers umap-learn hdbscan matplotlib plotly pandas numpy

This project demonstrates how unsupervised topic modeling using BERTopic can provide deep insights into large-scale corporate communication. Such analysis can be extended for sentiment tracking, compliance monitoring, and organizational behavior analysis.

Author
Sania Kaleem
MS Data Science
Muhammad Ali Jinnah University
FA24-MSDS-0009

