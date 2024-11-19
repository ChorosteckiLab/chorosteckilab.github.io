---
layout: page
title: ncRNAs in cancer diagnosis and therapy
description: Sequence-agnostic method for RNA structure comparison in lncRNAs.
img: assets/img/UC04.png
importance: 3
category: ongoing
---

Long non-coding RNAs are essential regulators at all levels of cellular processes and interact with RNA-binding proteins and other molecules. Their misregulation leads to a wide spectrum of diseases, including cancer and immune disorders. While their sequences are usually poorly conserved, lncRNA secondary structures often are, underlining their functional relevance. Despite the continuous growth of RNA structural data, efficient tools to compare and identify conserved structures remain limited.

In this project, we suggest using the Siamese Convolutional Neural Network (SCNN) to analyze RNA secondary structure. SCNNs, proven in tasks such as face recognition, calculate structural similarities without the need for sequence alignment, thereby overcoming significant limitations of traditional methods. Preliminary results using RNases P data illustrate that SCNNs can successfully identify conserved structures within RNA families and distinguish them from unrelated sequences.

Our approach will explore conserved lncRNA structures by integrating datasets from experimental approaches like SHAPE. This project aims to explain how conserved motifs underpin lncRNA functions, further understanding their role in diseases, and uncover new therapeutic opportunities.




<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/UC03.png" title="Integrating multi-omics approaches for therapeutic targeting of ncRNAs in Cancer" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
	Targeting ncRNAs with structural element lockers (SELs). Considering an ensemble of co-existing structures to identify common structural elements and design a shared SEL.
</div>


