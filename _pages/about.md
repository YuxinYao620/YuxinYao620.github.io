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

Welcome to my website. I am Yuxin Yao, a 2nd Year PhD student in Information Engineering at University of Cambridge, supervised by Prof. Joan Lasenby. 
I obtained my Master of Engineering degree integrated with my bachelor at University College London. 

My current research focus on computer vision. My research interests includes: 

1. 4D Reconstruction and Novel View Synthesis with Gaussian Splatting.
2. Geometric Deep Learning.
3. Generative AI.

I am currently seeking for collaborations on project in these fields. Please contact me if you are interested!

## Project Experience:

### Simplifying and Generalising Equivariant Geometric Algebra Networks

Supervised By: Professor Joan Lasenby at Cambridge, collaborated with Christian Hockey

- Developed a simplified and generalized equivariant Geometric Algebra Transformer (CGATr) with a generalized signature by removing constraints on geometric signatures.
- Analyzed and experimented with the Geometric Algebra Transformer (GATr) to study the effectiveness of its components.
- Applied CGATr to protein structure prediction, N-body dynamics, and camera pose estimation, showcasing its potential in geometric deep learning.
- Presented this work at the 9th Conference on Applied Geometric Algebras in Computer Science and Engineering (Amsterdam, NL).
- Protein Structure Prediction Comparison between CGATr and common neural network: 
![Predicted protein structure](/files/CGATr-protein.png)
<!-- - Explained and studied the Geometric Algebra Transformer (GATr), and experimented with the effectiveness of each component of the GATr. 
- Constructed a simplified and flexible equivariant geometric algebra transformer, CGATr, with a generalized signature. Simplified and editted the GATr, removed the contraint in geometric signature which makes it fits all the geometric signatures. 
- Applied the CGATr to protein structure prediction, N-body dynamics and camera pose estimation, demonstrate strong potential of understanding geometric informaiton and more efficient geometric deep learning. 
- Gave a talk in the 9th conference on Applied Geometric Algebras in Computer Science and Engineering (Amsterdam, NL) -->

### Unsupervised Visual Relocalization 

Supervised By: Professor Simon Julier at UCL as final year project

- Implemented the method in 
[Unsupervised Metric Relocalization Using Transform Consistency Loss](https://arxiv.org/abs/2011.00608)
- Utilized direct image alignment to find the relative transformation between the query image and reference images. Employed the Gauss-Newton method in searching optimized transformations between the feature maps of the query and reference image.
- Generated dataset with CARLA for training/testing.
- Constructed U-Net inferring feature maps and saliency maps of 2D images, extracting important features and masking out moving objects occluding the features.

<!-- ![Feature map and Saliency map example:](https://raw.githubusercontent.com/YuxinYao620/YuxinYao620.github.io/main/files/unsup.png) -->
- Image and Saliency map example, the saliency map masks the fast moving part:
![Feature map and Saliency map example:](/files/unsup.png)

<!-- <img src="./files/unsup.png" width="200" height="100"> -->
- Github: [Unsup_vis_relocal](https://github.com/YuxinYao620/unsup_vis_relocal.git)

---

### Human Motion Prediction on Egocentric Dataset 

Supervised By: Professor Siyu Tang at ETH Zurich Computer Vision and Learning Group 

- Trained a motion prior of the egocentric dataset EgoBody which recorded the first person perspective video with Holo-lens under social interaction scenario. Predicted the motion for future 8 or 9 frames given the body model of the first 1 or 2 frames.
- Familarized and used smpl-x and smpl model. Applied AMASS and Egobody dataset to GAMMA model for a body regressor and marker predictor, which uses conditional VAE with DLow method, and GRU.

<!-- <video src="https://github.com/YuxinYao620/YuxinYao620.github.io/blob/3bdad6245d13b306a7d943365e8638976922f3c0/files/ego.mov" controls="controls" style="max-width: 700px;">
</video> -->
- Predicted future 8-9 frames example: 
![Predicted future 8-9 frames](/files/ego.gif)
- Github: [Gamma_with_Egobody](https://github.com/YuxinYao620/Gamma_with_Egobody.git)


---

### For more previous projects and detailed description, please check my [CV](/files/YuxinYao_CV_2024.pdf)
---


## Publication

- Hockey, C., **Yao, Y.**, Lasenby, J. Simplifying and Generalising Equivariant Geometric
Algebra Networks. The 9th conference on Applied Geometric Algebras in Computer Science
and Engineering (Abstract accepted )

- Chen, H., Li, Z., **Yao, Y**. (2022, November). Multi-agent reinforcement learning for fleet
management: a survey. In 2nd International Conference on Artificial Intelligence, Automation,
and High-Performance Computing (AIAHPC 2022) (Vol. 12348, pp. 611-624). SPIE.

- Yan, Y., Schaffter, T., Bergquist, T., ...**Yao, Y**..,... DREAM Challenge Consortium. (2021). A
Continuously Benchmarked and Crowdsourced Challenge for Rapid Development and Evaluation
of Models to Predict COVID-19 Diagnosis and Hospitalization. JAMA network open, 4(10),
e2124946-e2124946.
