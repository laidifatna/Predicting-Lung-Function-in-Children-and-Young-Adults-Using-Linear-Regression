# Predicting Lung Function in Children and Young Adults Using Linear Regression

## Objective

Predict forced expiratory volume (FEV) using age, height, sex, and smoking status.

**Research question:** How accurately can basic physical measurements predict lung function in children and young adult?

## Dataset

The dataset is publicly available through the Journal of Statistics Education. It contains 654 observations of children and young adults aged 3–19 from East Boston, collected during the 1970s.

- [Download the data](https://jse.amstat.org/datasets/fev.dat.txt)
- [Dataset documentation](https://jse.amstat.org/datasets/fev.txt)
- [Published analysis](https://jse.amstat.org/v13n2/datasets.kahn.html)

This project uses existing public research data (no new patient data are collected).
## Variables

- **fev:** Volume exhaled of a forced breath, in litres (Target variable)
- **age:** Age in years (Predictor)
- **height:** Height in inches (Predictor)
- **sex:** 0= female, 1 = male (Predictor)
- **smoke:** 0 = non-smoker, 1 = smoker (Predictor)

## Methodology

1. Inspect the dataset and check missing values and unusual measurements.
2. Explore relationships using scatterplots and Pearson correlations.
3. Divide the data into training and test sets.
5. Fit multiple linear regression using all four predictors.
6. Compare multiple linear regression model with a baseline model.
7. Use cross-validation within the training set to assess consistency.
8. Evaluate the selected model.

## Evaluation Metrics

- **MAE:** average absolute prediction error in litres.
- **RMSE:** prediction error in litres, emphasizing larger mistakes.
- **R²:** performance relative to predicting the evaluation-set mean.
- Compare predicted FEV with actual test values.
- Residual Plot to check prediction errors.
- Q-Q plot to check for normality.
