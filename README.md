# PointCloud SLAM using Iterative Closest Point (ICP)

This project implements a 3D pointcloud SLAM pipeline using Iterative Closest Point (ICP). 
It covers pointcloud preprocessing, voxel downsampling, robust nearest‑neighbor matching, 
pose estimation, and failure recovery.

---

## 🚀 Features

- Load and process 3D LiDAR point clouds (`.ply`)
- Voxel grid downsampling for efficiency
- KD‑Tree nearest‑neighbor correspondence search
- Point‑to‑point ICP with outlier rejection and convergence checks
- Incremental SLAM with pose tracking and fallback handling
- Global map generation and trajectory logging

---



## 📊 Outputs

- Estimated scan‑to‑scan transforms  
- Reconstructed global pointcloud  
- ICP metrics such as RMSE and fitness  
- Debug logs showing convergence and failure recovery  

---

## 📝 Reflection Summary

The accompanying notebook discusses:
- Effects of downsampling and how voxel size influences accuracy  
- Cases where nearest‑neighbor correspondences mislead ICP  
- How convergence conditions behave in noisy or partial‑overlap scans  
- Robust techniques used to maintain stable SLAM performance  
