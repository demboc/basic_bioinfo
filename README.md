## Sequence Alignments using MAFFT and MUSCLE CLIs and Phylogenetic Tree construction with FastTree

Overview: 
input sequences > MAFFT/MUSCLE > output file of your aligned sequence in .afa or .fasta extension

Reminder: Make sure you have your sequences saved into one input file in fasta format and named input_file.fasta

Example:  
	>organism_1
	ATGCAGATGCGAGGTCGGAGAATTTCCGAGAT  
	>organism_2
	AGATATTTAGGAATAGGACGATAAAGGCTAGA  
	>organism_3
	AAAGGTTAAGCCCGTAGCCGATAGCCGAGATA  

### MAFFT

For MAFFT alignments, use the following code to run a quick alignment with automatic parameters.
		
  	mafft --auto input_file.fasta > alnd_seqs.afa

### MUSCLE

For MUSCLE, use the following code to run a quick alignment with automatic parameters.

	muscle -align input_file.fasta -output alnd_seqs.afa

