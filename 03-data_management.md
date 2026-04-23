# Data management

## Formative assignment RNA-seq DAUR2

``` r
fs::dir_tree(here::here("C:/Users/Ben/Documents/daur2_rnaseq"))
```

```
## C:/Users/Ben/Documents/daur2_rnaseq
## ├── analysis
## │   ├── formative_assignment_BvD_LE.html
## │   └── formative_assignment_BvD_LE.Rmd
## ├── data_processed
## │   ├── bam
## │   │   └── sample_1.bam
## │   └── counts
## │       └── read_counts.rds
## ├── data_raw
## │   └── fastq
## │       └── sample_1.fastq
## ├── README.html
## ├── README.md
## └── scripts
##     ├── alignment_mapping_plot_BvD_LE.R
##     └── fastq_dump_BvD_LE.sh
```



``` r
cat(readLines("C:/Users/Ben/Documents/daur2_rnaseq/README.md"), sep = "\n")
```

```
## # Project: DAUR2 RNA-seq analysis iPSC versus fibroblasts
## This folder contains the RNA-seq files used for the DAUR2 formatieve assignment in the DSFB1 course: a RNA-seq analysis of fibroblasts and induced pluripotent stem cells (iPSC).
## 
## <br>
## 
## ## Folder structure:
## `/analysis`  
## contains figures, images and other results of the analysis.  
## `/data_processed/bam`  
## contains aligned BAM files and alignment statistics.  
## `/data_processed/counts`  
## contains read count files used for DESeq2 analysis.  
## `/data_raw/fastq`  
## contains original FASTQ files.  
## `/scripts`  
## contains all scripts used for data processing and analysis.
## 
## <br>
## 
## ## Analysis workflow
## 1. Download FASTQ files
## 2. Quality control by FastQC
## 3. Alignment to hg38 reference genome
## 4. Feature counting by featureCounts
## 5. Differential expression analysis by DESeq2
## 6. GO-term enrichment analyse
## 
## <br>
## 
## ## Author:
## Andreas von Balen
```

## Portfolio repository
Portfolio repository
