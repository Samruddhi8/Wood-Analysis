# Analysis Pipeline

## Project Overview
This project analyzes 27 wood samples (Robinie and Buche species) to detect warping and defects using 3D laser scans (PLY) and 2D images.

## Key Findings
*   **Buche** wood shows significantly higher warping (Avg Warp Score: 15.8) compared to **Robinie** (Avg Warp Score: 13.0).
*   3 samples were flagged as "Warped" (IDs: 69, 70, 71) — all were Buche.

## Pipeline Steps
1.  **Preprocessing:** Aligned 3D scans and removed noise using Statistical Outlier Removal.
2.  **Alignment:** Used PCA to orient boards in 3D space.
3.  **Analysis:** Calculated surface flatness and extracted texture features.

## Files
*   `wood_processing_pipeline.ipynb`: The main Python code.
*   `final_qc_summary.csv`: The calculated metrics for all samples.
*   `average_warp_by_species.png`: Chart showing warp difference by species.
