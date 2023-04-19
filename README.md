# Parameter Optimization of SVM
Assignment for UCS654

## About SVM and Parameter Optimization

Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily, it is used for Classification problems in Machine Learning.

Some of the most important parameters of SVM such as kernel, C, and gamma can be changed in order to achieve a higher accuracy. This is called as Hyperparameter Tuning. 

We can perform this task using Random Search for optimizing these parameters.

## Dataset
Anuran Calls (MFCCs) Data Set

This dataset was used in several classifications tasks related to the challenge of anuran species recognition through their calls. It is a multilabel dataset with three columns of labels. This dataset was created segmenting 60 audio records belonging to 4 different families, 8 genus, and 10 species. Each audio corresponds to one specimen (an individual frog), the record ID is also included as an extra column. We used the spectral entropy and a binary cluster method to detect audio frames belonging to each syllable. The segmentation and feature extraction were carried out in Matlab. After the segmentation we got 7195 syllables, which became instances for train and test the classifier. These records were collected in situ under real noise conditions (the background sound). Some species are from the campus of Federal University of Amazonas, Manaus, others from Mata AtlÃ¢ntica, Brazil, and one of them from CÃ³rdoba, Argentina. The recordings were stored in wav format with 44.1kHz of sampling frequency and 32bit of resolution, which allows us to analyze signals up to 22kHz. From every extracted syllable 22 MFCCs were calculated by using 44 triangular filters. These coefficients were normalized between -1 â‰¤ mfcc â‰¤ 1. The amount of instances per class are:

Families:
Bufonidae 68
Dendrobatidae 542
Hylidae 2165
Leptodactylidae 4420

Genus:
Adenomera 4150
Ameerega 542
Dendropsophus 310
Hypsiboas 1593
Leptodactylus 270
Osteocephalus 114
Rhinella 68
Scinax 148

Species:
AdenomeraAndre 672
AdenomeraHylaedactâ€¦ 3478
Ameeregatrivittata 542
HylaMinuta 310
HypsiboasCinerascens 472
HypsiboasCordobae 1121
LeptodactylusFuscus 270
OsteocephalusOophaâ€¦ 114
Rhinellagranulosa 68
ScinaxRuber 148


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
![Capture]https://raw.githubusercontent.com/TheSaltisHere/Parameter-Optimization-of-SVM/main/graph.png


















