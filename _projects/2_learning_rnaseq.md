---
layout: page
title: Learning RNA-seq
description: A concept-first curriculum, from what a transcriptome is to interpreting differential expression.
img:
importance: 2
category: teaching
---

Most RNA-seq tutorials teach the commands. A student who follows one can produce a
volcano plot and cannot tell you what the y-axis means, why the p-values were adjusted,
or whether the result is real. That student gets stuck the first time the data
misbehaves.

I wrote this to train an undergraduate summer student with a strong quantitative
background and no molecular biology. It is concept-first: the statistics come before the
code, and every plot is introduced by asking what it should look like if the experiment
worked, before producing it.

**What is in it**

- A concept-only slide deck covering what RNA-seq measures and why, from gene to
  transcriptome to counts to differential expression. No pipelines, no code to run yet.
- A prequel on what comes off a sequencer, how to read a FASTQ, what read QC catches, and
  how nf-core/rnaseq produces the count matrix everything else starts from.
- A standalone sandbox on simulated data for the hardest idea in the subject: what a
  p-value is, why twenty thousand tests break it, and what Benjamini-Hochberg does about
  that.

It worked with the student it was written for, so I rebuilt it on the public Bioconductor
`airway` dataset and released it. The count matrix is regenerated in the exact shape
nf-core emits, so a student who learns on it recognizes real pipeline output.

Code MIT, teaching material CC BY 4.0.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    <a href="https://github.com/julgrandvallet/learning-rnaseq" class="btn btn-primary">View on GitHub</a>
  </div>
</div>
