[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.on007463-blue)](https://doi.org/10.82901/nemar.on007463)

This dataset consists of 8 participants completing functional localizer and movie-viewing tasks in both Very High Density Diffuse Optical Tomography (VHD-DOT) and fMRI. Sessions 1 and 2 for each subject include the VHD-DOT data in SNIRF format while sessions 3 or more include the fMRI data in NIFTI format. 

Preprocessed fMRI data used for comparisons to VHD-DOT are in the /derivatives folder and are in NIFTI format. 

More information on this data can be found here: 
Morgan Fogarty, Sean M. Rafferty, Zachary E. Markow, Anthony C. O’Sullivan, Calamity F. Svoboda, Tessa George, Kelsey King, Dana Wilhelm, Kalyan Tripathy, Emily M. Mugler, Stephanie Naufel, Allen Yin, Jason W. Trobaugh, Adam T. Eggebrecht, Edward J. Richter, Joseph P. Culver; Functional brain mapping using whole-head very high-density diffuse optical tomography. Imaging Neuroscience 2025; 3 IMAG.a.54. doi: https://doi.org/10.1162/IMAG.a.54

## Contributed notes (version 1.1.2)

- The SNIRF files store /nirs/probe/landmarkLabels as a 2-D (1, N) string array; SNIRF v1.1 specifies a 1-D string array, and MNE-Python 1.13 fails on the 2-D form, so the files do not open in MNE. The SNIRF files are unchanged in this version.
- The 11 channels.tsv files of sub-S06 are stored as annexed files (not as text in git); they are not changed in this version and still name both wavelengths of a channel S1-D1 (duplicate names).
