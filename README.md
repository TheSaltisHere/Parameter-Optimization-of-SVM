# Parameter Optimization of SVM
Assignment for UCS654

## About SVM and Parameter Optimization

Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily, it is used for Classification problems in Machine Learning.

Some of the most important parameters of SVM such as kernel, C, and gamma can be changed in order to achieve a higher accuracy. This is called as Hyperparameter Tuning. 

We can perform this task using Random Search for optimizing these parameters.

## Dataset
Anuran Calls (MFCCs) Data Set

This dataset was used in several classifications tasks related to the challenge of anuran species recognition through their calls. It is a multilabel dataset with three columns of labels. This dataset was created segmenting 60 audio records belonging to 4 different families, 8 genus, and 10 species. Each audio corresponds to one specimen (an individual frog), the record ID is also included as an extra column. We used the spectral entropy and a binary cluster method to detect audio frames belonging to each syllable. The segmentation and feature extraction were carried out in Matlab. After the segmentation we got 7195 syllables, which became instances for train and test the classifier. These records were collected in situ under real noise conditions (the background sound). Some species are from the campus of Federal University of Amazonas, Manaus, others from Mata AtlÃ¢ntica, Brazil, and one of them from CÃ³rdoba, Argentina. The recordings were stored in wav format with 44.1kHz of sampling frequency and 32bit of resolution, which allows us to analyze signals up to 22kHz. From every extracted syllable 22 MFCCs were calculated by using 44 triangular filters. These coefficients were normalized between -1 â‰¤ mfcc â‰¤ 1. The amount of instances per class are:

##Result Table
| Sample  | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
| -----   | ------------- | ----------- | ------- | ------------ |
| 1 | 0.934 | poly | 1.23 | 2.46 |
| 2 | 0.962 | rbf | 2.34 | 2.56 |
| 3 | 0.942 | rbf | 3.43 | 6.72 |
| 4 | 0.96 | rbf | 1.32 | 3.64 |
| 5 | 0.945 | rbf | 1.52 | 3.39 |
| 6 | 0.956 | rbf | 2.60 | 3.13 |
| 7 | 0.937 | rbf | 0.21 | 0.24 |
| 8 | 0.954 | rbf | 1.24 | 1.57 |
| 9 | 0.943 | rbf | 1.27 | 5.67 |
| 10 | 0.95 | rbf | 0.3 | 6.5 |

## Convergence
![graph](https://user-images.githubusercontent.com/73683708/233207173-945ebd99-1c48-4509-9847-7c32d05b3643.png)

## Discussion
The graph is made for the sample which has best accuracy. Because the sample was big number of iterations had to be low as more would be extremely time consuing.Numnber of iterations was set to 10 .Sample has the best accuracy of 0.962 having kernel = rbf, nu= 2.34 and epsilon=2.56.

## Written By
Name : RIshab Chakrabarti
  
Roll No. : 102003688

Sub-Group: 3CO26
















