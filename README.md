# Homework-2-NLP-

## Q6 Bigram Language Model (MLE)

### Description

The model is trained on a small corpus and computes the probability of sentences based on bigram probabilities.

---

## Training Corpus
The model is trained using the following sentences:
- `<s> I love NLP </s>`
- `<s> I love deep learning </s>`
- `<s> deep learning is fun </s>`

---

## Functionality
The program performs the following steps:
1. Reads and tokenizes the training corpus
2. Computes unigram counts
3. Computes bigram counts
4. Estimates bigram probabilities using MLE
5. Computes the probability of any given sentence
6. Tests the model on two sentences
7. Prints which sentence the model prefers and why

---

## Bigram Probability Formula
Bigram probabilities are computed using:
P(w2 | w1) = count(w1, w2) / count(w1)

The probability of a sentence is the product of all its bigram probabilities.

---

## How to Run
1. Ensure Python 3 is installed
2. Save the program as `bigram_model.py`
3. Run the script using:
   python bigram_model.py

---

## Output
The program prints:
- Unigram counts
- Bigram counts
- Probability of each test sentence
- Which sentence is preferred by the model

---

## Result Explanation
The model usually prefers `<s> I love NLP </s>` because:
- It is shorter
- All its bigrams appear in the training data
- Longer sentences result in smaller probabilities due to multiplication

---

## Limitations
- No smoothing is applied
- Unseen bigrams receive probability 0
- Demonstrates the zero-probability problem in language modeling

---


