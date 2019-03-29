# Analysis and visualization of chromatin folding

<p>
<img align="right" src=/Documents/Logo/Foto-DNA_MMarti_0.jpg?raw=True>

- [Overview](#overview)
- [Material](#material)
- [Target Audience](#target-audience)
  - [Technical pre-requisites](#technical-pre-requisites)

## Overview

3C-based methods, such as Hi-C, produce a huge amount of raw data as pairs of DNA reads that are spatially close in the cell nucleus. Overall, these interaction matrices have been used to study how the genome folds within the nucleus, that is one of the most fascinating problems in modern biology. The rigorous analysis of the paired-reads using computational tools has been essential to fully exploit the experimental technique, and to study how the genome is folded in the space. Currently, there is a huge expansion on the wealth of data on genome structure with the availability of many datasets of Hi-C experiments down to 1 kb resolution (see for example: http://hic.umassmed.edu/welcome/welcome.php ; http://promoter.bx.psu.edu/hi-c/view.php or http://www.aidenlab.org/data.html ). 

This tutorial is about the use of TADbit, a software designed and developed to manage all the dimensionalities of the Hi-C data:
</p>

 - 1D - Map paired-end sequences to generate Hi-C interaction matrices
 - 2D - Normalize matrices and identify constitutive domains (compartments, TADs)
 - 3D - Generate populations of model structures which reproduce the Hi-C interaction matrices
 - 4D - Compare samples at different time points

## Material

| Core pipeline               | Annex                 |
|-------------------------|------------|
|<ul><li>[Hi-C Quality check](Notebooks/Methods-3-Hi-C%20quality%20check.ipynb)</li><li>[Mapping](Notebooks/Methods-4-Mapping.ipynb)</li><li>[Parsing mapped reads](Notebooks/Methods-5-Parsing%20mapped%20reads.ipynb)</li></ul> | <ul><li>[Software installation](Notebooks/Materials-2-Preparing%20your%20computer%20for%20the%20HiC%20data%20analysis.ipynb)</li><li>[Prepare reference genome](Notebooks/Methods-2-Preparation%20of%20the%20reference%20genome.ipynb)</li><li>[Design HiC experiment](Notebooks/Materials-1-Design%20of%20the%20HiC%20experiment.ipynb)</li><li>[Retrieve HiC dataset](Notebooks/Methods-1-Retrieve%20published%20HiC%20datasets.ipynb)</li></ul> |
| <ul><li>[Filterind reads](Notebooks/Methods-6-Filtering%20mapped%20reads.ipynb)</li><li>[Normalization](Notebooks/Methods-7-Bin%20filtering%20and%20normalization.ipynb)</li></ul> | <ul><li>[Compare/merge experiments](Notebooks/Methods-9-Compare%20and%20merge%20Hi-C%20experiments.ipynb)</li></ul> |
| <ul><li>[Compartments and TADs](Notebooks/Methods-8-Compartments%20and%20TADs%20detection.ipynb)</li></ul> |  |
| <ul><li>[Parameter optimization](Notebooks/Methods-10-Modeling%20parameters%20optimization.ipynb)</li><li>[Model optimization](Notebooks/Methods-11-3D%20Models%20production%20and%20analysis.ipynb)</li></ul> |  |

## Target Audience

The tutorial is designed for experimental researchers and bioinformaticians at the graduate and post-graduate levels which are interested in studying the genome spatial organization. 

### Technical pre-requisites

Recommended Linux and basic Python programming skills, graduate level in Life Sciences. All hands-on will be given at 3 levels of computational expertise (web platform, command-line tool and python scripting).
