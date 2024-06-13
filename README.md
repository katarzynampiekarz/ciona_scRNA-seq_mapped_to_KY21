# _Ciona_ scRNA-seq mapped to KY21 gene model

## About

The raw data obtained from Cao et al. (2019; GSM3764781; https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM3764781) were re-mapped to the KY21 gene models (http://ghost.zool.kyoto-u.ac.jp/download_ht.html) using RNA STARsolo package (toolshed.g2.bx.psu.edu/repos/iuc/rna_starsolo/rna_starsolo/2.7.8a) on a Galaxy server (usegalaxy.org, Galaxy Version 2.7.8a; The Galaxy Community, 2024 update) to generate files containing raw barcodes, raw genes, and raw gene counts that were then used as an input to generate Seurat objects (Seurat v4; Hao, Hao et al., 2021). The Seurat objects were then processed following the Seurat Guided Clustering Tutorial (vignettes/pbmc3k_tutorial.Rmd), with some modifications. All ten developmental stages were re-analyzed:

1) iniG
2) midG
3) earN
4) latN
5) iniTI
6) earTI
7) midTII
8) latTI
9) latTII
10) larva

## Data

The data is available on OSF: https://osf.io/2gvwq/
The files for each developmental stage are organized in a separate folder. Each folder has three subfolders:
1) "final" - containing the jpg image of the final clustering, R (Seurat) object, and h5ad object that can be used in cellxgene
2) "mapping" - RNA STARsolo output files used to generate Seurat objects
3) "markers" - list of markers identified for each cluster, as well as plots showing the expression of top markers

## References

Cao C, Lemaire LA, Wang W, Yoon PH, Choi YA, Parsons LR, Matese JC, Wang W, Levine M, Chen K (2019). Comprehensive single-cell transcriptome lineages of a proto-vertebrate. Nature 571, 349–354. https://doi.org/10.1038/s41586-019-1385-y.

Hao Y, Stuart T, Kowalski MH, Choudhary S, Hoffman P, Hartman A, Srivastava A, Molla G, Madad S, Fernandez-Granda C, Satija R (2023). “Dictionary learning for integrative, multimodal and scalable single-cell analysis.” Nature Biotechnology. doi:10.1038/s41587-023-01767-y, https://doi.org/10.1038/s41587-023-01767-y.

Hao Y, Hao S, Andersen-Nissen E, III WMM, Zheng S, Butler A, Lee MJ, Wilk AJ, Darby C, Zagar M, Hoffman P, Stoeckius M, Papalexi E, Mimitou EP, Jain J, Srivastava A, Stuart T, Fleming LB, Yeung B, Rogers AJ, McElrath JM, Blish CA, Gottardo R, Smibert P, Satija R (2021). “Integrated analysis of multimodal single-cell data.” Cell. doi:10.1016/j.cell.2021.04.048, https://doi.org/10.1016/j.cell.2021.04.048.

The Galaxy Community. The Galaxy platform for accessible, reproducible, and collaborative data analyses: 2024 update, Nucleic Acids Research, 2024; gkae410, https://doi.org/10.1093/nar/gkae410.
