PI-Extract Dataset
=================

This repository contains the dataset and annotation guidelines of the following paper.

> Duc Bui, Kang G. Shin, Jong-Min Choi, and Junbum Shin, "Automated Extraction and Presentation of Data Practices in Privacy Policies," Proceedings on Privacy Enhancing Technologies (PETS), 2021.


## Dataset Description

The dataset contains privacy policy sentences with annotated data practices.
There are four types of data actions:

| Label       | Action performed on the data object            |
|-------------|------------------------------------------------|
| COLLECT     | Collected or used by the first party.          |
| SHARE       | Collected by a third party.                    |
| NOT_COLLECT | Not collected and not used by the first party. |
| NOT_SHARE   | Not collected by a third party.                |


`dataset` directory contains 4 directories for the 4 data-practice labels.
Each subdirectory contains 3 annotation files for `train`, `validation` and `test` splits.

The annotation files use the CoNLL-03 annotation format.
Each line contains four space-separated fields: the word, its part-of-speech (PoS) tag, its chunk tag 
and its entity tag.
Since we do not use the PoS and chunking information, these fields are empty.
The entities are encoded in the IOB scheme.


The annotation guidelines are provided in `annotation_guidelines.pdf`