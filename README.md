# Patch Based Principal Component Analysis for Image Compression
This repository contains code for a problem related to image compression in pattern recognition using PCA. The problem involves compress subimages of the original image by representing them with relatively few features.

## Course Information

This problem is related to a *Statistical Pattern Recognition* course taught by Professor Mohammad Rahmati (<rahmati@aut.ac.ir>) in the Computer Engineering department at Amirkabir University of Technology (AUT) in Tehran, Iran. The course was offered in the Fall of 2021.

## Problem Description

The problem involved testing the performance of Principal Component Analysis (PCA) in an image processing application, specifically image compression. The approach considered involved using PCA to compress subimages of the original image by representing them with relatively few features. The task involved several steps:
> A function called "patch_extract()" was implemented to extract non-overlapping 8x8 pixel blocks from an input image and return a matrix of vectorized blocks of the image as its columns.
> The covariance matrix of the output from "patch_extract()" was used to perform PCA analysis. The first 20 largest eigenvalues and their corresponding eigenvectors were reported, and the mean image was displayed along with the eigenvectors that corresponded to the 8 largest eigenvalues.
> The subimages were compressed using the mean vector and the eigenvectors corresponding to the k = 2, 5, 10, and 20 largest eigenvalues.
> The low-dimensional representations of the subimages were used to reconstruct each subimage, with the mean value included.
> A function called "patch_reconstruct()" was implemented to merge the reconstructed subimages and create a 448x600 pixel image. The reconstructed and original images were displayed together, and the effect of k on the results was discussed.

Overall, the results showed that PCA can effectively compress images while preserving their features. As the value of k increased, the reconstructed images became more similar to the original image, but the size of the compressed data also increased. Therefore, a trade-off must be made between image quality and data size.


![Output](/output.png)
![Output](/output-2.png)


## Repository Contents

The repository contains Python code for the problem described above, as well as a Jupyter notebook that explains the problem and provides a step-by-step cells for running the code.

## Feedback

If you have any feedback or suggestions for improving this code, please feel free to open an issue in the repository as well as send an email to Mohsen Ebadpour (<m.ebadpour@aut.ac.ir> , <mohsenebadpour@outlook.com>).

