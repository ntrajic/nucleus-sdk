# Nucleus SDK
Nucleus SDK with instructions and examples on how to use Nucleus APIs

## Overview
Nucleus SDK is a suite of high-performance text-analytics APIs developed by 
SumUp Analytics, Inc and subject to Terms of Services available at www.sumup.ai. 
Copyright SumUp Analytics Inc, 2019.

Those APIs enable end-users to perform the following tasks:
1. Analytics
* Topic modeling
* Topic transfer learning for propagation analysis of prevalence, sentiment and consensus
* Sentiment analysis at the Topic and Document level
* Consensus analysis at the Topic level
* Named Entity tagging (strict match)
* Summarization at the Topic and Document level
* Content recommendation at the Topic level
* Historical analysis of prevalence, sentiment and consensus at the Topic level
* Author connectivity analysis
* Topic exposure variation, as building block for time-series predictive modeling

2. Dataset Management
* Dataset creation (whole pre-processing pipeline)
* Metadata-based documents' selection
* Document rendering
* Dataset management


12 languages are currently supported by those APIs: English, Chinese (Simplified and Traditional), Japanese, 
Portuguese, Spanish, German, Russian, Italian, French, Arabic, Farsi.

The core task, topic modeling, has been benchmarked against Scikit-Learn, Gensim 
and AWS Comprehend topic models and delivers 100x speed-up with 2x accuracy on a 
wide range of dataset sizes, complexity and languages. More details can be found 
at www.sumup.ai in Nucleus Solution Brief (https://www.sumup.ai/SumUp%20Real-Time%20Text%20Analytics%20Solution%20Brief.pdf)

## Python SDK
Python SDK is available in [*python*](python) directory.

## Javascript SDK
Javascript SDK is available in [*javascript*](javascript) directory.

## Note to Jupyter Notebook users
We strongly recommend that rapid testing done in Jupyter Notebook be limited to 
1,000 documents being uploaded through our APIs from within the notebook.

Jupyter Notebooks suffer from file descriptor leakage and this will cause your 
tests on large datasets being uploaded from within these notebooks to error out 
with a message such as 'Too many open files'.

Once your rapid testing is done in notebook, best is to move to scripts to perform 
testing and exploration on much larger corpuses.
