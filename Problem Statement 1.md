##  Problem Statement 1:

Use chest X-ray images dataset obtained from [https://github.com/ieee8023/covid-chestxray-dataset](https://github.com/ieee8023/covid-chestxray-dataset) and [https://www.kaggle.com/c/rsna-pneumonia-detection-challenge](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge) to 

### Task 1: Processing of IEEE8023 data:
1. Cleaning of metadata
2. Processing the  Clinical Notes to determing patient symptoms and find if more variables can be included using the same.
3.   Use the feature set to train different DNNs and validate the result

### Task 2:  Processing RSNA images

1. Use the -ray image dataset to build a neumonia classifier which doesn't predict existence of COVID-19. 
2. Use transfer learning or some other method to combine this network and that of task 1 to build better classifiers for pneumonia.