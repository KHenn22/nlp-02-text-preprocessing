# Web Mining and Applied NLP Project Report

Web Mining and Applied NLP | Project 02 | Custom Report

## Overview

This project introduces text preprocessing
as a foundation for natural language processing.

The objective is to demonstrate how raw text
can be tokenized, normalized, cleaned,
and prepared for systematic analysis.

The project compares the results of
different preprocessing operations
to show how cleaning decisions affect
the representation of text.

## Tools and Methods

The project uses:

- Python for text processing and analysis.
- Local text files for input data.
- Regular expressions for punctuation removal.
- Tokenization for separating text into words.
- Lowercasing for text normalization.
- Stopword filtering for reducing common vocabulary.
- Polars for calculating token frequencies.
- Matplotlib for visualizing preprocessing results.
- Logging for execution records.
- Ruff, ty, and pytest for code verification.
- Zensical and GitHub Pages for published documentation.

The example script reads text records,
combines them into a corpus,
and applies a sequence of preprocessing operations.

The analysis compares raw and cleaned token counts
and identifies frequently occurring words.

## Verification

A successful execution displays:

    Pipeline executed successfully!

The script records execution details in a project log.

The output includes token counts,
frequency distributions,
and preprocessing comparison charts.

Automated tests provide additional verification
of the project's expected behavior.

## Interpretation

Text preprocessing transforms raw language
into a representation suitable for analysis.

Lowercasing, punctuation removal,
and stopword filtering change the resulting
token distribution.

These operations can reduce unwanted noise,
but they may also remove meaningful information.

Understanding these tradeoffs is important
when preparing text for traditional NLP
and modern language-model applications.

## Custom Project

Author: Kevin Hennelly

## Problem

Does stemming change which words appear most frequent, and how much
does it reduce the vocabulary?

## Data

- Source: `data/text_data.txt`, the example data from Denise Case's
  nlp-02-text-preprocessing project (MIT License).
- The original data was kept so results could be compared directly
  to the example's baseline.

## Techniques Applied

- Same pipeline as the example: tokenization, lowercasing,
  punctuation removal, stop word and short token filtering.
- Added: stemming with NLTK's PorterStemmer after stop word removal.

## Methods and Settings

- Stemmer: PorterStemmer (NLTK). Chosen because it is simple and
  widely used.
- Frequency table and bar chart use stemmed tokens instead of
  cleaned tokens.

## Custom Modifications

- Prediction: If I add stemming, total tokens stay the same but
  unique tokens decrease, because stemming renames words rather
  than removing them.
- Result: Total cleaned tokens stayed at 46; unique tokens dropped
  from 38 to 37. Two forms of "remove" merged into "remov."
- Unexpected: Many stems are not real words (e.g., "languag," "mani").


## Documentation Index

- **Home** - this landing page
- [**Project Instructions**](project-instructions.md)
- [**Glossary**](glossary.md)

## Project Links

- [GitHub Repository](https://github.com/denisecase/nlp-02-text-preprocessing)
- [Example Script](https://github.com/denisecase/nlp-02-text-preprocessing/blob/main/src/nlp/text_preprocessing.py)
- [Example Notebook](https://github.com/denisecase/nlp-02-text-preprocessing/blob/main/notebooks/text_preprocessing.ipynb)
- [Example Data](https://github.com/denisecase/nlp-02-text-preprocessing/blob/main/data/text_data.txt)
- [Custom Script](https://github.com/KHenn22/nlp-02-text-preprocessing/blob/main/src/nlp/text_preprocessing_hennelly.py)
- [Custom Notebook](https://github.com/KHenn22/nlp-02-text-preprocessing/blob/main/notebooks/text_preprocessing_hennelly.ipynb)


## Project Resources

- [Project Instructions](project-instructions.md)
- [Professional Python Guide](https://denisecase.github.io/pro-analytics-02/)
- [Professional Python Project Explainer](https://pup-pack.github.io/professional-python-project-explainer/)
