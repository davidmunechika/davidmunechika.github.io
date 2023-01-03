---
layout: paper
id: visual-auditor
categories: papers
permalink: papers/visual-auditor
title: "Visual Auditor: Interactive Visualization for Detection and Summarization of Model Biases"
authors: 
    - David Munechika
    - Zijie J. Wang
    - Jack Reidy
    - Josh Rubin
    - Krishna Gade
    - Krishnaram Kenthapadi
    - Duen Horng Chau
venue: IEEE Visualization Conference
venue-shorthand: VIS
location: Oklahoma City, OK, USA
year: 2022
url: /papers/visual-auditor
pdf: https://arxiv.org/abs/2206.12540
code: https://github.com/poloclub/visual-auditor
preview: https://youtu.be/ZGCVtu2fcbc
recording: https://youtu.be/MRv0hUtMvDc
selected: true
type: conference
figure: /images/visual-auditor-main.png
doi: 10.48550/arXiv.2206.12540
featured: true
feature-order: 1
feature-title: Visual Auditor
feature-description: Interactive Visualization for Detection and Summarization of Model Biases
image: /images/visual-auditor-main.png
coming-soon: false
bibtex: |-

  @inproceedings{munechika2022visual,
    title={Visual Auditor: Interactive Visualization for Detection and Summarization of Model Biases},
    author={Munechika, David and Wang, Zijie J and Reidy, Jack and Rubin, Josh and Gade, Krishna and Kenthapadi, Krishnaram and Chau, Duen Horng},
    booktitle={2022 IEEE Visualization and Visual Analytics (VIS)},
    pages={45--49},
    year={2022},
    organization={IEEE}
  }
---
    
As machine learning (ML) systems become increasingly widespread, it is necessary to audit these systems for biases prior to their deployment. Recent research has developed algorithms for effectively identifying intersectional bias in the form of interpretable, underperforming subsets (or slices) of the data. However, these solutions and their insights are limited without a tool for visually understanding and interacting with the results of these algorithms. We propose Visual Auditor, an interactive visualization tool for auditing and summarizing model biases. Visual Auditor assists model validation by providing an interpretable overview of intersectional bias (bias that is present when examining populations defined by multiple features), details about relationships between problematic data slices, and a comparison between underperforming and overperforming data slices in a model. Our open-source tool runs directly in both computational notebooks and web browsers, making model auditing accessible and easily integrated into current ML development workflows. An observational user study in collaboration with domain experts at Fiddler AI highlights that our tool can help ML practitioners identify and understand model biases.
