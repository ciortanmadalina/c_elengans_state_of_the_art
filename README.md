# Single cell RNA seq method comparaison

Run the project by following the next steps:

1. Clone github repo:

git clone https://github.com/ciortanmadalina/single-cell-sota.git

2. Start docker and mount github code:

sudo docker run -d -p 8787:8787 -v $PWD/single-cell-sota:/home/rstudio/single-cell-sota quay.io/hemberg-group/scrna-seq-course-rstudio 

Ths project compares the following methods:
- Seurat
- Monocle
- SC3 : freezes during clustering phase

on the following datasets:

- deng (https://www.ncbi.nlm.nih.gov/pubmed/24408435 : 
To illustrate clustering of scRNA-seq data, we consider the Deng dataset of cells from developing mouse embryo (Deng et al. 2014). We have preprocessed the dataset and created a SingleCellExperiment object in advance. We have also annotated the cells with the cell types identified in the original publication (it is the cell_type2 column in the colData slot). )
- Peripheral Blood Mononuclear Cells (PBMCs) from a healthy donor.(wget -c http://cf.10xgenomics.com/samples/cell-exp/2.0.1/pbmc8k/pbmc8k_filtered_gene_bc_matrices.tar.gz)
- C-elegans

