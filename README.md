## Dataset overview

The BovineAAEyes80 is a dataset comprising 80 RGB images of 11 different bovines belonging to Aberdeen-Angus breed. The dataset is specially suited for detection/segmentation of iris/pupil regions of the bovine's eye, fundamental problems in automatic biometric recognition of animals. 

For each RGB image, there are three accompanying ground-truth label pictures, indicating the pixels that belong to three possible regions:
  - Outer border pixels (pixels inside the closed area delimited by iris' outer border, i.e. iris + pupil pixels),
  - Inner border pixels (pixels inside the closed area delimited by iris' inner border, i.e. pupil pixels),
  - Iris ROI pixels (outer border pixels _minus_ inner border pixels, i.e. iris pixels).
  
Each image shows the bovine's head pictured from the left or right side. The photos have been taken at night using a regular visible light camera, employing the camera's built-in flash. The capture distance from the camera to the animal varies between 100 cm and 200 cm.

Image resolution is 2100x1575 pixels for all images. Each picture is labeled as \<_animal number_\>\_\<_image number_\>, with animal number ranging from 1 to 11, and image number starting at 1 for each different bovine.

### Files organization

There is a separate subfolder for each of the four types of images:
  - RGB images are at `data/rgb/`,
  - Outer Border labels are at `data/labels_outer_border/`,
  - Inner border labels are at `data/labels_inner_border/`,
  - ROI labels are at `data/labels_roi/`.

For example: RGB image `5_1.png` can be found at subfolder `data/rgb/5_1.png`, whilst the corresponding ROI labels image is located at `data/labels_roi/5_1.png`.

You can [download the dataset](https://github.com/juanilarregui/BovineAAEyes80/archive/master.zip) (~500MB) or [view the project on Github](https://github.com/juanilarregui/BovineAAEyes80).

### Results of our segmentation method

A table of the results achieved by our segmentation method, for every image, can be seen in [this link](https://raw.githubusercontent.com/juanilarregui/BovineAAEyes80/master/results_per_image.png).
