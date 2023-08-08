# Topics Discussed 

For this part of the workshop a Seurat object of a single-cell dataset will be provided. Cells in the dataset will be already clustered in what we believe is the optimal clusters. The following downstream tasks will be performed:

DAY1
* Discover the marker genes of a particular cluster by performing a Differential Gene Expression analysis (you will be assigned one cluster)
* Visualize the Differentially Expressed Genes (DEGs) using the build-in functions of Seurat violin and feature plot
   1. plot the top 10 DEGs of your cluster on the UMAP
   2. discover the PGCs in the UMAP of the Tyser dataset (hint: look for expression of NANOS3)
   3. plot the top 3 DEGS of your cluster as violin plot

* Visualize the DEGs using a volcano plot
  4. make a vulcano plot between your cluster and cluster 13
  
* Visualize the DEGs, or your gene set of choice, using a heatmap
  5. choose 10 genes of your choice and plot the expression in a heatmap in all clusters
  
* Customize your visualizations, by, for example, adding a dendrogram to the heatmap
  6. put a dendrogram on the clusters
  7. put a dendrogram in the genes (but not on the clusters)
  8. add 5 more genes and remove 3 genes, make the heatmap and put a dendrogram on the clusters
  
* Perform a Gene Ontology enrichment analysis with gProfiler
  9. peform GO on the DEGs of your assigned cluster
  
* Perform a Gene Ontology enrichment using REACTOME (if there is still time in day 1)
  10. Go to REACTOME, paste your DEG list, etc


DAY2  
* Explore the dataset repository and visualization tool  [CELLxGENE](https://cellxgene.cziscience.com/).
  1. go online and find an data set on human ovary, normal sequenced using 10x genomics (click explore)
  2. change in 'embedding choice' to tsne
  3. color the data set per 'donor-id': how many cells does pat9 have?
  4. how many granulosa cells are in the dataset (hint: check 'cell_type')
  5. how many donors contributed cells to 'cell_type': granulosa cell
  6. visualise gene TFPI on the UMAP: what cluster does it correspond to? and to what cell-type?
  7. Calculate DEGS between cluter 16 and all the rest of the data set
  8. calculate the DEGs between cluster 16 and cluster 0
  9. take the top  degs and check how speciif they are for cluster 16

* Install Python and then [CELLxGENE](https://github.com/chanzuckerberg/cellxgene) on your machine. [Convert](https://mojaveazure.github.io/seurat-disk/articles/convert-anndata.html) the Seurat object into an [AnnData](https://anndata.readthedocs.io/en/latest/) object. Interactively explore your dataset using it
  3. open Tyser dataset
  2. color the data set per 'cluster_ID': how many cells does 'axial mesoderm' have?
  4. how many 'seurat-clusters' are in the dataset?
  2. what is the cluster that contains 'erythroblasts'? How many erythorbvlasts are there is this dataset?
  5. Find out what cluster includes endothelial cells (hint: check expression of PECAM1)
  6. visualise gene NANOS3 on the UMAP
  7. Calculate DEGS between cluter 3 and all the rest of the data set
  8. calculate the DEGs between cluster 3 and cluster 12
  9. take the top degs and check how speciif they are for cluster 3
  
* Work on LUMC High Performance Computer (Shark)
* Other topics of interest? 😃  
