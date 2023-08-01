# Single Cell RNA-seq Analysis Workshop

The aim of this workshop is to provide a researcher with no prior coding experience the necasssary skills to perform their own analysis on a single-cell RNA-seq dataset. 

## R language resources
An basic knowledge of R programing language is beneficial, though not strictly necessary to perfom an analysis. There are several free beginner's courses for R, a simple web search will render a few. Here are a couple:

* https://lumc.github.io/rcourse/HLO_202301/S01L01l_index.html (Taught at LUMC)
* https://r-crash-course.github.io/

## Seurat package
[Seurat](https://satijalab.org/seurat/index.html) is a toolkit for single cell genomics written in R. It is developed and maintained by the Satija Lab, New York Genome Center. Is is probably the most popular single-cell analysis package.

### Guided clustering tutorial
The most common tasks that are relevant for any single-cell data analysis are covered in this [Seurat tutorial](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html), complete with a toy dataset. We typically use this tutorial as a basis for any analysis.

### Dataset integration
Identifying cell populations present accross multiple datasets can be problematic under standard workflows. Seurat includes a set o methods to match, ir align, shared cell populations accross datasets. The 
