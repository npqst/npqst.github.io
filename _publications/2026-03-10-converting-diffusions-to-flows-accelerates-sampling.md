---
title: "Converting diffusions to flows accelerates sampling and suggests over-conditioning of co-folding models on sequence"
collection: publications
category: manuscripts
permalink: /publication/2026-03-10-converting-diffusions-to-flows-accelerates-sampling
excerpt: ''
date: 2026-03-10
venue: 'Learning Meaningful Representations of Life @ 14th International Conference on Learning Representations'
# slidesurl: 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'https://openreview.net/pdf?id=ru5TpgipOW'
citation: 'Quast et.al. (2026). &quot;Converting diffusions to flows accelerates sampling and suggests over-conditioning of co-folding models on sequence.&quot; <i>Learning Meaningful representations of Life @ 14th International Conference on Learning Representations</i>. 1(1).'
---
Deep generative models can predict protein structures from sequence with high accuracy; however, sampling from these models remains computationally burdensome, with current protocols using hundreds of iterations through the trained model to obtain a final predicted structure. To accelerate sampling and improve the interpretability of the prediction trajectories, we convert the stochastic diffusion sampling process into a deterministic flow process. We show that the conversion of pre-trained, diffusion-based structure prediction models to probability-flow ODEs yields equivalent performance on the FoldBench benchmark alongside a 20x sampling speed-up. Furthermore, we demonstrate the effects on prediction diversity and use the intermediate predictions made along the de-noising trajectory to show that deep generative structure prediction methods are strongly conditioned on the sequence and MSA embeddings, appearing to make predictions with weak sensitivity to the noise initialisation. Finally, we discuss the implications of strong sequence conditioning for generative protein structure prediction and protein design, as well as pointing to future experiments that build on our initial results.

