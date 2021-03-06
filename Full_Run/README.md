# Summer_Project/Full_Run
Contains code and files for an example run to generate CG potentials for a system of 20Na+ ions.

File Types:
*.ipynb Jupyter notebook file, contains python code
*.mmol MagiC topology file (see /Other_Jupyter_Notebooks/Creating_Rdfs.ipynb to see creation)
*.mcm MagiC topology file, generated by rdf.py
*.inp MagiC rdf.py input file
*.rdf MagiC RDF file
*.pot MagiC potential file
*.in LAMMPS input file
*.table LAMMPS potential file
*.xtc LAMMPS trajectory file
*.png image files containing graphs

/LAMMPS_Inputs/
Contains the *.in input files used to run the simulations to generate the training data

/LAMMPS_Potentials/
Contains the *.table potential files used to run the simulations to generate the training data

/LAMMPS_Trajectories/
Contains the *.xtc trajectory files from the simulations run to generate the training data

/Magic_Potentials/
Contains the *.pot potential files used to run the simulations to generate the training data
Used as the outputs during the training of the network

/RDF_Inputs/
Contains the *.inp input files used to generate RDFs for training from the LAMMPS trajectories

/RDFs/
Contains the *.rdf RDF files generated from the LAMMPS trajectories
Used as the inputs during the training of the network

/Setup/
Contains files used to run initial simulation and generate initial RDFs. Potential is taken from
MagiC Tutorial 1 (Na-Cl)

/Test/
Contains the final output potential as well as files from simulation using that potential

/Model<>/
Each contains a trained network, with Model7 having the best performance

Full_Run.ipynb
Contains complete worked example

See Summer_Project/Project_Summary.pdf for overview on how the methodolgy works
