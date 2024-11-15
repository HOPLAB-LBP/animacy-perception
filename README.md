

[![DOI](https://zenodo.org/badge/700855057.svg)](https://doi.org/10.5281/zenodo.14165546)

# animacy-perception

This is the code for the paper "A computational deep learning investigation of animacy perception in the human brain", currently in revision.

The original code was developed by Stefanie Duyck and can be found [here](https://github.com/SDuyck/animacy-perception).

## How to use:
### Get the data
All datafiles needed to run the training or statistical analyses can be found [here](https://osf.io/7xcg9/).

*The .pth weight files consist of partial zip files, which need to be downloaded and put back together. 

HOW to Combine and Decompress the Parts:

1- When you want to reconstruct and decompress the original folder, first combine the parts:
bash
cat myfolder.tar.gz.part* > myfolder_combined.tar.gz

2- Then, decompress the combined file:
bash
tar xzvf myfolder_combined.tar.gz

### animacy-perception.ipynb
Script consists of 2 parts:
  - First part is to run the primary network training: Finetuning 'Animal bias'
  - Second part is to load a .pth weights file and to extract the image vectors from the output layer with the test set used in the paper

### Animacy-perception-statistics.ipynb
Script to redo all the analyses reported in the paper and to display the graphs.
