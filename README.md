# Analyzing Historical Stock/Revenue Data & Building a Dashboard (IBM Data Analyst Capstone)

[![Coursera Course](https://img.shields.io/badge/Coursera-IBM%20Data%20Analyst-0056D2?logo=coursera)](https://www.coursera.org/learn/python-project-for-data-science)
[![Python 3.12](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-FA0F00?logo=jupyter)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Project Overview

This project is the final assignment for the **"Python Project for Data Science"** course, part of the **IBM Data Analyst Professional Certificate** on Coursera. The goal was to take on the role of a Junior Data Analyst at a financial analytics firm. I was tasked with collecting, processing, and visualizing stock and revenue data for two major companies, **Tesla (TSLA)** and **GameStop (GME)**, to present meaningful insights to potential investors.

The project demonstrates a complete data analysis workflow, from data extraction (using APIs and web scraping) to generating interactive-style visualizations.

## 🎯 Project Objectives

- **Collect and Prepare Data:** Use Python libraries like `yfinance` to fetch historical stock data and `BeautifulSoup` to scrape revenue data from the web.
- **Analyze Trends:** Organize and manipulate the extracted data to identify patterns in stock prices and revenue over time.
- **Build a Dashboard:** Create a dual-axis time-series plot to visually compare a company's stock price against its revenue, highlighting key trends.

## 🔧 Tools & Libraries Used

The project was developed in a **Jupyter Notebook** environment, using the following technologies:

- **Data Collection:**
  - `yfinance`: To download historical market data from Yahoo Finance.
  - `requests` & `BeautifulSoup (bs4)`: For web scraping HTML tables containing revenue data.
- **Data Manipulation & Analysis:**
  - `pandas`: For structuring, cleaning, and processing data into DataFrames.
- **Data Visualization:**
  - `matplotlib.pyplot`: To create the final static comparison graphs.

## 🚀 Key Steps Performed

The project notebook is structured around six main tasks, which were completed successfully:

1.  **Tesla Stock Data Extraction:** Used the `yfinance` library to extract Tesla's historical stock data (max period) into a DataFrame (`tesla_data`), reset the index, and display the first five rows.
2.  **Tesla Revenue Data Scraping:** Sent an HTTP request to a specified URL, parsed the HTML using `BeautifulSoup`, extracted the Tesla revenue table into a DataFrame (`tesla_revenue`), cleaned the data (removing "$" and commas), and displayed the last five rows.
3.  **GameStop Stock Data Extraction:** Repeated the `yfinance` process for GameStop (`GME`), creating the `gme_data` DataFrame, resetting the index, and displaying the first five rows.
4.  **GameStop Revenue Data Scraping:** Repeated the web scraping process for GameStop's revenue from a different URL, creating and cleaning the `gme_revenue` DataFrame, and displaying the last five rows.
5.  **Tesla Visualization:** Utilized the provided `make_graph` function to plot Tesla's historical share price and revenue on a single timeline.
6.  **GameStop Visualization:** Utilized the `make_graph` function to plot GameStop's historical share price and revenue.

## 📊 Key Results & Visualizations

The analysis revealed distinct trends for each company:

### Tesla (TSLA)
*   **Analysis Period:** Stock Data (Up to June 14, 2021) & Revenue Data (Up to April 30, 2021).
*   **Trend:** Between 2018 and 2021, **both Tesla's stock price and revenue showed strong, correlated growth**. The share price skyrocketed alongside a steady increase in reported quarterly revenue.

![Tesla Stock and Revenue Graph](images/tesla_graph.png)
*(Note: Ensure this image path is correct or remove the line if you don't have a separate `/images` folder)*

### GameStop (GME)
*   **Analysis Period:** Stock Data (Up to June 14, 2021) & Revenue Data (Up to April 30, 2021).
*   **Trend:** The graph shows a **dramatic surge in GameStop's stock price around 2021**, which was not accompanied by a similar increase in revenue. This decoupling is a classic indicator of a short-squeeze event (as seen in early 2021) rather than growth driven by fundamental business performance.

![GameStop Stock and Revenue Graph](images/gamestop_graph.png)
*(Note: Ensure this image path is correct or remove the line if you don't have a separate `/images` folder)*

## 🏁 How to Run the Notebook

1.  **Clone the repository** to your local machine or open it directly in Google Colab.
    ```bash
    git clone <your-repo-url>
