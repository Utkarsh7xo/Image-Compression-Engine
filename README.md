# JPEG-like Image Compression Engine

This repository contains a JPEG-like image compression engine built using Python and Jupyter Notebook. The project implements a simplified version of the JPEG compression algorithm for grayscale images, including key steps like Discrete Cosine Transform (DCT), quantization, and Huffman encoding.

---

## Features

1. **2D Discrete Cosine Transform (DCT):**  
   Computes the 2D DCT coefficients for non-overlapping image patches, a core step in JPEG compression.

2. **Quantization:**  
   Implements the quantization step to reduce precision in the DCT coefficients, allowing for higher compression ratios with minimal quality degradation.

3. **Huffman Encoding:**  
   Utilizes Huffman coding to further compress the quantized DCT coefficients. You can choose between custom or pre-built Huffman tree implementations.

4. **File Format for Compression:**  
   Compresses image data into a custom file format, which can later be read and displayed, accurately reconstructing the compressed image.

5. **Quality Factor Simulation:**  
   Simulates different compression quality factors and generates RMSE (Root Mean Squared Error) vs. BPP (Bits Per Pixel) curves, helping visualize the compression performance.

6. **Performance Analysis:**  
   Plots the RMSE vs. BPP graph for at least 20 different images, offering insights into the efficiency and quality of the image compression engine.

---

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Utkarsh7xo/Image-Compression-Engine.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd Image-Compression-Engine
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
   - Open the notebook file (`compression_engine.ipynb`).
   - Follow the steps to load images, apply compression, and visualize the results.

---

## File Structure

- **Photos/**: Folder containing sample grayscale images for testing the compression algorithm.
- **README.md**: This file.
- **requirements.txt**: A list of required Python libraries.

---

## Key Metrics

1. **Root Mean Squared Error (RMSE):**  
   A metric to measure the difference between the original and compressed images, used to evaluate compression quality.

2. **Bits Per Pixel (BPP):**  
   Measures the number of bits used per pixel in the compressed image, reflecting the compression ratio.

### RMSE vs. BPP Plot:
- The notebook simulates 20+ different images with varying compression quality factors, generating RMSE vs. BPP plots to analyze the trade-offs between compression efficiency and image quality.

---

## Dependencies

- Python 3.8 or higher
- Numpy
- Matplotlib
- OpenCV
- Pillow
- Jupyter Notebook

You can install the necessary dependencies using the following command:
```bash
pip install -r requirements.txt
```