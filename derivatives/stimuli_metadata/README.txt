This is the README file for the BOLD Moments Dataset ./derivatives/stimuli_metadata folder.

Contents of this directory correspond to derivatives of the stimulus set, such as features, annotations, and frames.

frames_middle: Contains a .jpg file of the middle frame of each video. This middle frame was also used as model input for the frame annotations in "llm_frame_annotations.json".

ME_feats_matlab: Contains motion energy (ME) features of each video computed from the Matlab implementation of the motion energy model (https://github.com/gallantlab/motion_energy_matlab).

mp4_h264: The stimuli set reformatted into H.264 compressed .mp4 files. Mainly reformatted for convenience, this format is slightly more flexible across platforms for loading and viewing, such as if you wish to load the videos in a web browser for additional annotation experiments.

stimuli: The experimental stimuli set found in the root directory ./stimuli/test/ and ./stimuli/train/ folders copied over into one folder and renamed just to keep its video ID from 0001 - 1102.

annotations.json: metadata for the stimulus set.

annotations_filednames.json: Descriptions of metadata fields corresponding to the 'annotations.json' folder.

frames.zip: Contains each stimulus video's frames as a .jpg file. Useful for model inputs.

llm_frame_annotations.json: Contains five sentence text descriptions of just the middle frame of each video (from 'frames_middle' folder) generated by GIT model version git-large-coco (Wang et al., 2022).