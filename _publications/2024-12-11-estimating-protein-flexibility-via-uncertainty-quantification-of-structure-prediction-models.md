---
title: "Estimating protein flexibility via uncertainty quantification of structure prediction models"
collection: publications
category: manuscripts
permalink: /publication/2024-12-11-estimating-protein-flexibility-via-uncertainty-quantification-of-structure-prediction-models
excerpt: ''
date: 2024-12-11
venue: 'Machine Learning for Structural Biology @ NeurIPS 2024'
paperurl: 'https://www.mlsb.io/papers_2024/Estimating_protein_flexibility_via_uncertainty_quantification_of_structure_prediction_models.pdf'
citation: 'Quast & Sweeney et. al., (2024). &quot;Estimating protein flexibility via uncertainty quantification of structure prediction models.&quot; <i>Machine Learning for Structural Biology @ NeurIPS 2024</i>. 1(1).'
---
Deep learning architectures such as AlphaFold2, have effectively solved the protein structure prediction problem, however, they do not rigorously account for confor- mational variance in structures despite many proteins exhibiting flexible regions in which a single amino acid sequence may occupy a variety of conformations. In particular, using confidence metrics such as the pLDDT score, it is not readily possible to distinguish between regions of the protein structure where the prediction model is uncertain because the region is out-of-distribution or because the region is intrinsically flexible. Here, we use a novel approach to estimate protein flexibility via uncertainty quantification. Specifically, we reformulate the protein structure pre- diction problem as sampling a backbone function from a Gaussian process which enables us to cast flexibility estimation as aleatoric uncertainty quantification. We adapt the AlphaFold2 Structure Module architecture to produce such estimates of aleatoric uncertainty and compare these to existing proxies for conformational variance. We demonstrate the utility of our formalisation for approximating protein flexibility in a prediction framework, and our experiments demonstrate the promise of our method whilst emphasising the relationship between epistemic and aleatoric uncertainty in protein structure prediction.
