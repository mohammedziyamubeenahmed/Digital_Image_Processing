# Fourier Descriptor-Based Shape Reconstruction (MATLAB GUI)

A MATLAB-based interactive application for extracting object boundaries from images, computing Fourier descriptors, and reconstructing shapes using a user-defined percentage of retained Fourier coefficients.

This project demonstrates classical shape representation and reconstruction using Discrete Fourier Transform (DFT) integrated into a graphical user interface.

---

## 🚀 Features

### 1️⃣ Graphical User Interface (GUI)
- Load image files
- Select processing operations
- Specify percentage of Fourier coefficients
- Visualize intermediate and reconstructed outputs
- Save computed Fourier descriptors

### 2️⃣ Closed Boundary Edge Extraction
- Convert image to grayscale
- Perform edge detection
- Apply morphological closing to ensure a closed contour
- Extract boundary points of the primary object

### 3️⃣ Fourier Descriptor Computation

Boundary points are converted into complex representation:

\[
z_k = x_k + i y_k
\]

The Discrete Fourier Transform (DFT) is applied to generate the Fourier descriptor.

### 4️⃣ Shape Reconstruction

- User selects percentage of Fourier coefficients to retain
- Higher frequencies are truncated
- Inverse DFT reconstructs the boundary
- Visualization of original vs reconstructed shape

### 5️⃣ Descriptor Saving

- Save Fourier coefficients to `.mat` file
- Enables reuse and further analysis

---

## 🧠 Methodology

1. Load input image
2. Perform edge detection (e.g., Canny)
3. Apply morphological operations (closing)
4. Extract ordered boundary points
5. Compute DFT of boundary sequence
6. Retain selected percentage of coefficients
7. Perform inverse DFT for reconstruction
8. Visualize comparison

---

## 🛠️ Requirements

- MATLAB R2021a or later
- Image Processing Toolbox



