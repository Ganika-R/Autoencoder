## Aim
To implement an Autoencoder using the MNIST dataset for dimensionality reduction, image reconstruction, and visualization of latent-space representations.

## Dataset
- **Dataset:** MNIST Handwritten Digits Dataset
- **Training Images:** 60,000
- **Testing Images:** 10,000
- **Image Size:** 28 × 28 pixels
- **Original Dimension:** 784

## Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn

## Tasks Performed

### Task A: Dataset Preparation
- Loaded the MNIST handwritten digits dataset.
- Explored the dataset shape, data type, and pixel value range.
- Displayed sample handwritten digit images.
- Normalized pixel values between 0 and 1.
- Reshaped images from 28 × 28 into 784-dimensional vectors.

### Task B: Implementing the Autoencoder
- Implemented an Encoder and Decoder using Dense layers.
- Used ReLU activation in hidden layers.
- Used a bottleneck layer with 32 neurons.
- Used Sigmoid activation in the output layer.
- Combined the Encoder and Decoder to build the complete Autoencoder.
- Compiled the model using the Adam optimizer and Mean Squared Error (MSE) loss function.

### Task C: Model Training and Performance Evaluation
- Trained the Autoencoder for 20 epochs.
- Used a batch size of 256.
- Evaluated the model using test reconstruction loss.
- Plotted training and validation loss.
- Compared original images with reconstructed images.

### Task D: Dimensionality Reduction and Feature Visualization
- Extracted latent-space representations using the Encoder.
- Reduced the feature representations from 32 dimensions to 2 dimensions using PCA.
- Visualized the latent features based on digit classes.
- Compared original and decoded images.
- Saved the trained Encoder, Decoder, and Autoencoder models.

## Model Architecture

**Encoder:**
- Input Layer: 784 neurons
- Hidden Layer: 128 neurons (ReLU)
- Bottleneck Layer: 32 neurons (ReLU)

**Decoder:**
- Input Layer: 32 neurons
- Hidden Layer: 128 neurons (ReLU)
- Output Layer: 784 neurons (Sigmoid)

## Dimensionality Reduction

- Original Dimension: 784
- Compressed Dimension: 32
- Reduction: 784 → 32

## Results
- Successfully implemented and trained an Autoencoder.
- Compressed MNIST images into 32-dimensional latent representations.
- Visualized latent features using PCA.
- Reconstructed handwritten digit images.
- Plotted training and validation loss to evaluate model performance.
- Saved the trained models as `.keras` files.

## Saved Models
- `Encoder.keras`
- `Decoder.keras`
- `Autoencoder.keras`

## Conclusion
Successfully implemented an Autoencoder using the MNIST dataset. The model performed dimensionality reduction from 784 to 32 dimensions, visualized latent-space features using PCA, and reconstructed handwritten digit images.
