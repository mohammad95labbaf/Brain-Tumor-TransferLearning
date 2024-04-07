# Brain-Tumor-TransferLearning


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
