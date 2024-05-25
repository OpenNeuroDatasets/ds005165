README file for the ./derivatives/versionA/MNI152 folder in the BOLD Moments Dataset.

GLM: contains data pertaining to the General Linear Model computation.
GLM/ROIs: contains the ROI definitions for each subject and intermediate ROI definition calculations, such as probability maps, t-contrast probability maps, resliced atlases, and ROI masks for each subject as described in the ROI definition procedure in the manuscript.
GLM/betas-localizer: estimated the BOLD signal of the localizer experiment (session 1) using a canonical Hemodynamic Response Function model first smoothed with a 9mm kernel.
GLM/betas-mainexp/FIR_TRs_1_4: estimated TRs 1-4 of the main experiment's (sessions 2-5) BOLD signal using a Finite Impulse Response model with no smoothing applied.
GLM/betas-mainexp/FIR_TRs_5_9: estimated TRs 5-9 of the main experiment's (sessions 2-5) BOLD signal using a Finite Impulse Response model with no smoothing applied.
GLM/organized_betas: the beta value contents of "FIR_TRs_1_4" and "FIR_TRs_5_9" restructured into folders separated by subject, TR, and video. This was an intermediate formatting step to make the input of some analyses easier.

Repeated file structures are shown once and subsequently denoted with an elipses (...) at the repeated level.

Directory tree
.
├── GLM
│   ├── ROIs
│   │   ├── intermediate
│   │   ├── sub-01
│   │   ├── ...
│   │   └── sub-10
│   ├── betas-localizer
│   │ 	├── sub-01
│   │ 	│   	└── ses-01
│   │   │   		└── localizer
│   │ 	...
│   │ 	└── sub-10
│   ├── betas-mainexp
│   │   ├── FIR_TRs5_9
│   │	│   ├── sub-01
│   │	│   │   ├── ses-02
│   │	│   │   │   ├── test
│   │	│   │   │   └── train
│   │	│   │   ├── ses-03
│   │	│   │   │   ├── test
│   │	│   │   │   └── train
│   │	│   │   ├── ses-04
│   │	│   │   │   ├── test
│   │	│   │   │   └── train
│   │	│   │   └── ses-05
│   │	│   │       ├── test
│   │	│   │       └── train
│   │	│   ...
│   │	│   └── sub-10
│   │   └── FIR_TRs_1_4
│   │	    ├── sub-01
│   │	    │   ├── ses-02
│   │	    │   │   ├── test
│   │	    │   │   └── train
│   │	    │   ├── ses-03
│   │	    │   │   ├── test
│   │	    │   │   └── train
│   │	    │   ├── ses-04
│   │	    │   │   ├── test
│   │	    │   │   └── train
│   │	    │   └── ses-05
│   │	    │       ├── test
│   │	    │       └── train
│   │	    ...
│   │	    └── sub-10
│   └── organized_betas
│   	├── sub01
│   	│    ├── TR01
│   	│    │   ├── 0001
│   	│    │   ...
│   	│    │   └── 1102
│   	│	...
│   	│    └── TR09
│   	...
│   	└── sub10 
└── prepared_data
    ├── prepared_allvoxel_pkl
    │   ├── TR1
    │   ├── ...
    │   ├── TR9
    │   └── TRavg56789
    ├── prepared_reliable_pkl
    │   ├── TR1
    │   ├── ...
    │   ├── TR9
    │   └── TRavg56789
    └── prepared_searchlight_pkl

