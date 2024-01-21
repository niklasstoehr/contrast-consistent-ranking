# Contrast-Consistent Ranking (CCR)
⛰️ Repo accompanying the EACL 2024 paper: "Unsupervised Contrast-Consistent Ranking with Language Models"

**Niklas Stoehr, Pengxiang Cheng, Jing Wang, Daniel Preotiuc-Pietro, Rajarshi Bhowmik** <br>
**ETH Zurich, Bloomberg**

[arXiv link to paper](https://arxiv.org/abs/2309.06991)

We prepared a [Google Colaboratory notebook](https://colab.research.google.com/drive/1FzRUjpENIbGuauYjs6XTxdKV_m86ExR4?usp=sharing) that lets you reproduce most of the experiments presented in the paper.

The notebook first installs all required dependencies and instantiates class and functions needed
  - utils: helper or "util" functions such as converting pairwise to global rankings and vice versa
  - dataloading: functions for loading the datasets and "formulating" the prompts based on templates
  - embedder: script for pairing data instances, also tokenization and embedding
  - taskbuilding: PyTorch dataloader and training loop functionality
  - objectives: unsupervised probing losses and supervised counterparts
  - probes: scipt containing the probing models, i.e., linear regression models that are to be trained
  - prompts: scipts for running the prompting baselines with constrained decoding

As of now, the notebook is limited to two synthetic datasets, one focused on "fact-based" ranking tasks and one focused on "in-context" ranking tasks. We additionally publish our curated dataset of manually extracted [WikiLists rankings](https://docs.google.com/spreadsheets/d/17YVihsTguie9IhT-q5oDP3tSeShaJEEHNH-0OJVSipw/edit?usp=sharing).
