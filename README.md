## Sequence Alignments using MAFFT and MUSCLE CLIs and Phylogenetic Tree construction with FastTree

Overview: 
input file in .fasta extension > MAFFT/MUSCLE > output file of your aligned sequence in .afa or .fasta extension

Reminder: Make sure you have your sequences are saved into one input file in fasta format and saved in .fasta extension

More information on [FASTA formats](https://en.wikipedia.org/wiki/FASTA_format)  

How your sequences should look in your input file:  
	>organism_1
	ATGCAGATGCGAGGTCGGAGAATTTCCGAGAT  
	>organism_2
	AGATATTTAGGAATAGGACGATAAAGGCTAGA  
	>organism_3
	AAAGGTTAAGCCCGTAGCCGATAGCCGAGATA  

### Step 1: Installing the Tools  
MAFFT
1. On the Ubuntu window, run the command below to download MAFFT
> wget https://mafft.cbrc.jp/alignment/software/mafft_7.526-1_amd64.deb
2. Install the package
> sudo dpkg -i mafft_7.526-1_amd64.deb
3. Check the location and version of MAFFT
> which mafft
> mafft --version

MUSCLE
1. Go to [MUSCLE](https://www.drive5.com/muscle/manual/install.html) to download the binary file. 
2. Follow the instructions, essentially "To install it, all you do is download or copy the binary to a directory that is accessible from the computer where you want to run the code. For convenience, you may want to rename the binary file to muscle to avoid typing long names like muscle3.8.98_i86linux32."


### Step 2: Alignments  
MAFFT

For MAFFT alignments, use the following code to run a quick alignment with automatic parameters.
		
  	mafft --auto input_file.fasta > alnd_seqs.afa  

MUSCLE

For MUSCLE, use the following code to run a quick alignment with automatic parameters.

	muscle -align input_file.fasta -output alnd_seqs.afa

