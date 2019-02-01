# PDB Nucleotide Mutator

This Python file exists to allow us to `make` tleap interpret nucleotides
of one type as another type, via changing some atom and residue names,
as well as deleting some lines, within the source PDB files.

This script is intentionally not generalizable, because different nucleotide
modifications require different line replacements, and PDB files themselves are
not always formatted the same way.

So, if you're using this, make sure you understand how it works first and
generate the appropriate parameters for `mutate_residue` by hand.
Then you should be golden.

## Usage

`python mutate_pdb_file.py [PDB_File_1]`

Or, if you want to do multiple PDB File mutations:

`python mutate_pdb_file.py [PDB_File_1] [PDB_File_2] ...`
