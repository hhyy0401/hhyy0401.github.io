---
layout: post
title: Unsupervised Inductive Graph-Level Representation Learning via Graph-Graph Proximity
subtitle : Yunsheng Bai et al. / IJCAI / 2019
tags: [GNN, NAS, representation learning]
author: Hyunju Kim
comments : False
---

[Abstract]

- embeddings of two graphs preserve their graph-graph proximity
- suggest UGraphEMB (unsupervised manner)

[1. Introduction]

**Q. Can we embed an entire graph into a vector in an unsupervised way, and how? (in unsupervised manner)**

- graph2vec: not inductive
- supervised method: use only “intra-graph” information

[2. The proposed approach: UGraphEmb]

- generate one embedding per graph from node embeddings using Multi Scale Node Attention (MSNA)

[2.1 Inductive Graph-Level Embedding]

- node embedding generation
    - inductivity
    - permutation-invariance
    
    ⇒ GCN: aggregate node embeddings of itself and neighbors
    
    ⇒ or other models - Graphsage, GAT, GIN
    
    ⇒ here, choose GIN
    
- Graph embedding generation
    - generate one embedding per graph using node embeddings
        
        ![Untitled](/assets/img/inductive/Untitled.png)
        
        ![Untitled](/assets/img/inductive/Untitled%201.png)
        

![Untitled](/assets/img/inductive/Untitled%202.png)

[2.2 Unsupervised loss via inter-graph proximity preservation]

- Definition of graph proximity
    - label
    - domain knowledge & human experts
    - domain-agnostic & well-accepted metrics (GED, MCS)
- prediction of graph proximity
    - difference between the predicted distance and the ground-truth distance
        
        ![Untitled](/assets/img/inductive/Untitled%203.png)
        
    - if metric is similarity
        
        ![Untitled](/assets/img/inductive/Untitled%204.png)