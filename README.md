# mrn_simulator_releases
Executables of the Mott Resistor Network Simulator

The executables have been tested on a clean Ubuntu 20.04 LTS installation.
The packet libumfpack5 must be installed first. 

To run the simulation, execute the batch file ./startProgram. Alternatively, execute the file resistorNetwork2D in the bin folder, passing as 1st argument the path to the
input file, and as 2nd argument the path to the output file.

Several files are generated for each run: 

1) t_I_V_R contains, from left to right, the time-step of the simulation, the current that flows through the sample, the voltage of the sample and its resistance
2) temp_map contains n matrixes, where n is the length of the simulation. Each matrix is of size L x W (length per width of the sample) and each element is the temperature of the cell normalized by the transition temperature (340)
3) metallic_fraction contains a matrix of size W x n, each cell represents the metallic fraction for the corresponding column of the sample

Since GitHub doesn't allow to upload files greater than 25 MB, I haven't uploaded the whole temp_map files, but only the snapshots close to the transition. These can be found in the temp_map subfolders inside output_files
