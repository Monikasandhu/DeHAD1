# Uploading Protein Sequences from Excel to FASTA Format using Python

## Overview
This Python script allows users to convert protein sequences stored in Excel files to FASTA format. The tool is designed for ease of use and can be particularly useful for researchers in the field of bioinformatics.

## Requirements
- Python 3.x
- `pandas` library
- `openpyxl` library (for reading Excel files)

## Installation
To install the required libraries, run the following command:
```bash
pip install pandas openpyxl
```

## Excel File Format
The Excel file should contain one column with the header 'Protein Sequence'. Each row below the header should contain a protein sequence.

Example:
| Protein Sequence |
|------------------|
| SEQUENCE1        |
| SEQUENCE2        |

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/Monikasandhu/DeHAD1.git
   cd DeHAD1
   ```
2. Run the script:
   ```bash
   python convert_to_fasta.py <path_to_excel_file> <output_fasta_file>
   ```
   - `<path_to_excel_file>`: Path to the input Excel file.
   - `<output_fasta_file>`: Name of the output FASTA file to be created.

## Example
```bash
python convert_to_fasta.py protein_sequences.xlsx output.fasta
```

## Output
The script will generate a FASTA file with the protein sequences, where each sequence is formatted as follows:
```
>ProteinID
SEQUENCE1
>ProteinID
SEQUENCE2
```

## Notes
- Ensure that the Excel file path is correct.
- The output will be saved in the same directory as the script unless a different path is specified.

## License
This project is licensed under the MIT License.