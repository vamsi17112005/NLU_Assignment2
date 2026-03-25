# NLU_Assignment2

## Natural Language Understanding  

This repository contains my implementation for Assignment-2, which includes:

- Problem 1: Learning Word Embeddings (Word2Vec)  
- Problem 2: Character-Level Name Generation using RNN variants  

---

## Problem 1: Word Embeddings

In this part, I trained Word2Vec models on IIT Jodhpur-related text data.

- Collected and cleaned text from PDFs and text files  
- Applied preprocessing (tokenization, stopword removal, etc.)  
- Implemented:
  - CBOW  
  - Skip-gram (with negative sampling)  
- Evaluated using nearest neighbors and analogy tasks  
- Visualized embeddings using PCA  

Outputs:
- corpus.txt  
- wordcloud.png  
- cbow.png, skip_gram.png  

---

## Problem 2: Name Generation

In this part, I trained models to generate Indian names character by character.

Models used:
- RNN  
- BLSTM  
- RNN + Attention  

Evaluation metrics:
- Novelty → percentage of new names  
- Diversity → uniqueness of generated names  

Results:

| Model | Novelty | Diversity |
|------|--------|----------|
| RNN | 95.6% | 0.85 |
| BLSTM | 100% | 0.746 |
| Attention | 100% | 0.432 |

Observations:
- RNN gave the best balance of realistic and diverse names  
- BLSTM learned patterns but outputs were more synthetic  
- Attention produced more variation but also repetition  

---

## How to Run

Install dependencies:

  pip install numpy pandas torch nltk matplotlib PyPDF2 wordcloud scikit-learn
  
  Run Problem 1: 
  
  cd Problem-1
  
python b23cm1045_nluq1.py

Run Problem 2:

cd Problem-2

python b23cm1045_nluq2.py


---

## Author

Vamsi Krishna  
B23CM1045  
CSL7640 - Natural Language Understanding  

---

## Note

All models are implemented from scratch without using pre-trained embeddings.
