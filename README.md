Overview: 
input sequences > MAFFT/MUSCLE > FastTree > your chosen tree viewer > pdf figure

Reminder: Make sure you have your sequences saved into one input file in fasta format and named input_file.fasta
Example:
	>organism_1
	ATGCAGATGCGAGGTCGGAGAATTTCCGAGAT
	>organism_2
	AGATATTTAGGAATAGGACGATAAAGGCTAGA
	>organism_3
	AAAGGTTAAGCCCGTAGCCGATAGCCGAGATA
	

Step 1: Alignments

MAFFT
For MAFFT alignments, use the following code to run a quick alignment with automatic parameters.
		
  	mafft --auto input_file.fasta > alnd_seqs.afa

MUSCLE
For MUSCLE, use the following code to run a quick alignment with automatic parameters.

	muscle -align input_file.fasta -output alnd_seqs.afa

Step 2: Tree Construction

Use the following command to create a phylogenetic tree file (in newick format with the .tre extension) using FastTree

	FastTree -nt -gtr -gamma alnd_seqs.fasta > tree.tre
