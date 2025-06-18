# Sentiment Analysis - SATUSEHAT Mobile App Reviews

A comprehensive sentiment analysis project that analyzes user reviews from Google Play Store for the SATUSEHAT Mobile application using multiple machine learning models including LSTM, SVM, and RandomForest.

## About SATUSEHAT Mobile

SATUSEHAT Mobile adalah aplikasi kesehatan masyarakat resmi dari Kementerian Kesehatan RI yang menyediakan layanan kesehatan terintegrasi dan rekam medis elektronik. SATUSEHAT Mobile merupakan transformasi serta pengembangan dari aplikasi PeduliLindungi yang akan menjadi gaya hidup baru masyarakat agar #TetapSEHAT dan #MakinSEHAT.

## Project Overview

This project performs sentiment analysis on user reviews of the SATUSEHAT Mobile application from Google Play Store to understand user satisfaction and identify areas for improvement. The analysis employs three different machine learning approaches to compare their effectiveness in sentiment classification.

## Features

- **Data Collection**: Web scraping of Google Play Store reviews for SATUSEHAT Mobile
- **Multiple ML Models**: Implementation of LSTM, SVM, and RandomForest algorithms
- **Comprehensive Analysis**: Detailed sentiment classification and model comparison
- **Model Testing**: Evaluation and testing of different approaches

## Project Structure

```
sentiment-analysis-SATUSEHAT-Mobile/
├── datasets/
│   └── satusehat_reviews.csv          # Raw review data from Google Play Store
├── notebooks/
│   ├── Analisis_Sentimen_Aplikasi_SAT... # Main sentiment analysis notebook
│   ├── Datasets_Scraping.ipynb       # Data collection and scraping
│   └── Testing_Model.ipynb           # Model evaluation and testing
├── .gitignore                        # Git ignore file
└── requirements.txt                  # Python dependencies
```

## Models Implemented

### 1. LSTM (Long Short-Term Memory)
- Deep learning approach for sequential text processing
- Captures long-term dependencies in review text
- Suitable for understanding context and sentiment flow

### 2. SVM (Support Vector Machine)
- Traditional machine learning classifier
- Effective for text classification tasks
- Good performance with high-dimensional data

### 3. RandomForest
- Ensemble learning method
- Robust against overfitting
- Provides feature importance insights

## Dataset

The dataset consists of user reviews scraped from Google Play Store for the SATUSEHAT Mobile application, containing:
- Review text
- User ratings
- Review timestamps
- Other relevant metadata

## Getting Started

### Prerequisites

Install the required dependencies:

```bash
pip install -r requirements.txt
```

### Usage

1. **Data Collection**
   ```bash
   jupyter notebook notebooks/Datasets_Scraping.ipynb
   ```
   Run this notebook to collect fresh review data from Google Play Store.

2. **Sentiment Analysis**
   ```bash
   jupyter notebook notebooks/Analisis_Sentimen_Aplikasi_SAT...
   ```
   Execute the main analysis notebook to:
   - Preprocess the review data
   - Train LSTM, SVM, and RandomForest models
   - Compare model performances
   - Generate sentiment insights

3. **Model Testing**
   ```bash
   jupyter notebook notebooks/Testing_Model.ipynb
   ```
   Use this notebook for model evaluation and performance testing.

## Key Analysis Components

### Data Preprocessing
- Text cleaning and normalization
- Tokenization and vectorization
- Handling Indonesian language text
- Feature extraction for different models

### Model Training
- LSTM neural network architecture
- SVM with optimal hyperparameters
- RandomForest ensemble configuration
- Cross-validation and performance optimization

### Evaluation Metrics
- Accuracy scores
- Precision, Recall, and F1-score
- Confusion matrices
- Model comparison analysis

## Results and Insights

The project provides:
- Comparative analysis of three different ML approaches
- Sentiment distribution of SATUSEHAT Mobile reviews
- Model performance benchmarks
- Actionable insights for app improvement

## Technologies Used

- **Python**: Primary programming language
- **Jupyter Notebook**: Development environment
- **scikit-learn**: Traditional ML algorithms (SVM, RandomForest)
- **TensorFlow/Keras**: Deep learning (LSTM)
- **pandas**: Data manipulation
- **numpy**: Numerical computations
- **matplotlib/seaborn**: Data visualization
- **BeautifulSoup/Selenium**: Web scraping

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-analysis`)
3. Commit your changes (`git commit -am 'Add new analysis feature'`)
4. Push to the branch (`git push origin feature/new-analysis`)
5. Create a Pull Request

## Acknowledgments

- Indonesian Ministry of Health for developing SATUSEHAT Mobile
- Google Play Store for providing review data
- Open-source machine learning community for tools and libraries
