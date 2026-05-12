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

## Project Structure


neoantigen-pipeline/
│
├── src/
│   └── Peptide.py
├── input/
│   ├── proteinSeq.txt
│   └── mutationAAC.txt
├── output/
│   └── mutateseq.fsa
