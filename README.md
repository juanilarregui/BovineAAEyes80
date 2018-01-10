## Dataset description

The BovineAAEyes80 is a dataset comprising 80 RGB images of 11 different bovines belonging to Aberdeen-Angus breed. For each RGB image, there are three accompanying ground-truth label pictures, indicating the pixels that belong to three possible regions:
  - Outer border pixels (pixels inside the closed area delimited by iris' outer border, i.e. iris + pupil pixels),
  - Inner border pixels (pixels inside the closed area delimited by iris' inner border, i.e. pupil pixels),
  - Iris ROI pixels (outer border pixels - inner border pixels, i.e. iris pixels).
  
The dataset is specially suited for detection/segmentation of iris/pupil regions of the bovine's eye, fundamental problems in automatic biometric recognition of animals. 

Each image shows the bovine's head pictured from the left or right side. The photos have been taken at night using a regular visible light camera, employing the camera's built-in flash. The capture distance from the camera to the animal varies between 100 cm and 200 cm.

Image resolution is 2100x1575 pixels for all images. Each photo is labeled as \<animal number\>_<image number>, with animal number ranging from 1 to 11, and image number starting from 1 for each different bovine.

For each image, a binary ground truth mask with white pixels belonging to the iris region has been manually created by the authors. Additionally, ground truth masks for the region surrounded by the outer border and the region surrounded by the inner border have been included for a more precise evaluation. An example of the three ground truth masks and the respective output of the proposed solution for one image of the dataset are shown in Figure \ref{fig:ALLmasks}.



```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
