---
layout: about
title: about
permalink: /
subtitle: Cancer genomics, epigenomics, and pipelines that can be checked.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Division of Hematology, Oncology and Bone Marrow Transplant</p>
    <p>University of Colorado</p>
    <p>Anschutz Medical Campus</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a bioinformatics analyst at the University of Colorado Anschutz Medical Campus,
embedded in a multi-PI shared resource in the Department of Pediatrics. My work runs
across germline and somatic variant analysis, bulk and single-cell RNA-seq, ATAC-seq
and CUT&RUN, applied mostly to childhood leukemia, neuro-oncology and cancer evolution.

Most of what I do is building analysis that other people can rely on and reproduce.
That means containerized Nextflow pipelines on HPC for six laboratories, written records
of the decisions behind duplicate handling and normalization and filtering, and where it
matters, a second independent implementation to check the first one. A recent benchmark
found that the standard normalization method reports a real fourfold loss of signal as a
significant gain, which is the kind of result you only find if you go looking.

I work in R and Python, on nf-core and Nextflow, in the Bioconductor and tidyverse
ecosystems. I also teach: an asynchronous R course for researchers, four mentored trainees,
and an invited faculty workshop at AACR on using large language models for scientific
programming.

Co-author on work in the *New England Journal of Medicine*, *Leukemia*, *EBioMedicine*,
*Brain Pathology* and *Blood*. Originally from Mexico City, currently in Colorado, and
happy to hear from people working on genomics anywhere.
