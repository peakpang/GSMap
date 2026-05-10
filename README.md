# GSMap: 2D Gaussians for Online HD Mapping

Accurate High-Definition (HD) map construction is critical for autonomous driving, yet existing methods face a fundamental trade-off: vectorization-based approaches preserve topology but struggle with geometric fidelity, while rasterization-based approaches enable precise geometric supervision but produce unstructured outputs. To bridge this gap, we propose GSMap, a novel framework that unifies both paradigms via a learnable 2D Gaussian representation. Each map element is modeled as an ordered sequence of 2D Gaussians, whose centers correspond to the vertices of the vectorized polyline/polygon. This formulation enables simultaneous optimization through: (1) Differentiable rasterization that enforces pixel-level geometric constraints, and (2) Topology-aware vectorization that maintains structural regularity. Experiments on both nuScenes and Argoverse2 demonstrate that our Gaussian-based representation effectively unifies geometric and topological learning, achieving significant performance improvements and demonstrating strong compatibility with existing HD mapping architectures.


## Motivation

<div align="center">
<img src=assets\motivation.png>
</div>

## Overview of GSMap

<div align="center">
<img src=assets\pipeline.png>
</div>
