---
title: 'Projects'
permalink: /projects/
classes: wide
toc: true
header:
    overlay_image: /assets/images/logan-liu-KYBLVEtEDgc-unsplash_cropped.jpg
    overlay_filter: 0.2
    caption: "Photo by [Logan Liu](https://unsplash.com/@liu169) on [Unsplash](https://unsplash.com)"
---
## Bounding Box Editor [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/BoundingBoxEditor)
<p align="center">
    <img src="https://raw.githubusercontent.com/mfl28/BoundingBoxEditor/master/src/main/resources/icons/app_icon.svg" height="80" width="80" align="center" alt="Bounding Box Editor logo"/>  
    <br/>
    <img src="https://raw.githubusercontent.com/mfl28/BoundingBoxEditor/master/demo-media/logo-text.svg" height="30" width="260" align="center" alt="Bounding Box Editor logo text"/>  
</p>
A multi-platform desktop image annotation application that allows you to easily create ground-truth annotations for classification and segmentation models. Simply chose an image folder, create rectangular and general polygonal bounding boxes and export them in the most common formats used in object detection. You can also import existing annotations and modify them within the program.
{% include figure image_path="https://raw.githubusercontent.com/wiki/mfl28/BoundingBoxEditor/demo-media/polygon_drawing.gif" alt="Bounding Box Editor Demo"%}

**Used Technology**
* Java and the <a href="https://openjfx.io/">JavaFX</a> UI-Framework
* [Gradle](https://gradle.org/) build tool
* Automatic UI-testing using [TestFX](https://github.com/TestFX/TestFX) and [JUnit 5](https://junit.org/junit5/)
* Multi-platform installer and portable image creation using the [jpackage](https://openjdk.java.net/jeps/343) Java 14 packaging tool, the [Badass JLink Gradle plugin](https://github.com/beryx/badass-jlink-plugin) and [github-actions](https://github.com/mfl28/BoundingBoxEditor/actions)  

[Latest Release](https://github.com/mfl28/BoundingBoxEditor/releases/latest){: .btn .btn--info}
[User Manual](https://github.com/mfl28/BoundingBoxEditor/wiki){: .btn .btn--primary}
[Code](https://github.com/mfl28/BoundingBoxEditor){: .btn .btn--primary}
<p align="center">
<a href="https://www.jetbrains.com/?from=BoundingBoxEditor">
<img src="https://upload.wikimedia.org/wikipedia/commons/1/1a/JetBrains_Logo_2016.svg">
</a>
</p>
<p align="center" style="font-size: 12pt">Special thanks to <a href="https://www.jetbrains.com/?from=BoundingBoxEditor"> JetBrains</a> for supporting this project with an Open Source license to their developer tools!  </p>


<hr style="height:3px;color:black;background-color:black">

## Pytorch Cpp [<i class="fab fa-fw fa-github"></i>](https://github.com/prabhuomkar/pytorch-cpp) 
<p align="center">
    <img src="https://raw.githubusercontent.com/prabhuomkar/pytorch-cpp/master/images/pytorch_cpp.png" height= "320" width="320" align="center"/>  
</p>
(*in collaboration with [Omkar Prabhu](https://github.com/prabhuomkar)*)   
C++ implementations of Machine- and Deep Learning tutorials for reasearchers. In detail, I implemented the intermediate and advanced tutorials and created the CMake build system generation and the Docker-containerized build option. The tutorials can be built and run locally on Windows, Linux and MacOs. The build script will automatically download the correct libtorch version and all necessary datasets to make it easy to get started. It is also possible to build and run the tutorials directly through a prepared Jupyter Notebook on Google Colab or [in a Docker container](https://github.com/mfl28/pytorch-cpp#using-docker).

**Used Technology**
* C++ and [PyTorch](https://pytorch.org/) C++ API (Libtorch)
* CMake
* Google Colab
* Docker, docker-compose
* Travis CI

[Open in Google Colab](https://colab.research.google.com/github/prabhuomkar/pytorch-cpp/blob/master/notebooks/pytorch_cpp_colab_notebook.ipynb){: .btn .btn--info}
[Code](https://github.com/mfl28/pytorch-cpp){: .btn .btn--primary}

### Example from advanced tutorials: Image Captioning
This tutorial shows how to create a model that generates textual descriptions of images. As training and testing dataset the [Flickr8K](https://github.com/jbrownlee/Datasets/releases/tag/Flickr8k) images are used. The model archicture is an encooder-decoder network incorporating visual attention as described in the [Show, Attend and Tell](https://arxiv.org/abs/1502.03044) paper. The attention masks are visualized as an overlay on the image so it is possible to see where the model "looks". The tutorial executable accepts many arguments that allow the user to customize the model architecture and experiment with different values for hyper-parameters.

[Code](https://github.com/mfl28/pytorch-cpp/tree/master/tutorials/advanced/image_captioning){: .btn .btn--primary}

<hr style="height:3px;color:black;background-color:black">

## Machine Learning [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning) 
A non exhaustive list of my machine learning projects.

**Used Technology**
* Python and JupyterLab
* PyTorch, OpenCV, Pandas, Scikit-Learn
* Google Colab, Docker

[Code](https://github.com/mfl28/MachineLearning){: .btn .btn--primary}

### Mltools Library [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#mltools-library-) 
A Python library that provides functions as well as dataset classes for object detection and classification and models for semantic segmentation.

[Code](https://github.com/mfl28/MachineLearning/tree/master/mltools){: .btn .btn--primary}

### Satellite Imagery Feature Detection [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#kaggle-competition-dstl-satellite-imagery-feature-detection-notebook--) 
A Jupyter Notebook project showing how to perform semantic segmentation in order to locate buildings in satellite images from the [Kaggle Dstl Satellite Imagery Feature Detection Challenge](https://www.kaggle.com/c/dstl-satellite-imagery-feature-detection).

**Used Technology**
* U-Net (fully convolutional model architecture)
* rasterio, geopandas, shapely
* Adversarial Validation
* Custom trainer, loss- and metrics-recorder classes

[Code](https://github.com/mfl28/MachineLearning/tree/master/notebooks){: .btn .btn--primary}

### Humpback Whale Fluke Detection [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#humpback-whale-fluke-detection-notebook--) 
The aim of this project was to detect humpback whale flukes in images from [Kaggle Humpback Whale Identification Challenge](https://www.kaggle.com/c/humpback-whale-identification). The ground-truth bounding boxes where created using [Bounding Box Editor](/projects/#bounding-box-editor-).

**Used Technology**
* Faster RCNN model
* Custom dataset class to parse XML annotation files
* Custom transform class to transform images and bounding box annotations

[Code](https://github.com/mfl28/MachineLearning/tree/master/notebooks){: .btn .btn--primary}

### Humpback Whale Identification [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/MachineLearning#kaggle-competition-humpback-whale-identification-notebook--) 
A notebook showing how to train a classifier to identify specific humpback whales in images according to the [Kaggle Humpback Whale Identification Challenge](https://www.kaggle.com/c/humpback-whale-identification).

**Used Technology**
* Resnet model 
* FastAI deeplearning library
* Oversampling to counter low number of samples for most classes

[Code](https://github.com/mfl28/MachineLearning/tree/master/notebooks){: .btn .btn--primary}

<hr style="height:3px;color:black;background-color:black">

## Utilities
### OpenGL Cpp Starter [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/opengl-cpp-starter) 
An easy to use starter code for OpenGL C++ projects using modern CMake. Automatically fetches, builds and links commonly used libraries like [glfw](https://github.com/glfw/glfw), [glad](https://github.com/Dav1dde/glad), [glm](https://github.com/g-truc/glm), [stb_image](https://github.com/nothings/stb) and (optionally) [assimp](https://github.com/assimp/assimp).

**Used Technologies:**
* OpenGL (core mode)
* CMake
* [Azure Devops Pipelines CI/CD](https://dev.azure.com/mfl28/opengl-cpp-starter/_build)

[Code](https://github.com/mfl28/opengl-cpp-starter){: .btn .btn--primary}

<hr style="height:3px;color:black;background-color:black">

## Courses
### Coursera Machine Learning [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/CourseraMachineLearning)
Python-implementations for programming exercises in Andrew Ng's excellent Machine Learning course (originally taught using Octave/Matlab).  

**Used Technologies:**
* Python - numpy, scikit-learn, matplotlib, pandas

[Code](https://github.com/mfl28/CourseraMachineLearning){: .btn .btn--primary}

### Hack Assembler [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/HackAssembler)
C++-implementation of an assembler for the Hack assembly-language as defined in the [nand2tetris](https://www.nand2tetris.org/) course.

**Used Technologies:**
* Google Test Framework
* CMake
* [Azure Devops Pipelines CI/CD](https://dev.azure.com/mfl28/HackAssembler)

[Code](https://github.com/mfl28/HackAssembler){: .btn .btn--primary}

### Hack VM-Translator [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/HackVMTranslator)
C++-implementation of a translator for the Hack-platform's virtual machine language as defined in the [nand2tetris](https://www.nand2tetris.org/) course.

**Used Technologies:**
* Google Test Framework
* CMake
* [Azure Devops Pipelines CI/CD](https://dev.azure.com/mfl28/JackCompiler/)

[Code](https://github.com/mfl28/HackVMTranslator){: .btn .btn--primary}

### Jack Compiler [<i class="fab fa-fw fa-github"></i>](https://github.com/mfl28/JackCompiler)
C++-implementation of a compiler for the Jack programming language as defined in the [nand2tetris](https://www.nand2tetris.org/) course.

**Used Technologies:**
* Google Test Framework
* CMake
* [Azure Devops Pipelines CI/CD](https://dev.azure.com/mfl28/HackVMTranslator)

[Code](https://github.com/mfl28/JackCompiler){: .btn .btn--primary}
