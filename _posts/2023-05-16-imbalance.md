---
layout: post
title: Imbalanced Graph Classification via Graph-of-Graph Neural Networks
subtitle : Yu Wang et al. / CIKM / 2022
tags: [GNN, classification, imbalance]
author: Hyunju Kim
comments : False
---

[Abstract]

- introduce G2GNN which alleviates the graph imbalance issue
- globally, construct GoG based on kernel similarity
- locally, topological augmentation via masking node features

[1. Introduction]

- real case: imblanace
    - ex) chemical space (active - inactive)
- problems of GNN on imbalanced datasets
    - incliniation to learning towards majority classes
    - poor generalization from gien scarce training data to abounding unseen testing data
- current solutions
    - augmenting data via under- or over- sampling
    - assigning weights
    - constructing synthetic training data
    
    ⇒ designed on point-based data
    
    ⇒ performance on graph-structured data is unclear
    
- graph-structured data
    - pre-training
    - adversarial training
- propose Graph-of-Graph Neural Networks (G2GNN)

[2. Problem formulation]

![Untitled](/assets/img/imbalance/Untitled.png)

[3. Related work]

- graph imbalance problem
    - current learning works are for node imbalance classification.
    - graph imbalance classification remains largely unexplored
- graph of graphs
- graph augmentations

[4. The proposed framework]

![Untitled](/assets/img/imbalance/Untitled%201.png)

- global governace: GoG propagation
- local explorer: topological augmentation

[4.1 Global Imbalance Mitigation: Graph-of-Graph Construction / Propagation]

- intuition: SMOTE, mixup (handling class imblance)

[4.1. Basic GNN encoder]

- GIN
- global-sum pooling

[4.1.2 Graph of Graphs Construction]

- edge of GoG: based on their topological similarity
    - leverage the graph kernel (Shortest Path Kernel)
- edge homophily
    
    ![Untitled](/assets/img/imbalance/Untitled%202.png)
    
    ![Untitled](/assets/img/imbalance/Untitled%203.png)
    

[4.1.3 Graph of Graphs Propagation]

- l-th-layer GoG propagation
    
    ![Untitled](/assets/img/imbalance/Untitled%204.png)
    

[4.2 Local Imbalance Mitigation: Self-consistency Regularization via Graph Augmentation]

- augmentation

[4.2.1 Removing edges]

[4.2.2 Masking node features]

- zeroing **entire** features of some nodes

[4.2.3 Self-Consistency Regularization]

[4.3 Objective Function and Prediction]

![Untitled](/assets/img/imbalance/Untitled%205.png)

[4.4 Algorithm]

![Untitled](/assets/img/imbalance/Untitled%206.png)