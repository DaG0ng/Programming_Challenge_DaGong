# Programming_Challenge_DaGong

Da Gong's Programming Challenge.

## Virtual Environment

The whole project is based on Anaconda Jupyter Notebook.

## Usage

python jupyter notebook
run all cells of [Jupyter Notebook](notebook/Programming_Challenge.ipynb)


## Summary of Results

| Article Name  | Sentiment Score |
| ------------- | ------------- |
| Floods hit South Africa’s KwaZulu-Natal province again  | -0.9898 |
| Mozambique: Cyclone Gombe death toll rises to 53| -0.996|
| Mozambique announces new prime minister after cabinet reshuffle|-0.9038|
| Analysis: Can African gas replace Russian supplies to Europe?|-0.9908|
| Dozens dead from Tropical Storm Ana in southern Africa|-0.9945|
| Southern Africa bloc SADC extends Mozambique mission|0.6893|
| Climate change and famine | -0.9843|
| In Mozambique, Kagame says Rwandan troops’ work not over|-0.9069|
| Rwanda, Mozambique forces recapture port city from rebels|-0.7817|
| Rwanda deploys 1,000 soldiers to Mozambique’s Cabo Delgado|-0.9964  |

![line chart](plotly_result.jpg?raw=true)

## Conclusion

Most articles of Mozambique is quite negative since its most about disasters or civil wars. However, I believe this result can be further
verified through more sentiment analysis on more articles.

## Format of Json File

The format is simple. The key is generated articles id from 0 and the value is the corresponding text of each articles web pages.

## Pre-processing of Data

1. Use only the content of articles excluding titles and sub-titles.
2. Get rid of site-footer and referenced twitter since they are not part of the articles.

## Choose of Sentiment Analysis Tool

I used en-sentiment pre-trained model from Flair Library as the tool for computing sentiment analysis.

Below is the introduction from Flair Library Page:
>Flair is:

>A powerful NLP library. Flair allows you to apply our state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), part-of-speech tagging (PoS), special support for biomedical data, sense disambiguation and classification, with support for a rapidly growing number of languages.

>A text embedding library. Flair has simple interfaces that allow you to use and combine different word and document embeddings, including our proposed Flair embeddings, BERT embeddings and ELMo embeddings.

>A PyTorch NLP framework. Our framework builds directly on PyTorch, making it easy to train your own models and experiment with new approaches using Flair embeddings and classes.


## Total Operation Time

Total Operation Time: 8.395648002624512s
Might need more time first time loading pre-trained library model

## License
[MIT](https://choosealicense.com/licenses/mit/)