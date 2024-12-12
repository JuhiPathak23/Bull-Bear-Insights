# 📊 Bull and Bear Insights 📉

Welcome to the **Bull and Bear Insights** notebook! This project is designed to provide a detailed Exploratory Data Analysis (EDA) of stock price data for JPMorgan Chase and Goldman Sachs. Using various visualization techniques, we’ll uncover insights into stock performance, trading volumes, and market trends. 📈

## 🔍 What is EDA?

Exploratory Data Analysis (EDA) is a crucial step in data analysis that involves summarizing and visualizing data to uncover patterns, anomalies, & insights. Promoted by John Tukey, EDA helps in forming hypotheses and preparing data for further modeling. It includes checking assumptions, handling missing values, and transforming variables. 

### Types of EDA:

- **Univariate Non-graphical**
- **Multivariate Non-graphical**
- **Univariate Graphical**
- **Multivariate Graphical**

## 🛠️ Project Procedure

1. **Import Data**: Load the stock price datasets for JPMorgan Chase and Goldman Sachs.
2. **Preprocess Data**: Clean and prepare the data for analysis.
3. **Visualize Data**: Create visualizations to analyze trends and patterns.
4. **Inference**: Draw conclusions from the visualized data.

## 📈 Tools and Libraries

- **Matplotlib** & **Seaborn**: Traditional libraries for data visualization.
- **Plotly**: A modern library offering interactive and customizable plots.

## 📚 Key Analyses

- **Volume Analysis**: Examine trading volumes to understand market activity.
- **Price Trends**: Analyze opening and closing prices over time.
- **Daily Range**: Study daily fluctuations to gauge volatility.
- **Daily Returns**: Assess daily performance and market sentiment.
- **Comparative Analysis**: Compare key metrics between JPMorgan Chase and Goldman Sachs.

## 📊 Visualizations

### Volume Analysis

Visualizes trading volumes over time for each company.

### Price Trends

Compares opening and closing prices to observe market sentiment.

### Daily Range

Shows the daily trading range to evaluate stock volatility.

### Daily Returns

Displays daily returns to identify performance trends.

### Comparative Analysis

Compares mean values of stock prices and trading metrics between JPMorgan Chase and Goldman Sachs.

## 📥 Data Files

- `JPMorgan Chase.csv`: Historical stock prices for JPMorgan Chase.
- `The Goldman Sachs.csv`: Historical stock prices for Goldman Sachs.

## 📖 Example Usage to implement

```python
import pandas as pd
import plotly.express as px

# Load data
df1 = pd.read_csv("path/to/JPMorgan_Chase.csv")
df2 = pd.read_csv("path/to/Goldman_Sachs.csv")

# Example analysis
def volume_analysis(df, cmp):
    fig = px.line(df, x='Date', y='Volume', title=f'Volume of Stock Traded for {cmp}')
    fig.show()

volume_analysis(df1, 'JPMorgan Chase')
