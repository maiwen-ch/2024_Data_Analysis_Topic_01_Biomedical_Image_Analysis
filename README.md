# Topic 01: Biomedical Image Analysis

Supervisor:

* PD Dr. Karl Rohr     (k.rohr@uni-heidelberg.de)
* Dr. Leonid Kostrykin (leonid.kostrykin@bioquant.uni-heidelberg.de)
* Kerem Celikay        (kerem.celikay@bioquant.uni-heidelberg.de)
* Janis Meyer          (janis.meyer@bioquant.uni-heidelberg.de)
* Leonie Thomas (Tutor)

## Introduction

Image analysis methods are important to extract relevant information from biomedical image data. Typically, a large amount of data needs to be analyzed to draw statistically significant conclusions.

Manual analysis of the image data is tedious, time-consuming, and subjective. Thus, computer-based image analysis is needed, which enables fast, reproducible, and accurate automated analysis of the data.

To extract information from the image data, methods for different image analysis tasks are required. Typical tasks are image preprocessing, feature extraction, segmentation, object recognition, tracking, and image registration. The projects within the topic "Biomedical Image Analysis" comprise different image analysis tasks using different methods and image modalities. The image analysis methods will be implemented in Python using existing libraries (e.g., NumPy, Scikit-learn).

## Objective

### Human Face and Handwritten Digit Recognition

The objective of projects 1 and 2 is to implement and evaluate classification methods for human face and handwritten digit recognition using K-nearest neighbors. First, statistical measures for performing data normalization should be computed. Second, data dimension reduction should be performed by principal component analysis (PCA) and the results should be visualized. Third, the dataset should be split into training and test datasets in order to perform human face or handwritten digit recognition.

- **Project 1:** Implementation and evaluation of K-nearest neighbors (KNN) algorithm for human face recognition.
- **Project 2:** Implementation and evaluation of K-nearest neighbors (KNN) algorithm for handwritten digit recognition.

The key steps of the projects (e.g., determination of the K-nearest neighbors) must be implemented by the students. Pre-implemented functions may only be used for verification of the results!


### Cell Nuclei Segmentation

The objective of projects 3 and 4 is to implement and evaluate methods for segmentation of cell nuclei (Otsu thresholding or clustering method). First, the image segmentation method should be implemented. Second, a popular evaluation measure known as "Dice score" should be implemented and tested using synthetically generated images. The methods should be applied to cell nuclei images and the average Dice score should be computed. For Otsu thresholding, the implemented segmentation method should be extended by local thresholding using a sliding window scheme. For the clustering method, the colored images should be converted to different color models and the segmentation results should be compared to the RGB color representation model.

- **Project 3:** Implementation and evaluation of Otsu thresholding.
- **Project 4:** Implementation and evaluation of clustering method.

The key steps of the projects (e.g., Otsu's method, thresholding, Dice score) must be implemented by the students. Pre-implemented functions may only be used for verification of the results!

## Description of datasets

### Human Face and Handwritten Digit Recognition

The Yale Face Database of human faces consists of 165 images from 15 subjects. Per subject exist 11 images with the following facial expressions or configurations: center-light, with glasses, happy, left-light, without glasses, normal, right-light, sad, sleepy, surprised, and wink. The images are grayscale images normalized by size (320×243 pixels) and stored as GIF files.

The datset for digit recognition is from the MNIST database (Modified National Institute of Standards and Technology database) of handwritten digits consisting of a training set (60.000 images) and a test set (10.000 images). The images are size-normalized (28×28 pixels) and centered, and the labels are stored in CSV files (comma-separated values). Each line of these files represents an image. The first column represents the label (the digit depicted in the image).

### Cell Nuclei Segmentation

The image data for cell nuclei segmentation with Otsu thresholding consists of three different datasets. The first dataset consists of 6 images showing GFP transfected GOWT1 mouse embryonic stem cells. The images have a size of 1024×1024 pixels and show 10–20 cell nuclei per image. The second dataset consists of 18 images of mouse embryonic cells stained with Hoechst. The images have a size of 1344×1024 pixels and include around 60 cell nuclei per image. The third dataset consists of four images with HeLa cells stably expressing H2b-GFP. The images have a size of 1100×700 pixels and show 30–50 cell nuclei per image.

The dataset for segmentation based on clustering consists of two colour images. The first image has a size of 1024×1024 pixels and consists of fluorescently labeled cell nuclei. The second image has a size of 1200×1200 pixels and shows yeast cells. The clustering method should also be applied and evaluated on one of three datasets used for Otsu thresholding.

## Literature

### Human Face and Handwritten Digit Recognition

- Gerbrands, J.J. "On the relationships between SVD, KLT and PCA." Pattern Recognition (1981), vol. 14, issues 1-6, pp 375-381
- Belhumeur, P.N., Hespanha, J.P. and Kriegman, D. "Eigenfaces vs. Fisherfaces: Recognition Using Class Specific Linear Projection." IEEE Transactions on Pattern Analysis and Machine Intelligence (1997), vol. 19, pp 711-720.
- Netzer, Y. et al. "Reading Digits in Natural Images with Unsupervised Feature Learning." Proceedings of the Workshop on Neural Information Processing Systems (2011)
- Gareth, J. et al. "An introduction to statistical learning." Springer New York (2013), Chapter 4.4

### Cell Nuclei Segmentation

- Otsu, N. "A threshold selection method from gray-level histograms." IEEE Transactions on Systems, Man, and Cybernetics 9:1 (1979), pp 62-66.
- MacKay, D. "An Example Inference Task: Clustering." Information Theory, Inference and Learning Algorithms (2003), Chapter 20
- Coelho, L.P., Shariff, A., and Murphy, R.F. "Nuclear segmentation in microscope cell images: a hand-segmented dataset and comparison of algorithms." IEEE Proceedings of the International Symposium on Biomedical Imaging, pp. 518-521 (2009).

## How to structure your project

### Project proposal

For all projects within the topic "Biomedical Image Analysis" the first task
is to define a *project proposal*, which should include

- List of planned analysis steps
- Intended workflow for using Git
- Milestones (important achievements)
- Deliverables (result for each milestone)
- Approximate timetable
