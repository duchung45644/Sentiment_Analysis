# Sentiment Analysis on Reviews

This project aims to classify reviews into positive and negative sentiments using various machine learning models. The process includes data loading, text preprocessing, visualization, and model training.

## Table of Contents
- [Sentiment Analysis on Reviews](#sentiment-analysis-on-reviews)
  - [Table of Contents](#table-of-contents)
  - [Steps Involved](#steps-involved)
    - [1. Data Loading](#1-data-loading)
    - [2. Text Preprocessing](#2-text-preprocessing)
    - [3. Data Visualization](#3-data-visualization)
    - [4. Model Training and Evaluation](#4-model-training-and-evaluation)
      - [Models Used:](#models-used)

## Steps Involved

### 1. Data Loading
- The dataset is loaded from a CSV file.
- Duplicates are removed to ensure unique entries for training the model.

### 2. Text Preprocessing
- **Contractions Expansion:** Converts shortened forms like "don't" into "do not."
- **HTML Tag Removal:** Uses `BeautifulSoup` to remove any HTML tags present in the reviews.
- **Emoji and Punctuation Removal:** Removes unnecessary symbols, emoticons, and punctuation marks.
- **Stopwords Removal:** Eliminates common stopwords (e.g., 'the', 'and') using NLTK's English stopwords list.
- **Lemmatization:** Reduces words to their base forms (e.g., "running" becomes "run") for better generalization.

### 3. Data Visualization
- **Pie Chart:** Visualizes the distribution of positive and negative reviews.
- **Word Length Analysis:** Compares the distribution of word lengths in positive and negative reviews.
- **Kernel Distribution Plot:** Shows the distribution of word lengths for each sentiment category.

### 4. Model Training and Evaluation
- **Train-Test Split:** The dataset is split into training (80%) and testing (20%) sets.
- **TF-IDF Vectorization:** The reviews are transformed into numerical features using TF-IDF for model input.

#### Models Used:
- **Decision Tree Classifier:** Achieved an accuracy of ~71.4%.
- **Random Forest Classifier:** Achieved an accuracy of ~84.9%.
