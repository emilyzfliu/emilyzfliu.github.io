---
title: "Structured Latent Variable Models for Articulated Object Interaction"
collection: papers
# category: manuscripts
permalink: /_papers/2023-05-26-structured-lvms
excerpt: 'This paper explores how a robot can learn a low-dimensional representation of doors from videos of them opening or closing, enabling the inference of door-related parameters and interaction outcomes. Instead of relying solely on labeled datasets, the study employs a semi-supervised approach using the Neural Statistician, a structured latent variable model that separates shared context-level variables (common across all images of the same door) from instance-level variables (specific to each image). The model effectively generates realistic door image embeddings, which outperform context-free baselines in tasks such as predicting door parameters and optimizing actions in a visual bandit door-opening scenario, demonstrating its utility for more efficient and accurate robotic interaction.'
date: 2023-05-26
# venue: 'Journal 1'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2305.16567'
citation: 'Structured Latent Variable Models for Articulated Object Interaction. Emily Liu, Michael Noseworthy, Nicholas Roy. 2023.'
---

In this paper, we investigate a scenario in which a robot learns a low-dimensional representation of a door given a video of the door opening or closing. This representation can be used to infer door-related parameters and predict the outcomes of interacting with the door. Current machine learning based approaches in the doors domain are based primarily on labelled datasets. However, the large quantity of available door data suggests the feasibility of a semisupervised approach based on pretraining. To exploit the hierarchical structure of the dataset where each door has multiple associated images, we pretrain with a structured latent variable model known as a neural statistician. The neural satsitician enforces separation between shared context-level variables (common across all images associated with the same door) and instance-level variables (unique to each individual image). We first demonstrate that the neural statistician is able to learn an embedding that enables reconstruction and sampling of realistic door images. Then, we evaluate the correspondence of the learned embeddings to human-interpretable parameters in a series of supervised inference tasks. It was found that a pretrained neural statistician encoder outperformed analogous context-free baselines when predicting door handedness, size, angle location, and configuration from door images. Finally, in a visual bandit door-opening task with a variety of door configuration, we found that neural statistician embeddings achieve lower regret than context-free baselines.