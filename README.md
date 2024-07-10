# K-means Image contour detector
This project was developed as part of the subject VC (Computer Vision) at FIB - UPC Barcelona, using Matlab. It implements a system for segmenting objects in images using the K-means clustering algorithm. The system allows users to manually indicate the object to segment with a rectangular box, and then segments it, marking its outline in red. <br><br>

## Objective

Implement a system that detects the contourn of objects in color images where the object is distinguishable from the background by its color. <br><br>

> [!IMPORTANT]
> Dependencies: MATLAB with Image Processing Toolbox <br><br>
> You can find the detailed project process in the document titled  *project_structure_and_results.pdf*

<br>
    
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
- Use these decisions to segment the object and display the result. <br><br>


## Results

The method works well when the object is clearly distinguishable from the background in terms of color and when the object is centered in the image. However, the method may struggle with images where the object is not centered or the background has similar colors to the object. <br><br>

## How to Use

- Launch Matlab application.
- Load your image.
- Run the script and manually select the object using a rectangular box.
- The segmented object will be displayed with its outline marked in red.

<br><br>

    
---

## Screenshots

Project step by step:

![Screenshot from 2024-07-10 21-14-33](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/906cc088-78eb-4c4c-96e6-7aa1d9aa60ec)

![Screenshot from 2024-07-10 21-14-44](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/b1d7f6c7-fd74-4a52-872b-042d68056076)

![Screenshot from 2024-07-10 21-15-01](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/8d16c172-0052-4f5d-948e-b277dc018b03)

![Screenshot from 2024-07-10 21-15-32](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/88ac3f51-b387-4888-ad1b-53ebe637a139)

![Screenshot from 2024-07-10 21-15-43](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/0bc3c2fd-3c48-4a42-a6b2-337771a50adb)

Another result:

![resultat1](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/a96484c1-40c3-47c4-9e35-f1208b8331ea) 

<br><br>

K-means color clustering results I love:

![cheetah](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/712db451-f35f-4e79-9e32-92b4f5c3a7c2)

![cheetah7](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/9eb68546-63d6-497b-aac5-c6697875be14)

![lion](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/70e4dc8f-6986-4702-86f3-64588639070d)

![tiger1](https://github.com/ArnauCS03/k-means-image-contour-detector/assets/95536223/c78b626f-e4c1-44b8-b41c-1e1d583f6368)


<br><br>
