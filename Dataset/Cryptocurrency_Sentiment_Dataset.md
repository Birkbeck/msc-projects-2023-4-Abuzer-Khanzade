# Cryptocurrency Tweets Sentiment Dataset

This project utilizes a raw sentiment dataset, sourced from Kaggle, which includes tweets related to cryptocurrencies along with sentiment analysis scores. The dataset is a cornerstone for analyzing the impact of public sentiment on Bitcoin price prediction models. Due to its large size (~633 MB), the dataset is not directly included in this repository but is accessible through the links provided below.

## Download Links

1. **Primary Source**: [Cryptocurrency Tweets with Sentiment Analysis Dataset on Kaggle](https://www.kaggle.com/datasets/fabioturazzi/cryptocurrency-tweets-with-sentiment-analysis?resource=download)  
2. **Backup Source**: [Download from Google Drive](https://drive.google.com/drive/folders/1Hu54CwF5PJvy6bwDSVpGmLrVEkas3I3I?usp=sharing)

## Instructions for Usage

To utilize this dataset in the project, please follow these steps:

1. **Choose a source**: Access the dataset from either the Kaggle link (primary source) or the Google Drive link (backup source).
2. **Download the dataset**:
   - For Kaggle: Log in to your Kaggle account (if required) and download the dataset file.
   - For Google Drive: Open the provided folder link, locate the dataset file, and download it directly.
3. **Extract the files**: If the dataset is compressed (e.g., `.zip`), extract the contents to access the raw data file(s).
4. **Organize the files**: Place the extracted dataset in the `Dataset` folder within this repository for consistency.
5. **Match file paths**: Ensure that the file paths in the project notebook/code correctly point to the location of the downloaded dataset.

## Dataset Details

- **Source**: Kaggle and Google Drive (Backup)
- **Description**: This dataset comprises tweets related to cryptocurrencies, enriched with sentiment analysis scores. These scores represent the public's sentiment towards cryptocurrencies and are categorized as negative, neutral, or positive, along with a compound score summarizing the overall sentiment.
- **File Size**: Approximately 633 MB
- **Columns**:
  - `neg`: Negative sentiment score
  - `neu`: Neutral sentiment score
  - `pos`: Positive sentiment score
  - `compound`: Overall sentiment score
  - Additional metadata about tweets, such as date, time, and content.

## Use in the Project

The dataset plays a vital role in this project as it provides the sentiment features used to enhance the predictive capabilities of time series models like ARIMA and SARIMA. While all preprocessing steps are implemented in the project code, having access to the raw data ensures reproducibility and allows for future modifications or analyses.

## Note on Backup

In case the Kaggle dataset becomes unavailable or if their access policies change, the dataset is also hosted on Google Drive to ensure its availability for future use. The backup provides an additional layer of reliability for maintaining the project's functionality over time.
