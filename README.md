# ICSSWaT
This project is for Industrial Control system using Proxity based approach on SWaT (PAD-SWaT)


# Dataset 
Short Description of Data:  Secure Water Treatment (SWaT), launched on 18 Mar 2015 by Chief Defence Scientist Prof. Quek Tong Boon, is a water treatment testbed for research in cyber security.  There are currently seven versions of the Secure Water Treatment Dataset called A1 A2 (2015), A3 (2017), A4 A5 (2019), A6 (2019) and A77 (2019) (2020). The testbed serves as a key asset for researchers in Singapore and abroad who are aiming at the design of secure CPS. 

# Pre-processing 
- classify the dataset in to sensor and actuator_columns  
- preprocessoing the data with onehot encoding for catagorical data (actuator_columns) and Normalize numrical data with min max scaler   
- binarize label 
- Use mutual info to feature select 10% of the columns and transform the train and test sets accordingly
- classfifying the data train and test 

#  A model of machine learning that has been employed 
- density-based spatial clustering of applications with noise (DBSCAN)
- One-class SVM (OCSVM) 
- Index-based KNN 
- Brute-force KNN
- Gaussian Mixture Model (GMM) 
