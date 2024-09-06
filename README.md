# Boundless: Synthetic Data Generation for Urban Object Detection
Boundless is a photo-realistic synthetic data generation system for enabling highly accurate object detection in dense urban streetscapes. It is based on the Unreal Engine 5 City Sample project with improvements for accurate 3D bounding box collection across different lighting and scene variability conditions.

## Overview
Boundless aims to replace massive real-world data collection and manual ground-truth object annotation with an automated and configurable process. It generates synthetic image datasets that can be used to train object detection models for urban environments, particularly for medium-altitude camera perspectives where real-world training data is scarce.

## Key Features

* Dynamic lighting and weather conditions (rain, snow, dust, heat waves)
* Improved anti-aliasing for higher quality frame rendering
* Enhanced level of detail for distant objects
* Accurate 3D and 2D bounding box generation
* Export options in KITTI and YOLO formats
* Digital twin capability for replicating real-world intersections

## Pretrained Models

| Training Dataset | Pedestrian AP@0.5 | Vehicle AP@0.5 | mAP@0.5 | Download Link |
|------------------|-------------------|----------------|---------|---------------|
| VisDrone         | 24.8              | **86.9**       | 55.8    | [Download](https://drive.google.com/file/d/1kZfsv_EIuFZtHClfIBJY4qh2pnrszoRT/view?usp=sharing)  |
| CARLA            | 14.9              | 75.4           | 45.1    | [Download](https://drive.google.com/file/d/1WHc7OvdA2xMzv_xHwD-m4--a_f_l-9r8/view?usp=sharing)  |
| Boundless        | 24.0              | 81.8           | 52.9    | [Download](https://drive.google.com/file/d/1ozCNA-FpeN4MxgYHvcYul-sRmxkPN5G2/view?usp=sharing)  |
| Boundless + Digital Twin | **47.5**  | 85.7           | **66.6**| [Download](https://drive.google.com/file/d/14Z-hrOpL6xLZThHVIjNi5Kj9eq7tvWX-/view?usp=sharing)  |

## Dataset

We provide datasets generated with the simulator for training object detection models. The provided datasets are formatted in the YOLO dataset format.

### Medium-Altitude Dataset
This dataset was used for the experimental results presented above.

[Download (Google Drive)](https://drive.google.com/file/d/1eAZ6rOMB66Pph6R_nIje_5Y2-CC1DgEW/view?usp=drive_link)

### CARLA dataset

[Download (Google Drive)](https://drive.google.com/file/d/1IXrtJHkTDGGnnmtF_HCdl_lFVF2WIvBa/view?usp=sharing)

### Acknowledgements

If you use Boundless, pre-trained models or datasets in a scientific publication, we would greatly appreciate using the following citation:

```
@misc{turkcan2024boundlessgeneratingphotorealisticsynthetic,
      title={Boundless: Generating Photorealistic Synthetic Data for Object Detection in Urban Streetscapes}, 
      author={Mehmet Kerem Turkcan and Ian Li and Chengbo Zang and Javad Ghaderi and Gil Zussman and Zoran Kostic},
      year={2024},
      eprint={2409.03022},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2409.03022}, 
}
```
