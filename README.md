# Embedding-Level Geometric Evaluation of Face Anonymization

This repository contains the experimental code for evaluating face anonymization strength at the embedding level using ArcFace representations and PCA-based geometric analysis.

## Overview

The study compares three regimes:

- Original images
- Gaussian blur anonymization
- GAN-based identity swapping

Identity separability is evaluated in embedding space using:

- PCA projection
- Intra-class variance
- Inter-centroid distance
- Explained variance ratio

## Dataset

Experiments were conducted using a subset of the LFW dataset (100 identities × 10 images each).

## Methodology

1. ArcFace embeddings (512-D) are extracted using InsightFace.
2. Embeddings are standardized and projected using PCA.
3. Identity separability metrics are computed.
4. Geometric changes across anonymization regimes are analyzed.

## Reproducibility

To run the notebook:

1. Install dependencies:

pip install -r requirements.txt

2. Open the notebook in Google Colab.
3. Upload the LFW dataset archive.
4. Run all cells sequentially.

## Notes

The implementation is intended for research and academic reproducibility purposes.
