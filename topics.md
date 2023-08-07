# Topics

For this part of the workshop a Seurat object of a single-cell dataset will be provided. Cells in the dataset will be already clustered in what we believe is the optimal clusters. The following downstream tasks will be performed:
* Discover the marker genes of a particular cluster by performing a Differential Gene Expression analysis.
* Visualize the Differentially Expressed Genes (DEGs) using a volcano plot
* Visualize DEGs, or your gene set of choice, using a heatmap
* Customize your visualizations, by, for example, adding a dendrogram to the heatmap
* Explore the dataset repository and visualization tool  [CELLxGENE](https://cellxgene.cziscience.com/). Is there a dataset of your interest? Can you see any added value to the interactive visualizations provided by the tool?
* Install Python and then [CELLxGENE](https://github.com/chanzuckerberg/cellxgene) on your machine. Interactively explore your dataset using it. You first need to [convert](https://mojaveazure.github.io/seurat-disk/articles/convert-anndata.html) the Seurat object into an [AnnData](https://anndata.readthedocs.io/en/latest/) object
