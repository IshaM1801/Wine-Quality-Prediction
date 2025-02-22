# 🍷 Wine Quality Prediction

## 📌 Project Description
This project uses machine learning to predict the quality of red wine based on its chemical properties. The dataset used is `winequality-red.csv`, which contains various physicochemical attributes of wine samples. A **Random Forest Classifier** is trained to classify wines as either **good quality** (1) or **bad quality** (0) based on a threshold.

## 📂 Dataset Information
- **Source:** UCI Machine Learning Repository
- **Rows:** 1599
- **Columns:** 12 (including the target column "quality")
- **Features:**
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

## 🛠️ Dependencies
Make sure you have the following libraries installed before running the project:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## 🚀 Implementation Steps
1. **Load the Dataset** 📥
2. **Data Exploration & Visualization** 📊
3. **Data Preprocessing** 🧹
4. **Train-Test Split** 📑
5. **Train Random Forest Classifier** 🌲
6. **Evaluate Model Performance** ✅
7. **Build a Prediction System** 🔮

## 🔍 Data Analysis
- **Correlation Heatmap**: Displays the relationships between different features.
- **Bar Charts**: Show how acidity and citric acid influence wine quality.

## 🎯 Model Performance
- **Algorithm Used:** Random Forest Classifier 🌲
- **Accuracy on Test Data:** 93.1% 🎯

## 🔮 Predictive System
To make a prediction, provide wine sample data:
```python
input_data = (7.4,0.7,0.0,1.9,0.076,11.0,34.0,0.9978,3.51,0.56,9.4)
input_data_as_array = np.asarray(input_data)
input_data_reshaped = input_data_as_array.reshape(1,-1)
output = model.predict(input_data_reshaped)
print('Good Quality Wine' if output == 1 else 'Bad Quality Wine')
```

## 📜 License
This project is open-source and free to use under the MIT License.

## 📬 Contact
For any queries, feel free to reach out! 📩

Happy Coding! 🚀

