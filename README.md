# HADDOCK2.4 web server protocol data

This repository provides the data files for performing the HADDOCK2.4 web server protocols described in the following manuscript:

  * Honorato R.V., Giulini M., Reys V., Trellet M.E., Jiménez-García B., Schaarschmidt J.,  Koukos P.I., Rodrigues J.P.G.L.M., Karaca E., van Zundert, G., Roel-Touris J., van Noort, C.W., Jandová Z., Melquiond A.S.J. and Bonvin A.M.J.J.  The HADDOCK2.4 web server: A leap forward in integrative modelling of biomolecular complexes. _To be submitted_ (2023)


Input data, reference structures and HADDOCK parameter file (json) are provided for the following protocols:

1. Modeling of an antibody-antigen complexes using a priori NMR information	defining the epitope on the antigen and the knowledge of the hypervariable loops on the antibody
2. Coarse-grained protein docking on a nucleosome particle: PRC1 ubiquitination module bound to the Nucleosome

The content of the two directories is the following:

### antibody-antigen

  * _4G6K_clean.pdb_: HADDOCK-ready, pre-processed unbound form of the antibody
  * _4I1B_clean.pdb_: HADDOCK-ready, pre-processed unbound form of the antigen
  * _4G6M_clean.pdb_: Pre-processed reference structure of the complex to allow for easy comparison with the HADDOCK models
  * _job_params.json_: The HADDOCK2.4 server parameter file corresponding to the described protocol. This file can be used for direct submission to the [submit file](https://bianca.science.uu.nl/haddock2.4/submit_file) interface of the server.

A full run result page for this system is available at: https://wenmr.science.uu.nl/haddock2.4/result/4242424242/264063-Antibody-Antigen-NMR


### nucleosome

  * _4r8p_clean.pdb_: HADDOCK-ready, pre-processed nucleosome structure (bound form)
  * _3rpg_clean.pdb_: HADDOCK-ready, pre-processed unbound form of the PRC1 ubiquitination module
  * _4r8p_reference.pdb_: Pre-processed reference structure of the complex to allow for easy comparison with the HADDOCK models
  * _job_params.json_: The HADDOCK2.4 server parameter file corresponding to the described protocol. This file can be used for direct submission to the [submit file](https://bianca.science.uu.nl/haddock2.4/submit_file) interface of the server.
  * _histones-passive.list_: ASCII text file containing the list of solvent accessible residue on the nucleosme side used to define the passive residues for docking
  * _lys-cys-linkage.tbl_: CNS-formatted distance restraint file for the defineing the CYS (PRC1) to LYS (nucleosome) linkage (ambiguously defined to two LYS residues)

A full run result page for this system is available at: https://wenmr.science.uu.nl/haddock2.4/result/4242424242/264564-Nucleosome-Docking-CG


