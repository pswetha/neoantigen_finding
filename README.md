# neoantigen_finding
# Neoantigen Peptide Sequence Generator

A simple Python-based pipeline for generating wild-type (WT) and mutant-type (MT) peptide sequences from amino acid mutations.

This tool extracts 17-mer peptide sequences surrounding mutation positions and creates FASTA output for downstream neoantigen prediction workflows.

---

## Features

- Reads protein sequence input
- Reads amino acid mutation list
- Generates:
  - Wild-type peptide
  - Mutant peptide
- Produces FASTA formatted output
- Useful for neoantigen discovery pipelines

---



Input Files
1. Protein Sequence File

File: proteinSeq.txt

Example:
MKTIIALSYIFCLVFADYKDDDDK

2. Mutation File

File: mutationAAC.txt

Format:

A10T
Y15F
Meaning:

Mutation	Description
A10T	Alanine at position 10 changed to Threonine
Y15F	Tyrosine at position 15 changed to Phenylalanine
Output File

Generated File:
mutateseq.fsa
Example Output:
>WTA10T
LSYIFCLVFADYKDDDD

>MTA10T
LSYIFCLTFADYKDDDD
**How It Works**

The script:

Reads mutation positions
Extracts 17-mer peptide around mutation
Generates:
WT peptide
MT peptide
Writes sequences in FASTA format
**Run the Script**
</> Bash
python Peptide.py

**Applications**
Cancer Immunotherapy
Neoantigen Discovery
Personalized Vaccine Design
Tumor Mutation Analysis


**publication**
Analysis of Somatic Mutations in the TCGA-LIHC Whole Exome Sequence to Identify the Neoantigen for Immunotherapy in Hepatocellular Carcinoma
Pulakuntla Swetha Current Issues in Molecular Biology (2023) DOI: 10.3390/cimb46010009 


