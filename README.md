# Leveraging Front and Side Cues for Monocular 3D Object Detection

This project is implemented based on the [mmdet3D](https://github.com/open-mmlab/mmdetection3d) framework.

## Abstract

<!-- [ALGORITHM] -->

3D object detection, as an essential part of perception, is needed in various intelligent applications, including autonomous driving, autonomous sailing, etc. The cost-competitive monocular 3D object detection has drawn increasing attention recently. However, it still suffers an inferior accuracy especially for occluded objects due to the limited camera view. Inspired by compositional models, in which an object is represented as a combination of multiple components, this paper proposes a new monocular 3D object detection method that decreases the impact of occlusion by utilizing an object's front and side cues. To do this, the features are extracted from a decoupled front and side representation and then fused by an attention-based module to obtain a more consistent feature distribution. An uncertainty-guided depth ensemble based on geometry is further applied to refine the depth prediction. Experiment results demonstrate that as compared to the conventional methods, the proposed method significantly improves the detection performance for occluded objects while still satisfying real-time efficiency, with the Average Precision on 40 recall positions (AP40) respectively increasing by 10.23% for partly occluded objects and 12.22% for mostly occluded objects in the KITTI benchmark. 
## Results

### KITTI

Detailed performance on KITTI 3D detection (3D/BEV) is as follows, evaluated by AP11 and AP40 metric:

|             |     Easy      |    Moderate    |     Hard      | mAP_11/mAP_40 |
|-------------|:-------------:|:--------------:|:-------------:|:-------------:|
| Car (AP11)  | 25.77 / 32.52 | 19.66 / 24.46  | 17.19 / 21.79 |[model](https://drive.google.com/file/d/1l43RYQnUhUJnumdKxHlTkIP030gIBPE9/view?usp=sharing)|
| Car (AP40)  | 20.91 / 28.88 | 14.17 / 20.02  | 11.68 / 16.90 ||
