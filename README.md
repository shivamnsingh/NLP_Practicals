# NLP Practicals

A set of eleven short Jupyter notebooks that walk through the core building blocks of Natural Language Processing, from raw-text cleanup to a simple text classifier. Each notebook is self-contained and focuses on one technique.

## Contents

| # | Notebook | Topic | Main library |
|---|----------|-------|--------------|
| P1 | `P1 - Text Preprocessing.ipynb` | Cleaning and preprocessing text data loaded from a Kaggle dataset (student admission records) | pandas, kagglehub |
| P2 | `P2- Sentence Segmentation & Tokenization.ipynb` | Splitting text into sentences and words | NLTK |
| P3 | `P3 - LemmaStem.ipynb` | Stemming vs. lemmatization | NLTK (Porter stemmer, WordNet lemmatizer) |
| P4 | `P4 - POS Tagging.ipynb` | Part-of-speech tagging | NLTK |
| P5 | `P5 - GRA via POS.ipynb` | Analyzing the grammatical makeup of a user-entered sentence by tagging it and counting each POS tag | NLTK |
| P6 | `P6 - N-grams.ipynb` | Generating unigrams, bigrams and trigrams | NLTK |
| P7 | `P7 - POS using NN.ipynb` | POS tagging with a neural pipeline | spaCy (`en_core_web_sm`) |
| P8 | `P8 - NER.ipynb` | Named entity recognition | spaCy (`en_core_web_sm`) |
| P9 | `P9 - EnglishTextNLP.ipynb` | Spelling checking for English text | pyspellchecker |
| P10 | `P10 - TD-IDF.ipynb` | TF-IDF feature extraction | scikit-learn |
| P11 | `P11 - TextClassNLP.ipynb` | Text classification with a bag-of-words model and Multinomial Naive Bayes | scikit-learn |

## Getting started

1. Clone the repository:
   ```bash
   git clone https://github.com/shivamnsingh/NLP_Practicals.git
   cd NLP_Practicals
   ```
2. Install the dependencies:
   ```bash
   pip install jupyter pandas nltk spacy scikit-learn pyspellchecker kagglehub
   python -m spacy download en_core_web_sm
   ```
3. Launch Jupyter and open any notebook:
   ```bash
   jupyter notebook
   ```

The NLTK notebooks download the resources they need (such as `punkt` and `wordnet`) on first run. P1 downloads its dataset through `kagglehub`, which may require Kaggle credentials.

## Suggested order

The notebooks are numbered in the order they build on each other: preprocessing and tokenization (P1 to P3), then tagging and grammar (P4 to P8), then spelling and feature extraction (P9, P10), and finally classification (P11).
