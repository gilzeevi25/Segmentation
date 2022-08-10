# Segmentation
![visitors](https://visitor-badge.glitch.me/badge?page_id=gilzeevi25.Segmentation.issue.1) <br/>
Image segmentation various methods almost from scratch:
in this project i will demonstrate several methods for image segmentation. my goal is to implement each method by myself, and then possibly, add some nice adjustments for improving.
the evaluation method will be F - score measurement which uses precision and recall (specific formulation inside the notebook)

I will use images from The Weizmann Horse Database which contains 328 side-view color images of horses that were also manually segmented for ground truth evaluations.
the credit goes to Eran Borenstein and his site: https://www.msri.org/people/members/eranb/

in this project you can find the following implementations:
### 1.Global & Local (adaptive) thresholds segmentation variations
### 2.Region growing with automatic seeds generation
  for automatic seeds generation i found local minimas using **peak_local_max from skimage.feature**
  for region growin i used BFS & Queue data structure
### 3.K-MEANS clustering
 Accepting both gray and RGB images
### 4.Graph Normalized Cut - recursive implementation
 As presented in Normalized Cuts and Image Segmentation,by Shi and Malik. [link](https://people.eecs.berkeley.edu/~malik/papers/SM-ncut.pdf)
 
  i used 0 and median for thresholding the 2nd lowest eigenvalue, and limited the recursion to depth = 3. 
  the partition works as perfect binary tree 
