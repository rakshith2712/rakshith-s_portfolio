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