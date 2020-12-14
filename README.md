PI-Extract Dataset
=================

This repository contains the dataset and annotation guidelines of the following paper.

> Duc Bui, Kang G. Shin, Jong-Min Choi, and Junbum Shin, "Automated Extraction and Presentation of Data Practices in Privacy Policies," Proceedings on Privacy Enhancing Technologies (PETS), 2021.


## Dataset Description

`dataset` contains 4 directories for the 4 data-practice labels.
Each directory contains 3 annotation files for `train`, `validation` and `test` splits.

The annotation files use the CoNLL-03 annotation format.
Each line contains four space-separated fields: the word, its part-of-speech (PoS) tag, its chunk tag 
and its entity tag.
Since we do not use the PoS and chunking information, these fields are empty.
The entities are encoded in the IOB scheme.


The annotation guidelines are provided in `annotation_guidelines.pdf`