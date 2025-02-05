## Phylogenetic Tree construction with FastTree & Tree visualization

Overview: 
input file in .afa format > FASTTREE > output file in .tre format for viewing in Tree Visualization software > .pdf file of your tree 

### Step 1: Installing the Tools
FastTree

    curl -O http://www.microbesonline.org/fasttree/FastTree.c
or 
    
    gcc -O3 -finline-functions -funroll-loops -Wall -o FastTree FastTree.c -lm

Figtree
http://tree.bio.ed.ac.uk/software/figtree/

### Step 2: Phylotree Building
1. Make sure you have your aligned sequences in one .afa file
2. Use the following command to create a phylogenetic tree file (in newick format with the .tre extension) using FastTree

        FastTree -nt -gtr -gamma alnd_seqs.fasta > tree.tre

3. At this point, you have your phylogenetic tree ready for viewing. You can use any tree viewing software (FigTree or even MEGA).

### Step 3: Viewing your Tree
1. Now that you have your .tre file, we can view them using FigTree.
2. 
