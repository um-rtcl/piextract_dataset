PI-Extract Dataset
=================

## Research Paper
This repository contains the dataset and annotation guidelines of the following paper.

**Automated Extraction and Presentation of Data Practices in Privacy Policies** [[pdf]](https://rtcl.eecs.umich.edu/rtclweb/assets/publications/2021/pets21-duc.pdf)  
Duc Bui, Kang G. Shin, Jong-Min Choi, and Junbum Shin  
*Proceedings on Privacy Enhancing Technologies (PETS), 2021*

**Bibtex** entry:

```
@article{piextract_pets21,
  author = {Duc Bui and Kang G. Shin and Jong-Min Choi and Junbum Shin},
  doi = {doi:10.2478/popets-2021-0019},
  url = {https://doi.org/10.2478/popets-2021-0019},
  title = {Automated Extraction and Presentation of Data Practices in Privacy Policies},
  journal = {Proceedings on Privacy Enhancing Technologies},
  number = {2},
  volume = {2021},
  year = {2021},
  pages = {88--110}
}
```


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
Each subdirectory contains 2 annotation files for the `train` and `validation` splits.

The annotation files use the CoNLL-03 annotation format.
Each line contains four space-separated fields: the word, its part-of-speech (PoS) tag, its chunk tag 
and its entity tag.
Since we do not use the PoS and chunking information, these fields are empty.
The entities are encoded in the IOB scheme.


The annotation guidelines are provided in `annotation_guidelines.pdf`
