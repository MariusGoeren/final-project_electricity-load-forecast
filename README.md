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
  XGBoost regression forecasting experiments including parameter tuning and model evaluation.

- **40-DeepLearning_weather.ipynb**  
  Training and interpretation of a Temporal Fusion Transformer (TFT) model including variable importance and attention analysis.

- **41-TFT-interpretation.ipynb**  
  Create some plots to interpret the results of the TFT model predictions.

---

## 🎯 Project Goals

- Understand weather‑driven electricity load patterns through exploratory analysis.  
- Build machine learning models (XGBoost).  
- Develop deep learning forecasting architectures (Temporal Fusion Transformer).  
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

### 2️⃣ Create a Python environment
- Using venv for EDA part:
  - & "C:\Users\**your-name**\AppData\Local\Programs\Python\Python314\python.exe" -m venv venv-eda
    - if **python version 14** is not available -> install first
  - .\venv-eda\Scripts\activate
  - python.exe -m pip install --upgrade pip

- Using venv for ML part (XGB/TFT):
  - & "C:\Users\**your-name**\AppData\Local\Programs\Python\Python312\python.exe" -m venv venv-eda
    - if **python version 12** is not available -> install first
  - .\venv-ml\Scripts\activate
  - python.exe -m pip install --upgrade pip

- Using venv for TFT interpretation part:
  - & "C:\Users\**your-name**\AppData\Local\Programs\Python\Python312\python.exe" -m venv venv-eda
    - if **python version 12** is not available -> install first
  - .\venv-tft-plots\Scripts\activate
  - python.exe -m pip install --upgrade pip

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
- using **venv-eda**
- 10-EDA_weather.ipynb
- 11-EDA_weather_3_splits_for_XGB.ipynb

### 2️⃣ Machine Learning Models
- using **venv-ml**
- 30-XGBRegressor_weather.ipynb

### 3️⃣ Deep Learning Models
- using **venv-ml**
- 40-DeepLearning_weather.ipynb

### 4️⃣ Interpretability
- using **venv-tft-plots**
- 41-TFT-interpretation.ipynb

---
## 📈 Included Analyses
### 🔍 EDA   
- Missing values inspection
- Distribution analysis
- Weather correlations
- Daily, weekly, yearly seasonality patterns
- Moving averages, smoothing, trend detection
- Cyclic encoding

### 🌲 XGBoost
- Dataset splitting strategy
- Hyperparameter tuning
- Feature importance evaluation
- Prediction vs. actual comparison

### 🔮 Temporal Fusion Transformer (TFT)
- Variable selection network
- Attention mechanisms
- Time‑step relevance visualizations
- Global & local interpretability

---
## 📝 Future Improvements
- Connecting the Influx DB directly to the model
- Automatically making continuous predictions
- Incorporate additional weather features and lags
- TFT hyperparameter optimization with Optuna
- Add production plans to make better predictions

---
# 📬 Author
Marius Gören
- Machine Learning & M&E Automation Specialist
