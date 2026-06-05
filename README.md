# Nerf_smallsizeobejects-
Comparative Evaluation of Structure-from-Motion, Neural Radiance Fields (NeRF), and Gaussian Splatting for 3D Reconstruction of Reflective Small Objects


##Project Description

This project investigates the effectiveness of modern 3D reconstruction techniques for digitizing small reflective objects using only consumer-grade smartphone imagery. The study focuses on a metal lantern with intricate perforated patterns and reflective surfaces, making it a challenging object for traditional photogrammetry methods.

The workflow begins with capturing a 360° video of the object using a smartphone. Frames are extracted from the video and processed using Structure-from-Motion (SfM) techniques in COLMAP to estimate camera poses and generate a sparse 3D point cloud. The resulting reconstruction serves as a geometric baseline for comparison.

Using the camera poses obtained from COLMAP, the same dataset is then used to train Neural Radiance Fields (NeRF) and Gaussian Splatting models through Nerfstudio. These neural rendering approaches are evaluated for their ability to reconstruct fine geometric details, handle reflective surfaces, and produce photorealistic novel-view renderings.

The project aims to analyze the strengths and weaknesses of classical photogrammetry and neural rendering methods when applied to difficult real-world objects exhibiting:

Reflective metallic surfaces
Repetitive geometric patterns
Thin structural details
Complex lighting interactions

Performance is evaluated through:

Reconstruction completeness
Geometric consistency
Visual quality of rendered views
Sparse point cloud analysis
Computational requirements
Standard image-quality metrics such as PSNR, SSIM, and LPIPS

The broader motivation is to explore practical and accessible approaches for cultural heritage digitization, where small artifacts often present significant challenges for conventional 3D reconstruction pipelines.
