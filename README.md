# Single Cell RNA-seq Analysis Workshop

The aim of this workshop is to provide a researcher with no prior coding experience the necessary skills to perform their own analysis on a single-cell RNA-seq dataset. 

## R language resources
An basic knowledge of R programming language is beneficial, though not strictly necessary to perform an analysis. There are several free beginner's courses for R, a simple web search will render a few. Here are a couple:

* https://lumc.github.io/rcourse/HLO_202301/S01L01l_index.html (Taught at LUMC)
* https://r-crash-course.github.io/

## Seurat package
[Seurat](https://satijalab.org/seurat/index.html) is a toolkit for single cell genomics written in R. It is developed and maintained by the Satija Lab, New York Genome Center. Is is probably the most popular single-cell analysis package.

### Guided clustering tutorial
The most common tasks that are relevant for any single-cell data analysis are covered in this [Seurat tutorial](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html), complete with a toy dataset. We typically use this tutorial as a basis for any analysis.

### Dataset integration
Identifying cell populations present across multiple datasets can be problematic under standard workflows. Seurat includes a set o methods to match, or align, shared cell populations across datasets. These methods first identify cross-dataset pairs of cells that are in a matched biological state (‘anchors’), can be used both to correct for technical differences between datasets (i.e. batch effect correction), and to perform comparative scRNA-seq analysis of across experimental conditions. A workflow employing the default Seurat integration approach can be found [here](https://satijalab.org/seurat/articles/integration_introduction). It must be noted, however, that we have observed that this default approach typically results in over-correction, or in other words, removes too much biological variance. In our experience, using function [RunFastMNN](http://htmlpreview.github.io/?https://github.com/satijalab/seurat-wrappers/blob/master/docs/fast_mnn.html) typically renders more balanced results.
