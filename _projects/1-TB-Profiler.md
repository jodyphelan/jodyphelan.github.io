---
layout: default
name: TB-Profiler
intro: Predicting tuberculosis drug resistance from NGS data
img: /assets/img/tb-profiler-logo-rectangle.png
tags:
    - Tuberculosis
    - NGS
    - Software
---


{% include figure.html url="/assets/img/tb-profiler-logo-rectangle.png" description="" %}


![downloads](https://img.shields.io/conda/dn/bioconda/tb-profiler.svg?style=flat) ![licence](https://camo.githubusercontent.com/68294f22dd92b36b437cec0d17cda6829f1d37d6a2c270f0cc6a4c549e5b8e45/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f6a6f64797068656c616e2f544250726f66696c65722e737667) ![install](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat) ![commit](https://img.shields.io/github/last-commit/jodyphelan/TBProfiler?color=blue)

# What is it?
TB-Profiler is a command-line tool used to process whole genome sequencing data to predict lineage and drug-resistance. The pipeline searches for small variants and big deletions associated with drug resistance. It will also report the lineage. By default it uses trimmomatic to trim the reads, BWA (or minimap2 for nanopore) to align to the reference genome and bcftools (or GATKv4/freebayes) to call variants. The tool has been downloaded and used by researchers around the globe.

# Development
The software was developed using a mixture of custom python and open source bioinformatic software. It was designed with speed and resource usage in mind, being able to run on commodity hardware.

{% include figure.html url="/assets/img/tb-profiler_uml.svg" description="A UML schema of the pipeline" %}


# Documentation
To find out more about this tool please visit the [documentation page](https://jodyphelan.gitbook.io/tb-profiler/).

# Webserver
If you don't have access to a linux or macOS environment you can still use tb-profiler by using our webserver: [http://tbdr.lshtm.ac.uk/](http://tbdr.lshtm.ac.uk/).
You can upload your next generation sequencing data in fastQ format. When you upload your data, the run will be be assigned a unique ID. Please take a note of this ID as you will need to to find your results later. Batch upload of samples is also possible.

# Citation
If you plan to use TB-Profiler in your work please cite [this paper](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-019-0650-x) and include both the version of tb-profiler and the database.
