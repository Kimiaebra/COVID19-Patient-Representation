# COVID19-Patient-Representation
Modeling patient variability in scRNA-seq data

# Team: 
  Kimia Ebrahimi (ge28dey@mytum.de)
  
  Farhad M. Dehkordi
  
  Sandra Rjeschn
  
  Almut Voigts

# Supervisor:
  
  Vladimir Shitov
 
  Till Richter
  
  Malte Lücken

# Project Outline
Single-cell transcriptomics has revolutionized our understanding of cellular diversity in human biology, highlighting how individual differences in genetics, lifestyle, and acquired characteristics influence cellular behavior. This variability is crucial for understanding diverse disease manifestations and responses to treatments across individuals. Despite the potential insights, studies on inter-individual variations in single-cell data have been limited, primarily due to the small size of datasets. With the growth of single-cell datasets, we now have the opportunity to explore these individual differences more thoroughly. This project aims to apply recent patient representation methods, including deep learning[1,2], optimal transport[3,4], and distribution-based approaches[5,6], to analyze COVID-19 datasets[7,8]. We will investigate the effectiveness of these methods in capturing patient-specific differences in COVID-19, and explore the adaptation of self-supervised methods from image analysis to single-cell data [9,10] for modeling patient variability.

# Tasks 
1) Implement the contrastive learning framework to represent samples from single-cell RNA sequencing data for COVID-19
2) Adjust the model's hyperparameters manually and via usefull tools such as Optuna[11]
3) Create evaluation metrics for assessing patient representation derived from the contrastive model
4) Evaluate current methods and aim to surpass them using self-supervised deep learning techniques
   

<img width="685" alt="Screenshot 2024-03-17 at 2 50 17 PM" src="https://github.com/Kimiaebra/COVID19-Patient-Representation/assets/92225508/5a5bb869-e3a6-4373-b3e6-451ff4f1884b">


# Data:
We used single-cell RNA sequencing datasets from large cohorts of COVID-19 patients with differing disease severity.

We used the Stephenson et al. COVID-19 dataset [7] for benchmarking.It consists of single-cell transcriptomics data from **143 patients** across the UK, either healthy or with asymptomatic, mild, moderate, severe and critical COVID- 19. **1,141,860 cells** were registered and **781,123** passed quality control. The variable of interest in this dataset is called **’Status’**

The application of self-supervised method was explored on the COvid-19 Multi-omics Blood ATlas (COMBAT) dataset [8], which included records for **140 patients** with **783,704 cells per in- dividual**. The variable of interest in this dataset is called **’Outcome’**


# Literature
1. De Donno, C., Hediyeh-Zadeh, S., Moinfar, A.A. et al. Population-level integration of single-cell datasets enables multi-scale analysis across samples. Nat Methods 20, 1683–1692 (2023). https://doi.org/10.1038/s41592-023-02035-2
2. Boyeau, P. et al. Deep generative modeling for quantifying sample-level heterogeneity in single-cell omics. 2022.10.04.510898 Preprint at https://doi.org/10.1101/2022.10.04.510898 (2022).
3. Chen, W.S., Zivanovic, N., van Dijk, D. et al. Uncovering axes of variation among single-cell cancer specimens. Nat Methods 17, 302–310 (2020). https://doi.org/10.1038/s41592-019-0689-z
4. Joodaki, M. et al. Detection of PatIent-Level distances from single cell genomics and pathomics data with Optimal Transport (PILOT). 2022.12.16.520739 Preprint at https://doi.org/10.1101/2022.12.16.520739 (2022).
5. Wang, H., Torous, W., Gong, B. & Purdom, E. Visualizing scRNA-Seq Data at Population Scale with GloScope. 2023.05.29.542786 Preprint at https://doi.org/10.1101/2023.05.29.542786 (2023).
6. Yi, H. & Stanley, N. scLKME: A Landmark-based Approach for Generating Multi-cellular Sample Embeddings from Single-cell Data. 2023.11.13.566846 Preprint at https://doi.org/10.1101/2023.11.13.566846 (2023).
7. Stephenson, E., Reynolds, G., Botting, R.A. et al. Single-cell multi-omics analysis of the immune response in COVID-19. Nat Med 27, 904–916 (2021). https://doi.org/10.1038/s41591-021-01329-2 
8. Ahern, D. J. et al. A blood atlas of COVID-19 defines hallmarks of disease severity and specificity. Cell 185, 916-938.e58 (2022).
9. Chen, T., Kornblith, S., Norouzi, M. & Hinton, G. A Simple Framework for Contrastive Learning of Visual Representations. Preprint at https://doi.org/10.48550/arXiv.2002.05709 (2020).
10. Grill, J.-B. et al. Bootstrap your own latent: A new approach to self-supervised Learning. Preprint at https://doi.org/10.48550/arXiv.2006.07733 (2020).
11. Akiba, T., Sano, S., Yanase, T., Ohta, T., & Koyama,M. (2019). Optuna: A next-generation hyper-parameter optimization framework
