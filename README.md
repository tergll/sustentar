# Sustentar recycling
## Project Definition
This project aims to analyze recycling behavior across different residential areas using computer vision. By detecting and categorizing objects in waste images, it identifies patterns in how communities sort their recyclables. The goal is to uncover discrepancies or inefficiencies between areas and use this data to inform targeted policy changes or educational interventions. Ultimately, it enables a data-driven approach to improving recycling compliance and environmental impact.


This repo is mainly for collecting the collab notebooks for the project in one place

## Code notebooks
**1. Demonstrating how object detection by "Yolo" model works + cropping to zoom into the desk:**

https://colab.research.google.com/drive/1CVTBW4LzLCr6rbmZ6yEzN3RwXJDm5qrv?usp=sharing

This notebook demonstrates how to crop the top portion of selected images and use a YOLO object detection model to identify and visualize specific objects within the cropped sections. It refines the detection process by adjusting the confidence threshold to capture even faint object predictions, allowing users to see more detailed results. The workflow is ideal for testing detection accuracy on manually prepared images from a recycling context or household setting.

**2. Using "Yolo" model to categorize objects and crop around that object:**

https://colab.research.google.com/drive/16k7_Abm5hh9VLqV-T7k6OfQDCckvxewc?usp=sharing

This notebook automatically processes a collection of recycling-related photos by first cropping the relevant part of each image, then using a YOLO object detection model to identify and extract specific objects (like tables, bottles, or bags). Each detected object is saved into folders categorized by type, allowing for organized analysis or further use. The entire process is designed to automate visual sorting and object isolation from real-world environmental images.

**3. Clustering**

https://colab.research.google.com/drive/1LwI4KhkRTpGnrKtJijNV-7sY_gQ2LCiC?usp=sharing

This notebook clusters similar-looking images using deep learning and unsupervised clustering. It begins by extracting a zipped folder of object images, excluding one category (dining table), and consolidates them into a single directory. It then uses a pre-trained ResNet18 model to extract feature embeddings from each image, representing their visual content. These embeddings are clustered using DBSCAN and Agglomerative Clustering to group similar images. The results are visualized both through image grids and a 2D map using t-SNE for dimensionality reduction. The pipeline combines PyTorch for feature extraction, scikit-learn for clustering and visualization, and OpenCV/Matplotlib for image processing and plotting.

