---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<hr>

<h2>GPR-Net: Multi-view Layout Estimation via a Geometry-aware Panorama Registration Network</h2>
<p><a href="/files/GPRNet.png"><img class="alignleft size-full wp-image-377" src="/files/GPRNet.png" alt="" width="600"></a></p>
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
<p><a href="/files/nicograph.jpg"><img class="alignleft size-full wp-image-377" src="/files/nicograph.jpg" alt="" width="600"></a></p>
<p>Chi-Han Peng, Jiayao Zhang, Chia-Chia Chen, Yun-Wei Lin<br>
<a href="https://www.art-science.org/nicograph/nicoint2023/#nicoint2023-award">NICOGRAPH International 2023</a>. <font color="red">*Best Short Paper Award</font><br>
<a href="https://pengchihan.co/papers/NICOGRAPH2023_final.pdf">Paper (author's version)</a>&nbsp;|&nbsp;<a href="https://arxiv.org/abs/2111.12018">Paper (previous Arxiv version)</a>&nbsp;|&nbsp;<button onclick="function_NICOGRAPH2023()">BibTex</button>
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
<a href="https://pengchihan.co/papers/Peng_High-Resolution_Depth_Estimation_for_360deg_Panoramas_Through_Perspective_and_Panoramic_WACV_2023_paper.pdf">Paper</a>&nbsp;|&nbsp;
<a href="https://pengchihan.co/papers/Peng_High-Resolution_Depth_Estimation_WACV_2023_supplemental.pdf">Supplemental</a>&nbsp;|&nbsp;
<a href="https://pengchihan.co/papers/1428-wacv-post.pdf">Poster</a>&nbsp;|&nbsp;
<a href="https://pengchihan.co/papers/1428-wacv.mp4">Video</a>&nbsp;|&nbsp;
Code (coming soon)&nbsp;|&nbsp;<button onclick="function_WACV2023()">BibTex</button>
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
<p><a href="/files/BIBE_Results.png"><img class="alignleft size-full wp-image-377" src="/files/BIBE_Results.png" alt="" width="600"></a></p>
<p>Chi-Chen Lee, Po-Tsun Paul Kuo, and Chi-Han Peng<br>
<a href="https://bibe2022.asia.edu.tw/">IEEE International Conference on BioInformatics and BioEngineering (BIBE)</a>, 2022 (short paper)<br>
<a href="https://pengchihan.co/papers/BIBE2022_paper.pdf">Paper</a>&nbsp;|&nbsp;<a href="https://arxiv.org/abs/2211.05420">Arxiv</a>&nbsp;|&nbsp;<button onclick="function_BIBE2022()">BibTex</button>
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
<p><a href="/files/STAG2022_teaser.jpg">
<img class="alignleft size-full wp-image-377" src="/files/STAG2022_teaser.jpg" alt="" width="600"></a></p>
<p>Syuan-Rong Syu and Chi-Han Peng<br>
<a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a>, 2022<br>
<a href="https://pengchihan.co/papers/STAG2022_CameraPlacement.pdf">Paper</a>&nbsp;|&nbsp;
<a href="https://pengchihan.co/papers/STAG2022-Optimizing the placements of 360 panorama cameras in indoor environments.pptx">Slides</a>&nbsp;|&nbsp;
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
<p><a href="/files/STAG2022_poster_architecture.jpg"><img class="alignleft size-full wp-image-377" src="/files/STAG2022_poster_architecture.jpg" alt="" width="600"></a></p>
<p>Chia-Ying Shih and Chi-Han Peng<br><a href="https://www.stag-conference.org/2022/">Smart Tools and Applications in Graphics (STAG)</a> (poster) 2022.<br>
<a href="https://pengchihan.co/papers/STAG_poster.pdf">Paper</a>&nbsp;|&nbsp;
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
<p><a href="/files/CGW2021_teaser.png"><img class="alignleft size-full wp-image-377" src="/files/CGW2021_teaser.png" alt="" width="600"></a></p>
<p>Sio-Keong Si, Jheng-Wei Su, Chi-Han Peng, Kuo-Wei Chen, Felix Chang, Chih-Yuan Yao, and Hung-Kuo Chu <br>
Computer Graphics Workshop (CGW), 2021 <font color="red"> *Best Paper Award</font><br>
<a href="https://pengchihan.co/papers/Reconstructing-3D-Indoor-Layout-from-Multiple-Panoramic_Images_CGW2021.pdf">Paper</a></p>
<p>Abstract:<br>
We propose a novel framework to estimate room layouts from multiple panoramas taken inside the same room with registration. Our solution consists of the following major components. First, we propose a boxification line prediction network that can predict boxification lines for each panorama in the same room. Second, we propose a graph-cut based binary segmentation that produces room layouts with sharp corners and straight walls. Third, we also annotated one multi-view consistent layout dataset for this new layout prediction framework. Our quantitative results show an improvement over single-view room layout estimation algorithms.</p>

<hr>

<h2>Manhattan Room Layout Reconstruction from a Single 360∘ Image: A Comparative Study of State-of-the-Art Methods</h2>
<p><a href="/files/IJCV2021_teaser.png"><img class="alignleft size-full wp-image-377" src="/files/IJCV2021_teaser.png" alt="" width="600"></a></p>
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
<p><a href="/files/checkerboard.png"><img class="alignleft size-full wp-image-377" src="/files/checkerboard.png" alt="" width="600"></a></p>
<p>Chi-Han Peng*, Caigui Jiang*, Peter Wonka, Helmut Pottmann<br>
ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH ASIA 2019)<br>
<a href="https://pengchihan.co/papers/checkerboard_main.pdf">Paper</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/checkerboard_additional_materials.pdf">Additional Materials</a> | <a href="https://pengchihan.co/papers/checkerboard_video_SIGA19.mp4">Video</a>&nbsp;|&nbsp;<button onclick="function_Sig2019()">BibTex</button>
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
<p><a href="/files/DulaNet.png"><img class="alignleft size-full wp-image-377" src="/files/DulaNet.png" alt="" width="600"></a></p>
<p>Shang-Ta Yang, Fu-En Wang, Chi-Han Peng, Peter Wonka, Min Sun, Hung-Kuo Chu<br>Conference on Computer Vision and Pattern Recognition (CVPR), 2019<br>
<a href="https://arxiv.org/abs/1811.11977">Paper (Arxiv)</a>&nbsp;|&nbsp;
<a href="https://cgv.cs.nthu.edu.tw/projects/dulanet">Project</a>&nbsp;|&nbsp;
<a href="https://github.com/SunDaDenny/DuLa-Net">GitHub</a>&nbsp;|&nbsp;<button onclick="function_CVPR2019()">BibTex</button>
<div id="CVPR2019" style="display:none;">
@inproceedings{Yang:2019:DuLa-Net,<br>
author    = {Yang, Shang-Ta and Wang, Fu-En and Peng, Chi-Han and Wonka, Peter and Sun, Min and Chu, Hung-Kuo},<br>
title     = {DuLa-Net: {A} Dual-Projection Network for Estimating Room Layouts From a Single {RGB} Panorama},<br>
booktitle = {IEEE Conference on Computer Vision and Pattern Recognition, {CVPR} 2019},<br>
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

<h2>Designing Patterns using Triangle-Quad Hybrid Meshes</h2>
<p><a href="/files/hybrid.jpg"><img class="wp-image-87 aligncenter" src="/files/hybrid.jpg" alt="layout" width="600"></a></p>
<p>Chi-Han Peng, Helmut Pottmann, Peter Wonka<br>ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH 2018)<br>
<a href="https://pengchihan.co/papers/hybrid/DesigningPatternsUsingTriangleQuadHybridMeshes_main.pdf">Paper (authors' version)</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/hybrid/DesigningPatternsUsingTriangleQuadHybridMeshes_additional_materials.pdf">Additional Materials</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/hybrid/DesigningPatternsUsingTriangleQuadHybridMeshes.mp4">Video</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/hybrid/DesigningPatternsUsingTriangleQuadHybridMeshes_models.zip">Models</a>&nbsp;|&nbsp;<button onclick="function_Sig2018()">BibTex</button>
<div id="Sig2018" style="display:none;">
@article{10.1145/3197517.3201306,<br>
author = {Peng, Chi-Han and Pottmann, Helmut and Wonka, Peter},<br>
title = {Designing Patterns Using Triangle-Quad Hybrid Meshes},<br>
year = {2018},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {37},<br>
number = {4},<br>
issn = {0730-0301},<br>
doi = {10.1145/3197517.3201306},<br>
journal = {ACM Trans. Graph.},<br>
month = {jul},<br>
articleno = {107},<br>
}
</div>
<script>
function function_Sig2018() {
  var x = document.getElementById("Sig2018");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We present a framework to generate mesh patterns that consist of a hybrid of both triangles and quads. Given a 3D surface, the generated patterns fit the surface boundaries and curvatures. Such regular and nearly regular triangl-equad hybrid meshes provide two key advantages: first, novel-looking polygonal patterns achieved by mixing different arrangements of triangles and quads together; second, a finer discretization of angle deficits than utilizing triangles or quads alone. Users have controls over the generated patterns in global and local levels. We demonstrate applications of our approach in architectural geometry and pattern design on surfaces.</p>

<hr>

<h2>Computational Network Design from Functional Specifications</h2>
<p><a href="/files/ComputationalNetworkDesignFromFunctionalSpecifications.png"><img class="alignnone  wp-image-87" src="/files/ComputationalNetworkDesignFromFunctionalSpecifications.png" alt="layout" width="600"></a></p>
<p>Chi-Han Peng, Yong-Liang Yang, Fan Bao, Daniel Fink, Dong-Ming Yan, Peter Wonka, Niloy J. Mitra<br>ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH 2016)<br>
<a href="https://pengchihan.co/wp-content/uploads/2018/04/functional_layout.pdf">Paper</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/wp-content/uploads/2018/04/functional_layout.pptx">Slides</a>&nbsp;|&nbsp;<button onclick="function_Sig2016()">BibTex</button>
<div id="Sig2016" style="display:none;">
@article{10.1145/2897824.2925935,<br>
author = {Peng, Chi-Han and Yang, Yong-Liang and Bao, Fan and Fink, Daniel and Yan, Dong-Ming and Wonka, Peter and Mitra, Niloy J.},<br>
title = {Computational Network Design from Functional Specifications},
year = {2016},<br>
issue_date = {July 2016},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {35},<br>
number = {4},<br>
issn = {0730-0301},<br>
doi = {10.1145/2897824.2925935},<br>
journal = {ACM Trans. Graph.},<br>
month = {jul},<br>
articleno = {131},<br>
}
</div>
<script>
function function_Sig2016() {
  var x = document.getElementById("Sig2016");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
Connectivity and layout of underlying networks largely determine agent behavior and usage in many environments. For example, transportation networks determine the flow of traffic in a neighborhood, whereas building floorplans determine the flow of people in a workspace. Designing such networks from scratch is challenging as even local network changes can have large global effects. We investigate how to computationally create networks starting from only high-level functional specifications. Such specifications can be in the form of network density, travel time versus network length, traffic type, destination location, etc. We propose an integer programming-based approach that guarantees that the resultant networks are valid by fulfilling all the specified hard constraints and that they score favorably in terms of the objective function. We evaluate our algorithm in two different design settings, street layout and floorplans to demonstrate that diverse networks can emerge purely from high-level functional specifications.</p>

<hr>

<h2>Computing Layouts with Deformable Templates</h2>
<p><a href="/files/pentagon.png"><img class="alignnone  wp-image-87" src="/files/pentagon.png" alt="layout" width="600"></a></p>
<p>Chi-Han Peng, Yong-Liang Yang, and Peter Wonka<br>ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH 2014)<br>
<a href="https://pengchihan.co/papers/tiling/">Project Page</a> | <a href="https://pengchihan.co/papers/tiling/Computing_Layouts_with_Deformable_Templates.pdf">Paper (authors' version)</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/tiling/Computing_Layouts_with_Deformable_Templates_additional_materials.pdf">Additional Materials</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/tiling/Computing_Layouts_with_Deformable_Templates_Siggraph2014.pptx">Talk Slides</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/tiling/Computing_Layouts_with_Deformable_Templates_fastforward.pptx">Fast-Forward Slides</a>&nbsp;|&nbsp;<button onclick="function_Sig2014()">BibTex</button>
<div id="Sig2014" style="display:none;">
@article{10.1145/2601097.2601164,<br>
author = {Peng, Chi-Han and Yang, Yong-Liang and Wonka, Peter},<br>
title = {Computing Layouts with Deformable Templates},<br>
year = {2014},<br>
issue_date = {July 2014},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {33},<br>
number = {4},<br>
issn = {0730-0301},<br>
doi = {10.1145/2601097.2601164},<br>
journal = {ACM Trans. Graph.},<br>
month = {jul},<br>
articleno = {99},<br>
numpages = {11},<br>
}
</div>
<script>
function function_Sig2014() {
  var x = document.getElementById("Sig2014");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
In this paper we tackle the problem of tiling a domain with a set of deformable templates. A valid solution to this problem completely covers the domain with templates such that the templates do not overlap. We generalize existing specialized solutions and formulate a general layout problem by modeling important constraints and admissible template deformations. Our main idea for the solution is to break the layout algorithm into two steps: a discrete step to layout the approximate template positions and a continuous step to refine the template shapes. Our approach is suitable for a large class of applications, including floorplanning, urban layouts, and arts and design.</p>

<hr>

<h2>Exploring Quadrangulations</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2014/03/exploring_quadrangulations_2.png"><img class="alignnone  wp-image-87" src="https://pengchihan.co/wp-content/uploads/2014/03/exploring_quadrangulations_2.jpg" alt="exploring_quadrangulations_2" width="600"></a></p>
<p>Chi-Han Peng, Michael Barton, Caigui Jiang, and Peter Wonka<br>
ACM Transactions on Graphics (to be presented at SIGGRAPH 2014)<br>
<a href="https://pengchihan.co/papers/explore/">Project Page</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/explore/ExploringQuadrangulations%20main_paper.pdf">Paper (authors' version)</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/explore/ExploringQuadrangulations%20additional_materials.pdf">Additional Materials</a>&nbsp;|&nbsp;<a href="http://www.youtube.com/watch?v=9dvSntCIE60&amp;feature=youtu.be">Video (youtube)</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/explore/ExploreQuadrangulations%20meshes.zip">Models</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/explore/Exploring_Quadrangulations_Siggraph2014.pptx">Talk Slides</a>&nbsp;|&nbsp;<a href="https://pengchihan.co/papers/explore/Exploring_Quadrangulations_fastforward.pptx">Fast-Forward Slides</a>&nbsp;|&nbsp;<button onclick="function_Sig2014a()">BibTex</button>
<div id="Sig2014a" style="display:none;">
@article{10.1145/2541533,<br>
author = {Peng, Chi-Han and Barton, Michael and Jiang, Caigui and Wonka, Peter},<br>
title = {Exploring Quadrangulations},<br>
year = {2014},<br>
issue_date = {January 2014},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {33},<br>
number = {1},<br>
issn = {0730-0301},<br>
doi = {10.1145/2541533},<br>
journal = {ACM Trans. Graph.},<br>
month = {feb},<br>
articleno = {12},<br>
numpages = {13},<br>
}
</div>
<script>
function function_Sig2014a() {
  var x = document.getElementById("Sig2014a");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We present a framework for exploring topologically unique quadrangulations of an input shape. First, the input shape is segmented into surface patches. Second, different topologies are enumerated and explored in each patch. This is realized by an efficient subdivision-based quadrangulation algorithm that can exhaustively enumerate all mesh topologies within a patch. To help users navigate the potentially huge collection of variations, we propose tools to preview and arrange the results. Furthermore, the requirement that all patches need to be jointly quadrangulatable is formulated as a linear integer program. Finally, we apply the framework to shape-space exploration, remeshing, and design to underline the importance of topology exploration.</p>

<hr>

<h2>Connectivity Editing for Quad-Dominant Meshes</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2014/03/tower.png"><br><img class="wp-image-48 alignnone" src="https://pengchihan.co/wp-content/uploads/2014/01/connectivity_editing_for_quad_dominant_meshes.png" alt="connectivity_editing_for_quad_dominant_meshes" width="600" height="300"></a></p>
<p>Chi-Han Peng and Peter Wonka<br>Eurographics Symposium on Geometry Processing (SGP) 2013<br>
<a href="https://dl.dropboxusercontent.com/u/4064057/Connectivity%20Editing%20for%20Quad%20Dominant%20Meshes%20SGP2013.pdf">Paper</a>&nbsp;|&nbsp;<a href="https://dl.dropboxusercontent.com/u/4064057/Connectivity%20Editing%20for%20Quad%20Dominant%20Meshes%20SGP2013%20additional%20materials.pdf">Additional Materials</a>&nbsp;|&nbsp;<a href="http://www.youtube.com/watch?v=HRCELTuOGXw&amp;feature=youtu.be">Video (youtube)</a>&nbsp;|&nbsp;<a href="https://dl.dropboxusercontent.com/u/4064057/qdedit%20SGP%20slides.pptx">Slides</a>&nbsp;|&nbsp;<button onclick="function_SGP2013()">BibTex</button>
<div id="SGP2013" style="display:none;">
@inproceedings{10.1111/cgf.12171,<br>
author = {Peng, Chi-Han and Wonka, Peter},<br>
title = {Connectivity Editing for Quad-Dominant Meshes},<br>
year = {2013},<br>
publisher = {Eurographics Association},<br>
doi = {10.1111/cgf.12171},<br>
booktitle = {Proceedings of the Eleventh Eurographics/ACMSIGGRAPH Symposium on Geometry Processing},<br>
pages = {43–52},<br>
numpages = {10},<br>
}
</div>
<script>
function function_SGP2013() {
  var x = document.getElementById("SGP2013");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We propose a connectivity editing framework for quad-dominant meshes. In our framework the user can edit the mesh connectivity to control the location, type, and number of irregular vertices (with more or less than four neighbors) and irregular faces (non-quads). We provide a theoretical analysis of the problem, discuss what edits are possible and impossible, and describe how to implement an editing framework that realizes all possible editing operations. In the results we show example edits and illustrate advantages and disadvantages of different strategies for quad-dominant mesh design.</p>

<hr>

<h2>Connectivity Editing for Quadrilateral Meshes</h2>
<p><a href="https://pengchihan.co/wp-content/uploads/2014/03/teaser.png"><img class="wp-image-50 alignnone" src="https://pengchihan.co/wp-content/uploads/2014/01/connectivity_editing_for_quadrilateral_meshes.png" alt="connectivity_editing_for_quadrilateral_meshes" width="600" height="218"></a></p>
<p>Chi-Han Peng, Eugene Zhang, Yoshihiro Kobayashi, and Peter Wonka<br>ACM Transactions on Graphics (Proceedings of ACM SIGGRAPH ASIA 2011)<br><a href="https://pengchihan.co/papers/connectivity/">Project Page</a>&nbsp;|&nbsp;<a href="http://www.public.asu.edu/~pchihan/connectivity/ConnectivityEditingForQuadrilateralMeshes.pdf">Paper</a>&nbsp;|&nbsp;<a href="http://www.public.asu.edu/~pchihan/connectivity/ConnectivityEditingForQuadrilateralMeshes_additional_material.pdf">Additional Materials</a>&nbsp;|&nbsp;<a href="http://www.youtube.com/watch?v=7h4fcjdqA8Q">Video (youtube)</a>&nbsp;|&nbsp;<a href="https://dl.dropboxusercontent.com/u/4064057/SiggraphAsia2011_Presentation.pptx">Slides</a>&nbsp;|&nbsp;<button onclick="function_Sig2011()">BibTex</button>
<div id="Sig2011" style="display:none;">
@article{10.1145/2070781.2024175,<br>
author = {Peng, Chi-Han and Zhang, Eugene and Kobayashi, Yoshihiro and Wonka, Peter},<br>
title = {Connectivity Editing for Quadrilateral Meshes},<br>
year = {2011},<br>
issue_date = {December 2011},<br>
publisher = {Association for Computing Machinery},<br>
address = {New York, NY, USA},<br>
volume = {30},<br>
number = {6},<br>
issn = {0730-0301},<br>
doi = {10.1145/2070781.2024175},<br>
journal = {ACM Trans. Graph.},<br>
month = {dec},<br>
pages = {1–12},<br>
numpages = {12},<br>
}
</div>
<script>
function function_Sig2011() {
  var x = document.getElementById("Sig2011");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script></p>
<p>Abstract:<br>
We propose new connectivity editing operations for quadrilateral meshes with the unique ability to explicitly control the location, orientation, type, and number of the irregular vertices (valence not equal to four) in the mesh while preserving sharp edges. We provide theoretical analysis on what editing operations are possible and impossible and introduce three fundamental operations to move and re-orient a pair of irregular vertices. We argue that our editing operations are fundamental, because they only change the quad mesh in the smallest possible region and involve the fewest irregular vertices (i.e., two). The irregular vertex movement operations are supplemented by operations for the splitting, merging, canceling, and aligning of irregular vertices. We explain how the proposed highlevel operations are realized through graph-level editing operations such as quad collapses, edge flips, and edge splits. The utility of these mesh editing operations are demonstrated by improving the connectivity of quad meshes generated from state-of-art quadrangulation techniques.</p>

<hr>

<h2>User-Assisted Mesh Simplification</h2>
<p><img class="wp-image-63 alignnone" src="https://pengchihan.co/wp-content/uploads/2014/01/userassistedmeshsimplification1.png" alt="userassistedmeshsimplification" width="600" height="246"></p>
<p>Tan-Chi Ho, Yi-Chun Lin, Jung-Hong Chuang, Chi-Han Peng, Yu-Jung Cheng<br>
VRCIA '06 Proceedings of the 2006 ACM international conference on Virtual reality continuum and its applications<br>
<a href="https://dl.dropboxusercontent.com/u/4064057/User%20Assisted%20Mesh%20Simplification.pdf">Paper</a>&nbsp;|&nbsp;<button onclick="function_VRCIA()">BibTex</button>
<div id="VRCIA" style="display:none;">
@inproceedings{10.1145/1128923.1128934,<br>
author = {Ho, Tan-Chi and Lin, Yi-Chun and Chuang, Jung-Hong and Peng, Chi-Han and Cheng, Yu-Jung},<br>
title = {User-Assisted Mesh Simplification},<br>
year = {2006},<br>
isbn = {1595933247},<br>
publisher = {Association for Computing Machinery},<br>
doi = {10.1145/1128923.1128934},<br>
booktitle = {Proceedings of the 2006 ACM International Conference on Virtual Reality Continuum and Its Applications},<br>
pages = {59–66},<br>
numpages = {8},<br>
}
</div>
<script>
function function_VRCIA() {
  var x = document.getElementById("VRCIA");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}
</script>
<br>
Abstract:<br>
During the last decade, many simplification methods have been proposed to generate multi-resolution meshes for real-time applications. Practitioners have found that these methods alone usually fail to produce satisfactory result when models of very low polygon count are desired. This is due to the fact that the existing methods take no semantic or functional metric into account, and moreover, each error metric has its own strength and weakness. In this paper, we propose a user-assisted mesh simplification framework that allows users to improve the quality of simplified meshes derived by any error metric. The framework consists of two stages. The first stage employs a weighting scheme that allows users to refine a unsatisfactory region to achieve a user-specified resolution. The second stage is a local refinement scheme aiming to provide a user-guided fine-tune to recover local sharp features. The proposed weighting scheme differs from the previous approaches in that the weights are used to directly reorder the edge collapsing sequence rather than weighting the collapsing cost. Such a direct reordering mechanism ensures a predictable increase of resolution in the selected region, and is both error-metric and resolution independent.</p>

<hr>

<h2>Posters</h2>
<p><b>Connectivity Control for Quad-Dominant Meshes with Applications in Urban Design</b><br>Chi-Han Peng<br>Advances in Architectural Geometry (AAG) 2014<br><a href="https://dl.dropboxusercontent.com/u/4064057/AAG2014_poster_ChiHanPeng.pdf">Poster</a></p>
<p><b>Feature Detection in Aerial Images</b><br>Cheng Pan, Yifan Zhang, and Chi-Han Peng (Advisers: John Femiani, Anshuman Razdan, and Peter Wonka)<br>SIAM Data Mining Conference (SDM) 2011 Doctoral Forum<br><a href="https://dl.dropboxusercontent.com/u/4064057/FeatureDetectionInAerialImagesPoster.pdf">Poster</a></p>