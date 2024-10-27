# TGCN: a deep learning framework for improving cancer driver gene identification based on Transformer and graph convolutional network
## Abstract
We propose a method called TGCN, which is based on the integration of Transformer and graph convolutional network (GCN), aiming to improve cancer driver gene identification. Firstly, we compose multivariate feature matrices of genes from multi-omics data and multi-dimensional positional embedding derived from the gene association networks. Secondly, the multivariate feature matrices are fed into a Transformer module to learn the feature representations of genes. Finally, we utilize a Chebyshev GCN classifier to yield the identification results of cancer driver genes based on the feature representations.<br>
![Image text](https://github.com/wannaBMD/TGCN/blob/main/image/Figure1.jpg)
## Data
The multi-omics data and gene association networks used in TGCN can be found in the './data/' folder:<br>
'./data/pan/mut_features_miRNA_sub_du.txt': The 51-dimensional vector of multi-omics data.<br>
'./data/pan/': The folder contains the pan-cancer data required by TGCN for gene sets from different PPI sources.<br>
'./data/Specific cancer/': The folder contains the specific cancer types data required by TGCN for gene sets from different PPI sources.<br>
All data are used as input or output for programs in './Preprocess_data_required/'.<br>
## Requirements
- Python 3.8<br>
- PyTorch 1.12.1+cu113<br>
- PyTorch Geometric 2.5.2<br>
- dgl 1.1.1+cu113<br>
- jupyter notebook 7.2.1<br>
- ipykernel 6.29.5<br>
- ipython 8.12.3<br>
- numpy 1.24.4<br>
- pandas 2.0.3<br>
## Usage
If you want to regenerate the data files required for TGCN to identify cancer driver genes, please run the programs in the './Preprocess_data_required/' folder.<br>
Run the programs in the './TGCN_identification/' folder to view TGCN's performance of identifying driver genes for pan-cancer or single-type cancers, to view the performance on independent test sets, or to predict novel potential cancer driver genes using TGCN.<br>
Run the programs in the './Ablation experiments/' folder to view the results of ablation experiments.<br>
Please pay attention to the name differences of files from different PPI sources when running the program.<br>
