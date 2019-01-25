---
layout: post
title: "New paper: 'Rare geometries: revealing rare categories via dimension-driven statistics'"
data: 2019-1-25 9:20:00
categories: jekyll update
---

We just submitted a new paper, 'Rare geometries: revealing rare categories via dimension-driven statistics', 
to an upcoming machine learning conference. The idea of the paper is to use the *kappa*-profile, 
a rich geometric statistic, to classify unlabeled sets of points within the context of the rare category detection problem.
The thought is that even if two classes are not separable in the available features (this is generally not assumed in rare category detection),
they often have other geometric properties that can distinguish them.
The *kappa*-profile can often detect these differences and use them
to estimate which class an unlabeled point belongs to.
The algorithm works very well on synthetic data where the two different
classes are drawn from manifolds of different intrinsic dimension. It also is effect 
for detecting rare category points for at least one class in the Ecoli dataset.


Here is a link to the arXiv preprint (coming soon) and here is a link to the code on GitHub (coming soon).
