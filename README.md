# Sentiment-Analysis-with-BERT

In this repository you will learn how to fine-tune BERT for sentiment analysis. Here we have done the required text preprocessing (special tokens, padding, and attention masks) and build a Sentiment Classifier using the amazing Transformers library by Hugging Face!

# What is BERT?
BERT (introduced in this paper) stands for Bidirectional Encoder Representations from Transformers. If you don't know what most of that means - you've come to the right place! Let's unpack the main ideas:

Bidirectional - to understand the text you're looking you'll have to look back (at the previous words) and forward (at the next words)
Transformers - The Attention Is All You Need paper presented the Transformer model. The Transformer reads entire sequences of tokens at once. In a sense, the model is non-directional, while LSTMs read sequentially (left-to-right or right-to-left). The attention mechanism allows for learning contextual relations between words (e.g. his in a sentence refers to Jim).
(Pre-trained) contextualized word embeddings - The ELMO paper introduced a way to encode words based on their meaning/context. Nails has multiple meanings - fingernails and metal nails.
BERT was trained by masking 15% of the tokens with the goal to guess them. An additional objective was to predict the next sentence. Let's look at examples of these tasks:

# Sentiment Classification with BERT and Hugging Face
There are a lot of helpers that make using BERT easy with the Transformers library. Depending on the task you might want to use https://huggingface.co/docs/transformers/model_doc/bert#bertforsequenceclassification  , https://huggingface.co/docs/transformers/model_doc/bert#bertforquestionanswering or something else.
