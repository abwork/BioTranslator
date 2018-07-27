<strong>BioTranslator</strong> is a python script that puts together a collection of functions that can be used to translate DNA sequence (in fastafile format) into a protein sequence (in fastafile format).

<strong>HOW IT WORKS</strong>

The steps in the script are roughly the following:
<ol>
<li>Reads in the fasta file</li>
<li>Stores the sequences in a dictionary</li>
<li>Generates the six possible frames for each sequence (+1, +2, +3 and -1, -2, -3)</li>
<li>Swaps the DNA sequences for protein sequences</li>
<li>Finds the longest protein sequence between an open and close marker</li>
<li>Stores the longest protein sequence for each DNA sequence in a dictionary</li>
<li>Can save the protein sequences on a fasta file or print the sequences on the terminal</li>
</ol>

<strong>HOW TO USE</strong>

The script can be used by entering the following into the terminal:

<em>$ python biotranslator.py -i dnasequences.fa -o proteinsequence.fa -p</em>

N.B. Please substitute dnasequences.fa and proteinseqeuence.fa according to your filenames and paths.

<em>Explanation of options:</em>

<em>-i</em> (--ifile) must be followed by the fasta file <br>
<em>-o</em> (--ofile) must be followed by the name where the protein sequences will be stored<br>
<em>-p</em> is an option that allows printing the protein sequences on the terminal<br>
<em>-h</em> prints a very simple help<br>
