﻿
# [Итоговый проект курса «Машинное обучение в бизнесе»](https://github.com/a-zadorozhnyi/ML-in-business/tree/final_project)
## Technology Stack:

ML: Sklearn, Pandas, Numpy, Pycaret

API: Flask

## Data Set:
https://archive.ics.uci.edu/ml/datasets/HTRU2
### Description:
HTRU2 is a data set which describes a sample of pulsar candidates collected during the High Time Resolution Universe Survey (South) [1].  
  
Pulsars are a rare type of Neutron star that produce radio emission detectable here on Earth. They are of considerable scientific interest as probes of space-time, the inter-stellar medium, and states of matter (see [2] for more uses).  
  
As pulsars rotate, their emission beam sweeps across the sky, and when this crosses our line of sight, produces a detectable pattern of broadband radio emission. As pulsars  
rotate rapidly, this pattern repeats periodically. Thus pulsar search involves looking for periodic radio signals with large radio telescopes.  
  
Each pulsar produces a slightly different emission pattern, which varies slightly with each rotation (see [2] for an introduction to pulsar astrophysics to find out why). Thus a potential signal detection known as a 'candidate', is averaged over many rotations of the pulsar, as determined by the length of an observation. In the absence of additional info, each candidate could potentially describe a real pulsar. However in practice almost all detections are caused by radio frequency interference (RFI) and noise, making legitimate signals hard to find.  
  
Machine learning tools are now being used to automatically label pulsar candidates to facilitate rapid analysis. Classification systems in particular are being widely adopted,  
(see [4,5,6,7,8,9]) which treat the candidate data sets as binary classification problems. Here the legitimate pulsar examples are a minority positive class, and spurious examples the majority negative class. At present multi-class labels are unavailable, given the costs associated with data annotation.  
  
The data set shared here contains 16,259 spurious examples caused by RFI/noise, and 1,639 real pulsar examples. These examples have all been checked by human annotators.  
  
The data is presented in two formats: CSV and ARFF (used by the WEKA data mining tool). Candidates are stored in both files in separate rows. Each row lists the variables first, and the class label is the final entry. The class labels used are 0 (negative) and 1 (positive).  
  
Please note that the data contains no positional information or other astronomical details. It is simply feature data extracted from candidate files using the PulsarFeatureLab tool (see [10]).

**Attribute Information:**

Each candidate is described by 8 continuous variables, and a single class variable. The first four are simple statistics obtained from the integrated pulse profile (folded profile). This is an array of continuous variables that describe a longitude-resolved version of the signal that has been averaged in both time and frequency (see [3] for more details). The remaining four variables are similarly obtained from the DM-SNR curve (again see [3] for more details). These are summarised below:  
  
1. Mean of the integrated profile.  
2. Standard deviation of the integrated profile.  
3. Excess kurtosis of the integrated profile.  
4. Skewness of the integrated profile.  
5. Mean of the DM-SNR curve.  
6. Standard deviation of the DM-SNR curve.  
7. Excess kurtosis of the DM-SNR curve.  
8. Skewness of the DM-SNR curve.  
9. Class  
  
HTRU 2 Summary  
17,898 total examples.  
1,639 positive examples.  
16,259 negative examples.

**Target:** class

### Clone repository and create project

```
$ git clone https://github.com/a-zadorozhnyi/ML-in-business/tree/final_project
$ cd D:\Geekbrains\Машинное обучение в бизнесе\9\final_project
$ docker build -t course_project .

```

### [](https://github.com/busiko7/Geekbrains/tree/b039fb30ab83ae408f7f1d60556722be899df16e/machine_learning_in_business/course_project#run-docker)Run docker

```
$ docker run -d -p 8080:8080 course_project

```

### Go to  [http://localhost:8080](http://localhost:8080/)  or  [http://127.0.0.1:8080/](http://127.0.0.1:8080/)
