# Sentiment-Analysis
This project utilizes two powerful models, VADER and RoBERTa, for sentiment analysis on textual data. We use VADER from NLTK and the Hugging Face transformers with RoBERTa. The combination of these models aims to provide a robust and accurate analysis of sentiment in various contexts. It also includes a transformers pipeline as an easy way to run sentiment predictions on textual input.

### VADER Model:
VADER model is a pre-built sentiment analysis tool designed specifically for text data, such as tweets, reviews or other short messages. In this project ,we use NLTK, a powerful Python library for natural language processing, which includes VADER for sentiment analysis. VADER assigns a polarity score to each word in a given sentence. The sum of these scores provides an overall sentiment polarity for the entire sentence. VADER doesn't understand the context of the whole sentence, but assigns a score to the sentiment of each word based on its adjacent words alone.

### RoBERTa Model:
RoBERTa model, is a state-of-the-art NLP model that builds upon the transformer architecture introduced by BERT. Sentiment analysis can be acheived by integrating the Hugging Face transformers library using the RoBERTa model. The tokenised representation of the text is passed to this model, which after being fine-tuned further provides a polarity score for the text. RoBERTa understands the context of the sentence, and hence not only assigns the polarity score to the words independently, but assigns it based on its context. 

The predictions/scores from these two models are compared allowing us to see the differences between each observation and what each feature looks like. We use Seaborn's pairplot to acheive this visualisation.

We also experiment with a transformers pipeline. This will provide a quick and easy way to run sentiment predictions on input texts.
