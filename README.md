Identity-Preserving Facial Age Progression via StyleGAN2

[![ML](https://img.shields.io/badge/ML-Generative%20AI-blue)](#) 
[![Framework](https://img.shields.io/badge/Framework-PyTorch-red)](#)
[![Impact](https://img.shields.io/badge/Impact-Missing%20Persons-green)](#)

Project Overview
This project implements a sophisticated machine learning algorithm designed to simulate facial evolution across time while strictly preserving the underlying identity of the subject. Developed as a potential solution for identifying missing persons from outdated childhood photographs, this system addresses a critical social challenge: the **3.8 lakh unresolved missing person cases in India**.

By leveraging **StyleGAN2** and advanced latent space manipulation, the model ensures that facial aging is realistic rather than just a cosmetic filter, maintaining the unique biometric characteristics required for identification.

Technical Architecture
The core challenge of age progression is preventing "identity drift" during the aging process. This project solves this by combining generative power with geometric and facial recognition constraints:

* **StyleGAN2 Backbone**: Utilized for high-fidelity facial synthesis and a well-structured latent space
* **Latent Code Manipulation**: Employs a dual approach for editing latent vectors, including **SeFa (Semantic Factorization)** to isolate age-related factors
* **Identity Constraint (ArcFace)**: Integrated **ArcFace similarity scoring** to calculate and minimize identity loss between the source and the generated aged image
* **Precision Masking**: Applied **face-parsing masks** to ensure that modifications are localized to aging features (like skin texture and bone structure) without distorting key identifiers like eye shape or facial proportions

Key Features
* **High Fidelity**: Maintains resolution and realistic textures across different age milestones
* **Identity Preservation**: Specifically calibrated to pass facial recognition benchmarks even after significant age transformation
* **Attention-Guided Editing**: Uses attention mechanisms to ensure latent edits are focused on relevant facial regions

Impact & Vision
> "Every single iteration of this model contributed to my knowledge of generative models, shifting my focus from building simple solutions to architecting sophisticated AI products."

This project represents the intersection of **technical engineering** and **social responsibility**. Beyond its humanitarian applications, the underlying technology of identity-consistent attribute manipulation has significant applications in the **cosmetic and fashion industries** for virtual aging and skin-care efficacy visualization.

Tech Stack
* **Language**: Python 
* **Deep Learning**: PyTorch 
* **Computer Vision**: StyleGAN2, ArcFace, SeFa 

