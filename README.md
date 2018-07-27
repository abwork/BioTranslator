BioTranslator is a python script that puts together a collection of functions that can be used to translate DNA sequence (in fastafile format) into a protein sequence (in fastafile format).

HOW IT WORKS

The steps in the script are roughly the following:

Reads in the fasta file
Stores the sequences in a dictionary
Generates the six possible frames for each sequence (+1, +2, +3 and -1, -2, -3)
Swaps the DNA sequences for protein sequences
Finds the longest protein sequence between an open and close marker
Stores the longest protein sequence for each DNA sequence in a dictionary
Can save the protein sequences on a fasta file or print the sequences on the terminal

HOW TO USE

The script can be used by entering the following into the terminal:

$ python biotranslator.py -i dnasequences.fa -o proteinsequence.fa -p

N.B. Please substitute dnasequences.fa and proteinseqeuence.fa according to your filenames and paths.

Explanation of options:

-i (--ifile) must be followed by the fasta file
-o (--ofile) must be followed by the name where the protein sequences will be stored
-p is an option that allows printing the protein sequences on the terminal
-h prints a very simple help
