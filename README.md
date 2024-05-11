# smoothingNGram
Apply Bayesian statistics through DLM to smooth a 4-gram frequency series. Video demonstrating the code and the smoothing theory is [here](https://youtu.be/GxO03B-0xFg).

# Goal
To find the trend of some phrases in English.

# Data
 - The source is Google Books Ngram Viewer. However, the data can also be obtained using package `ngramr` in R. To get the raw data, use `smoothing=0`.
 - Time range: 1980-2019
 - The ngram data is based on a certain corpus. In this project, we see the ngram data using English corpus, American English corpus, British English corpus, and fiction corpus.

# Method
After getting the raw data, we fit the Dynamic Linear Model (aka filtering in state space model terms). Then, we smooth the filtered sequence using propositions for smoothing.
