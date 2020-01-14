<!-- badges: start -->
[![Launch Rstudio Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KrogdahlLab/AquaFly-SeawaterGutHealth-Aquaculture-2019/master?urlpath=rstudio)
<!-- badges: end -->

# AquaFly-SeawaterGutHealth-Aquaculture-2019
This repository contains the data and code to reproduce the results presented in the paper **Total replacement of fish meal with black soldier fly (*Hermetia illucens*) larvae meal does not compromise the gut health of Atlantic salmon (*Salmo salar*)**.

## Run codes online
To run the analyses online, simply click on the `launch binder` badge above to start an RStudio instance. Note that multi-core parallel computing won't be availbe for the RStudio stance we use here. Thus, delete the codes for running parallel parametric bootstraps if you run the analyses via binder.

## Run codes locally
To run the analyses locally, download this repository as a zipped file. After decompression, open the R project file (`AqFl2_GutHealth.Rproj`) in the RStudio and run the R codes directly from the project root directory. Versions of R packages for each anaylsis can be found in the session information (*_sessionInfo.txt) under the same folder of R codes.

## File organization
Below is an overview of the file organization descending to level-3 directories.
```
root
├── AqFl2_GutHealth.Rproj
├── DESCRIPTION
├── LICENSE
├── README.md
├── analysis
│   ├── code
│   │   ├── histology.R
│   │   ├── histology_sessionInfo.txt
│   │   ├── organosomatic_index.R
│   │   ├── organosomatic_index_sessionInfo.txt
│   │   ├── qPCR_ref_DI.R
│   │   ├── qPCR_ref_DI_sessionInfo.txt
│   │   ├── qPCR_ref_PI.R
│   │   ├── qPCR_ref_PI_sessionInfo.txt
│   │   ├── qPCR_target_DI.R
│   │   ├── qPCR_target_DI_sessionInfo.txt
│   │   ├── qPCR_target_PI.R
│   │   └── qPCR_target_PI_sessionInfo.txt
│   ├── exploratory_analysis
│   │   ├── OSI_boxPlot.pdf
│   │   ├── OSI_violin.pdf
│   │   ├── histology_histogram.pdf
│   │   ├── qPCR_ref_DI_barPlot.pdf
│   │   ├── qPCR_ref_DI_boxPlot.pdf
│   │   ├── qPCR_ref_DI_pointDiagram.pdf
│   │   ├── qPCR_ref_PI_barPlot.pdf
│   │   ├── qPCR_ref_PI_boxPlot.pdf
│   │   ├── qPCR_ref_PI_pointDiagram.pdf
│   │   ├── qPCR_target_DI_boxPlot.pdf
│   │   ├── qPCR_target_DI_heatmap.pdf
│   │   ├── qPCR_target_DI_violin.pdf
│   │   ├── qPCR_target_PI_boxPlot.pdf
│   │   ├── qPCR_target_PI_heatmap.pdf
│   │   └── qPCR_target_PI_violin.pdf
│   └── model_diagnostics
│       ├── OSI_LMMs_residual.pdf
│       ├── OSI_welch-t_qqplot.pdf
│       ├── qPCR_DI_LMMs_residual.pdf
│       ├── qPCR_DI_welch-t_qqplot.pdf
│       ├── qPCR_PI_LMMs_residual.pdf
│       └── qPCR_PI_welch-t_qqplot.pdf
├── data
│   ├── README.md
│   ├── clean_data
│   │   ├── AqFl2_qPCR_ref_DI.csv
│   │   ├── AqFl2_qPCR_ref_PI.csv
│   │   ├── AqFl2_qPCR_target_DI.csv
│   │   ├── AqFl2_qPCR_target_PI.csv
│   │   └── Interplate_calibration.xlsx
│   └── raw_data
│       ├── AqFl2_LightCycler_files
│       ├── AqFl2_histology.csv
│       └── AqFl2_organosomatic_index.csv
└── results
    ├── figures
    │   ├── Figure 1.tiff
    │   ├── Figure 2.tiff
    │   ├── Figure 3.tiff
    │   └── Figure 4.tiff
    │   └── Figure S1.tiff
    │   └── Figure S2.tiff
    └── reference_gene_ranks
        ├── ref_gene_rank_DI.pdf
        └── ref_gene_rank_PI.pdf
```
## Acknowledgements
The R package [holepunch](https://karthik.github.io/holepunch/) was used to make the present R project binder-ready. Thanks are due to the *holepunch* developer Karthik Ram, who kindly helped to configure the Docker file and get the binder up and running.
