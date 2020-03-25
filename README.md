## Documentation of past work

Highlights of recent advancements in Healthcare | AI sector referring papers presented at ML4H workshop of NeurIPS 2018.

## Broad Categories

**1. Human Robot Interaction:**
a. EEG processing to classify and map's brain intents.
b. EMG processing; RL for prosthetics.

**2. Diagnosis/Prognosis:**

a. Use lesser compute resources to train and deploy Deep Learning algorithms

b. Augment Data to train Deep Learning models

c. Using patient symptom description, past EHR, clinician's comments, basic test results and radiology based results to shortlist and predict exact medical condition/diseases.



## 1. Human Robot Interaction

Involves different paradigms of mapping EEG, EMG signals to different intents and using them as inputs for various electronic/robotic tasks.

## 2. Prognosis/Diagnosis

### a. Reducing required compute resources by substituting 3D CNN's with 2D CNNs and additional algorithms.

#### 1: Convolutional LSTM   
Disease Detection in Weakly Annotated Volumetric Medical Images using a Convolutional LSTM Network
[https://arxiv.org/abs/1812.01087](https://arxiv.org/abs/1812.01087)
-> Binary  classifier of emphysema in lung cancer using low power CT images.

#### Additional algorithm 2: Recurrent convolutional gated graph propagators 
Radiotherapy Target Contouring with Convolutional Gated Graph Neural Network [https://arxiv.org/abs/1904.03086](https://arxiv.org/abs/1904.03086)
-> Esophageal Cancer Radiotherapy Target Treatment Contouring dataset of 81 patients which includes tomography images with radiotherapy target.

### b.  Augment Data to train Deep Learning models

Lack of Data which has been addressed in the papers:
1. Material for Radiology education
2. 3D image reconstruction
3. High intravariance in training images for classifiers
4. Less frequent classes

Solutions:
### a. Using Generative Adversarial Networks (Solves 1,2,3,4):
**i. Augment radiology images with different classes and conditions for education purposes.** 
-> Provides different content for students without having to go through NDA's.

**ii. Make a 3D image of charge potential of epicardial plane of heart using multi-lead ECG signal.**   
-> Can diagnose certain diseases better, offers better visualization, not significantly better than the currently available systems.

**iii. Patch based semi-supervised learning to classify Fundus images** - Retinopathy.

**iv. General-to-Detailed GAN for Infrequent Class Medical Images**
->  For classes with less examples, use available examples to train a GAN and use it to generate more examples for the class. Now use these examples to train over CNN.

### b. Clustering networks (Solves 3):

**Prototypical Clustering Networks for Dermatological Disease Diagnosis** 
[https://arxiv.org/abs/1811.03066](https://arxiv.org/abs/1811.03066)
-> Uses clustering nets to identify varied data of a single class as a single class hence outperforms conventional CNNs in case of data with variance in individual classes. Uses clustering nets to identify varied data of a single class as a single class hence outperforms conventional CNNs in case of data with variance in individual classes.
-> Used for classifying skin images into dermal conditions.

#### c. Reinforcement Learning based models (Solves 3,4):
Integrating Reinforcement Learning to Self Training for Pulmonary Nodule Segmentation in Chest X-rays
[https://arxiv.org/pdf/1811.08840.pdf](https://arxiv.org/pdf/1811.08840.pdf)
**Train CNN models as classifiers for medical images. Use this model as reward function to train RL(MDP) model whose policies label classes.** 
-> Used for segmentation of pulmonary nodule in chest X-rays.

### c.  Augment Data to train Deep Learning models
Combine patient's description of symptoms, doctor's description of symptoms, pathology test results and radiology images to accurately predict the disease/medical condition of the patient.

**i. DeepSPINE: Automated Lumbar Vertebral Segmentation, Disc-level Designation, and Spinal Stenosis Grading Using Deep Learning** 
[https://arxiv.org/abs/1807.10215](https://arxiv.org/abs/1807.10215)
-> (1) a natural-language-processing scheme to extract level-by-level ground-truth labels from free-text radiology reports for the various types and grades of spinal stenosis 
(2) accurate vertebral segmentation and disc-level localization using a U-Net architecture combined with a spine-curve fitting method, and 
(3) a multi-input, multi-task, and multi-class convolutional neural network to perform central canal and foraminal stenosis grading on both axial and sagittal imaging series inputs with the extracted report-derived labels applied to corresponding imaging level segments.

**ii. Here is a list of diseases which are diagnosed using radiological images and involve similar exchange of dialogue** 
[https://www.radiologyinfo.org/en/submenu.cfm?pg=disease-condition](https://www.radiologyinfo.org/en/submenu.cfm?pg=disease-condition)
