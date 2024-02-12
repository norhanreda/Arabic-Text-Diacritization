# Arabic-Text-Diacritization

## Introduction

Diacritics are short vowels with a constant length that are spoken. The same word in the Arabic language can have different meanings and different pronunciations based on how it is diacritized.

In this project, we implement a pipeline to predict the diacritic of each character in an Arabic text using Natural Language Processing techniques.

## Project Pipeline
![Alt text](images/pipeline.png)

## Project Phases
### Data Processing

- Split the sentences with punctuations.
- Split into smaller sentences of length no more than `500` characters (without
counting diacritics).
- Remove all the non-Arabic characters.
- Remove diacritics.
- Start each sentence with `<s>` and end it with `</s>`
(both will have a corresponding class ‘no diacritics’ ‘’)

### Feature extraction
- One Hot encoding `char level`
- Trainable embeddings `char level`
- Word2vec embeddings + oneHot `word and char level`

### Model
- BLSTM
- RNN

<img src="images/model.png" alt="Alt text" width="500" height="500">

### Evaluation

`Diacritic Error Rate (DER) = 1 - Accuracy`

<img src="images/evaluation.png" alt="Alt text" width="600" height="300">


## Results

Final model used for the test set submission on Kaggle: **BLSTM model with char embedding layer**

`Team: The Powerpuff Girls`

<!-- <p align="center">
<img src="images/comp2.jpg" alt="Alt text" width="250" height="500">
<img src="images/comp2.jpg" alt="Alt text" width="250" height="500">
<img src="images/comp3.jpg" alt="Alt text" width="250" height="500">
</p> -->

<p align="center">
<img src="images/comp11.png" alt="Alt text" width="250" height="500">
<img src="images/comp22.png" alt="Alt text" width="250" height="500">
<img src="images/comp33.png" alt="Alt text" width="250" height="500">
</p>

