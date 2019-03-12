# kaggle-Leanplum

Solutions for Leanplum Kaggle Competition.

# Overview

The goal is to predict the whether a user will purchase in next 7 and 14 days. Since the data is large, we upload it to **GCP** and use **BigQuery** to preprocess the data, then finish all the work on local machine. 
Our pipeline is: Upload the GCP -- Preprocess data using BigQuery -- Download the data -- Data Cleaning, Feature Engineer and Model Building on local machine 

# Data

Due to the Non-disclosure agreement, I can't post the real data here, also the data is very large, it has 50GB totally for 5 datasets.

# Result

Due to the severe *data leakage* problem, the AUC could be easily achieved 0.99+ which made our model useless. We still, however, learned how to build our pipeline, preprocessed the large scale data on GCP and BigQuery, and the sliding window idea for time related machine learning problem.