# wine_quality_analysis
The project includes a predictive system where you can input wine chemical properties and receive a classification output:  Good Quality Wine  Bad Quality Wine
---
## Project Overview
This project analyzes the **Red Wine Quality Dataset** and builds a **Machine Learning classification model** to predict whether a wine is of **good quality** based on its physicochemical properties.  

The project includes:
- Data loading and inspection
- Exploratory Data Analysis (EDA)
- Data visualization
- Correlation analysis
- Data preprocessing
- Label binarization
- Model training using **Random Forest Classifier**
- Model evaluation
- A predictive system for new wine samples

---

## Objective
The goal of this project is to identify how different chemical properties of wine influence quality and to develop a predictive model that classifies wine quality effectively.

---

## Dataset Information
The dataset used in this project is the **Red Wine Quality Dataset**, which contains various physicochemical features of red wine samples, such as:

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality (target variable)

---

## Project Workflow

### 1. Data Collection
- Loaded the dataset into a Pandas DataFrame
- Checked the shape of the dataset
- Displayed the first few rows
- Verified missing values

### 2. Exploratory Data Analysis (EDA)
Performed statistical analysis and visualizations to understand the dataset:
- Distribution of wine quality scores
- Volatile acidity vs quality
- Citric acid vs quality
- Additional feature-based visual analysis

### 3. Correlation Analysis
- Generated a correlation matrix
- Built a heatmap to identify positive and negative correlations between variables

### 4. Data Preprocessing
- Separated features (`X`) and target (`quality`)
- Prepared the data for model training

### 5. Label Binarization
Converted the target variable into binary classes:
- **1** → Good quality wine (`quality >= 7`)
- **0** → Not good quality wine (`quality < 7`)

### 6. Train-Test Split
- Split the dataset into training and testing sets
- Used an **80/20 split** for model evaluation

### 7. Model Training
Trained a **Random Forest Classifier** on the processed dataset.

### 8. Model Evaluation
- Evaluated model performance using **Accuracy Score**
- Achieved approximately **91.67% accuracy** *(update if needed based on your final output)*

### 9. Predictive System
Built a simple prediction pipeline to classify a new wine sample as:
- **Good Quality Wine**
- **Bad Quality Wine**

---

## Technologies Used
- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## Machine Learning Model
- **Algorithm:** Random Forest Classifier
- **Evaluation Metric:** Accuracy Score

---

## Key Insights
- Certain features such as **alcohol**, **volatile acidity**, and **sulphates** show meaningful relationships with wine quality.
- Correlation heatmaps help identify which variables may have stronger influence on the target.
- Random Forest performed well for this binary classification problem and provided strong predictive accuracy.

---

## Project Structure
```bash
wine-quality-analysis/
│── wine_quality_analysis.ipynb
│── README.md
│── winequality-red.csv
