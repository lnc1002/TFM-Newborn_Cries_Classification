# TFM Newborn Cries Classification

[![made-with-python](https://img.shields.io/badge/Coded%20with-Python-21496b.svg?style=for-the-badge&logo=Python)](https://www.python.org/)
[![made-with-latex](https://img.shields.io/badge/Documented%20with-LaTeX-4c9843.svg?style=for-the-badge&logo=Latex)](https://www.latex-project.org/)
![GitHub repo size](https://img.shields.io/github/repo-size/AdrianArnaiz/Brain-MRI-Denoiser-Autoencoder?style=for-the-badge&logo=Github)

***********

**Master's Thesis. Master's in Biomedical Data Science at Universitat Rovira i Virgili.**

#### Author
* **Lucía Núñez Calvo** 

#### Tutors: 
* **Dr. Daniel Urda Muñoz**
* **Dr. Santiago Marco** 

***************
* [Report (81 pages)](https://github.com/lnc1002/TFM-Newborn_Cries_Classification/blob/1806046903a4d8f420dd2c82541413d88430cc4b/doc/MT-MBDS.pdf)
* [Notebooks (10 files)]
***************

## Abstract
Analysing how a newborn baby reacts to different stimuli is crucial to diagnose possible neurological conditions. Traditionally, these assessments have been performed manually by health professionals, which to some extent leads to subjectivity, and possible misdiagnosis. In addition, such assessments require the immediate availability of a specialist, which in critical situations can delay assessments, putting the baby’s health at risk.

This project uses advanced tools such as **Deep Learning**, and **Machine Learning** to automate, and improve the detection, and **classification of newborn cries** in order to detect possible pathologies or diseases. Artificial Intelligence analyses of newborn videos, provides a consistent, and accurate assessment of newborn responses to stimuli can be achieved, accelerating the diagnosis of a possible disease.

Specifically, this study focuses on the detection of **Hypoxic-Ischaemic Encephalopathy (HIE)** by assessing newborn crying in response to nociceptive stimuli. To achieve this goal, several audio analysis approaches have been applied, with the project focusing on the employing of Machine Learning models, trained on labelled cry data, which have demonstrated high accuracy in the recognition of cry patterns.
This study explores feature extraction techniques such as Mel-Frequency Cepstral Coefficients (**MFCC**), and Linear Predictive Coding (**LPC**), and has implemented models such as Multilayer Perceptron (**MLP**), Support Vector Machine (**SVM**), and Long Short-Term Memory (**LSTM**). Promising results have been achieved with these models, with accuracies
of up to 90%.

The above methods not only help to detect HIE, but also open up the possibility of diagnosing other health problems through cry analysis. This research thus highlights the potential of machine learning to improve paediatric diagnosis, and neonatal care.



**Keywords**: Deep Learning, Machine Learning, Audio analysis, Classification of crying, Newborns, Mel Frequency Cepstral Coefficients (MFCC), Linear predictive coding (LPC), Multilayer Perceptron (MLP), Support Vector Machine (SVM), Long Short-Term Memory
(LSTM), Hypoxic Ischaemic Encephalopathy



## General Diagram of the Project
![](doc/figures/Project-Diagram.png)

#### Experiments:
* **With Multi-class Classification**:
    * Whithout cross-validation:
        * Extract features with **MFCC**, model **MLP**
        * Extract features with **LPC**, model **MLP**
        * Extract features with **MFCC**, model **SVM** with **One-Vs-Rest**
        * Extract features with **MFCC**, model **SVM** with **One-Vs-One**
        * Extract features with **LPC**, model **SVM** with **One-Vs-Rest**
        * Extract features with **LPC**, model **SVM** with **One-Vs-One**
        * Extract features with **MFCC**, model **LSTM**
        * Extract features with **LPC**, model **LSTM**
    * **Whith cross-validation**:
        * Extract features with **MFCC**, model **MLP**
        * Extract features with **LPC**, model **MLP**
        * Extract features with **MFCC**, model **SVM** with **One-Vs-Rest**
        * Extract features with **MFCC**, model **SVM** with **One-Vs-One**
        * Extract features with **LPC**, model **SVM** with **One-Vs-Rest**
        * Extract features with **LPC**, model **SVM** with **One-Vs-One**
        * Extract features with **MFCC**, model **LSTM**
        * Extract features with **LPC**, model **LSTM**
     
* **With Binary Classification**:
    * Whithout cross-validation:
        * Extract features with **MFCC**, model **MLP**
        * Extract features with **LPC**, model **MLP**
        * Extract features with **MFCC**, model **SVM** 
        * Extract features with **LPC**, model **SVM**
        * Extract features with **MFCC**, model **LSTM**
        * Extract features with **LPC**, model **LSTM**
    * **Whith cross-validation**:
        * Extract features with **MFCC**, model **MLP**
        * Extract features with **LPC**, model **MLP**
        * Extract features with **MFCC**, model **SVM**
        * Extract features with **LPC**, model **SVM**
        * Extract features with **MFCC**, model **LSTM**
        * Extract features with **LPC**, model **LSTM**



| Model | Features | Cross-validation | F1-score (0, 1) | Accuracy | AUC   |
|-------|----------|------------------|-----------------|----------|-------|
| MLP   | MFCC     | No               | 0.69, 0.92      | 0.87     | 0.95  |
| MLP   | LPC      | No               | 0.62, 0.89      | 0.83     | 0.91  |
| MLP   | MFCC     | Yes              | 0.71, 0.93      | 0.89     | 0.95  |
| MLP   | LPC      | Yes              | 0.61, 0.90      | 0.84     | 0.91  |
| SVM   | MFCC     | No               | 0.67, 0.91      | 0.86     | 0.94  |
| SVM   | LPC      | No               | 0.61, 0.90      | 0.84     | 0.89  |
| SVM   | MFCC     | Yes              | 0.70, 0.93      | 0.88     | 0.94  |
| SVM   | LPC      | Yes              | 0.64, 0.92      | 0.87     | 0.90  |
| LSTM  | MFCC     | No               | 0.70, 0.93      | 0.89     | 0.95  |
| LSTM  | LPC      | No               | 0.64, 0.92      | 0.86     | 0.90  |
| LSTM  | MFCC     | Yes              | 0.72, 0.94      | 0.90     | 0.94  |
| LSTM  | LPC      | Yes              | 0.63, 0.92      | 0.86     | 0.90  |


### Quanlitative Results
![](doc/figures/cualitative-results.png) 
![](doc/figures/clips.png) 

