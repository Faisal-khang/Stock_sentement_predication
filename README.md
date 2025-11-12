# 📈 Stock Sentiment Analysis

## ⭐ Description

Stock Sentiment Analysis evaluates the emotional tone in text sources (news, social media, financial reports) related to a stock to determine whether sentiment is **positive, negative, or neutral**.

Public opinions heavily influence investor behavior and market price movement. Positive outlook may lead to rising prices, while negative sentiment may trigger selling and price drops.

---

## ✅ Why Sentiment Matters

* Market is influenced by psychology
* Positive sentiment → buy → price increases
* Negative sentiment → sell → price decreases

| Example Text                     | Sentiment |
| -------------------------------- | --------- |
| "Company reports record profits" | Positive  |
| "Company under investigation"    | Negative  |

---

## 📂 Data Sources

* News headlines
* Twitter / X posts
* Reddit comments
* Financial blogs
* Company reports

---

## 🔧 How It Works

1. Collect data
2. Clean and preprocess text
3. Convert text to numerical form (TF-IDF/Word2Vec/BERT)
4. Apply sentiment models

   * Rule-based (VADER)
   * ML / DL models
5. Output sentiment score (pos/neg/neutral)

---

## ✅ Example Code (VADER)

```python
from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer

analyzer = SentimentIntensityAnalyzer()

text = "Stock price of Tesla is expected to rise after strong earnings!"
score = analyzer.polarity_scores(text)

print(score)
```

Example output:

```
{'neg': 0.02, 'neu': 0.30, 'pos': 0.68, 'compound': 0.90}
```

---

## 📊 Applications

* Stock trend forecasting
* Portfolio management
* Market monitoring
* Risk analysis

---

## ✅ In Stock Prediction Models

SentimentScore can be used as a feature:

```
Close, Volume, MA_5, Lag_1, SentimentScore
```

---

## 📈 Insights

Sentiment combined with technical indicators helps improve prediction performance and interpret market psychology.
