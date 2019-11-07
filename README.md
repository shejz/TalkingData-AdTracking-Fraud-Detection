# [TalkingData AdTracking Fraud Detection Challenge](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)


## Description
Fraud risk is everywhere, but for companies that advertise online, click fraud can happen at an overwhelming volume, resulting in misleading click data and wasted money. Ad channels can drive up costs by simply clicking on the ad at a large scale. With over 1 billion smart mobile devices in active use every month, China is the largest mobile market in the world and therefore suffers from huge volumes of fraudulent traffic. 

- Build a machine learning model to determine whether a click is fraud or not.


Competition link: [TalkingData AdTracking Fraud Detection Challenge](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection)

## Model and LB score (AUC-ROC)
**Model**: xgboost and lightgbm

**Evaluation Metric**: area under the ROC curve (AUC-ROC)

**Training and verification**: Some models use the data of 11.07-11.09, and some models use the data of 11.07-11.08. Randomly select **50 million** rows of data for verification.

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
- Big Datasets (TalkingData provides training data for **185 million samples**.)
- Imbalanced Data

**Solution References:**
- [Big Datasets](https://www.kaggle.com/yuliagm/how-to-work-with-big-datasets-on-16g-ram-dask)
- Fixing imbalanced data with LightGBM
  [link1:](https://www.kaggle.com/pranav84/lightgbm-fixing-unbalanced-data-lb-0-9680)
  [link2:](https://www.kaggle.com/alexanderkireev/experiments-with-imbalance-nn-arch-9728)
- Feature Engineering
  [link1:](https://www.kaggle.com/nanomathias/feature-engineering-importance-testing)
  [link2:](https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection/discussion/53634#latest-578234)
- LightGBM
  [link1:](https://www.kaggle.com/aharless/kaggle-runnable-version-of-baris-kanber-s-lightgbm)
  [link2:](https://www.kaggle.com/asraful70/talkingdata-added-new-features-in-lightgbm)
-[XGBoost](https://www.kaggle.com/joaopmpeinado/talkingdata-xgboost-lb-0-966)
