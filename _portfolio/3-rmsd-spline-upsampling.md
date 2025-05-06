---
title: "RMSD for length-mismatched protein structures"
excerpt: "Implementation for calculating root-mean-square deviation of length-mismatched proteins via spline upsampleing and dynamic time warping.<br/><img src='/images/spline_upsampling_figure.png' width='200'>"
collection: portfolio
---

<img src='/images/spline_upsampling_figure.png' width='200'>

* [github](https://github.com/npqst/different-length-euclidian-rmsd)

Protein structures are typically compared by calculating the RMSD between atom positions, often restricted to Ca. 
However, this poses a problem when comparing chains of different lengths. 
In order to compare different length CDR3 loop structures, we implement a method for upsampling of the backbone coordinates to match in length. 
We use spline upsampling to re-sample the shorter loop Ca coordinates by polynomial interpolation, and compare the new coordinates. 
For chains of the same length this distance calculation is equivalent to standard RMSD. 
Empirically, we find that this method is upper bound by the RMSD, which we find by calculating the distance between two equivalent length loops after upsampling.
We also implemented a version of the dynamic time warping (DTW) algorithm, an alternative method based on optimally matching coordinates in the longer loop to coordinates in the shorter loop. 
While this method is in use, it is liable to spurious, non-RMSD like results when comparing very different structures, such that sequence aligned coordinates are substantially further than DTW match coordinates, resulting in low distances despite structural dissimilarity. 
We therefore opt for the former method; both methods are implemented as a small python package with a common API.
