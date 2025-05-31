---
title: "On Membership Inference Attacks in Knowledge Distillation"
collection: publications
category: published
permalink: /publication/on-membership-inference-attacks-in-knowledge-distillation
date: 2025-05-17
venue: 'arXiv preprint'
slidesurl: 'https://arxiv.org/abs/2505.11837' # Use as abstract link
paperurl: 'https://arxiv.org/pdf/2505.11837'
bibtexurl: '/files/on-membership-inference-attacks-in-knowledge-distillation.bib'
citation: '<strong>Ziyao Cui</strong>, Minxing Zhang, Jian Pei' # Use as author names
---

Nowadays, Large Language Models (LLMs) are trained on huge datasets, some including sensitive information. This poses a serious privacy concern because privacy attacks such as Membership Inference Attacks (MIAs) may detect this sensitive information. While knowledge distillation compresses LLMs into efficient, smaller student models, its impact on privacy remains underexplored. In this paper, we investigate how knowledge distillation affects model robustness against MIA. We focus on two questions. First, how is private data protected in teacher and student models? Second, how can we strengthen privacy preservation against MIAs in knowledge distillation? Through comprehensive experiments, we show that while teacher and student models achieve similar overall MIA accuracy, teacher models better protect member data, the primary target of MIA, whereas student models better protect non-member data. To address this vulnerability in student models, we propose 5 privacy-preserving distillation methods and demonstrate that they successfully reduce student models’ vulnerability to MIA, with ensembling further stabilizing the robustness, offering a reliable approach for distilling more secure and efficient student models. Our implementation source code is available [here](https://github.com/richardcui18/MIA_in_KD).