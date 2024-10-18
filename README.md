# Erling Haaland Goal Scoring Probability Analysis

## Overview
This project analyzes Erling Haaland's goal-scoring probability based on various factors when he takes a shot. By examining his historical shot data, we aim to build a predictive model that estimates the likelihood of scoring based on shot conditions.

## Data
The dataset includes information about each shot taken by Erling Haaland, featuring attributes such as:

- `minute`: The minute of the match when the shot was taken
- `result`: Outcome of the shot (e.g., goal, missed, saved)
- `X` and `Y`: Coordinates of the shot
- `xG`: Expected goals metric for each shot
- `situation`: Context of the shot (e.g., open play, penalty)
- Additional match-related information

## Methodology
1. **Data Preprocessing**: Cleaned the dataset by handling missing values, encoding categorical variables, and removing unnecessary columns.
2. **Exploratory Data Analysis (EDA)**: Conducted EDA to visualize and understand the distribution of goals scored under different conditions.
3. **Feature Engineering**: Developed features relevant to shot conditions while omitting the defensive statistics of the opposition.
4. **Model Selection**: Employed a Random Forest Classifier to predict whether a shot results in a goal.
5. **Model Evaluation**: Assessed the model's performance using accuracy, precision, recall, and F1-score metrics.

## Results
- **Accuracy**: 0.82
- **Classification Report**:
  - Precision for no goal: 0.85
  - Recall for no goal: 0.93
  - F1-score for no goal: 0.89
  - Precision for goal: 0.71
  - Recall for goal: 0.50
  - F1-score for goal: 0.59

## Conclusion
The model achieves an accuracy of 82% in predicting Erling Haaland's goal-scoring probability based on shot conditions. This analysis highlights the importance of specific situational factors when evaluating scoring likelihood.

## Acknowledgments
- (https://understat.com/) for providing the dataset.
