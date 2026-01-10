---
title: "On Membership Inference Attacks in Knowledge Distillation"
collection: publications
category: published
permalink: /publication/on-membership-inference-attacks-in-knowledge-distillation
date: 2025-05-17
venue: 'arXiv preprint; Under review at the 64th Annual Meeting of the Association for Computational Linguistics (ACL 2026)'
slidesurl: 'https://arxiv.org/abs/2505.11837' # Use as abstract link
paperurl: 'https://arxiv.org/pdf/2505.11837'
bibtexurl: '/files/on-membership-inference-attacks-in-knowledge-distillation.txt'
citation: '<u>Ziyao Cui</u>, Minxing Zhang, Jian Pei' # Use as author names
---

Large language models (LLMs) are trained on massive corpora that may contain sensitive information, creating privacy risks under membership inference attacks (MIAs). Knowledge distillation is widely used to compress LLMs into smaller student models, but its privacy implications are poorly understood. We systematically evaluate how distillation affects MIA vulnerability across six teacher-student model pairs and six attack methods. We find that distilled student models do not consistently exhibit lower MIA success than their teacher models, and in some cases demonstrate substantially higher member-specific attack success, challenging the assumption that knowledge distillation inherently improves privacy. We attribute this to mixed supervision in distillation: for vulnerable training data points, teacher predictions often align with ground-truth labels, causing student models to learn overly confident predictions that amplify the separability between members and non-members; conversely, for non-vulnerable points, teacher predictions and ground-truth frequently diverge, providing inconsistent learning signals. To mitigate this, we propose three practical interventions -- restricting distillation to non-vulnerable points, adding a low-dimensional Bottleneck Projection, and a normalization variant (NoNorm). Experiments show these methods reduce both aggregate and member-specific MIA success while preserving model utility, improving privacy-utility trade-offs for distilled LLMs.