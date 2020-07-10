# Project Introduction
This project focuses on categorizing and explaining prediction errors of image recognition model using ObjectNet dataset, Visual Saliency Maps and Neural
Network architectures. The main focus is to introspect the model architecture to identify the patterns or rules which leads to drop in the perfoemnace of the models on different datasets.

  This is a Scientific Team Project with a team size of 6.

### Motivation:

  ![ObjectNet Performance Drop Image](https://github.com/prafulladiwesh/ObjectNetIntrospection/blob/master/Images/PerformanceDrop.png)
  
  With the new ObjectNet dataset there is 40-45% drop in the performance of the pretrained SOTA Neural Network Architectures which is trained on ImageNet data. 

### ObjectNet Dataset:

  * ObjectNet is a collection of real world images with simple household interior items.
  * Freely available but updating model parameter is not allowed.
  * For the purpose of generalization, it is only the test set with 50,000 images(same as ImageNet test set).
  * 313 classes with 113 overlapping ImageNet classes.
  * To distinguish it with training set, images in objectnet are marked with red border of one pixel size.
  * Objects are taken from phone cameras with:
    * 4 backgrounds (kitchen, livingrooms, bedrooms & washrooms)
    * 3 viewpoints (top, angled at 45 degrees, and side)
    * 50 object rotations (Rotations were uniformly distributed on a sphere)
    
    ![Image Comparison](https://github.com/prafulladiwesh/ObjectNetIntrospection/blob/master/Images/ObjectNet_ImageNet.png)
    
    Original [ObjectNet Paper](https://objectnet.dev/objectnet-a-large-scale-bias-controlled-dataset-for-pushing-the-limits-of-object-recognition-models.pdf) can be found here.

### Goal of the project:

  1. To check if the model is distracted by other objects present in background and foreground.
  2. To check if the model gives importance to color features.
  3. To check if the model is invariant to rotation.

### Implementation Steps:

  1. Manual introspection of the (mis)classification images using Saliency Maps for understanding the pattern.
  2. Identifying object/class location in the Image using segmentation methodologies.
  3. Color Feature Introspection & Image Enhancement.
  4. Check Rotation and Translation invariance.

# Individual Contribution:

  1. Manual Interospection to find the pattern and rule in the (mis)classification.
  2. Find potential hypothesis out of the pattern
  3. Color Feature Introspection & Image Enhancement.
  4. Rotation and Translation Invariance check.
  
  
### Note : This is an ongoing project. Any changes done will be pushed in this repository. 
