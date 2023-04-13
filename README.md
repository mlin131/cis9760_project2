Project2: Analyzing IMDB Datasets

Author: Mingxing (Max) Lin

Date Created: 04/13/2023

Class: CIS9760

Project Objective: In this project, provisioning a Spark Cluster on AWS EMR for loading and running some analysis to answer a few simple question on IMDB'S datasets from Kaggle through Jupyter Notebook.

Project Procedure: 
First step, I create a EMR cluster configuration, I set software configurtion as emr-5.31.0 , also I select Spark and Livy and unselect Pig. The networking EC2 Subnet is configured and instance types are m5.xlarge. I keep the EC2 key pair as default (No Key pair found) . I waited 10 mintues for cluster to be created as shown below:
![Cluster Configuration](https://user-images.githubusercontent.com/119923435/231897996-55f54bbe-f968-4ef9-a8e3-591b071898f2.PNG)

Second step, I created notebooks and choose previous created cluster. Waited for 1-2 minutes for Notebook to be created as shown below:
![Notebook Configuration](https://user-images.githubusercontent.com/119923435/231898014-7e21bd32-80b2-4e9e-afc3-25d98b119c51.PNG)

Third step: in Jupyter notebook, I uploaded Project2_Analysis.ipynb file. I set Jupyter Notebook Kernel as Pyspark. Then, I install all necessary packages pandas version 1.0.3 and matplotlib verison 3.2.1, and import pandas, numpy, matplotlib packages. I also load all data from S3 into a Spark dataframe object as shown below:

![Capture1](https://user-images.githubusercontent.com/119923435/231903340-c2af3813-9896-4582-8db6-20111a1ed5c0.PNG)
![Capture3](https://user-images.githubusercontent.com/119923435/231903344-fa4b2178-383a-409d-a7c1-39913c0c830b.PNG)
![Capture](https://user-images.githubusercontent.com/119923435/231903250-de0aa229-04c6-4634-9fdb-68eeef676619.PNG)

Final step: after everything set up, I started to analyzing Genres, job categories, answering Questions and extre credit analysis using python.
