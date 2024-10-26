# TGCN:a deep learning framework for improving cancer driver gene identification based on Transformer and graph convolutional network
## Abstract
We propose a method called TGCN, which is based on the integration of Transformer and graph convolutional network (GCN), aiming to improve cancer driver gene identification. Firstly, we compose multivariate feature matrices of genes from multi-omics data and multi-dimensional positional embedding derived from the gene association networks. Secondly, the multivariate feature matrices are fed into a Transformer module to learn the feature representations of genes. Finally, we utilize a Chebyshev GCN classifier to yield the identification results of cancer driver genes based on the feature representations.<br>
![Image text](https://github.com/wannaBMD/TGCN/blob/main/image/Figure1.jpg)
## Data
The multi-omics data and gene association networks used in TGCN can be found in the './data/' folder:<br>
'./data/pan/mut_features_miRNA_sub_du.txt': Among the 51-dimensional vector of multi-omics data, 48 dimensions are the same as in EMOGI, consisting of gene mutation rates, differential DNA methylation rates, and differential expression rates, which span across 16 different cancer types. We adopt the same way as HWC to calculate the differential expression scores of miRNAs associated with genes.<br>
'./data/pan/string_850/', './data/pan/CPDB/' and './data/pan/BioPlex/': The folder contains the pan-cancer data required by TGCN for gene sets from different PPI sources.<br>
'./data/Specific cancer/': The folder contains the specific cancer types data required by TGCN for gene sets from different PPI sources.<br>
All data is used as input or output for programs in './Preprocess_data_required/'.<br>
