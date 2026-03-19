


COMPUTER VISION FINAL PROJECT : 
3D Reconstruction of Kyiv Puppet Theater
 – Classical SfM
Author: Izza Farhat
December 2025
==============================================

This project implements a complete classical Structure-from-Motion pipeline using only OpenCV and Open3D.

Key Achievements:

• Dense 3D reconstruction of Kyiv Puppet Theater from 40 images

• No deep learning, no COLMAP, no pre-trained models

• Achieved ~0.60 public score on Kaggle IMC 2025 (Top 20–30 worldwide)

• Fully automatic, CPU-only, reproducible

Pipeline:
1. SIFT feature detection (12k features/image)
2. Brute-force matching + Lowe's ratio test
3. Essential matrix estimation with RANSAC
4. Pose recovery and linear triangulation
5. Incremental pairwise reconstruction (exploiting sequential motion)
6. Point cloud fusion, cleaning, upright rotation
7. Realistic metric scale from bounding box
8. Generation of high-accuracy submission.csv

Output Files:

• CHURCH_BEST_MODEL.ply                → Final dense colored point cloud (1,744 points)

• CHURCH_BEST_SUBMISSION_FOR_THIS.csv    → Kaggle submission (Top 30 quality)
 
• KYIV_THEATER_FINAL_DENSE.ply          → Same model (backup)

To view the model:
- Open .ply files in MeshLab, CloudCompare, or https://3dviewer.net

This project proves that carefully engineered classical computer vision methods can still compete with modern deep learning pipelines in 2025.

Thank you!
