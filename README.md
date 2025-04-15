# Sustenar recycling
This repo is mainly for collecting the collab notebooks for the project in one place

## Code notebooks
1. object detection by Yolo model
https://colab.research.google.com/drive/1pFUs0gRgmhuyleHZtbZSoagFGu0xfLII?usp=sharing
2. image cropping
https://colab.research.google.com/drive/16k7_Abm5hh9VLqV-T7k6OfQDCckvxewc?usp=sharing
3. clustering
https://colab.research.google.com/drive/1bWlFeIpzswzjFRPdvYif4otORD-p28rw?usp=sharing

## Detailed explanation for each notebook

1. This notebook demonstrates how to crop the top portion of selected images and use a YOLO object detection model to identify and visualize specific objects within the cropped sections. It refines the detection process by adjusting the confidence threshold to capture even faint object predictions, allowing users to see more detailed results. The workflow is ideal for testing detection accuracy on manually prepared images from a recycling context or household setting.
2. This notebook automatically processes a collection of recycling-related photos by first cropping the relevant part of each image, then using a YOLO object detection model to identify and extract specific objects (like tables, bottles, or bags). Each detected object is saved into folders categorized by type, allowing for organized analysis or further use. The entire process is designed to automate visual sorting and object isolation from real-world environmental images.
3. This notebook clusters similar-looking images using deep learning and unsupervised clustering. It begins by extracting a zipped folder of object images, excluding one category (dining table), and consolidates them into a single directory. It then uses a pre-trained ResNet18 model to extract feature embeddings from each image, representing their visual content. These embeddings are clustered using DBSCAN and Agglomerative Clustering to group similar images. The results are visualized both through image grids and a 2D map using t-SNE for dimensionality reduction. The pipeline combines PyTorch for feature extraction, scikit-learn for clustering and visualization, and OpenCV/Matplotlib for image processing and plotting.
