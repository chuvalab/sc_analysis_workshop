# Topics Discussed 

For this part of the workshop a Seurat object of a single-cell dataset will be provided. This concerns cells from a gastrulating human embryo from [Tyser et al.(2020)](https://www.nature.com/articles/s41586-021-04158-y). Cells in the dataset will be already clustered in what we believe is the optimal clusters. The following downstream tasks will be performed:

## DAY 1
* Intro to R markdown
* Explore the meta data of Seurat object
* Discover the marker genes of a particular cluster by performing a Differential Gene Expression analysis (you will be assigned one cluster)
* Visualize the Differentially Expressed Genes (DEGs) using the build-in functions of Seurat violin and feature plot
  * visualize the expression of the top 10 DEGs of your cluster on the UMAP
  * discover the PGCs in the UMAP of the Tyser dataset (hint: look for expression of NANOS3)
  * plot the top 3 DEGS of your cluster as violin plot

* Visualize the DEGs using a volcano plot
  * make a volcano plot between your cluster and cluster 13
  
* Visualize the DEGs, or your gene set of choice, using a heatmap
  * select 10 genes of your choice and plot the expression in a heatmap in all clusters
  * Plot top 100 most variable genes from this dataset on a heatmap
  
* Customize your heatmap, by, for example, removing the dendrogram
  * remove the dendrogram from clsuters (columns) or genes (rows)
  * Keep the original order for the genes in your heatmap
  * Z-score values heatmap
  
* Perform a Gene Ontology enrichment analysis with gProfiler
  * peform GO enrichment analysis on the DEGs of your assigned cluster
  
* Perform a Gene Ontology enrichment using REACTOME (if there is still time in day 1)
  * go to REACTOME, paste your DEG list, etc
 
* Knit your Rmd!


## DAY 2  
* Explore the dataset repository and visualization tool [CELLxGENE](https://cellxgene.cziscience.com/).
  1. go online and find an data set on human ovary, sequenced using 10x genomics (click explore)
  2. change the 'embedding choice' to tsne
  3. color the data set per 'donor-id': how many cells does pat9 have?
  4. how many granulosa cells are in the dataset (hint: check 'cell_type')
  5. how many donors contributed cells to 'cell_type': granulosa cell
  6. visualise gene TFPI on the UMAP: what cluster does it correspond to? and to what cell-type?
  7. Calculate DEGS between cluter 16 and all the rest of the data set
  8. calculate the DEGs between cluster 16 and cluster 0
  9. take the top  degs and check how speciif they are for cluster 16

* [Install](https://github.com/chuvalab/sc_analysis_workshop/blob/main/cellxgene_installation_windows.md) Python and then [CELLxGENE](https://github.com/chanzuckerberg/cellxgene) on your machine. [Convert](https://mojaveazure.github.io/seurat-disk/articles/convert-anndata.html) the Seurat object into an [AnnData](https://anndata.readthedocs.io/en/latest/) object. Interactively explore your dataset using it
  1. open Tyser `.h5ad` file with CELLxGENE
  2. color the data set per 'cluster_ID': how many cells does 'axial mesoderm' have?
  4. how many 'seurat-clusters' are in the dataset?
  5. what is the cluster that contains 'erythroblasts'? How many erythorbvlasts are there is this dataset?
  6. Find out what cluster includes endothelial cells (hint: check expression of PECAM1)
  7. visualise gene NANOS3 on the UMAP
  8. Calculate DEGS between cluter 3 and all the rest of the data set
  9. calculate the DEGs between cluster 3 and cluster 12
  10. take the top degs and check how speciif they are for cluster 3
  
* Working with LUMC High Performance Computer (Shark). For more see [here](https://pubappslu.atlassian.net/wiki/spaces/HPCWIKI/pages/37520089/Workshops)
* Other topics of interest? 😃  
