<h1 align="center">
  Text Summarization
</h1>

<h2 align="center">Persian Text Summarization, Both Abstractive and Extractive Methods</h2>

<div align="center">

[![Contact](https://img.shields.io/badge/contact-Parisa.rostaamii%40gmail.com-yellow.svg)](mailto:Parisa.rostaamii@gmail.com)

</div>

<h2 align="center">Text Summarization with Sequence-to-Sequence Model using TensorFlow (Abstractive)</h2>

Welcome to my Text Summarization project implemented in Python using TensorFlow. This project aims to create a sequence-to-sequence model for automatic text summarization. The model learns to generate concise and meaningful summaries for given article texts.

## Project Overview

Text summarization is a critical task in natural language processing, with applications ranging from news article summarization to document abstraction. This project demonstrates the end-to-end process of building a text summarization model using TensorFlow. The project is divided into several key steps:

1. **Data Preparation**
    - Utilized popular libraries such as NumPy and Pandas for efficient data handling and analysis.
    - Loaded and mounted Google Drive to access necessary dataset files.
    - Processed and cleaned the dataset, focusing on the 'summary' and 'article' columns.
    - Generated informative features like 'text_length' and 'summary_length' to analyze article and summary lengths.
    - Preprocessed the text data by removing punctuation and non-Persian characters.

2. **Data Tokenization**
    - Employed TensorFlow's powerful Tokenizer to tokenize the textual data.
    - Created tokenized sequences for both the article text and summary data.
    - Padded sequences to ensure uniform lengths for input and output sequences.

3. **Seq2Seq Model Setup**
    - Configured the sequence-to-sequence model using TensorFlow's Functional API.
    - Established the encoder component to embed and process the input article text.
    - Utilized a GRU layer to capture the final hidden state of the encoder.

4. **Decoder Model Setup**
    - Set up the decoder model to predict the summary based on the encoder's output.
    - Incorporated another GRU layer for decoding, implementing teacher forcing by feeding the actual summary output during training.

5. **Model Training**
    - Utilized the compiled model to train on the preprocessed data.
    - Trained the model to predict accurate summaries from input article text.
    - Applied the Nadam optimizer and sparse categorical cross-entropy loss for effective training.
    - Iterated the training process for a predefined number of epochs.

6. **Inference and Decoding**
    - Prepared the trained model for inference by configuring the decoder model.
    - Utilized the trained model to predict summaries for new, unseen article texts.
    - Decoded the predicted indices into words, reconstructing the summarized text.


## Conclusion

This project showcases the complete implementation of a sequence-to-sequence model for automatic text summarization using TensorFlow. By following the outlined steps, you can effectively build and train a model to generate concise and relevant summaries from given article texts. Whether you're interested in the mechanics of text processing, model training, or inference, this project provides a comprehensive guide to dive into the exciting world of text summarization.

Feel free to contribute, experiment, and adapt this project to your own use cases and datasets. Happy coding!


<h1 align="center">
 Persian Text Summarization (Extractive Method)
</h1>

<div align="center">

[![Contact](https://img.shields.io/badge/contact-Parisa.rostaamii%40gmail.com-yellow.svg)](mailto:Parisa.rostaamii@gmail.com)

</div>


Welcome to my Persian Text Summarization project implemented using an extractive method. This project focuses on generating concise summaries from given Persian text using a ranking algorithm.

## Project Overview

Text summarization is an essential task in natural language processing, and this project demonstrates an extractive approach to summarizing Persian text. The project is divided into the following key steps:

1. **Data Collection**
    - Utilized web scraping to collect Persian text data from various sources.
    - Used the `urllib` and `BeautifulSoup` libraries to extract text from web pages.

2. **Text Preprocessing**
    - Tokenized the collected text into sentences and words using NLTK.
    - Removed stopwords and irrelevant words from the tokenized text.

3. **Sentence Ranking**
    - Utilized word frequency to rank sentences based on their relevance.
    - Calculated the ranking score for each sentence and selected the top ones.

4. **Summarization Function**
    - Developed a function to generate summaries by selecting top-ranked sentences.
    - The function provides flexibility to choose the desired number of sentences in the summary.



## Conclusion

This project showcases an extractive approach to Persian text summarization using basic natural language processing techniques. By following the outlined steps, you can create simple yet effective summaries from given Persian text. Feel free to customize and expand upon this project to suit your specific use cases and datasets.



**Contact**: [Parisa.rostaamii@gmail.com](mailto:Parisa.rostaamii@gmail.com)


