---
layout: page
title: CUT&RUN normalization benchmark
description: Which correction recovers a genome-wide change in signal, and which one hides it?
img:
importance: 1
category: software
---

Differential binding analysis assumes most regions do not change. Library-size
normalization is built on that assumption: it scales samples so the bulk of regions sits
at a log fold-change of zero.

When a treatment changes signal genome-wide, that assumption fails in a specific and
dangerous way. The method cannot represent "everything went down", so it reports the
global shift as noise and returns a symmetric, zero-centred result that looks entirely
reasonable.

This pipeline measures how much that costs. Every method under test consumes the same
consensus regions and the same count matrix, so any difference in the result is
attributable to normalization and nothing else.

**Validated on simulated data with a planted ground truth.** Spike-in normalization
recovers a true fourfold loss at 98% directional purity. Library-size normalization
reports that same loss as a significant *gain* at 480 regions: the wrong sign, with high
confidence.

It also enforces an engine parameterization that is easy to get silently wrong. edgeR
normalization factors scale library size; DESeq2 size factors are already the complete
scaling. Multiplying the latter by library size counts depth twice, which in earlier work
manufactured a 40% discrepancy between two engines that in fact agreed. The pipeline
asserts the two effective scalings match and stops if they do not.

Nextflow DSL2, with Docker, Singularity and SLURM profiles. Self-checking analysis
scripts and continuous integration on every commit.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    <a href="https://github.com/julgrandvallet/cutandrun-normalization-benchmark" class="btn btn-primary">View on GitHub</a>
  </div>
</div>
