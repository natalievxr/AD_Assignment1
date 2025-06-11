## AD_Assignment1
# Text Analysis with NLTK and spaCy
This repository contains code for analyzing text collections using NLTK and spaCy natural language processing libraries. The project includes sentence splitting, word tokenization, frequency analysis, stemming comparison, POS tagging across multiple languages, and Named Entity Recognition evaluation.

## Overview
The analysis is divided into two main parts:

## Part 1: Text Analysis
* Sentence splitting and word tokenization on a collection of text art stories
* Word frequency statistics and visualization of the 25 most common words
* Stemming comparison using Porter and Lancaster stemmers
* POS tagging analysis of three translations of "Tom Sawyer" in different languages
## Part 2: Named Entity Recognition
* NER using spaCy on the same text collection
* Manual annotation of sample sentences
* Performance evaluation (Precision, Recall, F1 Score)
### Key Findings
### Word Frequency Analysis
* Common stop words dominated the frequency counts in the raw text.
* After stemming, similar patterns emerged but with normalized word forms.
* Porter stemmer produced more natural stems, while Lancaster was more aggressive.

### Stemming Comparison
* Lancaster stemmer reduced words more aggressively than Porter.
* Porter maintained better readability of stems.
* Both stemmers improved word frequency counts by combining variant forms.

### POS Tag Distribution
* Comparable distribution patterns across languages
* Notable differences in noun, pronoun, and determiner usage between languages
* These differences reflect inherent linguistic structures of each language

### Named Entity Recognition
* Evaluation metrics show moderate performance of spaCy's NER
* Common errors included missed entities and incorrect entity type classifications
* Performance varied by entity type (PERSON, ORG, LOC, etc.)

### Technologies Used
* Python 3
* NLTK
* spaCy (including language models for English, German, and French)
* Matplotlib and Seaborn for visualization
* Pandas for data manipulation
  
### Usage

The Jupyter notebook contains all code and analysis steps. To run:

Install required libraries: pip install nltk spacy pandas matplotlib seaborn

Download required spaCy models:
python -m spacy download en_core_web_sm

python -m spacy download de_core_news_sm

python -m spacy download fr_core_news_sm

Run the notebook with the data files in the relative paths as specified
