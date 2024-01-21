---
permalink: /
title: "Yuxin Yao"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io). -->

Welcome to my website. I am Yuxin Yao, a 1st Year PhD student in Information Engineering at University of Cambridge, supervised by Prof. Joan Lasenby. 
I obtained my Master of Engineering degree integrated with my bachelor at University College London. 

My current research focus on computer vision. My research interests includes: 

1. Human Pose estimation under heavy occlusion
2. Human motion generation 

I am currently seeking for collaborations on project in these fields. Please contact me if you are interested. 

## Project Experience:
### Unsupervised Visual Relocalization 

Supervised By: Dr. Simon Julier at UCL as final year project

- Reconstructed the method in 
[Unsupervised Metric Relocalization Using Transform Consistency Loss](https://arxiv.org/abs/2011.00608)
- Utilized direct image alignment to find the relative transformation between the query image and reference images. Employed the Gauss-Newton method in searching optimized transformations between the feature maps of the query and reference image.
- Generated dataset with CARLA. Collected the RGB images, depth images, and camera intrinsicand extrinsic. Inferred the pixel-wise depth map from the depth images, and the relative transformation between collected images.
- Constructed U-Net inferring feature maps and saliency maps of 2D images, extracting important features and masking out moving objects occluding the features.

<!-- ![Feature map and Saliency map example:](https://raw.githubusercontent.com/YuxinYao620/YuxinYao620.github.io/main/files/unsup.png) -->
- Feature map and Saliency map example:
![Feature map and Saliency map example:](/files/unsup.png)

<!-- <img src="./files/unsup.png" width="200" height="100"> -->
- Github: [Unsup_vis_relocal](https://github.com/YuxinYao620/unsup_vis_relocal.git)

---

### Human Motion Prediction on Egocentric Dataset 

Supervised By: Dr. Siyu Tang at ETH Zurich Computer Vision and Learning Group 

- Trained a motion prior of the egocentric dataset EgoBody which recorded the first person perspective video with Holo-lens under social interaction scenario. Predicted the motion for future 8 or 9 frames given the body model of the first 1 or 2 frames.
- Familarized and used smpl-x and smpl model. Applied AMASS and Egobody dataset to GAMMA model for a body regressor and marker predictor, which uses conditional VAE with DLow method, and GRU.



<!-- <video src="https://github.com/YuxinYao620/YuxinYao620.github.io/blob/3bdad6245d13b306a7d943365e8638976922f3c0/files/ego.mov" controls="controls" style="max-width: 700px;">
</video> -->
- Predicted future 8-9 frames. 
![Predicted future 8-9 frames](/files/ego.gif)
- Github: [Gamma_with_Egobody](https://github.com/YuxinYao620/Gamma_with_Egobody.git)


---

### For more previous projects and detailed description, please check my [CV](/files/PhD_CV.pdf)