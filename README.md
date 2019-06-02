# Offline Character Recognition System

<b>Programming Languages/Software:</b> R, RStudio

<b>Skills Used:</b><br> 
Neural Networks<br>
SVM<br>
kNN<br>
PCA<br>
Cluster Analysis<br>
Exploratory Analysis

## Introduction

Handwriting is unique to every individual. The ability to systematically recognize letters that are handwritten has made great strides; however, there still remains a level of complexity due to the individuality of how each one of us writes a letter or word. This project uses machine learning and cluster analysis to recognize handwritten alphanumeric characters. 

## Exploratory Analysis

There are two files, one with labeled data containing 1,000 observations and one with unlabeled data containing 10,000 observations. Both files contain 3,136 predictor variables (Pixel.1 to Pixel.3136), all of which were binary variables containing only 0 or 1. When consumed as a unit, these predictor variables form a 56 x 56 image of the represented digit. There are no missing values in this dataset.

Sample of plotted letters and numbers are provided below. 

<div align=center><img src="/images/image001.png"></div>

Looking at the distribution of each character, there is little variability on average in how people draw their characters. 1's and K's seem to have the widest distributions while 9's and J's have the smallest. Furthermore, there are few outliers in this dataset and some characters have no outliers at all.

<div align=center><img src="/images/image002.png"></div>

### Letter Similarities

<div align=center><img src="/images/image003.jpg"></div>

Rules

•	5 and S: square top = 5, rounded top = S
•	6 and G: square bottom = G, round bottom = 6
•	2 and Z: curved bottom = Z, else = 2
•	1 and I: tilted =1, else = I. 
•	0 and O: tall circle = 0, round/wide circle = O
