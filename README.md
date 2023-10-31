# ESE-GB-DNN
# A dense Neural Network for evaluation of solvation free energies based on Generalized-Born terms

Introduction and User's Guide

ESE-EE-DNN is a method for evaluation of solvation free energies of molecules and ions [2]. It requires the solute molecular geometry and the total charge only. To obtain the solvation free energy, first electronegativity-equalization atomic charges are calculated. Subsequently, the solute van der Waals surface is constructed, and induced surface charges and the COSMO electrostatic energy are computed. The results, as well as three solvent features are fed into a Dense Neural Network that eventually yields the solvation free energy.

ESE-EE-DNN is an improved machine-learning adaptation of my ESE-EE scheme [3], which is in turn based on the uESE [3] and xESE [4] that we developed jointly with Alexander Voityuk.

The supported elements are H, C, N, O, F, Si, P, S, Cl, Br, I.

The ESE-EE-DNN solvation free energy can be calculated by the program ESE-EE-DNN, which can be downloaded here free of charge:

ESE-EE-DNN.exe – Windows version

ESE-EE-DNN.x – Linux version

The ESE-EE-DNN program can be run from the command line as follows:

ESE-EE-DNN.exe xyz-file -charge charge -solvent solvent

If your solvent is not in this list, you can use the following call format:

ESE-EE-DNN.exe xyz-file -charge 
charge -Eps dielectric_constant -BP boiling_point_°C -Nheavy  number_of_non_hydrogen_atoms_in_solvent

Once you use results calculated by the ESE-EE-DNN program, you should include at least the following citations:

1. S. F. Vyboishchikov, ESE-EE-DNN program, Girona, 2023

2. S. F. Vyboishchikov, J. Chem. Inf. Model.,2023, 63, in press. DOI: 10.1021/acs.jcim.3c00922

and preferably also cite our previous related work:

3. S. F. Vyboishchikov, J. Comput. Chem., 2023, 44, 307–318. DOI: 10.1002/jcc.26894

4. S. F. Vyboishchikov, A. A. Voityuk, Chemical Reactivity, vol. 2: Approaches and applications, S. Kaya, L. von Szentpály, G. Serdaroğlu, K. Guo (Eds.), Elsevier, Amsterdam, 2023, 399–427. DOI: 10.1016/B978-0-32-390259-5.00021-4

5. S. F. Vyboishchikov, A. A. Voityuk, J. Chem. Inf. Model., 2021, 61, 4544–4553. DOI: 10.1021/acs.jcim.1c00885

6. S. F. Vyboishchikov, A. A. Voityuk, J. Comput. Chem., 2021, 42, 1184–1194. DOI: 10.1002/jcc.26531

7. A. A. Voityuk, S. F. Vyboishchikov, Phys. Chem. Chem. Phys. 2020, 22, 14591–14598. DOI: 10.1039/d0cp02667k

8. A. A. Voityuk, S. F. Vyboishchikov, Phys. Chem. Chem. Phys., 2019, 21, 875–874. DOI: 10.1039/c9cp03010g

Questions related to the ESE-EE-DNN method and program should be addressed to Sergei Vyboishchikov.
