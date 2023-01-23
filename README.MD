# :newspaper_roll: :newspaper: Extracting Stock Sentiment from News Headlines

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org)  [![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/) 
[![](https://img.shields.io/badge/SciPy-654FF0?style=for-the-badge&logo=SciPy&logoColor=white)](https://www.scipy.org) 
[![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org)
[![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)


## Introduction 
In this notebook, we will use __sentiment analysis__ on __financial news headlines from FINVIZ.com__ to gain investing insights. By understanding the emotions behind the headlines, we can predict the market's sentiment towards a stock and make educated guesses on its performance, allowing for informed trading decisions. The use of data science in processing this vast amount of information allows for quick analysis,
unlike the traditional method of spreading news via radio, newspapers and word of mouth which used to take days.

## Importing the HTML Files
To import the HTML files for Facebook and Tesla, we will use the os library to locate the files on our local system and read them into memory. This will allow us to access the data in the files and perform sentiment analysis on the headlines to generate investing insight and make educated guesses about stock performance.

## Vader Sentiment Analysis
Vader Sentiment Analysis is a pre-trained model that uses natural language processing (NLP) to determine the sentiment of a given text. It is specifically designed to analyze social media text, which typically includes a lot of slang, emoticons, and other non-standard forms of language. The model uses a combination of lexical heuristics, such as word-level sentiment scores, and grammatical heuristics, such as the use of negation and punctuation, to determine the overall sentiment of the text. 
The output of the model is a sentiment score on a scale of -1 to 1, where -1 represents a negative sentiment, 0 represents a neutral sentiment, and 1 represents a positive sentiment.

## Extracting the Headlines
Let's extract the news headlines from the HTML files we imported into memory. We can see that the relevant information is located within the text inside the <td> and <a> tags of each table row (<tr>). We will use this information to create a structured data set for further analysis.
More details can be found [here](https://github.com/iqrabismii/Stock-Sentiment-from-News-Headlines/blob/main/ExtractStockSentimentFromNewsHeadlines.ipynb)
  
## Implementing the Vader Function 
  
Using VADER "as is" for sentiment analysis on financial news headlines may not be sufficient for producing profitable results.
  A more effective approach would involve creating a specialized lexicon specific to financial news and potentially developing a custom model.
  I used the vader sentiment analysis method to classify the headlines in the financial news dataset as negative, neutral, or positive. 
  I then integrated the results of this analysis into the original dataset for further visualization and analysis.
  
 ## Insights 
 It was observed that Tesla had more negative score as compared to FB. Also, Stock for FB was observed for one particular and most of the headlines were neutral. 
  
