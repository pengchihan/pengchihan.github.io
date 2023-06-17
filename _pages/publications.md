---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<hr>

<h2>GPR-Net: Multi-view Layout Estimation via a Geometry-aware Panorama Registration Network</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2023/05/GPRNet.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2023/05/GPRNet.png" alt="" width="600"></a></p>
<p>Jheng-Wei Su, Chi-Han Peng, Peter Wonka, Hung-Kuo Chu<br>
IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR) 2023, <a href="https://sites.google.com/view/omnicv2023">Omnidirectional Computer Vision Workshop (Omnicv2023)</a><br>
<a href="https://arxiv.org/abs/2210.11419">Paper (Arxiv)</a>&#20;|&#20;<button onclick="function_CVPRW2023()">BibTex</button>
<div id="CVPRW2023" style="display:none;">
@InProceedings{Su_2023_CVPRW,<br>
    author    = {Jheng-Wei Su, Chi-Han Peng, Peter Wonka, Hung-Kuo Chu},<br>
    title     = {GPR-Net: Multi-view Layout Estimation via a Geometry-aware Panorama Registration Network},<br>
    booktitle = {IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR) Workshop},<br>
    month     = {June},<br>
    year      = {2023},<br>
}
</div>
<script>
function function_CVPRW2023() {
  var x = document.getElementById("CVPRW2023");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
</p>
<p>Abstract:<br>
Reconstructing 3D layouts from multiple 360∘ panoramas has received increasing attention recently as estimating a complete layout of a large-scale and complex room from a single panorama is very difficult. The state-of-the-art method, called PSMNet, introduces the first learning-based framework that jointly estimates the room layout and registration given a pair of panoramas. However, PSMNet relies on an approximate (i.e., "noisy") registration as input. Obtaining this input requires a solution for wide baseline registration which is a challenging problem. In this work, we present a complete multi-view panoramic layout estimation framework that jointly learns panorama registration and layout estimation given a pair of panoramas without relying on a pose prior. The major improvement over PSMNet comes from a novel Geometry-aware Panorama Registration Network or GPR-Net that effectively tackles the wide baseline registration problem by exploiting the layout geometry and computing fine-grained correspondences on the layout boundaries, instead of the global pixel-space. Our architecture consists of two parts. First, given two panoramas, we adopt a vision transformer to learn a set of 1D horizon features sampled on the panorama. These 1D horizon features encode the depths of individual layout boundary samples and the correspondence and covisibility maps between layout boundaries. We then exploit a non-linear registration module to convert these 1D horizon features into a set of corresponding 2D boundary points on the layout. Finally, we estimate the final relative camera pose via RANSAC and obtain the complete layout simply by taking the union of registered layouts. Experimental results indicate that our method achieves state-of-the-art performance in both panorama registration and layout estimation on a large-scale indoor panorama dataset ZInD.
</p>

<hr>

<h2>Distortion Reduction for Off-Center Perspective Projection of Panoramas</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2021/11/representative.jpg"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2021/11/representative.jpg" alt="" width="600"></a></p>
<p>Chi-Han Peng, Jiayao Zhang, Chia-Chia Chen, Yun-Wei Lin<br>
<a href="https://www.art-science.org/nicograph/nicoint2023/#nicoint2023-award">NICOGRAPH International 2023</a>. <font color="red">*Best Short Paper Award</font><br>
<a href="https://pengchihan.co/wp-content/uploads/2023/05/NICOGRAPH2023_final.pdf">Paper (author's version)</a>&#20;|&#20;<a href="https://arxiv.org/abs/2111.12018">Paper (previous Arxiv version)<br></a>&#20;|&#20;<button onclick="function_NICOGRAPH2023()">BibTex</button>
<div id="NICOGRAPH2023" style="display:none;">
@InProceedings{Peng_2023_NICOGRAPH,<br>
    author    = {Chi-Han Peng, Jiayao Zhang, Chia-Chia Chen, Yun-Wei Lin},<br>
    title     = {Distortion Reduction for Off-Center Perspective Projection of Panoramas},<br>
    booktitle = {NICOGRAPH International},<br>
    month     = {June},<br>
    year      = {2023},<br>
}
</div>
<script>
function function_NICOGRAPH2023() {
  var x = document.getElementById("NICOGRAPH2023");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
</p>
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

<h2>High-Resolution Depth Estimation for 360◦ Panoramas through Perspective and Panoramic Depth Images Registration</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2022/10/WACV_overview.jpg"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2022/10/WACV_overview.jpg" alt="" width="600"></a></p>
<p>Chi-Han Peng and Jiayao Zhang<br>
<a href="https://wacv2023.thecvf.com/">IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)</a>, 2023<br>
<a href="https://arxiv.org/abs/2210.10414">Paper (Arxiv)</a>&#20;|&#20;Code (coming soon)&#20;|&#20;<button onclick="function_WACV2023()">BibTex</button>
<div id="WACV2023" style="display:none;">
@InProceedings{Peng_2023_WACV,<br>
    author    = {Peng, Chi-Han and Zhang, Jiayao},<br>
    title     = {High-Resolution Depth Estimation for 360deg Panoramas Through Perspective and Panoramic Depth Images Registration},<br>
    booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},<br>
    month     = {January},<br>
    year      = {2023},<br>
    pages     = {3116-3125}<br>
}
</div>
<script>
function function_WACV2023() {
  var x = document.getElementById("WACV2023");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
</p>
<p>Abstract:<br>
We propose a novel approach to compute high-resolution (2048x1024 and higher) depths for panoramas that is significantly faster and qualitatively and qualitatively more accurate than the current state-of-the-art method (360OMonoDepth). As traditional neural network-based methods have limitations in the output image sizes (up to 1024x512) due to GPU memory constraints, both 360OMonoDepth and our method rely on stitching multiple perspective disparity or depth images to come out an unified panoramic depth map. However, to achieve globally consistent stitching, 360OMonoDepth relied on solving extensive disparity map alignment and Poisson-based blending problems, leading to high computation time. Instead, we propose to use an existing panoramic depth map (computed in real-time by any panorama-based method) as the common target for the individual perspective depth maps to register to. This key idea made producing globally consistent stitching results a straightforward task. Our experiments show that our method generates qualitatively better results than existing panorama-based methods, and further outperforms them quantitatively on datasets unseen by these methods.
</p>

<hr>

<h2>H&E Stain Normalization using U-Net</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2022/10/BIBE_Results.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2022/10/BIBE_Results.png" alt="" width="600"></a></p>
<p>Chi-Chen Lee, Po-Tsun Paul Kuo, and Chi-Han Peng<br>
<a href="https://bibe2022.asia.edu.tw/">IEEE International Conference on BioInformatics and BioEngineering (BIBE)</a>, 2022. (short paper)</br>
<a href="https://pengchihan.co/wp-content/uploads/2022/11/BIBE2022_paper.pdf">Paper</a>&#20;|&#20;<a href="https://arxiv.org/abs/2211.05420">Arxiv</a>&#20;|&#20;<button onclick="function_BIBE2022()">BibTex</button>
<div id="BIBE2022" style="display:none;">
@INPROCEEDINGS {9973557,<br>
author = {C. Lee and P. Kuo and C. Peng},<br>
booktitle = {2022 IEEE 22nd International Conference on Bioinformatics and Bioengineering (BIBE)},<br>
title = {H&amp;E Stain Normalization using U-Net},<br>
year = {2022},<br>
month = {nov},<br>
pages = {29-32},<br>
doi = {10.1109/BIBE55377.2022.00014},<br>
publisher = {IEEE Computer Society},<br>
}
</div>
<script>
function function_BIBE2022() {
  var x = document.getElementById("BIBE2022");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
</p>
<p>Abstract:<br>
We propose a novel hematoxylin and eosin (H&E) stain normalization method based on a modified U-Net neural network architecture. Unlike previous deep-learning methods that were often based on generative adversarial networks (GANs), we take a teacher-student approach and use paired datasets generated by a trained CycleGAN to train a U-Net to perform the stain normalization task. Through experiments, we compared our method to two recent competing methods, CycleGAN and StainNet, a lightweight approach also based on the teacher-student model. We found that our method is faster and can
process larger images with better quality compared to CycleGAN. We also compared to StainNet and found that our method delivered quantitatively and qualitatively better results.</p>

<hr>

<h2>Optimizing Placements of 360◦ Panoramic Cameras in Indoor Environments by Integer Programming</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2022/10/STAG2022_teaser.jpg">
<img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2022/10/STAG2022_teaser.jpg" alt="" width="600"></a></p>
<p>Syuan-Rong Syu and Chi-Han Peng<br>
<a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a>, 2022.</br>
<a href="https://arxiv.org/abs/2211.07296">Arxiv</a>&#20;|&#20;<button onclick="function_STAG2022()">BibTex</button>
<div id="STAG2022" style="display:none;">
@inproceedings {10.2312:stag.20221260,<br>
booktitle = {Smart Tools and Applications in Graphics - Eurographics Italian Chapter Conference},<br>
title = {{Optimizing Placements of 360° Panoramic Cameras in Indoor Environments by Integer Programming}},<br>
author = {Syu, Syuan-Rong and Peng, Chi-Han},<br>
year = {2022},<br>
publisher = {The Eurographics Association},<br>
ISSN = {2617-4855},<br>
ISBN = {978-3-03868-191-5},<br>
DOI = {10.2312/stag.20221260}<br>
}
</div>
<script>
function function_STAG2022() {
  var x = document.getElementById("STAG2022");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We propose a computational approach to find a minimal set of 360◦ camera placements that together sufficiently cover an indoor environment for the building documentation problem in the architecture, engineering, and construction (AEC) industries. Our approach, based on a simple integer programming (IP) problem formulation, solves very efficiently and globally optimally. We conducted a study of using panoramas to capture the appearances of a real-world indoor environment, in which we found that our computed solutions are better than human solutions decided by both non-professional and professional users.</p>

<hr>

<h2>Floor Plan Exploration Framework Based on Similarity Distances</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2022/10/STAG2022_poster_architecture.jpg"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2022/10/STAG2022_poster_architecture.jpg" alt="" width="600"></a></p>
<p>Chia-Ying Shih and Chi-Han Peng<br><a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a> (poster), 2022.<br>
<a href="https://arxiv.org/abs/2211.07331">Arxiv</a>&#20;|&#20;<button onclick="function_STAG2022p()">BibTex</button>
<div id="STAG2022p" style="display:none;">
@inproceedings {10.2312:stag.20221263,<br>
booktitle = {Smart Tools and Applications in Graphics - Eurographics Italian Chapter Conference},<br>
title = {{Floor Plan Exploration Framework Based on Similarity Distances}},<br>
author = {Shih, Chia-Ying and Peng, Chi-Han},<br>
year = {2022},<br>
publisher = {The Eurographics Association},<br>
ISSN = {2617-4855},<br>
ISBN = {978-3-03868-191-5},<br>
DOI = {10.2312/stag.20221263}<br>
}
</div>
<script>
function function_STAG2022p() {
  var x = document.getElementById("STAG2022p");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
Computational methods to compute similarities between floor plans can help architects explore floor plans in large datasets to avoid duplication of designs and to search for existing plans that satisfy their needs. Recently, LayoutGMN delivered state-of-the-art performance for computing similarity scores between floor plans. However, the high computational costs of LayoutGMN make it unsuitable for the aforementioned applications. In this paper, we significantly reduced the times needed to query results computed by LayoutGMN by projecting the floor plans into a common low-dimensional (e.g., three) data space. The projection is done by optimizing for coordinates of floor plans with Euclidean distances mimicking their similarity scores
originally calculated by LayoutGMN. Quantitative and qualitative evaluations show that our results match the distributions of the original LayoutGMN similarity scores. User study shows that our similarity results largely match human expectations.</p>

<hr>