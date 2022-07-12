# pygnewslib
Python Library for getting/fetching news from google news.

## Installation:
```nano
pip install pygnewslib
```
## For Upgradation(pythmath):
```nano
pip install --upgrade pygnewslib
```

## Usage:
```py
from pygnewslib import GoogleNews

google_news = GoogleNews()
json_resp = google_news.news('Pakistan')
results = []
for ar in json_resp:
    results.append(ar["title"])

for i in range(len(results)):
    # printing all trending news
    print(i + 1, results[i])
```

