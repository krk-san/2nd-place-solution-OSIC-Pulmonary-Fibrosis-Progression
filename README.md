# OSIC Pulmonary Fibrosis Progression 2nd place solution

## Final Solution
 I tried many methods, but in the end, the ensemble of Quantile Regression and EfficientNet B3 was the best solution for me. I clustered patients based on FVC changes for the last few weeks and prepared a validation set with Stratifield K-Fold. Based on this, I trained each model. For the feature 'Percent', I used only the measurements of the first visit. This seems to have been one of the reasons for the victory. Quantile Regression Model is also trained in the inference code for normalization with the test data.

## How to run

```2nd-place-solution.ipynb``` - contains inference part with EfficientNetB3 and Quantile Regression model


```quantile-regression-inference.ipynb``` - contains training and inference part with Quantile Regression model

```train-efficientnet.ipynb``` - contains training part with Quantile Regression model


## Acknowledgements
 My solution is based on the following notebooks and discussion, thanks to Kagglers!

- Linear Decay
[https://www.kaggle.com/miklgr500/linear-decay-based-on-resnet-cnn](https://www.kaggle.com/miklgr500/linear-decay-based-on-resnet-cnn)


- Quantile Regression
[https://www.kaggle.com/ulrich07/osic-multiple-quantile-regression-starter](https://www.kaggle.com/ulrich07/osic-multiple-quantile-regression-starter)

- EfficientNets + Quantile Regression
[https://www.kaggle.com/khoongweihao/efficientnets-quantile-regression-inference](https://www.kaggle.com/khoongweihao/efficientnets-quantile-regression-inference)

- Patients Clustering
[https://www.kaggle.com/c/osic-pulmonary-fibrosis-progression/discussion/168610](https://www.kaggle.com/c/osic-pulmonary-fibrosis-progression/discussion/168610)
