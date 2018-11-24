Hello!   This is the code repository for the [Our Tripal module showcase site](https://uofs-pulse-binfo.github.io/our-modules/)!  This site showcases Tripal modules developed by the University of Saskatchewan, Pulse Bioinformatics group and in use at [KnowPulse](http://knowpulse.usask.ca/portal).  Our hope is that you'll consider trying out our modules and collaborating with us!


### Setting up your own site

You can use this repo as a template for your own show case site!

* Clone the repository
* Post modules in the `_posts` folder.  See below for format.
* Change variables in `_config.yml`.  In particular set the URL and base URL to your github pages location.
* install [jekyll](https://jekyllrb.com/docs/installation/).
* run `jekyll serve` to test your site.
* build with `jekyll build`, and push to your repository.
* Configure [github pages](https://pages.github.com/)  for your repo.  This site builds to `_site/` (which is ignored in `.gitignor)`, and Github automatically builds on commit.


### post format
The below file is an example post.

```
---
layout: post
title:  "Tripal BLAST UI"
img: blast_ui_submission.png
homepage: https://www.drupal.org/project/tripal_blast
github: https://github.com/tripal/tripal_blast
zenodo_badge:
zenodo_url:
see_live: http://knowpulse.usask.ca/portal/blast/nucleotide/nucleotide
---

* Provides a simple UI for users to run NCBI BLAST through a Tripal site.
* Ideal for providing organism-specific BLAST services.

```
