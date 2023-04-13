Project2: Analyzing IMDB Datasets

Author: Mingxing (Max) Lin

Date Created: 04/13/2023

Class: CIS9760

Project Objective: In this project, provisioning a Spark Cluster on AWS EMR for loading and running some analysis to answer a few simple question on IMDB'S datasets from Kaggle through Jupyter Notebook.

Project Procedure: 
First, I create a EMR cluster configuration, I set software configurtion as emr-5.31.0 , also I select Spark and Livy and unselect Pig. The networking EC2 Subnet is configured and instance types are m5.xlarge. I keep the EC2 key pair as default (No Key pair found) . I waited 10 mintues for cluster to be created as shown below:

