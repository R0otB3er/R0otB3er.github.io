---
title: "BVH Construction Algorithm"
excerpt: "Optimizing a part of a Ray tracing program by 50%"
collection: portfolio
---

**Technologies**: C++, CUDA, GPU Compute<br>
**Role**: GPU Optimization & Algorithm Engineering<br>
**Links**: [Repository](https://github.com/yaannsloot/cuda-lbvh)<br>

A high-performance bounding volume hierarchy (BVH) construction optimization project designed to accelerate rendering. The application features:

### Algorithmic Translation
* Changed the core construction algorithm from a standard LBVH to H-PLOC (Hierarchical Parallel Locally-Ordered Clustering).
* Implemented the novel H-PLOC approach directly from the academic research pseudo-code provided in the source paper.
* Engineered a solution that constructs the binary BVH in a single kernel launch, fully eliminating costly host-device synchronization dependency chains.

### Technical Implementation
* **Wave Intrinsics**: Leveraged GPU wave intrinsics (equivalent to CUDA warps of 32 work items) to maximize parallelism during cluster merging.
* **Self-Directed Learning**: Researched and applied advanced GPU wave intrinsics independently, mastering hardware-level concepts that expanded significantly beyond the standard course curriculum.
* **Data Management**: Managed 64-bit Morton codes, parent IDs, and cluster indices efficiently within allocated memory regions to minimize overhead.

**Key Features**:
* Maintained BVH quality comparable to leading algorithms like PLOC++ while achieving substantially lower construction times.
* Replaced iterative multi-kernel approaches with a unified, high-speed bottom-up construction pipeline.
* Optimized wave utilization to achieve an average of 66% during critical nearest neighbor searches by caching cluster data.
* Implemented an efficient top-down algorithm to convert binary BVHs to wide BVH formats in a single kernel launch.