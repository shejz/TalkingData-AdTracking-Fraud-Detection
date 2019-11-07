# [TalkingData AdTracking Fraud Detection Challenge](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)


## Description
Fraud risk is everywhere, but for companies that advertise online, click fraud can happen at an overwhelming volume, resulting in misleading click data and wasted money. Ad channels can drive up costs by simply clicking on the ad at a large scale. With over 1 billion smart mobile devices in active use every month, China is the largest mobile market in the world and therefore suffers from huge volumes of fraudulent traffic. 

- Build a machine learning model to determine whether a click is fraud or not.


Competition link: [TalkingData AdTracking Fraud Detection Challenge](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)

## Model and LB score (AUC-ROC)
**Model**: xgboost and lightgbm

**Training and verification**: Some models use the data of 11.07-11.09, and some models use the data of 11.07-11.08. Randomly select **10 million** rows of data for verification.

|Model|Public score|Private score|Final rank| 
|---|---|---|---|
| LGBM |0.98122|0.98206| 223th ([Top 6%](https://www.kaggle.com/shielaj/competitions))|

**The libraries used are**:  
- numpy
- pandas
- matplotlib, 
- seaborn
- sklearn
- lightgbm
- xgboost

**Challenges**:
- Big Datasets (TalkingData provides training data for **185 million samples**, including data between 2017.11.06 and 2017.11.09.)
- Imbalanced Data

**Evaluation Metric**
- area under the ROC curve (ROC-AUC)

