# Final Round Submission for Data Got Talent 2024 by Team Pentagon
## Team Members:
- Nguyen Duy Duan
- Le Tuan Nguyen
- Phan My Kim
- Lam My Ngoc
- Tran Ngoc Bich Tran

## Project Introduction
### Company Context:
- Racing and Wagering Western Australia (RWWA) is the governing body for horse and greyhound racing in Western Australia, responsible for ensuring the vitality and sustainability of this industry in the region. As part of its mission, RWWA oversees off-course betting activities associated with racing. This is carried out through Western Australia TAB, a state-owned enterprise managing up to 300 retail betting locations and operating an online betting service branded as 'TABtouch'. WA TAB allows customers to place bets on various racing events, including horse and greyhound races, as well as a range of other sports, both domestic and international.
- TAB offers two types of betting: Fixed-odds and Pari-mutuel for both Racing and Sports categories.

## Environment Setup

To run the notebooks in this project, install the following Python libraries:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn pmdarima keras statsmodels
```

## Project Structure

```bash

|-- data
|   |-- CusData.csv
|   |-- ForecastTotalTurnover.csv
|   |-- rfm_2021.csv
|   |-- rfm_2022.csv
|   |-- rfm_c.csv
|   |-- TAB_Betting_Data.csv
|   |-- TransactionData.csv
|
|-- models
|   |-- best_arima_model.pkl
|   |-- best_gru_model.pkl
|   |-- best_lstm_model.pkl
|
|-- EDA.ipynb
|-- TimeSeries.ipynb
|-- RFM.ipynb
|-- RFMbyYear.ipynb
|-- Pentagon_Slide.pdf
|-- Pentagon_Report.pdf
|-- RWWA.pbix
```

### Description of Project Components:
- `data` folder: Contains the provided and generated data files during the analysis process.
  - `TAB_Betting_Data.csv`: Betting transaction data provided by the organizers. [Link](https://zrcy7-my.sharepoint.com/:x:/g/personal/ndoubled26_zrcy7_onmicrosoft_com/EfXNOsY7tOlEkaOUmszG7zUBLIKjzYkPg5WO6WgiplR0XA?e=FsTXPs)
  - `CustData.csv`: Demographic data of individual players after data exploration and cleaning. [Link](https://zrcy7-my.sharepoint.com/:x:/g/personal/ndoubled26_zrcy7_onmicrosoft_com/ESPsU6ArpRtEgsbUDKNV9JEBijfRpNtNVG_uhcA-enpiqw?e=D13sBB)
  - `TransactionData.csv`: Transaction data after removing demographic factors of players.
  - `rfm_c.csv`, `rfm_2021.csv`, `rfm_2022.csv`: Stores R, F, M metrics for each player across the entire dataset and separately for each year.
  - `ForecastTotalTurnover.csv`: Predicted revenue for Q1 2023 of the business.

- `models` folder: Contains files of models built to predict WA TAB's future revenue.
  - `best_arima_model.pkl`: The most optimal ARIMA model selected by the team.
  - `best_gru_model.pkl`: The most optimal RNN GRU model identified after multiple tests.
  - `best_lstm_model.pkl`: The most optimal RNN LSTM model identified after multiple tests.

- `EDA.ipynb`: Executes the process of exploring and cleaning the raw data.

- `TimeSeries.ipynb`: Converts raw data into time-series data by day, builds and evaluates models, and forecasts revenue.

- `RFM.ipynb`, `RFMbyYear.ipynb`: Calculates R, F, M metrics, stores them in `rfm_c.csv`, and calculates them separately by year to evaluate customer trends, storing results in `rfm_2021.csv` and `rfm_2022.csv`.

- `Pentagon_Slide.pdf` and `Pentagon_Report.pdf`, `RWWA.pbix`: The team's report on predictions and business analysis.

## Visualization Analysis
[Business Performance Report of WA TAB](https://app.powerbi.com/view?r=eyJrIjoiNGZiMDAwZTUtZjU3NC00YjM1LThmYjktMjBhZTg0NTljYmY0IiwidCI6IjY4NDJkZjllLTQwMmUtNDg1OC04OTNiLTY5YzIwNGUxOTgyMSIsImMiOjEwfQ%3D%3D&pageName=ReportSection&fbclid=IwAR3u9Ox69hszMHjlqyLpCYPYoOFMd0S-UV8hVDfp_lF802CL3RvBvzVc2f4_aem_ASIYly-TgWpv9NVkATJKZDRNGJ7RRZh5u-nsxj5ov1Oy6h_i9U8A5ETUQt3UtCGI3P3stsS0TotffyNo3ug5JVwM)

## Related Documents

- Data for the Final Round of Data Got Talent 2024
- Python Libraries: 
[NumPy](https://numpy.org/),
[Pandas](https://pandas.pydata.org/),
[Scikit-learn](https://scikit-learn.org/stable/),
[Matplotlib](https://matplotlib.org/),
[Seaborn](https://seaborn.pydata.org/),
[Pmdarima](https://pypi.org/project/pmdarima/),
[Keras](https://keras.io/guides/),
[Statsmodels](https://www.statsmodels.org/stable/index.html)
- [RFM Model](https://www.putler.com/rfm-analysis/)
- Deep Learning Techniques: [RNN GRU](https://www.geeksforgeeks.org/gated-recurrent-unit-networks/),
[RNN LSTM](https://www.geeksforgeeks.org/long-short-term-memory-lstm-rnn-in-tensorflow/)
- Machine Learning Techniques: [ARIMA](https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/)

### Authors: `Team Pentagon` from the University of Economics and Law, VNU-HCM
