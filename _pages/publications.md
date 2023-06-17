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
IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR) 2023,<br>
<a href="https://sites.google.com/view/omnicv2023">Omnidirectional Computer Vision Workshop (Omnicv2023)</a><br>
<a href="https://arxiv.org/abs/2210.11419">Paper (Arxiv)</a>&nbsp;|&nbsp;<button onclick="function_CVPRW2023()">BibTex</button>
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
<a href="https://pengchihan.co/wp-content/uploads/2023/05/NICOGRAPH2023_final.pdf">Paper (author's version)</a>&nbsp;|&nbsp;<a href="https://arxiv.org/abs/2111.12018">Paper (previous Arxiv version)</a>&nbsp;|&nbsp;<button onclick="function_NICOGRAPH2023()">BibTex</button>
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
<a href="https://arxiv.org/abs/2210.10414">Paper (Arxiv)</a>&nbsp;|&nbsp;Code (coming soon)&nbsp;|&nbsp;<button onclick="function_WACV2023()">BibTex</button>
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
<a href="https://bibe2022.asia.edu.tw/">IEEE International Conference on BioInformatics and BioEngineering (BIBE)</a>, 2022 (short paper)<br>
<a href="https://pengchihan.co/wp-content/uploads/2022/11/BIBE2022_paper.pdf">Paper</a>&nbsp;|&nbsp;<a href="https://arxiv.org/abs/2211.05420">Arxiv</a>&nbsp;|&nbsp;<button onclick="function_BIBE2022()">BibTex</button>
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
<a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a>, 2022<br>
<a href="https://arxiv.org/abs/2211.07296">Arxiv</a>&nbsp;|&nbsp;<button onclick="function_STAG2022()">BibTex</button>
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
<p>Chia-Ying Shih and Chi-Han Peng<br><a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a> (poster) 2022.<br>
<a href="https://arxiv.org/abs/2211.07331">Arxiv</a>&nbsp;|&nbsp;<button onclick="function_STAG2022p()">BibTex</button>
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

<h2>Reconstructing 3D Indoor Layout from Multiple Panoramic Images (結合深度學習與圖形最佳化方法之多視角室內全景影像三維格局重建)</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2021/08/CGW2021_teaser.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2021/08/CGW2021_teaser.png" alt="" width="600"></a></p>
<p>Sio-Keong Si, Jheng-Wei Su, Chi-Han Peng, Kuo-Wei Chen, Felix Chang, Chih-Yuan Yao, and Hung-Kuo Chu <br>
Computer Graphics Workshop (CGW), 2021 <font color="red"> *Best Paper Award</font><br>
<a href="https://pengchihan.co/wp-content/uploads/2021/08/Reconstructing-3D-Indoor-Layout-from-Multiple-Panoramic_Images_CGW2021.pdf">Paper (Author's version)</a></p>
<p>Abstract:<br>
We propose a novel framework to estimate room layouts from multiple panoramas taken inside the same room with registration. Our solution consists of the following major components. First, we propose a boxification line prediction network that can predict boxification lines for each panorama in the same room. Second, we propose a graph-cut based binary segmentation that produces room layouts with sharp corners and straight walls. Third, we also annotated one multi-view consistent layout dataset for this new layout prediction framework. Our quantitative results show an improvement over single-view room layout estimation algorithms.</p>

<hr>

<h2>Manhattan Room Layout Reconstruction from a Single 360∘ Image: A Comparative Study of State-of-the-Art Methods</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2021/08/IJCV2021_teaser.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2021/08/IJCV2021_teaser.png" alt="" width="600"></a></p>
<p>Chuhang Zou, Jheng-Wei Su, Chi-Han Peng, Alex Colburn, Qi Shan, Peter Wonka, Hung-Kuo Chu, and Derek Hoiem<br>
International Journal of Computer Vision (IJCV), 2021<br>
<a href="https://arxiv.org/pdf/1910.04099.pdf">Paper (Preprint)</a>&nbsp;|&nbsp;<button onclick="function_IJCV2021()">BibTex</button>
<div id="IJCV2021" style="display:none;">
@article{898f68bc4970428688b5ebb33a7ea681,<br>
title = "Manhattan Room Layout Reconstruction from a Single 360 ∘ Image: A Comparative Study of State-of-the-Art Methods",<br>
author = "Chuhang Zou and Su, {Jheng Wei} and Peng, {Chi Han} and Alex Colburn and Qi Shan and Peter Wonka and Chu, {Hung Kuo} and Derek Hoiem",<br>
year = "2021",<br>
month = may,<br>
doi = "10.1007/s11263-020-01426-8",<br>
volume = "129",<br>
pages = "1410--1431",<br>
journal = "International Journal of Computer Vision",<br>
issn = "0920-5691",<br>
publisher = "Springer",<br>
number = "5",<br>
}
</div>
<script>
function function_IJCV2021() {
  var x = document.getElementById("IJCV2021");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
Recent approaches for predicting layouts from 360◦ panoramas produce excellent results. These approaches build
on a common framework consisting of three steps: a preprocessing step based on edge-based alignment, prediction
of layout elements, and a post-processing step by fitting a 3D layout to the layout elements. Until now, it has been
difficult to compare the methods due to multiple different design decisions, such as the encoding network (e.g., SegNet or ResNet), type of elements predicted (e.g., corners,
wall/floor boundaries, or semantic segmentation), or method of fitting the 3D layout. To address this challenge, we summarize and describe the common framework, the variants,
and the impact of the design decisions. For a complete evaluation, we also propose extended annotations for the Matterport3D dataset, and introduce two depth-based evaluation metrics.</p>

<hr>

<h2>Checkerboard Patterns with Black Rectangles</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2019/08/teaser.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2019/08/teaser.png" alt="" width="600"></a></p>
<p>Chi-Han Peng*, Caigui Jiang*, Peter Wonka, Helmut Pottmann<br>
ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH ASIA 2019)<br><a href="https://pengchihan.co/papers/checkerboard_main.pdf">Paper (authors' version)</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/checkerboard_additional_materials.pdf">Additional Materials</a> | <a href="https://pengchihan.co/papers/checkerboard_video_SIGA19.mp4">Video</a>&nbsp;|&nbsp;<button onclick="function_Sig2019()">BibTex</button>
<div id="Sig2019" style="display:none;">
@article{10.1145/3355089.3356514,<br>
author = {Peng, Chi-Han and Jiang, Caigui and Wonka, Peter and Pottmann, Helmut},<br>
title = {Checkerboard Patterns with Black Rectangles},<br>
year = {2019},<br>
issue_date = {December 2019},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {38},<br>
number = {6},<br>
issn = {0730-0301},<br>
doi = {10.1145/3355089.3356514},<br>
journal = {ACM Trans. Graph.},<br>
month = {nov},<br>
articleno = {171},<br>
numpages = {13},<br>
}
</div>
<script>
function function_Sig2019() {
  var x = document.getElementById("Sig2019");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
Checkerboard patterns with black rectangles can be derived from quad meshes with orthogonal diagonals. First, we present an initial theoretical analysis of these quad meshes. The analysis reveals many possible applications in geometry processing and also motivates the numerical optimization for aesthetic and functional checkerboard pattern design. Second, we describe an optimization algorithm that transforms initial 2D and 3D quad meshes into quad meshes with orthogonal diagonals. Third, we present a 2D checkerboard pattern design framework based on integer programming inspired by the logo design of the 2020 Olympic games. Our results show a variety of 2D and 3D checkerboard patterns that can be derived from 2D or 3D quad meshes with orthogonal diagonals.</p>

<hr>

<h2>DuLa-Net: A Dual-Projection Network for Estimating Room Layouts from a Single RGB Panorama</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2019/03/DulaNet.png"><img class="alignleft size-full wp-image-377" src="https://pengchihan.co/wp-content/uploads/2019/03/DulaNet.png" alt="" width="600"></a></p>
<p>Shang-Ta Yang, Fu-En Wang, Chi-Han Peng, Peter Wonka, Min Sun, Hung-Kuo Chu<br>Conference on Computer Vision and Pattern Recognition (CVPR), 2019<br>
<a href="https://arxiv.org/abs/1811.11977">Paper (Arxiv)</a>&nbsp;|&nbsp;<a href="https://github.com/SunDaDenny/DuLa-Net">GitHub</a>&nbsp;|&nbsp;<button onclick="function_CVPR2019()">BibTex</button>
<div id="CVPR2019" style="display:none;">
@inproceedings{Yang:2019:DuLa-Net,<br>
author    = {Yang, Shang-Ta and Wang, Fu-En and Peng, Chi-Han and Wonka, Peter and Sun, Min and Chu, Hung-Kuo},<br>
title     = {DuLa-Net: {A} Dual-Projection Network for Estimating Room Layouts From a Single {RGB} Panorama},<br>
booktitle = {{IEEE} Conference on Computer Vision and Pattern Recognition, {CVPR} 2019},<br>
pages     = {3363--3372},<br>
year      = {2019}<br>
} 
</div>
<script>
function function_CVPR2019() {
  var x = document.getElementById("CVPR2019");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We present a deep learning framework, called DuLa-Net, to predict Manhattan-world 3D room layouts from a single RGB panorama. To achieve better prediction accuracy, our method leverages two projections of the panorama at once, namely the equirectangular panorama-view and the<br>perspective ceiling-view, that each contains different clues about the room layouts. Our network architecture consists of two encoder-decoder branches for analyzing each of the two views. In addition, a novel feature fusion structure is proposed to connect two branches, which are then jointly trained to predict the 2D floor plans and layout heights. To learn more complex room layouts, we introduce the Realtor360 dataset that contains panoramas of Manhattan world room layouts with different numbers of corners. Experimental results show that our work outperforms recent state-of-the-art in prediction accuracy and performance, especially in the rooms with non-cuboid layouts.</p>

<hr>