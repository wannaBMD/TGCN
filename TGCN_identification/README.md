## Running TGCN
- './TGCN.ipynb': Running this program can obtain TGCN's performance of identifying pan-cancer driver genes. We adopted the average AUC and the average AUPRC from ten five-fold cross-validations as evaluation indicators.<br>
- './TGCN_sct.ipynb': Running this program can obtain TGCN's performance of identifying single-type cancer driver genes. We adopted the average AUC and the average AUPRC from ten five-fold cross-validations as evaluation indicators.<br>
- './indenpend_test.ipynb': Running this program can obtain TGCN's performance on independent test sets. We adopted the AUPRC as evaluation indicators.<br>
- './novel_gene.ipynb': Runing this program can obtain the prediction score file for unlabeled genes ('pred_novel.txt'), where a higher score indicates a greater likelihood of the gene being a novel cancer driver. The genes order of the prediction score file corresponds to the gene name order of the 'novel_gene.txt' file in the '../data/pan/' folder.<br>
