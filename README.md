# Fish Weight Estimation using Machine Learning Models

This study aims to estimate the weight of the fish from their measurements through machine learning models. This exercise will show interpretations as well as rationale regarding which machine learning model was used for optimal results.

Interpretation:

1. Species_Pike has outliers ['Weight']
2. There is a positive correlation between all of the numeric features and the target ['Weight']
3. We have strong correlations. Multicolinearity could be a concern if using a linear model.
4. The data is fairly right skewed. Again something to be aware of if using a linear model (a transformation might work here).
5. The data is fairly right skewed.
6. Based on the above analysis I will not proceed with a linear model.

**Baseline Model Report**

*   Baseline Training RMSE: 310.95221969579575

*   Baseline Testing RMSE: 341.5013713155734

*   Baseline Training R2: 0.0

*   Baseline Testing R2: -0.03090919367721323

**KNN Model Report**

*   KNN Training RMSE: 54.32274843149043

*   KNN Testing RMSE: 80.32340347183468

*   KNN Training R2: 0.9694805890705459

*   KNN Testing R2: 0.9429678540483883

**Random Forest Model Report**

*   Random Forest Training RMSE: 22.127351161568132

*   Random Forest Testing RMSE: 55.025973799092924

*   Random Forest Training R2: 0.9949362584240106

*   Random Forest Testing R2: 0.9732347698069479

Conclusion:

The Random Forest model is the model I would choose to put into production. This is due to the lowest testing RMSE at 53.79 and the highest testing R2 at 97%.

