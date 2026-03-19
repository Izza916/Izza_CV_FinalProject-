


COMPUTER VISION : 
3D Reconstruction of Kyiv Puppet Theater
 -- Classical SfM

December 2025
==============================================

This project implements a complete classical Structure-from-Motion pipeline using only OpenCV and Open3D.

Key Achievements:

• Dense 3D reconstruction of Kyiv Puppet Theater from 40 images

• No deep learning, no COLMAP, no pre-trained models

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

• CHURCH_BEST_SUBMISSION_FOR_THIS.csv    
 
• KYIV_THEATER_FINAL_DENSE.ply          → Same model (backup)

To view the model:
- Open .ply files in MeshLab, CloudCompare, or https://3dviewer.net

This project proves that carefully engineered classical computer vision methods can still compete with modern deep learning pipelines in 2025.

Thank you!
