README file for the ./derivatives/versionA/MNI152/prepared_data folder in the BOLD Moments Dataset.

This folder contains prepared fmri data used for subsequent analyses.

"prepared_allvoxel_pkl" contains the fMRI beta estimates in a dictionary format at all voxels. The data is organized by TR as well as values for averaged TRs 5-9. The "TRavg56789" is the recommended data to use unless you specifically want to use estimates at different TRs in your analysis.
"prepared_reliable_pkl" contains the contents of "prepared_allvoxel_pkl" but after split-half reliability analysis to identify reliable voxels for each subject.
"prepared_searchlight_pkl" contains searchlight results on the testing set for each subject and upper and lower noise ceilings.

Directory tree
.
├── prepared_allvoxel_pkl
│   ├── TR1
│   ├── TR2
│   ├── TR3
│   ├── TR4
│   ├── TR5
│   ├── TR6
│   ├── TR7
│   ├── TR8
│   ├── TR9
│   └── TRavg56789
├── prepared_reliable_pkl
│   ├── TR1
│   ├── TR2
│   ├── TR3
│   ├── TR4
│   ├── TR5
│   ├── TR6
│   ├── TR7
│   ├── TR8
│   ├── TR9
│   └── TRavg56789
└── prepared_searchlight_pkl
