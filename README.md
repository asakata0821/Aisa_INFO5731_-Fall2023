# Japanese-American Incarceration Oral History (JAIOH) Analysis

## Overview

We are at a crucial juncture in history, where the stories of our ancestors, preserved in various formats, are increasingly accessible. Historically, archiving was a manual process managed by archivists, which proved to be time-consuming. However, with the rise of digital technology, there is an urgent need for automation and digitalization [1].

This project addresses this challenge by exploring solutions and tools for effective digital archiving. Our focus is on applying **Natural Language Processing (NLP)** and **Machine Learning (ML)** models to the history of Japanese-American Incarceration. We will analyze four online collections: the Densho repository, the Japanese American Service Committee (JASC), the Japanese American Museum of San Jose (JAMSJ), and Discover Nikkei. Our research aims to answer the following questions:

1. **What are the narrators' descriptions**, including their nationality, race, age, and birthplace?
2. **Are there common characteristics or points** among each incarceration camp?
3. **What activities or significant events** are associated with individuals mentioned by multiple narrators?

Our objective is to extract valuable insights and contextual information from these methods.


## Overview

This project involves the analysis of historical narratives from four collections: Densho repository, JASJ, JAMSJ, and Discover Nikkei. The goal is to extract insights and categorize text data through various methodologies including descriptive analysis, entity extraction, text classification, sentiment analysis, and topic modeling.

## Table of Contents

1. [Data Collection and Processing](#data-collection-and-processing)
2. [Methodologies](#methodologies)
   - [Descriptive Analysis](#descriptive-analysis)
   - [Entity Extraction](#entity-extraction)
   - [Annotation Scheme](#annotation-scheme)
   - [Text Classification](#text-classification)
   - [Sentiment Analysis](#sentiment-analysis)
   - [Word Cloud Generation](#word-cloud-generation)
   - [Topic Modeling](#topic-modeling)
3. [Data Analysis](#data-analysis)

## Data Collection and Processing

### Overview

Our project analyzes a set of 1,153 transcripts collected from diverse sources. The data collection involves web scraping, data structuring, and handling various formats and inconsistencies.

### Data Collection

**Setup: Importing Libraries and Tools**
- Libraries Used: BeautifulSoup, requests, urllib.error, re, os, csv, zipfile
- Tools: Python, Google Colab

**Process**
1. **Web Scraping**:
   - Parsed HTML/XML documents using BeautifulSoup.
   - Mimicked browser requests to avoid blocks.
   - Collected data such as narrator names, descriptions, and transcripts.

2. **Data Structuring**:
   - Organized data into dictionaries and CSV files.
   - Compressed CSV files into ZIP format for each collection.

**Challenges and Solutions**
- Adapted scraping techniques to handle varied formats.
- Managed special characters and speaker changes.

## Methodologies

### Descriptive Analysis

**Setup: Importing Libraries**
- Libraries Used: re, datetime, pandas, NumPy, SpaCy

**Process**
1. **Data Extraction**:
   - Extracted narrator information using regular expressions and SpaCy.

2. **Categorization**:
   - Classified narrators based on their birth year relative to 1942.

**Challenges and Solutions**
- Developed custom functions to handle data format variations.

### Entity Extraction

**Setup: Importing Libraries**
- Libraries Used: SpaCy, pandas

**Process**
1. **Named Entity Recognition (NER)**:
   - Utilized SpaCy’s pre-trained model for entity extraction.

**Challenges and Solutions**
- Chose SpaCy for its comprehensive NER tags.

### Annotation Scheme

**Setup: Defining Categories**
- Categories: Pre-war background, Life After Removal, Military Services, Redress Movement, Legal Challenges, Government’s Decision, Returning of Ethnic Japanese

**Process**
1. **Category Definition**:
   - Created and validated an annotation scheme for the narratives.

**Challenges and Solutions**
- Applied the scheme to validate its relevance with a subset of narrators.

### Text Classification

**Setup: Importing Libraries**
- Libraries Used: NumPy, Pandas, Torch, sklearn, Transformers

**Process**
1. **Model Training**:
   - Trained a BERT model for text classification.
   - Managed GPU limitations by adjusting data size.

2. **Performance Evaluation**:
   - Evaluated model performance using accuracy, precision, recall, and F1 score.

**Challenges and Solutions**
- Improved accuracy through iterative adjustments.

### Sentiment Analysis

**Setup: Importing Libraries**
- Libraries Used: re, nltk, transformers, torch.nn, scipy, pandas, numpy

**Process**
1. **Model Choice**:
   - Used RoBERTa for sentiment analysis of lengthy transcripts.

**Challenges and Solutions**
- Managed extensive transcript lengths with RoBERTa.

### Word Cloud Generation

**Setup: Preprocessing**
- Libraries Used: Not specified

**Process**
1. **Text Preprocessing**:
   - Cleaned and tokenized text data for visualization.

2. **Visualization**:
   - Generated word clouds to represent frequently used words.

**Challenges and Solutions**
- Refined dataset to remove additional stopwords.

### Topic Modeling

**Setup: Importing Libraries**
- Libraries Used: BERTopic, pandas, nltk

**Process**
1. **Text Cleaning**:
   - Cleaned and tokenized text for topic modeling.

2. **Topic Identification**:
   - Identified and visualized topics using BERTopic.

**Challenges and Solutions**
- Controlled the number of sub-topics for clarity.

## Data Analysis

**Overview**

The analysis includes descriptive statistics, entity extraction comparisons, and performance evaluations for text classification and sentiment analysis.

### Descriptive Analysis

**Process**
- Analyzed patterns in 40 narratives related to birthplaces and camp locations.

### Entity Extraction

**Process**
- Compared SpaCy and BERT for entity extraction, choosing SpaCy for its range of tags.

### Annotation Scheme

**Process**
- Validated the annotation scheme with a subset of 10 narrators.

### Text Classification

**Process**
- Compared GPT-3.5, LLaMA, and BERT, selecting BERT for its performance.

### Sentiment Analysis

**Process**
- Chose RoBERTa for its efficiency in handling lengthy transcripts.

### Topic Modeling

**Process**
- Limited the number of sub-topics for better clarity in topic modeling.

---

For further details and code implementations, please refer to the respective Jupyter Notebooks and scripts in the 'JAIOH_Code' repository.
