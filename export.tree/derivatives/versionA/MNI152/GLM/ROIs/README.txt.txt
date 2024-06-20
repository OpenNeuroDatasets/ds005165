README file for the ROIs folder in the BOLD Moments Dataset.
Since the file structure of subject directories repeats, we show the tree contents of only one subject (sub-01) to increase readability.

Each subject folder contains the file "sub-XX_masterMask_top1000.mat". The .mat file
contains a whole brain volume where each voxel takes on a value corresponding to one of 
the 22 ROIs. See the accompanying file "LUT_ROI_BMD.txt" for the ROI lookup table.

content:
.
├── intermediate
├── sub-01
├── sub-02
...
└── sub-10