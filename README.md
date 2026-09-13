## Introduction

Path planning is a fundamental problem in robotics and autonomous navigation, where an Unmanned Aerial Vehicle (UAV) must determine a feasible, efficient, and collision-free path from a given start position to a specified goal while avoiding obstacles.

This project focuses on the study and comparative evaluation of classical, sampling-based, and hybrid path-planning approaches in 2D obstacle environments. The study examines **A\***, **Artificial Potential Field (APF)**, **Rapidly-exploring Random Tree (RRT)**, **RRT\***, and **Hybrid RRT\*+APF** approaches to understand their behavior and performance under different environmental conditions.

## Project Overview

The path-planning algorithms are evaluated in grid-based 2D environments with three different map sizes: **20×20, 60×60, and 100×100**. For each map size, sparse and dense obstacle configurations are considered, resulting in different levels of environmental complexity.

The experiments use consistent start and goal positions, obstacle configurations, and iteration settings wherever applicable to enable a fair comparison between the approaches. The performance of the algorithms is evaluated using quantitative and qualitative observations, including **path generation success, completion time, path characteristics, and obstacle collision behavior**.

The study initially evaluates A\*, RRT, and APF and is extended to include **RRT\*** and **RRT\*+APF**. RRT\* improves upon RRT through cost-based parent selection and rewiring to produce more optimal paths, while the hybrid RRT\*+APF approach combines global sampling with potential-field guidance to improve convergence and path smoothness.

The results demonstrate the trade-offs between **path optimality, computational efficiency, convergence, and robustness** across different planning approaches. The experimental outputs and performance comparisons are provided in this repository along with the complete project report.

## Algorithms Studied

- **A\*** – Graph-based search algorithm using path cost and heuristic guidance.
- **APF** – Uses attractive and repulsive potential fields to guide the UAV toward the goal while avoiding obstacles.
- **RRT** – Sampling-based approach that incrementally explores the free space through a randomly generated tree.
- **RRT\*** – An optimized variant of RRT using cost-based parent selection and rewiring for improved path optimality.
- **RRT\*+APF** – Hybrid approach combining RRT\* exploration with APF guidance for improved convergence and path smoothness.
