# CNV Scripts

This reposititory contains scustom cripts that were written to run Manta and to solve specific problems or specifc requirements that arose during CNV discovery and quality control.

## AF0.py

This script was used as part of the Manta QC filtering to remove variants that had allele frequencies =0 after individuals genotypes flagged wiith FAIL 1 2 or 3 had been set to missing.  

## ExHet_filtering.py

This script was used to remove variants that had excessive heterozygosity scores <1 x10e-15 

## Manta.config

Config file used during execution of the Manta nextflow pipeline. 

## Manta.nf

Nextflow pipeline used to execute Manta and Graphtyper. 

## StitchSiteFiltering.py

This script was used to produce the final Genome STRiP VCF from the matrix created during the merging, deduplication and stitching pipeline.

## mergeVCFs.sh

This script was used at multiple stages of execution of Genome STRiP, when step had to be run separately on each chromosome. The output files for each chromosome had to be merged before the next step could be executed. 

## remove_stutter.py

This was a script used to remove duplicate sites that were produced during SV genotyping due to an a error Genome STRiP SVGenotyper error. 
