# StockBot
AI-Based Form 4 Filing Interpretations for Improved Stock Market Information Availability to Public 
Pratyush Saxena, Winston Wang, Sumedh Anuganti, Prudhvi Kodali



Abstract 

This project provides raw information from SEC Form 4 filings, visual interpretations of this data, and uses an artificial intelligence model to interpret the filings for traders of all levels to better understand the motivation of certain insider transactions. Form 4 filings can offer unique insights into the potential changes in the stock of a company, yet they are often not utilized to their full potential because they are complex to understand and many novice traders aren’t even aware of their existence. Our goal is to create a Flask-based website that uses web scraping techniques to gather data from SEC’s EDGAR API and Yahoo Finance. Then, this data will be analyzed by a model to generate the most likely explanation as to why a certain transaction was made, allowing the public to make more informed decisions in their future trades.


How To Run Code:

To run the code from the GitHub repository 2025pKodali/SysLab, begin by cloning the repository using git clone https://github.com/2025pKodali/SysLab.git and navigating into the project directory. Make sure you have Python installed (preferably 3.9 or above) and install the required libraries with pip install -r requirements.txt. The project is organized around a network-driven analysis of insider trading activity. The sec_form_4_scraper.py script collects insider trading data by scraping SEC Form 4 filings for a given list of companies, organizing relevant trade details into a structured format such as JSON. This data is then analyzed using trade_analysis_bot.py, which applies a series of logic-based filters and to assess the potential significance of each trade. The app.py file is the core Flask web server that connects everything together, allowing users to input a stock ticker and visualize insider trading patterns via a browser interface. Running python app.py will launch the local web application, typically accessible at http://127.0.0.1:5000/, where you can interact with the data and explore recent trading behaviors.
