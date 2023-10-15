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
        accuracy: 0.9327922077922078
    - name: F1
      type: f1
      value:
        f1: 0.9328356856137137
---

# bert_base_uncased

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the banking77 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2798
- Accuracy: {'accuracy': 0.9327922077922078}
- F1: {'f1': 0.9328356856137137}

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

| Training Loss | Epoch | Step | Validation Loss | Accuracy                         | F1                         |
|:-------------:|:-----:|:----:|:---------------:|:--------------------------------:|:--------------------------:|
| No log        | 1.0   | 313  | 0.5606          | {'accuracy': 0.8694805194805195} | {'f1': 0.8632383764972809} |
| 1.3465        | 2.0   | 626  | 0.3441          | {'accuracy': 0.9123376623376623} | {'f1': 0.9127017123917218} |
| 1.3465        | 3.0   | 939  | 0.2819          | {'accuracy': 0.9262987012987013} | {'f1': 0.9263826267949322} |
| 0.1841        | 4.0   | 1252 | 0.2840          | {'accuracy': 0.9275974025974026} | {'f1': 0.927696291077944}  |
| 0.0515        | 5.0   | 1565 | 0.2798          | {'accuracy': 0.9327922077922078} | {'f1': 0.9328356856137137} |


### Framework versions

- Transformers 4.34.0
- Pytorch 2.0.0+cu118
- Datasets 2.14.5
- Tokenizers 0.14.1
