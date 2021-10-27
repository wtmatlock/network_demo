# Genomic Network Demo

## Set up

1) Download software:
  - Cytoscape: https://cytoscape.org/download-platforms.html
  - Mash: `conda install -c bioconda mash` \
  Check things are working with `mash --help`

2) Download data:
- `scp -r abc123@rescomp1.well.ox.ac.uk:"/well/bag/fnd111/network_demo" ./` \
This directory contains 100 .fsa plasmid genomes, and 2 .tsv metadata files.

## Generating Mash edgelist

1) `cd ./network_demo`

2) `cat ./*.fsa > ./plasmids.fsa`

3) `mash triangle -E ./plasmids.fsa > ./edgelist.tsv`



