This repository contains all the required data and code to reproduce the analyses and visualization in the following study:

> Kun Guo, Petr Pyšek, Milan Chytrý, Jan Divíšek, Martina Sychrová, Zdeňka Lososová, Mark van Kleunen, Simon Pierce, Wen-Yong Guo. Stage dependence of Elton’s biotic resistance hypothesis of biological invasions. Nature Plants. Accepted.

## How to use:

> 1. Download this repo as .zip file and unzip it to a folder.

> 2. Open *WorldPlantInvasion.Rproj* with Rstudio.

> 3. Open [*BioticResistance_InvasionContinuum.qmd*](https://github.com/kun-ecology/BioticResistance_InvasionContinuum/main/BioticResistance_InvasionContinuum.qmd) and load [*Data4BioticResistance_InvasionContinuum.RData*](https://github.com/kun-ecology/BioticResistance_InvasionContinuum/main/Data4BioticResistance_InvasionContinuum.RData) to access all the code and data used for analyses and figure reproduction.

> 4. The folder [*figures*](https://github.com/kun-ecology/BioticResistance_InvasionContinuum/main/figures) contains all figures included in main text and supplementary. While all figures were generated in R, Adobe Illustrator was used for refinements.

> 5. The folder [*results*](https://github.com/kun-ecology/BioticResistance_InvasionContinuum/main/results) contains all intermediate results of the SES values of phylogenetic and functional metrics. Due to potential long calculation times, you may import *pd.mpd.mntd2024.RDS* for further analyses.

## File structure

- `BioticResistance_InvasionContinuum.qmd`: Main analysis script
- `Data4BioticResistance_InvasionContinuum.RData`: Primary dataset
- `figures`: Folder containing all generated figures
- `results`: Folder containing intermediate calculation results

## **NOTE on computation**

> Calculating SES values for phylogenetic and functional metrics with large datasets (>10,000 plots and > 1,000 species) is computationally intensive. This study used custom functions i.e., *fst.ses.pd*, *fst.ses.mpd*, *fst.ses.mntd* from the R package [**ecoloop**](https://github.com/kun-ecology/ecoloop), with parallelization implemented via R package [**furrr**](https://furrr.futureverse.org/). 

> Even with a high-performance server (2 Intel Xeon Gold 6226 R CPU and 256 GB memory), calculation took approximately 2 hours. Computation time may vary significantly depending on your hardware.

## Contact

> For any questions or issues, please open an issue in this respository.