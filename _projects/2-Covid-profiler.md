---
layout: default
name: COVID-Profiler
intro: Automated analysis of Sars-Cov-2 sequencing data
img: /assets/img/covid-profiler-logo.png
tags:
    - Sars-Cov-2
    - NGS
    - Python
---
{% include figure.html url="http://genomics.lshtm.ac.uk/static/covid_profiler_logo.png" description="" %}


# About

 COVID-Profiler is a collection of tools which allow users to analyse Sars-Cov-2 sequencing and immunological data. Here is a non exaustive list of features:

 * Alignment and visualisation
 * Variant calling and functional annotation
 * Phylogenetic reconstruction
 * Primer conservation analysis

<div class="row">
    <div class="col-md-4">
        <img src="http://genomics.lshtm.ac.uk/static/example_pileup.png">
    </div>
    <div class="col-md-4">
        <img src="http://genomics.lshtm.ac.uk/static/example_phylogeny.png">
    </div>
    <div class="col-md-4">
        <img src="http://genomics.lshtm.ac.uk/static/primer_map.png">
    </div>
</div>

# Development

The pipeline is developed using python. Sequences are aligned to the reference genome (NC_045512.2) using minimap2  Variants are called using paftools.js from the minimap2 package and bcftools and transformed into a fasta alignment. IQ-TREE is used to reconstruct the phylogeny. Sample data is downloaded from NCBI nucleotide database using Entrez Direct. The website is built using flask. All the code is available from [here](https://github.com/jodyphelan/covid-profiler).

# Citation

A manuscript is currently under review. If you would like to cite, please use [this preprint](https://www.biorxiv.org/content/10.1101/2020.04.28.066977v1)
