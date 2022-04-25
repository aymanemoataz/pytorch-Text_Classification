# pytorch-Text_Classification

## Dataset : UCC - Unhealthy comments corpus :
The goal of this practical project is to implement state-of-the-art NLP models in pytorch to perform multi-label text classification on the high-quality UCC dataset. This dataset was published in 2020 in the paper [Six Attributes of Unhealthy Conversation](https://arxiv.org/abs/2010.07410). 

The dataset now contains over 80,000 healthy and unhealthy comments. In addition to the binary labels, it also captures 6 unhealthy sub-attributes, such as (1) hostile, (2) insulting and trolling, (3) dismissive .... (6) unfair generalization. For some of these attributes, this was the first large publicly available dataset that captured them.

## Model training :
The original paper aimed to present the dataset and they trained a BERT model on the text classification task. I used the BERT-base, T5 and roBERTa models. The latter had better scores in the classification of unhealthy labels.

<p align="center">
<img src="https://github.com/aymanemoataz/pytorch-Text_Classification/blob/main/images/train.png" width="270px" height="210px">
<img src="https://github.com/aymanemoataz/pytorch-Text_Classification/blob/main/images/validation.png" width="270px" height="210px">
</p>



## Results :
Given that the original paper was published in 2020 and focused on the dataset, I was able to replicate the same performance measure the authors used and achieve better scores for all labels before any hyperparameter optimization steps.

<p align="center">
<img src="https://github.com/aymanemoataz/pytorch-Text_Classification/blob/main/images/scores.png" width="500px" height="400px">
</p>

The authors scored 50% for the classification of the label sarcasm and talked about the difficulty of detecting sarcasm. With the fine-tuned roBERTa model, I was able to achieve a score of 75% without hyper parameter optimization.

