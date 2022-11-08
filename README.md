# RCFV_Reader
RCFV Reader is a new software to quickly calculate normalised relative compositional frequency variability.
==================================================================================================================================================================
INSTALLATION
In addition to perl, RCFV Reader uses the cpan module FAST::Bio::SeqIO
You can install this module using:

cpanm FAST::Bio

If you don't have cpan, you can get it here:
https://www.cpan.org/
It's a really useful way to get access to a whole range of accessible modules for perl

==================================================================================================================================================================
RCFV Reader, James F. Fleming & Torsten H Struck, 2022.
Welcome to RCFV Reader. RCFV Reader accepts FASTA files as input, and then outputs 6 files.
To run RCFV Reader on nucleotide data, input the command as follows:

perl RCFVReader.pl dna <filename> <prefix for output files>

for amino acid data, input the command like this:

perl RCFVReader.pl protein <filename> <prefix for output files>

the 6 output files are:
- RCFV.txt - this file contains the total RCFV and nRCFV of the entire dataset.
- csRCFV.txt - this file contains a list of the character-specific RCFVs of your input dataset
- ncsRCFV.txt - as per csRCFV.txt, but with ncsRCFV values
- tRCFV.txt - this file contains a list of the taxon-specific RCFVs of your input dataset
- ntRCFV.txt - as per tRCFV.txt, but with ntRCFV values
- Frequencies.txt - this file contains the per taxon character frequencies, and the mean per taxon character frequencies across the dataset (as used by RCFV, NOT the total dataset character frequencies)

I hope you enjoy this fast new way to use normalised Relative Composition Frequency Variability! If you have any questions or queries, or notice any bugs, contact me at:
j.f.fleming\@nhm.uio.no
==================================================================================================================================================================

