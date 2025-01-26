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
|--Code/
|   |--The Impact of Social Sentiment on Time Series Models for Bitcoin Price Prediction.ipynb
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
```
---
# Installation

## Clone the Repository
```bash
git clone https://github.com/Birkbeck/msc-projects-2023-4-Abuzer-Khanzade.git
cd msc-projects-2023-4-Abuzer-Khanzade
```
# Install Dependencies
## Create a virtual environment:
```
python -m venv venv
```
```
source venv/bin/activate           # On Windows: venv\Scripts\activate

```

## Install the required libraries:
```
pip install -r requirements.txt
```

# Run the Project
1. Open the Jupyter Notebook:
```
jupyter notebook "The Impact of Social Sentiment on Time Series Models for Bitcoin Price Prediction.ipynb"
```

2. Follow the cells for data preprocessing, model training, evaluation, and visualization.

---

# Methodology

## Data Collection:

- Bitcoin price data: Historical data obtained from Yahoo Finance (2013–2021).
- Sentiment data: Sourced from a Kaggle dataset containing over 824,000 cryptocurrency-  related tweets.


## Feature Engineering:

- Technical indicators like SMA, EMA, RSI, and MACD were added to capture market trends.
- Sentiment features (positive, neutral, negative, compound scores) were merged with Bitcoin price data for integration into models.


## Model Development:

- ARIMA and SARIMA models were developed with and without sentiment integration to evaluate the effect of sentiment data.
- Models were iteratively improved through hyperparameter tuning and validation.


## Evaluation Metrics:

- Models were evaluated using RMSE, MAE, and MAPE.
- Visualizations included residual analysis, actual vs. predicted prices, Residual plots, and ACF plots.

---

## Results

The integration of sentiment analysis into ARIMA and SARIMA models greatly improved the accuracy of Bitcoin price predictions. ARIMA models with sentiment data reduced RMSE by 59.88%, while SARIMA models with sentiment achieved the best overall performance, lowering RMSE by 56.52%, MAE by 21.53%, and MAPE by 18.85%. These findings demonstrate the value of incorporating sentiment data to better capture market trends. However, challenges like overfitting in ARIMA models and Bitcoin's high volatility still pose limitations.

---

## Conclusion

This project highlights the significant role of sentiment analysis in enhancing Bitcoin price prediction using time series models. Combining sentiment features and technical indicators with ARIMA and SARIMA models led to much better prediction accuracy, with sentiment-enhanced SARIMA models outperforming other approaches. The results emphasize the importance of considering market sentiment in understanding the complex nature of cryptocurrency markets. Despite some challenges, this study lays the groundwork for further advancements, such as exploring deep learning models and developing real-time prediction pipelines.

---

## Tools and Libraries

- Libraries: pandas, numpy, matplotlib, scikit-learn, statsmodels, yfinance, joblib
- Tools: Jupyter Notebook, Yahoo Finance API, Kaggle datasets

---

## License
This project is licensed under the MIT License.

---

## Contact
- Author: Mohammed Abuzer Khanzade
- Email: mohammedabuzerk@gmail.com
- Institution: Birkbeck, University of London
- Supervisor: Dr. Jan Hidders

