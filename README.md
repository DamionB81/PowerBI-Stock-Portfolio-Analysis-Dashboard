# Power BI Stock Portfolio Dashboard

This repository showcases an interactive **Power BI dashboard** built to analyze stock portfolio performance, trading volume, and sector allocation.  
The dashboard brings together **time series, scatter plots, geographic mapping, KPIs, and portfolio weighting visuals** to deliver actionable insights for investors.

---

##  Features

- **Custom KPIs with DAX**: Built measures to calculate Average Daily Volume, YTD performance, Portfolio Value, Weighting, and other key metrics.


- **Stock Prices Over Time**: Line and area charts showing total close price trends by ticker symbol.  
- **Volatility & Price Change**: Scatter plot of average price range vs. average price change by company and year.  
- **Trading Volume**: Line charts and KPIs for daily, min, max, and YTD average trading volumes.  
- **Geographic Insights**: Map visuals by U.S. zip code and exchange symbol.  
- **Portfolio Analysis**: Table and ribbon charts showing portfolio weighting, close price, and value by ticker.  
- **Benchmarking**: Comparisons across NYSE vs NASDAQ performance.

---

## Repository Structure

- `Stock_Portfolio_Dashboard.pbix` → Main Power BI file  
- `images/` → Dashboard screenshots (for quick preview)  
- `README.md` → Project documentation  

---

## 📸 Dashboard Preview

### Stock Prices by Ticker
![Area Chart](/Image/Area%20Chart.png)

### Price Range vs. Price Change
![Scatter Chart](/Image/Scatter%20Plot.png)

### Geographic Distribution of Exchanges
![Map Visual](/Image/Exchange%20by%20Zip%20Code.png)

### Trading Volume
![Line Chart](/Image/Line%20Chart.png)  
![Card Visuals](/Image/Card%20Visuals.png)

### Security & Portfolio Analysis
![Security Page](/Image/Security%20Page.png)  
![Ribbon Chart](/Image/Ribbon%20Chart.png)  
![Line Chart View](/Image/Portfolio%20Value%20line%20chart.png)  
![Table Visual](/Image/Table%20Visual.png)

### Exchange Analysis
![Exchange Page](/Image/Exchange%20Page.png)

---


## 🗄️ Data Model

The dashboard is built using a **star schema** to optimize reporting and analysis.  

### DAX Measures

The model includes custom measures created with DAX to calculate portfolio and trading KPIs:

- **Average Daily Volume**
- **Average Price Change**
- **Average Price Range**
- **Count of Securities**
- **Current Close Price**
- **Current Portfolio Value**
- **Max Daily Volume / Min Daily Volume**
- **Portfolio Value**
- **Total Close Price / Total Portfolio Value / Total Volume / Total Weighting**
- **YTD Avg Daily Volume / YTD Max Daily Volume / YTD Min Daily Volume**



![Data Model](/Image/Data%20Model.png)

### Tables

- **factActivity**  
  Stores trading metrics such as close price, portfolio value, price change, price range, and trading volume.  

- **dimDate**  
  Provides calendar attributes (day, month, month name, year) for time-series analysis.  

- **dimSecurity**  
  Contains company details, ticker symbol, industry, weighting, and location data (address, city, state, country, zip code).  

- **dimExchange**  
  Contains exchange-level details including exchange symbol, type, currency, location, and website.  


##  How to Use

1. Download the `.pbix` file from this repository.  
2. Open in **Power BI Desktop**  
3. Use the provided visuals interactively, or connect your own dataset for live updates.

---

## 📈 Tools & Tech

- **Power BI Desktop** (data modeling & visualization)  
- **Stock Market Data** (Yahoo Finance / CSV inputs)  
- **GitHub** (version control & portfolio showcase)
-  **DAX Measures** for KPI calculations (e.g., Avg Daily Volume, Portfolio Value, YTD metrics)


---

💡 *For the full interactive experience, download the `.pbix` file and open it in Power BI Desktop.*
