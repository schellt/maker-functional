# Adjustment of MAKER's functional annotation scripts

## Description
The [MAKER](https://www.yandell-lab.org/software/maker.html) scripts `maker_functional_gff`, `maker_functional_fasta` and `ipr_update_gff` are not compatible or don't use the full information provided with latest [Swiss-Prot's](https://www.uniprot.org/) `uniprot_sprot.fasta` and [InterProScan](https://github.com/ebi-pf-team/interproscan).

## Usage
There is no difference in usage to the original scripts.

## Changes
- `maker_functional_gff` and `maker_functional_fasta` now include the functions provided in the header of the Swiss-Prot's fasta file
- `ipr_update_gff` now includes the Reactome pathway informations, the date of the InterProScan analysis with the attribute `_IPRDate=`. The information from methods Seg, Coils, SignalPHMM, TMHMM, SignalP, Phobius and MobiDBLite are skipped.
