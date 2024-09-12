# CS249 Course Project: Review of Numerical Abstract Domains

## Project Overview

This project is part of the CS249 course at the University of California, Riverside. The goal was to read and review two foundational papers in the field of abstract domains used in program analysis: 
1. **The Octagon Abstract Domain** (2007)
2. **Fast Polyhedra Abstract Domain** (2017)

## Abstracts

### 1. The Octagon Abstract Domain (2007)

The Octagon Abstract Domain introduces an abstract domain that is more expressive than intervals but less computationally intensive than polyhedra. It allows representation of constraints of the form \( \pm x \pm y \leq c \), enabling more precise reasoning about relationships between variables in program analysis. This paper presents efficient algorithms for manipulating octagons, using Difference-Bound Matrices (DBMs) to represent these constraints. The Octagon domain strikes a balance between precision and efficiency, with a worst-case complexity of \( O(n^2) \) for memory and \( O(n^3) \) for operations. However, its scalability remains limited, making it suitable only for small-scale programs.

### 2. Fast Polyhedra Abstract Domain (2017)

The Fast Polyhedra Abstract Domain paper introduces a new approach to mitigate the computational complexity of the traditional polyhedral domain by decomposing polyhedra into partitions. This technique retains the precision of polyhedral analysis while significantly improving performance. The authors also introduce their tool, ELINA, which outperforms prior approaches like PPL and NewPolka by utilizing decomposition alongside advanced performance optimizations. Despite its complexity, particularly with widening and narrowing operations, Fast Polyhedra proves to be more scalable and feasible for large test cases, offering impressive results in static program analysis.

## Citations

1. Miné, Antoine. "The Octagon Abstract Domain." _Higher-Order and Symbolic Computation_, 2007.
2. Singh, Gagandeep, et al. "Fast Polyhedra Abstract Domain." _International Static Analysis Symposium_, 2017.
