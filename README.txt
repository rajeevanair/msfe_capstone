Sentiment Analysis based stock market recommendations

Technology : Python
Version : 3.7.6

Packages needed : 
import time
import requests
from bs4 import BeautifulSoup
import os
import pandas as pd
import progressbar

from pandas_datareader import data as pdr
import yfinance as yf
yf.pdr_override()

import nltk
import twython
from nltk.corpus import stopwords
from nltk.tokenize import word_tokenize
from nltk.sentiment.vader import SentimentIntensityAnalyzer

nltk.download('stopwords')
nltk.download('punkt')
nltk.download('vader_lexicon')

First the package should be installed in the machine. Use this code snippet to do that : 
pip install <package_name>
