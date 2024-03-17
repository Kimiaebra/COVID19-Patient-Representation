# COVID19-Patient-Representation
Modeling patient variability in scRNA-seq data

Single-cell transcriptomics has enabled profound insights into cellular heterogeneity in human tissues and organs. However, as individuals differ in their genetics, acquired characteristics, and lifestyle choices, so do their cellular profiles. Modelling these differences in cellular profiles may help us understand how disease can manifest differently across individuals and why some people respond to a drug while others don’t. To date, investigations on inter-individual differences in single-cell data have been lacking due to datasets typically only profiling cells from few individuals. As single-cell datasets are starting to grow in size, we now have the opportunity to study these effects if we understand how to model these inter-individual differences from this data. Currently, a few so-called patient representation methods have been developed to address this task. They include deep learning [1, 2], optimal transport [3, 4], and distribution-based methods [5, 6]. In this project, we will use these methods on COVID-19 datasets [7, 8] to understand how they are best applied to gain insight into patient differences in COVID-19. We will further explore how self-supervised methods that were recently proposed for image analysis may be adapted to single-cell data [9, 10] to model patient variability.

# Objective:
The goal of this internship is to evaluate patient variation in single-cell data from COVID-19 patients. We will first aim to identify patient groups with different clinical conditions from the single-cell data and investigate the drivers behind these differences. Finally, we will compare existing methods and try to beat them with self-supervised deep-learning methods that we will adapt from computer vision to single-cell applications.

<img width="685" alt="Screenshot 2024-03-17 at 2 50 17 PM" src="https://github.com/Kimiaebra/COVID19-Patient-Representation/assets/92225508/5a5bb869-e3a6-4373-b3e6-451ff4f1884b">


# Data:
We used single-cell RNA sequencing datasets from large cohorts of COVID-19 patients with differing disease severity. We used the Stephenson et al. COVID-19 dataset [7] for benchmarking, while The application of self-supervised method was explored on the COvid-19 Multi-omics Blood ATlas (COMBAT) dataset [8]

# Literature
1. De Donno, C., Hediyeh-Zadeh, S., Moinfar, A.A. et al. Population-level integration of single-cell datasets enables multi-scale analysis across samples. Nat Methods 20, 1683–1692 (2023). https://doi.org/10.1038/s41592-023-02035-2
2. Boyeau, P. et al. Deep generative modeling for quantifying sample-level heterogeneity in single-cell omics. 2022.10.04.510898 Preprint at https://doi.org/10.1101/2022.10.04.510898 (2022).
3. Chen, W.S., Zivanovic, N., van Dijk, D. et al. Uncovering axes of variation among single-cell cancer specimens. Nat Methods 17, 302–310 (2020). https://doi.org/10.1038/s41592-019-0689-z
4. Joodaki, M. et al. Detection of PatIent-Level distances from single cell genomics and pathomics data with Optimal Transport (PILOT). 2022.12.16.520739 Preprint at https://doi.org/10.1101/2022.12.16.520739 (2022).
5. Wang, H., Torous, W., Gong, B. & Purdom, E. Visualizing scRNA-Seq Data at Population Scale with GloScope. 2023.05.29.542786 Preprint at https://doi.org/10.1101/2023.05.29.542786 (2023).
6. Yi, H. & Stanley, N. scLKME: A Landmark-based Approach for Generating Multi-cellular Sample Embeddings from Single-cell Data. 2023.11.13.566846 Preprint at https://doi.org/10.1101/2023.11.13.566846 (2023).
7. Stephenson, E., Reynolds, G., Botting, R.A. et al. Single-cell multi-omics analysis of the immune response in COVID-19. Nat Med 27, 904–916 (2021). https://doi.org/10.1038/s41591-021-01329-2 
8. Ahern, D. J. et al. A blood atlas of COVID-19 defines hallmarks of disease severity and specificity. Cell 185, 916-938.e58 (2022).
