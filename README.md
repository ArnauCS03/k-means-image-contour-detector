# K means Image contour detector
This project was developed as part of the subject VC (Computer Vision) at FIB - UPC Barcelona, using Matlab. It implements a system for segmenting objects in images using the K-means clustering algorithm. The system allows users to manually indicate the object to segment with a rectangular box, and then segments it, marking its outline in red.

## Objective

Implement a system that detects the contourn of objects in color images where the object is distinguishable from the background by its color.

## Procedure

User Input for Object Selection:
- The user indicates the object to segment by drawing a rectangular box around it.

Convert Image to HSV:
- Convert the image from RGB to HSV format to handle the cyclic nature of the hue component.

K-means Clustering:
- Apply K-means clustering on the HSV components to group colors into k clusters.
- Experiment with different values of k (between 4 and 10).

Determine Object Colors:
- Identify which color clusters primarily fall within the user-defined rectangle.
- Create a mask indicating the object region.

Segmentation Decision:
- Compare the frequency of each color inside and outside the rectangle to decide which colors belong to the object.
- Use these decisions to segment the object and display the result.

---

## Screenshots
