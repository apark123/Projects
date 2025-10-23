# Penguin Species Prediction

A practical machine learning project that predicts penguin species based on physical traits like culmen (bill) size and the island they live on — using the Palmer Penguins dataset.

---

## What This Project Is About
This notebook walks through the full machine learning workflow — from exploring the data to building and evaluating predictive models.  
The goal is to determine which features best distinguish penguin species, and how accurately we can classify them using simple models.

This dataset was chosen because it’s cleaner and more realistic than the classic Iris dataset — it reflects real-world data while still being easy to visualize and interpret.

---

## Data Overview
The project uses `palmer_penguins.csv`, which includes:

- Quantitative features: Culmen Length, Culmen Depth, Flipper Length, Body Mass  
- Qualitative features: Island, Sex  
- Target variable: Species  

The data was analyzed using `pandas`, `matplotlib`, and `seaborn` to understand trends and relationships.

---

## Key Findings
After exploring the dataset:
- Culmen Length and Culmen Depth were the most distinct numerical features between species.  
- Island was the strongest categorical predictor, as some species are found only on specific islands.  

Visualizations like histograms and scatterplots confirmed these relationships clearly.

---

## Data Preparation
A helper function `prep_data()` was created to:
- Encode categorical values (such as Island) into numerical codes  
- Drop missing values  
- Split the data into predictor (`X`) and target (`y`) variables  

The dataset was then divided into:
- 80% training data  
- 20% testing data  

---

## Modeling
Three supervised learning models from `scikit-learn` were tested:

1. **Logistic Regression** – fast, interpretable, and achieved around 97% accuracy  
2. **Decision Tree** – flexible, easy to understand, and reached about 99% accuracy  
3. **Random Forest** – ensemble of trees with similar 99% accuracy and more stability  

Cross-validation was used to tune hyperparameters like `C` for Logistic Regression and `max_depth` for tree models.

---

## Results and Insights
All models performed extremely well, achieving accuracies between 95% and 99%.  

- Decision Trees offered the best balance of performance and interpretability.  
- Random Forests performed equally well but required more computation.  
- Logistic Regression was slightly less accurate but efficient and simple.  

In short, Island, Culmen Length, and Culmen Depth were sufficient to classify penguin species with near-perfect accuracy.

---

## Reflection
This project highlights how effective basic feature selection and visualization can be before moving to complex models.  
Even with a small dataset, careful exploration and model testing can produce highly accurate results.

---

## Tools and Libraries
- Python 3  
- pandas, NumPy  
- matplotlib, seaborn  
- scikit-learn  

---
---

## Author
**Andrew Park**  
Data Analyst
Email: andrewpark470@gmail.com  
Phone: 818-522-1277
