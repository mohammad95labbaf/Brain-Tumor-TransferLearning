# Brain-Tumor-TransferLearning

### Dataset:
- The dataset utilized for this study is the **Brain Tumor MRI Dataset** sourced from Kaggle.
- It consists of a carefully curated collection of brain MRI scans specifically chosen to facilitate research in automated brain tumor detection and classification using the Keras library.
- The dataset aims to enhance diagnostic accuracy and includes a randomized subset (20% of the original data) categorized into 'yes' (tumor present) and 'no' (healthy) tumor classes for both training and validation purposes.

### Investigated Approaches:

1. **VGG16 + FC (VGG16 with Fully Connected Layers)**:
   - VGG16 is a deep CNN architecture comprising 16 weight layers.
   - It was pre-trained on the ImageNet dataset.
   - Additional fully connected layers are incorporated for classification.

2. **VGG + CNN2D (VGG16 with Additional Convolutional Layers)**:
   - This approach extends VGG16 by introducing more convolutional layers for enhanced feature extraction.

3. **ResNet50 + FC (ResNet50 with Fully Connected Layers)**:
   - ResNet50, a deep residual network with 50 layers, addresses the vanishing gradient problem using skip connections.
   - Fully connected layers are added for classification.

4. **ResNet50 + CNN2D (ResNet50 with Additional Convolutional Layers)**:
   - Building upon ResNet50, this variant incorporates additional convolutional layers.

5. **ViT (Vision Transformer) + FC (Fully Connected Layers)**:
   - Originally designed for natural language processing, ViT is a transformer-based architecture.
   - It has been adapted for image classification by treating images as sequences of patches.
   - Fully connected layers are employed for classification⁷.

### Investigation Objectives:
- Evaluate the effectiveness of transfer learning using pre-trained models (VGG16, ResNet50, and ViT) for brain tumor classification.
- Compare the performance of different architectures in terms of accuracy, sensitivity, specificity, and other relevant metrics.
- Gain insights into how transfer learning impacts model convergence, generalization, and robustness.


## Instructions for Kaggle API
1. **Download Kaggle API**:
    - Install the Kaggle API by running `pip install kaggle`.

2. **Kaggle API Token**:
    - Go to your Kaggle account settings and generate an API token.
    - Save the token as `kaggle.json` in the root directory of this repository.

3. **Download Dataset**:
    - Use the Kaggle API to download the dataset:
        ```
        kaggle datasets download -d  preetviradiya/brian-tumor-dataset
        ```

4. **Upload Kaggle API Token to Colab/Notebook**:
    - If using Colab or Jupyter Notebook, upload the `kaggle.json` token to your environment.
    - Use the following code snippet:
        ```python
        from google.colab import files
        files.upload()
        ```

5. **Unzip Dataset**:
    - Unzip the downloaded dataset:
        ```
        unzip brian-tumor-dataset.zip
        ```
