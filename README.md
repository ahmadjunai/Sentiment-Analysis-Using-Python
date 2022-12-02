# Sentiment-Analysis-Using-Python

from textblob import Textblob
from newspaper import Article

url = 'https://www.bbc.com/news/uk-england-london-52963555'
article = Article(url)

article.download()
article.parse()
article.nlp()

text = article.summary
print(text)
blob = Textblob(text)
sentiment + blob.sentiment.polarity_# -1 to 1
print (sentiment)
