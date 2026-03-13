# ⚡ Electricity Load Forecasting — Final Project
Predicting short‑term electricity demand using exploratory analysis, classical ML models, deep learning architectures, and interpretability techniques.  
This project was developed as part of a final learning module in time‑series forecasting & machine learning.  

---

## 📂 Repository Structure

Main notebooks in the repository root:

- **10-EDA_weather.ipynb**  
  Initial exploratory data analysis for weather & load variables.

- **11-EDA_weather_3_splits_for_XGB.ipynb**  
  Extended EDA including preparation of train/validation/test splits for XGBoost models.

- **30-XGBRegressor_weather.ipynb**  
  XGBoost regression forecasting experiments including parameter tuning, model evaluation and feature importances.

- **40-DeepLearning_weather.ipynb**  
  Deep learning experiments (LSTM/GRU architectures) for multivariate electricity‑load forecasting.

- **41-TFT-interpretation.ipynb**  
 Training and interpretation of a Temporal Fusion Transformer (TFT) model including variable importance and attention analysis.

---

## 🎯 Project Goals

- Understand weather‑driven electricity load patterns through exploratory analysis.  
- Build machine learning models (XGBoost, tree‑based regressors).  
- Develop deep learning forecasting architectures (LSTM/GRU/Seq2Seq).  
- Train and interpret a Temporal Fusion Transformer (TFT).  
- Compare the performance of multiple forecasting methodologies.  

---

## 🧠 Technologies Used

### Core Stack
- **Python 3.12+**
- pandas, numpy  
- matplotlib, seaborn, plotly  
- scikit‑learn  
- XGBoost  
- TensorFlow / Keras  
- PyTorch + PyTorch Lightning  
- PyTorch Forecasting (for TFT)

---
## 🚀 Getting Started

### 1️⃣ Clone the repository

- git clone https://github.com/MariusGoeren/final-project_electricity-load-forecast.git
- cd final-project_electricity-load-forecast

---
### 2️⃣ Create a Python environment
- Using venv for EDA part:
  - & "C:\Users\**your-name**\AppData\Local\Programs\Python\Python314\python.exe" -m venv venv-eda
    - if **python version 14** is not available -> install first
  - .\venv-eda\Scripts\activate
  - python.exe -m pip install --upgrade pip

- Using venv for ML part:
  - & "C:\Users\**your-name**\AppData\Local\Programs\Python\Python312\python.exe" -m venv venv-eda
    - if **python version 12** is not available -> install first
  - .\venv-\Scripts\activate
  - python.exe -m pip install --upgrade pip

- Using venv for ML part:
  - python3.12 -m venv .venv
  - source .venv/bin/activate       # Linux/Mac
  - .venv\Scripts\activate          # Windows

---
### 3️⃣ Install requirements
If a requirements.txt exists:
- pip install -r requirements.txt

If not, install the needed dependencies manually:
#### 📦 Base packages
- pip install numpy pandas matplotlib seaborn plotly scikit-learn

#### 🌲 XGBoost
- pip install xgboost

#### 🤖 Deep Learning (TensorFlow)
- pip install tensorflowWeitere Zeilen anzeigen

#### 🔥 TFT + PyTorch Forecasting
- CPU-based installation:
  - pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
  - pip install pytorch-lightning
  - pip install pytorch-forecasting

- For GPU/CUDA, install PyTorch according to NVIDIA compatibility (optional).

---
## 📊 Running the Notebooks
Recommended order:

### 1️⃣ Exploratory Data Analysis

- 10-EDA_weather.ipynb
- 11-EDA_weather_3_splits_for_XGB.ipynb

### 2️⃣ Machine Learning Models

- 30-XGBRegressor_weather.ipynb

### 3️⃣ Deep Learning Models

- 40-DeepLearning_weather.ipynb

### 4️⃣ Interpretability

- 41-TFT-interpretation.ipynb

---
## 📈 Included Analyses
### 🔍 EDA   ????????????????????????????????????????????
- Missing value inspection
- Distribution analysis
- Weather correlations
- Daily, weekly, yearly seasonality patterns
- Moving averages, smoothing, trend detection

### 🌲 XGBoost   ????????????????????????????????????????????
- Dataset splitting strategy
- Hyperparameter tuning
- Feature importance evaluation
- Prediction vs. actual comparison

### 🤖 Deep Learning   ????????????????????????????????????????????
- Timeseries windowing
- LSTM/GRU forecasting architectures
- Model training, validation curves
- Multi‑step prediction evaluation

### 🔮 Temporal Fusion Transformer (TFT)   ????????????????????????????????????????????
- Variable selection network
- Attention mechanisms
- Time‑step relevance visualizations
- Global & local interpretability

---
## 📝 Future Improvements   ????????????????????????????????????????????
- Add ARIMA/Prophet benchmarks for classical comparison
- Incorporate additional weather features and lags
- Hyperparameter optimization with Optuna
- Extend TFT to multi‑regional forecasting
- Add probabilistic forecasting metrics

---
# 📬 Author
Marius Gören
- Machine Learning & M&E Automation Specialist
