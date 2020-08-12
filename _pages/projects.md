---
title: 'Projects'
layout: single
permalink: /projects/
author_profile: true
classes: wide
toc: true
---
## Bounding Box Editor [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/BoundingBoxEditor)
<p align="center">
    <img src="https://raw.githubusercontent.com/mfl28/BoundingBoxEditor/master/src/main/resources/icons/app_icon.svg" height= "80" width="80" align="center"/>  
</p>
A multi-platform (available on Linux, Mac and Windows) desktop image annotation application that allows you to easily create ground-truth annotations for classification and segmentation models. Simply chose an image folder, create rectangular and general polygonal bounding boxes and export them in two of the most common formats used in object detection. You can also import existing annotations and modify them within the program.
{% include figure image_path="https://raw.githubusercontent.com/wiki/mfl28/BoundingBoxEditor/demo-media/polygon_drawing.gif" alt="Bounding Box Editor Demo"%}

**Used Technology**
<div style="float: left; width: 50%;">
<ul>
<li>Java and the <a href="https://openjfx.io/">JavaFX</a> UI-Framework</li>
<li>Automatic UI-testing using <a href="https://github.com/TestFX/TestFX">TestFX</a> and <a href="https://junit.org/junit5/">JUnit 5</a></li>
<li><a href="https://dev.azure.com/mfl28/BoundingBoxEditor/_build">Azure Devops Pipeline CI</a></li>
</ul>
</div>
<div style="float: right; width: 50%;">
<p align="center">
<a href="https://www.jetbrains.com/?from=BoundingBoxEditor">
<img src="https://upload.wikimedia.org/wikipedia/commons/1/1a/JetBrains_Logo_2016.svg">
</a>
</p>
<p align="center" style="font-size: 12pt">Special thanks to <a href="https://www.jetbrains.com/?from=BoundingBoxEditor"> JetBrains</a> for supporting this project with an Open Source license to their developer tools!  </p>
</div>

[Latest Release](https://github.com/mfl28/BoundingBoxEditor/releases/latest){: .btn .btn--info}
[User Manual](https://github.com/mfl28/BoundingBoxEditor/wiki){: .btn .btn--primary}

<hr style="height:3px;color:black;background-color:black">

## Pytorch Cpp [<i class="fab fa-fw fa-github"></i>](https://github.com/prabhuomkar/pytorch-cpp) 
<p align="center">
    <img src="https://raw.githubusercontent.com/prabhuomkar/pytorch-cpp/master/images/pytorch_cpp.png" height= "320" width="320" align="center"/>  
</p>
(*in collaboration with [Omkar Prabhu](https://github.com/prabhuomkar)*)   
C++ implementations of Machine- and Deep Learning tutorials for reasearchers. In detail, I implemented the intermediate and advanced tutorials and created the CMake build system generation.

**Used Technology**
* C++ and PyTorch C++ API (Libtorch)
* CMake build system generation
* Travis CI

<hr style="height:3px;color:black;background-color:black">

## Machine Learning Projects [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning) 
A non exhaustive list of my machine learning projects.

**Used Technology**
* Python and JupyterLab
* PyTorch, OpenCV, Pandas, Scikit-Learn
* Google Colab

### mltools library [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#mltools-library-) 
A Python library that provides functions as well as dataset classes for object detection and classification and models for semantic segmentation.

### Satellite Imagery Feature Detection [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#kaggle-competition-dstl-satellite-imagery-feature-detection-notebook--) 
A Jupyter Notebook project showing how to perform semantic segmentation in order to locate buildings in satellite images from the [Kaggle Dstl Satellite Imagery Feature Detection Challenge](https://www.kaggle.com/c/dstl-satellite-imagery-feature-detection).

**Used Technology**
* U-Net (fully convolutional model architecture)
* Rasterio, Geopandas, Shapely
* Adversarial Validation
* Custom trainer, loss- and metrics-recorder classes

### Humpback Whale Fluke Detection [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#humpback-whale-fluke-detection-notebook--) 
The aim of this project was to detect humpback whale flukes in images from [Kaggle Humpback Whale Identification Challenge](https://www.kaggle.com/c/humpback-whale-identification). The ground-truth bounding boxes where created using [Bounding Box Editor](/projects/#bounding-box-editor-).

**Used Technology**
* Faster RCNN model
* Custom dataset class to parse XML annotation files
* Custom transform class to transform images and bounding box annotations

### Humpback Whale Identification [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#kaggle-competition-humpback-whale-identification-notebook--) 
A notebook showing how to train a classifier to identify specific humpback whales in images according to the [Kaggle Humpback Whale Identification Challenge](https://www.kaggle.com/c/humpback-whale-identification).

**Used Technology**
* Resnet model 
* FastAI deeplearning library
* Oversampling to counter low number of samples for most classes
