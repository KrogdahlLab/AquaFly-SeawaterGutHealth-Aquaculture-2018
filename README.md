<!-- badges: start -->
[![Launch Rstudio Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/KrogdahlLab/AquaFly-SeawaterGutHealth-Aquaculture-2019/master?urlpath=rstudio)
<!-- badges: end -->

## Total replacement of fish meal with black soldier fly (*Hermetia illucens*) larvae meal does not compromise the gut health of Atlantic salmon (*Salmo salar*)
### doi: https://doi.org/10.1016/j.aquaculture.2020.734967

Limited availability of sustainable feed ingredients is a significant concern in salmon aquaculture. Insects may become an important, sustainable resource for expanding the raw material repertoire. Herein, we present data from a 16-week seawater feeding trial with Atlantic salmon (initial body weight, 1.4 kg) fed either a reference diet with a combination of fish meal, soy protein concentrate, pea protein concentrate, corn gluten and wheat gluten as protein source, or a test diet wherein all the fish meal and most of the pea protein concentrate were replaced by black soldier fly larvae meal. The gut health of fish was evaluated using endpoints including organ and tissue indices, histopathology variables and gene expression indicative of lipid metabolism, immune responses, barrier functions and detoxification/stress responses. A higher relative weight of distal intestine was found in fish fed the insect meal diet. Steatosis of enterocytes was observed in the proximal and mid intestine in both diet groups, albeit, less severe in the proximal intestine of fish fed the insect meal diet. Inflammatory morphological changes, similar to those induced in the distal intestine by standard soybean meal, were present in all the examined intestinal segments, with a higher degree of submucosa cellularity in the proximal intestine of insect meal diet fed fish, the only notable diet effect. Few deferentially expressed genes were identified in the proximal or distal intestine. In summary, total replacement of fish meal with black soldier fly larvae meal did not compromise the gut health of Atlantic salmon.

### How to regenerate results
## Run code online
To run the analyses online, click the `launch binder` badge located at the top of this README file. After clicking the badge, this repository will be turned into an RStudio instance that has all the dependencies installed. Then run all the R code online and regenerate results presented in the paper. Note that multi-core parallel computing is not available for the RStudio stance we use here. Thus, skip the code for running parallel parametric bootstraps if you run the analyses online.

## Run code locally
To run the analyses locally, download this repository as a zipped file. After decompression, open the R project file (`AqFl2_GutHealth.Rproj`) in the RStudio and run the R code directly from the project root directory. Versions of R packages for each analysis can be found in the session information (*_sessionInfo.txt) under the same folder where R code is stored.

## File organization
Below is an overview of the file organization in this repository.
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
    │   ├── Figure 4.tiff
    │   ├── Figure S1.tiff
    │   └── Figure S2.tiff
    └── reference_gene_ranks
        ├── ref_gene_rank_DI.pdf
        └── ref_gene_rank_PI.pdf
```
## Acknowledgements
The R package [holepunch](https://karthik.github.io/holepunch/) was used to make the present R project binder-ready. Thanks are due to the *holepunch* developer Karthik Ram, who kindly helped to configure the Docker file and make the binder work.
