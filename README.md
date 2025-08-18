# Rakshith-s_portfolio

# [ Project 1: 911 Call Analysis Model ](https://rakshith2712.github.io/rakshith-s_portfolio/911_call_analysis_model)
This is a my first project while learning data analysis during my Bachelor's Degree

* Data was downloaded from kaggle (https://www.kaggle.com/mchirico/montcoalert)
* **Data Import & Exploration:** Learned to load large real-world datasets using Pandas, inspect data structure with .info() and .head(), and explore high-frequency categories using .value_counts().
* **Feature Engineering:** Created new columns such as Reason, Hour, Month, Day of Week, and Date by parsing and transforming datetime fields with pd.to_datetime() and .apply() functions.
* **Data Visualization Skills:** Used Matplotlib and Seaborn to create bar plots, line plots, and heatmaps, including countplot, lmplot, and clustermap to identify patterns and trends in emergency calls.
* **Categorical Mapping:** Applied mapping dictionaries to make categorical data (e.g., day numbers → day names) more readable for analysis.
* **Trend & Pattern Analysis:** Analyzed call distribution by Reason (Traffic, EMS, Fire), observed seasonal and daily patterns, and identified peak hours and days for each emergency type.
* **Correlation Insights:** Used heatmaps and clustermaps to visualize correlations between time-based variables (Day of Week × Hour, Day of Week × Month) for deeper temporal pattern recognition.
* **Practical Data Analysis Workflow:** Followed an end-to-end process — from loading raw data to preprocessing, feature creation, and building visual insights — replicating a typical real-world data analytics pipeline.

# [ Project 2: Finance Analysis Model ](https://rakshith2712.github.io/rakshith-s_portfolio/finance__analysis_model)
This is my second project while learning data analysis during my second internship at Exposys Data Labs

* Data was downloaded from Wikipedia (https://en.wikipedia.org/wiki/Financial_crisis_of_2007%E2%80%9308)
* **Data Acquisition with APIs:** Learned to use pandas_datareader to get past stock data for different banks from online sources (Stooq) and automatically collect it for chosen date ranges using datetime.
* **Multi-Index DataFrames:** Put all banks’ stock data into one MultiIndex Pandas DataFrame to keep it organized and make comparisons easier.
* **Return Calculations:** Used the pct_change() method to find daily returns, which helped understand stock ups and downs and how prices change over time.
* **Exploratory Data Analysis (EDA):** Used .max(), .idxmin(), .idxmax(), and .std() to find the highest prices, best/worst trading days, and the most changeable stocks.
* **Risk & Distribution Analysis:** Showed return patterns for different banks in certain periods (like 2008 crisis, 2015) using Seaborn histograms and pairplot to check connections.
* **Correlation Insights:** Made heatmaps and clustermaps to see how bank stock prices move together and to find similar movement groups.
* **Time-Series Visualization:** Created rolling averages, line charts, and candlestick charts to see trends, moving averages, and stock behavior over time.
* **Technical Analysis Tools:** Used Cufflinks for interactive charts, making candlesticks, simple moving averages (SMA), and Bollinger Bands for deeper financial checks.
* **Crisis Impact Study:** Saw how big financial events (like the 2008 crisis) impacted many banks at the same time, linking stock data to real events in the economy.

# [ Project: Heart Rate Signal Analysis & Prediction](https://rakshith2712.github.io/rakshith-s_portfolio/heart__rate_signal_analysis_and_prediction)
This is a Research project for Concordia Unviersity, completed during my Masters degree for a course Pervasive Computing for Healthcare Applications - COEN 691

**Data Collection & Preprocessing**
* Imported heart rate datasets (Actigraph.csv, April74.csv) and merged signals (HR and HR1).
* Dropped irrelevant rows, aligned time indices, and resampled data to 1-second intervals with interpolation.
* Generated sliding window averages (30s) to prepare supervised learning features.

**Signal Processing & Feature Engineering**
* Visualized heart rate distributions using KDE plots.
* Applied Fast Fourier Transform (FFT) to analyze frequency components.
* Implemented a Butterworth bandpass filter (1–4 Hz) to extract physiological HR signals.
* Used peak detection to identify beats from filtered signals.

**Machine Learning Models**

* Built supervised dataset (X = HR30s, y = HR130s).
* Implemented and compared multiple regression models:
* Linear Regression
* Support Vector Regression (SVR)
* K-Nearest Neighbors (KNN) with hyperparameter tuning (GridSearchCV)
* Decision Tree Regression (optimal depth search)
* Random Forest Regression

**Deep Learning Model**
* Designed and trained an LSTM neural network for sequential heart rate prediction.
* Normalized input data and reshaped into time-series format for LSTM.
* Compared actual vs. predicted values using line plots and scatter plots.

**Model Evaluation**
* Evaluated all models using MAE, MSE, and RMSE.
* Visualized model performance using bar plots (log scale for MSE).
* Categorized predicted HR values into “Good” (60–100 bpm) and “Bad” heart rate ranges.
