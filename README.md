# Sport Texts Classification — Ball or No-Ball

This project classifies Polish-language texts based on whether the described sport involves a ball.

## Task

Given a short text about a sport, predict:

- `1` — if it describes a ball sport  
- `0` — if it does **not** describe a ball sport

## Project Structure

- `train/` — compressed training data (`train.tsv.gz`)  
- `dev-0/` — validation input (`in.tsv`) and labels (`expected.tsv`)  
- `test-A/` — final test input and (optionally) expected labels  
- `cc.pl.300.vec` — pretrained FastText embeddings for Polish (download separately)  
- `network.ipynb` — main notebook for training and evaluating the model  
- `requirements.txt` — list of required Python packages  
- `config.txt` — optional configuration file

## Getting Started

### 1. Install dependencies

It's recommended to use a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 2. Download embeddings and sports texts
Download and extract the [Polish FastText embeddings](https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.pl.300.vec.gz) into the project directory.


### 3. Run the model

Open and run `network.ipynb` to train and evaluate the model.

