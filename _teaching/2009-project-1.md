---
title: "High Performance DGEMM on GPUs"
collection: teaching
type: "Library"
permalink: /teaching/2009-project-1
venue: "ICT,CAS"
date: 2009-01-01
location: "City, Country"
---

Dense matrix operations are important problems in scientific and engineering computing applications. 
There have been a lot of works on developing high performance libraries for dense matrix operations.
Basic Linear Algebra Subprograms (BLAS) is a de facto application programming interface standard for publishing libraries to perform basic linear algebra operations such as vector and matrix multiplication.
The first BLAS is released as a building block of LAPACK, which is a performance portable library for implementing dense linear algebra.
Hardware vendors (Intel, AMD, IBM, etc.) also provide BLAS librariesy tuned on their own processors, i.e. MKL and ACML. 
It is well-known that the performance of BLAS depends on the underlying hardware.

Recently, multi/many-core CPU technology has been become mainstream since it shows advantage for avoiding power wall and instruction level parallelism wall.
As a hardware accelerator, the GPU has outpaced the standard CPU in performance and has been extensively used in general-purpose computing applications including numerical computation. 
Since dense matrix operations are compute intensive and exhibit regular memory access patterns, they are well suited for the GPU. 
To develop BLAS performance on GPU, NVIDIA released CUBLAS included in CUDA Toolkit, and AMD released ACML-GPU library.
Besides, we also observed that CUBLAS3.2 is much better than CUBLAS3.0, which was released in early of 2010. 
CUBLAS3.2 improved performance of double-precision matrix multiplication (DGEMM) by 100%, which is an important kernel in High Performance Computing.

* So, what are the technical details behind the performance improvement?
* What's the performance efficiency achieved by now? Is there any more room for a further performance improvement?

Besides, the scale of applications is becoming larger and larger, so will the matrices used in DGEMM. 
When the matrix scale is too large to put into GPU memory, there will be data transfer between CPU memory and GPU memory. 
The data transfer will lower down the DGEMM performance.
* What's the bottleneck of large scale DGEMM?
* What can we do to alleviate data transfer, and make use of GPU more efficiently?

In the project, we focus on solving these problems on both NVIDIA and ATI platforms. 
