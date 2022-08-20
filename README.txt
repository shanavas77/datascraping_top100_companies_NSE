--Top 100 Companies in India by Market Capitalization - NSE (As of 19th Aug 2022)--

import pandas as pd

url = "https://www.moneycontrol.com/stocks/marketinfo/marketcap/nse/index.html"

df = pd.read_html(url)
df = df[0]
print(df)
df.to_csv('data5.csv', index=False)

--Top Gainers--

url = "https://www.moneycontrol.com/"

df = pd.read_html(url)
df = df[5]
print(df)
df.to_csv('top_gainers.csv', index=False)

--Top Losers--

url = "https://www.moneycontrol.com/"

df = pd.read_html(url)
df = df[7]
print(df)
df.to_csv('top_losers.csv', index=False)

--Most Active --

url = "https://www.moneycontrol.com/"

df = pd.read_html(url)
df = df[3]
print(df)
df.to_csv('most_active.csv', index=False)