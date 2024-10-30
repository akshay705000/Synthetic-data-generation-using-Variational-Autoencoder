
# Synthetic Data Generation using Variational Autoencoder (VAE)

This project focuses on generating high-quality synthetic data for credit card transactions using Variational Autoencoders (VAE). The synthetic dataset retains key statistical characteristics of the original dataset while ensuring data uniqueness and no duplicates. This solution is particularly valuable for secure data sharing and experimentation without compromising privacy.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Pipeline Description](#pipeline-description)
- [Results](#results)

## Project Overview
The **Synthetic Data Generation using VAE** project is designed to generate realistic synthetic data that maintains the statistical integrity of the original dataset. Using a VAE, the model captures latent representations of the data and samples from this latent space to produce unique and realistic synthetic data points.

## Features
- **Data Preprocessing Pipeline**:
  - Handling of missing values
  - Timestamp formatting
  - Encoding of categorical variables
  - Normalization of numerical data

- **Synthetic Data Generation**:
  - Utilizes a Variational Autoencoder (VAE) to generate synthetic transactions
  - Produces 2 million unique transactions with preserved statistical features
  - Ensures data uniqueness and non-duplication

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Synthetic-Data-Generation-VAE.git
   cd Synthetic-Data-Generation-VAE
   ```

2. Install the required dependencies, run the code and generate results:
   ```bash
   run the attached .ipynb file
   ```
## Pipeline Description
1. **Data Preprocessing**:
   - **Missing Values**: Fills in or discards rows based on pre-defined thresholds.
   - **Timestamp Formatting**: Converts timestamps to a uniform format.
   - **Encoding**: Categorical features are label encoded or one-hot encoded.
   - **Normalization**: Applies standardization for numeric fields to improve model performance.

2. **VAE Model Architecture**:
   - **Encoder**: Encodes the input data into a lower-dimensional latent space.
   - **Latent Space Sampling**: Samples from the latent space, following a normal distribution.
   - **Decoder**: Reconstructs synthetic data points from the sampled latent space.

3. **Data Generation**: Generates synthetic data by sampling from the learned latent space and reconstructing it through the decoder.

## Results
- Generated a synthetic dataset of **2 million unique transactions**.
- Maintained the **statistical properties** of the original dataset while ensuring no duplicate data points.
- Successfully preserved feature distributions, which can be verified using evaluation metrics.
