# Load bio and chem dataset to GL2vec

I used GL2vec model to get the embedding of biology and chemistry data.

The model is from the following paper:

Chen, Hong, and Hisashi Koga. "Gl2vec: Graph embedding enriched by line graphs with edge features." *International Conference on Neural Information Processing*. Springer, Cham, 2019.

## Installation

I used the following Python packages for core development. I tested on `Python 3.6`.

```
pytorch                   1.8.1
torch-geometric           1.0.3
torch-scatter             2.6.0 
torch-sparse              0.6.9
rdkit                     2019.03.1.0
typing-extension          3.7.4.3
numpy                     1.18.1
networkx                  2.5.1
karateclub                1.0.24
gensim                    3.8.3
tqdm                      4.60.0
```

## Dataset download

All the necessary data files can be downloaded from the following links.

For the chemistry dataset, download from [chem data](http://snap.stanford.edu/gnn-pretrain/data/chem_dataset.zip) (2.5GB), unzip it, and put it under `chem/`.
For the biology dataset, download from [bio data](http://snap.stanford.edu/gnn-pretrain/data/bio_dataset.zip) (2GB), unzip it, and put it under `bio/`.



Dataset from the following paper: 

Weihua Hu*, Bowen Liu*, Joseph Gomes, Marinka Zitnik, Percy Liang, Vijay Pande, Jure Leskovec. Strategies for Pre-training Graph Neural Networks. ICLR 2020.

## Print embedding

If you want to print the biology(chemistry) embedding , you should first go to the  `bio/`( `chem/`).

For biology embedding.

```
python GL2vec.py --dataset unsupervised
```

For chemistry embedding.

```
python GL2vec.py
```

