# MMASD-A-Multimodal-Dataset-for-Autism-Intervention-Analysis

This is the repository for MMASD: A Multimodal Dataset for Autism Intervention Analysis.
![selected scenes](./sample_data/scene.jpg)

### Row 1
Caption for row 1

![Alt Text 1](sample_data/sq_20583_D16_000.gif "Caption for gif 1") ![Alt Text 2](sample_data/sq_20583_D16_000.gif "Caption for gif 2") ![Alt Text 3](sample_data/sq_20583_D16_000.gif "Caption for gif 3") ![Alt Text 4](sample_data/sq_20583_D16_000.gif "Caption for gif 4")

### Row 2
Caption for row 2

![Alt Text 5](sample_data/sq_20583_D16_000.gif "Caption for gif 5") ![Alt Text 6](sample_data/sq_20583_D16_000.gif "Caption for gif 6") ![Alt Text 7](sample_data/sq_20583_D16_000.gif "Caption for gif 7") ![Alt Text 8](sample_data/sq_20583_D16_000.gif "Caption for gif 8")

### Row 3
Caption for row 3

![Alt Text 9](sample_data/sq_20583_D16_000.gif "Caption for gif 9") ![Alt Text 10](sample_data/sq_20583_D16_000.gif "Caption for gif 10") ![Alt Text 11](sample_data/sq_20583_D16_000.gif "Caption for gif 11")


We presents a novel privacy-preserving open-source dataset, MMASD as a Multi Modal ASD benchmark dataset, collected from play therapy interventions of children with Autism. 
MMASD includes data from 32 children with ASD, and 1,315 data samples segmented from over 100 hours of intervention recordings.
It covers 11 different activities in 3 themes, and consists of four privacy-preserving modalities of data: 
![4 different modalities](./sample_data/Teaser_3.jpg)

- (1) Optical flow: derived from raw RGB video, for each frame, we have **_x.jpg and **_y.jpg, representing the horizontal and vertical components, respectively

<table>
  <tr>
     <td>
      <table>
        <caption>video</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>x-component</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_x.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>y-component</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_y.gif" width="220" height="150"></td>
        </tr>
      </table>
    </td>
  </tr>
</table>



- (2) 2D skeleton: generated via OpenPose, 25 body keypoints. For detailed keypoints information, please refer to https://cmu-perceptual-computing-lab.github.io/openpose/web/html/doc/md_doc_02_output.html#pose-output-format-body_25.

<table>
  <tr>
    <td>
      <table>
        <caption>video</caption>
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

- (3) 3D skeleton: generated via Regression of Multiple 3D People (ROMP), 71 body keypoints. The 71 joints are 24 SMPL joints + 30 extra joints + 17 h36m joints. For details please refer to https://github.com/Arthur151/ROMP/blob/master/simple_romp/README.md.

<table>
  <tr>
    <td>
      <table>
        <caption>video</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <caption>3D skeleton</caption>
        <tr>
          <td><img src="sample_data/sq_20583_D16_000_3d.gif" width="360" height="240"></td>
        </tr>
      </table>
    </td>
  </tr>
</table>

- (4) Clinician ASD evaluation scores of children, including demographic information (age, gender, etc.) and autism related evaluation scores such as ADOS-2.

Due to the file size limit, we have uploaded the data to google drive, which can be easily accessed at https://tinyurl.com/mr3rd2dp.


# Reference:

OpenPose: https://github.com/CMU-Perceptual-Computing-Lab/openpose

ROMP: https://github.com/Arthur151/ROMP


