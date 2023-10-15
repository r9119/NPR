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
        accuracy: 0.9318181818181818
    - name: F1
      type: f1
      value:
        f1: 0.931761811198371
---

# distilbert_base_uncased

This model is a fine-tuned version of [bert-base-uncased](https://huggingface.co/bert-base-uncased) on the banking77 dataset.
It achieves the following results on the evaluation set:
- Loss: 0.3734
- Accuracy: {'accuracy': 0.9318181818181818}
- F1: {'f1': 0.931761811198371}

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
| No log        | 1.0   | 313  | 0.4137          | {'accuracy': 0.9058441558441559} | {'f1': 0.9060107320727019} |
| 0.0974        | 2.0   | 626  | 0.3840          | {'accuracy': 0.9207792207792208} | {'f1': 0.9209670309762171} |
| 0.0974        | 3.0   | 939  | 0.3771          | {'accuracy': 0.9282467532467532} | {'f1': 0.9282383702746585} |
| 0.0415        | 4.0   | 1252 | 0.3744          | {'accuracy': 0.9295454545454546} | {'f1': 0.9294711907234606} |
| 0.0079        | 5.0   | 1565 | 0.3734          | {'accuracy': 0.9318181818181818} | {'f1': 0.931761811198371}  |


### Framework versions

- Transformers 4.34.0
- Pytorch 2.0.0+cu118
- Datasets 2.14.5
- Tokenizers 0.14.1
