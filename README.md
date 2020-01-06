# Summarizing textual data

## Background

There are nearly 2 billion websites active on the internet and nearly 3 million emails being sent per second. This is huge amount of data in the form of audio, video, images, or text, and a lot of it is either redundant or does not contain much useful information. The most efficient way to get access to the most important parts of the data, without having to go through redundant and insignificant data, is to **summarize** the data in a way that it contains non-redundant and useful information only.

### Text Summarization

* A subdomain of Natural Language Processing (NLP).
* Deals with extracting summaries from huge chunks of texts.
* Techniques:
  * Simple NLP-based techniques
  * Deep learning-based techniques

---

## Goal

Summarizing textual data from Wikipedia Articles using automatic text summarization with simple NLP-based technique.

## Dataset

A Wikipedia Article: https://en.wikipedia.org/wiki/Natural_language_processing

## Dependencies

* Beautiful Soup 4
* Lxml
* Nltk

`pip install -r requirements.txt`

## Simple NLP-based Text Summarization Steps

* **Convert Paragraphs to Sentences**
  * Split the paragraph whenever a period is encountered.
* **Text Preprocessing**
  * Remove all the special characters, stop words and numbers from all the sentences.
* **Tokenizing the text to sentences and to words**
  * Get the list of all the sentences and the words that exist in the sentences.
* **Find the Word Frequencies**
  * Find the number of times each word occurs in the text.
* **Find the Weighted Word Frequencies**
  * Find the weighted frequency of each word by dividing its frequency by the frequency of the most occurring word.
* **Find the Sentence Scores**
  * Plug the weighted frequencies in place of the corresponding words in the original sentences and find their sum.
* **Sort the Sentences in Descending Order of the Sum**
  * The sentences with highest frequencies summarize the text.
