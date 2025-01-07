ABSTRACT

Introduction: Cardiovascular disease (CVD) has been the leading cause of death in Malaysia since the
1980s, with myocardial infarction (MI) and stroke being significant contributors.

Research gao:  Conventional risk scores like the Framingham Risk Score (FRS) are widely used for
predicting CVD, but their 10-year risk assessment often lacks population specificity,
particularly for the Malaysian demographic, and fails to capture short- to medium-term
risks. This limitation may lead to missed opportunities for timely interventions, especially
given the rapid progression of CVD in some patients. 

Hypothesis: In response to this gap, this study developed a 3-year CVD risk prediction and event classification model tailored to
Malaysia's diverse demographic landscape, addressing the need for a more accurate and
timely risk assessment tool. 

Data: Utilizing data from the REDISCOVER registry, which included 12,617 participants from eight Malaysian states, two distinct models were
constructed. The first model predicted the occurrence of CVD events (CVD vs. No CVD),
while the second classified specific CVD events, particularly MI and stroke. 

Methodology: Data preprocessing involved median imputation for missing values and resampling to balance
the classes. Feature selection was performed using Recursive Feature Elimination(RFE),
SHAP-based selection, backward elimination as well as correlation analysis for noise
reduction. The models trained included Random Forest (RF), XGBoost, Decision Trees
(DT), Gradient Boosting Machine (GBM), Support Vector Classifier (SVC), and K-
Nearest Neighbors (KNN). Ensemble models were also created using a stacking
approach. Model performance was evaluated based on accuracy, area under the curve
(AUC), classification reports, and confusion matrices. 

Results: In the first model, the RF model using the top 26 selected features achieved an AUC of 0.8587, outperforming the
Framingham Risk Score (FRS), which had an AUC of 0.8343. The RF model also
outperformed FRS in terms of the Net Reclassification Index (NRI), showing a 19%
improvement at a 5% cut-off point. While the calibration of the RF model was similar to
FRS, the Brier score was slightly higher for the RF model (0.01176) compared to FRS
(0.01173), and the log loss was marginally greater (0.05720 for RF vs. 0.0568 for FRS).
        The second model, aimed at classifying specific CVD events, utilized an RF ensemble
approach with the top 14 selected features. The model demonstrated strong predictive
performance, achieving an AUC of 0.944, indicating excellent discrimination between
the different CVD events. Despite the limited sample size, the confusion matrix
demonstrated good classification performance, correctly classifying most cases of MI and
stroke. This outcome suggests that even with a relatively small number of features, the
model effectively captured the critical patterns associated with these specific CVD events.

Conclusion: This study demonstrates that the developed models offer robust and accurate 3-year
predictions specifically tailored to the Malaysian population. The first model provides a
reliable approach to predicting CVD risk within a 3-year timeframe, while the second
model effectively classifies specific cardiovascular events over the same period. The
results indicate significant improvements over traditional methods, underscoring the
potential for these models to enhance CVD risk assessment and intervention in Malaysia.
