# Database Search and Annotation Using NCBI BLASTP

## 1. Aim
To compare an insulin protein query with protein database sequences using NCBI BLASTP and interpret sequence similarities.

## 2. Introduction
BLASTP compares a query amino-acid sequence against a protein database. It reports similar sequences with statistics such as query coverage, percent identity, E-value, alignment length, and gaps. These measures should be interpreted together.

## 3. Query details
- Intended query: insulin protein from the common bottlenose dolphin (*Tursiops truncatus*)
- Candidate accession selected earlier: XP_004317908.1
- Query type: protein
- Format: FASTA

**Required verification:** `data/sample.fasta` is a placeholder. Replace it with the exact query sequence used for the search and verify the accession and search settings.

## 4. Tools
- NCBI Protein database: https://www.ncbi.nlm.nih.gov/protein/
- NCBI BLAST: https://blast.ncbi.nlm.nih.gov/Blast.cgi

## 5. Method
1. Retrieve the intended protein record from NCBI in FASTA format.
2. Select Protein BLAST (BLASTP).
3. Paste the complete amino-acid FASTA record into the query field.
4. Select a suitable protein database and record the search settings.
5. Run the search and inspect the results table.
6. Record protein name, organism, accession, query coverage, identities, percent identity, E-value, and gaps.
7. Open representative alignments and interpret the matches.
8. Verify the exact query and full accession annotations before submission.

## 6. Results
 The gray whale insulin record (MBW01439.1) shows 100% query coverage, 105/110 identities (95.45%), no gaps, and an E-value of 4 × 10^-68. The bowhead whale insulin record (XP_061059793.1) also shows 100% coverage and 105/110 identities (95.45%), with an E-value of 1 × 10^-67. The beluga whale insulin isoform X2 record (XP_022446765.1) shows 100% coverage, 95/110 identities (86.36%), 12 gaps, and an E-value of 5 × 10^-59. The horseshoe bat insulin record (KAN3685427.1) shows 100% coverage, 98/110 identities (89.09%), no gaps, and an E-value of 2 × 10^-57.

See `results/annotation_table.csv` for the visible results and `results/blast_results.txt` for the transcription.

## 7. Discussion
The very small E-values indicate strong statistical evidence for sequence similarity. High query coverage means most or all of the query is represented in the alignment. Percent identity indicates exact amino-acid matches. Gaps may reflect insertions/deletions or sequence-length differences.

The top hit is annotated as gray whale insulin, not dolphin insulin. This is possible in a similarity search, but the exact query FASTA sequence and search parameters should be checked. The fifth hit is a partial hypothetical protein and should be interpreted cautiously.

## 8. Conclusion
The displayed BLASTP results show strong sequence similarity between the query and several insulin-related mammalian protein records. The gray whale and bowhead whale records each show 95.45% identity over 110 aligned positions and very small E-values. This demonstrates how sequence-search tools can identify similar proteins. A final biological conclusion should follow verification of the actual query sequence, search settings, and full database annotations.

## 9. References
1. NCBI Protein database: https://www.ncbi.nlm.nih.gov/protein/
2. NCBI BLAST: https://blast.ncbi.nlm.nih.gov/Blast.cgi
