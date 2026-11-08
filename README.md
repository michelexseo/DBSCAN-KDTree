# DBSCAN-KDTree

A personal showcase of my work evaluating clustering algorithms for autonomous racing in Formula Student.

## Project context

The goal of the original project was to find an effective way to cluster LiDAR points for an autonomous Formula Student race car. The input points come from a 3D LiDAR sensor and are first filtered with ground removal. Clustering is then used to identify the cones that delimit the track.

The team's original implementation used a straightforward DBSCAN algorithm. We tested multiple approaches to find the best fit for our setup and the average number of points processed at the time. A KD-tree-based approach performed best in those tests, so I developed and evaluated KD-tree implementations for the project. The system was intended to run on an NVIDIA Jetson Orin.

## Original project

The KD-tree work and its surrounding project are part of [Peace44/DBSCAN](https://github.com/Peace44/DBSCAN), specifically the [`KDTREE_DBSCAN`](https://github.com/Peace44/DBSCAN/tree/basic_optimized/KDTREE_DBSCAN) directory on the `basic_optimized` branch.

This repository is a personal showcase of that work. Benchmark results depend on the dataset, algorithm configuration, and hardware; comparisons should use the same inputs and settings when reporting performance.
