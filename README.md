The CSV and pkl files contain the necessary data
to reproduce the plots and tables reported in "GALIC: Hybrid Multi-Qubitwise Pauli Grouping for Quantum Computing Measurement". 
## bias_fidelity.csv
Data for Figure 2 & 3 and Table 4. Note that we only collected fidelity data for the $H_4$, 
$H_6$, and $LiH$ for computational efficiency, missing values are denoted with -1. 

## h6_design_space_variance.csv
Data for Fig. 5

## h6_design_space_fermionic_adapt_bias.csv and h6_design_space_qubit_adapt_bias.csv
Data for Figs 6a and 6b.

## ibm_results_hartree_fock.pkl
Data for IBM Hartree-Fock sampling. The important fields for each scheme ("FC", "QWC", "HEC", "GALIC") can be described as follows:

* "results": a Qiskit BitArray containing the sampled results of a 600,000 shot-budget run.
* "partitions": a list of operator groups
* "circuits": a list of circuits diagonalizing the group, constructed using the CZ method from Crawford et al. 2021
* "rotations": a dictionary containing a mapping from operators to the diagonal basis
* "parity": a numpy array denoting the sign of each operator relative to its diagonalized counterpart: 1 for -1 and 0 for 1
