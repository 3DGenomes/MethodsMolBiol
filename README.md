# Analysis and visualization of chromatin folding

<p>
<img align="right" src=/Documents/Logo/Foto-DNA_MMarti_0.jpg?raw=True>

- [Overview](#overview)
- [Target Audience](#target-audience)
  - [Technical pre-requisites](#technical-pre-requisites)
    - [TADbit API](#tadbit-api)
- [Course material](#course-material)

## Overview

3C-based methods, such as Hi-C, produce a huge amount of raw data as pairs of DNA reads that are spatially close in the cell nucleus. Overall, these interaction matrices have been used to study how the genome folds within the nucleus, that is one of the most fascinating problems in modern biology. The rigorous analysis of the paired-reads using computational tools has been essential to fully exploit the experimental technique, and to study how the genome is folded in the space. Currently, there is a huge expansion on the wealth of data on genome structure with the availability of many datasets of Hi-C experiments down to 1 kb resolution (see for example: http://hic.umassmed.edu/welcome/welcome.php ; http://promoter.bx.psu.edu/hi-c/view.php or http://www.aidenlab.org/data.html ). In this course, participants will learn to use TADbit, a software designed and developed to manage all the dimensionalities of the Hi-C data:
</p>

 - 1D - Map paired-end sequences to generate Hi-C interaction matrices
 - 2D - Normalize matrices and identify constitutive domains (compartments, TADs)
 - 3D - Generate populations of model structures which reproduce the Hi-C interaction matrices
 - 4D - Compare samples at different time points

Participants can bring specific biological questions and/or their own 3C data to analyze during the course. At the end of the course, participants will be familiar with the TADbit software, and will be able to fully analyze Hi-C data. *Note: Although the TADbit software is central in this course, alternative software will be discussed for each part of the analysis.*

## Target Audience

The course is designed for experimental researchers and bioinformaticians at the graduate and post-graduate levels which are interested in studying the genome spatial organization. 

It is likely that the participants to this course aim at getting involved in generating Hi-C data for  chromosome structure determination, or that they just want to be able to correctly interpret and analyse publicly available data.

### Technical pre-requisites

Recommended Linux and basic Python programming skills, graduate level in Life Sciences. All hands-on will be given at 3 levels of computational expertise (web platform, command-line tool and python scripting).

#### TADbit API

This tutorial is associated with a __specific version of TADbit__, if you wish to reproduce exactly the results in the notebooks you should use the version of TADbit tagged `3DAROC_2018`.

To install this version do:

    git clone https://github.com/3dgenomes/tadbit
    cd tadbit
    git checkout tags/3DAROC_2018
    sudo python setup.py install

## Material

|                  | Lectures (pdf)                          | Core pipeline (notebooks)               | Annex (notebooks)                 |
|-------------------|----------------|-------------------------|------------|
| Day1 | <ul><li>[Welcome](/Presentations/Day1/01_20180917_Welcome.pdf)</li><li>[Intro structure determination](/Presentations/Day1/02_20180917_introduction_to_structure_determination.pdf)</li><li>[3D Genomes overview](/Presentations/Day1/03_20180917_3D-genomes_overview.pdf)</li><li>[Intro TADbit](/Presentations/Day1/04_20180917_Intro_TADbit.pdf)</li><li>[NGS for HiC](/Presentations/Day1/05_20180917_NGS_for_HiC.pdf)</li><li>[Intro UNIX](/Presentations/Day1/06_20180917_linux.pdf)</li><li>[Intro Python](/Presentations/Day1/07_20180917_python.pdf)</ul></li> |<ul><li>[Hi-C Quality check](/Notebooks/00-Hi-C%20quality%20check.ipynb)</li><li>[Mapping](/Notebooks/01-Mapping.ipynb)</li><li>[Parsing mapped reads](/Notebooks/02-Parsing%20mapped%20reads.ipynb)</li></ul> | <ul><li>[Software installation](/Notebooks/A0-Preparing%20your%20computer%20for%20HiC%20data%20analysis.ipynb)</li><li>[Prepare reference genome](/Notebooks/A1-Preparation%20reference%20genome.ipynb)</li><li>[Download Hi-C experiment](/Notebooks/A2-Download%20published%20Hi-C%20experiments.ipynb)</li></ul> |
| Day2 | <ul><li>[Morning wrap up](/Presentations/Day2/01_20180918_Summary_of_day_1.pdf)</li><li>[Chromatin and 3Cs](/Presentations/Day2/02_20180918_Chromatin_and_3Cs.pdf)</li><li>[TADbit](/Presentations/Day2/03_20180918_TADbit.pdf)</li><li>[Applications (I): Caulobacter](/Presentations/Day2/04_20180918_Applications(II)_Caulobacter.pdf)</li></ul>| <ul><li>[Filterind reads](/Notebooks/03-Filtering%20mapped%20reads.ipynb)</li><li>[Normalization](Notebooks/04-Bin-filtering%20and%20normalization.ipynb)</li></ul> | <ul><li>[Compare/merge experiments](/Notebooks/A3-Compare%20and%20merge%20Hi-C%20experiments.ipynb)</li></ul> |
| Day3 | <ul><li>[Morning wrap up](/Presentations/Day3/01_20180919_Summary_of_day_2.pdf)</li><li>[Applications(II) TAD hormone](/Presentations/Day3/02_20180919_Applications(II)_TAD_hormone.pdf)</li><li>[Applications (III) SOX2 Dynamics](/Presentations/Day3/02_20180920_Applications(IIIa)_SOX2Dynamics.pdf)</li></ul>| <ul><li>[Compartments and TADs](/Notebooks/05-Compartments%20and%20TADs.ipynb)</li></ul> | <ul><li>[Align and compare TADs](/Notebooks/A4-Align%20and%20compare%20TADs.ipynb)</li></ul> |
| Day4 | <ul><li>[Morning wrap up](/Presentations/Day4/01_20180920_Summary_of_day_3.pdf)</li><li>[Applications(IV): Super-resolution Imaging and modeling](/Presentations/Day4/03_20180920_Applications(IIIb)_IMGR.pdf)</li></ul>| <ul><li>[Parameter optimization](/Notebooks/06a-Modeling%20-%20parameter%20optimization.ipynb)</li><li>[Model optimization](/Notebooks/06b-Modeling%20-%20model%20optimization.ipynb)</li></ul> | <ul><li>[Analysis of 3D models](/Notebooks/A5-Modeling%20-%20analysis%20of%203D%20models.ipynb)</li></ul> |
| Day5 | <ul><li>[Morning wrap up](/Presentations/Day5/01_20180921_Summary_of_day_4.pdf)</li><li>[Multiscale Genomics](/Presentations/Day5/02_20180921_MuG.pdf)</li><li>[Nucleosome dynamics](/Presentations/Day5/NucDyn_3DAROC18.pdf)</li><li>[MC-DNA and Chromatin Dynamics](/Presentations/Day5/3DAROC_mcdna_chromdyn_juergenwalther_21_09_18.pdf)</li></ul> |  |
