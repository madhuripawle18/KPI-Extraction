# KPI-Extraction

## Problem Statement

Extraction of Investor’s KPI’s and a brief description of KPI usage from a document, given it has investment related KPI in it.
For this we decided to divide the project into 2 main parts:
1) Classify the documents into “Investment related” and “Not Investment related”
2) Extract the KPI’s from the classified documents

## Data Available

We have 704 business articles(papers) in pdf format; which include KPI’s related to customers, investment and employees.

## Data Cleaning

The given data come in PDF format which could not immediately be edited and analyzed.
- We converted the pdfs to text files using PDFMiner.
- We removed the stopwords, converted the text into lower case and stemmed every word in this
text for better training of the classifier using nltk.
- Porter Stemmer was used for stemming.
- Out of 704 files we successfully converted 698 files into text files. (There was error with
encodings of the remaining files due to non-english characters)
