## miRmine data package

`miRmine` database is a collection of expression profiles from different publicly available miRNA-seq datasets, **Panwar et al (2017) miRmine: A Database of Human miRNA Expression**, prepared with this data package as RangedSummarizedExperiment.


# Installation 

To install the latest development version, use the `devtools` package (available [here](https://github.com/hadley/devtools))

```
devtools::install_github("duxan/miRmine")
```
<!--- 
# Vignette

The vignette contains all the preprocessing steps as well as some use-cases. It can be found in the "vignettes/miRmine.html" file. After installation, the vignette can be accessed from R:

```
browseVignettes("miRmine")
```

# DE with miRmine
library("DESeq2")
ddsSE <- DESeqDataSet(miRmine, design = ~ Disease)
ddsSE <- ddsSE[ rowSums(counts(ddsSE)) > 1, ]
dds <- estimateSizeFactors(ddsSE, type="iterate") # can take long time
dds <- DESeq(dds)
res <- results(dds)
res

--->

