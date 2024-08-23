# Jupyter (Modern) Museum

## Overview

The **Jupyter (Modern) Museum** project explores the intersection of art and technology by applying computer vision techniques to famous artworks. The primary goal is to analyze and manipulate these artworks, providing both visual and technical insights. The project is divided into two main parts: the first focuses on color quantization and cartooning of images, while the second allows users to create "pop art" versions of these images through interactive widgets.

## Objectives

### Part 1: Color Quantization and Cartooning

The first part of the project involves analyzing three iconic artworks from different artistic movements, each created using distinct techniques and with different artistic goals. The objective is to highlight these goals by performing color quantization using the k-means algorithm, which simplifies the image chromatically by mapping each pixel to the nearest of the `k` most frequent colors in the painting. The quantized image is then combined with enhanced edges to create a cartoon-like version of the original.

### Part 2: Pop Art Effect

The second part of the project is more technical and builds on the cartoonized images. It allows users to create "pop art" versions of these images by altering the colors according to their preferences. This is done through an interactive interface where users can select and replace colors, creating unique artistic expressions inspired by the pop art movement.

## Tools and Libraries

The project makes use of the following tools and libraries:

- **OpenCV**: For image processing and edge detection.
- **Matplotlib**: For image visualization.
- **NumPy**: For numerical computations.
- **SciPy**: For convolution operations during edge detection.
- **scikit-image**: For image conversion between different formats.
- **IPython Widgets**: For creating an interactive user interface.

## Workflow

### Test Case 1: "Mona Lisa" by Leonardo da Vinci

1. **Edge Detection**: Convert the image to grayscale and apply a bilateral filter to preserve edges while reducing noise. The Sobel operator is used to detect edges, and an interactive slider allows the user to adjust the edge detection threshold.

2. **Color Quantization**: The k-means algorithm is implemented to reduce the number of colors in the image. The algorithm iterates to minimize distortion until a low distortion threshold is achieved, yielding a simplified, cartoon-like version of the image.

3. **Combination**: The quantized image is combined with the detected edges to produce the final cartoonized image.

### Test Case 2: "Madonna" by Edvard Munch

Similar to the first test case, the image is processed to enhance its emotional intensity. The color quantization and edge detection emphasize the dark background and the contrast between the figures, enhancing the artwork's emotive impact.

### Pop Art Effect

An interactive interface allows users to apply a pop art effect to the cartoonized images. Users can select specific pixels and alter their colors using sliders that control the red, green, and blue color channels. The updated image is displayed in real-time, and users can save their final creation.

## How to Use

1. **Installation**: Clone the repository and install the required Python libraries.
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   pip install -r requirements.txt
   ```

2. **Running the Notebook**: Open the Jupyter notebook and execute the cells in order. The notebook provides step-by-step instructions and interactive widgets.

3. **Customization**: Modify the parameters in the notebook to experiment with different values for color quantization, edge detection, and pop art effects.

4. **Saving Results**: The notebook allows you to save your final images by clicking the "Save Image" button after applying the pop art effect.

## Observations

- **Mona Lisa**: The cartoonization emphasizes the focus on the subject, blurring the background and retaining the distinct features of the woman's face.
- **Madonna**: The quantization enhances the emotional intensity, accentuating the dark, brooding background against the light skin tones of the figures.

## Conclusion

The Jupyter (Modern) Museum project offers a unique blend of art and technology, allowing users to explore the effects of modern image processing techniques on classical artworks. Through this project, we gain insights into both the technical and artistic aspects of image manipulation, providing a platform for further exploration and creativity.
