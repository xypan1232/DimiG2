# DimiG2 for inferring disease-associated miRNAs
The microRNAs (miRNAs) play crucial roles in many biological processes involved in diseases and miRNAs function with protein coding genes (PCGs). In this study, we present a semi-supervised multi-label framework to integrate PCG-PCG interactions, PCG-miRNA interactions, PCG-disease associations by integrating disease hierarchy into graph convolutional network (GCN). DimiG is then trained on a graph, which is further used to score associations between diseases and miRNAs.

# software dependency
  * <a href=https://github.com/scikit-learn/scikit-learn>sklearn</a> <br>
  * GCN
  * <a href=https://pytorch.org/>PyTorch 0.4 or 0.5</a> <br>
  * Python 2.7

## Installation of GCN
Here we modified the orginal GCN (https://github.com/tkipf/pygcn) to support multi-label learning. <br> 
```python setup.py install```

# Data depedency: <br>
   - PCG-PCG interaction file "9606.protein.links.v10.txt.gz" can be downloaded from <a href="https://string-db.org/">STRING</a> v10 database. <br>
   - Disease-PCG assications file "human_disease_integrated_full.tsv" can be downloaded from <a href="https://diseases.jensenlab.org/Downloads">DISEASES </a> database. We also upload the file human_disease_integrated_full.zip in this repository, please decompress it at directory data/.  <br>
   - PCG-miRNA interaction file "9606.v1.combined.tsv.gz" can be downloaded from <a href="https://rth.dk/resources/rain/">RAIN</a> v1.0 database. <br>
   - GTEx_Analysis_2016-01-15_v7_RNASeQCv1.1.8_gene_median_tpm.gct.gz from GTEx website <br>
   - gencode.v19.genes.v7.patched_contigs.gtf.gz  from GTEx website <br>
   - The above three files need be saved at dir "data/". <br> 


