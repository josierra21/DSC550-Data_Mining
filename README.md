# DSC550-Data_Mining
# Credit Card Fraud Detection with Machine Learning

This project applies machine learning techniques to detect fraudulent credit card transactions using a publicly available dataset. It explores the challenges of working with highly imbalanced data and compares different classification models to identify the most effective approach.

## Dataset

- **Source**: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Description**: Contains 284,807 transactions, each with 28 anonymized features (from PCA), transaction time, amount, and a binary `Class` label indicating fraud (1) or not (0).

## Project Steps

1. **Exploratory Data Analysis (EDA)**  
   - Visualized class imbalance and feature distributions.  
   - Identified patterns and potential outliers, such as extreme values in features like V2.

2. **Data Preparation**  
   - Original dataset was split into training, testing, and validation sets.  
   - A balanced dataset was also created by undersampling the majority class to allow fair model training.

3. **Modeling**  
   Multiple models were trained and evaluated on both the imbalanced and balanced datasets:
   - Logistic Regression  
   - Shallow Neural Networks   
   - Random Forest  
   - Gradient Boosting Classifier  
   - Linear Support Vector Classifier 

4. **Evaluation**  
   - Models were evaluated using accuracy, precision, recall, and F1-score on the validation and test sets.  
   - Logistic Regression on the balanced dataset delivered the most consistent performance with:  
     - 95% accuracy  
     - 96% precision (fraud class)  
     - 93% recall (fraud class)

## Final Model

- **Selected Model**: Logistic Regression (trained on the balanced dataset)  
- **Reason**: Simple, interpretable, and consistently high performance across key metrics.

## Future Improvements

- Evaluate models on real-world imbalanced data.  
- Explore synthetic sampling, cost-sensitive training, or ensemble strategies.  
- Integrate into an automated fraud detection pipeline for real-time monitoring and decision-making.
