---
permalink: /
title: "Welcome to Guangming Tan's Homepage"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I have focused on high performance computing (HPC) since 2002 when I was a Ph.D candidate. In the field of HPC, my research interest includes parallel algorithm and programming, parallel architecture. I also have a keen interest in interdisciplinary research between HPC and  bioinformatics.

My research
======

* Autotuning

We have developed novel autotuning techniques for sparse matrices computations for more than ten years, which is one of the most important kernels in HPC. First, in my PLDI’13 paper, we formulated the performance optimization as a classification problem of format-implementation and leverages machine learning approaches to find out the best format-implementation match. This is the first sparse autotuning work that is input-adaptive and extends to more than 1000 different matrices. Second, we proposed a set of algorithmic patterns and built a new autotuning system for sparse computation in graph problems. The published paper is selected as the best paper candidate in PPoPP’19. Third, we defined the sparse computation as 3D dimensional space of format-kernel-conversion, and proposed an AI-based approaches that directly generates high performance codes from input matrices. The novel autotuning system creates totally new formats which are never found by human. The work was published in SC’22.

* Parallel Algorithm 

Another interest is parallel algorithm for GPU heterogeneous architecture. In 2010, we proposed an efficient instruction scheduling algorithm on NVIDIA Fermi GPU and implemented a DGEMM routine of the highest performance in the world (SC 2011). In that work we developed a reverse engineering tool to decode GPU machine code. The tool was extended for tunning deep learning kernel on NVIDIA Kepler GPU (PPoPP 2018). Recently, we proposed a large-scale parallel LU factorization algorithm on more than 10000 GPUs. The algorithm is applied to Linpack benchmark and achieve highest peak performance in 2019 (TPDS 2021). In 2022, we proposed an extremely efficient sparse LU algorithm on a large-scale manycore based supercomputer. The algorithm achieved a peak performance of 64Petaflops (5% efficiency), which is the best performance for sparse LU in the world until now. It pushes 2.5 million-atom Ab Initio electronic-Structure simulation of complex metallic heterostructures with DGDFT (ACM Gordon Bell Prize finalist in 2022).


News
======
1. I'm here
