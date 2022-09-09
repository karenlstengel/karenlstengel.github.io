---
title: "Performance Portable Solid Mechanics via Matrix-Free $p$-Multigrid"
collection: publications
permalink: /publication/2022-05-24-perf-portable-solids
excerpt: 'We demonstrate that matrix-free p-multigrid methods provide significant performance gains on modern HPC systems over sparse, assembled matrices for hyperelastic solid mechanics problems.'
date: 2022-05-24
venue: 'Preprint - arXiv'
---
<!-- TO DO -->
Finite element analysis of solid mechanics is a foundational tool of modern engineering, with low-order finite element methods and assembled sparse matrices representing the industry standard for implicit analysis. We use performance models and numerical experiments to demonstrate that high-order methods greatly reduce the costs to reach engineering tolerances while enabling effective use of GPUs; these data structures also offer up to 2x benefit for linear elements. We demonstrate the reliability, efficiency, and scalability of matrix-free $p$-multigrid methods with algebraic multigrid coarse solvers through large deformation hyperelastic simulations of multiscale structures. We investigate accuracy, cost, and execution time on multi-node CPU and GPU systems for moderate to large models (millions to billions of degrees of freedom) using AMD MI250X (OLCF Crusher), NVIDIA A100 (NERSC Perlmutter), and V100 (LLNL Lassen and OLCF Summit), resulting in order of magnitude efficiency improvements over a broad range of model properties and scales. We discuss efficient matrix-free representation of Jacobians and demonstrate how automatic differentiation enables rapid development of nonlinear material models without impacting debuggability and workflows targeting GPUs. The methods are broadly applicable and amenable to common workflows, presented here via open source libraries that encapsulate all GPU-specific aspects and are accessible to both new and legacy code, allowing application code to be GPU-oblivious without compromising end-to-end performance on GPUs.

[Download paper here](http://academicpages.github.io/files/perf-portable-solids.pdf)

Recommended citation:  
@article{brown2022performance,
  title={Performance Portable Solid Mechanics via Matrix-Free $ p $-Multigrid},
  author={Brown, Jed and Barra, Valeria and Beams, Natalie and Ghaffari, Leila and Knepley, Matthew and Moses, William and Shakeri, Rezgar and Stengel, Karen and Thompson, Jeremy L and Zhang, Junchao},
  journal={arXiv preprint arXiv:2204.01722},
  year={2022}
}
