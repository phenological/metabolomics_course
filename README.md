# Metabolomics Course 2025

## Installation Instructions

This guide will help you set up your environment for the **2025 Metabolomics** course.  
You will install **R**, **RStudio**, essential packages for metabolomics, Git for version control, and configure GitHub integration.


1. Install R and RStudio
   - Download RStudio from: https://posit.co/download/rstudio-desktop/

2. Launch RStudio

3. Install libraries for metabolomics
   - R has a great package manager and CRAN archive. Install some useful libraries:
     - install.packages("devtools")
     - install.packages("ggplot2")

4. Bioconductor Package Manager
   - Some users prefer Bioconductor for additional libraries: https://www.bioconductor.org/
     - install.packages("BiocManager")
     - Test Bioconductor by installing ropls:
       - BiocManager::install("ropls")
       - More info: https://bioconductor.riken.jp/packages/3.17/bioc/html/ropls.html

5. GitHub Setup for R Development
   - Some libraries are hosted on GitHub, which is also useful for development:
     - Create a GitHub account
     - Install Git. On macOS, use Homebrew:
       - /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
       - brew install git
     - Configure GitHub for R/RStudio: https://happygitwithr.com/https-pat
       - Create access token: usethis::create_github_token()
       - Setup access token: gitcreds::gitcreds_set()

6. Install In-House Libraries from GitHub
   - Use devtools to install the following libraries from github.com/phenological:
     - devtools::install_github("phenological/fusion")
     - devtools::install_github("phenological/nmr.spectra.processing")
     - devtools::install_github("phenological/mva.plots")

7. My First R Notebook
   - Create and run your first R Notebook to begin exploring metabolomics.