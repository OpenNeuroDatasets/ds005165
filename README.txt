README file for the Nifti folder in the BOLD Moments Dataset.

This folder contains the raw mri data converted to Nifti format and the experimental stimuli.

The file structure of this folder follows the BIDS format.
Repeated file structures are shown once and subsequently denoted with an elipses (e.g. ...) at the repeated level.

File Structure:
.
├── stimuli
│   ├── localizer
│   │   ├── Bodies
│   │   ├── Faces
│   │   ├── Objects
│   │   ├── Scenes
│   │   └── Scrambled15G
│   ├── test
│   └── train
├── sub-01
│   ├── ses-01
│   │   ├── anat
│   │   ├── fmap
│   │   └── func
│   ├── ses-02
│   │   ├── fmap
│   │   └── func
│   ├── ses-03
│   │   ├── fmap
│   │   └── func
│   ├── ses-04
│   │   ├── fmap
│   │   └── func
│   └── ses-05
│       ├── fmap
│       └── func
...
└── sub-10

Data collection notes:
All data collection notes explained below are detailed here for the purpose of full
transparency and should be of no concern to researchers using the data i.e. these
inconsistencies have been attended to and integrated into the BIDS format as if these
exceptions did not occur. The correct pairings between field maps and functional runs
are detailed in the .json sidecars accompanying each field map scan.

Subject 2:
Session 1: Subject repositioned head for comfort after the third resting state scan, 
approximately 1 hour into the session. New scout and field map scans were taken. 
In the case of applying a susceptibility distortion correction analysis, session 
1 therefore has two sets of field maps, denoted by “run-1” and “run-2” in the 
filename. The “IntendedFor” field in the field map’s identically named .json sidecar 
file specifies which functional scans correspond to which field map.

Session 4: Completed over two separate days due to subject feeling sleepy. All 3 
testing runs and 6/10 training runs were completed on the first day, and the last 
4 training runs were completed on the second day. Each of the two days for session 
4 had its own field map. This did not interfere with session 5. All scans across 
both days belonging to session 4 were analyzed as if they were collected on the same 
day. In the case of applying a susceptibility distortion correction analysis, session 
4 therefore has two sets of field maps, denoted by “run-1” and “run-2” in the filename. 
The “IntendedFor” field in the field map’s identically named .json sidecar file 
specifies which functional scans correspond to which field map.

Subject 4:
Sessions 1 and 2: The fifth (out of 5) localizer run from session 1 was completed at 
the end of session 2 due to a technical error. This localizer run therefore used the 
field map from session 2. In the case of applying a susceptibility distortion correction 
analysis, session 1 therefore has two sets of field maps, denoted by “run-1” and 
“run-2” in the filename. The “IntendedFor” field in the field map’s identically named 
.json sidecar file specifies which functional scans correspond to which field map. 

Subject 10:
Session 5: Subject moved a lot to readjust earplug after the third functional run (1 
test and 2 training runs completed). New field map scans were collected. In the case of
 applying a susceptibility distortion correction analysis, session 5 therefore has two 
sets of field maps, denoted by “run-1” and “run-2” in the filename. The “IntendedFor” 
field in the field map’s identically named .json sidecar file specifies which 
functional scans correspond to which field map.