<center>

# Video Semantic Segmentation with <br> Distortion-Aware Feature Correction

[Jiafan Zhuang](https://scholar.google.com/citations?user=KbWzCu4AAAAJ&hl=zh-CN) &nbsp;&nbsp;&nbsp;&nbsp;[Zilei Wang](https://scholar.google.com/citations?hl=zh-CN&user=tMO7jm4AAAAJ) &nbsp;&nbsp;&nbsp;&nbsp;[Bingke Wang]()

[VIM Lab, University of Science and Technology of China](http://vim.ustc.edu.cn/)

</center>

<video src="https://www.youtube.com/watch?v=8Q9SuW-7rS0&feature=youtu.be" width="800px" height="600px" controls="controls"></video>

<center>

## Abstract
</center>

&nbsp;&nbsp;&nbsp;&nbsp;Video semantic segmentation targets to generate accurate semantic map for each frame in a video. For such a task, conducting  per-frame image segmentation is generally unacceptable in practice due to high computational cost. To address the issue, many works use the flow-based feature propagation to reuse the features of previous frames, which actually exploits the content continuity of consecutive frames. However, the optical flow estimation itself inevitably suffers inaccuracy and consequently would cause the propagated features distorted. In this paper, we propose a distortion-aware feature correction method with aims of improving video segmentation performance at a low price. The core idea is to mainly correct the features on distorted regions using the current frame, while the propagated features are reserved for other regions. As a result, a lightweight network can be enough to achieve promising segmentation results. In particular, we propose to predict the distorted regions in the image space by utilizing the consistency of distortion patterns for images and features, such that the high-cost feature extraction for the current frames can be avoided. We conduct the extensive experiments on Cityscapes and CamVid, and the results show that our proposed method significantly outperforms previous methods and achieves the state-of-the-art performance on both segmentation accuracy and speed.

<center>

## Framework
</center>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/framework.png" width="860"/>

<center>

## Visualization
</center>

<center>

### Cityscapes
</center>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

<center>

### CamVid
</center>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

<img src="https://github.com/jfzhuang/DAVSS.github.io/blob/master/image/cityscapes_56.png" width="860"/>

## Materials

## Citation
```
@article{zhuang2020video,
  title={Video Semantic Segmentation with Distortion-Aware Feature Correction},
  author={Zhuang, Jiafan and Wang, Zilei and Wang, Bingke},
  journal={arXiv preprint arXiv:2006.10380},
  year={2020}
}
```