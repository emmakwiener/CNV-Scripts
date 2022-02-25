# CNV Variant set and Scripts

This repository contains the intersection variant call set data as well as custom scripts. Scripts include those that were written to run Manta and to solve specific problems or specifc requirements that arose during CNV discovery and quality control.

## AF0.py

This script was used as part of the Manta QC filtering to remove variants that had allele frequencies =0 after individuals genotypes flagged with a FAIL 1 2 or 3 had been set to missing.  

## ExHet_filtering.py

This script was used to remove variants that had excessive heterozygosity scores <1 x10e-15 

## Manta.config

Config file used during execution of the Manta nextflow pipeline. 

## Manta.nf

Nextflow pipeline written to execute Manta and Graphtyper. 

## StitchSiteFiltering.py

This script was used to produce the final Genome STRiP VCF from the matrix created during the merging, deduplication and stitching pipeline.

## mergeVCFs.sh

This script was used at multiple stages of execution of Genome STRiP, whenever a step had to be run separately on each chromosome. The output files for each chromosome had to be merged before the next step could be executed. 

## remove_stutter.py

This was a script used to remove duplicate sites that were produced during SVgenotyping due to a issue encountered wihen running Genome STRiP SVGenotyper. 

## Intersection Variant Dataset

The intersecting variant call set comprised of 9001 variants called by both Manta and Genome STRiP
