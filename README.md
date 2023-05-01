# ETF Analyzer

The ETF Analyzer Web Application is a financial tool that allows users to analyze the performance of a hypothetical fintech ETF. The application provides insights into the daily and cumulative returns of individual assets within the ETF as well as the overall portfolio. By using advanced SQL queries, Python, and the Voilà library, users can visualize and explore the performance data in an interactive and user-friendly manner.

The main problem this project addresses is the need for a comprehensive tool to analyze the performance of ETFs, particularly in the fintech sector. This web application enables users to assess the historical returns of different assets within the ETF, identify top-performing stocks, and evaluate the overall portfolio's performance. It empowers investors, financial professionals, and enthusiasts to make informed decisions based on data-driven analysis.

---

## Technologies

To use the ETF Analyzer Web Application, you will Python 3.7 or higher and the following dependencies:

* [pandas](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint.

* [voila](https://github.com/voila-dashboards/voila) - A library that turns individual Jupyter notebooks into interactive web pages

* [SQLAlchemy](https://pypi.org/project/SQLAlchemy/) - allows you to access and manage SQL databases using Pythonic domain language.

* [hvplot](https://hvplot.holoviz.org/) - API for data exploration and visualization.

* [pathlib](https://docs.python.org/3/library/pathlib.html) - Provised method to interact with the filesystem.


---

## Installation Guide

To install and run the ETF Analyzer Web Application, follow these steps:

    1. Clone the project repository from GitHub
```python
    git clone https://github.com/your-username/etf-analyzer.git
```
    2. Navigate to the project directory
```python
    cd etf-analyzer
```
    3. Create a virtual environment (optional but recommended)
```python
    python3 -m venv venv
```
    4. Activate the virtual environment
```python
    Windows:
    venv\Scripts\activate
    macOS/Linux:
    source venv/bin/activate
```
    5. Install the required dependencies
```python
    pip install -r requirements.txt
```
    6. Run the web application
```python
    voila app.ipynb
```
    7. Open your web browser and access the application at http://localhost:8866/


---

## Usage

### Analyzing a Single Asset in the ETF

1. Select the desired asset from the sidebar menu.
2. Review the first and last five rows of the asset's data to identify the available date range.
3. Explore the interactive visualization of the asset's daily returns.
4. Analyze the cumulative returns over time using the provided line plot.

### Optimizing Data Access with Advanced SQL Queries

1. Access the closing prices for a specific asset above a certain threshold.
2. Review the resulting DataFrame to examine the selected dates and closing prices.
3. Find the top 10 daily returns for a specific asset.
4. Review the resulting DataFrame to identify the dates and corresponding daily returns.

### Analyzing the ETF Portfolio

1. Review the joined DataFrame containing all four assets in the ETF.
2. Create a DataFrame that averages the daily returns for all four assets.
3. Calculate the annualized return for the ETF portfolio.
4. Calculate the cumulative returns of the ETF portfolio over time.
5. Visualize the cumulative return values using the provided interactive line plot. 

---

Upon launching the web page via Voila the following should appear:

![Screeen Recording](Images/web_page.mov)

---

## Contributors

Brought to you by Rosalinda Olvera Fernandez and instructor Firas Obeid.

---

## License

This project is licensed under the MIT License.




