# Project Description

## Assignment Overview

When using machine learning for classification, things are easiest if classes are “balanced” – that is, when the number of observations belonging to each of the classes are of the same order of magnitude. Unfortunately, this is often not the case. In this assignment, you will work with a dataset of car-insurance claims and try to classify claims into fraudulent (1) and non- fraudulent (0). There are more than 10,000 claims in the dataset, but only around 100 are fraudulent. Nevertheless, we want to create a model that helps the insurance provider target its investigation efforts. For this, we consider two options: 

(i) synthetically creating new data to make the dataset more balanced, and 

(ii) using an auto-encoder to represent “normal” (non- fraudulent) claims and applying it to distinguish fraudulent claims – a form of anomaly detection.

## Task Description

1. Briefly discuss why it is more difficult to find a good classifier on such a dataset than on one where, for example, 5,000 claims are fraudulent, and 5,000 are not. In particular, consider what happens when undetected fraudulent claims are very costly to the insurance company.

2. Load the dataset "Insurance_claims.csv" and clean it as appropriate for use with machine learning algorithms. A description of the features can be found at the end of this document.

3. Start by creating a (deep) neural network in TensorFlow and train it on the data. Using training and validation sets, find a model with high accuracy, then evaluate it on the test set. In particular, record both the accuracy and AUC. Briefly discuss what issues you observe based on the metrics.

4. The file "SMOTE.ipynb" explains the process in detail and shows how to change the dataset with an example. You can copy and adjust the code to make it work within your analysis. You can adjust the "sampling_strategy" parameters as you see fit, particularly if you want to fine-tune your model in part 5.

5. Create a new (deep) neural network and train it on your enhanced dataset. Use training and validation sets derived from the enhanced dataset to find a model with high accuracy. Evaluate your final model on a test set consisting only of original data. Again, record the accuracy and AUC. Briefly discuss the changes you would expect in the metrics and the actual changes you observe. Would you say that you are now doing better at identifying fraudulent claims?
