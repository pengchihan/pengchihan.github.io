---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<hr>

<h3>GPR-Net: Multi-view Layout Estimation via a Geometry-aware Panorama Registration Network</h3>
<p><a href="https://pengchihan.co/wp-content/uploads/2023/05/GPRNet.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2023/05/GPRNet.png" alt="" width="600"></a></p>
<p>Jheng-Wei Su, Chi-Han Peng, Peter Wonka, Hung-Kuo Chu<br>
IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR) 2023, <a href="https://sites.google.com/view/omnicv2023">Omnidirectional Computer Vision Workshop (Omnicv2023)</a>, to appear.<br>
<a href="https://arxiv.org/abs/2210.11419">Paper (Arxiv)</a>
</p>
<p>Abstract:<br>
Reconstructing 3D layouts from multiple 360∘ panoramas has received increasing attention recently as estimating a complete layout of a large-scale and complex room from a single panorama is very difficult. The state-of-the-art method, called PSMNet, introduces the first learning-based framework that jointly estimates the room layout and registration given a pair of panoramas. However, PSMNet relies on an approximate (i.e., "noisy") registration as input. Obtaining this input requires a solution for wide baseline registration which is a challenging problem. In this work, we present a complete multi-view panoramic layout estimation framework that jointly learns panorama registration and layout estimation given a pair of panoramas without relying on a pose prior. The major improvement over PSMNet comes from a novel Geometry-aware Panorama Registration Network or GPR-Net that effectively tackles the wide baseline registration problem by exploiting the layout geometry and computing fine-grained correspondences on the layout boundaries, instead of the global pixel-space. Our architecture consists of two parts. First, given two panoramas, we adopt a vision transformer to learn a set of 1D horizon features sampled on the panorama. These 1D horizon features encode the depths of individual layout boundary samples and the correspondence and covisibility maps between layout boundaries. We then exploit a non-linear registration module to convert these 1D horizon features into a set of corresponding 2D boundary points on the layout. Finally, we estimate the final relative camera pose via RANSAC and obtain the complete layout simply by taking the union of registered layouts. Experimental results indicate that our method achieves state-of-the-art performance in both panorama registration and layout estimation on a large-scale indoor panorama dataset ZInD.
</p>

<hr>

<h3>Distortion Reduction for Off-Center Perspective Projection of Panoramas</h3>
<p><a href="https://pengchihan.co/wp-content/uploads/2021/11/representative.jpg"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2021/11/representative.jpg" alt="" width="600"></a></p>
<p>Chi-Han Peng, Jiayao Zhang, Chia-Chia Chen, Yun-Wei Lin<br>
<a href="https://www.art-science.org/nicograph/nicoint2023/">NICOGRAPH International 2023</a>, to appear.<br>
<a href="https://pengchihan.co/wp-content/uploads/2023/05/NICOGRAPH2023_final.pdf">Paper (author's version)</a> | <a href="https://arxiv.org/abs/2111.12018">Paper (previous Arxiv version)</br></a></p>
<p>Abstract:<br>
A key assumption of perspective projection is that linear features in 3D shall remain linear after being projected to the 2D screen. 
This assumption is preserved when we draw a spherical panorama perspectively in arbitrary viewing directions and field-of-views 
as long as the camera position is fixed at the center. However, when the camera moves away from the center, barrel-like distortions 
appear and such assumption breaks. To address this issue, we propose modifications to the equirectangular-to-perspective (E2P) projection 
that significantly reduced distortion of linear features when the camera position is away from the center. We compared with other common methods
that aim to augment panoramas with 3D information including: 1) building a point cloud augmented with per-pixel depth and 2)
building a 3D room model according to room layouts, and found that our method produced rendering results with less linearity
distortion measured quantitatively and qualitatively.
</p>

<hr>