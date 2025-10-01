# PrognosAI: AI-Powered Predictive Maintenance with Time-Series Sensor Data  

## Project Overview  

**PrognosAI** is an AI-based predictive maintenance system designed to estimate the **Remaining Useful Life (RUL)** of industrial machines using multivariate time-series sensor data. The system is prototyped on the **NASA CMAPSS dataset** and can generalize to similar equipment such as turbines, pumps, and motors. By leveraging deep learning models like **LSTM**, PrognosAI helps reduce unexpected downtime, optimize asset usage, and support timely maintenance decisions.  

---

## Workflow  

1. **Data Ingestion**  
   - Load and clean the CMAPSS sensor dataset, which contains cycle-wise engine measurements.  

2. **Feature Engineering**  
   - Generate rolling window sequences for time-series analysis.  
   - Compute RUL targets for each engine.  

3. **Model Training**  
   - Train deep learning models (LSTM or GRU) to predict RUL from sensor sequences.  

4. **Model Evaluation**  
   - Evaluate prediction performance using **RMSE**.  
   - Compare predicted RUL vs actual RUL.  

5. **Alert Thresholding**  
   - Set thresholds to trigger maintenance alerts based on predicted RUL.  

6. **Visualization & Dashboard**  
   - Display RUL trends, prediction insights, and alert zones via interactive dashboards.  

---

## Architecture  

![](Aspose.Words.072c5ff2-ae53-4611-8571-688eb115c598.001.png)  

---

## Technology Stack  

- **Python** – Core programming language  
- **Pandas, NumPy** – Data manipulation  
- **Matplotlib, Seaborn** – Data visualization  
- **TensorFlow / Keras** – LSTM model training  
- **Scikit-learn** – Preprocessing and metrics  
- **Streamlit / Flask** – Dashboard or API interface  
- **Docker** – Optional deployment  
- **NASA CMAPSS Dataset** – Source of time-series sensor data  

---

## Milestones  

### 1. Data Preparation & Feature Engineering  
- **Goal:** Load, clean, and prepare CMAPSS data for training.  
- **Deliverables:**  
  - Cleaned and preprocessed dataset  
  - Scripts for data loading and preprocessing  
  - Rolling window sequences  
  - Computed RUL targets  
- **Evaluation:**  
  - Data integrity and missing values check  
  - Correctness of rolling window sequences  
  - Accuracy of RUL target calculations  
  - Proper documentation of preprocessing steps  

### 2. Model Development & Training  
- **Goal:** Implement and train an LSTM/GRU model for RUL prediction.  
- **Deliverables:**  
  - Model architecture implemented  
  - Trained weights and checkpoints  
  - Training & validation loss curves  
  - Scripts for model definition, training, and saving  
- **Evaluation:**  
  - Training convergence (loss reduction)  
  - Initial validation performance (predicted vs actual RUL)  
  - Correct model implementation  

### 3. Model Evaluation & Performance  
- **Goal:** Assess model accuracy and predictive power.  
- **Deliverables:**  
  - RMSE scores on test dataset  
  - Predicted vs actual RUL plots  
  - Bias/error analysis  
  - Evaluation report  
- **Evaluation:**  
  - RMSE within acceptable threshold  
  - Visual consistency in plots  
  - Identify model limitations  

### 4. Risk Thresholding & Alerts  
- **Goal:** Convert RUL predictions into actionable maintenance alerts.  
- **Deliverables:**  
  - Defined alert thresholds (warning, critical)  
  - Alert trigger logic  
  - Example alert scenarios  
- **Evaluation:**  
  - Effectiveness in early failure detection  
  - Accuracy of triggered alerts  
  - Practical applicability  

### 5. Visualization & Dashboard  
- **Goal:** Build interactive dashboards for monitoring RUL and alerts.  
- **Deliverables:**  
  - Charts showing RUL trends  
  - Dashboard for live RUL predictions and alerts  
  - Streamlit/Flask-based interface  
- **Evaluation:**  
  - Clarity and insightfulness of visualizations  
  - Dashboard usability and responsiveness  
  - Ability to communicate asset health and risk clearly  
