---
title: "Parallelizing Node-Level Explainability in Graph Neural Networks"
---

# Parallelizing Node-Level Explainability in Graph Neural Networks

#### Oscar Llorente Gonzalez (ollorente@comillas.edu)

---

## Explainability in Deep Learning

<img src="images/xai.png" width="70%"/>

---

## What are Graph Neural Networks?

<img src="images/gnn.png" width="80%"/>

---

## Explainability in Graph Neural Networks

<img src="images/xai_gnn.png" width="100%"/>

---

## What is Gradient Mixing?

If a node is a neighbor or two other nodes, in the backward gradient coming from those nodes will be averaged. If your explanation depends on it, then it is contaminated.

<img src="images/gradient_mixing.png" alt="drawing" width="100%"/>

---

## Why XAI in a GNN cannot be parallelized?

<img src="images/gradient_mixing_example.png" width="100%"/>

---

## Proposed Methodology

<div class="multicolumn">
<div>

<img src="images/flow.png" alt="drawing" width="100%"/>

</div>

<div>

The proposed methodology to avoid XAI contamination has the following steps:
- Graph partitioning.
- Reconstruction of broken cluster-border neighbors.
- Batch creation and explainability computation.

</div>

---

## Graph Partitioning

<img src="images/clusters.png" width="100%"/>

---

## Border Reconstruction

<img src="images/borders.png" width="100%"/>

---

## Batch Explainability

<img src="images/batches.png" width="100%"/>

---

## Results

<img src="images/cora_results.png" width="100%"/>

