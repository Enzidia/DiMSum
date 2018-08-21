<p align="left">
  <img src="./Dumpling.png">
</p>

# Overview

Welcome to the GitHub repository for DiMSum: A pipeline for pre-processing of paired-end reads from deep mutational scannning (DMS) data.

# Required Software

To run the DiMSum pipeline you will need the following software and associated packages:

* **[Python](https://www.python.org/downloads/) v3.6** (argparse, biopython)
* **[R](https://www.r-project.org/) v3.3** (data.table, seqinr, optparse, parallel, reshape2, ggplot2, plyr)
* **[FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/) v0.11.3**
* **[cutadapt](https://cutadapt.readthedocs.io/en/stable/) v1.16**
* **[USEARCH 32-bit](https://drive5.com/usearch/download.html) v10.0**
* **fastx_collapser** from the [FASTX Toolkit](http://hannonlab.cshl.edu/fastx_toolkit/download.html) v0.0.13

# Installation

```
git clone https://github.com/CRG-CNAG/DiMSum.git
```
Add the cloned DiMSum repository base directory to your path. You can do this by adding the following line at the bottom of your ~/.bashrc file:
```
export PATH=YOUR_DIMSUM_DIR:$PATH
```
Get a description of DiMSum command-line arguments with the following:
```
DiMSum -h
```

# Pipeline

The DiMSum pipeline processes paired-end reads (in FASTQ format) from deep mutational scanning (DMS) experiments to produce variant counts for each sample. These counts are suitable for use in downstream analyses of epistasis and [protein structure determination](https://github.com/lehner-lab/DMS2structure).

To run this pipeline, you will first need to describe your experimental design (e.g. in MSExcel) and save this as a tab-separated plain text file. You can download [this](./example_experimentDesign.txt) file to use as a template.

Additionally, if your raw FASTQ sequencing files contain multiplexed samples you will need to provide a tab-separated plain text file describing how barcodes map to samples. You can download [this](./example_barcodeDesign.txt) file to use as a template.

## Stage 1: DEMULTIPLEX



## Stage 2: FASTQC

## Stage 3: UNZIP

## Stage 4: SPLIT

## Stage 5: CUTADAPT

## Stage 6: USEARCH

## Stage 7: UNIQUE

## Stage 8: FILTER

## Stage 9: MERGE



(Vector illustration credit: <a href="https://www.vecteezy.com">Vecteezy!</a>)
