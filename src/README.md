### The approach is spread across CARAT is found in:
- 1. The explainer model is in : ExplainXformer
- 2. The counterfactual genetaion algorithm is in : recourse_Xformer

### The directory AD_Model contains the anomaly detetcion model used for comparative evaluation     

### The directories AD_APE and AD_MEAD are for model analysis (stability)

### Baseline models : FIMAP, RCEAA, ReplaceM, Xformer-R

----------------------------------------


- The data is in ./../GenratedData
- Preprocessing code : `data_preprocessing`. Please do not run this since the real data corpus is not sharable due to legal reasons.    
- The data source is real world shipment data from Panjiva Inc., belonging to time period Jan 2015 to Dec 2017 and cannot be shared due to legal reasons.  
- KGE is the folder for Knowledge Graph Embeddings. We have included the pretrained embeddings.
- Pretrained models for the Explainer is also included
----------------------------------------

To generate counterfactuals :

From the `scr` directory:
`cd recourse_Xformer`       
`CUDA_VISIBLE_DEVICES=0,1 python3 executor.py --dir us_import1 --num_anomalies 10 --num_cf 50`

-----------------------------------------