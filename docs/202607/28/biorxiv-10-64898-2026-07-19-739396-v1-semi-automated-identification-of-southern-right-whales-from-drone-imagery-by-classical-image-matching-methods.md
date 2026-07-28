---
title: Semi-automated identification of southern right whales from drone imagery by classical image matching methods
title_zh: 基于经典图像匹配方法的无人机影像南露脊鲸半自动识别
authors: "Fabry, B., Jacobs, G., Bartl, J., Fabry, M."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.19.739396v1.full.pdf"
tags: ["query:drone-vg-det"]
score: 6.0
evidence: 利用无人机图像进行目标识别
tldr: "南露脊鲸个体识别依赖头部胼胝体图案，手动比对大规模目录耗时费力。现有自动化方法需要大量训练数据或重训练，难以用于小型无人机目录。本研究评估了HOG和对称对数倒角距离两种经典图像相似性方法，在标准化头部图像上测试375个查询。HOG首次匹配正确率96.3%，对数倒角94.7%，结合风险评分后提升至98.1%。结果表明经典配准图像匹配是一种实用工具，无需深度学习即可高效识别。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 569, \"height\": 426, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 568, \"height\": 258, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1209, \"height\": 788, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 631, \"height\": 261, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1155, \"height\": 1798, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1119, \"height\": 1085, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1104, \"height\": 705, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1633, \"height\": 668, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739396-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1288, \"height\": 2008, \"label\": \"Figure\"}]"
motivation: 手动比对南露脊鲸头部胼胝体图案费时，现有自动化方法需大量训练数据或重训练，难以用于小型无人机目录。
method: 使用HOG和对称对数倒角距离两种经典图像相似性方法，从标准化无人机头部图像中进行匹配识别。
result: "HOG rank-1准确率96.3%（361/375），对数倒角94.7%（355/375），结合风险评分后达98.1%（368/375）。"
conclusion: 经典配准图像匹配方法无需大量训练数据，可有效应用于南露脊鲸无人机照片的个体识别。
---

## 摘要
每头南露脊鲸（Eubalaena australis）可通过头部角质化粗糙斑块组成的稳定图案——胼胝体模式进行个体识别。然而，将无人机影像与大型目录进行手动比对非常耗时。对于南露脊鲸而言，自动化照片识别在小型或不断增长的无人机目录中仍难以常规实施，因为许多方法需要大量训练数据或在新增个体时重新训练。本文评估了两种用于标准化背部头部图像个体识别的经典图像相似性方法：定向梯度直方图（HOG）和对称对数倒角距离。我们使用来自198头已知重复观测鲸鱼的375张查询图像，对411张个体参考图像进行测试。HOG在375例中有361例（96.3%）首次将正确鲸鱼排名第一，而对数倒角在355例（94.7%）中排名第一。所有错误的rank-1匹配均可通过查询-参考距离分布计算的高风险分数识别。一种结合规则，从风险分数较低的方法中选择排名第一的候选者，将rank-1准确率提高到368例（98.1%）。这些结果表明，经典配准图像匹配为南露脊鲸照片识别提供了一种实用工具。

## Abstract
Individual southern right whales (Eubalaena australis) can be identified from the callosity pattern on the head, a stable pattern of roughened keratinized patches. Manual comparison of drone images with large catalogs, however, is time-consuming. For southern right whales, automated photo-identification remains difficult to implement routinely in small or growing drone-based catalogs, because many approaches require substantial training data or retraining when new individuals are added. Here we evaluate two classical image-similarity methods for individual identification from standardized dorsal head images: histograms of oriented gradients (HOG) and a symmetric log-chamfer distance. We tested 375 query images from 198 known whales with recurrent sightings against 411 reference images of as many individual whales. HOG ranked the correct whale first in 361 of 375 cases (96.3%), whereas log-chamfer ranked the correct whale first in 355 cases (94.7%). All incorrect rank-1 matches could be identified by a high risk score computed from query-reference distance distributions. A combined rule selecting the first-ranked candidate from the method with the lower risk score increased rank-1 accuracy to 368 cases (98.1%). These results show that classical registered image matching provides a practical tool for southern right whale photo-identification.