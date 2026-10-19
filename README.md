# Image Splicing Detection through Noise Variance

A CS663 image-processing group project at IIT Bombay.

## Approach

- Computes DCT-domain statistics to estimate global and local image noise variance.
- Uses local 8×8 DCT features and 32×32 aggregation windows to construct a noise-variance map.
- Clusters the local map with two-class K-means to visualize candidate regions with inconsistent noise.
- Explores the global estimator under added Gaussian noise.

## Materials

- [Local noise estimation and segmentation](notebooks/local_noise_splicing.ipynb)
- [Global noise experiment](notebooks/global_noise_variance.ipynb)
- [Team presentation](presentations/CS663_Image_Splicing.pptx)

## Setup

Install dependencies with `pip install -r requirements.txt` and open the notebooks with `jupyter lab`. The local notebook imports `google.colab.patches`; run it in Google Colab or replace the display helper for local use.

Test images are not included. Replace the original `/content/` and Windows image paths with your own input images.
