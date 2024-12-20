# Virus Taxonomy Classification with GeNomad

This project utilizes GeNomad, a tool designed to classify viral sequences based on taxonomy.

## Requirements

Before running this project, ensure that the following software is installed on your system:

- **GeNomad** (`genomad` tool, version 1.8.0) [Installation Instructions](https://github.com/virtool/genomad) for installation.
- **Python 3** (for further processing scripts, if necessary)
- A **Fasta file** of genomic sequences to be processed.

Also need access to the **GeNomad database** (v1.3 or higher).

## Installation

1. Install GeNomad (if not already installed):
   - Download the GeNomad tool and database.
   - Install according to the instructions in the [GeNomad Documentation](https://github.com/apcamargo/genomad).
2. Prepare Data:
   - Ensure you have a combined FASTA file (`combined.fasta`) containing the genomic sequences to process.

## Running GeNomad

Once GeNomad is installed, and your sequences are ready, run the following command to classify your sequences:

```bash
genomad end-to-end --cleanup --splits 8 combined.fasta genomad_output /work/groups/VEO/databases/geNomad/v1.3

## References

Camargo, A. P., Roux, S., Schulz, F., Babinski, M., Xu, Y., Hu, B., Chain, P. S. G., Nayfach, S., & Kyrpides, N. C. — Nature Biotechnology (2023), DOI: 10.1038/s41587-023-01953-y .
```