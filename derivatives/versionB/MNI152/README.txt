README file for the ./derivatives/versionB/MNI152 folder in the BOLD Moments Dataset.

GLM: contains data pertaining to the General Linear Model computation.
GLM/mask: contains the group mask (voxels defined for all subjects) as well as each subject's mask. Useful for getting the affine transform.
GLM/parcels: contains the indices for all ROIs at a group level, before subject-specific definition of the categorical ROIs. Also has intermediate files for BMDgeneral definition and probability maps from the localizer.
GLM/sub-XX/ROIs: ROI indices for subject specific ROIs. These are identical to those in GLM/parcels/group_parcels except for the categorically selective ROIs.
GLM/sub-XX/prepared_betas: The subject's z-scored betas, noise ceilings, and localizer t-contrasts
GLM/sub-XX/ses-XX: the beta estimates and other output straight from GLMsingle.

prepared_allvoxel_pkl/sub-XX: For each subject, the z-scored beta values contained within the ROI.
prepared_searchlight_pkl: contains searchlight estimates and upper and lower noiseceilings across the whole brain.

