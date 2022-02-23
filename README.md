# ICSSWaT
This project is for Industrial Control system using Proxity based approach on SWaT (PAD-SWaT)

# Statement of the problem  
- Industrial control system (ICS) is built computational algorithms and physical components for various mission-critical tasks by combining computational algorithms and physical components for various mission-critical tasks. ICS comprise supervisory control and data acquisition (SCADA), distributed control systems (DCS), and programmable logic controllers (PLC). Because of its nature, it is usually found in large places and is geographically dispersed. This sort of network connectivity is vulnerable to hacking. Water treatment and disruptions, transportation, robotics, electricity grids, and automation systems are among of the most well-known ICS applications.  


# Objective 
- The goal of this study is to detect anomalies in industrial control systems using a Proximity-based approach Anomaly Detection (PAD) and applying hyperparameter tuning to formalize the problem from statistical point of view over the Securing Water Treatment (SWaT) dataset 


# Architecture for PAD SWaT  


![Proximity based anomaly detection (1) (1)](https://user-images.githubusercontent.com/75506002/152689179-7541c2e5-64bf-48cc-9288-8e4cd3f02687.jpg)



# Dataset 
Short Description of Data:  Secure Water Treatment (SWaT), launched on 18 Mar 2015 by Chief Defence Scientist Prof. Quek Tong Boon, is a water treatment testbed for research in cyber security.  There are currently seven versions of the Secure Water Treatment Dataset called A1 A2 (2015), A3 (2017), A4 A5 (2019), A6 (2019) and A77 (2019) (2020). The testbed serves as a key asset for researchers in Singapore and abroad who are aiming at the design of secure CPS. 

# Pre-processing 
- Classify the dataset in to sensor and actuator_columns  
- preprocessoing the data with onehot encoding for catagorical data (actuator_columns) and Normalize numrical data with min max scaler   
- Binarize label 
- Use mutual info to feature select 10% of the columns and transform the train and test sets accordingly
- Classfifying the data train and test 

#  A model of machine learning that has been employed 
- One-class SVM (OCSVM) 
- Index-based KNN 
- Gaussian Mixture Model (GMM) 
- density-based spatial clustering of applications with noise (DBSCAN) 

# Predicting anomalies with developed model 
- Measure the Performance of the model 
- We used 37 attack points from the SWaT data set

# Dataset link 
- itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/
