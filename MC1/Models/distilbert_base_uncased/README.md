---
license: apache-2.0
base_model: bert-base-uncased
tags:
- generated_from_trainer
datasets:
- banking77
metrics:
- accuracy
- f1
model-index:
- name: distilbert_base_uncased
  results:
  - task:
      name: Text Classification
      type: text-classification
    dataset:
      name: banking77
      type: banking77
      config: default
      split: test
      args: default
    metrics:
    - name: Accuracy
      type: accuracy
      value:
        accuracy: 0.9347402597402598
    - name: F1
      type: f1
      value:
        f1: 0.934673454742274
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# distilbert_base_uncased

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the banking77 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2750
- Accuracy: {'accuracy': 0.9347402597402598}
- F1: {'f1': 0.934673454742274}
- F1 Macro: 0.9347
- F1 Micro: 0.9347

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 32
- eval_batch_size: 64
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- num_epochs: 5

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy                         | F1                         | F1 Macro | F1 Micro |
|:-------------:|:-----:|:----:|:---------------:|:--------------------------------:|:--------------------------:|:--------:|:--------:|
| No log        | 1.0   | 313  | 0.5595          | {'accuracy': 0.8584415584415584} | {'f1': 0.8495892822843605} | 0.8496   | 0.8584   |
| 1.307         | 2.0   | 626  | 0.3344          | {'accuracy': 0.9116883116883117} | {'f1': 0.9120481581706692} | 0.9120   | 0.9117   |
| 1.307         | 3.0   | 939  | 0.2894          | {'accuracy': 0.9243506493506494} | {'f1': 0.9244180020715221} | 0.9244   | 0.9244   |
| 0.1762        | 4.0   | 1252 | 0.2833          | {'accuracy': 0.9305194805194805} | {'f1': 0.9304095827271768} | 0.9304   | 0.9305   |
| 0.0516        | 5.0   | 1565 | 0.2750          | {'accuracy': 0.9347402597402598} | {'f1': 0.934673454742274}  | 0.9347   | 0.9347   |


### Framework versions

- Transformers 4.34.0
- Pytorch 2.0.0+cu118
- Datasets 2.14.5
- Tokenizers 0.14.1
