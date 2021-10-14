# Genomic Network Demo

## Set up

1) Download software:
  - Cytoscape: https://cytoscape.org/download-platforms.html
  - Mash: `conda install -c bioconda mash` \
  Check things are working with `mash --help`

2) Download data:
- `scp -r abc123@rescomp1.well.ox.ac.uk:"/well/bag/fnd111/network_demo" ./` \
This directory contains 100 .fsa plasmid genomes, and 3 .tsv metadata files.

## Generating Mash edgelist

1) `cat ./*.fsa > ./plasmids.fsa`

2) `mash triangle -E ./plasmids.fsa > ./edgelist.tsv`



