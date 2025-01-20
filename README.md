# The Impact of Social Sentiment on Time Series Models for Bitcoin Price Prediction

## Overview
This repository contains the implementation of an MSc Data Science project investigating the role of sentiment analysis in improving Bitcoin price predictions using time series forecasting models (ARIMA and SARIMA). The project integrates technical indicators and sentiment data derived from cryptocurrency-related tweets to enhance predictive accuracy and robustness.

---

## Features
- **Time Series Models**: ARIMA and SARIMA with and without sentiment integration.
- **Sentiment Analysis**: Integration of cryptocurrency-related sentiment scores.
- **Technical Indicators**: SMA, EMA, RSI, MACD, and others for better feature engineering.
- **Comprehensive Evaluation**: Includes performance metrics (MAE, RMSE, MAPE) and visual comparisons.

---

## Project Structure
```plaintext
|-- The Impact of Social Sentiment on Time Series Models for Bitcoin Price Prediction.ipynb
|
|-- Dataset/
|   |-- bitcoin_data.csv                 # Raw Bitcoin data (2013–2021)
|   |-- cleaned_bitcoin_data.csv         # Preprocessed Bitcoin data
|   |-- enhanced_bitcoin_data.csv        # Bitcoin data with additional features
|   |-- cleaned_sentiment_data.csv       # Preprocessed sentiment data
|   |-- bitcoin_with_sentiment.csv       # Merged Bitcoin and sentiment data
|   |-- Cryptocurrency_Sentiment_Dataset.md  # Documentation for the sentiment dataset
|
|-- Results/
|   |-- ARIMA with Sentiment/            # ARIMA model results with sentiment
|   |-- ARIMA without Sentiment/         # ARIMA model results without sentiment
|   |-- SARIMA with Sentiment/           # SARIMA model results with sentiment
|   |-- SARIMA without Sentiment/        # SARIMA model results without sentiment
|   |-- Evaluation/                      # Evaluation metrics and summaries
|   |-- iterative model improvements/    # Iterative performance improvements
|   |-- bitcoin price overtime           # Price trend visualization
|   |-- bitcoin trading volume overtime  # Volume trend visualization
|   |-- technical indicator plot         # Technical indicators visualization
|
|-- requirements.txt                     # Python libraries and dependencies
|-- LICENSE                              # MIT License for the project
|-- README.md                            # Repository documentation
|-- .gitignore                           # Files to ignore in the repository

# Installation

## Clone the Repository
```bash
git clone https://github.com/Birkbeck/msc-projects-2023-4-Abuzer-Khanzade.git
cd msc-projects-2023-4-Abuzer-Khanzade



Install Dependencies
Create a virtual environment:

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate


Install the required libraries:

pip install -r requirements.txt


Run the Project
1. Open the Jupyter Notebook:

  jupyter notebook "The Impact of Social Sentiment on Time Series Models for Bitcoin Price   Prediction.ipynb"

2. Follow the cells for data preprocessing, model training, evaluation, and visualization.


Methodology

Data Collection:

Bitcoin price data: Historical data obtained from Yahoo Finance (2013–2021).
Sentiment data: Sourced from a Kaggle dataset containing over 824,000 cryptocurrency-  related tweets.


Feature Engineering:

Technical indicators like SMA, EMA, RSI, and MACD were added to capture market trends.
Sentiment features (positive, neutral, negative, compound scores) were merged with Bitcoin price data for integration into models.


Model Development:

ARIMA and SARIMA models were developed with and without sentiment integration to evaluate the effect of sentiment data.
Models were iteratively improved through hyperparameter tuning and validation.


Evaluation Metrics:

Models were evaluated using RMSE, MAE, and MAPE.
Visualizations included residual analysis, actual vs. predicted prices, Residual plots, and ACF plots.


Results

Integrating sentiment analysis into ARIMA and SARIMA models significantly improved Bitcoin price prediction, with ARIMA reducing RMSE by 59.88% and SARIMA achieving the best overall performance, reducing RMSE by 56.52% and improving MAE by 21.53% and MAPE by 18.85%. These results highlight the value of sentiment data in capturing market dynamics, though challenges like residual kurtosis and overfitting in ARIMA models remain due to Bitcoin’s high volatility.


Conclusion

This project demonstrates the significant impact of sentiment analysis on improving Bitcoin price predictions using time series models. By integrating sentiment features and technical indicators into ARIMA and SARIMA models, predictive accuracy was substantially enhanced, with sentiment-enhanced SARIMA models outperforming baseline approaches. The results highlight the importance of external factors, such as market sentiment, in capturing the complex dynamics of cryptocurrency markets. Despite challenges like Bitcoin’s high volatility and residual issues in ARIMA models, this study provides a foundation for future advancements, including the adoption of deep learning models and real-time prediction systems.


Tools and Libraries

Libraries: pandas, numpy, matplotlib, scikit-learn, statsmodels, yfinance, joblib
Tools: Jupyter Notebook, Yahoo Finance API, Kaggle datasets


License
This project is licensed under the MIT License.

Contact
Author: Mohammed Abuzer Khanzade
Email: mohammedabuzerk@gmail.com
Institution: Birkbeck, University of London
Supervisor: Dr. Jan Hidders
