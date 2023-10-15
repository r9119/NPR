# NPR Mini Challenge 1 - Rami Tarabishi
This mini challenge covers Natural Language Processings (NPR) task about evaluating and discussing two separate models for text classification. The models are trained on the [banking77](https://arxiv.org/abs/2003.04807) dataset, which is a dataset of 13,083 customer service queries labeled with 77 intents. The models are evaluated on the test set of the dataset, which contains 3,080 queries.

# Prerequisites
To run the code in the notebook the packages in the `requirements.txt` file need to be installed. This can be done by running the following command in the terminal:
```bash
pip install -r requirements.txt
```

No GPU is strictly required to run the code, but it is recommended to use a GPU to speed up the training process.

# Repo structure
The repo is structured as follows:
- `MC1_NPR_Rami_Tarabishi.ipynb`: The notebook containing the code for training and evaluating the models.
- `README.md`: This readme file.
- `requirements.txt`: The file containing the required packages to run the code in the notebook.
- `Models`: The folder containing the trained models and their results.
- `Models/bert_base_uncased`: The folder containing the trained model and its results for the `bert_base_uncased` model.
- `Models/bert_base_uncased/README.md`: The readme file containing the results of the `bert_base_uncased` model.
- `Models/distilbert_base_uncased`: The folder containing the trained model and its results for the `distilbert_base_uncased` model.
- `Models/distilbert_base_uncased/README.md`: The readme file containing the results of the `distilbert_base_uncased` model.
- `Models/TF_IDF_SVM`: The folder containing the fitted SVM and TF-IDF vectoriser.