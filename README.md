<!--
Name of your teams' final project
-->
# Applications-of-Stock-Market-Predictor


<!--
List all of the members who developed the project and
link to each members respective GitHub profile
-->
Developed by: 
- [Elayne Blancas](https://github.com/eb3770) - `New York University`
- [Gregory Perez](https://github.com/gap85) - `Cornell University` 
- [Jonathan Zamudio](https://github.com/jz034) - `University of Arkansas` 

## Description
<!--
Give a short description on what your project accomplishes and what tools is uses. In addition, you can drop screenshots directly into your README file to add them to your README. Take these from your presentations.
-->
Our Stock Market Predictor dictates whether an individual stock will either over-perform
or under-perform, calculate the long and short gains of the portfolios stocks, and obtain
the portfolios stock average return and Sharpe Ratio. We used yfinance API to obtain
a decade of daily historical stock data from Yahoo Finance for the top 30 Standard and
Poor (S&P) 500 companies. Our data consisted of non-negative stock values with no upper
bound for weekdays and non holidays. Our Stock Market Predictor uses Random Forest
as a baseline for our LSTM model. To prevent over-fitting, we dropped 20 percent of our
data, a common practice used in machine learning. Additionally, in an effort to obtain a
higher accurate score, we use a decade of the stockˆas history to predict its future trends.
In making this model pipeline, we would use the 3 prior years as our training data. This
pipeline would take the years of data and go over it in a series of sequences, each sequence
containing 240 days. This sequence of data would then give us the value of the stock. Our
model has 60% to 70% training accuracy. Our predictor would advice for a long investment
on either Comcast Company or Adobe, and a short investment on either Protector Gamble
Company or Salesforce. Although this type of predictor is difficult to generalize, our future
work would be to include sentimental analysis, web scraping, and Beautiful soup for real
time data to mitigate for its volatility. Our model does not account for anything external
and should, therefore, not be used as a main investment tool.

## Usage instructions
<!--
Give details on how to install fork and install your project. You can get all of the python dependencies for your project by typing `pip3 freeze requirements.txt` on the system that runs your project. Add the generated `requirements.txt` to this repo.
-->
Run notebook in Google Colab.