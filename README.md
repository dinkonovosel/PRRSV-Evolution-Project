# PRRSV-Evolution-Project — reproducibility materials

This repository provides scripts, configuration files, and derived datasets used in the manuscript:
"Intensive industrial farming structures reticulate viral evolution through sustained population overlap".


## What this repository contains
- **Scripts and configuration files** used to run the analyses: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Scripts]`
- **Input files** for each analysis step (alignments/metadata): `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Sequences)
- **Derived datasets**: codon-aligned FASTA files and alignments masked/filtered after removal of recombinant and/or selected regions

## Important note about software
This study does not provide a new standalone software package. Analyses rely on established third-party tools
(MAFFT, 3SEQ, RDP5, HyPhy, BEAST, HybridCheck, Dsuite, ARGweaver-D) plus R scripts.
Each tool has its own installation instructions; links are listed below.

## System requirements
### Operating systems tested
- macOS
- Linux (Ubuntu)

### Third-party software used
- 3SEQ (https://github.com/olli0601/3SEQ)
- RDP5 (https://web.cbio.uct.ac.za/~darren/rdp.html)
- HyPhy (https://hyphy.org)
- BEAST (https://beast.community)
- HybridCheck (https://github.com/vanOosterhoutLab/HybridCheck)
- Dsuite (https://github.com/millanek/Dsuite)
- ARGweaver-D (https://github.com/CshlSiepelLab/argweaver-d-analysis)
- Generax (https://github.com/BenoitMorel/GeneRax)
- ThirdKind (https://github.com/simonpenel/thirdkind)

### Hardware
No non-standard hardware is required for the demo. Full BEAST analyses may benefit from multi-core CPU/HPC.

## Installation
Install the third-party tools following their official documentation.
R packages required for plotting/summary are listed in: `[path/to/R_requirements_or_script_header]`.

Typical installation time on a normal desktop computer: **~15–30 min** (excluding optional tools such as BEAST/RDP5).

## How to run (overview)
Analyses are organized by step; each step has an input file and a corresponding script/config:
- Alignment: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Sequences)
- Recombination detection: [https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Recombination)
- Introgression: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Introgression)
- Selection-aware filtering: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Selection)
- Bayesian phylogenetics: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Phylogeny)
- Summary/plots: `[https://github.com/dinkonovosel/PRRSV-Evolution-Project/tree/main/Scripts)

## Demo
Demo data: 
Run:
- exact command are given in input files for each software

Expected output:
- `for each calculation was give output file together with input file in the same .zip folder

Expected runtime:
- **depends form ~2–10 minutes for the most of softwares while for BEAST, ARGweaver, SBP could be 2 weeks on multi-core CPU/HPC.

## Data availability
No new raw sequencing reads were generated. All analysed sequences are publicly available from NCBI GenBank;
GenBank accession numbers are included in the taxon labels.

Derived alignments used for analyses are provided in Alignments.
