# Visual Localization with OrienterNet

This repository contains a Google Colab notebook that demonstrates visual localization using the **OrienterNet** model. Given an image and a coarse location prior, this project can determine the precise geo-pose (latitude, longitude, and orientation) of the camera.

This implementation leverages the official [OrienterNet repository](https://github.com/facebookresearch/OrienterNet) from Facebook Research and uses **OpenStreetMap** for map data.

## Getting Started

### Prerequisites

* A Google Account to run the Colab notebook.
* An image for which you want to determine the location. You can also use the example images provided in the notebook.
* A coarse location (e.g., an address) for the image.

### Running the Notebook

1.  Open the `Slam.ipynb` notebook in Google Colab.
2.  Follow the instructions in the notebook and run the cells sequentially.
3.  The notebook will first clone the OrienterNet repository and install the necessary dependencies.
4.  You can either choose one of the example images or upload your own.
5.  Provide a coarse location prior for your image.
6.  The notebook will then run the OrienterNet model to predict the precise location and orientation.

## How it Works

The notebook uses the following steps for visual localization:

1.  **Input**: An image and a coarse location (address).
2.  **Map Query**: Queries OpenStreetMap for the map data around the given coarse location.
3.  **Model Inference**: Uses the pre-trained OrienterNet model to compare the input image with the map data and predict the camera's pose.
4.  **Output**: Visualizes the predicted location and orientation on the map.

## Results

Here are some example visualizations from the notebook:

**Input Image and OpenStreetMap Raster:**

**Location Prior on the Map:**

*(You can replace the above placeholders with actual screenshots from your notebook's output.)*

## Acknowledgments

This project is based on the following research paper:

> **OrienterNet: Visual Localization and Orientation Estimation using OpenStreetMap**
>
> [GitHub Repository](https://github.com/facebookresearch/OrienterNet)

Special thanks to the authors of OrienterNet for making their code publicly available.
