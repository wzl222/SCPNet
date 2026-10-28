SCPNet: Scattering-Consistency-Constrained Underwater Image Enhancement

Official PyTorch implementation of SCPNet, a physics-guided underwater image enhancement framework based on scattering-consistency constraints.

Paper: SCPNet: Scattering-Consistency-Constrained Underwater Image Enhancement
Conference: Asian Conference on Machine Learning (ACML 2026)

Introduction

Underwater images often suffer from color distortion, low contrast, and loss of structural details due to wavelength-dependent light attenuation and scattering. Although deep learning methods have achieved promising results, purely data-driven approaches may produce visually plausible results that are inconsistent with underwater image formation physics.

To address this issue, we propose SCPNet, a physics-guided underwater image enhancement framework that incorporates scattering-consistency constraints into the network optimization process.

SCPNet jointly predicts the enhanced image, a latent scattering intensity map, and a global backscatter color. A differentiable scattering reconstruction process is introduced to establish consistency between the enhanced result and the observed underwater image.

Method Overview

SCPNet consists of three main components:

1. Image Restoration Backbone

An encoder-decoder architecture extracts multi-scale features and reconstructs enhanced underwater images.

2. Scattering Parameter Estimation

Two prediction heads estimate a latent scattering intensity map and a global backscatter color to characterize the underwater degradation process.

3. Scattering-Consistency Constraint

A differentiable scattering reconstruction mechanism provides an auxiliary physics-guided training objective, encouraging consistency between the restored image and the observed underwater image.

The framework combines data-driven image restoration with approximate underwater imaging physics.

Network Architecture

[Insert the SCPNet architecture figure here.]
