# AI Pracrical Exam: 
# By Sanskar 
# N-Gram Language Model
Python implementation of an N-gram language model with Laplace smoothing and sentence generation. 

Some NLTK functions are used (`nltk.ngrams`, `nltk.FreqDist`), but most everything is implemented by hand.

Note: the `LanguageModel` class expects to be given data which is already tokenized by sentences. If using the included `load_data` function, the `train.txt` and `test.txt` files should already be processed such that: 
1. punctuation is removed
2. each sentence is on its own line  

See the `data/` directory for examples.

---

Example output for a trigram model trained on `data/train.txt` and tested against `data/test.txt`:
```
Loading 3-gram model...
Vocabulary size: 23505
Generating sentences...
...
<s> <s> the company said it has agreed to sell its shares in a statement </s> (0.03163)
<s> <s> he said the company also announced measures to boost its domestic economy and could be a long term debt </s> (0.01418)
<s> <s> this is a major trade bill that would be the first quarter of 1987 </s> (0.02182)
...
Model perplexity: 51.555
```
The numbers in parentheses beside the generated sentences are the cumulative probabilities of those sentences occurring.

---
