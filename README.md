# Understand Open Targets data with language models

This repository contains code to train and evaluate language models on Open Targets data.

Open Targets data is separated in different datasets, I want to automate the process of understanding the relationships between datasets. Since this cannot be done directly with the data schemas, the idea is to *generate embeddings from the schema and a subset of data for each dataset and then use the model to draw those relationships*.

## Wiki
This is a semantic query engine that uses a language model to understand the meaning of a query and return the most relevant results. As embedding model I am using `gtr-t5-xl` from [sentence-transformers](https://huggingface.co/sentence-transformers/gtr-t5-large) as a starting point because of its high performance on semantic search tasks according to [benchmarks](https://huggingface.co/spaces/mteb/leaderboard). On top of that, it is easy and free to use.
As a note, [this article](https://medium.com/@nils_reimers/openai-gpt-3-text-embeddings-really-a-new-state-of-the-art-in-dense-text-embeddings-6571fe3ec9d9) is an interesting comparison of the performance against expensive, larger models like OpenAI's GPT-3, showing that the gain in performance is not worth the economic and computational cost.


The language model is trained on Open Targets data and is able to understand the meaning of a query and return the most relevant results. 


---

## Installation

To install the dependencies, create a virtual environment and install the requirements:
```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Usage

TBD