# 🩺 Heart Disease Predictor

![Model](https://img.shields.io/badge/Model-Random%20Forest-blue) ![Python](https://img.shields.io/badge/Python-3.12-green) ![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 Overview
A Python-based ML project to predict heart disease using the UCI Heart Disease dataset. Built in Google Colab, it uses Random Forest to predict disease severity (0: No, 1-4: Yes). Features preprocessing, EDA, model training, and user predictions.

## 🚀 Features
- 🧹 Preprocesses data: missing values, encoding, scaling.
- 📈 EDA: Visualizes distributions, correlations, feature importance.
- 🌳 Random Forest model (~85-90% accuracy).
- 💾 Saves model/scaler with `joblib`.
- 📥 User predictions via CSV upload.
- 🔑 Kaggle API for dataset download.

## 🛠️ Technologies
- Python 3.12 🐍
- Pandas, NumPy 📊
- Scikit-learn 🤖
- Matplotlib, Seaborn 🎨
- Joblib 📦
- Kaggle API 🔐

## ⚙️ Installation
1. Clone repo:
   ```bash
   git clone https://github.com/your-username/Heart_Disease_Predictor.git
   cd Heart_Disease_Predictor
   ```
2. Set up Kaggle API:
   - Download `kaggle.json` from Kaggle.
   - Place in `~/.kaggle/` (Linux/Mac) or `C:\Users\YourUsername\.kaggle\` (Windows).
   - Run: `chmod 600 ~/.kaggle/kaggle.json`.
3. Install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   pip install pandas numpy matplotlib seaborn scikit-learn joblib kaggle
   ```

## ▶️ Usage
- **Colab**: Upload `Disease_Predictor.ipynb`, run cells, upload `kaggle.json`.
- **Local**: Run `jupyter notebook Disease_Predictor.ipynb`.
- **Predict**: Use `Heart_user_template.csv`, fill data, upload for predictions (0 = No disease, 1+ = Disease).

Example Input:
```
age,trestbps,chol,fbs,restecg,thalch,exang,oldpeak,slope,ca,thal,sex_Female,sex_Male,cp_asymptomatic,cp_atypical angina,cp_non-anginal,cp_typical angina
58,130,220,1,normal,150,FALSE,1.4,flat,0,fixed defect,0,1,0,0,0,1
```

## 📊 Workflow
- Load dataset, preprocess data.
- Train Random Forest model.
- Evaluate accuracy, confusion matrix.
- Save model/scaler.
- Predict with user-uploaded CSV.

## 🔮 Future Improvements
- Streamlit/Flask app 🌐
- Add XGBoost, neural networks 🧠
- Cloud deployment (AWS/GCP) ☁️

## 👨‍💻 Author
- [Your Name]
- [Your LinkedIn]
- [Your Email]

## 📄 License
MIT License

## 🙏 Acknowledgments
- Dataset: [UCI Heart Disease](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)
- Built with ❤️ in Google Colab