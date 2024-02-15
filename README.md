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

# demo video to the deployed model


https://github.com/norhanreda/Arabic-Text-Diacritization/assets/88630231/957e03d9-2413-4c80-9397-f48874075f0e



## Contributors <a name = "Contributors"></a>

<table>
  <tr>
    <td align="center">
    <a href="https://github.com/asmaaadel0" target="_black">
    <img src="https://avatars.githubusercontent.com/u/88618793?s=400&u=886a14dc5ef5c205a8e51942efe9665ed8fd4717&v=4" width="150px;" alt="Asmaa Adel"/>
    <br />
    <sub><b>Asmaa Adel</b></sub></a>
    </td>
    <td align="center">
    <a href="https://github.com/Samaa-Hazem2001" target="_black">
    <img src="https://avatars.githubusercontent.com/u/82514924?v=4" width="150px;" alt="Asmaa Adel"/>
    <br />
    <sub><b>Samaa Hazem</b></sub></a>
    </td>
    <td align="center">
    <a href="https://github.com/norhanreda" target="_black">
    <img src="https://avatars.githubusercontent.com/u/88630231?v=4" width="150px;" alt="norhan reda"/>
    <br />
    <sub><b>Norhan reda</b></sub></a>
    </td>
    <td align="center">
    <a href="https://github.com/Hoda233" target="_black">
    <img src="https://avatars.githubusercontent.com/u/77369927?v=4" width="150px;" alt="HodaGamal"/>
    <br />
    <sub><b>HodaGamal</b></sub></a>
    </td>
  </tr>
 </table>



