---
title: "On Membership Inference Attacks in Knowledge Distillation"
collection: publications
category: published
permalink: /publication/on-membership-inference-attacks-in-knowledge-distillation
date: 2026-06-06
venue: 'ACM SIGKDD Explorations Newsletter, Volume 28, Issue 1'
slidesurl: 'https://dl.acm.org/doi/10.1145/3820356.3820359' # Use as abstract link
paperurl: 'https://dl.acm.org/doi/pdf/10.1145/3820356.3820359'
bibtexurl: '/files/on-membership-inference-attacks-in-knowledge-distillation.txt'
citation: '<u>Ziyao Cui</u>, Minxing Zhang, Jian Pei' # Use as author names
---

Large language models (LLMs) are trained on massive corpora that may contain sensitive information, creating privacy risks under membership inference attacks (MIAs). Knowledge distillation is widely used to compress LLMs into smaller student models, but its privacy implications are poorly understood. We systematically evaluate how distillation affects MIA vulnerability across six teacher-student model pairs and six attack methods. We find that distilled student models do not consistently exhibit lower MIA success than their teacher models, and in some cases demonstrate substantially higher member-specific attack success, challenging the assumption that knowledge distillation inherently improves privacy. We attribute this to mixed supervision in distillation: for vulnerable training data points, teacher predictions often align with ground-truth labels, causing student models to learn overly confident predictions that amplify the separability between members and non-members; conversely, for non-vulnerable points, teacher predictions and ground-truth frequently diverge, providing inconsistent learning signals. To mitigate this, we propose three practical interventions -- restricting distillation to non-vulnerable points, adding a low-dimensional Bottleneck Projection, and a normalization variant (NoNorm). Experiments show these methods reduce both aggregate and member-specific MIA success while preserving model utility, improving privacy-utility trade-offs for distilled LLMs.