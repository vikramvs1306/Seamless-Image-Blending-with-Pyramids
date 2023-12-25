Image Blending using Image Pyramids

This project demonstrates the technique of image blending using image pyramids, specifically utilizing the concept of Gaussian and Laplacian pyramids. The process creates visually appealing blended images by combining features from two source images.

Key Concepts:
- Image Pyramids: Tools for downscaling and upscaling images.
- Gaussian Pyramid: Used for smoothing and reducing the resolution.
- Laplacian Pyramid: Captures the image details.

Steps for Image Blending:
1. Load two source images and a mask image.
2. Construct Gaussian pyramids for both source images and the mask.
3. Build Laplacian pyramids from the Gaussian pyramids for the two source images.
4. Blend each level of the Laplacian pyramids according to the corresponding level of the Gaussian pyramid mask.
5. Reconstruct the blended image from the blended Laplacian pyramid by expanding and adding levels.

The Python code utilizes OpenCV and NumPy libraries for image processing and the Matplotlib library for displaying the results.

Key Functions:
- `resize_mask`: Adjusts the mask size to match the image dimensions.
- `build_gaussian_pyramid`: Generates a Gaussian pyramid for a given image.
- `build_laplacian_pyramid`: Creates a Laplacian pyramid from a Gaussian pyramid.
- `blend_pyramids`: Blends two image pyramids based on a mask pyramid.
- `reconstruct_image`: Reconstructs an image from its Laplacian pyramid.

Implementation:
- Reading of images and mask using OpenCV.
- Generation of Gaussian and Laplacian pyramids for both images.
- Blending of the pyramids and reconstruction of the final image.
- Normalization and saving of the blended image.
- Display of the final blended image.

This project provides a practical application of image pyramids in the context of image blending, showcasing the effectiveness of multi-scale image processing techniques.
