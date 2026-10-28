# Task 02 — Database Search and Annotation

## Objective
Search a public sequence database, record the BLAST parameters, and interpret the best matches.

## Query
- Organism: *Bottlenose dolphin (tursiops truncatus*
- Accession Id:XP_004317908.1
- Query type: Protein 
- Program: BLASTP
- Database shown: core_nt

NCBI query record: https://www.ncbi.nlm.nih.gov/nuccore/LC481759.1  
NCBI BLAST: https://blast.ncbi.nlm.nih.gov/Blast.cgi

## Reproduce the search
1. Open the NCBI record above and choose FASTA.
2. Save the complete sequence in `sample.fasta`.
3. Open NCBI BLAST, select Protein BLAST (blstn)p and paste the sequence.
4. Run the search with the database you used.
5. Compare the live results with `annotation_table.csv` .
7. Download the full BLAST report and update `blast_results.txt`.

## Interpretation
Query cover shows how much of the query aligns. Percent identity shows the proportion of aligned positions that match. A very low E-value supports a statistically significant match. The top visible hit has 100% coverage and 100% identity, supporting an exact match across the reported alignment. Lower identities in other same-species records indicate sequence differences.

## Limitations
Hit values were transcribed from photos and must be verified against the live report. The complete query sequence is not included because it was not legible enough to transcribe from the photo. Download it from NCBI before submitting. Similarity supports sequence identification but does not alone prove every biological conclusion.
