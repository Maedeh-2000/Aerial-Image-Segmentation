# Aerial Image Segmentation & Land-Cover Classification

A pattern recognition and geospatial machine learning project focused on segmenting and classifying high-resolution aerial imagery using RGB, infrared (IR), and Digital Surface Model (DSM) data.

The project explores both unsupervised image segmentation and supervised semantic classification using methods such as K-Means, SLIC superpixels, and Random Forest.

## Project Overview

The objective of this project was to investigate different approaches for extracting meaningful spatial objects and land-cover information from high-resolution aerial imagery.

The workflow combines image processing, segmentation, feature extraction, and machine learning classification.

### Main workflow

- Preparation of RGB, infrared, and DSM imagery
- Image exploration and preprocessing
- Chessboard segmentation
- K-Means clustering
- SLIC superpixel segmentation
- Feature extraction from image segments
- Random Forest classification
- Semantic land-cover prediction
- Evaluation and visualization of classification results

## Dataset

The project uses high-resolution aerial imagery from the **ISPRS Potsdam dataset**.

The available information includes:

- RGB imagery
- Infrared (IR) information
- Digital Surface Model (DSM)
- Reference land-cover labels

The combination of spectral and elevation information enables the analysis of both appearance and geometric characteristics of urban objects.

## Image Segmentation

Several segmentation approaches were investigated to divide the aerial imagery into meaningful regions.

### Chessboard Segmentation

A regular grid-based segmentation was used as a simple baseline for dividing the image into spatial units.

### K-Means Clustering

K-Means was applied as an unsupervised clustering method to group pixels or image regions based on similarity in their feature space.

### SLIC Superpixels

SLIC (Simple Linear Iterative Clustering) was used to generate compact superpixels that better follow object boundaries in the aerial imagery.

This provides more meaningful spatial units for subsequent feature extraction and classification.

## Semantic Classification

A **Random Forest classifier** was used for supervised land-cover classification.

Features derived from the available image channels and segmented regions were used to distinguish different land-cover categories.

The workflow demonstrates how traditional machine learning can be combined with object-based image analysis for semantic interpretation of aerial imagery.

## Tools & Technologies

- Python
- Jupyter Notebook
- NumPy
- Matplotlib
- scikit-learn
- scikit-image
- Random Forest
- K-Means
- SLIC Superpixels
- RGB / IR imagery
- Digital Surface Models (DSM)

## Key Skills Demonstrated

- Pattern recognition
- Geospatial machine learning
- Aerial image analysis
- Image segmentation
- Feature extraction
- Unsupervised learning
- Supervised classification
- Random Forest classification
- Object-based image analysis
- Geospatial data visualization

## Repository Structure

```text
Aerial-Image-Segmentation/
├── README.md
├── notebooks/
│   ├── image-segmentation.ipynb
│   └── semantic-classification.ipynb
└── images/
    └── project visualizations
