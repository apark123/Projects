# 🐧 Penguin Species Prediction

A fun and practical machine learning project that predicts **penguin species** based on physical traits like their bill (culmen) size and the island they live on — using the famous **Palmer Penguins dataset**.

---

## 💡 What This Project Is About
This notebook walks through the full machine learning workflow — from exploring the data to building and evaluating predictive models.  
The goal is to figure out **which features best distinguish penguin species**, and how accurately we can classify them using simple models.

I chose this dataset because it’s cleaner and more interesting than the classic Iris dataset — it’s real-world, slightly messy, and involves adorable penguins.

---

## 📥 Data Overview
We use `palmer_penguins.csv`, which includes:
- **Quantitative features:** Culmen Length, Culmen Depth, Flipper Length, Body Mass  
- **Qualitative features:** Island, Sex  
- **Target variable:** Species  

The data is loaded and visualized using **pandas**, **matplotlib**, and **seaborn** to understand patterns and relationships.

---

## 🔍 What We Found
After exploring the dataset:
- **Culmen Length** and **Culmen Depth** stood out as the most distinct numerical features across species.  
- **Island** turned out to be a powerful categorical predictor — since certain penguin species only live on specific islands.  

We confirmed this visually with histograms and scatterplots, showing clear separation between species when plotting these features.

---

## ⚙️ Preprocessing
I wrote a simple `prep_data()` function that:
- Converts categorical values (like Island) into numeric codes  
- Drops missing values  
- Splits the data into predictors (`X`) and target (`y`)

Then, the dataset is split into training (80%) and testing (20%) sets.

---

## 🤖 Modeling
I tested three supervised learning models from **scikit-learn**:

1. **Logistic Regression** — fast and interpretable; reached ~97% accuracy.  
2. **Decision Tree** — learned flexible rules and hit ~99% accuracy.  
3. **Random Forest** — combined multiple trees for ~99% accuracy and higher robustness.

All models were tuned using **cross-validation** to find the best parameters, such as `C` for Logistic Regression and `max_depth` for tree models.

---

## 📈 Results & Insights
Every model performed extremely well (95–99% accuracy range).  
However:
- **Decision Trees** worked best overall — simple, interpretable, and accurate.  
- **Random Forests** performed similarly but required more computation.  
- **Logistic Regression** was slightly less accurate but very efficient.  

The main takeaway: **Island**, **Culmen Length**, and **Culmen Depth** are enough to predict penguin species with nearly perfect accuracy.

---

## 💭 Reflections
This project was a fun reminder of how much insight you can get from visualization and careful feature selection — even before touching complex models.

If the “**Penguin Apocalypse**” ever comes, at least this model will know which species we’re dealing with 🧊🐧.

---

## 🧠 Tools & Libraries
- Python 3  
- pandas, NumPy  
- matplotlib, seaborn  
- scikit-learn  

---

## ▶️ How to Run
1. Clone or download the repo.  
2. Place `palmer_penguins.csv` in the same directory.  
3. Open `PenguinSpeciesPrediction.ipynb` and run the cells in order.  

---

## 👤 Author
**Andrew Park**  
Data Analyst | Data Enthusiast  
📧 andrewpark470@gmail.com  
📞 818-522-1277
