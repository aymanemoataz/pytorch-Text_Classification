# pytorch-Text_Classification

## Multi label comment classification | Repository overview :

## Dataset : UCC - Unhealthy comments corpus :
The goal of this practical project is to implement state-of-the-art NLP models in pytorch to perform multi-label text classification on the high-quality UCC dataset. This dataset was published in 2020 in the paper [Six Attributes of Unhealthy Conversation](https://arxiv.org/abs/2010.07410). 

The dataset now contains over 80,000 healthy and unhealthy comments. In addition to the binary labels, it also captures 6 unhealthy sub-attributes, such as (1) hostile, (2) insulting and trolling, (3) dismissive .... (6) unfair generalization. For some of these attributes, this was the first large publicly available dataset that captured them.

## Data Preprocessing :



## Model training :
The original paper aimed to present the dataset and they trained a BERT model on the text classification task. I used the basic BERT-base, T5 and roBERTa models. The latter had a better score in the classification of unhealthy labels.

## Results :



