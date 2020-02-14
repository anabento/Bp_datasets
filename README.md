# Bp-example-datasets
Bp isolate sequences for OR, NY and MN

SNPs were called in each state dataset separately (MN, NY, OR) – do you also need them combined? (it’s not hard). Alignments and trees also include “Reference” which matches Bp_C374_Illumina_final_ISmasked.fasta.
 
Bp-example-datasets.tsv -- Year of isolation, state, and public accession numbers
 
20191218-core-MN.full.biosample.0[1234].aln.gz – Full-length alignment (4.1 Mbp) with SNPs incorporated in to reference genome (C734) for each isolate.
 
20191219-core-MN.biosample.aln – Alignment of core variable positions only (see lengths below).
 
20191219-core-MN.biosample.fasttree.tre – Newick tree calculated from core variable positions, just for a quick snap shot of each dataset.
 
 
MN – 260 isolates – 360 variable sites
NY – 165 isolates – 313 variable sites
OR – 201 isolates – 254 variable sites

For each state dataset separately: (1) download alignments *.0[1234].aln.gz, (2) gunzip, (3) concatenate. Each ‘slice’ is an intact fasta alignment, so the order you recombine them doesn’t matter.
 
Also included are the variable-site only alignments and corresponding newick trees for context. SNPs were called as described in the msystems paper (in brief, read mapping to C734 via snippy v4 and the aligned ‘genomes’ are simply imputed from the reference)
