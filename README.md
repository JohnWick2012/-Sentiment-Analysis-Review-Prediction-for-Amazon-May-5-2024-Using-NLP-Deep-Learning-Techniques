# Amazon Reviews Sentiment Analysis and Prediction
# Dated: 5TH May 2024 Reviews

## Project Overview
This project aims to analyze sentiments and predict review sentiments for Amazon using Natural Language Processing (NLP) techniques and Deep Learning. The project involves preprocessing text data, performing exploratory data analysis, sentiment analysis, topic modeling, and building an LSTM model for sentiment prediction.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Preprocessing Text Data](#preprocessing-text-data)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Sentiment Analysis](#sentiment-analysis)
- [Topic Modeling](#topic-modeling)
- [LSTM Model for Sentiment Prediction](#lstm-model-for-sentiment-prediction)
- [Evaluation and Visualization](#evaluation-and-visualization)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset
The dataset used in this project is a collection of Amazon reviews obtained from Kaggle. It contains reviews along with ratings, timestamps, and other metadata.

## Installation
To run this project, you need to have Python installed. You can install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```

## Project Structure
```
amazon-reviews-sentiment-analysis/
│
├── data/
│   └── amazon_reviews.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── eda.py
│   ├── sentiment_analysis.py
│   ├── topic_modeling.py
│   └── lstm_model.py
│
├── requirements.txt
├── README.md
└── main.py
```

## Preprocessing Text Data
Text preprocessing involves cleaning the text data by:
- Converting to lowercase
- Removing punctuation and numbers
- Removing stopwords

## Exploratory Data Analysis (EDA)
EDA is performed to understand the distribution of scores and the temporal aspects of the reviews. Visualizations are created using Matplotlib and seaborn.

## Sentiment Analysis
Sentiment analysis is conducted using TextBlob to categorize reviews into positive, negative, or neutral sentiments. A sentiment label is assigned based on the polarity score.

## Topic Modeling
Topic modeling is performed on negative reviews using Gensim's LDA model to extract key topics that highlight common themes of dissatisfaction among users.

## LSTM Model for Sentiment Prediction
An LSTM model is built using Keras to predict the sentiment of reviews. The model architecture includes an embedding layer, LSTM layer, and a dense output layer with softmax activation for multiclass classification.

## Evaluation and Visualization
The model performance is evaluated using metrics such as accuracy, confusion matrix, classification report, ROC curves, and AUC scores. Training history is visualized to ensure proper model validation.

## Results
The LSTM model achieved high accuracy in predicting sentiments of Netflix reviews. The insights from sentiment analysis and topic modeling provide valuable information about user sentiments and common issues faced by Netflix users.

## Contributing
Contributions are welcome! If you have any suggestions or improvements, please submit a pull request or open an issue.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
