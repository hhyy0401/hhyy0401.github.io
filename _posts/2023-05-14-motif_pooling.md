---
layout: post
title: An attention Multi-scale co-evolving model for dynamic link prediction
subtitle : Guozhen Zhang et al. / WWW / 2023
tags: [GNN, link prediction, motif pooling]
author: Hyunju Kim
comments : False
---


[Abstract]

- dynamic link prediction
- propose Attentional Multi-scale Co-evolving Network (AMC-Net)
    - model multi-scale structural information by a motif-based GNN with multi-scale pooling
    

[1. Introduction]

![Untitled]({{ site.baseurl }}/assets/img/motif_pooling/Untitled.png)

- two types of important information
    - temporal information
        - characterizes evolving dynamics of the network
    - structural information
        - network topology
    
    ⇒ Those two are deeply connected
    
    - microscopic level (node, edge)
    - mesoscopic level (groups)
    - macroscopic level (whole network)
    
    ⇒ temporal dynamics of different structural scales complement one another and are coherent in the meantime
    
    - existing works model the two types of information independently
    - to bridge the gaps, this paper presents an AMCNet
- The first to study the inherent correlations among the evolving dynamics of different structural scales for dynamic link prediction

[2. Problem formulation]

- For a given historical series of snapshots G={G(1), G(2), …, G(T)}, aim to predict the link structure at the future time steps: G={G(T+1), …, G(T+n)}

[3. AMCNET]

[3.1 Multi-scale Representation Learning]

![Untitled]({{ site.baseurl }}/assets/img/motif_pooling/Untitled%201.png)

- motif based pooling
    - for a given set of motifs M
    - motif-based graphs
        
        ![Untitled]({{ site.baseurl }}/assets/img/motif_pooling/Untitled%202.png)
        

[4. Experiments]

![Untitled]({{ site.baseurl }}/assets/img/motif_pooling/Untitled%203.png)

![Untitled]({{ site.baseurl }}/assets/img/motif_pooling/Untitled%204.png)

- three-node motifs → boosts the AUC
- four-node motifs → small performance improvement
- three-node motifs are the most informative