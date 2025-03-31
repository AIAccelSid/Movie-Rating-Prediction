# 📌 Netflix Movie Rating Prediction

## 🎬 Project Overview
This project predicts movie ratings based on historical data using **machine learning regression techniques**. It leverages **Random Forest Regressor** and **Linear Regression** models to estimate how a user might rate a given movie.

## 🚀 Features
✅ **Efficient Data Preprocessing**: Optimized memory usage with proper data types.
✅ **Feature Engineering**: Extracts meaningful features such as movie age, name length, and user average rating.
✅ **Machine Learning Models**: Implements both **Linear Regression** and **Random Forest Regressor**.
✅ **Model Evaluation**: Calculates **MSE, RMSE, R², MAE, and Accuracy** for performance assessment.
✅ **Single Prediction Support**: Accepts a single **User_ID & Movie_ID** input and predicts the rating.
✅ **Heatmap Visualization**: Generates a heatmap of feature correlations.
✅ **Model Saving & Loading**: Saves trained models for future use.

---

## 📂 Dataset
The project utilizes two datasets:
1. **Netflix_Dataset_Rating.csv** → Contains User_ID, Movie_ID, and Rating.
2. **Netflix_Dataset_Movie.csv** → Contains Movie_ID, Year, and Movie Name.

---

## 📌 Setup & Installation
1️⃣ Clone the repository:
```bash
git clone https://github.com/yourusername/netflix-rating-prediction.git
cd netflix-rating-prediction
```

2️⃣ Install required dependencies:
```bash
pip install -r requirements.txt
```

3️⃣ Run the training script:
```bash
python train_model.py
```

4️⃣ Predict ratings for a single user & movie:
```bash
python predict_single.py
```

---

## 🎯 Usage
### **Training the Model**
```python
python train_model.py
```
This script:
✅ Loads data and preprocesses it.
✅ Trains **Linear Regression & Random Forest** models.
✅ Saves models & scaler for future predictions.
✅ Evaluates models using MSE, RMSE, R², MAE.

### **Predicting a Single Rating**
```python
python predict_single.py
```
You can change `User_ID` and `Movie_ID` inside `predict_single.py` before running it.

Example Output:
```
🎬 Predicted Rating for User 712664 and Movie 3: 3.58/5
```

---

## 📊 Model Evaluation Results
| Model | MSE | RMSE | R² | MAE | Accuracy |
|--------|-------|------|------|------|---------|
| Linear Regression | 1.1182 | 1.0575 | 0.0103 | 0.8826 | 33.73% |
| Random Forest | 1.0614 | 1.0302 | 0.0606 | 0.8454 | 35.56% |

---

## 📈 Heatmap Visualization
The project generates a **heatmap** to analyze feature correlations:
```python
import seaborn as sns
import matplotlib.pyplot as plt
plt.figure(figsize=(10,6))
sns.heatmap(data.corr(), annot=True, cmap='coolwarm', fmt='.2f')
plt.title('Feature Correlation Heatmap')
plt.show()
```

---

## 📜 License
This project is **open-source** under the MIT License. Feel free to use and improve it!

---

## 🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit pull requests.

---

## 📧 Contact
📩 **Your Name** – [your_email@example.com](mailto:your_email@example.com)
🌍 GitHub: [yourusername](https://github.com/yourusername)

---

