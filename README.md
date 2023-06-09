# MMASD-A-Multimodal-Dataset-for-Autism-Intervention-Analysis

This is the repository for MMASD: A Multimodal Dataset for Autism Intervention Analysis. Dataset can be accessed at https://tinyurl.com/mr3rd2dp.

<!-- ![selected scenes](./sample_data/Activities.jpg) -->

#### Theme 1 -- Robotic-assisted therapy: Arm Swing, Body Swing, Chest Expansion, Squat
<img src="sample_data/Low_Resolution_Images/as_40533_D8_001_i.gif" alt="Alt Text 1" width="200"> <img src="sample_data/Low_Resolution_Images/bs_20594_D1_001_y.gif" alt="Alt Text 2" width="200" > <img src="sample_data/Low_Resolution_Images/ce_40753_D16_000_i.gif" alt="Alt Text 3" width="200" > <img src="sample_data/Low_Resolution_Images/sq_40023_D8_001_i.gif" alt="Alt Text 4" width="200" >

#### Theme 2 -- Rhythm: Drumming, Maracas Forward Shaking, Maracas Shaking, Sing and Clap
<img src="sample_data/Low_Resolution_Images/dr_40493_D16_023_n.gif" alt="Alt Text 5" width="200" > <img src="sample_data/Low_Resolution_Images/mfs_40743_D1_001_y.gif" alt="Alt Text 6" width="200" > <img src="sample_data/Low_Resolution_Images/ms_40143_D8_007_y.gif" alt="Alt Text 7" width="200" > <img src="sample_data/Low_Resolution_Images/sac_40683_D1_000_y.gif" alt="Alt Text 8" width="200" >

#### Theme 3 -- Yoga: Frog Pose, Tree Pose, Twist Pose
<img src="sample_data/Low_Resolution_Images/fg_41093_D8_009_y.gif" alt="Alt Text 9" width="200" > <img src="sample_data/Low_Resolution_Images/tr_41063_D8_011_y.gif" alt="Alt Text 10" width="200" > <img src="sample_data/Low_Resolution_Images/tw_41113_D1_010_y.gif" alt="twist pose" width="200" >

We presents a novel privacy-preserving open-source dataset, MMASD as a Multi Modal ASD benchmark dataset, collected from play therapy interventions of children with Autism. 
MMASD includes data from 32 children with ASD, and 1,315 data samples segmented from over 100 hours of intervention recordings.
It covers 11 different activities in 3 themes, and consists of four privacy-preserving modalities of data: 

![4 different modalities](./sample_data/Teaser.jpg)

1) Optical flow: derived from raw RGB video, for each frame, we have **_x.jpg and **_y.jpg, representing the horizontal and vertical components, respectively. Note originally optical flow is saved as .npy files, but due to the size limit, we convert them to .jpg format by mapping the optical flow to gray scale range.

<table>
  <tr>
     <td>
      <table>
        <caption>Video</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>X-component</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_x.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>Y-component</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_y.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
  </tr>
</table>



2) 2D skeleton: generated via OpenPose, 25 body keypoints. For detailed keypoints information, please refer to https://cmu-perceptual-computing-lab.github.io/openpose/web/html/doc/md_doc_02_output.html#pose-output-format-body_25.

<table>
  <tr>
    <td>
      <table>
        <caption>Video</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>2D skeleton</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_y_2d.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
  </tr>
</table>

3) 3D skeleton: generated via Regression of Multiple 3D People (ROMP), 71 body keypoints. The 71 joints are 24 SMPL joints + 30 extra joints + 17 h36m joints. For details please refer to https://github.com/Arthur151/ROMP/blob/master/simple_romp/README.md.

<table>
  <tr>
    <td>
      <table>
        <caption>Video</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>3D skeleton</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_y_3Dpose.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
  </tr>
</table>

4) Clinician ASD evaluation scores of children, including demographic information (age, gender, etc.) and autism related evaluation scores such as ADOS-2.

Due to the file size limit, we have uploaded the data to google drive, which can be easily accessed at https://tinyurl.com/mr3rd2dp.


# Reference:

OpenPose: https://github.com/CMU-Perceptual-Computing-Lab/openpose

ROMP: https://github.com/Arthur151/ROMP


