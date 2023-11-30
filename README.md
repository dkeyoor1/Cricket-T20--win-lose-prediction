# Predicting Cricket T20 Match Outcomes Using Logistic Regression
Overview

This project aims to develop a machine learning model to predict the outcome of cricket T20 matches based on real-time match data. The model utilizes logistic regression to analyze factors such as the number of runs needed, balls left, wickets remaining, and current run rate to determine the probability of each team winning or losing.

Data Preparation

The project utilizes historical cricket match data from Kaggle's IPL dataset. The data is preprocessed to extract relevant features and prepare it for model training. This involves:

Calculating the number of balls per over

Converting missing dismissal information to numerical values

Calculating wickets remaining based on dismissals

Calculating the current run rate (CRR) and required run rate (RRR)

Encoding categorical variables (batting team, bowling team, and city)

Model Building

A logistic regression model is trained on the preprocessed data. The model learns the relationship between the extracted features and the match outcome (win or loss).

Real-time Prediction

To predict the outcome of a live match, real-time data is scraped from cricbuzz. This data includes the current score, balls left, runs needed, and teams playing. The extracted information is then preprocessed and fed into the trained logistic regression model to predict the probability of each team winning or losing.

## Project Structure

The project consists of four main steps:

1. **Data Preparation:** Preprocess historical cricket match data to extract relevant features and prepare it for model training.

2. **Model Building:** Train a logistic regression model on the preprocessed data.

3. **Real-time Data Scraping:** Scrape real-time match data from cricbuzz.

4. **Prediction and Evaluation:** Preprocess the scraped data, feed it into the trained model, and evaluate the prediction accuracy.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Requests
- Beautiful Soup
- sklearn
- os

## Project Setup

1. Clone the project repository using Git.

2. Install the required dependencies using pip:

```bash
pip install pandas numpy matplotlib requests beautifulsoup4 sklearn os
