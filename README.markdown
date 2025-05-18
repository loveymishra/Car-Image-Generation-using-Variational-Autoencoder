# Car Image Generation using Variational Autoencoder

This project trains a Variational Autoencoder (VAE) on a dataset of car images to generate new car-like images. The code is implemented in Python using TensorFlow and Keras, and is provided in a Jupyter notebook.

## Dataset
The dataset used is "the-car-connection-picture-dataset" from Kaggle: [Kaggle Dataset Link](https://www.kaggle.com/datasets/prondeau/the-car-connection-picture-dataset).

## Prerequisites
- Python 3.x
- Required libraries (install via `pip install -r requirements.txt`):
  - `tensorflow`
  - `numpy`
  - `matplotlib`
  - `kaggle`

- Kaggle API credentials (`kaggle.json`). Obtain it from your Kaggle account and place it in the Colab environment or `~/.kaggle/` locally.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/car-vae-tutorial.git
   cd car-vae-tutorial
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the dataset using the Kaggle API (ensure `kaggle.json` is set up):
   ```bash
   kaggle datasets download -d prondeau/the-car-connection-picture-dataset
   unzip -q the-car-connection-picture-dataset.zip -d dataset
   ```

## Usage
1. Open the Jupyter notebook `car_vae_tutorial.ipynb` in Colab or locally:
   ```bash
   jupyter notebook car_vae_tutorial.ipynb
   ```
2. Run the notebook cells to:
   - Download and preprocess the dataset.
   - Build and train the VAE model.
   - Generate new car images.
3. Adjust parameters like `latent_dim` or `epochs` in the notebook as desired.

## Results
The notebook generates 16 new car images after training, displayed in a 4x4 grid. Results depend on training duration and hyperparameters.

## Try it on Colab
Run the notebook directly in Google Colab with GPU acceleration:  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yourusername/car-vae-tutorial/blob/main/car_vae_tutorial.ipynb)

## Tutorial
For a detailed step-by-step tutorial, read the Medium article: [Generating Car Images with Variational Autoencoders](https://medium.com/@loveymishra60/car-image-generation-using-variational-autoencoder-281b0707789d).

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions.

## License
This project is licensed under the MIT License.
