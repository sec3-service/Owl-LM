# Large Language Model for Blockchain Transaction 

This repository contains resources for working with training LLM on blockchain transaction data. Here we share the finetuned model and tokenizer with some examples of how to use them. We will share more resources in the future.

The finetuned model and tokenizer are hosted at the folder LLM_for_Blockchain.

## Contents
`README.md`: This file.

`example.csv`: Contains samples of Ethereum transactions for classification. This dataset includes detailed transaction data.

`example_hash.csv`: Contains samples of Ethereum transactions for classification. This dataset does not include detailed transaction data.

`example.ipynb`: A Jupyter notebook that provides example usage of the model.

`requirements.txt`: Lists the Python dependencies required for using the code in this repository.

`LLM_for_Blockchain`: folder containing the LLM model.

## Installation
Clone this repository:

``git clone https://github.com/username/LLM-for-Blockchain.git``

Navigate to the cloned repository:

``cd LLM-for-Blockchain``

Install the required Python dependencies:

``pip install -r requirements.txt``

## Usage
Use example.ipynb as a guide to classify Ethereum transactions using the provided model. You can run the notebook using Jupyter.

You can also use the model and tokenizer directly from Hugging Face:


```
from transformers import AutoModelForSequenceClassification, AutoTokenizer

tokenizer = AutoTokenizer.from_pretrained("hubert233/LLM_for_Blockchain")

model = AutoModelForSequenceClassification.from_pretrained("hubert233/LLM_for_Blockchain")
```
