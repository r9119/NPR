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
- name: bert_base_uncased
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
        accuracy: 0.9243506493506494
    - name: F1
      type: f1
      value:
        f1: 0.9244645146398242
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# bert_base_uncased

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the banking77 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.3937
- Accuracy: {'accuracy': 0.9243506493506494}
- F1: {'f1': 0.9244645146398242}
- F1 Macro: 0.9245
- F1 Micro: 0.9244

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
| No log        | 1.0   | 313  | 0.4017          | {'accuracy': 0.910064935064935}  | {'f1': 0.9099178948730132} | 0.9099   | 0.9101   |
| 0.0839        | 2.0   | 626  | 0.3756          | {'accuracy': 0.923051948051948}  | {'f1': 0.9228317252486437} | 0.9228   | 0.9231   |
| 0.0839        | 3.0   | 939  | 0.3942          | {'accuracy': 0.9217532467532468} | {'f1': 0.9215410940404721} | 0.9215   | 0.9218   |
| 0.0382        | 4.0   | 1252 | 0.3922          | {'accuracy': 0.9224025974025974} | {'f1': 0.9224608930249076} | 0.9225   | 0.9224   |
| 0.0064        | 5.0   | 1565 | 0.3937          | {'accuracy': 0.9243506493506494} | {'f1': 0.9244645146398242} | 0.9245   | 0.9244   |


### Framework versions

- Transformers 4.34.0
- Pytorch 2.0.0+cu118
- Datasets 2.14.5
- Tokenizers 0.14.1
