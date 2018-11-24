---
layout: post
title:  "Tripal BLAST UI"
img: blast_ui_submission.png
github: https://github.com/tripal/tripal_blast
zenodo_badge:
zenodo_url:
see_live: http://knowpulse.usask.ca/portal/blast/nucleotide/nucleotide
---

* Provides a simple UI for users to run NCBI BLAST through a Tripal site.
* Ideal for providing organism-specific BLAST services.

Specifically it provides blast program-specific forms (blastn, blastp, tblastn, blastx are supported). In the future, there will be a single form where you will be able to select either a nucleotide or a protein database to BLAST against regardless of the type of query and it will decide which BLAST program to use based on the combination of query/database type (ie: if you selected a protein database on the nucleotide BLAST form then blastx would be used).

BLAST submissions result in the creation of Tripal jobs which then need to run from the command-line. This ensures that long running BLASTs will not cause page time-outs but does add some management overhead and might result in longer waits for users depending on how often you have cron set to run Tripal jobs. You can alternatively use the Tripal Jobs Daemon to automate running of Tripal Jobs reducing user wait time and your own workload.

The BLAST results page is an expandable summary table with each hit being listed as a row in the table with query/hit/e-value information. The row can then be expanded to include additional information including the alignment. Download formats are allow users to download these results in the familiar tabular, GFF3 or HTML NCBI formats.
