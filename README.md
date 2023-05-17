# MMASD-A-Multimodal-Dataset-for-Autism-Intervention-Analysis

This is the repository for MMASD: A Multimodal Dataset for Autism Intervention Analysis.

We presents a novel privacy-preserving open-source dataset, MMASD as a Multi Modal ASD benchmark dataset, collected from play therapy interventions of children with Autism. 
MMASD includes data from 32 children with ASD, and 1,315 data samples segmented from over 100 hours of intervention recordings. 
It consists of four privacy-preserving modalities of data: 
- (1) Optical flow: derived from raw RGB video, for each frame, we have **_x.jpg and **_y.jpg, representing the movement in x and y axis, respectively
- (2) 2D skeleton: generated via OpenPose, 25 body keypoints
- (3) 3D skeleton: generated via Regression of Multiple 3D People (ROMP), 71 body keypoints
- (4) Clinician ASD evaluation scores of children, such as ADOS scores.

Due to the file size limit, we have uploaded the data to google drive, which can be easily accessed at https://tinyurl.com/mr3rd2dp.

We presented sample files for in each modality under "sample_data" folder. 

# Reference:

OpenPose: https://github.com/CMU-Perceptual-Computing-Lab/openpose

ROMP: https://github.com/Arthur151/ROMP
